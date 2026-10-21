---
title: Digital Theory and Experimentation Using Integrated Circuits (raw source)
source_url: /run/media/yutae/Data/Digital_Theory_and_Experimentation.pdf
ingested: 2026-10-22
sha256: 5352c223ae41834dd0d422e343b6f125981e360981fc9339e69bce983457211b
---
# Digital Theory and Experimentation Using Integrated Circuits (raw source)

> **Note:** PDF 내장 텍스트 레이어 사용 (OCR 없음). `pdftotext -layout` 추출. PDF는 로컬 참조용 (`raw/books/*.pdf` git-ignored).

## Book metadata
- **제목/원서:** Digital_Theory_and_Experimentation.pdf
- **저자:** Morris E. Levine (College of Staten Island, City University of New York), Revised and Enlarged
- **페이지 수:** 297 (pdfinfo Pages)
- **범위:** 297p, 20개 실험(Digital Theory & Experimentation) — XOR·풀-가산기·플립플롭·2진 카운터·시프트 레지스터·슈머트 트리거·IC 타이머(74122/74121/555)·인코더/디코더·RAM, 연산기·D/A·A/D·CMOS·다진동기·원샷
- **특기:** 실험 중심 — 실험당 '이론+절차+질문' 구조

## OCR/추출 주의
- 추출: pdftotext (양호)

## Text (all 297 pages)

===== PAGE 1 =====
          DIGITAL THEORY
   AND EXPERIMENTATION
USING INTEGRATED CIRCUITS

            SED AND ENLARGED
               M rris E.Levine

===== PAGE 2 =====

===== PAGE 3 =====
이GIT시．. THEORY
AND EXPERIMENTATION
USING INTEGRATED
CIRC내TS
REVISED AND ENLARGED


     Morris E. Levine
     college of Staten Is/and
     c/ry Univers/ty (7/ New York

===== PAGE 4 =====

===== PAGE 5 =====
Contents




PRE FACE


TO THE INSTRUCTOR


TO THE STUDENT


    fxperiPnenr 7

BASIC LOGIC FUNCTIONS                                    1


    Experimenr 2

BOOLEAN ALGEBRA AND SIMPLIFICATION OF LOGIC EQUATIONS   11


    Experimenr 3

DEMORGAN'S THEOREM                                      23


    f쟈7erment 4

TTL NAND/NOR GATES-DEFINITIONS AND OPERATION            31




                                       iU

===== PAGE 6 =====
    fxperiment 5

THE "EXCLUSIVE-OR" AND ITS APPLICATIONS                          45


    fXPeriment 6

FULL-ADDER AND FULL-SUBTRACTOR                                   55


    fxpezment ;7

BISTABLE OR FLIP-FLOP (FF)                                       65


    fxperimenr 8

BINARY COUNTERS AND THE BINARY NUMBER SYSTEM                     85


    즈7xperimenr 9

DIVIDE-BY-N COUNTERS AND DECADE COUNTERS                         99


    Experiment 끄）

SHIFT REGISTERS AND RING COUNTERS                                115


    Expe月mem //

PULSE FORMING AND SHAPING; THE SCHMITT TRIGGER                   133


    Experiment /2

INTEGRATED-CIRCUIT TIMERS-THE 74122, 74121, AND 555              147


    E쟈7er'menr ／β

DECODING AND ENCODING                                            157


    E쟈7eriment 14

RANDOM-ACCESS MEMORIES; (RAM)-SCRATCH PAD MEMORIES               169


    ExPeriment 15

THE OPERATIONAL AMPLIFIER                                        177


    Experfment 16

DIGITAL-TO-ANALOG (D/AJ AND ANALOG-TO-DIGITAL (AID) CONVERSION   189




                                           iv

===== PAGE 7 =====
     Experiment / 7

COMPLEMENTARY SYMMETRY MOS (CMOS)-PRINCIPLES AND CHARACTERISTICS                            199



     fxperiment 18

COMPLEMENTARY SYMMETRY MOS (CMOS)-TTL INTERFACE                                             209


ASTABLE MULTIVIBRATOR                                                                 217
Classes of multivibrators. Operation of collector-coupled multivibrator. Frequency of
collector-coupled multivibrator. Nonsymrnetrical rnultivibrator. Multivibrator
synchronization
F니P-FLOP                                                                            225
Description and use. Flip-flop operation. Transistor switching modes
THE ONE-SHOT (MONOSTABLE) MULTIVIBRATOR AND SCHMITT
TRIGGER                                             229
One-shot multivibrator. Schmitt trigger.

MIXERS, MODULATORS, AND DEMODULATORS                                                 235
Nonlinear distorlion. Mixer. Amplitude modulation. Percent modulation. Side frequen-
cies. Radio frequencies. Envelope detector.
PHASE-LOCKED LOOP                                                            243
Phase detector. VCO. Phase-locked loop. Free-running mode. Capture and lock.
Locked output. FM output. The 565
THE SILICON CONTROLLED RECTIFIER (SCR)                                              249
Voltage-current characteristic. Gate control of forward breakover voltage. SCR rat-
ings. SCR used as a rectifier

      ApPendix 겨

CATHODE-RAY OSCILLOSCOPE (CRO)                                                              257

      Appendix B

LOGIC SYMBOLS                                                                               259

      계ppenmX (?

THE UNIT-LOAD CONCEPT                                                                       261


      쟈'pendix D

IC LOGIC DIAGRAMS AND PIN CONNECTIONS (TOP VIEW)                                            263


      Appendix f

GLOSSARY OF LOGIC AND INTEGRATED-CIRCUIT TERMINOLOGY                                        271


      月Ppendix f

REFERENCES                                                                                  277


      Appendtx G

IC SOCKET, SWITCH BANK. AND EQUIPMENT                                                       279



                                                             v

===== PAGE 8 =====

===== PAGE 9 =====
neFoce



Since the publication of the first edition of this manual, the companion textbook, Digital Theory
and Practice Using Integrated Circuits, has been published. When the textbook was written, it was
organized and coordinated with the laboratory manual to form one integrated course of study in "
digital electronics with the textbook theoretical development and laboratory experiments follow-
ing in the same order. In this second edition of the laboratory manual, this organization and
coordination has been continued. The laboratory experiments and the text develop the building
blocks in the same order with each reinforcing the other.
      This laboratory manual has been developed to provide laboratory training and experience in
digital electronics using integrated circuits in the laboratory environment of the industrial elec-
tronics laboratory. As in the industrial electronics laboratory, all the measurements (with very
minor exceptions) are made using the cathode-ray oscilloscope. This manual therefore serves two
purposes. Besides providing the digital techniques experience, it also provides intensive and thorough
training in the use of the CRO as a universal tool for the measurement and analysis of digital circuits.
      There are five primary techniques used for the analysis of digital circuits and theory. They are:
          l
          Voltage levels
          1




    ^ J
    ,
    1 ^
          Logic levels; 1 010,1 or F,H or L,0N or 0FF
          1




          Logic diagrams
          1



          4
      J   Mapping methods
          1




    \
    '    Sequential operations. The CR0 is used to demonstrate and perform the analysis. Timing is of extreme
          ·




importance in sequential digital systems.

The experimental measurements of this manual develop the technique of using the CR0 to'analyze
the timing of sequential systems. All five methods are integrated to advance understanding of
digital principles.
      Eighteen experiments are included in this manual to provide thorough coverage of digital
principles. They begin with a series of experiments on the principles of logic. These are followed
with experiments on arithmetic operations. Several experiments cover the material on counters,
counter techniques, the binary number system, decoding-encoding, memory techniques, and pulse

                                                    vii

===== PAGE 10 =====
generation and pulse shaping and the IC Schmitt trigger. The operational amplifier has become of
great importance in digital techniques. Two experiments develop the principles and applications
of the op-amp in D/A and AID conversion. Two experiments with CMOS develop the principles
and characteristics of this logic family.
     New in this second edition are the following:

      I. A section "To the Student" has been added.
      2. Experiment 1. The AND and OR gates using dk'des have been eliminated. Added is a section using an
AND-OR-INVERT gate.
      3. Experiment 6. A 4-bit MSL full-adder is used to illustrate how MSI simplifies logic circuity. This IC is
used to perform addition and complementary subtraction. LEDs are used to show the logic levels.
      4. Experiment 10. A 5-bit MSI shift register is used to simplify the wiring. To provide a visual display of
data movement in a shift register, LEDs are used to show the logic levels.
      5. Experiment 11. This now combines two experiments from the first edition into one experiment on pulse
forming and shaping and the Schmitt trigger.
      6. Experiment 12. This is entirely new and discusses integrated-circuit timers: types 74121, 74122, and
the 555.
     7.   Experiment 13. Adds a seven-segment LED display to the experiment on decoding and encoding.
      8. Experiment 14: A 64-bit RAM replaces the 16-bit RAM and shows how LSI memories can be used for
code conversion.
      9. Experiments 17 and 18. These are new and are on CMOS logic. Experiment 17 is on CMOS principles,
noise immunity, and high-frequency dissipation. Experiment 18 covers the interface between CMOS and TTL. Al-
though numbered 17 and 18, if one desires to discuss CMOS early in the semester, these experiments can be per-
formed after Experiment 4.

      Experiments follow a uniform format and are divided into three sections:

       1. The experimental laboratory data. Data tables are marked with the letter E.
       2. Required results. The experimental data are analyzed and converted to general logic levels. Correspond-
ing tables are marked R.
       3. Discussion. In this section the student is required to answer a series of questions which are based upon
the experimental results and which integrate the data and digital theory. Corresponding tables are marked with the
letter D.

     Many types of IC logic families have been developed. Any one family could be used to pro-
vide a complete set of'experiments. This manual provides experience with TTL, the operational
amplifier, and CMOS.
     Whenever possible, an experiment starts with the basic building of a logic operation. Once the
principle has been developed, it is replaced by an MSI unit. This provides students with an under-
standing of the logic and gives them a feeling for the trend in integrated circuits toward MSI and
LSI and, in addition, simplifies the wiring of more complex circuits.
     All the ICs used in this manual are of the 14-pin or 16-pin dual-in-line (DIP) construction.
Appendix G gives constructional details of a laboratory IC socket and switch bank arrangement
which readily lends itself to the wiring and breadboarding needs of a laboratory and to squad
organization and participation. The IC socket is mounted on a - in. aluminum channel and the
pins are connected to universal 5-way binding posts. This permits the use of stackable banana
plug leads for interconnection.
     I wish to express my appreciation to Richard Brown, John Gappa, and Gilbert Bank, labora-
tory technicians at the College of Staten Island, for their suggestions and assistance, particularly
with respect to the socket and switch bank construction; to the students at the College of Staten
Island for their help; to Professor Jack Waintraub of Middlesex County College for his suggestions
and assistance in the revision of the first edition; to Dr. Irving Kosow, with respect to the format;
and to Mrs. Jean Johnson for her assistance, excellent typing, and proofreading of the manuscript.

                                                       v沚

===== PAGE 11 =====
To the Instructor




The ICs used in the experiments are all in the dual-in-line 14-pin or 16-pin configuration. A con-
venient method of storage is in the plastic shipping container used by the IC manufacturers for
shipping production quantities of ICs to the users.
     The ICs used in the experiments (as is true for semic9nductors in general) do not have a great
overvoltage tolerance before their dissipation is exceeded. The procedure suggested in Appendix A,
of calibrating the CRO and checking the power supply voltage against it, if carefully followed at the
beginning of each experiment, will protect the ICs against overvoltage and at the same time piovide
some additional CRO experience.
     Voltage measurements should be made to within 0.1 V.
     The ICs used have short internal connections and high FT. If allowed to remain in the active
region, there is a great possibility of parasitic oscillation. This can occur in obtaining the transfer
characteristics in Experiment 4. The bypass capacitor at the gate input is a parasitic oscillation
suppressor. For the same reason, a pulse generator should have a short rise and fall time, especially
when toggle flip-flops are being used, to prevent the buildup of oscillations and a resultant false
count. Should there be any such suspicion, Schmitt trigger IC types 7413 or 7414 can be used to
reduce rise and fall times of pulse generafr.-q.
     If the pulse generator is square-wave-centered around zero voltage, it cannot be used with the
ICs, since they will not accept negative-going gate input voltages. A small-signal diode can be used
across the pulse generator to clip the negative-going portion of the wave.
      Although the wiring in some of the experiments is somewhat complex, a wiring layout as close
as possible to the circuit drawing will help in troubleshooting.
     Students should be encouraged to write the values of the logic variables at each point of the
logic diagrams in the manual.
     If a dual-beam or dual-trace CRO is available, the bistable action of Experiment 8 can best be
demonstrated if the beams are displaced horizontally from each other or one beam is operated with
a lower brightness.
                                                  j;K

===== PAGE 12 =====
F LIP-F LOP OUTPUT MEASUREMENTS: A PRECAUTION-CRO ISOLATION


A long lead from a bistable, or counter, or intermediate outputs of a counter, or monostable multi-
vibrator may cause undesired loading and prevent the bistable from toggling or dividing properly,
or the monostable from functioning properly. If such difficulties are encountered, a composition
2200-a decoupling resistor at the IC end of the lead can eliminate the loading problems. The lead
length from the 2200-a resistor to the IC should be kept short. This decoupling may be needed
both for the CRO vertical input and for external triggering.

                                  To
                                  K〕           2200n                              CRO
                                          ㅇ－---/\/\/\/－ㅇ                           O

IC PIN CONNECTIONS AND IDENTIFICATION


The ICs used in this manual are made in the dual-in-line case. The IC pin terminals progress in a
counterclockwise direction as seen from the top side away from the pins. The ICs are in either
14-pin TO-l 16 (EIA designation) or 16-pin configurations. In these ICs pin I is located by an
identifying symbol, or the location of pins I and 14 (14 pin IC) or pins 1 and 16 (16 pin IC) are
identified by an index notch at the end of the case where these pins are located. This is illustrated
in the figure below.
                                                    I이：) View (away from pins)
     Index                                                               Index




             갸_       4 13 12 11 10             9     8
                                                                         Notch\
                                                                               \           ㅣ16 15 14 13 12 11 10 9
   Pini            工：:7J 4~   -
                                  Q
                                  U
                                      A
                                      `
                                           '=
                                           U
                                                ‘극
                                                U     '              Pin 1                         2   3    4   5   6   7   8
                                                                  Identification //         I_
                                                                                      災·
Identificatio
      Notch，

                    (a)       14-pinTO-116                                                   (b)   16-pin
                                                Dual in-line pin location.




                                                              x

===== PAGE 13 =====
To the 닷udent




Digital electronics has become the most important field in electronics and one of the most im-
portant technological fields today. It is involved in all aspects of modern technology, such as data
processing, data transmission, radio, TV, timekeeping, industrial control, and instrumentation for
many fields of science. Digital electronic circuits and systems are becoming increasingly more corn-
plex, yet analysis of such systems will reveal that they are all combinations of simple and basic
building blocks.
     This laboratory manual was developed to provide you with laboratory experiments and experi-
ence to let you more easily understand the theoretical material covered in the classroom, and to
provide practical illustrations of how combinations of these simple building blocks can yield corn-
plex and useful systems. In addition, the experiments and laboratory experience will provide you
with experience in fault analysis and equipment maintenance.
     To analyze the performance of these digital blocks, the most useful measuring tool is the
cathode-ray oscilloscope (CRO) because it not only measures voltage but it can measure time, dis-
playing both the waveforms`of digital electronics and their relative time of occurrence. Almost all
of the measurements in this manual are performed using the CRO.
     In later experiments the wiring becomes complex. Try to wire them so that the wiring is
organized by placing the ICs and switch banks to look like the circuit diagram of the manual. Wire
using as short leads as conveniently possible. Leads that are too long introduce capacitive loading
and may introduce spurious pulses and glitches, which may give incorrect results in sequential cir-
cuits such as counters and shift registers. If trouble occurs, neat and orderly wiring will make it
easier to locate the fault.
     If trouble does occur, rewire only as a last resort. Try to determine what logic levels should
occur at points in the circuit as a 'result of the input levels. If they do not occur as predicted, slowly
disassemble the circuit at that point until you obtain an expected result. The circuit can then be
gradually reassembled until the fault reoccurs. Marking the circuit diagram with the Boolean ex-
pressions in terms of the logic inputs is of great usefulness.
                                                   xi

===== PAGE 14 =====
 1. Basic Logic Functions
 2. Boolean Algebra
 3. DeMorgan's Theorem
                                                                       1
                                                                       1
                                                                           1       ]
                                                                                   1   1
                                                                                                       1   1
                                                                                                           1
                                                                                                               驪a      1


                                                                       1   1       1   l               1
 4. TTL NAN D/NOR Gates                                                1       1
 5. Exclusive OR                                                       1   1       1                       1                           1
 6. Full Adder/Full Subtractor                                         1   1       1           1       1                           1   1
 7. Bistable                                                           1   1                                               1
 8. Binary Counters                                                    1                               1                   3
 9. Divide by N Counters                                                                                                   4                   1
10. Shift Registers                                                    1                                                       3                   1
11. Pulse Forming/Shaping: Schmitt Trigger                             1       1                   1
12. Integrated Circuit Timers: 74122. 74121, 555   1                               1                                                                   1   1
13. Decoding/Encoding                                                              1                   `       1   1           1               1
14. Random Access Memories (RAM)                                       1       1                                                           1
15. Operational Amplifier                              2
16. D/A and A/D Conversion                             2                           1   1                                                       1
1]. CMOS Principles and Characteristics                        1
18. CMOS - TTL Interface                                   1       1                       1

                                                   Integrated-Circuit Types and Experiments in Which They Are Used

===== PAGE 15 =====
      Measure voltages as accurately as possible. Be sure that the CRO is measuring voltage correctly.
You can do this by using the CRO internal calibrator. You should be able to measure voltages to
within 0. 1 V. If you do not need this precision later, you can discard it.
      Some of the experiments require graphs. Plot these as you take the data. This will reveal data
errors and inadequate data.
      When CRO sketches are required, they should be drawn carefully on your laboratory manual
graphs. They should be drawn accurately enough so that you can read voltage and time from them
at any point. Generator waveforms should be displayed on the CRO with respect to the graticule
as closely as possible to those shown in the manual. The timing of relative waveforms in a digital
system cannot be displayed correctly without external triggering.
      Data obtained experimentally with the CRO are in volts. The required (R)section translates
these into logic levels I and 0. In the discussion(D)section these R logic levels are analyzed. Care-
ful study of the R data and of your textbook will enable you to answer these questions.




                                                xw

===== PAGE 16 =====

===== PAGE 17 =====
                                                                               Experiment]



Basic Logic Functions




OBJECT


     1. To study the basic logic functions AND,OR,INVERT, NAND,and NOR.
     2. To study the representation of these functions by truth tables, logic diagrams, and Boolean algebra.



INTRODUCTORY THEORY


In electronic logic circuits inputs and outputs occur as voltage levels. These inputs and outputs are
dual valued or dual leveled. To provide a common basis for comparison it has become usual to
represent the two levels symbolically as I or 0. In one circuit the I might be +20 V and the 0 might
be - 10 V. In some other circuit the I might be +15 V and the 0 might be +1 V. Despite the differ-
ence in voltage levels, a basic operation will be the same using either pair of voltages.

     AND:     A multi-input circuit in which the output is a 1 only if all inputs are 1.
     0R:    A multi-input circuit in which the output is a I when any input is a 1.
     INVERT: The output is 0 when 仕1e input is 1, and 仕ie output is 1 when the input is 0.
     NAND:      AND followed by INVERT.
     NOR:     OR followed by INVERT.
       Truth table: Representation of the output logic levels of a logic circuit for every possible combination of
levels of the inputs. This is best done by means of a systematic tabulation.




                                                          1

===== PAGE 18 =====
EOt기PMENT R （기RED

    CRO, dc coupled and calibrated
    dc power supply, +5 Vat 50 mA
    IC type 7400 quad 2-input NAND gate
    IC type 7402 quad 2-input NOR gate
    IC tvoe 7404 hex inverter
    IC type 7420 dual 4-input NAND gate
    IC type 7432 quad 2-input OR gate
    IC type 7451 dual 2-wide, 2-input AND-OR-INVERT gate
    Switch bank, 5 switches per bank

                                         IC manufacturers' part numbers.
                                                                    7exas          National
               1:'pe      Motoroh               F'airchi끄／       Jnstrumen格      Semiconincr0r
               7400       MC7400P               7400PC            SN7400N           DM7400N
                          MC7400L               7400DC            SN7400J
               7402       MC7402P               7402PC            SN7402N           DM7402N
                          MC7402L               7402DC            SN7402J
               7404       MC7404P                7404PC           SN7404N           DM7404N
                          MC7404L                7404DC           SN7404J
               7420       MC742OP                7420PC           SN742OP           DM7420N
                          MC7420L                7420DC           SN7420J
               7432                              7432PC           SN7432P           DM7432N
                                                 7432DC           SN7432J
               745l                             745Ht             SN745lP           DM745 iN
                                                745 1DC           SN7451J



IC PIN CONNECTIONS

Each of these ICs ai'e in a 14-pin dual-in-line case. The base pins progress in a counterclockwise
direction as seen from the side away from the pins, as shown in Fig. 1-1. pin 1 is located by an
identifying symbol, or the location of pins I and 14 are identified by an index notch at the end of
the case where pins 1 and 14 are located.

                                         1
                                 ,:.h듀    .14
                                                  13 12 1' 10 9 8
                                                                                   Top view
                            Index n。 tch
                                                                                (away from pins)
                                   //｀∼ 1 2            3     4   5 6 7
              Pin 1 identification
                        Fig. 1-I . ic pin location, 14-pin dual-in-line (TO-I 16) case.


PRELIMINARY PRECAUTIONS

The ICs used in this experiment are fragile and have a small voltage overload margin. It is extremely
important that the exact required voltage be applied. The power supply voltage should be the last
connection made. Before connections to the power supply are made, its voltage should be checked
both against its own voltmeter and against the calibrated CR0.

                                                             2

===== PAGE 19 =====
     All measurements in this experiment are made with a calibrated CRO. Before making any
measurements, calibrate the CRO (see Appendix A). After the CR0 is calibrated, use it to check
the power supply voltage. If a disagreement occurs between the power supply voltmeter reading
and the CRO measurement, call the instructor.


EXPERIMENTAL PROCEDURE


For each part of the experiment apply the indicated voltage and make voltage measurements at the
points indicated to comlplete the tables. Use the CRO to measure the voltage. Use a sensitivity of
1 V/div and make measurements to within 0.1 V.


1.   ICORGate

                                                                                 Output
                                                                                 pin


                     t _                  亡－
                                                          Input
                                                                    ;;
                                                                                  /
                                                                                           cTRCO


                                                                                      ,/Cc= +5 V to pin 14
                  -o- ----o                               p·ns
                                                                                      0 (ground) to pin 7


                                                   Fig. 1-2. IC OR gate.

Note.' The IC type 7432 has four 2-input OR gates within its package. Only one of these gates is
used in this experiment. It is the gate whose input pins are pins 1 and 2 and whose output pin is pin
3. See Appendix D for complete logic diagram and pin connections.

                                               Table 1-lE. IC OR gate.
                                       Pin 1              /in2           Pin 3
                                               0                0
                                               0           +5
                                         +5
                                                                0
                                         +5
                                                           +5
2.   INVERT


                                                                                          Table l-2E. INVERT.
                                                                                           /in /      Pin 2
                                                                                                  0
                                                        `/cc= +5 V to pin 14                 +5
     工．
                                                        0 (ground) to pin 7


                          Fig. 1-3. IC inverter.

                                                                3

===== PAGE 20 =====
3.   OR + INVERT = NOR




           +5V_
                         _




                                        i.   )   743_      )3
                                                                          5j>      o
                                                                                       6

                                                                                             Vcc= +5V to pin 14

                     -E--o----o                                                              0 (ground) to pin 7
                                                                                                  Both ICs

                                             F성. 1-4. OR + INVERT.



                                                       Table L3E.

                                         74了2                              74(74
                             /in /               Pin2                      /in 6

                                   0                   0

                                   0              +5
                              +5                       0

                              +5
                                                  +5
4.   NOR




                  +5 V




                                                                                           \/cc= +5V to pin 14
                                                                                            0 (ground) to pin 7


                                                 Fig. 1-5. NOR.



                                                       Tableㅏ E.

                                       Pin 3                    /in2      Pin /

                                             0                        0

                                             0                   +5
                                        +5
                                                                      0

                                        +5
                                                                +5
                                                                      4

===== PAGE 21 =====
5.   2-Input NAND



                                                                        3
                                                 H74
                                                            7400



                                                                            Vcc= +5 V to pin 14
                                                                            0(ground) to pin 7

                                             Fig. 1-6. NAND.



                                               Table LSE.

                              Pin I              Pin2          /in 3

                                         0              0

                                         0             +5

                                    +5                  0

                                    +5
                                                       +5



6.   4-Input NAND




            +5 V


                                                                            \/Cc= +5 V to pin 14
                                                                             0 (ground) to pin 7




                                         Fig. 1.7. 4-input NAND.


                                              Table 1.6E.

                    /in /     Pin2               八n 4          /in 5         /in 6

                          0              0             0           0

                     +5
                                         0             0           0

                     +5
                              +5                       0           0

                     +5        +5                      +5          0

                     +5       +5                       +5          +5


                                                       S

===== PAGE 22 =====
7.   AND-OR-INVERT




                                   Fig. 1-8. 2.wide, 2.input AND-OR-INVERT gate.


The 7451, whose logic symbol is shown in Fig. 1-8, is a dual 2-wide, 2-input AND-OR-INVERT
gate. Determine the voltage of Y for the following inputs.

                                                    Table L7E.
                                            A            B            C    D        Y
                              l             0            0            0        0
                              2        +5                0            0        0
                              3        +5                U       +5            0
                             4         +5           +5
                                                                      0        0
                              5        +5
                                                    +5           +5            0
                             6         +5           +5           +5       +5
REQUIRED RESULTS


For each part of the experimental results complete the following truth tables. Use I and 0, defining
logic 1 as a voltage greater than 2.5 V and logic 0 as a voltage less than 1.0 V. Table l-1R corre-
sponds to the data of Table 1-1E, and so on. All tables should have ls and 0s.

                         Table 1-IR.                                                  Table l-2R.

                 ／쑈 /      ／功2              /in 3                                  /in /     Pin2




                                                             6

===== PAGE 23 =====
                Table 1-3R.                                                   Table l-4R.


/in /
        7行2

              Pin2
                                  749I

                                  Pin 6
                                                                  /in 3         Pin2
                                                                                               ㅣ
                                                                                            /in /




                                          Table 1-5R.
                              /in /           /in 2       /in 3




                                          Table I-6R.
                Pin 1         Pin2            /in 4       /in.5           Pin 6




                                          Table 1-7k.
                              A           B           C      D            Y
                     1

                     2

                     3

                     4

                     5

                     t


                                                7

===== PAGE 24 =====
DISCUSSION




                       A

                       B

                                     Fig. 1-9. L뺌Ic circuit 1.


   (a) What type of logic function will occur between A, B, and C in Fig. 1-9?



   (b) What type of logic function will occur between A, B, and Din Fig. 1-9?



   (c) Write a truth table in the columns of Table I-ID between A, B, C, and D, using is and Os
       for Fig. 1-9.


                                                Table 1-iD.
                                       」4        B        c   z)
                                        0        0
                                        0         l
                                            l    0
                                            l    1




                                                      8

===== PAGE 25 =====
4.   Express the Boolean equations between inputs and outputs in Table l-2D for each part of the
     experiment. Use letter inputs and outputs where they are used. With ICs the Boolean equation
     between input and output is expressed using the pin numbers. For example, suppose that we
     had a 2-input AND gate with inputs at pins 4 and 5 and output at pin 6. The IC specification
     data sheet would be written as 4' 5 = 6 (rather than pin 4' pin 5 = pin 6). Use pin numbers for
     parts 1 through 6 and letter inputs for part 7.

                                             Table L2D.
                      Part                    끄bolean Equation
                        l
                        2
                        3
                        4
                        5
                        6
                        7


5.   For part 7 (Tables l-7E and l-7R)

     (a) Comparing lines 1, 2, and 3, why is the output Y unchanged despite changes in A and C?




     (b) Comparing lines 3 and 4, both have two 1 inputs. Why is Y different in line 4 compared to
         line 3?




     (c) Comparing lines 4, 5 and 6, why do additional 1 inputs in lines 5 and 6 have no effect
         on Y?




                                                 9

===== PAGE 26 =====
6.   Complete the following truth table for the diagram of Fig. 1-10:



                                  A    B     A     B     K     L     Y
                                  0    0
                                  0    l
                                  l    0
                                  l    호




                                      Fig. 1.10. Logic circuit ㅍㅍ．




                                                 10

===== PAGE 27 =====
                                                              Experiment 2



Booleon AI9ebra
and Simplification
of Logic Equations


OBJECT


To study methods of representing and simplifying logic equations by Boolean algebra.


INTRODUCTORY THEORY


The exact implementation of many digital logic circuits will result in a circuit that functions as
expected. Nevertheless, many such circuits can be reduced to a simpler form by the application
of Boolean algebra and by Karnaugh mapping. The basic Boolean reducing equations are given
in Eqs. 2-1, 2-2, 2-3, 2-4, and 2-5.

                                             A· l =A                                        (2-la)
                                             A·0=0                                          (2-ib)
                                             A ' A= A                                       (2-ic)
                                             A·A=0                                          (2-id)
                                            A+ 1 = I                                        (2-2a)
                                            A+ 0 = A                                        (2.2b)
                                            A+ A= A                                         (2-2c)
                                            A+ A= 1                                         (2-2d)
                                                A= A                                         (2-3)



                                               11

===== PAGE 28 =====
                                               1· 1= 1                                        (2-4a)
                                                1·0=0                                         (2.4b)
                                               0·1= 0                                         (2-4c)
                                               0·0=0                                          (2.4d)
                                               1+1=l                                          (2-5a)
                                               1+ 0= 1                                        (2-Sb)
                                               0+ 1= 1                                        (2-5c)
                                               0+ 0= 0                                        (2.5d)

Using these as a base, more complex reducing equations can be derived. In simplification proce-
dures a variable and its complement are treated as separate variables and logic equations can be
expanded and combined as in ordinary algebra using the priorities of ordinary algebra. Reductions
of variables can then be performed using Eqs. 2-1, 2-2, 2-3, 2-4 and 2-5; similar reducing equations;
and Karnaugh maps.
     Equations 2-la, 2-Ib, 2-2a, and 2-2b are of special significance since they indicate how trans-
mission of data can be controlled or gated. From 2-la and 2-lb it can be seen that a 1 applied to an
AND gate permits data to be transmitted while a 0 blocks data transmission. Similarly, from 2-2a
and 2-2b, a 1 applied to an OR gate blocks transmission, whereas a 0 to an OR gate allows data
transmission.
     Karnaugh maps provide a graphic/visual means of logic simplification. They use Eqs. 2-1 and
2-2 as the basis for their justification.



EQUIPMENT REQUIRED


     CR0,dc coupled and calibrated
     dc power supply,+5 V at 50 mA
     Square-wave generator(SWG), 10 kHz,0 to +5 V
     IC type 7400 quad 2-input NAND gate
     IC type 7404 hex inverter
     IC type 7405 hex inverter, open collector
     IC type 7432 quad 2-input OR gate
     Switch bank,S switches per bank
     Two 5.6-k2 10% composition resistors

                                     ,c manufacturers'part numbers.
                                                             Teras       National
                乃4)e       Motoroh        Fairchild      Instruments   Semiconductor
                7400       MC7400P         7400PC         SN7400N         DM7400N
                           MC7400L         7400DC         SN7400J
                7404       MC7404P         7404PC         SN7404N         DM7404N
                           MC7404L         7404DC         SN7404J
                7405       MC740SP         7405PC         SN7405N         DM740SN
                           MC7405L         7405DC         SN740SJ
                7432                       7432PC         SN7432N         DM7432N
                                           7432DC         SN7432J


                                                    l2

===== PAGE 29 =====
PRELIMINARY PROCEDURE


CRO

To obtain the correct wave shapes it is necessary to use external triggering from the SWG. If a dual-
beam or dual-trace CRO is being used, one of the traces can be used to monitor the SWG output
while viewing the wave shapes at the required points.
     View the output of the 10-kHz SWG on the CRO and adjust its output to +5 V. Use EXT
TRIGGER from the SWG as shown in Fig. 2-1(a)and use NEG, AUTO TRIGGER. Adjust the CRO
horizontal sweep rate so that each cycle occupies two horizontal divisions as shown in Fig. 2-1(b).




                   SWG
                                     1_                                     O얹Oe f。rEXTall媤GGER
                                                                              VERTICAL
                                                                            O 5V/DIV
                                                                                           'ef。rms

                  10kHz
                  0 to +5 V            l                                    O

                                      (a) CRO Connections to SWG




 0
                                      (b) SWG Output Waveform
                         Fig. 2-1. Square-wave.generator(SWG)output waveform.



Power Supply

Check the power supply voltage against the calibrated CRO. See Appendix A.


EXPERIMENTAL PROCEDURE

For all ICs in this experiment: Vcc = +5 V to pin 14,0(ground) to pin 7.
     There are two procedures in this experiment. In one, a voltage table must be completed and
in the other, waveforms are viewed on the CRO and sketched on graph paper.
     When a table must be completed, ，∼V the CRO to make voltage measurements at the points
indicated to complete the table.
     Where a signal input is applied from the SWG, view the waveforms on the CRO and sketch the
waveforms at the indicated points on the graph paper provided with each part of the experiment.
Always use EXT TRIGGER to the CRO as shown in Fig. 2-1(a).




                                                 13

===== PAGE 30 =====
1.
     (a) Complete Table 2-1 E using Fig. 2-2(No SQUARE-WAVE GENERATOR)
                                                                     .

                                                                 Table 2-IE.
                                                         A           x             y
                                                             0
                                                        +5
                                    +5 V


                                                                         '               _2
                                    寸        ，                                 7404
                                                                              1）        乂
                                                 >"
                                                       SQUARE                                       To pin 3
                                        초．
                                                        WAVE
                                                                              0_                    for part 1(b)
                                                      GENERATOR
                                                        SWG                                  」．-
                                                                  rig. 2-2.


     (b) In Fig. 2-2 disconnect pin 3 from the switch and connect pin 3 to the SWG. View the
         waveform1s at the points indicated and sketch on Fig. 2-3.

                       ＇戶
         +5
     x
               0

          +5
     V
               0

                                                                  Fig. 2·3.




     (a)           Complete Tables 2-2E and 2-3E using Fig. 2-4.

                                                                                       (b)         Table 2-3E. Pin I
                            Table 2-2E. Pin 1                                                        connected to
                            connected to +5.                                                            ground.
                                A                                                                     J4        y
                                    0                                                                      0
                               +5
                                                                                                      +5

                                                                     14

===== PAGE 31 =====
                      +5V_                     -．   《
                                                                           74
                                                     0


                                                              Fig. 2-4.


(c)        In Fig. 2-4 disconnect pin 2 from the switch and connect pin 2 to the SWG. View and
           sketch the waveforms on Fig. 2-5.


           +5
 Pin 1
  at
 +5 V
                Y
           +5
Pm 1
 at 0
                0
                                                              Hg. 2·5.


(d)        Complete Table 2-4E using Fig. 2-6.

                                                         Table 2-4E.
                                                         J4            y
                                                              0
                                                         +5
                                      +5
                             亡             ，        f于2 "_                      Y



                                 里，
                                                              Fig. 2-6.



(e)        In Fig. 2-6 disconnect pins I and 2 from the switch and connect pins I and 2 to the
           SWG. Sketch the waveform on Fig. 2-7.

  +5
       V
       0
                                                              Fig. 2-7.

                                                                  l5

===== PAGE 32 =====
(f)   Complete Table 2-5E using Fig. 2-8.

                                                Table 2-SE.
                                                4             y
                                                     0
                                                +5
                     +5 V古
                         ，
                         ^

                         v

                         ㅗ



                                               n8. 2-8.

(g)   In Fig. 2-8 disconnect A from the switch and connect A to the SWG. View and sketch
      the waveform on Fig. 2-9.

       +5
      Y
            0

                                               Fig. 2·9.

      Note. A glitch (spurious short-duration pulse) may appear at Y. If it appears, it should
      be shown on the waveform. However, its effect is to be ignored in the discussion section
      of the experiment.




(a)   Complete Tables 2-6E and 2-7E using Fig. 2-10.

                     Table 2-6E. Pin '                        (b)         Table 2-7E. Pin 1
                     connected to +5.                                   connected to ground.
                 A                 /   y                                 '4                  I       Y
                     0                                                        0
                +5
                                                                        +5
                                         ㅇ놀b
       +5~- o



                                                          伊         X        3   )4
                             \--
                                                                                      7404       _
                                       0                 74



                                               Fig. 2-10.


                                                     16

===== PAGE 33 =====
(c)      In Fig. 2-10 disconnect pin 2 (type 7400) from the switch and connect it to the SWG.
         View and sketch the waveforms at the points indicated on Fig. 2-1 1.

             +5
  Pm 1 ×
at +5 V
        0

             +5
 Pin 1
at + 5 V Y
         0

             +5
 Pin 1                 x
at 0
                       0

             +5
Pin 1
 at0                   Y
                   0
                                                       Fig. 2J l.

(d) Complete Table 2-8E using Fig. 2-12.

                                                           Table 2-8E.
                                                   A             x       }r
                                                       0
                                                  +5
                               +5V



                                                                         1
                                                                              >2
                           <         ,                                             7404   _
                                         74oo,
                                             ,p
                               오．
                                                       Fig. 2·12.

(e)      In Fig. 2-12 disconnect A from the switch and connect A to the SWG. View and sketch
         the waveforms at the points indicated on Fig. 2-13.

                  +5
         x
                       0

             +5
         Y
                       0

                                                       Fig. 2J3.


                                                            l7

===== PAGE 34 =====
     (f) Complete Table 2-9E using Fig. 2-14.

                                                     Table 2-9E.
                                             A             /
                                                 0
                                            +5
           +5 V



                                                                            〕＞5
                                                 Fig. 2-l4.


     (g)    In Fig. 2-14 disconnect A from the switch and connect A to the SWG. View and sketch
            the waveforms at the points indicated on Fig. 2-15.

               +5
           x
                    0

               +5
           Y
                    0

                                                 Fig. 2.l5.

4.
Make the voltage measurements at the required points to complete Tables 2-b0E and 2-11E for the
configurations of Figs. 2-16 and 2-17. Note: locate AB on Fig. 2-16.

     (a)
                                                     Table 2-b0E.
                                   d4
                                            B            4β         X   y
                                        0        0
                                        0   +5
                                   +5            0
                                   +5
                                            +5
                                                      l8

===== PAGE 35 =====
                                                                  743)   _
                 1>             2
                       7404




+5VtE굿．  A   B                                  7400      Q       3)   6

                                                    743   )   6

                                                       -' G2
                               Fig. 2.16.




(b)
                                 Table 2-lIE.

                      」4
                                    fr      x   y

                           0         0

                           0        +5

                      +5             0

                      +5            +5




  +5 V




                               ng. 2－프7.

                                    효9

===== PAGE 36 =====
REQUIRED RESULTS


Complete the following tables corresponding to the voltage tables of the experimental data.
Assume positive logic, in which logic 1 > 2.5 V and logic 0< 0.5 V. All the tables should have Is
and Os.

                                                          Table 2-1R.
                                                      A       x




               Table 2-2R.                Table 23R.                    Table 2-4R.                        Table 2-SR.
                                          4           y                 '4             y                   J4         Y




     Table 26R.                        Table 2-7R.                           Table 2-8R.                            Table 2-9R,
ㅣA
           x        Y                         x       Y                 A          x         Y                  4         /




                                 Table 2-boR.                                              Table 2-I 1R.
                   月         B       AB           x       Y                    A           B




1기SCUSSION


1.   What is the function of the inverter between X and Y in part 3?




2.   (a)   For parts 1, 2, and 3, compare your data at Y with that at A. The Y data will be either 1,
           0, or the same as A. Enter the results Of Y as either 1, 0 or A in column Y. (Neglect any



                                                              20

===== PAGE 37 =====
           glitches that may have appeared in the waveforms.) For example, in parts 1(a)and 1(b),
           Y is the same as A and A has been entered in column Y;in parts 2(a)and 2(c), Y is always
           equal to 1. One(1)has been entered in column Y.


     (b) There is a Boolean equation which expresses the relationship between the input A and the
         output Y for each row of Table 2-l2D which has been demonstrated experimentally.
         This equation can be determined from the logic diagram. From the logic diagram and the
         experimental data, express this equation in the Boolean equation column (see Eqs. 2-1,
         2-2, 2-3). For example, in parts 1(a) and 1(b), the experimental data have shown that
         Y = A. The logic diagram is that of a double inversion. The Boolean equation is A = A
         and it has been entered in Table 2-l2D. For parts 2(a)and 2(c), the Boolean equation is
         A + 1 = 1. This has been entered into Table 2-l2D.


                                              Table 2-12D.
                                                y                  及7(7/a가i fquation
                          Part              A, 1, or 0       between／쨔,utA orSWG and γ
                1(a) and 1(b)                   A                      A =A
                2(a) and 2(c),pin 1 at +5       1                    A + 1= 1
                2(b) and 2(c), pin I at 0
                2(d) and 2(e)
                2(f) and 2(g)
                3(a) and 3(c),pin 1 at +5
                3(b) and 3(c),pin 1at 0
                3(d) and 3(e)
                3(f) and 3(g)



3.   Forpart4(a):
     (a)   What are the two inputs to gate G1 in terms of A and B?



     (b)   What is the output X in terms of A and B?



     (c)   What is the output Y in terms of A and B?



     (d) ' Based on your experimental results, what can we say (in Boolean terms) about the rela-
           tionship between X and Y? (Express in terms of A and B.)




                                                    2l

===== PAGE 38 =====
4.   For part 4(a), draw two Karnaugh maps and discuss your results for the inputs to (a)Gi and
     (b)G2.




5.   When the output of two gates(in this case inverters) are wired together(WIRED-COLLECTOR
     logic), we obtain a form of logic known as WIRED-OR,COLLECTOR-OR,PHANTOM-OR or
     IMPLIED-AND, DOT-AND. The most popular is WIRED-OR. This connection is permitted
     if the output collector loads are resistors (passive pull-up). TTL logic which has an active pull-
     up (the output collector load is another transistor) does not permit this because the output
     transistor may be damaged. However, some TTL ICs, such as the type 7405 inverter used in
     part 4(b), have an open output collector. This allows the use of a resistor as an output collec-
     tor load. Two or more output collectors can be wired together using a common load resistor
     for WIRE-COLLECTOR logic. The primary advantage of this type of logic, as can be seen from
     the WIRED-  OR designation, is the simple generation of OR/NOR logic without the need for an
     additional OR or NOR gate.
           From the truth table of part 4(b), what type of gate is formed by the two inverters at
     point X? At point Y? Write the Boolean equations between points X and Y and the inputs A
     and B.



6.   It is desired to gate (turn on and off) the output of a SWG by two separate gating signals.
     When both gating signals are at logic 1 (positive logic), the SWG output is transmitted. When
     the SWG output is not being transmitted, the output is to be at logic 1. Draw a logic diagram
     showing how to accomplish this using a NAND gate. Explain how the circuit operates.




7.    Repeat discussion problem 6 but change the diagram so that the output is to be at logic 0 when
      the SWG is not being transmitted and use a NOR gate. (Use inverters if necessary.) Explain
      how the circuit operates.




                                                   22

===== PAGE 39 =====
                                                                   ExperimenE 3



DeMor9on's Theorem




OBJECT


To simplify and modify Boolean logic equations by means of DeMorgan's theorem.


INTRODUCTORY THEORY


Frequently, the direct representation of a logic circuit results in a form that is not the most desir-
able immediately. For example, the solution may yield OR/NOR, whereas it is desired to use
AND/NAND. Sometimes the system solution results in a combination of OR/NOR and AND/NAND
when a single form of logic is desired.
     DeMorgan's theorem permits conversion of logic from OR/NOR to AND/NAND and
AND/NAND to OR/NOR. DeMorgan's theorem is given by Eqs. 3.

                                                      A+ B= A .B                                 (3a)
                                                      A·B =A+ B                                  (3b)

     The procedure in applying DeMorgan's theorem is the following:

             Replace AND with OR or OR with AND.
             Invert the variables.
     ^
     ,
             Invert the final result.
     ＾
         4
     珊
             If possible, simplify by applying double inversion.

    DeMorgan's theorem is applicable to any number of variables and to the whole or any part of a
Boolean equation.

                                                           23

===== PAGE 40 =====
EQUIPMENT REQUIRED


    CRO,dc and calibrated
    dc power supply,+5 V at 50 mA
    Switch bank, 5 switches per bank
    IC type 7400 quad 2-input NAND gate
    IC type 7402 quad 2-input NOR gate
    IC type 7404 hex inverter
    IC type 7405 hex inverter, open coilector
    IC type 7420 dual 4-input NAND gate
    5.6-ku 10% composition resistor



                                        IC manufacturers'part numbers.
                                                                7exas      National
                 Type       兀fαr0r0／α           Fairchil/    力i뵤7끄me壯S   Semiconductor

                7400         MC7400P            7400PC        SN7400N      DM7400N
                             MC7400L            7400DC        SN7400J

                7402        MC7402P             74O2PC        SN7402N      DM7402N
                            MC7402L             7402DC        SN7402J
                7404        MC7404P             7404PC        5N7404N      DM7404N
                            MC7404L             7404DC        SN7404J

                 7405        MC7405P            7405PC        SN740SN      DM7405N
                             MC7405L            7405DC        SN7405J
                 7420        MC742OP            7420PC        SN7420N      DM7420N
                             MC7420L            7420DC        SN7420J




EXPERIMENTAL PROCEDURE


For all the ICs in this experiment: VcC = +5 V to pin 14, 0 (ground) to pm 7.
     For each part of the experiment, wire the circuits shown and use the CRO to make voltage
measurements at the points indicated to complete the associated table.
     As you perform the experiment, for each point on the logic diagram express the Boolean
equation in terms of the input variables and write it on the diagram. For example, in part 1 you
should write A + B at point U, and you should write A + B at point X.




                                                        24

===== PAGE 41 =====
   +5 V




                                                    ng. 3-l.


                                              Table 3-1E.

          44                      B       U            V        1t/       X        Y
               0                  0
               0             +5
          +5                      0
          +5                 +5




               3 7404                         A       3)


                                                                >
                   >4
                                                                              Wi
                                                                                   >2
                                                                                        7404        _
                                                           4
+5 V


                                                                6
                                                                                               ))
                                                                                        7400,
                                               '>
                                                    Hg. 玉2.


                                              Table 3-2E.

                        A             A       B            1V         x       y
                         0                     0
                        0                     +5

                        +5                     0
                        +5                    +5


                                                      25

===== PAGE 42 =====
  +5 V




                                              Fig. 3-3.




                                             Table 3-3E.

                        」4
                                  B      U       V             l1'   x          y

                             0       0

                             0    +5

                        +5           0

                        +5        +5




                                                                                                                         >>>>>>
                                                                               +5 V (Vcc)

                                                                                    i5.
                                                                                               6k2                   ·

                                                                                                               L x
                                                                         · ㅓ
                                                                               7
                                                                               Z               9

                                                           3



+5 --m- --心                      O                     尸




    \-       \)-,
                                 녹b-
         A          B            C
   -O--c                         O

                                                 ㅓ
                                                                         -                。z

                                                                                          4
                                                                                                   742.
                                                                                                   7420
                                                                                                          )6
                                                                                                                 V
                                                       ㅡ                                                             …

                                                                                          仄J



                                                                         E
                                                       ●



                                               Fig. 玉4.

                                                  26

===== PAGE 43 =====
                                                                                                       Table 3-4E,
                                           』4
                                                             B                   C              』4
                                                                                                                B          C           z                 x           Y

                                                0             0                  0
                                                0             0             +5

                                                0            +5                  0
                                                0            +5             +5
                                      +5                      0                  0
                                      +5                      0             +5
                                      +5                     +5                  0
                                      +5
                                                             +5             +5




                                                                                                7400,      )O    _        三必                U

                                                                                                                                       3」

                                                                                                                          \        ,        2        740)        Q       )   Q
                                                                                                                                                                                 x
     V             --Q-       ----O




                                                                                                                          ", ajJ
+5
         -O-
                                                                                     L1              7400)

               A          B           C
                                                                                           "〕            8
                                                                                                7404                 9

                                                                                                                     1o    7400)            _i,




                                                                                                            0
                                                                                                                                       Q_
                                                                                          ">

                                                                                                                                                             7400
                                                                                                                                                    13


                                                                                                        Fig. 3-5.



                                                                                                       Table 3-SE.
                                                    A                  f1                 c            U              V        w                x            Y
                                                         0             0                  0
                                                         0             0                  +5

                                                         0        +5                      0
                                                         0        +5
                                                                                          +5

                                                    +5                 0                   0
                                                    +5                 0                  +5

                                                    +5            +5                       0
                                                    +5            +5                      +5


                                                                                                                27

===== PAGE 44 =====
REQUIRED RESULTS


Assume positive logic, I ㅌ > 2.5 V, 0 E < 0 . 5 V.
     Complete the following tables corresponding to each part of the experimental data obtained
using logic 1 and 0.

                                             Table 3-lR.
                        /l
                                 B       U       1/
                                                           w         x       y




                                             Table 玉2R.
                             A       A       B        1V         x       y




                                             Table 3-3R.
                        』4
                                 B       U       V         F1/       x       Y




                                             Table 3-4R.
                        A        A       B       c         z         x       y




                                                 28

===== PAGE 45 =====
                                             Table 3-SR.
                      A       B      c       U        V     FI,    x       Y




DISCUSSION

1. For part 1, in terms of the variables A and B, what are the Boolean algebra equations at U, V,
   W,X, and Y? Express the DeMorgan relationship between A, B, X,and Y.




2.   For part 2, in terms of the variables A and B and the inputs to Gi, what is the DeMorgan rela-
     tionship between X and Y?




3.   Draw Karnaugh maps for X and Y to explain the outputs X and Y of part 2.




4.   For part 3, in terms of the variables A and B, what are the Boolean algebra equations at U, V,
     W, X, and Y? Express the DeMoIb. ' relationship between A, B, X, and Y. Draw a Karnaugh
     map showing the relationship between A, B, X, and Y.




                                                 29

===== PAGE 46 =====
5.   For part 4, in terms of the variables A, B, and C, what are the values at X, Y, and Z? Express
     the DeMorgan relationship between A, B, C, X, Y, and Z. Explain the circuit operation at
     point Z. (See discussion problem 5, experiment 2.)




6.   For part 5, in terms of the variables A, B, and C, what are the values at U, V, W, X, and Y?
     Express the DeMorgan relationship between A, B, C, X, and Y.




                                                30

===== PAGE 47 =====
                                                                          Experiment Li



111 NAND/NOR Gates-
Definitions ond Operation



OBJECT

      1
      上
       1
           To study the operation of the TTL gate.
      n
      ,
       1
           To determine the loading rules for the 'VFL gate.
      n
      J
       1
           To define the logic levels 1 and 0.
      4
      ~
       .
           To determine the noise immunity of the TTL gate.
      <
      J
       1
           To compare positive and negative logic.
      '
      b
       ,
           To study the effect of capacity loading upon TTL switching rates.


INTRODUCTORY THEORY


It is not essential to know the internal construction and component values within a gate (or IC).
Digital ICs are frequently treated as black boxes and correctly perform logic function, provided that
their operating rules are understood and followed. However, as the object of this experiment is to
study the operation and rules of the 54/74 TI'L (transistor-transistor logic) series of ICs, the sche-
matic diagrams of two types of 2-input NAND gates, types 7400 and 7403, are given in Fig. 4-1.
      Transistor Q1 has two emitters at inputs A and B. These operate as a 2-input AND gate. Tran-
sistors Q2 and Q3 perform the operation of inversion. Transistor Q2 acts as a driver for transistor
Q3, which is driven into saturation in the low-level output state. 虹F培．     及L  （치』 」？9，爻嘴共쁘ky희
으므虹畦」    브e trans雙얀으4-j§→드쁘0뜨an브欠므世世」              그j밍〕
                                                      너kγ힛， 으典)ut state Q4二conducts and acts as an
en典뜨r∼工QlJ vertopr으vide-a low塑｝        F足典프ce꼰utpu드 This is called an active pull-up. Diode D is
needed for biasing puipbsiTIiiThe high-level oiitput state, transistors Q2 and Q3 are cut off. In



                                                        3l

===== PAGE 48 =====
                                   VCC - +5V                                    VCC = +5V



                                                  130요
                                                  '




        B
      mPUTS


伊 oCeo)4j      e1緇W夕
       i*       훈거4      -b叫솩 . =            '\
      (a) 7400 Active (Trahsistor I Pull-Up                                     (b) 7403 0pen Collector
                                        Fig. 4-I. Type 7400 TFL 2-input NAND gates.




    Fig. 4-1(b), the collector of Q3 is left open-circuited. This is to allow a resistor to be connected
    from the collector of Q3 to Vcc (passive pull-up) and permit wired-collector* logic.
         Assume that input B is at i-S V and input A is held at a low level, for example, by another
    gate of the 54/74 series. Current flows through the 4-k&2 resistor and the base-emitter diode of Q1
    to input A. This current is sinked to ground through the output transistor of the grounding gate.
             翅塑盤，
    We d聊끄르沙吟」       8自璽：j흐쿄逾釀 A UL is sometimes expressed as an equivalent
                rr,n1』
     resistance referred to the supply vltage. However, there is a limit to the number of ULs that an
     output transistor can sink, determined by the gain of the output transistor and its associated cir-
     cuitry. If we attempt to make the output transistor, such as Q3, carry too heavy a current, it will
     come out of saturation, reduce ground-level noise immunity,t and may even make the gate ineffec-
     tive if the output voltage exceeds the threshold voltage (see the next paragraph) of the next stage.
     The maximum number of ULs a gate can drive is called maximum fan-out and is specified on the
     IC manufacturer's data sheet. For types 7400 and 7403, maximum fan-out is 10.
           Assume in Fig. 4-1 that input B is at +5 V and input A is at ground. With current flowing
     through the 4-kf2 input resistor, the voltage at point N at the base of transistor Q1 is a jQ홱e drop
     (+0.7 V) above ground. 駟工프뜨르nt工9j姮迎山B上으．             迦쁘읒르J2f{h4匣l岬4 mus므些쯔 恥，                y）
                                                                                                   으쁘 e
     grou닢 (VBc of Q1 + VBE of Q2 + VBF of Q3). If the input voltage at point A is madiiibre posi-
   ' {r石,point N will follow it but will be 0.7 V more positive until N reaches 2.1 V with A at 1.4 V.
     At걘쁘jPP埈v쁘age level,갇 1e threshold voltag. th c에虹tQ￡＝地筵각止迦J긔工m坦끄f=t& anf-the
     ilpllLemJtte-base diode A cuts 石ff with point N clamped at土2그그．Transistors Q2 and Q3 and
     VCB -of Q1 co冠而ronly I1i騙而百T而dl                 ［ㅍf百됴荻升；漲－threshold voltage, forming a 2-input
     NAND gate.
           IC gates frequently have to drive capacitive loads. Consider an IC gate such as the type 7403
     with resistor load driving a capacitive load shown in Fig. 4-2.

            *Experiment 2, part 4(b) and discussion problem 5.
            t5ee the discussion of the theory of noise immunity later in this experiment.

                                                              32

===== PAGE 49 =====
                                                   vCC




                                             (a) Output Circuit




                                             (b) Input Waveform

                                                                      -




                                                        -

                                         (c) Output Waveform
                                             At X (Inverted I With C=0




                                           (dl Output Waveform
                                               At X With C
                                  Fig. 小2. Ic gate with capacitive load.


      Figure 4-2(a) shows the output circuit. Figure 4-2(b) shows the input gate waveform. Figure
4-2(c) shows the output waveform [inverted from (b)J with the capacitor C = 0. Figure 4-2(d)
shows the output waveform with a capacitor. When Q3 is driven into saturation, it is at a low resis-
tance and discharges C, so that the voltage across C 勺 0. When Q3 is turned off, the voltage at X
can increase only as the capacitor C is charged through RL. How fast it will charge is determined by
the time constant RLC.
      For the gate to successfully drive another gate and cause it to switch, the voltage at X in Fig.
4-2(a) must rise above the threshold voltage for a following gate. If C is too large or the switching
rate is too fast, the voltage at X, as shown in Fig. 4-2(d), cannot reach the threshold voltage before
the next cycle arrives and the following gate will not have time to switch. To solve this problem, it
is necessary that the time constant RLC be reduced. This can be done only by reducing RL, but this
additional current into Q3 subtracts from the drive capability of the gate. TTL gates such as type
7400 with active pull-ups solve this problem, but active pull-ups do not permit wired-collector logic.
     Noise immunity, expressed in volts, is an important consideration in the design and choice of
logic circuits. Noise immunity is a measure of the ability of a logic circuit to prevent unwanted
noise signals from changing a desired logic level in response to the noise.
      Consider the case of one gate driving a second gate of the same IC logic family, as shown in
Fig. 4-3. Suppose that at A, the output of gate K, is high. This will make C, the output of gate L,



                                       )
low. Suppose that noise in the form of (1) electromagnetic coupling to the wire AB, or (2) electro-


                                   (        "               ,         B
                                   K>        A
                                                    I           __J       L   )
                                                                                  __




                               Fig. 4-3. ic NAND gate driving second gate.

                                                   33

===== PAGE 50 =====
static coupling to the wire AB changes the voltage at B. How great a change in voltage downward
can be tolerated before gate L is affected? The voltage at B can change to the point where the logic
level of gate L changes. We have previously discussed the input voltage at which a gate changes
from one level to the other and defined it as the threshold voltage. Similar factors must be consid-
ered when the output of gate K (point A) is at a low voltage, and in this case at least an upward
voltage change to the threshold voltage will cause the output of gate L to go through an undesired
change. To evaluate these factors an IC input/output transfer characteristic is obtained which has
the general shape shown in Fig. 4-4. This curve is applicable to both gates in Fig. 4-3.


                                              4- - V0ut (high)


                                  H＝ ㅇ ＞
                                                      Threshold voltage

                                                                   I- - V。
                                                                         ut (low)


                                                  I


                             Fig. 牛4. Transfer characteristics of gates of F自g. 4-3.

    From this curve we can determine the noise immunity, which is expressed in the following
equations.
                         high-level noise immunity = VOut(high) - Vtbr四hOId             (4.1)
                              ground-level noise immunity = Vthr驪hOld - VOut(low)                      (4-2)

Voltage changes in excess of these values will affect the output logic levels.


EQUIPMENT REQUIRED


      CRO, dc coupled and calibrated; all voltage measurements are to be made with the CRO; two-channel is
advisable
     Square-wave generator (SWG); positive-going S V at 10 to 50 kHz; 500- 2 output impedance (max.)
     dc power supply, regulated to +5 V at 100 mA
     dc milliammeter, 2 mA
     Capacitor, 0.033〃F
     Capacitor, 0.01 pF
     IC type 7400 quad 2-input NAND gate
     IC type 7403 quad 2.input NAND gate, open collector
     500-cl, 3-turn, 5-W potentiometer
     1000-cl 10% composition resistor
     5.6-kcl 10% composition resistor
     Miscellaneous composition resistors from 100 17 to 10 kcl

                                           IC manufacturers' part numbers.

                                                                     Texas         National
                 Type        Motorola           Fairchikf        Instruments     Semiconductor

                 7400        MC7400P             7400PC           SN7400N              DM7400N
                             MC7400L             7400DC           SN7400J
                 7403        MC7403P             7403PC           SN7403N              DM7403N
                             MC7403L             7403DC           SN7403J


                                                          34

===== PAGE 51 =====
IC LOGIC DIAGRAMS


The logic diagrams, base pin connections, and loading rules for the 7400 IC and 7403 IC are shown
in Fig. 4-5. Note that:

      l.   The input loading is 1 UL. This is shown in parentheses next to each input.
      2.   The maximum fan-out is 10 UL. This is shown in parentheses next to each output.




            ;,;21，’
            (1)  긔-I )－《1.)
                        (10) (1),91。
                                   긔 )--8 (10)
            (1) 4                                                   (1) 12
                                                                                               11 n0)
            (1) 5                                                   (1) 13
                                   vcC = +5Volts to Pin 14
                                   0 (ground) to Pin 7

                               Fig. 小5. Logic diagram, pin connections, and loading rules
                                        for types 7400 IC and 7403 IC.


EXPERIMENTAL PROCEDURE


Connect pin 14 to +5 V and pin 7 to 0 (ground) for all ICs in this experiment.



1.   The Gate as an Inverter


             +5   1
                  U
                  찧
                  U
                  ＼
                                                                                       CRO vertical
                                                                                         1 V/div
             l.
                                           Fig.4-6. The gate as an inverter.


Make the measurements at the terminal indicated to complete Table 4-1E.

                                                            Table 4-1E.

                                               Voltage αr           Voltage αr
                                                 Pin /                ^n 3

                                                        0

                                                   +5
                                                               35

===== PAGE 52 =====
2.    Gating Action



     +5V

             《－          '        《，                           .                 740
                                                                                              CRO vertical
                                                                                              1 V/div
      I난－-
                                                          Fig. 4-7. 2-input gate.



       (a)   Make the measurements at the terminals indicated to complete Table 4-2E.


                                                                   Table 4-2E.

                                          Voltage αr Pin                     Voltage αr Pin
                                                    1               2              3
                                                    0               0
                                           +5                       0

                                                    0              +5
                                          +5
                                                                   +5



       (b)   Make the measurements at the terminals indicated to complete Table 4-3E. An (a)
             in this table means that the terminal indicated is to be disconnected from the switch
             of part 2(a) and the terminal is to be left floating.



                                                                   Table 4-3E.
                                          Voltage αr 月n                      Voltage αr Pin
                                                    1               2              3
                                               +5                  +5
                                               +5                   a   .




                                                    a
                                                                   +5
                                                    a               a


                                                        αDisconnected and floating.


3.     Loading Rules


       (a)        Determination of a UL. Measure the current in the circuit of Fig. 4-8.

                                                          I=                      mA

                                                                        36

===== PAGE 53 =====
                                                                             To CR0




                                        Fig. 小8. UL determination.


     (b) From the data of part 3(a), calculate the resistance of a UL referred to +5 V.

                                         R1UL =                n

     (c)    From the data of part 3(b), calculate the equivalent current and resistance corresponding
            to 10 UL. This corresponds to the load a gate output would see if it were driving 10 gate
            inputs. DO NOT PROCEED until you have checked your answer with the instructor.




     (d)    Increase the CRO vertical gain to 0.1 V/div and carefully measure the voltage at pin 3 in
            the circuit of Fig. 4-9.

                                   voltage at pin 3 =                volts




               卜4伊_
      +5V
                                                                                      CR0 vertical
                                                                                       0.1 V/div




                                 Fig. 4-9. Measurement of 이it1川．
                                                               t voltage.


     (e)    Repeat the measurement of the votta8e at pin 3 but with a resistor equal to 10 UL con-
            nected between +5 V and pin 3. Use a composition resistor having the nearest 10% value
            to the value calculated in 3(c).

                                   voltage at pin 3 =                volts


4.   Transfer Characteristics

     (a)    The transfer characteristic is a curve showing the output voltage plotted against 후he input
            voltage. The transfer region is quite sharp and narrow, and careful measurements have to
            be made to obtain accurate results tor a smooth curve. Ifl making tne measurements on
            the CRO, set the zero line on the CRO to allow a vertical deflection of at leastl5 vertical
            divisions and use the VERT sensitivities shown in Fig. 4-10. Measure voItage今 to within
            0.1 V.

                                                        37

===== PAGE 54 =====
         +5V                                                                             0       CR0 vertical
                                                +5V (VCC)
                                                                                                  1 V/div




                                                     _
                                            5.6 kf




                I
500 cl
3 turn
                                        7403)                                                     CRO vertical
                               小                                                                    1 V/div


                  >0.033pF
                 口：
                                    〃   ?       0
                                                 1
                                                     1
                                                     0   ㄷ
                                                         ～
                                                                                             Note: Capacitors are used to prevent
                                                                                                   parasitic oscillations. Keep
                                                                                                   leads short.

                               Fig. 4-10. Measurement of transfer characteristics.


(b) The following procedure is suggested in obtaining the data. Set the potentiometer in
    Fig. 4-10 to 0 V and measure the output voltage at pin 3. Now adjust the potentiometer
    to give an output voltage at pin 3 equal to approximately half the output voltage just
    obtained. Measure the input voltage at pin 1. Tabulate this set of input/output voltages
    in Table 4-4E and plot the point on Fig. 4-1 1. Vary the input potentiometer both above
    and below this mid-output voltage point and determine the maximum and minimum out-
    put voltages. Now vary the input potentiometer to obtain four approximately equally
    separated output voltage points between the midpoint and the maximum output voltage
    and four equally separated output voltage points between the midpoint and the mini-
    mum output voltage and measure the input voltage at each point. For each point plot it
    on Fig. 4-1 1 and tabulate the data in Table 4-4E. Complete the data by varying the
    input potentiometer so that the curve covers the complete input voltage range from 5 V
    to 0 V. Do not proceed until your instructor has approved your data and plotted curve.



                  Table 수4E.
                                                                                    5 ■■■■■1■■■■■■■■■■■■■1■■■■■
               Vpin /     Vpjp 3                                                        ·■u■■■1..■■1■1■.■..■.....
                                                                                        ■1■■■■■■■■■■■■■■·■■1■·■■■
                                                                                        ■·■■■■■·■1■■■■1■■■■■■■■■·
           Input         Output                                                     4 ■iu1u.   1u....uu. 1■u■uui■■




                                                                          ㄸ ― ＝ㅇ＞
                                                                                      ■■u■u■■■■u■uu■uuuuu■■■1■
           Voltage       F'oltage                                                     ■■■■■■■■■■■■■■1■■■■■■■■11




                                                                     > -m 드
                                                                                      1■■■■■■■■■■■■■■■■■■■■■■■·




                                                                  "= 0
                                                                                      .........................
                 0                                                                    ■■■■■．■■■1■■■■■·■·■■■■니■■■
                                                                                    3 .........................
                                                                                        .........................
                                                                                        ..u. .....................
                                                                                        ■■■■■1·■■■■·■11■■■■■■■■■■
                                                                                    ^
                                                                                         ■■■u■u1u1u■uuu1u■1■■u■■u
                                                                                    Z
                                                                                        ■uu.■■■■■■u■■u■u· ■uuuuuu
                                                                                        ■■■■■■■·1■1■■■■■■■■■·■■■■
                                                                                        口■■■■■■■1■■111■■■■■■■■■■■
                                                                                        ■■■■■1■■1■1■■■■1■■■■■·■■■
                                                                                        ■1■■■■■1■1■1■■■■■■1·■■■■■
                                                                                        ■■■■■·■■■■■■■■■■■1■■■■·■1
                                                                                        ■■■1■1■1■■1■1■■■■■■■■■■■■
                                                                                        ■■■■■■■■■■■■■■·1■■■■■■■■■
                                                                                        ·口·■■■1■■1■■■■■■■■■1■■■■1
                           2.5                                                                          .u. iuu
                                                                                    0 ■u.■■u■uuu.1u■auuu. 4
                                                                                     0     1   2     3         5
                                                                                                   Vin - Pin 1 - Volts

                                                                                        Fig. 4-I L Transfer characteristics.



                +5


                                                             38

===== PAGE 55 =====
                                                                                      O CRO vertical
                                                                                          1 V/div
                                                                                ―
                                                                                      O dc coupled
                                                                    +5V (Vcc)

                                                                       ㅗ
                                                                                손
                           To CRO
                        EXT TRIG NEG


                            l
                                              5.   6k                               5.6 k2

       SWG         n
       +5V         -                         , 3.        '                            O CRO vertical
                                                                        7403B
10 kHz to 50 kHz 0- ~-                                                                    1 V/div
                                   智3
                                                                                      0  dc coupled

                                                    T       C
                                                         0.033p F


                                        Fig. 4-12. Capacity loading.

    Pull-Up Resistors

In Fig. 4-12 the square-wave generator(SWG) rapidly switches gates A and B, alternately turning
the collector currents of Q2 and Q3 (see Fig. 4-I) on and off. Adjust the output of the SWG to
provide a positive-going 5-V peak signal at a frequency of 10 kHz. Adjust the CRO horizontal
sweep rate so that each cycle of the SWG occupies two horizontal divisions.
    (a) Disconnect the 0.033-MF capacitor shown in Fig. 4-12 to make C = 0. Adjust the CRO
        sweep and triggering so that a steady pattern of approximately five cycles is obtained.
        Use external triggering for the CRO from the square-wave generator as shown in Fig.
        4-12. Sketch the waveform at IC output pins 3 and 6 on Fig. 4-13.
    (b) Connect the 0.033-pF capacitor as shown in Fig. 4-12. This value of capacity is intended
        to simulate the effects that would occur if gate A and gate B were some distance apart
        and the connection between gate A and gate B was a long cable. The 0.033-zF simulates
        the cable capacity.
              Refer now to Fig. 4-1. When Q3 is conducting and in saturation, pin 3 of gate A is
        at ground potential. When Q3 is quickly made nonconducting by the SWG,the output at
        pin 3 cannot go to Vcc immediately, since the 0.033-iF capacitor has to charge up to
        VCC through the 5.6-kfl load resistor of Q3. This is determined by the time constant of
        the 5.6-kf2 resistor and the 0.033-'zF capacitor.
              Sketch the waveforms obtained at pins 3 and 6 on Fig. 4-13. The waveform should
        show the peak voltage reached at pin 3.
    (c) Increase the frequency of the sWG until the waveform at pin 6 just disappears. Sketch
        the waveform at pins 3 and 6 on Fig. 4-13. The waveform should show the peak voltage
        reached at pin 3.
    (d} Connect a 100042 composition resistor between pin 3 and Vcc. This is called a pull-up
        resistor. A pull-up resistor is a resistor connected from a point to the positive supply
        voltage. Sketch the waveforms at pins 3 and 6 on Fig. 4-13. The waveform should show
        the voltage reached at pin 3.




                                                        39

===== PAGE 56 =====
                  +5
     Part 5 (a)
       F기ri ;3
                              0

                  +5
     Part 5 (a)
      Pin 6
                              0

                   -*5
     Part 5 (b)
      Pm ;3
                              0

                       +5
     Part 5 (b)
       Pin 6
                              0

                         +5
     Part 5 (c)
      Pin 3
                              0

                       +5
     Part 5 (c)
      Pin 6
                              0

                       +5
     Part 5 (d)
       Pin 3
                              0

                         +5
     Part 5 )d(
       Pin 6
                              0
                                             Fig. 4-13.



REQUIRED RESULTS


Note: When Required Results sections are numbered, the problem numbers correspond to the sec-
tions in the experimental procedure.
I.    Using logic values I ㅌ > 2.5 V and 0 三 <0.5 V and based on the data of Table 4-IE, complete
      Table 4-1R. The table should have Is and Os.

                                              Table 4-1R.

                                            pin j         /in 3




                                                    40

===== PAGE 57 =====
2. (a)     Using logic values I 三 > 2.5 V and 0 = <0.5 V for positive logic and based on the data of
           Table 4-2E, complete Table 4-2Ra. The table should have is and 0s.

                                                Table 牛2Ra.
                                        /in /      /in2       /in了




     (b)   Using logic values 1 三 <0.5 V and 0 E> 2.5 V for negative logic and based on the data of
           Table 4-2E, complete Table 4-2Rb. The table should have is and 0s.

                                                Tabk 4-2Rb.
                                        Pin 7     ／和
                                                   ＇2         Pin 3




     (c)   Using logic values 1 = > 2.5 V and 0 = <0.5 V and based on the data of Table 4-3E,
           complete Table 4-3R. The table should have Is and 0s.

                                                Table 4-3R.
                                        Pin I      Pin2       /in 3


                                                      a

                                          a

                                          a           a




DISCUSSION


I.   Based on the data of Table 4-1R, draw the logic symbol for the gate operation between pins 1
     and 3. (Omit power supply pin connections.)




2.   (a)   Explain, using the data of Tables 4-2E and 4-2Ra (positive logic), what type of gate this
           is. Draw the logic symbol representing its operation. Write the Boolean algebra equation
           for the circuit using the pin numbers as the Boolean variables.


                                                 4l

===== PAGE 58 =====
     (b) Explain, using the data of Tables 4-2E and 4-2Rb (negative logic), what type of gate this
         is. Draw the logic symbol representing its operation. Write the Boolean algebra equation
         for the circuit using the pin numbers as the Boolean variables.




3.   Based on the data of Tables 4-3E and 4-3R, what logic value, 1 or 0, does an uncon;nected
     input assume (positive logic)?




4.   From a study of the IC circuit diagram of Fig. 4-1, compute tile curfent that would flow
     through the emitter of input A if A is connected to ground. Compare witil ,'cur eXPeiimental
     data obtained in part 3(a).




5.   Using transistor theory, why is the voltage measured in part 3(e) different from that in part
     3(d)?




6.   Referring to the graphical data of part 4 and Fig. 4-1 1, at what voltage applied to pin 1 does
     the voltage at pin 3 change most rapidly? Explain the reason for this value based on a study of
     Fig. 4-1.




7.   The questions in this section are based on noise immunity and the data of part 4. Carefully
     study the theory on noise immunity before answering the questions. Use the data of Fig. 4-1 1.
     (a)   What gate input voltage applied to pin 1 corresponds to the middle of the sharp transi-
           tion region of the gate output voltage of pin 3? (See Fig. 4-Il.) Call this the threshold
           voltage.




                                                42

===== PAGE 59 =====
    (b) What is the high-level noise immunity? Show calculations.




    (c)   What is the ground-level noise immunity? Show calculations.




   (d) Assume a minimum allowable ground-level noise immunity of 0.5 V. Based on the thresh-
       old voltage of Fig. 4-1 1, what is the maximum possible voltage for the 0 voltage level
       (positive logic)? Show calculations.




   (e)    Assume a minimum allowable high-level noise immunity of 0.5 V. Based on the threshold
          voltage of Fig. 4-1 1, what is the minimum possible voltage for the 1 voltage level (positive
          logic)? Show calculations.




8. These questions refer to the data of part 5.
   (a) Explain the waveforms at pins 3 and 6 for part 5(a).




   (b) Explain the waveforms at pins 3 and 6 for part 5(b). (Hint.' Consider the effect of the
       0.033-'zF capacitor.)




                                                 43

===== PAGE 60 =====
    (c) Carefully examine the amplitude of the wave shape at pin 3 for part 5(c)and compare it
        with the transfer curve and IC threshold voltage of part 4 and Fig. 4-1 1 of the experi-
        ment. From this, explain why the pattern at pin 6 disappeared.




   (d) Explain the wave shapes of part 5(d). Why did the pattern reappear?




    (e) What is the function of a pull-up resistor?




    (f) How many ULs does the l000- 2 pull-up resistor represent? With this pull-up resistor in
        the circuit, how many additional ULs can this IC drive?




    (g)   What are the advantages and disadvantages of a pull-up resistor?




9. Figure 4-12 is the logic diagram of a 2-input NAND gate followed by an inverter. Write the
   Boolean equation for Fig. 4-12 for positive logic. Write the Boolean equation for Fig. 4-12 for
   negative logic. This is to describe circuit operation between input pins 1, 2, and output pin 6.
   Discuss the reasons for your answers.




                                                44

===== PAGE 61 =====
                                                                    ExperimenI 5



The'tExcIusive-OR"
and fts ApplicaEions



OBJECT


  1. To study methods of generating the exclusive-OR function.       3. Binary comparators.
  2. The half-adder and half-subtractor.                             4. Parity generators.


INTRODUCTORY THEORY


The exclusive-OR (EOR) is a logic block that compares 2 bits of data. When the bits are alike, the
EOR output is a 0; and when the bits are not alike, the EOR output is a I. With inputs A and B,
the EOR equation is Eq. 5-1.

                                    EOR= AB+ AB= AB+ AB= AC)B                                     (5-1)

Although there are many ways of implementing the EOR, they can all be shown to reduce to one of
the forms of Eq. 5-1.
     The EOR has important applications in arithmetic and in data-checking circuits such as parity
generators and comparators.


EQUIPMENT REQUIRED


     CRO,dc and calibrated                                 IC type 7404 hex inverter
     dc power supply, +5 V at 50 mA                        IC type 7420 dual 4-input NAND gate
     IC type 7400 quad 2-input NAND gate                   IC type 7486 quad exclusive0R gate
     IC type 7402 quad 2-input NOk gate                    Two switch banks,5 switches per bank

                                                    45

===== PAGE 62 =====
                                         IC manufacturers'part numbers.
                                                                               Texas      National
                1pe            Motoroh              Falh'hild              Instrumen心   Semiconductor

                7400       MC7400P                  7400PC                  SN7400N       DM7400N
                           MC7400L                  7400DC                  SN7400J

                7402       MC74O2P                  74O2PC                  SN7402N       DM7402N
                           MC7402L                  7402DC                  SN7402J

                7404       MC7404P                  7404PC                  SN7404N       DM7404N
                           MC7404L                  7404DC                  SN7404J

                7420       MC742OP                  7420PC                  SN7420N       DM7420N
                           MC7420L                  7420DC                  SN7420J

                7486                                 7486PC                 SN7486N       DM7486N
                                                     7486DC                 SN7486J



EXPERIMENTAL PROCEDURE


For all ICs in this experiment: VC = +5 V to pin 14, 0 (ground) to pm 7.
     General: For each part of the experiment, wire the circuit shown. Make voltage measure-
ments at the points designated to complete the tables.


1.   Exclusive-OR Generation


      (a)
 +5 V


            A      B
     I:0→
                                         Fig. 5-1. Exclusive-OR generator.


                                                         Table 5-IE.

                                            A            B             x         x

                                                0             0

                                                0        +5
                                           +5                 0
                                                         +5
                                           +5
                                                                  46

===== PAGE 63 =====
山）




          Fig. 5-2. Exclusive-OR generator.


                             Table 5-2E.

                        A           B       x

                         0              0

                         0         +5

                   +5                   0

                   +5              +5
(c)
      《
          ng. 5-3. Exclusive-OR generator.



                             Table 5-3E.

                    J4             B        x

                         0              0

                         0         +5
                   +5                   0

                   +5              +5


                              47

===== PAGE 64 =====
(d)                                                                                                                                   Table 54E.

                                                                                                                        /l
                                                                                                                                            B      x

                                                                                 －∼＼
                                                                                                                             0              0
                                                                  -                7486              )-X
                                                                        ＼`
                                                                   】                        \3
         " '                                            O         Z      .                       I                           0              +5
                       ㅈ：-
                                                                       ／낟
                                          A             B
                                                                                       겯／
                                                                                                                        +5
                                                                                                                                            0
               -[-O-                          -c

                                                                                                                        +5
                                                                                                                                            +5

                                              Fig. 5-4. Exclusive-OR gate.


2.    Half-Adder, Half-Subtractor


Since the half-adder and half-subtractor require the exclusive-OR as part of their logic, any config-
uration of part 1 could be used. The simplest is used in part 2.

      (a)    Half-Adder, X + Y



                                                                                                 2   )
                                                                                                 1V1巨〉
                                                                                                     7486           3




                                          t: _
                                                                                                             740》                ＞2
                                                                                                             7400
                             "        v
                                              x             Y


                                                                             Fig. 5-S. Half-adder.
                                 I→                －O
                                                                                       Table 5-SE.

                                                                        x                   y            S     c

                                                                             0              0

                                                                             0         +5
                                                                       +5                   0

                                                                       +5              +5
       (b)   Half-Subtractor, X - Y




                                                                                   ;)L9_"_
                                                                                  ,p
                                                                              7400,
                                                                                                              7400)                    ]i
                                                                                                                                                 74。
                                                                                                                                                   。)B。



                                                                       Fig. 5-6. Half-subtractor.

                                                                                            48

===== PAGE 65 =====
                                                                                       Table 5-6E.

                                                                         x                  Y                       z)             Bα
                                                                              0             0
                                                                              0        +5

                                                                     +5                     0
                                                                                       +5
                                                                         +5
3.   Binary Word Comparator




                                                                                                2)             ,
                                                                                                                    74   二＞             3   i>   2-
 +5 V
                                                                                            4j                                          6 “〕
                                                                                                                                         "必 광
                                                                                                                                                           4   7420   P-   X
                                                                                    12
     A3           A2        A1                 A0
                                                                                                                                                      소．
        《）
        I： - c               c                     p                                13
                                                                                                          1/ 7486
                                                                                                          \\ 74D " "; 7404 10




                                                                                                                    74D" "
                                                                                                                         ＞肛
 +5Vi,r82g:ㅈB1＝-Bfl_
                                                                                                     I,
        I:   0-    c-   -        c-            -   p

                                                             Fig. 5-7. Binary word comparator.




Set A3, A2, A1, and A。 -the first binary word-to the values given in Table 5-7E and experimentally
determine the values of B3, B2, B1, and B。to make X < 0.5 V.


                                                                                  Table 5-7E.

                                      d3            계2         시                  계0                           B3             B2            B/   〃0
                                           0             0           0             0
                                           0        +5
                                                                +5                 0
                                      +5
                                                    +5          +5                 0
                                           0             0           0            +5

                                      +5                 0     +5                  0

                                                                                            49

===== PAGE 66 =====
4   Parity Generator



                                                                                                 7486




    +5Vp- -- o--- -o                                o_                                                  11

       B4>   -    83b-            B2
                                                                                             I

         r             -
                           -－∼→
                                                                            0




Set the binary word B4, B3, B2, B1, and B。to the values given in Table 5-8E and record the voltage
at X

                                                         Table 5-8E.

                                   B4      B3            B2            B1       B0       x

                                       0        0             0             0        0

                                       0   +5                 0        +5
                                                                                     0

                                   +5           0        +5                 0   +5
                                       0   +5            +5            +5            0

                                   +5      +5                 0        +5       +5
                                   +5           0        +5            +5       +5
                                       0   +5                 0             0        0

                                       0        0             0             0   +5



REQUIRED RESULTS


Assuming positive logic, complete the following truth tables based on the experimental data ob-
tamned for the corresponding parts. Use 1 ㅌ > 2.5 V and 0 ㅌ <0.5 V.




                                                                  50

===== PAGE 67 =====
                           Table 5-1k.                                           Table 5-2R.
                                         无
                  A                               x                         」4
                                                                                          B        X




                           Table S-3R.                                           Table 54R.
                       A             B       x                              A                     I




                           Table 5-SR.                                           Table 56R.
                  4        f1            S        c'
                                                                       x         y            D        B0




                                                       Table 5-7R.

                      계3        」2
                                             계＇        』40        B3       β2        B/
                                                                                                  B0




     Complete Table 5-8R for the experimental data. En the column marked T, total the number of
Is in the binary word B4, B3, B2, B1, B0. In the column marked P, indicate the parity of the word
"ODD"' or "EVEN."



                                                             Sl

===== PAGE 68 =====
                                              Table 5-8R.
                                                                        P,
                                                            T,
              B4      B3      B2     B1      B0        Tbrα／ is   《7z)f) (7' fyEN    x




DISCUSSION


1.   How does the circuit in part 1(a) using Fig. 5-1 generate the exclusive-OR function? Discuss
     particularly with reference to the inputs to G3.




     Show that the circuit of part 1(b) using Fig. 5-2 is the equivalent of Eq. 5-1 and thus generates
     the exclusive-OR function. (Hint: Use DeMorgan's theorem for the outputs of G1 and G2, and
     draw a Karnaugh map.)




3.   Show that the circuit of part 1(c) using Fig. 5-3 is the equivalent of Eq. 5-1 and thus generates
     the exclusive-OR function. (Hint.· Determine the inputs to G3 and draw a Karnaugh map.)




4.   Write out a truth table for a half-adder and compare wi.h the results of Tables 5-5E and 5-SR.
     Discuss.




                                                  52

===== PAGE 69 =====
5.   Write out a truth table for a half-subtractor and compare with the results of Tables 5-6E and
     5-6R. Discuss.




6.   Explain the circuit operation of the binary word comparator of part 3. Refer to your experi-
     mental data. If necessary, write a truth table.




7.   Discuss and explain the circuit operation of the parity generator of part 4. Refer to your ex-
     perimental data comparing columns T, P, and X from Tables 5-8E and 5-8R. (Hint: Establish
     a pattern for parity generator outputs in the following manner. Assume that you have a 2-bit
     parity generator. Determine its output. Now do the same for a 3-bit system and a 4-bit system
     and then generalize.)




8.   Why do we need word comparators and parity generators? Which parity is preferable, odd
     or even?




                                                53

===== PAGE 70 =====
     '...    구．
              ’卞“／닒   긷        f,,            1.y죠 r `;   ＼슥뇨．


峯：客 ,－· ：可／/「
            ［$J'「靷，亭쵯4\               *   d      ` `
                                          「     *〃 뇨




      $i,,：노
           「 :：」·
               －스…交盼
        r   .'r섭          4"         ．수쌉 ‘布芝뇨뇨

       l샌욹        ,亡숯1" 蕣：r秀甚騏玎' ,.1. ,-
       番轟꼇1   （坪多璡締” 動拉懈．     裡亨沙三i．  茗／/
       "j「k；∼e; ':.lr 滓.

===== PAGE 71 =====
                                                                Experiment6



F애-Adder and F예-Subtrackor




To study methods of generating circuits that perform the arithmetic operations of full addition and
full subtraction.


INTRODUCTORY THEORY

The full-adder and full-subtractor are the logic blocks that add or subtract 3 data bits. These logic
blocks can be implemented by directly following the logic equations for addition or subtraction.
However, this is not always the most convenient way of performing these operations. Although the
sum S and difference D logic basically cannot be reduced by Boolean algebra, it is possible to mod-
ify it. One way to do this is by the same exclusive-OR (EOR) circuitry with the sum S = A o B 0 C;
and the difference D = X o Y GI B1. The carry-out C。and borrow-out B。logic differ and can be
reduced with Karnaugh mapping. Complete addition for S and C。can be performed with 2 half-
adders and complete subtraction for D and B。with 2 half-subtractors. Since there is a difference in
the logic for C。and B。   , multibit subtraction is frequently performed by complement addition to
reduce the number of logic blocks required in arithmetic operations.


EQ(기PMENT REQUIRED

     CR0, dc and calibrated                            IC type 7410 triple 3-input NAND gate
     dc power supply, +5 Vat 50 mA                     IC type 7420 dual 4-input NAND gate
     Two switch banks, 5 switches                      IC type 7483 4-bit full-adder
     IC type 7400 quad 2-input NAND gate               IC type 7486 quad exclusive-OR gate
     IC type 7402 quad 2-input NOR gate                Five 68042 n0% resistors
     IC type 740사tex inverter                          Five red LEDs

                                                 55

===== PAGE 72 =====
                                           IC manufacturers'part numbers.

                                                                     7exas           Natfonal
                   Type         Motoro幻           Fairchild       Instruments     Senm?onαuctor

                   7400         MC7400P            7400PC          SN7400N          DM7400N
                                MC7400L            7400DC          SN7400J

                   7402         MC74O2P            74O2PC          SN7402N          DM7402N
                                MC74O2L            7402DC          SN7402J

                   7404         MC7404P            7404PC          SN7404N          DM7404N
                                MC7404L            7404DC          SN7404J

                   7410         MC74 lop           7410PC          SN74 iON         DM74 ION
                                MC7410L            74 IODC         SN74IOJ

                   7420         MC742OP            7420PC          SN7420N          DM7420N
                                MC7420L            7420DC          SN7420J

                   7483         MC7483P            7483PC          SN7483N          DM7483N
                                MC7483L            7483DC          SN7483J

                   7486                            7486PC          SN7486N          DM7486N
                                                   7486DC          SN7486J


EXPERIMENTAL PROCEDURE


For each part, wire the circuit shown and make voltage measurements at the points indicated to
complete the table.


1.   SUM in Full-Adder and DIFFERENCE in FuII-Subtractor


       S for X + Y + Ci




                                                                                  ）粥＞ )
       D for X - Y - B1


     a. ／기recrLogic



                                                                         n
                                                                         口
                                                         2




                                                             1_
                                             1>
                                 →－
                                                  7404
                                                                  d4 5
                                                                             기




                                                                       …
                                                                       巴
                                                                       。
                                                                       나
                                                                             M

                                                                                                              M

                                                                             'M                  므
                                                                                                 ―
                                                                                             2
                                                                      구禪


 " '   t《．            亡．
                                                                             쟤
                                                                                             -
                                                                                             -
                                                                                           Vcc = +5 V to pin 14
                                                                                           0(ground) to pin 7

                           Fig. 6-I. SUM in full-adder and DIFFERENCE in full-subtractor
                                     following Boolean equation 小rect logic.

                                                             56

===== PAGE 73 =====
                                              Table 6-IE.

                            Va緻ble                   J             X    L        ^f

                            Full-Adder               x             y    ci       S    8
                            Full-Su加ractor           x             y   易         D    g
                                                     0             0         0

                                                     0             0    +5
                                                     0        +5             0

                                                     0        +5       +5

                                               +5                  0         0

                                               +5                  0   +5

                                                +5
                                                              +5             0

                                               +5             +5        +5
b. fxclusivHㅍ）/? L四ic




           +5 V




              I
                        0              O                 0




                  Fig. 6-2. SUM in full-adder and 이FFERENCE in full-subtractor
                            with exclusive-OR logic.

                                              Table 6-2E.

                            Variable                J         K        L         ^f

                            Full-Adder              x              Y   ci        S

                            Full-Subtractor         x              y   易         Z)




                    x
                                                     0             0         0

                                                     0             0   +5

                                                     0        +5
                                                                             0

                                                     0        +5       +5
                                               +5                  0         0

                                               +5                  0   +5
                                               +5             +5             0

                                               +5             +5
                                                                       +5


                                                         57

===== PAGE 74 =====
2.   C。for Full-Adder


     C。for X + Y + C1

                                                                                                       \3
                                                                                                7400
                                                                                       2
                                                                                                        /)-
                                                                                                        \6        4
                                                                                                7400          ㅇ
                                                                                                       /

     '"'《 ㅋ，＝二
             《_                                                                                 7400
                                                                                                              8



                                                                                                                  Vcc = +5 V to pin 14

       I［크）    --<)     -－心
                                                                                                                  0 (ground) to pin 7




                                                               Table 6-3E.

                                             x                      y         (?   '       C。
                                                 0                  0              0
                                                 0                  0        +5

                                                 0             +5                  0
                                                 0             +5            +5
                                            +5                      0              0
                                            +5                      0        +5

                                            +5                 +5                  0
                                            +5                 +5            +5
3.   Full-Adder with Half-Adders
                                                               Table 64E.
      x + Y + C1
                                   x                       y            G              S          C。
                                        0                  0            0
                                        0                  0            +5

                                        0            +5                 0
                                        0            +5                 +5

                                   +5
                                                           0             0
                                   +5                      0            +5

                                   +5                +5                  0
                                   +5                 +5
                                                                        +5


                                                                        58

===== PAGE 75 =====
                                                      1             ＼흐 슨，
                                                                        ,, 2 _
                                                    ㅓ      ' " ""        0-          74o4   Q




                                                                                                             ,/cc= +5 V to pin 14
                                                                                                             0 (ground) to pin 7
     l:
               o-              o-
                                      -        p


                                                                                                      HA 2

                                                   Fig. 6-4. Full-adder with half-adders.

4.        2-Bit Parallel Binary Adder


               x1x0 -               x1    x0
          +Y1Y。                     +Yi   Yo
                SUM         C。
                             1 S1         So

Note: "+" here means addition.



                                                                        \b/
                                                                                            C。
                                                                                             o
                                                                                                                      一



            +5 V
                                                          74

                        0
                             尸      ㅜo                              沕
                                                                                                 13
                                                                                                        加
                                                                    ／
                                                                                                                                  1
           F
           U        V




                             尸      Y1




                                                                              ｀아이／
                            ,/cc = +5Vto pin 14
                            0(ground) to pin 7                                                                               Si
                                                    Fig. 6-5. 2-bit parallel binary adder.

                                                                         59

===== PAGE 76 =====
(a)   The circuit of Fig. 6-5 is that of a 2-bit parallel binary adder, which performs the addi-
      tion X1 X。plus Y1Y。= C。     1 S1 S。when the numbers X1X0, Y1Y0, and the sum C。      1 S1 S0
      are expressed in binary notation. Table 6-SE has two sections, an Experimental Data sec-
      tion for laboratory data and a Binary Equivalents section for checking the experimental
      data against actual binary numeric addition. Each row of Table 6-5E must be completed
      before proceeding to the next row. Make voltage measurements at the indicated points
      of Fig. 6-5 to complete the Experimental Data section.
            The Binary Equivalents section of Table 6-SE must now be completed. Using posi-
      tive logic, 1 三 > 2.5 volts, and 0 = <0.5 volt, express the numbers X1X。and Y1Y。in
      binary notation. Now, actually add them numerically and enter the sum as Sc (Sum Corn-
      puted) in the SC column. Now express the sum SE = C。       1S쵸 So (Sum Experimental) from
      the Experimental Data section in the SE column in binary notation. Sc and 5E should
      agree. If they do, proceed to the next row. If they do not agree, call the instructor.


                                                                       Table 6-SE.

                                                                                             Binary Equivalents
                          Experimental Data                                                 (in Binary Notation)
                                                                                                                   c。lSlso
                                                                                                     치兀7           (experi-
            Xl   xo        y/       yα            c〃        SI   옥그1
                                                                                     치xo    y／γ0   plus Y1 y0      memα／7

                                                                                                        Sc           SE
             0        0         0   0
            +5   +5
                           +5
                                    +5
            +5        0    +5
                                    +5
             0   +5
                           +5       0



(b)   Complete the experimental data in Table 6-6E.



                                                                       Table 66E.

                                         xl            xo              》가
                                                                                y0         q汀      SI        So
                                a             0             0               0   +5
                                b             0        +5
                                                                            0   +5
                                c             0        +5              +5       +5
                                d        +5                 0          +5            0
                                e        +5
                                                            0          +5       +5
                                                                 60

===== PAGE 77 =====
5.   4-Bit Binary FuU-Adder/2's-Complement 4-Bit Binary FutI-Subtractor

                                                                                                                                       1-5 V
The 7483 is an MSI 4-bit binary full-adder. It adds(+ means addition)
                                                                                                                                         -

                                                                              q시民 阮
                         Co                                                                          carry-rn (bit 0)
                                                        시

                                                                  AB S
                         i-A              A3
                         +B            s- B3           B2
carry-out (to bit 4) -p          c4        S3          S2


                                                                                                                             Fig. 6-6. LED polarity test.


     The sum or difference will be displayed by means of the LEDs (light-emitting diodes) in
Fig. 6-7. Before connecting the LEDs into the circuit of Fig. 6-7 check each LED-resistor combina-
tion for correct LED polarity by placing it across the 5-V supply as shown in Fig. 6-6. Then con-
nect them into the circuit of Fig. 6-7.




                                                                                                                        +   ㅗ                        瞰
                                                                                                                                                     渤
                                                                                                                                                                FU   V
                                                                                                                                                         枕

                                                                                                                        /
                                                                                                                        '
                                                                                                                                                                r




                                                 +5 V


                                                                                                                                           /11
                                                                                                                                                             的ㅗ ，




갸
         +5 V                                          5                      12




     d긱긱d
                                                 Vcc                     GND
                                                                                                    11

                                                                                                                                           /7-
            O                         Co                                                       B.
                                 1。
                                      Ac                                                            7
                                                                                                                             b
                                                                                               B1
            O                         A1                    7483
                                                                                                    4
                                 3                                                             B2

                                                                                                                                           7-
                                      A2                                                                                     9
                                                                                                    16.-
            O              =..
                                                                                           ,
                                                                                               B3                            10
                                      A3C4        s,
                                                  S3
                                                            s,
                                                             S2
                                                                         s,
                                                                         S1
                                                                                      s
                                                                                      S


                                                                                                                                           ／丁～-
                                            14         15
            O                                                                         e-
                                                                                                                             12
                                                                                                            11                   ^
                                                                                                                                 J
                                                                                                                                                  +5 V
                  +5 V


                                                                                                           680 1 resistors




                                                                                                                 LEDs
                                                                                                    \,     \,


                     Fig. 6.7. 4-bit binary full-adder/2's-complement binary full-subtractor.


                                                                                   61

===== PAGE 78 =====
      Note the add-subtract switch in Fig. 6-7.
      Add and subtract the binary numbers of Tables 6-7E and 6-8E. At the same time, check your
results by conversion to decimal.

                                               Table 6-7E. 4-bit binary addition.

                                                         Binary:                                                  Decimal:
                           」           plus       β       plus            (?()        =          꾜i'7i            月+B = S

                     A3 A2 A1A0            B3B2BI B0            C。
                                                                                 C4              S3 S2 S1S0

             l        1010                     0101                  0

             2        1010                     0011                  0
             3         l 11I                   0110                  0
            4         11 11                     1 1 11               0



                                   Table 6-8E. 4-bit 2's-complementary subtractor.

                                                         Binary.'                                             z)ecin1n/．·
                                   계           minus       β      =              difference                   A - B =D

                         A3A2A1A0                 B3B2B1B0                C4              s3s2s1s0
                 l        1010                     0101
                 2        1010                     001 1
                 3        1 111                    0110
                 4        111 1                    11 1 1
                 5        0101                     1010


REQUIRED RESULTS


Using positive logic, complete the following tables corresponding to the experimental data.
1ㅌ>2.5V, 0 ㅌ<0.5V.



   Tables 6-IR, 6.2R, 6-3R. Full-Adder.                                                                       Table 6-4R.
   x       Y         q         S          C。
                                                                                             x           y         Ci       S   C。
                                                                                                 0        0             0
                                                                                                 0        0        +5
                                                                                                 0       +5             0
                                                                                                 0       +5        +5
                                                                                            +5            0             0
                                                                                            +5            0        +5
                                                                                            +5           +5             0
                                                                                            +5           +5        +5


                                                                     62

===== PAGE 79 =====
      Complete Table 6-6R based upon the experimental data of part 4(b).


                                               Table 6-6R.
                          BinaDUVotation                                 Decimal Equivalent
                              치xo                                                        치시）
     치x0        Yl y0       plus Y1y0            C。
                                                  'sis)           차차7       Ylγ0       plus yiYo

                               8c,                  SE,
                          Sum Computed        Sum Experimental




【기SCUSSION

1.   Compare the full-adder data of parts 1, 2, and 3 with a truth table for a full-adder. Discuss
     your data. Explain the principle of obtaining full-adder output for:
     (a) the circuitry of parts 1 and 2;
     (b) the circuitry of part 3.




2.   Does CO in part 2 for the full-adder give correct results? Explain the equivalence of this circuit
     to the Boolean expression for

                                        Co = XYCi + XYC1 + XYC1 + XYCi

     (Hint: Use a Kamaugh map.)




3.   The Boolean expression for the borrow-out BO of a full-subtractor is given by BO = XYB, +
     XYBi + XYB' + XY7 ,. Show by means of a Karnaugh map that this can be reduced to XY +




                                                   63

===== PAGE 80 =====
     YB1 + XB1. Using the 7400 and 7410 ICs, draw a logic diagram showing pin connections for
     this B。reduced.




4.   In the required results for part 4(b), the computed sum Sc should be equal to the experimental
     sum SE. Is it?




5.   In Fig. 6-7 is a lit LED a I or a 0? Why?




6.   Explain how the add/subtract switch in Fig. 6-7 controls the 7483 /7486 operation to perform
     addition and 2s complement subtraction.




7.   In Table 6-7E explain the C4 values obtained.




8.   In table 6-8E explain the C4 values and the S3 S2 S1 S。values obtained.




                                                 64

===== PAGE 81 =====
                                                                 Experimenl7



Biskoble or Flip-Flop(FF)



OBJECT


To study the characteristics and operation of various types of bistables.


INTRODUCTORY THEORY


Bistable: Types and Definitions


The flip-flop (FF), bistable, or binary is a circuit with two (and only two)stable states. It remains
in one of the stable states until a signal changes it into the second stable state and remains in the
second stable state even upon removal of the signal. In a similar manner, a second signal can change
the circuit from its second stable state back to its first stable state.
     The standard FF symbol is shown in Fig. 7-1. It is common practice to designate the outputs
as Q and Q or levels I and 0. A typical truth table is shown in Table 7-1. The FF is defined only by
the states A and B given in Table 7-1.

                                                                        T = Trigger or Clock
        Table 7.1. FF states.
       State      Q       Q
         A       0         l
         B        l       0                         S
                                                  (or J)



                                                            Fig. 7-1. The flip-flop(FF).

                                                 65

===== PAGE 82 =====
     In a transistorized bistable two transistors are dc-coupled so that one transistor conducts while
the second transistor is reverse-biased and cannot conduct. The external circuit conditions and
components of the nonconducting side are arranged to keep one transistor in conduction (most fre-
quently in saturation), and the external circuit conditions and components of the conducting side in
turn are arranged to keep the second transistor cut off.
     Since the circuits for each transistor are identical, this symmetrical arrangement keeps either
transistor in the on or off state, thereby providing a bistable arrangement. An external signal is re-
quired to change the FF from one state to another. One way to do this is to apply a signal to the
on transistor in such a way as to make it nonconducting. This process, because of the dc coupling,
simultaneously tends to bring the nonconducting side into conduction. A temporary unstable con-
dition is quickly reached when both transistors are simultaneously conducting. One is trying to
cut off and the second to conduct. The condition is regenerative, with the result that the transition,
once initiated beyond a critical point, occurs very rapidly, and a stable reversal of state is reached.
     The IC flip-flop is a modification of the basic transistorized FF,and IC gates take the place of
the transistors previously discussed. Many different types of FFs have been designed. The basic
types used with ICs will be discussed.
     R-S or set-reset FF is defined as a bistable with SET and RESET inputs having the restriction
that both inputs cannot be simultaneously energized because the resultant state of the bistable is
indeterminate. The term CLEAR is frequently used in place of RESET. When made with two
NAND or NOR gates, this FF is frequently called a latch. Figure 7-2 gives the logic symbol for the
R-S flip-flop.



                                                                          O

                                                                （그   -O
                                 Fig. 7-2. Logic symbol for R-S flip-flop.


      Gated R-S flip-flop is identical to an R-S flip-flop with respect to logic and truth table. In-
formation can be transferred into the FF only when the gate is enabled. The terms CLOCKED,
STROBE, and SYNCHRONOUS are frequently used in place of GATED. Figure 7-1 also shows
the logic symbol of a gated R-S flip-flop.
      D or data FF is a binary that has a single data (D) input and a clock input. Figure 7-3 gives
the logic symbol for a D flip-flop.



                                O         D
                                          Clock
                                O        or trigger

                                           Fig. 7.3. D flip-flop.


     Master-slave FF consists of two dc-coupled, gated FFs. Information is transferred into the
master section during one state of the clock pulse and from the master to the slave during the
opposite state of the clock pulse. This arrangement isolates input and output and minimizes race
Pr《기：1ems.
      A block diagram of an R-S master-slave FF is shown in Fig. 7-4. The notation means that
information is entered into the master when the clock is 1, but the circle at the input to the slave
means that information from the master is prevented from entering the slave. When the clock goes

                                                      66

===== PAGE 83 =====
                                S                                                                 O   ,

       O0하  （        0-
                                     Master                                          Slave
      or trigger
                                                                                                            O




                                     Fig. 7-4. Master-slave clocked flip-flop.


to 0 no information can enter the master, but the clock input to the slave is at a 1 and information
from the master can now enter into the slave.
     T or toggle FF changes state after a trigger or clock pulse and obeys the truth tables of Table
7-2(a). It is common also to indicate the toggle truth table in the manner shown in Table 7-2(b).
The notation of Table 7-2(b) means that before the trigger pulse at tn, the bistable is in a state de-
fined as Q, and after one additional trigger pulse, tn+l, the bistable has toggled and is in the state
Q. A T flip-flop is frequently made by cross-connecting the inputs and outputs of a master-slave
FF, that is, by connecting S to Q and R to 0. Figure 7-5 gives the logic symbol for a T flip-flop.




                                           Fig. 7-5. T or toggle flip-flop.


                    Table 7-2(a). Toggle states.
            Before Trigger, r''     After Trigger, t,,.,.1                    Table 7-2(b). To 'e states.
              Q            Q          Q                Q                             tn       Q
              1            0          0                1
                                                                                               Q
                                                                                     tn+1
               0            l          l               0


     i-K flip-flop is a combination of R-S and T flip-flops. It has two inputs, J and K,the equiva-
lent of the R and S inputs. Whereas in the R-S flip-flop energizing the R-S inputs simultaneously is
forbidden, in the J-K flip-flop energizing the J and K inputs makes the FF toggle. The truth table
is given in Table 7-3. Note that the Q values are omitted since they are the opposite of the Q
output.

                                                fable 7-3. J-lK states.

                                                       rn         tn.
                                                                    ,.1
                                                   J         K     Q
                                                   0         0     Qn
                                                   l         0     1
                                                   0         l    0
                                                   1         l     Qn
                                                             67

===== PAGE 84 =====
IC NAND Gate Flip-Flops


R-s flip-Flop

     Consider Fig. 7-6. Define the set condidtions as Q = 1, Q = 0; define the reset conditions as
Q =0, Q = I. Assume that the FF is in the set condition and S= R= 1. This makes a= l, b =0,
d = I, and e = 1. These inputs make output c = I and f = 0. This is a stable condition and nothing
changes.




                                   Fig. 7-6. NAND gate R-S flip-flop.


     Now make S = 0 and R = 1. This makes both inputs a and b = 0, keeping c at I - Inputs d
and e are both 1 keeping f= 0. There is no change. S = 0 and R = I are the input conditions to set
the FF.
     Now make S = I and R = 0. With R = 0, input e becomes 0 and output f goes to a I. a and b
are both is, making c = 0. Hence. S = I and R = 0 makes Q = 0, Q = 1 and resets the FF.
     If both S and R = 0, Q and Q go to 1, which is not allowed.
     The truth table is given in Table 7-4.

                                   Table 7.4. R-$ flip-fl이）truth table.
                                      S        R        Q        Q
                                       l       1        No change
                                      0        1        l        0
                                       l       0        0        l
                                       0       0        Not allowed


     An IC NOR gate FF can be made in the same way. In the NOR gate IC. S = R = I is not
allowed, and S = R = 0 is the stable, no-change operating condition.


Clocked '77ip-Flop

     In Fig. 7-7, gates 3 and 4 form a simple latch. Information is clocked through gates I and 2.
If the clock is low, the outputs of gates 1 and 2 are high. The latch remains in its previous state no




                                                   68

===== PAGE 85 =====
matter what the levels of S and R are. Suppose that the clock goes high. If S= 1 and R = Q,,the'
output of gate 1 is 0 and of gate 2 is 1. This makes the output of gate 3 a 1 and the output 6 f
gate 4 a 0. The truth table is given in Table 7-5.




                        4 1>_', ㅢ 3)
    so_
                                                                                                           00


                                                           '
          이ock                                        百：
                Lb뇨戶



                                                                                                           00
    HO_

                                       Fig. 7-7. NAND gate clocked flip-flop.
           갼h
                               Table 7-5. Truth table: NAND gate docked FF.
                          (:7ock             S,
                                                               R                   Q                   Q
                               1            i\    .                          ;y
                                                                                                   ?
                                                                                                   :
                                                               흐＼
                                             0"                                        '   l   (
                                                                         \
                           '   1   .                                r\            '0
                                                               "r
                               0             0                               Does not change
                               0             1                 0             Stor,s last data


D orz）
     αrα Flip-Flop

     The D data FF, shown in Fig. 7-8, is a modification of the clocked FF. Data are available at
the D terminal as a I or a 0. The inverter ensures that two Os cannot be presented simultaneously
to the information input to gates 1 and 2. Only after the clock pulse has taken place are the data
stored and available at Q and Q.




                                            F눕．
                                              7-8. D (data) flip-flop.




                                                               69

===== PAGE 86 =====
Master-Slave aocked,Flip-Flop

     The master-slave FF (Fig. 7-9) consists of two clocked FFs. When the clock is 1, gates V
and W are enabled and information is transferred from S and R to the output of the master. How-
ever, the clock input to gates X and Y is at 0 (inputs to X and Y through an inverter), and the
master information is blocked from the slave. When the clock goes to 0, the clock input to gates X
and Y goes to 1 and the master information is transferred to the slave. The truth table is given in
Table 7-6.




                                X\ X
                                     1
                ^
                                                                                                  O○
                b
                        V




이0하〔




                                                                                                  0ㅇ
                    伊   w




           1Iㄴ                  Master                                          Slave

                                Fig. 7-9. NAND gate master-slave clocked flip-flop.


                                     Table 7-6. Truth table: master-slave FF.
                                           S       R         Q       Q
                                           l       0         l       0
                                          0         1        0       l


Toggle Flip-Flop from Master-Slave Flip-Flop

     Cross-connect S to Q, R to Q. Assume that the clock is a 0, Q = 1, and Q = 0. The cross con-
nection makes S = 0, R = I. With the clock low nothing happens. Now let the clock go to 1 and
back to 0. The truth table of the preceding section tells us that if S = 0 and R = I the output must
go to Q = 0, Q = 1 after the clock has gone to 1 and back to 0. But this has changed the state of
the FF, which is a toggle. Similarly, each clock pulse causes the FF to toggle.

f-K Flip-Flop

     The i-K flip-flop (Fig. 7-10)is a modification of the toggle FF. Input gates V and W are modi-
fied to have three inputs. The additional inputs are called the J-K inputs.



                                                        70

===== PAGE 87 =====
                                                                                                               乙
                                       /
                                   ).
                                                                                     ){.
                                            ㅓ》
（긔
O




              v
                  >   1
                                            b.
                                                                                >1
                                                                                                       )   ●
                                                                                                               Qㅇ




                                        Fig. 7-10. NAND gate i-K flip-flop.



       If J and K are both 1, the FF operates as a toggle FF, as in the preceding section. This must be
so, since in Boolean logic 1 " A = A.
       Now, let J = 1 and K = 0. If Q = 1 and Q = 0 when the clock goes to 1, there are three I inputs
to gate W. The output of gate W goes to 0. The output of gate V goes to 1. This makes the output
of the master at point a = 1 and at point b = 0. When the clock goes to 0, the information at a and
b is transferred to the slave, making Q = 1 and Q = 0.
       Again, let J = I and K = 0. Suppose that Q = I and Q = 0. The only way Q could have become
a 1 is for a to have been a 1 and b a 0. When the clock goes to 1, what are the inputs to gates W and
V? GateW: clock = l, J = l,0= 0. GateV: clock = l, J =0, 否= 1. Hence, theoutputsofgatesW
and V are 1 and the master latch does not change, and in this case also Q = 1 and Q = 0.
       Similar arguments hold for J = 0, K = 1. The truth table for the J-K flip-flop is shown in
Table 7-7. The truth table for this FF shows that it is an RST FF with the toggle properties occur-
ring when both J = K = 1.
      In Table 7-7, the notation t, refers to the state of the FF at the time before the clocking pulse.
t, .1 refers to the state of the FF after the clocking pulse.




                               Table 7-7. Truth table: i-K NAND gate FF.

                                        tn                        乙i+/
                                Before Ci（∼八 Pulse          After Clock Pulse
                                   J             K           Q           Q
                                   l             0            l          0
                                  0              l           0           l
                                   l             l           Q           Q                 To餌e
                                  0              0           Q           0                 No change



                                                       7l

===== PAGE 88 =====
EQL기PMENT REQ(기RED

     CRO, dc and calibrated                          IC type 7402 quad 2-input NOR gate
     dc power supply, +5 V at 50 mA                  IC type 7472 AND-gated J-K flip-flop
     Two switch banks, 5 switches per bank           SWG, +5 V at 10 kHz or single-pulse 50 'Js
     IC type 7400 quad 2-input NAND gate

                                             IC manufacturers' part numbers.
                                                                    7'exas            National
                    乃'pe       Motorola           Fairchild      Innruments         Semiconductor
                    7400       MC7400P             7400PC          SN7400N            DM7400N
                               MC7400L             7400DC          SN7400J
                    7402       MC7402P             7402PC          SN7402N            DM7402N
                               MC7402L             7402DC          SN7402J
                    7472       MC7472P             7472PC          SN7472N            DM7472N
                               MC7472L             7472DC          SN7472J



EXPERIMENTAL PROCEDURE


For all ICs in this experiment: vcc = +5 V to pm 14, 0 (ground) to pin 7.
      In each part of the experiment take CRO voltage measurements at the points indicated to
complete the accompanying tables. The CRO vertical amplifier is to be used dc-coupled with a gain
setting of 1 V/div and is to be used to make all the voltage measurements. Measure all voltages to
within 0.1 γ. A/' data are to be taken row by row.
      In each part of this experiment measurements have to be made at the two outputs Q and Q of
the FF. If a dual-trace or dual-beam CRO is available, both traces should be used for the two
points. If a single-trace CRO is used, the measurements will be made more rapidly and the FF
operation seen more readily if the CRO is connected to the Q and Q outputs by means of a switch.
In all measurements connect the Q side to the same CRO input terminal or to the same side of the
switch.

1.   R.-S Flip-Flop with NAND Gates




                                   Fig. 7-11. R-S mp-flop with NAND gates.

                                                        72

===== PAGE 89 =====
                                   Table 7-IF. NAND gate R-S flip-flop.

                                             S        R        Q          c

                                   l       +5             0

                                   2        +5       +5

                                   3             0   +5
                                   4       +5        +5

                                   5             0        0
                                   6a       +5       +5

                                   7             0        0
                                   8b      +5        +5
                                    aSwjtch S and R to +5 almost simul-
                              taneously, but switch S is to reach +5 before
                              switch R. This is to simulate a race condition.
                                    bswjtch S and R to +5 almost simul-
                              taneously, but switch R is to reach +5 before
                              switch S. Again, this is to simulate a race
                              condition.



2.   Gated A-S Flip-Flop


     a.   Gated R-S Flip-Flop｀〃ir/zNAND Gates




                               0


                                            PULSE GEN.
                                             Single.pulse
                                                50ps
                                                +5V
                                                                     그－
                                   Fig. 7-12. Gated flip-flop with NAND gates.




                                                          73

===== PAGE 90 =====
                                       Table 7-2E. Gated FF with NAND gates.
                                                 Gate               S                    R              (2          Q
                                   l              +5                     0               +5
                                   2              +5                +5                        0
                                   3              +5                     0               +5
                                   4             +5                      〕                    0
                                   5                   0                 0                    0
                                   6                   0                 0               +5
                                   7                   0                 0                    0
                                   8                   0            +5                   +5
                                   9                   0                 0               +5



    b.   Gated R-S Flip-flop with NAND Gates

      In Fig. 7-12, disconnect pins 5 and 10 from the gate switch and connect pins 5 and 10 to the
single-pulse generator.
      For each row, set switches S and R to the indicated values and read the values of Q and Q.
Then apply the single pulse where required and again read the values of Q and Q. Note: The "Before
Single Pulse" data for each row is the "After Single Pulse" data of the preceding row.

                                       Table 7-3E. Gated FF with NAND gates.
                                                                             Before Single                     After Single
                                                                                Pulse                             n41se
                                             S             R                        Q              Q           Q            Q
                            la
                                        +5                      0                                        －〔－
                                                                                                                     //＇一


                                                                                                   〃－
                                                                                                         ／一


                           2                 0             +5                */-"
                                                                                              二－
                           3            +5                      0
                           4                 0             +5
                           5                 0                  0
                           6            +5                      0
                           7                 0             +5
                           8                                    0
                                                                                                                   No
                                        +5
                           9                 0             +5
                                                                                                                   釘ngle
                                                                                                                   pulse
                          10                 5                  0
                          li                 0                  5
                                 aThiS sets the FF in a known state.




                                                                                    74

===== PAGE 91 =====
3.   D Flip-Flop


     +5 V




                                       -*
             Puke gen.
            Single pulse
               50ps
                +5V
                                             ㅋ         74   ◇             .




                                                 Fig. 7-13. D flip-flop.



As in part 2(b), the "Before Clock Pulse" entries are obtained from the "After Clock Pulse" data
from the preceding row.

                                                  Table 7-4E. D FF.
                                                     Before Clock                       After Clock
                                      z)ata             ／뇨lse                              Pulse

                                                      Q              Q                  Q            Q
                                                                                               //
                             Ia
                                        +5                       →一＞      /a

                                                                                   二，    /
                                                                     */
                                            0        *-/                       '
                             2
                             3              +5
                             4              0
                             5               0
                             6              +5
                             7               0
                                                                                             No
                             8              +5                                               clock
                                                                                             pulse
                             9               0

                            10               5
                                  aThis sets the FF in a known state.




                                                                7S

===== PAGE 92 =====
4.   AND-Gated J-K Master-Slave Flip-Flop


     a.            -1
          AN)Gated f-K Operation                                                                            -----F,－ㄱ
                                                                                                       Qu                              (,
                                                                                                                              \
                                                                                                                                       PR
                                                                                                       二J

                                                                                                                                  J             0   흐
                                                                                                                              7
                                                                                                                                      7472


                                                                                                            ㅕ
                                                                                                                          0 아
                                                                                                                            （
                                                                                                                              직
 +5V

                                                                                                                                            뮌
                                                                                                       oJ                         K             0

                                                                          노_
                                                                                                            ―
                                                                                                       0                              CLR
                  kb                                            K2
                                                                                                                                                        ―
                       」2
                                                                                                            -
                                                                               ㅡ                                                            ㅡ
                                                                     -o
                                                                                                            …                                           긔
                                                    PULSE GEN
                                                   SINGLE PULSE
                                                       50MS


                                               Fig. 7-14. AND-gated i-K flip-flop.


                                          Table 7-SE. AND-gated i-K operation.

                                                                                                   tn                        r'1+J
                                                                                                 Before                     After
                                                                                              Single Pulse               Single Pulse

                       슥         /2       /'           K1                 K2        K3             Q            Q        (2             Q
                                                                                                                    //
             a
                             0        0        0       +5                 +5        +5                                            /
                                                                                                            >/           //
                                                                                                                    /
                                                                                                            *//
             l               0        0        0            0                  0         0   *,/
            2          +5
                                      0        0            0                  0         0

             3         +5        +5
                                               0            0                  0         0

             4         +5        +5       +5                0                  0         0

             5               0        0        0       +5                      0         0

            6                0        0        0       +5                 +5             0

             7               0        0        0       +5                 +5        +5

             8         +5        +5
                                               0       +5                 +5             0

             9         +5        +5       +5
                                                       +5                 +5             0

            10         +5        +5            0       +5                 +5             0

            11         +5        +5
                                               0       +5                 +5        +5

            l2         +5        +5       +5
                                                       +5                 +5        +5

            l3         +5        +5       +5           +5                 +5        +5

            14          +5       +5       +5           +5
                                                                          +5        +5
                 a-'0 clear the FF
                                                                               76

===== PAGE 93 =====
     In Tables 7-SE and 7-6E, the notation t, refers to the state of the FF at the time tn before the
clocking pulse. tn+1 refers to the state of the FF at time tn+1 after the clocking pulse.


   b. J-K Mode Using 10-kHz SWG

    Change the output of the pulse generator to a 10-kHz square wave. Set the CRO controls to:

                                            AUTO trigger
                                            NEC slope
                                            INT trigger

     View the output of the SWG on the CRO. Adjust the horizontal time/div so that the wave-
form shown in Fig. 7-15 is obtained. View and record the waveforms on the graph paper of Fig.
7-15 for the following conditions. DO NOT change the time/div scale. Trigger CRO as indicated.


                  +5
           SWG
                        0                                                  -             -




           O      +5

   4(ba)슛긴豆 .


           a      +5
   4(bb) 읫긴t            。

                  +5
           0
    4(bc)슛긴등 0

            O
           --      +5
   4",H, J = +5
   " - ' K= 0           0



           O    +5
          J= 0
    4(be)
          K= +5 0



           a       +5                                                     7



    4(bf) <긴5           。

                                  Fig. 7-15. Waveforms for part 4(b).

                                                  77

===== PAGE 94 =====
         只zrr     (7mPur                       rhgger         ii        /2       J3   K1           K2         K3
         4(ba)       Q         EXT (NEG) from Q                +5       +5
                                                                                 +5   +5
                                                                                                   +5
                                                                                                              +5

         4(bb)           Q        EXT (NEG) from Q             +5       +5
                                                                                 +5   +5           +5         +5
         4(bc)           Q     INT                             +5
                                                                        +5       +5        0       +5         +5

         4(bd)           Q        INT                          +5
                                                                        +5       +5        0       +5         +5

         4(bc)           Q        INT                               0   +5       +5   +5           +5         +5
         4(bf)           Q        INT                               0   +5
                                                                                 +5   +5           +5         +5


   c.   Asynchronous Mode: PRESET//Y긱 and CLEAR /CL／리




                                                                                                   PR


                 \ kb7＼
        +5V- O---+-                   O-           O                                                      O



                                                                                           C CK
                                        ㅉ＼＝「
                                                                                                   7472


                                                                                      )
           -      -－七－        -{--.




                                                                                               K          Q
                                                                                                   CLR
                                                                                                    U
                          SWG
                         10 kHz
                          +5V



                                                 Fig. 7-16. Asynchronous mode.



     The PR input is used to set the Q output to a 1, and the Q output to a 0. The CLR input is
used to set the Q output to a 0 and the Q output to a 1. The PR and CLR inputs override all other
inputs.
     In table 7-6E, tabulate the voltages obtained for the following conditions. If a square wave is
seen, use the notation SW.




                                                              78

===== PAGE 95 =====
                                          Table 7-6E. Asynchronous operation.
                                               J         K           PR           CLR               Q   Q
                               1          +5
                                                        +5
                                                                     +5
                                                                                       +5
                               2         +5             +5                0       +5
                               3         +5                  0            0       +5
                              4                0        +5                0       +5
                               5               0             0            0        +5
                              6          +5
                                                        +5           +5                     0
                               7         +5                  0       +5                     0
                              8                0        +5                0       +5
                              9                0             0            0       +5
                             10          +5
                                                        +5                0                 0
                             11          +5                  0            0                 0
                             l2                0        +5                0                 0
                             13                0             0            0                 0



REQUIRED RESULTS


In completing the following tables, use positive logic, 1 = > 2.5 V,0 = <0 5 V.

1.   Use the following notation in completing the truth tables:

          1 and 0 for the logic states
          NC for no change
          NA for not allowed

          Based on the data of Table 7-1E, complete Table 7-lR, the truth table for the R-S flip-
     flop using NAND gates.


                                                             Table 7-IR.
                                                   R-S flip-flop with NAND gates.
                                                    S            R            Q                 Q
                                                    1            0
                                                    0            l
                                                    l            I
                                                    0            0




                                                                     79

===== PAGE 96 =====
2.   Based on the data of Tables 7-2E and 7-3E and using the same notation as in result 1, complete
     the following truth table, Tables 7-2R, 7-3R, for the gated R-S flip-flop of Fig. 7-12. The Q
     and Q columns are the output levels after the gating pulse.

                                                    Tables 7-2R,7-3R.
                                              Gated NAND gate R-S flip-flop.
                                               S          R             Q            Q
                                                l         0
                                               0               l
                                               0          0             NC           NC
                                                l              I        NA           NA


3.   Based on the data of Table 7-4E and using the same notation as in results 1 and 2, complete
     Table 7-4R for the D flip-flop.

                                                    Table 7-4R. D flip-flop.
                                       Data               tn
                                                                                 r   '1+ /

                                                      Q             0        Q               <2
                                          I           l             0
                                         0            l             0
                                         I            0             l
                                         0            0             l


4.   In completing the tables for the AND-gated J-K FF use the following notation:

          L 0 logic levels
          X-the state of this input does not affect the state of the output
          NC-no change

     (a) Clocked J-K mode. Use the results of Table 7-SE and waveforms of part 4(b) to corn-
     plete Table 7-SR. Note that the FF is symmetrical; the effect of the J inputs on Q is identical
     to the effect of the K inputs on Q.




                                                               80

===== PAGE 97 =====
                                              Table 7-SR. i-K mode.
                                                                           r   '1           r     /
                                                                                                '1+


                  ii      /2      心      K1        K2      K3         Q             Q   Q             Q
                   l       l      l       0
                   l      1       1                0
                   l      l       1                        0
                  0                       1         l      l
                          0               l        1       l
                                  0       l        1       l
                  0                       0                           1             0
                  0                       0                           0             1
                  l       I       1       l        1       l          l             0
                  1       1       l       l        l       l          0             l


      (b) Using the data of Table 7-6E of part 4, complete Table 7-6R for the asynchronous mode.
      Indicate toggling by Q in the Q column and Q in the Q column.

                                       Table 7-6R. Asynchronous mode.
                                         PR       cLR      Q          <2
                                          l        I
                                          0        I
                                          l        0
                                          0        0



【기SCUSSION


 1.    Explain how the 2-input NAND gate FF of part I and Fig. 7-11 has bistable properties and
       will stay in the stable state. Explain how the S and R inputs change the state of the bistable.




 2.    Explain why, in Fig. 7-11, S = 1, R = I is allowed but S = 0, R = 0 is not allowed.




                                                    8l

===== PAGE 98 =====
3.   An R-S bistable has momentarily been driven into the nonallowed state. Based on the data of
     lines 6 and 8 of Table 7-1 E, discuss the factors that determine into which of the allowed states
     it may return.




4.   Explain why, in Table 7-2E, the results of lines 1,2,3, and 4 differ from those of lines 5,6,7,
     8, and 9.




5.   It is desired to use a latch for temporary data storage of a completed arithmetic operation in a
     computer while another arithmetic operation is taking place. Based upon the data of Table
     7-2E, what gate level, 1 or 0,should be used to transfer data into the latch? What level should
     be used to isolate the latch from the arithmetic operation that is occurring?




6.   Based on the data of Table 7-3E, what does the single gate or strobe pulse do?




7.   The gated R-S flip-flops of part 2 have four gates. Figure 7-17 is an attempt to make a gated
     FF with two gates. However, it will not work correctly. Explain why it will not. (Hint: Con-
     sider all possible levels for R,S, and the gate.)




                                              F自g. 7-i7.




                                                 82

===== PAGE 99 =====
8.   The standard method of writing a truth table for the type 7472 is given in Table 7-7D.

                                          Table 7-7D. Function table.
                             INPUTS                              ouTPuTsa
                      PRESfT      CLE겨R       CL火：?K         J        K               Q        Q
                         L            H           x          x        x          H        L
                         H            L           x          x        x          L        H
                         L            L           x          x        x          H*
                                                                                          H*
                         H            H          丁1=         L        L          0。
                                                                                          Qo
                         H            H          J1-         H        L          H        L
                         H            H          -I그山        L       H           L        H
                         H            H          Jㄱ．.        H       H                TOGGLE
                          apositive logic: J = J1 . J2 . J3; K = K1 " K2 " K3.
                          Courtesy: Texas Instruments, Inc.



     (a)   Compare this with Table 7-SR and the waveforms of part 4(b) and explain why the J-K
           entries have the same meaning in both tables.




     (b)   To obtain a 1 in the Q column requires that J1, J2, and J3 be at 1. To obtain a 0 in the
           Q column requires that K1, K2, and K3 be at 1. How is this requirement shown on the
           type 7472 logic diagram?




     (c)   In the "OUTPUTS" column, what is the significance of the asterisks (*) next to the Hs
           in the third row?




     (d)   In the fourth row, what is the meaning of the Q。and Q。entries?




                                                        83

===== PAGE 100 =====
9.    From the wave pattern for part 4(b), what is the frequency of the output at Q for J = +5,
      K = +5? Show your calculations.




10.   What is the frequency that would be obtained at the Q output of FF 2?


                                                                Tog이e
                                                                 FF2
                800 HZH T      Toggle
                                             Fig. 7·l8.




11.   The logic diagram of the type 7472 has an inverting circle at the clock input. This means that
      data are transferred to the slave output when the clock goes to its logic zero level. The PR
      and CLR inputs have inverting circles also. What do these mean? (Hint: See Table 7-6E and
      Table 7-6R.)




                                                84

===== PAGE 101 =====
                                                                        Experiment8



Binary Counters and
The Binary Number System



OBJECT


     1.   To study the operation of binary counters.
     2.   To study binary counting and the representation of numbers in the binary number system.


INTRODUCTORY THEORY


Binary Counter


A binary or bistable FF has the characteristic of changing state with each incoming pulse and re-
verting to its original state after two pulses have been applied. After the second pulse there is
nothing to indicate whether zero or two pulses have occurred. However, if the return to the original
state is considered an "overflow" and is applied to a second binary, it will now also change its state;
this change in state, combined with that of the first binary, can be used to indicate that two pulses
have occurred.
      Additional binaries, similarly, can be cascaded beyond the first two and their states will mndi-
cate the number of pulses that have been applied to the input of the succession of binaries called
"binary-counter." In such a counter the count is represented in binary notation by the states of the
counter binaries or stages.
      If we represent the state of the binary before a pulse has appeared as a 0, and the opposite
state as a 1, we can then represent the number of incoming pulses in both binary notation and by
the state of the counter stages in an n-stage counter as

                            count = Bn2n-' +Bn_12"-2+ B1`_22"-3+···+B120                            (8-1)

                                                     85

===== PAGE 102 =====
In this representation the Bs (binary digits or bits) can be either 0 or I. For example, suppose that
we have a four-stage counter and 12 pulses have been applied. After 12 pulses we would find the
binary states(and Q outputs) as follows:

                                               Stage     Level

                                                             1 l
                                                             l ,
                                                  4

                                                   *
                                                    l
                                                    1
                                               `
                                               ^/n            0 0



And the count from Eq. 8-1 is

                         unt = I X 2(4-i) + 1 X 2(3-') + OX 2(2_ i) + OX 2('-') = 12
                        c。
                              =1X23+ lX22+ 0X2'+ 0X2《）=12

      In a binary, both outputs, the Q and Q terminals, can be made available, or only the single
terminal Q can be made available. When only the single terminal is available, the state of the various
stages are represented by the Q levels-either 1 or 0-and these levels are the B values in Eq. 8-1. If
both sides of the binary are available, the counter becomes more universal and can be used for mul-
tiple coincidence outputs or decoding; the complements of the count are available at the Q termi-
nals. Thus, the Q terminals count down, as opposed to the Q terminals, which count up.
      A binary counter must have provision for clearing the count so that it is at a total count of 0
before any new count pulses are applied to the counter if correct counts are to be obtained each
time a new train of pulses is to be counted.


Frequency Division

     When the incoming pulses occur at a regular rate or constant frequency, the frequency at the
output of the first binary is one-half that of the incoming frequency. Each binary in turn divides its
incoming frequency by 2 and, therefore, in an n-stage counter the output frequency at any stage is
( )P X the incoming frequency, where p is the number of stages up to the point of measurement.


Ripple (:bzmrer

      Figure 8-1(a) shows in block diagram a basic type of binary counter called a ripple counter. In
this type of counter the output of each FF triggers the next stage. This triggering takes place on a
l-to-0 transition. Suppose the condition exists in which all three FFs are in the 1 state and a trigger
pulse arrives at the input to FF 1. Any circuit has some propagation or switching time, and FFs are
no exception. As a result of this propagation or delay time, each stage arrives at its final state at a
time delayed by the previous stages, and the count "ripples" through the counter. For example, if
the switching time per bistable were 100 ns, in a three-stage counter such as shown in Fig. 8-1(a),
the output of FF 3 would arrive at its final state 300 ns after the trigger pulse if all three FFs had
to change state.
      From a counting standpoint or from a frequency-division standpoint this causes no problems,
but consider the following problem. Suppose that we are supplying input pulses to a binary counter
at a 200-ns rate and we have an operation that must be performed at the count where stages 1 and 5
in a five-stage counter are at a 1. This requires a coincidence or AND gate. But the fifth stage does
not arrive at its correct state until 500 ns of delay, and at this time two additional trigger pulses (or
counts) have been applied to the counter. The AND gate, therefore, is operated at an incorrect
count because of the FF switching times. Other coincidence gates may similarly give false indica-
tions or may be turned on and off at wrong times and thereby provide false triggering pulses.

                                                        86

===== PAGE 103 =====
                                                  0
                                          m
                 Clock           FF 1             0                  FF 2                    FF 3
                                              m

               (a) Three-stage binary ripple counter

                                                  Q

                                                      Qㅇ
                         T.
                                         -0
        Cl。    ck_ k             FF 1                          '1
                                                                     FF 2                    FF 3




                                                                                       A2)
                                                                              -1
                                                                                   4
                 (b) Three-stage synchronous(clocked) binary counter
                                                  Fig. 8-1. Cascade binary counters.


Synchronou화Clocke따 Binary Counter

     The difficulties with the ripple counter discussed above may be overcome with a counter in
which all stages are triggered simultaneously. The counter becomes more complex and is shown
in block form in Fig. 8-1(b). Examination of Fig. 8-1(b) shows that the trigger to FF 2 comes
from AND gate Al. Gate Al is enabled by a 1 from the Q output of FF 1 and the clock pulse.
Except for the gate Al delay (which in general is low compared to that of a FF), both FF 1 and
FF 2 are triggered simultaneously by the clock. The same is true for FF 3, which is clock-triggered
when FF 1 and FF 2 are in the I state. Hence, except for the single gate delays, all stages are
triggered simultaneously by the clock.

CRO Waveforms and Triggering

     The observation of counter wave patterns on a cathode-ray oscilloscope (CRO) provide a
powerful and rapid method of analysis of counter operation and possible malfunction. To obtain the
correct pattern and analyze it requires that the CRO be triggered at the correct time on the wave-
form. Consider the wavepatterns of a three-stage binary counter triggered on the 1-to-U transition

              Input sign키
                 d0햐（                                      T
              0 output
                FF 1

              0 output
                FF 2

              0 output
                FF 3
                              Hg. 8-2. Wave patterns for the 3-stage binary counter of Fig. 8-I.

                                                                    87

===== PAGE 104 =====
(positive logic), as shown m Fig. 8-2. To obtain the correct patterns, note that all the patterns
start with a negative-going transition. The only time all three FFs simultaneously have a negative-
going transition is when the Q output of FF 3 is going negative. Hence, to properly trigger the CRO
we must use external, negative-slope triggering from the Q output of FF 3.


EQUIPMENT REQUIRED


     CRO,dc and calibrated
     dc power supply,+5 V at 100 mA
     Square-wave generator(SWG), +5 Vat 10 kHz or single-pulse 50 j.is
     IC type 7400 quad 2-input NAND gate
     IC type 7420 dual 4-input NAND gate
     IC type 7472 AND gated J-K flip-flop; three required
     01-j.tF capacitor


                                          IC manufacturers'part numbers.
                                                                     Texas       National
                 乃ipe        j1rotorola        Fairci'i五f        Instruments   Semiconductor

                 7400        MC7400P            7400PC            SN7400N        DM7400N
                             MC7400L            7400DC            SN7400J
                 7420        MC742OP            742OPC            SN7420N        DM7420N
                             MC7420L            742ODC            SN7420J
                 7472        MC7472P            7472PC            SN7472N        DM7472N
                             MC7472L            7472DC            5N7472J



EXPERIMENTAL PROCEDURE


For all ICs in this experiment: Vcc = +5 V to pin 14, 0 (ground) to pin 7.

1.

     (a)   Wire the circuit of Fig. 8-3 for a three-stage binary ripple counter.
                View the wave shape at the output of the pulse generator. Use AUTO triggering,
           negative slope, and INT. Vertical is dc-coupled I V/div. Either vary the pulse generator
           frequency or adjust the CRO sweep speed so that 10 cycles of the pulse generator occupy
           exactly 10 horizontal divisions (see Fig. 8-5 on page 91). Now view the wave pattern at
           pin 8 of FF 3. It should have the appearance shown in Fig. 8-4. DO NOT at any time
           during the experiment change the pulse generator frequency or the CRO horizontal sweep
           frequency.




                                                            88

===== PAGE 105 =====
                                                                    土
                             1니 4 5
                                                                    四
                                                                                                                                        PA                                        `J 4                 PA
                                                                                                                                                                            b
                                                                                                                                                                            *
                                                                        0                                                                                0                                         I          0
  SWG                                                7472                                                                               7472                                                   /       7472
  .5V
                        12                                                                       1                                                                          12
d『 K) kllz                                       C CK                                                                       C 아ㄷ                                                               《 CK
 or single
                                                         FFt                                                                            FF2
                                                                U
                                                                                                                                                                                         --,


  Pm`e                                느
                                                                                                     ,       -＝卜
                                                                                                                                                                  -

  50p5                                                                  0
                                                                                                                                                             6.
                                                                                                 -已－-                            A                   0
                                                                                                                                                                                               7
                                                                                                                                                                             9-
                                                                            으－
                                                                                                                                                                                                                  요－
                                                                1
                                                                                                 lu-                         /          -   .   1                           10-
                                                                                                                   _-                   tL H
                                      ∼
                                                                                                                                                                            1t-
                                                                丁
                                                                                                 "-                              -1乙－




                                                                        +5V -－→－                                        To all pin 14s


                                                                                             궂ㅋ O.1〃F, ;Locate as탄ose

                                                                            0    '
                                                                                     .

                                                                                         -
                                                                                             l   1
                                                                                                         -    as possioue to an
                                                                                                                   1    Toallpin7s
                                                                                                                                                    us




                                                   Fig. &3. IC-binary ripple counter.


                        +5
                     FF3
                     Pin 8
                             .0
                                                                                                         I             I I
                                                   F恪 8-4. FF 3-pin 8-wave pattern.



  (b)        Change the pulse generator function to SINGLE PULSE.
                   Check the voltage levels at pin 8 of all three FFs. At least one should be at ground
             and at least one should be at approximately +5 V. If this condition does not exist, return
             the pulse generator momentarily to SQUARE WAVE and then back to SINGLE PULSE
             and once again check the pin 8 voltage levels. If necessary repeat again until the pin 8
             levels are not all alike.
                   Measure the voltage at the indicated IC terminal pins to complete Table 8-1E.

                                                                                                 Tab1e &lE.
                                                 /7／구3                                                       /7/72                                                    FF/
                                          Pin            Pin。           6                    Pm8                                                                            Pin 6
                                            Q8                                                Q                         PinQ '                      兜8                       Q




                                                                                             89

===== PAGE 106 =====
(c)   This can be done in the order indicated, or all pin 2s can be connected to ground
      simultaneously.

          1.   Connect pin 2 of FF 1 to ground and then remove the pin 2 ground connection.
          2.   Connect pin 2 of FF 2 to ground and then remove the pin 2 ground connection.
          3.   Connect pin 2 of FF 3 to ground and then remove the pin 2 ground connection.

          Measure the voltage at the indicated IC terminal pins to complete Table 8-2E.

                                                           Table 8-2E.
                                /7F 3                             /7/7 2                           /7/7/


                        /in 8           Pin 6           /)r71 8            /in 6           /in 8           /in 6
                          Q               Q               Q                 Q               Q               Q



(d) Binary counting. Operate the pulse generator, a single pulse at a time, to complete Table
    8-3E. Data are to be taken row by row. At pulse 0, the indicated voltage shown in Table
    8-3E should be obtained. Check these to make sure of the values before recording any
    voltages.

                                                           Table 8-3E.
                                        /7/73                              /7772                           F/7 /

                                /in 8           /in 6             Pin 8            Pin 6           Pin 8           月n 6
                 凡dse            Q               Q                  Q               Q               Q               c
                   0              0             七 +5                0              只．+5              0             二늑二+5


                   l
                   2
                   3
                   4
                   5
                   6
                   7



(e)   CRO wave patterns-correct triggering. Set pulse generator to 10-kHz square wave.
      View the waveforms at the IC terminal pins indicated. Sketch them as indicated on
      the graph paper of Fig. 8-5. For the CRO triggering use AUTO trigger, negative slope,
      dc-coupled, and external triggering from pin 8 (Q output) of FF 3. Vertical input, dc-
      coupled, 1 V/div.




                                                          90

===== PAGE 107 =====
      이ock
      101mz




       FiF 1
       Pin 8
                             1      2       3        4      5        6       7       8


      FiF2
      Pin 8



                    +5
      FiF3
      Pin 8              0



      FiF1
      Pin 6
                         0



      FiF2
                +5
      Pin 6
                         0


               +5
      FiF3
      Pin 6
                         0

                                 Fig. 8-5. Wave patterns for part 1(e). Correct triggering.


2.   CRO Wave Patterns-Incorrect Triggering


The patterns obtained in part 1(e) give the correct wave pattern. This part of the experiment will
demonstrate how incorrect patterns can be obtained with improper triggering. In describing the
patterns, indicate the description by means of the following letter code. If necessary, use more than
one letter to describe your results. Take the data column by column, starting with column A.

     a. Correct.
     b. Wrong phase-correct frequency.
     c. Unsteady or unrecognizable.




                                                            9l

===== PAGE 108 =====
                                                                        Table &4E.
                                fxT〃百G          fxT NfG           /ixT Nzr(;          ZixT NECF           fxTP0S
              l1'ave            TRIGGfR         r7굿JGGf7?         TR/(;G/r7?          TR／《7GE7?           rR/GGER                  NfG                    POS
             Shape                from            /yαm              /yα刀7               from                  /rα＇7i             7R/GGER              77궂：/（六7fR
             αr /in               clock         FF /, Pin 8       FF2, Pin 8          FF3, Pin 6         FF3, Pin 6                INT                   力Vr

                                          』4
                                                    B                   C                 D                    E                    /7
                                                                                                                                                           G

           Clock
           FF 1, pin 8
           FF l, pin6
           FF 2, pin 8
           FF2, pin 6
           FF 3, pin 8
           FF 3, pin 6



      3.
              a.    Sync加아7')n玎CLOCKED) Counter- Three-Stage


           Wire the circuit shown in Fig. 8-6. This is a three-stage clocked binary counter. The wave
      shapes obtained at pins 8 and 6 should be identical to those obtained in part 1(e) of the experiment.




 4



12*
                          .1
                               7472
                                      O
                                                              4

                                                                             /
                                                                                  J
                                                                                      7472
                                                                                              O
                                                                                                                            3-
                                                                                                                            4
                                                                                                                            5-

                                                                                                                           12
                                                                                                                                    ,       ）콘，       J     1
                                                                                                                                                          7472
                                                                                                                                                                 O
                                                                                                                                                                     8   T0EXT
                                                                                                                                                                         TRIG NEG

                    a다                                                        C CK

                                                                                                                                                                     \/
                     （                                                                                                                            C CK
                               FF1                                                     FF2                                                                FF3
                                                                                                                                                                     6
                                                                                                                                                  \
 9                        K           O                     9                     K           O                             9-
                                                                                                                                                      K          O
10                                                         10                                                              10
11 -－∼                                                     11                                                              11-




                                 4                            9                   12
                                                                                                         11                             加                        加
                                                                                                                             ^
             7400                         740                      74                    740                                 4
                                                                                                                             Z
      2                         5                         10                      13
                                                                                                                             二J




             Pulse gen.                                              +5 V                                 To all pin 14s
              10 kHz
                                                                                          I       0.lpFas 히ose
                SW
               -4-5 V
                                                                            .丁las
                                                                            。                      possibleT。
                                                                                                            to。l!
                                                                                                               ICspin7s



                                                Fig. 8-6. 3-stage synchronous (clocked) binary counter.


                                                                                 92

===== PAGE 109 =====
If they are not obtained, temporarily change the synchronization to INT and make sure that each
stage, starting from FF 1, operates properly. When all stages operate properly, sketch the wave
shapes on Fig. 8-7 at the points required. (Use external synchronization-negative slope-from pin 8
ofFF3.)



      （ 乂k
      Cl。ck     +5
    （긔
    (see Fig.
       8.5)          0



                +5
       FF
       Pin쵸          0



                +5
       FF2
       Pin8          0



                +5
       FF 3
       Pin 8         0



                +5
      7400
      Pinil          0



                +5
       7420
       Pin6          0



                +5
       7420
       Pin8          0

                         Fig. 8-7. Wave patterns for part 3(a)-synchronous (clocked) counter.




                                                         93

===== PAGE 110 =====
    b.    Synchronous Counter-EJ7ecr0/ Wiring Error

     In wiring a complex circuit a wiring error occasionally occurs, or a component may be defec-
tive. Analysis of the wave shapes obtained provides a clue to the location of the error. Even in a
simple circuit such as that of Fig. 8-6, the possibilities of a fault are many. In this part of the ex-
periment a fault is introduced. An analysis of the wave shapes obtained with the correct ones of
part a should determine the cause of the fault.
     The fault to be introduced is: "Remove the connection ab from pin 8 of FF 1 which goes to
pin 9 of the type 7400 IC and pin 2 of the type 7420 IC." Now sketch the wave shapes on Fig. 8-8
at the points indicated.



     Cl。 ck   +5
    (see Fig.
      8.5)     0



                  +5
         FF 1
         Pin8          0



                  +5
         FF2       '
         Pin8          0


                       ＇■
                       .
           E      4-
          “師
            ;
            ' `




                       0



                  +5
      7400
      Pinil            0
                                                                                                          `



                  +5
         7420
         Pin 6
                       0



                  +5
         7420
         Pin8          0

                           Fig. 8.8. Wave patterns for part 3(b)-synchronous counter with wiring error.




                                                               94

===== PAGE 111 =====
PE(긔기RED RESULTS


1.   (a)   Using the data of Table 8-3E for positive logic, complete Table 8-3R. Use logic ie\ cls I
           and 0.

                                                     Table 8-3R.

                  Q3    Q2    QI    BinaD)      Decimal Q3      Q2   QI        BinaD1 Decimal Col. A
                 Pin 8 Pin 8 Pin 8 〃m沚； 'er      Equ加. Pin 6 Pin 6 Pin 6      Numz)er Equiv.     구
           ／뇨lse F/73 /7/72 /7F / Q3Q2QJ          ofK   /7/7 3 ／下 2 /7/7 /    Q3Q2口／   ofL    cr7/. β
                                         K           A                           L         B
             0      0     0      0      000          0         l     l   l     i l l
              l

             2

             3

             4

              5

             6

             7




     (b)   Using the wave patterns of part 1(e), Fig. 8-5, for positive logic and at the indicated hori-
           zontal box, complete Table 8-5R using logic levels 1 or 0 as obtained.


                                                      Table 8-SR.
                               Box      Q3      Q2        QI        Q3   Q2     QJ
                                 l

                                 2

                                 3

                                 4

                                 5

                                 6

                                 7

                                 8




                                                     95

===== PAGE 112 =====
［기＄CUSSION

 1.    Explain the function and necessity for the grounding of the pin 2s of each of the FFs in part
       1(c). What does grounding all the pin 2s do? What was the binary count before and after the
       pin 2s were grounded?




 2.    Referring to Table 8-3R, column L is the                complement of column




 3.    Compare the progression of the count in columns A and B of Table 8-3R. Discuss with re-
       spect to both binary and decimal representation.




  4.   What is the maximum count capability of an eight-stage binary counter?
       Binary                     Decimal

  5.   Compare Table 8-3R with Table 8-SR and discuss. In your discussion, comment on the ease of
       analysis of correct counter operation using the method of part 1(d) or part 1(e). Which method
       of operation, SWG or single pulse, would you use if you had only a voltmeter available?




  6. If the clock frequency is 10 kHz, calculate the frequency at pin 8 of FF 1, pin 8 of FF 2, and
     pin 8 of FF 3 of Fig. 8-3. Show your calculations based upon a sweep speed of 100 ＇』s per
     division using Fig. 8-5.




  7.   Calculate the output frequency of a seven-stage binary ripple counter if the input frequency is
       1 MHz.




                                                  ,6

===== PAGE 113 =====
 8.   In part 2, which method of triggering (trigger point, trigger slope, column of Table 8-4E)gave
      the correct wave pattern at all points in the counter? Explain why it gave the correct pattern,
      [Hint: Refer also to part l(e).1




9.    Explain the operation of Fig. 8-6 with respect to the wave patterns of part 3(a).




10.   The wiring fault introduced in part 3(b) caused malfunctioning of the counter. Explain the
      resultant waveforms at pin 8 of FF 2 and pin 8 of FF 3 based on your analysis of the error
      and the waveforms obtained in part 3(b).




11.   What are the advantages and disadvantages of the ripple versus the synchronous counter?




12.   A binary has a switching time delay of 25 ns. It is used as the FF element in a six-stage ripple
      counter. The counter is in the 1 1 1111 state. A pulse changes the first stage to the 0
      state. How long after the first stage changes to the 0 state will the sixth stage change to the
      0 state?




                                                 ,7

===== PAGE 114 =====
              」   .    1                   i" .   r勻」   “   』

                                       』也m , ' 1            "      뇨"            한}   毋4,*   '   r   }컥   1=4旨，
                                                                                                              뻑三노

              「“   「      每, .1 .               零等 1；
                                       鞏 . 'n. <，    슈 " 咐3/t=
              斗∼“村뇨－h 갸三i엥 g'   r iiirf낡／나 ‘冬包令驪勘再江鉀*纖泣벼


              즈和骨：
                 「娑焚쓰弓


   r ｀洲‘簪
 , " ' n下d낳

臘3驛」      .．뇨冶嶠潑鐘客聊 ，,物h泌＜）γ兪m.．漱碁
얜〕
                    心 毖漱‘i村堪啼i瓣．沙，
梵．‘.',1, >: cij 걍iti｝
         큰'    . 二r   ;.
                                 .y三쵭礪
                               』 . 녀 1,                 . .1d 心；:r.r 耳씽
                               "1 1               , r二｀         / 》매긱 :    r 止 'd :
`             三，̀
                r뇨M        4       .     ` ; 노       놔                       '` →，:

'夕“4：叱    1:塔': ; 外－t1" 1公r1‘尹盈




                                                            羈南慽α含b作촤茗車茹帑 t｝눕蜘
                                                            '. 1      二   윅：:.

===== PAGE 115 =====
                                                                       Experiment9



Divide-by-N Counters
and Decade Counters



 OBJECT


      1. To study counters that divide the incoming frequency by counts other than binary powers and which use
cascaded T flip-flops.
     2. To study the count states of these counters.
     3. To study the weighted BCD decade counters 8421 and 2'421.
     4. To study the unused states of the 8421 counter.


INTRODUCTORY THEORY

The toggle or T flip-flop divides an incoming frequency by a factor of 2. Cascading T flip-flops
results in a final frequency which is the original frequency divided by (吉)P, where p is the number of
stages. Many applications require output frequencies which are a division of the input frequency by
a factor other than a power of 2. For example, the divide-by-lO counter is very useful and common.‘
      What is meant by a divide-by-N counter? This means primarily that there is an output fre-
quency that is 1/N of the input frequency. The output wave shape, not necessarily sine wave or
square wave, repeats itself at a repetition rate 1/N of the input frequency. A common way to build
a counter is to cascade T flip-flops. Let us assume that we have such a counter and that no incom-
ing signal is applied to the counter. We can examine the state of each binary and express it in
binary or equivalent notation. Let the signal voltage be applied. For each cycle or pulse of the in-
coming signal one or more of the FFs changes state. The FFs change state so that each incoming
pulse results in a different overall count state. In a divide-by-N counter there are N different count
states. After the Nth count the counter has returned to its original state and the process is repeated.
Such a counter, with its N different count states, is frequently designated as a counter of modulus
〃 or mod〃．

                                                     99

===== PAGE 116 =====
                                                                                        ,7 S




                                                                                        ,7
                                                                                               B
                                           A




   （기0하
      （



                                  Fig. 9-I. Mod-3 i-K,R-S counter..

      The basis for mod-N counters is the cascaded I flip-flop. Since p stages of T flip-flops have
2" count states, to divide by less than 2" requires that some of the count states must be skipped.
The number of T flip-flop stages that are required depends upon the count. A mod-N counter
requires p stages for values of N which fall between 2" and 2"-'. For example, a four-stage counter
(as a binary counter capable of dividing by 16) is required for values of N between 9 and 15.
      IC mod-N counters utilize the R-S and i-K properties of the master-slave FF to skip the re-
quired number of unwanted states. Both ripple and synchronous (clocked) counters can be built,
but ripple counters are simpler.
      A mod-3 counter which makes use of the i-K properties of the master-slave universal FF is
shown in Fig. 9-1. Since it has two stages, it is fundamentally capable of dividing by 4. How does
this counter skip one count state and divide by 3?
      In the circuit diagram of Fig. 9-1, QB is connected to the J input of FFA. The K input of
FFA is connected to logic 1. The state of FFB controls the operation of FFA. If Q8 = l, JA and
KA are both I and FFA toggles after a clock pulse. If QB = 0, J A = 0 and KA = 1 and FFA will go
to a 0 state (QA = 0, QA = 1) after a clock pulse. FFB operates in almost the same manner. J B is
connected to QA and KB to logic 1. If QA = 1, FFB toggles (JB and KB = 1). If QA = 0 (J8 = 0,
KB = 1), FFB goes to the 0 state (QB = 0. Q,= I) after a clock pulse.
      To start, assume that both FFs are in the 0 state.



  (？αm1r    JA      KA      QA     QA      /8     KB      QB             QB
                             0      l                      0             1
    0
             l       l       0      i      0       l       0             l
                             1      0                      0             l             FFA has toggled.
                                                                                       FFB forced to stay the same.
    l                                                           -   --   --   --   1

             l       I       l      0      l       I       0             I
                             0      l                      l             0             Both FFs toggle since
    2                                                                                  JA =KA = 1 andJB =KB = 1.
             0       l       0      l      0       l       l             0
                             0      l                      0             l             FFA forced to stay the same.
                                                                                       FFB forced into the 0 state.

===== PAGE 117 =====
      The counter is now back to its original state after three pulses and after three distinct count
states.
     The most common mod-N counter is the divide-by-b0 or the decade counter. It requires four
binary stages. Counters can be designed to have any possible state of the four binaries for any one
of the 10 counts. This results in the possibility of an extremely large number of decade counter
designs. Even if we restrict the design to counters which only progress upward in binary count, the
number is still very large.
      The weighted counter design, in which each binary has a weight, is a very common design. For
example, if we have a 2'42 I counter (this is frequently also written as 1242')and the counter is in
the count state 1101, the count number can be determined as follows:

                         Stage        Weight       State              cmd'nt
                           4          2 =2'         l      l × 2=2
                           3            4           1      1 X4=4
                           .            2           0      0X2 ==0
                           l            1           l      1Xl =l
                                                                 7 = total count


     In the past, 8421, 2'421, and 4221 decade counters were used, but at the present time the
8421 counter has become the most common. Such standardization has simplified the interface
problem to computers, printers, display devices, and similar equipment. These and many other
codes are binary-coded decimal (BCD). It has become common, however, to represent the 8421
code as BCD. However, to eliminate the confusion, the 8421 code is sometimes represented as
NBCD, since it progresses in binary in the normal sequence until 9 (binary 1001) and then re-
turns to 0.
     Figure 9-2 is the diagram of an NBCD (BCD)or 8421 decade counter. It makes use of the
R-S and J-K properties of the master-slave FF. FF I is a toggle FF. FF 2 is a i-K flip-flop with
J-K properties determined by the connection from Q of FF 4. FF 3 is a toggle FF and FF 4 is an
R-S flip-flop with its R-S properties determined by the states of FF 2 and FF 3. A i-K flip-flop
can be used for FF 4 since its R-S properties are the same as those of the master-slave R-S flip-flop.




                                         ,7
                                 ＜니
                                                                                                         ㅡ


                                          5
                                 mb




              1                                2
ock -----－《                                                           4        3                    4



｛ㅍ石i，스                                    C
                                                                                           .   ,7
                                                                                                C
                                 C                          -11
                                                                  C                    C




                                       Fig. 9-2. 8421 decade counter.


     Assume that the counter is in the 0000 state.

      1. This means that QofFF4 isata 1. The 1 connection from Qof FF4 toS1 ofFF2putsFF2inthe
toggle mode. FFs 1, 2,and 3 now count in binary up to a decimal count of 7, binary 111.

                                                     101

===== PAGE 118 =====
      2. At this point in the count, the Q outputs of FF2 and 3 are at a 1. This makes S1 and S2 of FF4 at 1 and
the Q output of FF 3 at a 0 makes C2 of FF4 = 0. At the eighth Count FF 1,2,and 3 all toggle. The Q output of
FF 1 is connected to the clock input of FF 4. With S1 and S2 of FF 4 = 1 and C1-C2 of FF 4 equal to 0, FF 4
operates as a clocked R-S flip-flop and FF 4 changes to the I state.
      3. The counter is now in the 1000 count stage(= decimal 8). The count state is designated by the state of
FF4,FF 3, FF 2, and FF 1 in order. At the ninth count FF 1 toggles and the count state is 1001.
     4. At this count Q of FF 4 is at 0. Q of FF4 is connected to S1 of FF 2, and this 0 input will prevent FF 2
from toggling (J-K properties of FF 2) at the tenth count when FF 1 toggles. The ninth count has made S1 and S2
of FF 4 have 0 inputs and the C1 input of FF4 has a 1 input after the ninth count. When FF 1 toggles at the tenth
count and goes to 0, this clock input to FF 4 makes FF 4 go to a 0(R-S properties of FF4). The counter is now
back to 0000 after the tenth count.

      Mod-N counters have states which are not used. The possibility exists, however, that the
counter may get into one of the unused states. Noise, for example, may cause one of the stages to
change its state at an undesired time. When the counter is first turned on, each stage arrives at its
initial state due to its own internal characteristics. Let us consider what can happen if the counter
happens to get into an unwanted state.
      One possibility is that it may progress into one of the desired states. It then continues to
operate properly. The other possibility is that it continually progresses and recycles through a
series of unwanted states in a subloop. Provisions then have to be made in the design of the counter
to take it into a wanted state.


EQUIPMENT REQUIRED


     CRO,dc and calibrated
     dc power supply, +5 V at 100 mA
     SWG,positive-going, 5-V pulses at 10 kHz or 50-ps single pulse
     0.01-pF capacitor, paper or ceramic, 25 to 400 V
     IC type 7472 AND gated i-K flip-flop; four required
     IC type 7490, decade counter

                                         IC manufacturers' part numbers.

                                                                  Texas           National
                 Type         Motorola        Fa加child        Instruments       Semiconductor

                 7472        MC7472P           7472PC           SN7472N           DM7472N
                             MC7472L           7472DC           5N7472J
                 7490        MC749OP           7490DC           SN7490N           DM7490N
                             MC749OL           7490PC           5N7490J



PRELIMINARY PROCEDURE


Each of the mod-N counters in this experiment will be studied with CRO wave patterns.
      Set the pulse generator repetition rate or the CRO horizontal sweep rate so that 10 cycles of
the incoming frequency occupy exactly 10 horizontal divisions of the CRO. Adjust the horizontal
position so that the vertical side of the pulse falls exactly on a vertical CRO line of the graticule.
Use negative slope, internal trigger, dc coupling for the trigger, and AUTO mode. DO NOT
CHANGE ThE REPETITION RATE OF ThE SWG OR THE CRO HORIZONTAL SWEEP RATE
DURING THE EXPERIMENT.


                                                      I02

===== PAGE 119 =====
      In the preliminary check of the operation of the counter it is best to use internal trigger. How-
ever, to obtain the correct pattern, the CR0 must be triggered externally from the 0 output oft/ic
/i'iα／stage w/r/7 negative slope.
      The experiment requires that the count states of each of the counters studied in this experi-
ment be determined. The count state always begins with the state of the final stage of the counter
and is expressed as a binary number corresponding to the state of the stages, as shown in Fig. 9-3.


              Clock
               ----
                                    FF 1     ---)
                                                                         FF 2       ----

                                                                                                    FF 3    ,       --0w             FF 4


                                    1                                     0                             1                                1
             Exan耳기 e

                  Count State
                                                            1        1     0        1


                                            FF4
                                               /                 FF3            FF2               FF1

                                                                 Fig. 9-3. Count state.



EXPERIMENTAL PROCEDURE

                                                                                                                                             TO EXT
1.    Mod-3 Counter                                                                                                                          TRIG NEG




                  12
                       4
                       5
                           -   1_
                                             J
                                                      古3
                                                    7472
                                                                 a
                                                                                            4-
                                                                                             5-
                                                                                           컁2 一
                                                                                                                \7   J
                                                                                                                         7472
                                                                                                                                     ㅣ   0      ,

                                        0아
                                         （                                                                      C CK
                                        ,
                                                    ㄴ ～
                                                           F 1                                                           FF 2                           `
                                                                                                                     K
                                                                                                                                                        ,
                                                                                                                                                        '
                                        7
                                                                                                                                                        /
                                                                                                        F亡
                                                                                                                T
                                                                                                                a
                                                                                                                O         n      d   4
                                                                                                                                 1
      SWG
                                                                                                                          H ㅔ小
                                                                         \/cc= +5V to                           F    Short       놀

                                                                                                                                 1



      +5V                                                                                                            leads
     104어z                                                                      pin 14
                                                                                                                ㅜ
                                                                                                                a
                                                                                                                          n          `
                                                                         0(ground)
                                                                                                                                 `
                                                                                                                O                /




                                                                         to pin 7

                                                            Fig. 9-4. Mod-3 counter.


                                                                              103

===== PAGE 120 =====
Adjust the SWG frequency or the CRO horizontal sweep rate so that each cycle occupies one hori-
zontal division as shown in Fig. 9-5 (Clock). Do not change for the remainder of the experiment.
     Check the Q output of FF 2 to see if the counter divides by 3. Use internal trigger. On the
curve sheet of Fig. 9-5 sketch the wave shapes as they appear at the following points:
     Use:

    NEG nUGGER                                              (a)   O0야＝
     AUTO                                                   (b)   FF 1 Q output
     EXT TRIGGER from Q output of final stage               (c)   FF 1 Q output
     dc nUGGER                                              (d)   FF 2 Q output
                                                            (e)   FF 2 0 output


                                            -       -
                     +5
      1 (a) Clock
                              0                 -




                    +5
    1(b) FF 1 O
                              0



                         +5
    1(c) FF 1 O
                              0



                    +5
    1(d) FF2O
                              0



                    +5
    1(e) FF2O
                              0                                                          』




                    +5
    2(a) FF3O
                              0


                     +5
    2(b) FF 3 Q
                              0

                                  Fig. 9-5. Wave patterns: mod-3 and mod-6 counters.




                                                        l（닉

===== PAGE 121 =====
2.   Mod-6 Counter


Figure 9-6 is the circuit for this counter. Note that it is exactly the same as that of Fig. 9-4 except
for the addition of a T flip-flop after FF 2 of Fig. 9-4.


                                                                                                         TO EXT
                                                                                                         TRIG NEG


4
                , J
                    7     7472
                                 O
                                         4



                                         2
                                          5                   J
                                                                   7472
                                                                          O

                                                                               12
                                                                                          J
                                                                                              7472
                                                                                                     O       -
                    ㅁ CK                     쎄          <     CK                      ㅁ CK


                )
                           FF1                                     FF2                        FF3
                                     6    9
                                                                                                         6
                                                                          （그              K          O
                                         10
                                         1j




           「→
                        To all pin 14s

         =0.0lpf
        겨：                       Short
                -                leads


                     》 To all pin Is      SWG
                                          +5 V
                    Vcc =+5 V to         10kHz
                           pin 14
                      0 Iground)
                      to pin 7



                                              Fig. 9-6. Mod-6 counter.



    Check the output of FF 3 for division by 6. On the same curve sheet used for part 1, Fig. 9-5,
draw the wave patterns as they appear at the following points:

     (a)        FF 3 Q output
     (b)        FF 3 Q output




                                                        l05

===== PAGE 122 =====
3.         Decade Counter 2'421 (or 1242')




                                                                                                                         ㅗL
                                                                                        1
                                                                                        U 4 5                     ,7
                                               m.U
                                                                                                -


                                                                         p
                      ,
                                               ,
                                                                                                -


                                    。
                                B                                                                                                                       스→*TO E
                                                                                                                                                            TRIG잦EC
 ；三
                      J                                             c7472
                                                                                                r                   7472
      -,    .   . .                                                                     1
                                              `2
12
                      0                                             CK                                        C
                                                                                                              ,
                                                                                                                  c〔

                                                                        FF2                                            FF3
                                                           -

                                                                    K                                             K                                     O
                                                                               O   =-   9-
                                                                                                                        棚
      m                                       1l`                       cI-R            10-         1_        7
                                                                                        Ii -
                                                                                                                                                   `1




 SWG
1OkHz
  Sv
                                                                                                                             Vcc- '5vIop,nI4
                                                     -.,          SHORT
                                                               Top,n 14,
                                                                                                                             0 Ig,o.zndl m p,n 7
                                        -L-
                                                                         F包. 9-7. Decade counter 2'421.


Check the output of FF 4 for frequency division by 10. Sketch the wave shapes on the curve sheet
of Fig. 9-8 as they appear at the following points:

           (a)            FF 1 Q output
           (b)            FF 2 Q output
           (c)            FF 3 Q output
           (d)            FF 4 Q output

     Note: One of the unused states of this counter is a state in which the counter will not count.
If, after checking the wiring, the counter still does not count, change the SWG to single pulse,
momentarily ground each of the CLR (pin 2) terminals to set the counter into the 0000 state, and
then" change the SWG back to 10 kHz. Check to see if the counter now counts in the correct man-
ner (output at FF 4 ÷ 10).




                                                                                                         k陌

===== PAGE 123 =====
                                                m-         -
                          +5
                                       r-                          「－   -
                                                                            -



      Clock
                               0



                     +5
                                                               r

3(a) FF 1 Q
                               0



                     +5
3(b) FF 2O
                               0



                 +5
3(c) FF3O
                               0



                +5
3(d) FF 4 O
                               0



                +5
4(a) FF 1 O
                               0



                +5
4(b) FF2O
                               0



                +5
4(c) FF3O
                               0




                                          V
                +5
4(d) FF4O
                               0            l

            Fig. 9.8. Wave patterns for part 3 (decade 2'421) and part 4 (decade NBCD 8421).




                                                     l07

===== PAGE 124 =====
          4.   Decade Counter NBCD 8421

          Check the output of FF 4 (Fig. 9-9) for frequency division by 10. Sketch the wave shapes on the
          curve sheet, Fig. 9-8, as they appear at the following points:

               (a)        FF 1 Q output
               (b)        FF 2 Q output
               (c)        FF 3 Q output
               (d)        FF 4 Q output


                                                                                                                                            To EXIT
                                                                                                                                            TRIG NEG

                                                                                                                              3

                                                                                                                                                  )
                                                                                                                                  )
                                                                                           3-
 3-
 4               ,        PR                                            PR                 4             PR              L1            PR
                                                                                    8
                                                      ,
                                                                                   ---o
 5-
                 7 」74720                            7 」7472 Q
                                                     '
                                                                                           5-        J
                                                                                                         7472
                                                                                                                O             5   J
                                                                                                                                       7472
                                                                                                                                              O

12                                        2                                               12                             12
                 C CK                                 C CK                                       O 아＜                             C아
                                                                                                                                   （

                                                                        FF2-                             FF3                           FF4
                                                                                                                          1_
                                                      ,
 9-
                                                                  l K         （그                    K           O   으」
                                                                                                                                   K          O

                                                                                                                         ：으
                                                                                                                                       CLR
                 ,'FF1O
10               I        CLR                         /                 CLJ                              CLR
11-   -




             SWG                                    To pin 14s
             -5 V
           10 kHz or                                      Short
                                                                                                VCC= + 5 V to pin 14
            Sin이e                                          leads                                0 (ground) to pm 7
             FM1se
             50 .zs
                                                    To pin is



                                                    Fig. 9-9. NBCD decade counter.



          5.   Unused States of the NBCD Counter

          This part of the experiment uses the same experimental setup as in Fig. 9-9.

                (a)       Change the pulse generator to a single pulse of 50 ' is.

                (b)       Reset the counter to the 0000 state using the CLR inputs.

                (c) r Set the counter to the 1010 state using the appropriate PR and CLR inputs. Note
                      that the state of FF 4 is that corresponding to the first bit in the state of the counter.
                      ( l0 7 FF4)

                (d)       Using the CRO (INT TRIGGER), measure the Q outputs of the four FFs. Your results
                          should agree with the operation performed in 5(c) above.

                (e)       Apply a single pulse, read the state of the counter, and tabulate in Table 9-1E. Continue
                          until you either reach a normal counter state based upon the results of the wave patterns
                          of parts 4(a), (b), (c), and (d) or you return to an unused counter state.

                                                                                    108

===== PAGE 125 =====
                                                     Table 9-1E.
                                              乃轍le          cOunt State




6.   IC Decade Counters


The TTL type 7490 counter used in this part of the experiment and in part 7 contains two sections;
a divide-by-2 section between pins 14 (input) and 12 (output) and a MOD-5 section with input to
pin 1 and output at pin 11 with intermediate outputs at pins 9 and 8. See the logic diagram,
Appendix D.




              SWG
              +5 V                                                            TO EXT
             10 kHz                                                           TRIG NEG
                                                   2 1 13
                                                   3 R,0 A12
                                                       /
                                                   4       Dli
                          vcc
                                                   5          10
                          +5 V
                                                   6 ,      B9
                                                   7 므9C8
                                                       7490
                                           0.0h』
                                               f
                                 'T  '     `h.?: Iea！」s'
                                  =.       d1 .ㄴ 50CK eI



                                         Fig. 9-10. NBCD IC decade counter.



      On the curve sheet on Fig. 9-11, plot the wave patterns that appear at the following outputs:

      (a)   Q1 output, A, pin 12
      (b)   Q2 output, B, pin 9
      (c)   Q3 output, C, pin 8
      (d)   Q4 output, D, pin 11

                                                           l09

===== PAGE 126 =====
                  +5
         Clock
                                 0-



                       +5
6(a) A, pin 12
             0



                       +5
    6(b) 8, pin 9
                 0



                            +5
    6(c) C, pin 8
                 0



                        +5
6(d) D, pin 11
                                 0




     FF 1 （그
                   +5
7(a)
 " p1n9                          0



                        +5
    (0) F,F 2 Q
7
    (b) pin8                     。



                  +5
     FE 3O
7(c) pinli                       。




            O+5
       FE 4 O
       FF
7(d)
       Pin12                     0

                                      Fig. 9-11. Wave patterns for parts 6 and 7.




                                                         l i0

===== PAGE 127 =====
7.   IC Divide-by-l0 Counter




                    SWG
                    +5 V
                   10kHz                                 -7U=
                                                            13
                                                         工－→2
                                                4:-      '- 3             12         》 T0 EXT
                                                                                       TRIG NEG
                                                            4             11
                                                            5             10
                                           中
                                    vcc
                                                    I-cu
                                    +5V                     6              9
                                           ―-
                                                            7             8
                                                    ㅌF             7490
                                           -
                                                    0.01pF
                                                    at IC socket

                                          Fig. 9-12. Divide.by-l0 counter.



On the same curve sheet as used for part 6, Fig. 9-1 1, plot the wave patterns that appear at the fol-
lowing outputs:

     (a) Pin 9           (c) Pinli
     (b) Pin 8           (d) Pin 12


REQUIRED RESULTS

Use logic I > 2.5 V and logic 0 <0.5 V. The count state is the representation as a binary number
of the FF states(Q output) beginning at the left with the state of the final FF.

1.   Complete Table 9-2R for the state of the mod-3 counter of part 1 based upon the wave patterns.

                                                    Table 9-2R. Mod-3 counter.
                                                           FF2              ／걋7/     cbunt
                               B0ㅈ        count           Q Output         QOutput   State
                                l               0
                               2                1
                                3               2




                                                            ln

===== PAGE 128 =====
2.   Complete Table 9-3R for the states of the mod-6 counter of part 2 based on its wave patterns.

                                             Table 9-3R. Mod-6 counter.
                                                  J가73          FF 2    FF /   count
                            B0ㅈ   cbunt            Q             Q        Q    State

                             l      0
                             2      I
                             3      2
                             4      3
                             5         4
                             6         >



3.   Complete Table 9-4R for the states and the equivalent decimal value of the count based upon
     the sum of the weighted values for the 2'42I counter of part 3 (see Introductory Theory).

                                           Table 9-4R. 2'421 decade counter.
                                                                                        Decimal
                                                                               count     cαzi鮮
             B9x     Count        F/74          F/73            FF2    FF J    State   Equivalent
                                                 Weighted Values
                                   2              4              2        1
               l       0
               2        l
               3       2
               4       3
               5       4
               6       5
               7       6
               8       7
               9       8
              l0       9


4.   Complete Table 9-5R for the states and the equivalent decimal value of the count based upon
     the sum of the weighted values for the 8421 BCD counter of part 4.




                                                         i i2

===== PAGE 129 =====
                                       Table 9-SR. 8421 BCD decade counter.
                                                                          count    Decimal
                      cba鮮      ／깊74      ／깊73         F772     FF /      State     count
                                           Weig加ed Values
                                  8         4           2        1
                        0
                        l
                        2
                        3
                        4
                        5
                        6
                        7
                        8
                        9



DISCUSSION

1.   10 kHz is the incoming frequency to the counter of part 1. What is the output frequency?
     How did you determine it? (Hint: Determine the period of each of the waves.)




2.   What is the output frequency of the counter of part 2?




3.   The BCD 8421 counter of part 4 counts in binary up to the count state of 1001 equivalent to
     decimal 9. At the tenth count only FFs 4 and 1 change state to return the counter to the
     initial state of 0000. Explain how this takes place. (Hint: Tabulate the J1, J2, and J3, and K1,
     K2, and K3 inputs after the ninth count. Then, based on the type 7472 truth tables, explain
     why the next count after 1001 is 0000. (In TTL a not-connected input assumes logic 1. See
     Experiment 4.)




                                                 il3

===== PAGE 130 =====
4.   Based on Table 9-lE, will a momentary transition into an unused state make the counter
     remain in a stable subloop which is not usable, or will the counter suffer only a temporary
     malfunction?




5.   It is desired to use the 60-Hz power line as the source of a periodic wave whose frequency is
     0.01 Hz.
     (a) If you were going to use a single counter, how many stages would be required?




     (b) What is the period of the 0.01-Hz wave?




     (c)   You want to use the same decade counter type 7490 used in parts 6 or 7 of the experi-
           ment and then build whatever else is needed to obtain the 0.01-Hz frequency by using
           the 7472 J-K FFs. Show how to obtain the 0.01-Hz frequency. Use a block diagram
           showing the ICs in each block.




6.   Based on the IC interconnection and wave patterns of part 6, what type of counter is the IC
     decade counter: SW output, 1242', or NBCD?



7.   Repeat question 6, but for the wave patterns of part 7.




                                                 n4

===== PAGE 131 =====
                                                                   Experiment O



Shift Re9isters
and Rin9 Counters


OBJECT


     1.   To study the shift register and its properties.
     2.   To study ring counters.
     3.   To study the twisted ring counter.


INTRODUCTORY THEORY


A register is a memory or data store. A shift register is a memory in which information is moved
or shifted one position at a time in response to a clocked command or shift pulse. The storage
element in an IC shift register is the bistable. and a shift register is a cascade combination of bi-
stables. The operation of a shift register is based on the directed R-S properties of R-S flip-flops or
the J-K properties of J-K flip-flops (J or K = 1). If the outputs (Q and Q)of a bistable chain are
connected to the J-K inputs (Q to J and Q to K) of the next bistable, a shift pulse will make a
following bistable assume or follow the state (data) of the previous stage. Succeeding shift pulses
can shift the data to other points in the register.
      Circuit arrangements of the shift register permit shifting data in either direction, left or right.
Shift registers are therefore called shift-right or shift-left registers.
      Any data bit is shifted one stage for each shift pulse and will appear at a point N stages away
delayed by the time of N shift pulses. A shift register can therefore be used as a delay.
      Serial-type information can be introduced into the first stage of the register 1 bit at a time.
After this bit-by-bit information has been transferred into and is stored in the register, the data in
all stages can be read out simultaneously in parallel form. This type of shift register is a serial-to-
parallel data converter. In a similar manner, information can be introduced into all the stages simul-
taneously in parallel form and read out of the last stage bit by bit by shifting the data toward the
last stage. In this form the shift register becomes a parallel-to-serial data converter.

                                                            l lS

===== PAGE 132 =====
             When the output of the last stage of a shift register is connected to the input of a shift register,
        data in the shift register circulate around the register. This is called a circulating shift register. It is
        the electrical equivalent of magnetic drum or disk storage.
              A circulating shift register in which only one stage is in a state different from all the other
        stages can be used as a ring counter, since the uniqueness of the position of this stage within the ring
        is determined by and is a measure of the number of shift pulses which are being counted. Such a
        counter has the advantage of being automatically decoded.
              When the output of a shift register is connected to the input in an inverse manner(Q to K and
        Q to J), the counter that results is called a Johnson, twisted-ring, switch-tail, or ring-tail counter,
        The counter fills up pulse by pulse until all stages are in the I state and then unfills until all stages
        are in the 0 state. This process repeats itself after a count of two times the number of stages, result-
        ing in a count capability of 2N, where N is the number of stages. To decode this counter requires
        only 2-input AND gates.


        EQ(기PMENT RE이기RED


             CRO, dc coupled and calibrated
             dc power supply, +5 Vat 100 mA
             SWG, 50ps+5 V, 10kHz, 1 Hz
             Switdr bat出, 8 switches
             Five 68047, 土10% composition resistors
             Five red LEDs
             IC type 7400 quad 2-input NAND gate
             Three IC type 7476 dual J-K FFs with PRESET and CLEAR
             IC type 7496 5bit shift-right shift register

                                                IC manufacturers' part numbers.
                                                                      Texas           National
                         乃'pe        ^iotoro故        Fairchild      介zstruments     Semiconductor
                         7400       MC7400P           7400PC          SN7400N          DM7400N
                                    MC7400L           7400DC          SN7400J
                         7476       MC7476P           7476PC          SN7476N          DM7476N
                                    MC7476L           7476DC          SN7476J
                         7496       MC7496P           7496PC          SN7496N          DM7496N
                                    MC7496L           7496DC          SN7496J



        EXPERIMENTAL PROCEDURE


        All data in this experiment are to be taken row by row.



0hift            Register

        Wire the circuit of Fig. 10-I of a 6-bit shift-right register. All switches, the CLR (CLEAR) and the
        PR (PARALLEL INFORMATION) switches are to be +5 V. The serial information switch is to
        be at 0.



                                                             n6

===== PAGE 133 =====
                                                 ` 《－
                                                                                                                                 춈5 v

                                          ,,,: ,, ,                            ,            亡－                   <-
                                                                         O                       O




-.
          r
                                                                                                                                                    - 1-i r---                                                                                        1-
                                                                                   -




                                               ；二76                                                                                                                                                                    ；얍
                                                                                                     ＋
                                                                                                                                     7476IC?
                                 pR                       ___
                                                                    pp
                                                                                   "
                                                                                        I
                                                                                        I
                                                                                                                       PR
                                                                                                                                                                                     I 1
                                                                                            尸
                                                                                                                                                                                                                                                      1
                                                                                                 I
                                                                                                                                 5                                         I'                                     15            9                     1
                        J             O                                                                                                                                                            」^        Q
                                                                                                                                                                                                             O
                                 A                    "    」 .           .＝스＋                        一                 A                                                                            A
                                                                                            1
              －《c
                                                                K                                                                                       CK                                         cK                   -   c CK
                    1                      4                                                                                     4                 12                                                             4         1
                                                                         O                                                                              K          O                                                                K


                                                                                                         I1ㄴ                                                                                                                                     ㄴ8   1I그
                                                                cLR                                                                                         cLR                      I I               CtR
                                                                                                                                                                                     I I
                                                                                   -J
                                                                                                                                               ㅡ                       _        _)     L_  _. __




                            8.i
                            SlgeI 1                                      a
                                                                                                                                                              ,4
                                                                                                                                                             8.
                                                                                                                                                            Slge 4
                                                                                                                                                                                                        8.1.5                           8. 6 ;
                                                                    8.
                                                                                                                                                                                                       Su..je 5                         Stge6



                                                                                                         Iv,e 7476         vㄸ 『 .5 V I,, Inn 5 0 Iq.o`.ndI 10 IOn 13

                                                                                                         TVI0 7400         Vr,. - .5 V IC니》,O 14. 0 Iq.orn'.II ionn7




                                                                             Fig. 10-I. 6-bit shift-right shift register.


     Set the pulse generator to single pulse.
     Now, clear all information from the shift register by connecting the CLR switch to ground and
then return it to +5.

     a.       Parallel In-.5:eria／ 九It

     Set is into both bits of IC 1 by switching the PR terminals connected to pins 2 and 7 of IC
1 to ground and then returning these PR terminals to +5. Now read the voltages at the Q terminals
of the shift register. They should be the values given in Table 10-1E.

                                                                                                                      Table lO-lE.
                                                          IC 1                                                              /c2                                                      IC 3
                                               Pin 7.5                   ／功 //                                 Pin 15                尸n //                        八
                                                                                                                                                                  ＇' 15                      Pifl 11
                                                勺 +5                      二뇝+5                                   0                      0                            0                             0




                                                                                                                            l l7

===== PAGE 134 =====
     Operate the pulse generator which is the shift pulse one pulse at a time. After each pulse, read
each of the Q terminal outputs and complete Table 10-2E. Enter data one row at a time.

                                                         Table l0-2E.
                                         IC I                        /(72                      /C13
                 Shift
                 ／뇨ise         Pin /.5          /in //     /in /.5          Pin /7   /in J.5          Pin / /
                    0            +5               +5          0               0        0                0
                    l
                    2
                    3
                    4
                    5
                   6


    b.
    Repeat the preceding procedure, clearing the register first, but set Is into FFA of IC 1 and
FFA of IC 2. Complete Table l0-3E.

                                                         Table l0-3E.
                                         IC 1                         k2                        IC 3
                 Shift
                 ／뇨Ise         Pin 15           Pin 11     ?n 15            Pin //   ^'i 15           Pin //
                   0            斗 +5              0         ｀첩 +5             0        0                0
                    l
                   2
                   3
                   4
                    5

    c. SerialIn-Parallel O"r

Clear the shift register. Jn this part serial information will be set into the shift register by the serial
input switch. Set the information switch to the voltage indicated and then apply a single shift pulse
to the register. Continue by applying the information into the register until all information has
been set into the register. Read the voltages and enter in Table 10-4E.




                                                            118

===== PAGE 135 =====
                                                       Table 10-4E. Serial in-parallel out.

                                Shift                            IC 1                          /c 2                                /c 3
                Se厄zl           Pulse
            Information        Number                  /in 15           Pin 11        /in 15          Pin //            /in 15             Pin / /
                                   0                         0            0             0                 0               0                  0
                 +5                l
                   0               2
                 +5                3
                   0               4

                  門                5
                 +5                6



    2.   Integrated-Circuit Shift Register


    This part of the experiment uses the 7496 5-bit shift-right shift register. It contains five master-
    slave R-S flip-flops. It has a serial data (DS) input, parallel data input capability (PE and P4 to P。
                                                                                                         ),
    and serial data output capability (Q4). All bits are cleared simultaneously with the CL input. mndi-
    vidual bits can be set through the individual PN inputs gated by the master PE (preset enable) input.
    Figure 10-2 shows the logic block diagram of the 7496.


                                           P0          00               P1       （긔              '2       Q2                  P3           03             P4   O4



  PE




                                                                                                                  ＼∼7
                                   SD                              SD                       SD                           SD                          SD
  DS -0     _                              0    -1■      －               O    --+-
                                                                                                 （그   -       -
                                                                                                                               O    --*-
                                                                                                                                                          （그



                                       0                           1                        2                             3                          4


                                                                                        R        0                R
                                   CD                              CD                       CD                           CD                          CD
                                                                                                                                                     p-   -




  CL

Clock

                                                      Fig. 10-2. 7496 logic block 미agram.




                                                                          프l 9

===== PAGE 136 =====
                  Basic Operation (Figure /0－刃

          Before operating the 7496 shift register, it is necessary to check the LEDs for correct polarity.
     At the junction of the 680-&2 resistor and each LED there is a connection to each of the Q outputs
     (Q4 to Q。   ). Disconnect one of these connections temporarily. This LED should be lit. If not,
     reverse it to make it light. Then replace the connection to the Q output. Repeat for the other four
     Q outputs.
           Set DS (serial data input) to 0.
           Set PE (master parallel input control) to 0.
          Clear all bits by connecting CL (clear) input to 0 and then to +5 V. All LEDs should be dark.
           Set P0, P1, P2, P3, and P4 to +5 V. Set PE to +5 V. All LEDs should be lit.
          Set P0 to P4 to 0. Set PE to 0. Set CL to 0 and then to +5 V. Set P。and P1 to +5 V. Set
     PE to +5 V and then to 0 V. L0 and L1 should be lit and L2.,. L3, and L4 dark.
          Single-pulse the pulse generator. The lit LEDs should move right one bit. Single pulse again
     and continue until all the data have been right-shifted out of the shift register.
          Set ls again into Q。and Q1. Complete Table 10-SE for the 7496 shift register. Use L (lit)
     and D (dark).


                 Pulse generator
                                                                                               +5 V
                     +5 V
                50ps single pulse
                       .r
                  Square wave                                                                           6802
                                                                                                       resistors


                                            '           ＝ㅍ－-
                                                1 CK    CL16
                                                                                 니）
                                                                                         /
                                                                                                        는일Ds
                                                2 P0   （긔. 15
            /
                                                3 Pi    O1 14




            / //
                                                4 P2    Q213
                                     Vcc        5   7496 12
            /
                                    =+5 V                       H   '
                                                6 P3    O311
                                                7P4     O410

                                                8PE     0S 9
            ！
            力
            ／
            -
                                                                                 CRO
                                                                            O VERT
PE
            /
                                                                           O EXT TRIG 1+)
                                                                            O GROUND
DS
            /
     +5 V

                                                Fig. 10-3. 5-bit shift-right shift register.

===== PAGE 137 =====
                                                   Table 10-SE.
                               Shiyt
                               ／뇨lse       L0       L1          L2   L3   L4
                                  0         L         L         D    D    D
                                  1
                                  2
                                  3
                                  4
                                  5


    b.   Circulating Shift Register- Truth Table

     In Fig. 10-3, disconnect wire AB from pin 9 of the 7496 to the serial data (DS) switch.
      Connect a wire from pin 9 (DS) of the 7496 to pin 10 (Q4) of the 7496. This creates a circu-
lating shift register. This is now Fig. 10-4.
      Clear the shift register.
      Set is into Q。and Q1 and complete Table 10-6E as you single-pulse the pulse generator.

                                                   Table 10-6E.
                                Shift
                                /ulse       L0       L,
                                                                乙2   L3   L4
                                  0         L             L     D    D    D
                                  l
                                  2
                                  3
                                  4
                                  5
                                  6
                                  7



    c.   CirculmngShift Reg价er-Data Progression

    Set the pulse generator to 1 pulse per second (pps), or operate the pulse generator manually at
about I pps and visually note the movement of data around the shift register.




                                                          l21

===== PAGE 138 =====
       d.     Circulating Shift Register- Waveforms

     In the circuit of Fig. 10-4, connect the CRO to the 7496 with the pulse generator at single
pulse. Connect the external trigger input to Q0 (pin 15). Use + slope and AUTO trigger (needed to
obtain the waveforms in correct relative timing).
     Clear the shift register and set Q。and Q1.


             Pulse generator
                                                                                                     +5 V
                  +5 V
            50 ps single pulse
                   or
              Square wave                                                                                    680 2
                                                                                                            resistors


                                               …7=         --
                                                                                                            L4
                                               1 CK CL16
                                                                                                                 RED

                                                                              /
                                                2P0     O015                                                     LEDs




                                                                              >/
               O                                3 P1    O, 14
                                                4 P2    O2 13
                ㅇ
                                   Vcc          5   7496    12
                                 = +5 V                          HI·
                                                61'3    O311




                                                                                                  >//>
                ㅇ
                                                7P4     O410
                                                8PE     DS 9
                ㅇ


                ㅇ


                ㅇ
               O
                                                                                       CRO
                                                                                  OVERT
                ○
               O
                                                                                  OEXT TRIG (+)
                                                                                  0 GROUND
+5 V                                                                   그－
                                          Fig. 10-4. 5-bit shift-right circulating shift register.




                                                                            l22

===== PAGE 139 =====
          Set the pulse generator (clock) to 10-kHz square wave and set it as shown in Fig. 10-5. View
     the waveforms(CRO vertical input) at outputs Q。to Q4 and sketch on Fig. 10-5.


                            +5
                  （기ock
                              0


                            +5
                      Q0
                              0



                            +5
                     O1
                              0



                            +5

                              o
                      Q2
                            +5
                     Q3
                              0



                            +5
                     O4
                              0

                                        Fig. 10.5. Waveforms for part 2(d), circulating shift register.



〈包      Quinary            Ring Counter (43210) (Fig. 10-4)

        a.          Single-Pulse Operation

                  Set pulse generator to single-pulse.
                  Clear the shift register.
                  Set Q。 .
                  Complete Table 10-7E using single-pulse operation.




                                                                     l23

===== PAGE 140 =====
                                       Table 10-7E. Quinary ring counter(43210).

                                  Count
                                  ／뇨lse        L0      L'         t2   L3          L4
                                   0           L       D          D     D          D

                                    l
                                   I


                                    3
                                   4
                                    5
                                    6
                                    7


    b.        Waveforms

     Change the pulse generator to 10-kHz square wave. View the waveforms at the Q outputs and
sketch on Fig. 10-6. Do not disassemble the circuit. It is to be modified to Fig. 10-7 for part 4.


                              -           -




                      0


                     +5
         O    [)
  Pin 15, 7496        0


                     +5
         （긔
  Pin 14, 7496        0



                     +5
      Q2
  Pin13, 7496             0



                     +5
      O3
  Pinll, 7496             0



                     +5
       Q4
  Pin 10, 7496            0

                                  Fig. I驪6. Waveformns for quinary counter, part 3.

                                                            l24

===== PAGE 141 =====
     4.    Twisted-Ring or Johnson Counter (Fig. 10-7)



                                                                                                   +5 V
                Pulse 嬖nerator
                     +5 V
               SOps Sin뜨기e pulse
                     Or
                 Square wave




                                                  `*'       -
                                              1 CK    CL16
                                                                                                              L.
                                              2 P。      Q0 15                                             //lLEDs
                  O                           3 P1     ( 1 `4

                                              4 p2      0213

                  O                  vcc      5      7496       12
                                   = +5 V
                                              6 P3      03 11

                  O                           7 p4      O4 10

                                              8 PE     DS 9

                  O
                                                                                 400


          -D      O                                                      VCC= +5 volts to pin 14
                                                                           0 (ground) to pin 7



                                                                                       CRO

                                                                              O VERT
PE                O
                                                                              O EXT       TRIG

                                                                              O GROUND
 +5 V
                                                                     I
                                            Fig. 10-7. Twisted-ring or Johnson counter.


           a.     Single- 뇨lse 0peration

          Clear the counter.
          Set the pulse generator to 1 pps (or manual operation) and visually note data progression
     around the counter.
          Set the pulse generator to single pulse.
          Clear the counter.
          Complete Table I 0-8E as single pulses are applied. Use the LEDs (L and D) to indicate the
     Q levels.




                                                                     l25

===== PAGE 142 =====
                          Table 10-8E. Twisted-ring counter.

                 G)Uflr
                 ／뇨lse         Qo       Qi         Q2     Q3         Q4
                   0           D        D          D       D         D

                    I

                    2

                    3

                    4

                    5

                    6

                    7

                    8

                    9

                   10

                  1l


b.   Waveforms

           +5
 Clock
                                    -
            0

           +5

     Q0
            0


           +5

     （기
            0


           +5

     Q2
            0


           +5

     Q3
            0


           +5
      O4
            0

                          Fig. 10-8. Twisted-ring counter, part 5.

                                             `26

===== PAGE 143 =====
   Clear the counter. Change the pulse generator to 10-kHz square wave (see Fig. 10-8, clock).
EXT trigger from Q0 (POS SLOPE). View Q0 to Q4 and sketch waveforms on Fig. 10-8.


REQUIRED RESULTS

Where logic levels are required to complete tables, use is and 0s. For voltage measurements use
positivelogic I ㅌ >2.5V, 0< 0.5V. ForLEDs, L =l, Dra0.

1.   (a)   Complete Table l0-IR for the data of Table l0-1E. Use the following equivalents for the
           bit numbers.

                Bit I IC 1A, Q output, pin 15                           Bit 4 IC 2B, Q output, pin 11
                Bit2IClB, Qoutput,pin 11                                Bit 5 IC 3A, Q output, pin 巧
                Bit 3 IC 2A, Q output, pin 15                           Bit 6 IC 3B, Q output, pin 11

                                     Table m1R. Parallel input to 6-bit shift register.
                             Bit number         6        S         4        3         2      1
                             Logic level


           Complete Table 10-2R for the serial output at the Q output pin 11 of IC 3 (bit 6) based
           on the data of Table I 0-2E.

                                     Table 10-2R. Serial output of 6-bit shift register.
                             Shift pulse        0         l        2        3         4      5
                             Logic level

     (b)   Complete Table 10-3Ra for the parallel input to the 6-bit shift register of part 1(b) (Table
           I0-3E, shift pulse 0).

                                     Table l0-3Ra. Parallel input to 6-bit shift register.
                             Bit number         6         5        4        3         2      1
                             Logic level

           Complete Table 10-3Rb for the serial output at the Q output pin 11 of IC 3 (bit 6) based
           on the data of Table 10-3E.

                                     Table I0-3Rb. Serial output of 6-bit shift register.
                             Shift pulse        0         1        2        3         4      5
                             Logic level


     (c)   Complete Table l0-4Ra for the serial input to the shift register based on the data of
           part 1(c) and Table l0-4E.

                                      Table 10-4Ra. Serial input to 6-bit shift register.
                              Shift pulse        l        2        3         4        5      6
                              Logic level

                                                      127

===== PAGE 144 =====
           Complete Table 10-4Rb for the parallel output of the shift register based on the data of
           part 1(c)and Table 10-4E(after shift pulse 6).

                                  Table 10-4Rb. Parallel output for 6-bit shift register.
                            Bit number        6             5       4          3        2       I
                            Logic level


2.   Complete Table 10-6R for the shift register (7496) of part 2(b) single pulse and part 2(d)
     waveforms.

                                                   Table lO-6R.
                                nnse        Qo          0   '      Q2        Q3        Q4
                                  0
                                   l
                                  2
                                  3
                                  4


3. (a)     Complete Table 10-7Ra for the count states of the quinary counter (43210 counter)
           based upon the data of Table 10-7E. The 43210 counter is a weighted 5-bit counter in
           which the position of the 1 corresponds to the weight assigned to its position. (Note:
           The position of the I in the code and the location of the stages on Fig. 10-2 are reversed.)

                                 Corresponds to                                Corresponds to
                                     stage 4                                       stage 0

                                                                43210

                                                     Table 10-7Ra.
                                              Count state-quinary counter.
                                            Counr Number                c；끄』
                                                                           〃2r State

                                                   0                      00001
                                                    I
                                                    2
                                                    3
                                                   4


     (b)   Using the wave patterns in Fig. 10-6 for part 3, complete the state table, Table 10-7Rb,
           for the 43210 counter. Also determine the count for each row by adding the weights for
           each state and show this in the last column.




                                                        l28

===== PAGE 145 =====
                                          Table IO-7Rb. State table-43210 counter.
                       Wave Pattern
                          Box             Q4      Q3         02       0   '     Qo       cbunt
                                                         Whg加                         (obtain 介om
                                                                                         sum《7/
                                           4       3         2            1     0    weighted values)
                            l
                            2
                            3
                           4
                            5


4.    Give the count state values for the twisted-ring counter of part 4 in Table 10-8R, based upon
      the data of Table 10-8E or the waveforms of part 4(b).

                                 Table I O-8R. Twisted-ring counter-count states.
                                                                  Cbunt State
                            cbn'ir 7Vumber        이7         QI       Q2        Q3   Q4
                                      0
                                  1
                                      2
                                      3
                                      4
                                      5
                                      6
                                      7
                                      8
                                      9



DISCUSSION

 1.    Compare Table lO-1R with Table lO-2R, Table 10-3Ra with Table lO-3Rb, and Table lO-4Ra
       with Table l0-4Rb, and comment about the ability of a shift register to:
       (a) Shift data.
       (b) Convert binary data from parallel to serial form.
       (c) Convert binary data from serial to parallel form.




                                                       129

===== PAGE 146 =====
2.   Based on the wave patterns of part 2(d), by how much are the data in Q0 output delayed until
     they get to Q4?




3.   A 100-bit shift register has data introduced into it in serial form. The data are being shifted
      with 50-kHz shift pulses.
     (a) How long will it take the data to reach the 70th bit?




     (b) How long will it take the same data to completely circulate through a 100-bit circulating
         shift register and appear in serial form again at the output?




4.   Based on the data of part 2, does a forbidden state in a ring counter continue or does it auto-
     matically arrive at a correct state? Explain the experimental results to illustrate your answer.




5.   Explain the relationship between the count states of the quinary ring counter Tables 10-7E
     and 10-7Ra and the wave patterns of part 3(b). Explain why it is necessary to trigger the
     CRO as indicated to obtain the correct relationship.




6.   A ring counter has developed a fault and the ring has opened. As a result the CRO patterns
     obtained as in part 3(b) cannot be obtained. Explain how you would determine at which
     stage the ring was open by the use of a single-pulse generator.




                                                l30

===== PAGE 147 =====
 7.   What is the relationship between the input frequency and the frequency of the wave seen at
      any of the Q outputs of the five-stage ring counter of part 2?




 8.   What is the relationship between the input frequency and the output frequency of the five-
      stage twisted-ring counter?




9.    What is the angular phase relationship between successive stages of a five-stage twisted-ring
      counter?




10.   Sketch the expected waveforms for a three-stage twisted-ring counter at the Q and Q outputs.
      What input frequency would be required to give a 60-Hz output? What is the phase relation-
      ship at the Q outputs between successive stages of the counter?




11.   Explain how a shift register and parallel adder are used in the arithmetic operation of multi-
      plication.




                                               13l

===== PAGE 148 =====
                                                                 ExperimenI B



Pulse Forming and Shaping;
The Schmitt Trigger




OBJECT


     1.   To study the transistor astable multivibrator.
     2.   To study the IC astable multivibrator.
     3.   To study the pulse stretcher/monostable.
     4.   To study the Schmitt trigger.


INTRODUCTORY THEORY


Astable Multivibrator


Figure 11-1 shows the circuit diagram of a transistor multivibrator. As can be seen, two transistors
are used in this circuit. Whereas in a transistor bistable the transistors were dc-coupled, leading to
stable conditions until disturbed by an external signal, the transistors in Fig. 11-1 are capacitor-
coupled. This results in two quasistable states, with Q1 conducting and Q2 off, and then Q1 cut off
and Q2 conducting. This interchange of conduction and cutoff condition occurs without any ex-
ternal signal. As will be shown shortly, the time each transistor is in the cutoff condition is deter-
mined by the time constant of the resistor and capacitor connected to its base. The circuit acts
to charge and discharge the coupling capacitors automatically.


                                                           133

===== PAGE 149 =====
                            Vcc                                                           Vcc



                                                                                                              C2




                 (a) Cascade representation                                 (b) Conventional representation
                                         Fig. 11-1. Astable multivibrator.


                                                                                 T = 0.7 RC




                        (a) RCcircuit                                        (b) VA versus time
                                          Fig. 11-2. Dc charging circuit.

     Consider a capacitor, resistor, and batteries as shown in Fig. 11-2. If the switch is closed, the
voltage across the capacitor is equal to V volts with point A at a voltage of -V volts. If the switch
were open, the A voltage would have to be +V volts. Now,start with the switch in the closed posi-
tion and open it at time t = 0. The voltage at point A must go from -V to +V with time constant
r = RC. We will be interested in the time it takes the voltage at A to go from -V to 0 V. Zero volts
is halfway between -V and +V. The capacitor has charged to half of its final voltage. This means
that we have to determine T in

                                                 0.5 = i - E -T/RC

The value of T that satisfies Eq.(1 니 ) is

                                                 T = 0.7RC = 0.7r

     We now have to show how the circuit of Fig. 11-1 performs the capacitor charging of Fig. 11-2.
     The circuit of Fig. 11-1 is a saturated circuit, to satisfy the conditions for saturation,

                                                                      H

                                                                                                                   (11-3)
                                                                k`
                                                        and
                                                                     1J -    '   1



                                   쫓B!   ci <hFEI              瓦길<- FE2
Assume that the VBE of the conducting transistor is equal to 0.
    To start, assume that Q1 is conducting and in saturation and Q2 is cut off, with a voltage across
C2 making the voltage at the base of Q2 = -Vcc volts (this surely cuts off Q2). Since Q2 is off, the




                                                        료34

===== PAGE 150 =====
voltage at the Q2 collector side of C1 is equal to Vcc and the other side of C1 connected to the base
of Q1 is at 0 volts. C1 therefore has a voltage equal to VcC across it.
     Now let us consider capacitor C2. At the Q1 collector side of C2 its voltage is equal to 0 and
at the other side (at the base of Q2) its voltage is equal to -vCc. We see that it will act like the
capacitor C of Fig. 11-2 at the time its switch was opened.
     In Fig. 11-1, Q2 is cut off, and therefore its base does not conduct. C2 charges toward +Vcc
through RB2, as did capacitor C of Fig. 11-2. When the voltage at the base of Q2, VBE2, reaches 0,
Q2 is turned on. Both its base and collector conduct heavily. This stops the charging of C2 toward
vcc. The time for the capacitor C2 to change its voltage from -Vcc to VBE2 = 0(halfway between
-Vcc and +Vcc)is given by Eq. 11-4.

                                             T=0.7R82C2                                         (11.4)

     As Q2 is turned on, its collector voltage rapidly goes to 0 V. However, capacitor C1 was
charged with a voltage Vcc across it, with the negative side of the voltage at the base of C1. It takes
time for a capacitor to change its voltage(RC time constant). Q2 turns on too rapidly for the charge
on C1 to change. As a result the voltage across C1 is maintained and the base of Q1 is driven to
-VCc volts. The operating condition of the two transistors now have been interchanged and the
process repeats. Q1 is now nonconducting for a time given by Eq. 11-5.

                                             T = 0.7RBICI

and the total time for a complete cycle is

                                        T = 0.7(RHICI + RB2C2)

If the circuit has identical components, R81 = RB2 = RB and C1 = C2 = C,

                                              T= l.4RBC

When the off transistor is turned on, its negative-going collector voltage is applied through the
coupling capacitor to the base of the on transistor. For a brief period of time both transistors are
conducting and in a regenerative mode. This speeds up the transition, which for an astable multi-
vibrator made with small-signal silicon planar transistors takes place in nanoseconds.
     Let us now consider the collector wave shape. In Fig. 11-1 we began with Q1 on and Q2 off.
Capacitor C2 had charged to the point where the voltage at its B2 side was equal to 0. Q1 had been
in saturation and the voltage at the Q1 collector side of C2 was essentially 0(VCESat Of Q1). At the
transition time the voltage across C2 was therefore equal to 0. After the transition Q1 is off and
the voltage on the B2 side of C2 must stay at 0, since Q2 is on. Since Q1 is off, C2 must charge
through Rc1 to vcc. The voltage at the collector side of the off transistor Q1 rises with a time
constant.

                                               r= Rc1C2                                          (11-8)

When a transistor turns on, RSa1 is a low resistance and the transition is sharp and very rapid. Figure
11-3 shows the wave shapes of Q1. The wave shapes of Q2 are the same except for the timing.
     If the collector waveform of Fig. 11-3 is to be made more square, the time constant Rc1C2 has
to be reduced. This can only be done by reducing Rc1, since changing C1 would change the time for
a cycle. But reducing Rc1 is in conflict with Eq. 11-3. Nevertheless, by using high hFE transistors,
a reasonable approximation to a square wave can be attained. The turn-on edge is always quite
sharp and is normally used for timing purposes.




                                                 l35

===== PAGE 151 =====
                              vcc
                  Collector
                  ofO1
                              0

                                          -p
                                                   F         T= 0.7 RB1
                                                                          RC1C2[                      f
                    Base 0
                    of O1
                              Vcc                                                                     l/
                                    Fig. 11-3. Collector and base waveforms of Q1.

     An IC astable multivibrator similar to the transistor astable can be made with two inverter
gates by capacity coupling successive gate outputs to inputs. In TTL no input transistor base is
brought out to a terminal pin. Therefore, to provide starting gain, it is necessary initially to bias the
gate transistors in the active region. This can be done with collector feedback resistors as shown in
the IC astable of Fig. 11-4. When operating, the output transistors are, as in the transistor astable,
driven into saturation. In the IC astable it is not possible to derive a simple expression for the
period.




                                    T_                            L        > i
                                                             Fig. 11-4. IC astable.
                                                                                          '




Pulse Stretcher


The pulse stretcher shown in Fig. 11-5 is used to extend a pulse width to provide additional time
for logic operations. The pulse width at B is longer than that at A because it takes capacitor C time
to charge up to the threshold voltage of gate 2.



            J그－ 늬 , 직，.                                               中
                                                                                                  느        」H
                                                                      T
                                                                                              〉
                                                                                      2
                 '
                                               '    -   TI
                                                                            C
                                                                      ―
                                                   Fig. 11-5. 1c pulse stretcher.

                                                                      l36

===== PAGE 152 =====
Schmitt Trigger


The Schmitt trigger is a regenerative circuit that switches output logic levels very rapidly when its
input voltage exceeds specific levels known as the trip levels. The higher voltage, called the upper
trip level.(UTL), causes the output to switch in one direction and the lower voltage, the lower trip
level(LTL), causes the output to switch and revert to its original state. This enables a slow-changing
voltage to be converted to a rapidly changing voltage at the trip points. This enables transfer of
information through small capacitors and also limits the time a switched gate is required to remain
in the active region. It also provides noise immunity.
      The difference in voltage between the UTL and LTL is called the hysteresis. Schmitt trigger
gates have a hysteresis symbol within their logic symbols (Fig. 11-6):

                                          hysteresis = UTL - LTL volts




                                     Fig. 11-6. Schmitt trigger NAND gate.


EQUIPMENT REQUIRED


     CRO,dc coupled and calibrated
     Power supply, +5 V dc at 50 mA
     IC type 7400, quad 2-input NAND gate
     IC type 7403, quad 2-input NAND gate open collector
     IC type 7414,hex Schmitt trigger inverter
     Two transistors, small-signal silicon, hFE mmn = 40(T1S98 or equivalent)
     Silicon sma끄-signal diode, 1N457, or equivalent
     Two 820- 2, 10% composition resistors
     Two 100042, 10% composition resistors
     Two 5600-11, 10% composition resistors
     Two 27,000-11, 10% composition resistors
     500-11, 3-turn potentiometer
     Two 0.01-pF capacitors
     Two 0.022-MF capacitors
     Two 0.033-jiF capacitors
     Square.wave generator, +5 V at 10-kHz or 50-'zs single pulse
     Sine-wave oscillator, 10 V p·p at 1000 Hz

                                         IC manufacturers' part numbers.

                                                                   Texas          National
                  Type        Motorola           Fairchik/     Innrumep甘1       Semicondwm7'

                  7400        MC7400P            7400PC         SN7400N           DM7400N
                              MC7400L            7400DC         SN7400J

                  7403        MC7403P            7403PC         SN7403N           DM7403N
                              MC7403L            7403DC         5N7403J

                  7414        MC74l4P            7414PC         5N7414N           DM7414N
                              MC7414L            7414DC         SN74l4J


                                                        l37

===== PAGE 153 =====
EXPERIMENTAL PROCEDURE


For all ICs in this experiment: VCc = +5 V to pin 14,0(ground) to pin 7.


1.   Transistor Astable

                                         +5 V

                                           !


                              輸
     Rc
                                                                RB2               C2




      （기
                                                                                Q2

                                                                               （기 = O2 = 지S98
                                                                                Rci = Rc2 = 1 k요

                                                                                RB1 = R82 = 27 k2
                                                                                C1,C2 see below



                                    Fig. 11-7. Transistor astable.


     (a)   C1 = 0.01 pF. C2 = 0.01 pF.
                On Fig. 11-8 sketch the waveforms of VCE1, VBE1, VCE2, and VBE2. Show thevoltage
           amplitudes and the time scale so as to be able to measure the frequency. Use external
           TRIG from the collector of Q2. At least two complete cycles should be shown.
                From the CRO waveforms enter data in the column marked la in Table li-1E.
           Do not proceed until your data have been checked by the instructor.

                                                                Table li-1E.
                                                                 la      lb
                                   Time（기 is in saturation
                                   Time Q2 is in saturation


     (b)   C1 = 0.01 ' tF, C2 = 0.033 MF.
                Sketch the wave shapes of VcE1, VBE1, v cE2, and VBE2 on Fig. 11-8. Particularly
           note the effect changing C1 from 0.01 PF to 0.033 pF has on the positive-going wave
           shape of the collector of Q2 and indicate this on your sketch. Enter the appropriate
           data in column lb of Table il-lE.




                                                 i38

===== PAGE 154 =====
                  Part 1 (a)                                                       Part 1 (b)



 VCE1                                                         VCE1




 VBE1                                                         VBE1




 VCE2                                                         VCE2




 VBE2                                                         VBE2



                          Fig. 11-8. Waveforms for parts 1(a)and 1(b).


2.   IC Astable

                                                        82012
                                                        一 _




                               /N   <           "




                    i      '        녀
                                        I   "       I
                                                        ：         'p
                                                                       \
                                                                           '   T
                                                        82012

                                    Fig. 11-9. ICastable.




                                                            l3,

===== PAGE 155 =====
                        V.   ,

                        p뉴t2(a)




                         vipart 2(a)



                                           Fig. 11-10. Waveforms for part 2.


      (a)   Cj= C2 =0.01pF
            Sketch the wave shapes at pins 3 and 1 on Fig. 11-10. Use external triggering from pin 3.

                                                  Time per cycle =

     (b)    C1 = C2 = 0.033 .tF

                                                  Time per cycle =


3.   Pulse Stretchers


     (a)    In the circuit of Fig. 11-11 with the SWG at 10 kHz, using external + trigger for the CRO
            from the SWG, sketch the wave shapes of the SWG and the output at pin 6 for C = 0.033
            〃F on Fig. 11-12. Plot two cycles of the wave shapes. Complete Table ll-2E.


                                                                               Vcc

                                     CRO
                                 EXT (+) TRIG
                                                                               I
                  SWG
                 10kHz
                  +5 V
                    or
               Single pulse
                  50 jls




                                                Fig. 11-1L Pulse stretcher.




                                                           140

===== PAGE 156 =====
               V SWG




               V pin 6




                             Fig. 11-12. Pulse stretcher wave shape.



                                                Table ll-2E.
                               c           Pulse Width at Pin 6 rpositive Sectio까
                                이』
                                 F
                             0.01 pF
                            0.022pF
                            0.033 pF



(b)   The circuit of part 3(a) was operated with a repetitive 50-as positive-going pulse genera-
      tor, but in this part it will be operated on a single-pulse basis. To view the pattern on a
      single-pulse basis requires that the CRO horizontal sweep controls be set so that a single
      pulse will trigger it. This is done by means of the level control.
            Start by setting the pulse generator at 10 kHz and C at 0.01〃F. View the output
      at pin 6 using + internal trigger and AUTO mode.
            Change the pulse generator to single pulse.
            Adjust the CRO level control(s) until a positive-going output pulse is seen for each
      single pulse from the pulse generator. Complete Table 11-3E.

                                                Table 11-3E.
                                            c          Pulse Wiith
                                         0.01 /IF
                                         0.022 jiF
                                         0.033 iiF
                                         0.055〃F
                                         0.065 pF




                                              l4l

===== PAGE 157 =====
4. Schmitt Trigger

    a.   Characteristics(Figure 7／·／刃


                                             +vcc




                                        500 &2




                                                    ng. 료l-i3.


      Begin with the 5004k potentiometer at 0 V (ground). Monitor the output voltage. Slowly
increase the inverter input voltage with the potentiometer until the output voltage switches from
level 1 to level 0. Measure the input voltage (UTL)                                UTL = --.- volts
      Again monitoring the output voltage, slowly decrease the input voltage until the output voltage
switches from level 0 to level 1. Measure the input voltage (LTL)                  LTL = --- volts


    b.   "駒uare" Wave from Sine WaverFigure //-／刃



                                                                                   CRO
                                                                           VERT
            1 kHz
          Sine wave
          generator                                                        EXT (+) TRIGGER
         10 volts p-p




                                    Fig. 11-14. "Square"-wave generator.


     Sketch the waveforms on Fig. 11-15 at points A (sine wave), B (clipped sine wave), and C
((Schmitt trigger output-square wave). Show between two and three cycles.




                                                       142

===== PAGE 158 =====
                 +5
           A
                  0




                                                                                                 1
                +5
           B
                  0



                +5
           C
                  0

                                 Fig. 11-15. "Square"-wave-generator waveforms.


REQUIRED RESULTS

1.   From Table 1 1-1E, complete the following in Table 1 1-1R.

                                                     Table 11-jR.
                                                                            ／뇨lse
                                         끄玎α／ Time                        RePetim가＇
                                         per Cycle          Frequency       Rate
                                 Ia
                                 lb


2.   (a)       In part 2, an approximate formula for the total period of the IC astable can be given as

                                                            P = AC

               where P is in microseconds, C in picofarads, and A is a constant. Determine the value of
               A for the experimental values of part 2(a).
     (b)       Using the values of C = 0.033 !IF in part 2(b), compute the period of oscillation using the
               value of A from part 2(a) and compare with your experimentally determined results.




3.   (a)       From the data of part 3(a), plot a curve of the amount the positive section of the or'
               pulse is stretched. (Increased in width compared to the width for C = 0.)




                                                      l43

===== PAGE 159 =====
                         0         0.01       0.02       0.03        0.04   0.05
                                          Capacity- C- Microfarads
                             ng. 11-16. Stretched pulse vs. capacity.


(b) From the plot determine the value of the constant N in

                                                     △P= NC

      where △P is in microseconds and C is in microfarads.




(c)   Plot the data of part 3(b) on Fig. 11-17.




                Pulse
                Width
                PS




                         0         0.02       0.04       0.06        0.08   0.10
                                            Capacity -   Microfarads

                               Fig. 11-17. Monostable pulse width.


(d)   From the plot determine the constant H and J in the formula

                                                 PW = HC + J

      where PW is the stretched pulse width in microseconds and C is in microfarads.




                                               144

===== PAGE 160 =====
4.   Compute the hysteresis of the IC Schmitt trigger.




［기SCUSSION

1.   In part I, explain why the collector negative-going transition is sharp and the positive-going
     transition is not.




2.   In part 1(a), compare the total period of the transistor astable with the theoretical value of
     1.4RBC.




3.   In part 1(b), compare the total period with the theoretical value.




4.   What are some possible applications for the pulse stretcher?




                                                 l4S

===== PAGE 161 =====

===== PAGE 162 =====
                                                                       ExperimenI 12



InIe9raIed-CircuiI Timers-
The7q122,7'1121,and555



OBJECT


     1.   To study the properties of the 74122 retriggerable resettable monostable multivibrator.
     2.   To study the properties of the 74121 monostable multivibrator.
     3.   To study the properties of the 555 timer.


INTRODUCTORY THEORY


Although the basic theory of the astable and monostable multivibrators has been studied in Experi-
ment 11, the development of integrated-circuit timers has provided circuit designers with logic
blocks of imnroved characteristics. All of these timers orerate by charging and discharging capaci-
tprs inrougn resistors, it is oniy necessary to aau external K anti U to set tne time or operation.
For additional simplification, some of these ICs have internal timing resistors.


The 74122(TTL Monostable)


Triggering occurs at a particular voltage level. Both positive- and negative-going trigger pulse edge
inputs are availab'e. When it is in its delay state, another trigger pulse applied to its trigger inputs
will cause the delay period to be triggered again and repetitive trigger pulses can make the delay
period as long as desired. For external capacitors greater than 1000 pF, the output pulse width PW
isgivenby Eq. 12-1:

                                      PW = 0.32RxCx(l.0 + 0.7/Rn)        fls                        l2-l)

                                                       147

===== PAGE 163 =====
where R,(in k2) and C, (in pF)are the external resistor and capacitor. The PW can be terminated
externally at any time by an appropriate input to the CD input. The logic symbol for the 74122 is
given in Fig. 12-1.



                                                                            8




                                      B   3

                                       B2 4




                               Fig. 12-1. 74122 retriggerable monostable.

The 74121 (TTL Monostable)
                                      外 三ltk-叱 M"-
                                                                     1-
                               큰ce.
Triggering occurs in the same manner as in the 74122. Once triggering has occurred, an internal
feedback latch acts to disable the input trigger circuit and prevents retriggering while the output
pulse is occurring. The pulse width PW is given by Eq. 12-2.

                                          Pw . 0.69RxC,     nS                               (12.2)

where Rx (in kZ) and C, (in pF) are the external resistor and capacitor. The logic symbol for the
74121 is given in Fig. 12-2.




                                      Fig. 12-2. 74121 monostable.

The 555 Timer (Linear)

The IC is not a TTL IC but is based upon linear IC technology. Therefore, it is not subject to TTL
supply voltage limitations but can operate up to a supply voltage of 18 V. Both monostable and
astable operation is available. Larger values of timing resistors (up to 2.7 M2) can be used corn-
pared to the 74121/22, which are limited to 40 k2, and it is capable of sinking much greater cur-
rents than the 74121/22 ICs. Within the IC, two voltage levels are set up at 吉VcC and 층Vcc by
means of three 5-k7 resistors.


                                                  l48

===== PAGE 164 =====
Monostable Mode[Figure /2．
                         了rα〃

     An external resistor R and C determine the timing. A negative-going triggering pulse is applied
to the trigger input. The capacitor charges through R up to 층Vcc and is then discharged. The pulse
width is given by Eq. 12-3, where R is in ohms and C is in farads:

                                                      PW= 1.IRC                 S                                                (12-3)

                         +vcc                                                                                +vcc




                           (a)
                                                                                                               (b)
              ng. 12-3(a). 555 monostable.                                                          Fig. 12.3(b). 555 astable.


Astable Mode[Figure 12-3(b)]                        1                                               어2只7卄디       d L 戶n』／%,

     In the astable mode the circuit retriggers itself. Two resistors, RA and RB, are used. The tim-
ing capacitor charges through RA and RB to 궁 V4c and discharges through RB to 去VCc, where the
circuit is retriggered. The charge time Tl (output high) is given by Eq. 12-4 (RA and R8 in ohms,
C in farads).
                                      T1 = 0.693(RA + RB)C                                    (12-4)

The discharge time T2 (output low) is given by Eq. 12.5.

                                                    12 = 0.693(R8)C

The total time for one cycle is given by Eq. 12-6.

                                      T = T1 + T2 = 0.693(RA + 2RB)C

The frequency f is given by Eq. 12-7.


                                                               f그－        Hz                                                     (12-7)
                                                                 T

The duty cycle D is given by Eq. 12-8.

                                      time     p
                                                                                                                                 (12-8)
                                 D=
                                             (out
                                                      utlow)      =   -   T2-       =   -   -   R
                                                                                                    Bh
                                         total time                   1 l + 12          2KB + KA



                                                                149

===== PAGE 165 =====
          EQt기PMENT REQUIRED


               CRO, dc coupled and calibrated
               Dc power supply, +5 V at 50 mA, regulated
               IC type 7404 hex inverter
               IC tvoe 74121 monostable multivibrator
               IC type 74122 retriggerable resettable multivibrator
               IC type 555 山ner
               SWG, +5 V, at 100 Hz to 10 kHz or 50- .zs single pulse
               Capacitor, I pF, tantalum
               Capacitor, 10 pF, tantalum
               Capacitor, 100 iF, tantalum
               kesistor, I kQ
               Resistor, 27 k2
               Resistor, 1 M&7
               Resistor, 470 n
               Red LED
               Switch bank

                                                   IC manufacturers' part numbers.
                                                                    Texas           National
                      Type        Motorola        Fairchi緘       InsnumenrS       Semicon/uctor       Signetics

                     555         MC1555           NE5 55              SN72555        LM555             555
                                 MC1455                                              LM555C

                     7404        MC7404P          7404PC              5N7404N        DM7404N
                                 MC7404L          7404DC              SN7404J

                     74121       MC74121P         74121PC             SN7412lN       DM74121N          N74121
                                 MC74l21L         7412lDC             5N74121J

                     74122       MC74122P         74122PC             SN74122N       DM74122N          N74122
                                 MC74l22L         74122DC             SN74122J



          EXPERIMENTAL PROCEDURE


①74122*               (Figure 12-4)


               RX = 27 k2
               cx = I zF
               A1 and A2 to 0
               B1 and CD to +5 V



                *Should the 74122 hang-up (fail to operate), CRO isolation may be required. Either follow the procedure dis-
          cussed in "To the Instructor" or use an oscilloscope probe.




                                                                  150

===== PAGE 166 =====
                          +5 v이ts
                                     Rx                          Cx




                                    缸                     13rh,,
                ＼℃―'`V-
                                    ^/V`_
                            O

                                                           RX         Cx
                            O                              Cx          Q                 VERT.




       ＼ 沖 ― X℃―1
                                                            74122                           CRO
                            O

                                                   -BB
                                                    .




                                                    ' 2
                            0                  -
                                                                 CD

                                               -
                                                                           Vcc =+5 V to pin 14
                                                                            0(ground) to pin 7
       Pulse generator
Single puke + 5 volts(JL)
            50 p5
              or
    Variable frequency
   Square wave +5 volts


                                    Fig. 12-4. 74122 야．
                                                      eration.


(a)   Using Eq. 12-1, compute the approximate PW.
            Set the CRO horizontal sweep rate so that the CRO will display this PW over
      approximately half of the screen width horizontally. Set the pulse generator to single-
      pulse (50 .Ls) and apply single pulses to trigger 74122. Measure the pulse width accu-
      rately by using the CRO trigger level control to display each output pulse at the same
      position on the CRO, beginning at the left side of the display. 1'his is done by advancing
      the level control until the output pulse is displayed in this manner.

                                      Pw =

(b)   Set the horizontal sweep rate so that the pulse is displayed with a width of approxi-
      mately one major division horizontally. Set the trigger level control to AUTO. Change
      the pulse generator to I 0-kHz square wave. Sketch the Q output on Fig. 12-5.

           +5
                0

                                    ng. 12-5. 74122 waveform.


(c)   Reduce the frequency of the pulse generator until the Q output just begins to have a
      section at 0 V. Record the frequency at which this occurs.

                                       f=
                                              l 51

===== PAGE 167 =====
     (d) Reduce . the frequency of the pulse generator until the Q output is approximately a
         square wave.
         1. Change CD to 0 V. What is its effect?




            2. Return CD to +5 V. Connect B1 to 0 V. What is its effect?




           3. Return B1 to +5 V. Connect A1 to +5 V. What is its effect? Then also connect
              A2 to +5 V. What is its effect?




2.   74121* (Figure 12-6)


      Rx = 27kn               +5 volts
      C, = I pF
      A1 and A2 toO



                                                                      Rx    Cx
                                                                      C',

                                                                       ^     Q

                                                                        74121


                                                                ㅍ）
                                                                      Vcc =+5Vtopin14
                                                                       0 (ground) to pin 7
                                        Pulse generator
                                 Single pulse +5 volts (JL)
                                             50 Ps
                                              or
                                      Variable frequency
                                    Square wave +5 volts


                                                         Fig. l2.6.

     *楡e comments for the 74122-CRO isolation.

                                                  152

===== PAGE 168 =====
        (a)         Using Eq. 12-2, compute the approximate PW.
                         Set the CRO horizontal -sweep rate so that the CRO will display this PW over
                    approximately half of the screen horizontally. Applying single pulses (50 Ls), measure
                    the pulse width PW as in part 1(a).

                                                 Pw =

        (b) Set the horizontal sweep rate so that the pulse is displayed with a width of approximately
            one major division horizontally. Set the trigger level control to AUTO. Change the pulse
            generator to 10-kHz square wave. Approximately sketch the Q output on Fig. 12-7.




               1-
                                               Fig. 12-7. 74121 wavefonn.

        (c)         Change C,, to 10 pF and as in part 2(a), using single pulses, measure the pulse width.

                                                 Pw =

        (d) Change C,, to 100 j.tF and measure the pulse width.

                                                 Pw =


                                                                           vcc= +5 V
             Timer

                                                                               I
（段555
        a.   MonostablerFigure /2－引

         R = 27 kn                                                         4             8
         C = I 1iF                                  R1 =             RESET             VCC
                                                    1 kQ
                                                                     TRIGGER

                                                                               555



                                                                            GROUND
                                                   470 fl                          1


        Fig. 12-8. 555 monostable                             LED
                   operation.




                                                                                         7404

                                                      Pulse generator
                                                   Single pulse +5 volts
                                                       50ss (J1쟈
                                                                                         Vcc= +5 V to pin 14
                                                                                          0 (ground) to pin 7

                                                            153

===== PAGE 169 =====
        Following the procedure of part 1(a)(Eq. 12-3), compute and measure the PW across RL.

                                  measured PW =

Connect the CRO across C and sketch the waveform. (Note: Use the external trigger on the CRO
from the output terminal of the 555-pin 3.) Sketch the output across RL also. Sketch on Fig. 12-9.

                  +5
              C
                   0


                  +5
         RL       。


                                    Fig. 12-9. 555 monostable waveforms.


   b. Monostable (Figure 12-8)

    R = 1 Mf
    C = 10uF

    Measure the PW using the timt the LED is lit.

                                     Pw =

   C.    月stab!아Figure 72·7이

    RA= 27 kZ
    kB = l아c2
    C = 1〃F
                                                  VcC= +5 V




                           RL
                         = 1 kn




                                      Fig. 12-10. 555 astable operation




                                                    l54

===== PAGE 170 =====
    Sketch the output waveform across RL and the waveform across C. The waveforms should
show times and voltage levels. Sketch on Fig. 12-11.

                                       T1 (high)=

                                       12 0ow)=
                                       T=


            +5
       RL
              0



              5
       C
              0

                                       Fig. 12-11. 555 astable waveforms,


REQUIRED RESULTS


Complete the following tables.

                                            Table 12-JR. Monostable.

                                                                      /)11/       P1t/       Percem
            Part     /C           RX            cx
                                                                   Computed     Measured    Difference

            1(a)   74122         27 kQ               1 iF

            2(a)   74121         27 k7               1 jiF
            2(c)   74121         27 k2         10uF

            2(d)   74121         27 k2        100 iF

            3(a)     55 c        27 k2               1 1iF
            3(d)     555          lMn           l0旴



                                       Table 12-2R. 555 Astable-Part 3(c)

                                                                                Percent
                                          cbmputed                 ^feasured   Difference

                            T (high)

                            T (low)

                            T
                            f

                            D




                                                             l55

===== PAGE 171 =====
DISCUSSION

I.   Discuss the results of Table 12-IR and 12-2R with respect to the differences between the corn-
     puted and measured results.




2.   Discuss the wave pattern of parts 1(b) and 1(c). What is the relationship between the frequency
     at which there is a 0-V section and PW?




3. Compare the wave patterns at a 10-kHz pulse generator input for the 74122 [part l(b)1 and the
   74121 [part 2(b)!. Explain the differences.




4. In order to use the pulse generator of Figs. 12-4 and 12-6 with input into the A terminals, it is
   necessary to place an inverter between the pulse generator and the A terminals. Explain.




5.   Based upon the 74122 logic diagram of Fig. 12-1 and your experimental data of part 1(d),cx-
     plain the operation of inputs A1, A2, B1, and C0. Can you suggest applications for these
     inputs?




                                                l56

===== PAGE 172 =====
                                                                         Experimenl 13



Decodin9 and Encodin9




OBJECT


     I.    To study the operations of decoding of electronic counters.
     2.    To study the operations of encoding and code conversion.


INTRODUCTORY THEORY


Decodit四

Electronic counters count in binary or some form of modified binary. Many applications such as
display device activation, multiplexing, and timing require conversion from the binary systqm and
its multibit count state to some form of decimal or single-output representation. This conversion
process fjqm binary to 笠坐뜨la1iskr으싼브s ecodin. This conversion makes「'use of an AND gate
whose inputs are the count state of the counter. Since any divide-by-N counter has N count states,
each count can be decoded by such an AND gate and N AND gates are required to decode all of the
counter states. For example, the two-stage binary counter shown in Fig. 13-I divides by 4 and has
four count states. To decode all four states requires four two-input AND gates with the decoding
shown.
      When the full count capability of a k-stage binary counter (=21c) is used, decoding all the count
states requires 2' gates with K inputs to each gate. When the count capability of a k-stage counter
is reduced to a value N, N gates (one for each count state) are required to decode the N count
states. However, there is some redundancy in the decoding and not all the decoding gates require
K inputs. This, therefore, results in decoding simplification.


                                                       l57

===== PAGE 173 =====
                                                                                        nn
                                                                                  -A
                                   A                               B                      0
         Clock- T           FFA                          FFB                      -B
                                           1-
                                                T                  百
                                   A
             H--0--04o--1- P40- 2_ *40-                    3- .4                  A
                                -                              -

     Clock                                                                                1
                                                    -
                                                                                  B
        A
             I          I              I            I
        A    I          I              I            I_
        B

        B


                            Fig. 13.1. 2-stage binary counter waveforms and decoding.



Encoding-Code Conversion


Encoding is the opposite of decoding. A binary code is generated for each given decimal value.
Encoding requires an 0R operation for each bit of the output code. The inputs to the OR gate are
determined by the decimal-to-output conversion requirement. Frequently, there is a requirement to
convert from one binary code to another. A straightforward procedure frequently employed is to
decode the initial binary code and then encode the new code.


EQUIPMENT REQI기RED


     CRO, dc coupled and calibrated
     dc power supply, +5 V at 50 mA
     IC type 7404 hex inverter
     Two IC type 7420 dual 4-input NAND gate
     IC type 7441/74141 BCD-to-deciinal decoder
     IC type 7447 BCD-to-seven-segment display driver
     IC type 7476 dual J-K FFs with PRESET and CLEAR
     IC type 7490 decade counter
     Seven-segm,ent LED display, MAN 71A/MAN 72A or equivalent
     Two switch banks, 5 switches per bank
     Seven 68042, 土10% composition resistors
     5.6-k2. 土10% composition resistor
     SWG, +5 V at 10 kHz or single-pulse 50 pa




                                                           l58

===== PAGE 174 =====
                                         IC manufacturers' part numbers.

                                                                      T匕xas            National
                      Type    4fotoro仇         Fairchild          Instruments        Semiconductor

                      7404    MC7404P             7404PC          SN7404N             DM7404N
                              MC7404L             7404DC          SN7404J

                      7420    MC742OP             7420PC          SN7420N             DM7420N
                              MC7420L             7420DC          SN7420J

                      7441A   MC7441AP            7441PC          SN74141N            DM7441AN
                              MC744IAL            7441DC          SN74141J            DM74141N

                      7447    MC7447P             7447PC          SN7447H             DM7447H
                              MC7447L             7447DC          SN7447J

                      7476    MC7476P             7476PC          SN7476H             DM7476N
                              MC7476L             7476DC          SN7476J

                      7490    MC7490P             7490PC          SN7490N             DM7490N
                              MC7490L             7490DC          SN7490J



EXPERIMENTAL PROCEDURE

                                                                                                TO CR0
1. , Decoding                                                                                   EXT TR G (NEG)
  구
                                                                                                      ^
      a.     2Stage及nα＇:},                                        7476
             0unter

                                             PR                                           PR
                                                       15                                           11   B
                                         J         0                                  J         0



                                    C CK                                         0 CK

                                                                                12
                                                   Q          A                       K         百 뜨－－百
                                             CLR                                          CLR




                                                                                                         I




            SWG
            +5 V
           10 kl- z




                                                   Type 7420         `/cc 볍+5 V to pin 14, 0 (ground) to pin 7
                                                   Type 7476         \/cc= +5 V to pin 5, 0 (ground) to pin 13

                                Fig. 13-2. 2-stage binary counter decoding gate.

                                                            l59

===== PAGE 175 =====
         +5
Clock
                   0



              +5
1 {a)1
                    0



              45
1(a)2
  A                     0



               +5
1(a)3
  B
                        0



                   +5
1(a)4
  B
                        0



                   +5
1(a)5
 AB                     o



                   +5
 1(a)6
 AB
                        0



    7+5
](a)
1(a)]
 AB
                        0



    8+5
1(a)8




                            Fig. 13-3. Waveforms for part 1(a .




                                           160

===== PAGE 176 =====
     View and sketch on the curve sheet of Fig. 13-3 the following waveforms:

     1.    0utput A waveform
     2.    Output A waveform
     3.    Output B waveform
     4.    Output B waveform

     For the following waveforms, pins 4 and 5 of the 7420 NAND gate can be left unconnected.

   5. NAND gate output (pin 6-type 7420)for input A to pin 1 (type 7420)and B to pin 2(type 7420)of the
NAND gate.
   6. NAND gate output (pin 6-type 7420)for input A to pin 1 (type 7420)and B to pin 2(type 7420)of the
NAND gate.
   7. NAND gate output(pin 6-type 7420)for input A to pin 1 (type 7420)and B to pin 2(type 7420)of the
NAND gate.
   8. NAND gate output (pin 6-type 7420)for input A to pin I (type 7420)and B to pin 2(type 7420)of the
NAND gate.


    b.    Mod-3 counter

     In this part of the experiment, the counter will be decoded for each of the count states, and
each decoding operation will be examined for possible redundancy.

                                                                                          To CRO Ext Triq (negi
                                                                                                  1



                          n                                        7476



                                        PR          15 A                             PR       11 6
                                   J            O                               J         O



                                   아
                                   （                                      6   0 CK

                                                                                              10 B
                                   K            0                               K         O
                                        1 L M                                       CLR



                          L-
                               -    -     -     -   -   -
                                                               -
           SWG
           +5V
          1아쥐z

                                                            Type 7476 VCC = +5V to Pin 5. 0 (ground) to Pin13
                                                            Type 7420 VCC = +5V to Pin 14, 0 (ground) to Pin 7

                                   Fig. 13-4. Mod-3 counter-decoding gate.

                                                              I6l

===== PAGE 177 =====
                    +5
         이0아＜
                              0




                         +5
         1(b)2
           A 0



                    +5
         1(b)3
           B
                              0



                    +5
         1(b)4
           B                  0



                    +5
         1(b)5
         AB                   0



                 +5
         1(b)6
          AB 0




         1(b)7
               +5
          ^B a

                                  Fig. 13-5. Waveforms for part 1(b).


     View and sketch on the curve sheet of Fig. 13-5 the following waveforms:

    1.    Output A waveform
    2.    Output A waveform
    3.    Output B waveform
    4.    Output B waveform

     For the following waveforms, pins 4 and 5 of the NAND gate (type 7420) can be left uncon-
nected.




                                                 `62

===== PAGE 178 =====
      After the decoded waveform has been viewed and sketched, the decoding is to be checked to
see if all the inputs are necessary. To do this, remove (one at a time) each of the inputs to the
decoding gates and view the pattern. If the decoded pattern changes, the input was necessary and
it should be reconnected. These results are to be tabulated in Table 13-lE.

   5. NAND gate output (pin 6 type 7420)for input Ato pin 1 (type 7420)and 豆 to pin 2 (type 7420) of the
NAND gate.
   6. NAND gate output (pin 6 type 7420) for input A to pin I (type 7420) andii to pin 2 (type 7420) of the
NAND gate.
   7. NAND gate output (pin 6 type 7420) for input A to pin 1 (type 7420) and B to pin 2 (type 7420) of the
NAND gate.

                                      Table 13-IE. Mod-3 counter decoding.
                                                  cbunt State               Necessary
                               O'unt           Basic NA7vZ)／꺄puts            ／꺄'uts
                                  0                       AB
                                  1                       AB
                                  2                       AB


    C.   Bcz) cbunter1`＇洌＇Decimalz沕coder-Single Pulse


                                                                                            To CR0 EXT
                                                                                        -－→TRIG (NEG)
                                            +5 V



                                           寸                                                 ：긍召16
                                                           L-
                                                                      --




                                                          r
                                                                2-.  13                      2 ⑨ ①15
          SWG                                                     R0
                                                                3-i A12                      3A（助4
          +5 V
                                                                4    Dli                   40 ④13


                                            l
         10 kHz
           or                                       Vcc                             Vcc
                                                                5                          5
                                                                                         -

                                                                       10                        12
          50ps                                     = +5 V                           = +5 V
                                                                                           6B 但：)11
                                                                                                       -J-
         SINGLE                                                       B9
         PULSE                                       －工
                                                                      c8                     7C ⑦ 10
                                                                                             8② J9
                                                                    Type
                                        +5 V                        7490                      Type
                                                                                              7441A


                      To
                 Type 7441A
                Decimal outputs




                               Fig. 13-6. Decade counter and decimal decoder.


    The type 7490 is an NBCD decade counter. The NBCD outputs are D, C, B, and A. The type
744lA is an NBCD to decimal decoder. The NBCD inputs are D, C, B, and A, and the decimal
outputs are encircled. The 7441A outputs have an open collector.


                                                          163

===== PAGE 179 =====
                         Set the SWG .to single pulse. Connect the 5.6-ku resistor and CRO input to output 5 (pin 14)
                   of the 7441A decoder. Reset the 7490 counter to zero by connecting both of its pins 2 and 3 to
                   +5 V momentarily and then returning pins 2 and 3 to ground. Measure the voltage at pin 14 of the
                   7441A and apply single pulses from the pulse generator. The voltage at output 5 should change at
                   the fifth pulse. Now apply pulses 6, 7, 8, and 9. The outputs for pulses 6, 7, 8, and 9 should be the
                   same as for pulses 0 through 4. If this does not occur, call the instructor.
                         Repeat in the same manner for output 7 (pin 10). Connect the 5.6-k2 pull-up resistor to pin
                   10 of the 7441A.
                        Change the output of the SWG to 10 kHz. Connect the 5.6-ku pull-up resistor and CRO to
                   each of the decimal outputs of the 7441 A decoder. View each of the outputs and sketch the out-
                   put on the curve sheet of Fig. 13-7 for decimal 0, decimal 5, and decimal 7.

                                 +5
                            0ock
                                           0


                                +5
                          Decimal
                             0 0



                                      +5
                          Decimal
                             5    0



                                      +5
                          Decimal
                            7    0

                                                                     Fig. 13-7. Waveforms for part 1(c).

              /-
닛띄Encoding-                      Decimal            to Excess 3 (Fig. 13-8) .




                   For all ICs in this part: Vcc = +5 V to pin 14, 0 (ground) to pin 7.
                        Measure the voltages at outputs D, C, B, and A to complete Table I 3-2E.

                                                                                Table 13-2E.
                                                                       Switch αr
                                                                                                                        .


                          Decimal                   0            1     2        了          4          5    z)   C   B       d4



                             0                 +5
                                                                 0     0        0          0          0
                             I                      0       +5
                                                                       0        0          0          0
                             2                      0            0    +5        0          0          0
                             3                      0            0     0        +5         0          0
                             4                      0            0     0        0       +5            0
                             5                      0            0     0        0          0     +5
                                                                                     i64

===== PAGE 180 =====
                                                 DECIMAL
                       +5 V




                                                                                            \




                          >＞鉀
                                                                       ^
                                                                       Z
                                                                           742
                                                                       b




                                                                                                > EXCESS3


                                                                           7420


                  11




                                                                           7420
                  13



                   Fig. 13-8. Decimal-to-excess 3 encoder(DCBA)for decimal digits 0 to 5.

3.   BCD Counter with Seven-Segment LED Display (Fig. 13-9)


To drive a seven-segment display it is necessary to first decode the NBCD inputs to decimal and
then encode the decimal values to the seven-segment code. Ths is accomplished in the 7447. The
7447 has open-collector outputs capable of sinking the segment currents needed to light the seg-
ments of a common anode seven-segment LED display.
     Set.LT(7447)to +5 V.
     Set the pulse generator to single pulse. Reset the counter to 0 with the R。control.
     Check the segment display by 」connecting LT to ground. All seven segments should be lit.
Then reconnect LT to +5 V.
     The segments of the seven-segment display are indicated on the diagram using the letters a to g.
These are circled on the 7447 driver.
     Pulse the SWG manually at about a one pulse per setond rate and note the display progression.

                                                    l65

===== PAGE 181 =====
                                                                                                      l
                                                                            ,680.
                                                                            resist。                   rs


                                                                                                vcc
                                                                                                                                     vcc
                                                                                                                 -          -
                        ,1    一                                    一
        p미se
                        nz
                                    14                        lB           16                                        1   (Dv 14
      generator
- 軌
                               o
                        n    ㄱRㅢ
                                    13                        2C       @15                                           2 (Z) (E) 13
                        U
                        <                                                                                  vcc
                                   A 12                       3 LT G:) 14                                            3          12
       騙n이e             4          D




                                                                        ⑥＠@ ④
       pulse                        11                        4        (E) 13                                        4      色：) 11
                                   c 9 8



                                                                                      2 1 0 9
                  vcc   n
                        J
       50 u』s                                                 5                                                      5      @10
       1- 5 V           ^
                        b          1
                                                              6D                                                     6           9
                        7            B c
                                                              7A                                                     7 (D 이：) 8
                                                              8
                             7490                                                                                        MAN 71A
                                                                                                                         MAN 72A
                                                                   7447
                                                                                                            7-segment LED display
                                           Vcc = -4-5 volts                                                     (or equivalent)

                                       Fig. 13-9. Decade counter with seven-segment[ED display.

===== PAGE 182 =====
REQUIRED RESULTS


Based on the results of Table 13-2E, complete Table 13-2R using Is and Os for the outputs D, C, B,
and A for logic values 1 > 2.5 V,0 <0.5 V.

                                     Table I3-2R. Decimal to excess 3.

                              Decimal          D          c       끄       J4
                                 0
                                 l
                                 2
                                 3
                                 4
                                 5



DISCUSSION


1.   A three-stage binary counter is shown in block diagram in Fig. 13-10. Draw a logic diagram
     (decoding gates with required inputs) showing how to decode it at a count of 5 and for a
     count of 6 (separate gates). The decoded outputs are to be at logic 1.



               Clock                   A                      T   B             C



                                     Fig. 13-10. 3-stage Mnary counter.




2.   The counter of Fig. 13-10 is to be decoded to generate an output of a 1 when the count is at
     counts of 4 or 5 or both. Show how to do this in the simplest way by drawing a logic diagram.




3.   Write the excess-3 code for the decimal numbers 0 through 5 and compare with the results of
     Table 13-2R. Do they agree?




                                                    l67

===== PAGE 183 =====
4.   Compare Table 13-2R with Fig. 13-8 and explain how the circuit of Fig. 13-8 generates the
     excess-3 code.




5.   A two-stage binary counter counts up in normal binary. It is desired to encode it according
     to the following code. Draw a logic diagram showing how to do this.


                                         Normal         Encoied
                                       ci7unt Stare      Output
                                           00             l0
                                           01             ll
                                           10             01
                                           11             00




6.   An "active high" output of a decoder is defined as a decoded output at a high (positive) voltage
     and an "active low" output is defined as the decoded output at a low positive voltage. Corn-
     plete the following statements with low or high based upon your experimental data.

          Part 1(a) active

               1(b) active

               1(c) active




                                                  l68

===== PAGE 184 =====
                                                                     ExperimenE]'l


Rondom-Access Memories;(IAM)
Scrolxh Pod Memories



OBJECT

     I.   To study the basic principles of semiconductor memories.
    2.    To study the operation of an MSI(TTL)64-bit memory cell.



INTRODUCTORY THEORY

Semiconductor random-access memories(RAMs) use R-S flip-flops as the building block. By'using
multigated inputs to control the operation of the FF, a FF in the memory can be randomly selected
with information written into and read out of the memory under external control.     .
     The memories used in this experiment enter data into each cell with positive logic, but the
information readout appears with negative logic. This is compatible with the entering of parallel
data into shift registers.


EQt기PMENT REQUIRED

    dc power supply, +5 Vat 100 MA
    CRO, dc coupled and calibrated
    Switch bank, 10 switches
    Two IC type 7400 quad 2-input NAND gate
    IC type 7403 quad 2-input NAND gate, open collector
    IC type 7489 64-bit random-access memory (with open-collector outputs)
    Four 680-`l, 土10% conipcsition resistors
    Four 5.6-k2, 土 10% composition resistors
    Four red LEDs

                                                     l69

===== PAGE 185 =====
                                                               IC manufacturers' part numbers.

                                                                                             了exas                National
                                      Type        2%fotorola           /:hirchild         Instruments           Semiconductor

                                      7400        MC7400P              7400PC              SN7400N                  DM7400N
                                                  MC7400L              7400DC              SN7400J

                                       7403       MC7403P              7403PC              SN7403N                  L)M7403N
                                                  MC7403L              7403DC              SN7403J
                                       7489       MC7489P              7489PC              SN7489N                  DM7489N
                                                  MC7489L              7489DC              SN74891



                    EXPERIMENTAL PROCEDURE


                    1.     2-Bit Random-Access Memory (Fig. 14-1)


                                                                                                                                      45V(Vcc)


                                                               CeI A                         극                                    56k요          56kr.2




                                                                                                                                                           SENSE


      H U 니 J ㄴm
H
ㅡ 一


?
/
       山H
                                                                                                      《－
                                                                                                     RA
                                                                                                               《，
                                                                                                               RB
                                                                                                                       l
                                                                                                                       ㅣ

      ㄸ 크                                                                                        工：니毓：而0               :
                                                                                                 =
                                                                                                           SELECT-   =j
                                                                                                           ㅣ                           1SENSE
                                                                                                                                                   1
                                                                                                                           7403
                   ?,                                                                                                                                  `




                                                                                                                    vcc = +5 Volts to pin 14
                                                                                                                          0 Iground) to pin 7
                                                                                                                          AIi ICc




                                                          Fig. 14-1. 2-1巾 random-access memory -


                        All switches must be at GROUND initially. To operate the memory, inform1ation must first be
                        written into a cell for storage. Information can then be read from the cell.




                                                                                    170

===== PAGE 186 =====
     To write data into a cell, two things must be done:

        Select where the information is going, cell A or cell B, by connecting the appropriate select switch
(WRITE SELECT A, WA,or WRITE SELECT B, WB)to +5 V.
      b. Write the level of information (0 or I) into the cell by connecting the appropriate W。or W1 switch to
+5 volts. One, but only one, of the WRITE switches must be connected to +5 V.

          Caution: only one bit (A or B) and only one level (I or 0) can be written at a time.

       . After information is written into a memory cell, return all WRITE SELECT and WRITE LEVEL switches
to ground.
      d. A stored 1 makes the "SENSE 1" output less than +0.5 V and the "SENSE 0" output greater than +2.5 V.
A stored 0 makes the "SENSE I " output greater than +2.5 V and the "SENSE 0" output less than 0.5 V.
          To read the stored information, connect the desired READ SELECT (RA or RB) switch (only one at a
time) to +5 V. After this is done, read the voltage levels at the SENSE 0 and SENSE 1 outputs. After the stored
information has been read, return the READ SELECT switch to ground.

     This data are to be taken one line at a time. Store the following information, check the FF
output, and sense the stored data by measuring the voltages at the following points to complete
Table 14-IE.

                                               Table 14-lE. 2-bit memory.

                      WRI7E                                                         READ
                                           A      B                    계                             B
              Bit 4          及rβ                            SEV5E /         SfNSIr ()     SE7VSf /       SE깊VSE〃

      I         0             0            0       0

      2         0             l            0       I

      3         1             0            l       0
      4         l             l            I       1


2.   64-Bit IC RAM-Type 7489 (Fig. 14-2)


The 7489 is a 64-bit RAM organized as a 16-word by 4-bit array. To reduce the number of input
addressing pins required to address 16 words, the words are addressed through four binary address-
ing inputs (DCBA) which are decoded within the IC. The outputs are open collector to allow for
memory expansion. The 7489 is enabled by means of two inputs, the memory enable (ME) and
write enable (WE), as shown in the following function table.



                      ME            lYE
                      Pin2         Pin 3          0peration                C'ondirion of Ot쨔)Ut$

                       L            L          Write                  Complement of data inputs

                       L            H          Read                   Complement of selected word

                       H            L          Inhibit storage    Complement of data inputs

                       H            H          Do nothing             테gh




                                                          l 7l

===== PAGE 187 =====
                                                Data inputs
                                       O-        o.----O----o---------- vcc




                                       c-
                                                 o-         o        c         '-
                                                                                         －ㄱ－
                               4            6         10       12




             긋긋긋긋
                                   D                                                                     Vcc
                                            D2         D3       D4
                                                                 ME O_

                          15
                               A

                                                                          O3
                                                                                                     V         MEMORY ENABLE
                                                                    WE
                                                                                                     V
                               B
                                                7489                                                           WRITE ENABLE
                          14                                              16
                                                                                     O
Address
                               C                                    Vcc             +5 V
 Inputs
                          13
                               D                                GND
                                                       S        S4
                                                                                                         Vcc =+5 volts to pin 16
                                       5        7          9                                              0 (ground) to pin 8

       Vcc
                                                                                               Vcc

                                                                            680 &2
                                                                           resistors




                           Sense
                                                                                               LEDs
                          outputs




                               Fig. 14-2. 64-bit random-access memory.


To operate the memory, the following procedure should be followed.

a.   ME and WE at +5 V.
b.* To write data into a memory location:
    1. Select memory location DCBA.
    2. Apply data to data inputs D4 to D1.
    3. SetMEandWEat0.
    4. SeLME and WE to +5 V.
c.   To read complement of data stored in a memory location:
     1. Select memory location DCBA.
     2. SetMEat0andWEat+5V.
     3. Read data at outputs S4 to S1.
     4. Set ME and WE to +5 V at the completion of a series of readings.


*Steps b3 and b4 must be performed for each write step.




                                                               l72

===== PAGE 188 =====
         d.    To obtain the complement of the initial random input data(no previous data storage):
               1. Select memory location DCBA.
               2. Apply random data to data inputs D4 to D1.
               3. SetMEat+5VandWEat0.
               4. Read complement of input data at outputs S4 to S1.
               5. SetMEandWEto+5V.

     In the following experimental procedure, assume positive logic for which logic 1 > +2.5 V
and logic 0 < +0.5 V. Record measured data as 1 or 0.


    e.        Operation and Testsfor DRO/NDRO and Volatility

         1.     ME and WE at +5 V before Vcc is connected to pin 16.
         2.     Select memory location DCBA = 1011.
         3.     Read the complement of the initial stored data. (ME = 0 V, WE = +5 V.).

                                                                                 S4S3S2S1 =

      4.        MEandWEat+5V.
     *5.        Write data D4D3D2D1 = 0110. (Set ME =0 V,WE = 0 V.)
      6.        MEandWEto+5V.
         7.     Read the complement of the stored data. (ME =0 V,WE = +5 V.)

                                                                                 S483828l =

         8.     MEandWEto+5V.
         9.     Read the complement of the stored data again.(Test for DRo/NDRO.)(as in step 7)

                                                                                 S483828l =

     10.        MEandWEto+5V.
     11. Disconnect the +5 V from the Vcc input, pin 16. Reconnect the +5 V (Vcc)to pin 16 and read the
complement of the data now stored (test for volatility).(ME = 0 V,WE = +5 V.)

                                                                                 S4S3S2S,'

     12.        MEandWEto+5V.*


    f.        7489Binary- 力ay Code Converter

     In Table 14-2E in the memory locations given in column A, store the data of column B. Only
change memory locations DCBA when ME and WE are at +5 V (H). This will prevent improper data
entry into memory and destruction of previously stored data. Then read the complements of the
stored data and enter the results in column C. (Note: The input data stored are the complement of
the Gray code for the binary numbers corresponding to the memory locations. The final result
stored yields a binary input-to-Gray code output converter.)


     4To the instructor (student). If in step 3, 54S35251 = 1001, change data to D4D3D3D1 = 0111.




                                                          l73

===== PAGE 189 =====
                                         Table 14-2E. 64-bit RAM.
                           A                       B                      C   '




                         dddress
                                                pαrα                 Stored z）αrα
                               及nti':y      to Be Stored            rCornplernenU
                               ／兀BA         D41乃D21기                  씨S352이
                     0          0000             l 11 I
                     1          0001             1110
                     2          0010             1 100
                     3          0011             1l 01
                     4          0100             1001
                     5          이01              1000
                     6          0110             1010
                     7          0111             1011
                     8          1000             0011

                     9          1001             0010
                    l0          1010             0000

                    l】          1011             0001
                    I2          1100             0101
                    l3          1101             0100
                    14          l 110            0110
                    l5          1111             011 1



REQUIRED RESULTS


Use positive logic 1 > +2.5 V and 0< +0.5 V and the sense output logic definition as defined by id.
     Complete Table 14-lR for the data of Table 14-IE. This table should have ls and Os.

                                             Table 14-IR. 2-bit memory.
                                                 S끄？Rf/)              SENSE/)
                                           Bit A          BitB   BitA             Bit β
                                     l       0               0
                                     2       0               l
                                     3       l               0
                                    4        l               1




                                                       l74

===== PAGE 190 =====
DISCUSSION

1.   Based upon the experimental data of part 2e(9), is the 64-bit RAM a DRO or a NDRO memory?




2.   Based upon the experimental data of part 2e(l I),is the 64-bit RAM volatile or nonvolatile?




3.   Why are the outputs of the 7489 presented in complementary form? (Hint.' What are the
     logic-level requirements for the present PR inputs of FFs,such as the 7472 and 7476?)




4.   Why are the outputs of the 7489 open collector?




5.   Are ferrite-core RAMs basically DRO or NDRO?




6.   Are ferrite-core RAMs volatile or nonvolatile?




                                                l75

===== PAGE 191 =====

===== PAGE 192 =====
                                                                                        /




                                                                        Experiment]5



The Operational Amplifier
                                              ．갸獅죤鈿




                                                                       上∼ 6 깃了＼ I '
                                                                                            v Ce.

OBJECT
                                                                 ％叔-    i
     1.   To study the operational amplifier as a precision analog voltage amplifier.
    2.    To study the operational amplifier as a multiplying and summing amplifier.
     3.   To study the operational amplifier as a comparator.
     4.   To study the operational amplifier as an integrator.


INTRODUCTORY THEORY


The operational amplifier, frequently called op-amp, is a high-voltage-gain high-input-impedance
dc-wideband inverting amplifier whose output voltage is 0 when the input voltage is 0 V. The
graphic logic symbol for an op-amp is shown in Fig. I 5-I.


                                               -{:〉ㄴ
                                    Fig. I 5-I. Operational amplifier (op-amp).


      An op-amp is powered with two power supplies (not shown), a positive and a negative voltage
supply. 15 V is fairly common for the voltages with transistor& and ICs. This enables the ampli-
tier to provide signal output voltages up to approximately 80% of the supply voltage and an ampli-
fier with 土 15-V supplies can provide output signal voltages of the order of 12 V before the out-
put 1iir=ts.

                                                        177

===== PAGE 193 =====
      Frequently, an op-amp has two inputs, an inverting and a noninverting input. The logic sym-
bol for this type of amplifier is shown in Fig. 1 5-2. In this amplifier the inputs ar6 connected in a
differential mode and the out秒ut voltage is the amplifier gain multiplied by the voltage difference
between the two input signals.



                                             牙＞                -
                                    Fig. 巧-2. Differ 'ntial input op-amp

      Historically, the op-amp was first developed for app!kiIi. ns in which feedback between out-
put and input was used. When this is done, the gain ot the amplifier can be made to depend only
on the values of the feedback components. With feedback, the amplifier is capable of"performing
the mathematical operations of addition, multiplication, division, differentiation, and integration
upon applied signal waveforms and in this form was the b..sic element of the analog computer. Log-
ically, only the amplifier with feedback should be called an up-amp, but so many other applications
have been developed for the amplifier that it is now comnmon practice to call the amplifier alone
an op-amp.
      Consider an op-amp with feedback as shown in Fig. l5- ? As will be shown shortly, point A,
the input to the amplifier, is at a voltage almost equal to 0, and p`,irit A is at a virtual ground.

                                                          5 k요


                             d V        1 k2
                                                                           V。
                                                                            ut
                              yin
                                       4너 mA                               +5 V

                                     Hg. 15-3. Op-amp with feedback.


     Apply a voltage V, = - 1 V. If point A is at ground, 1 mA must flow fro1u41oVi, through
the l-k요 resistor. However, point A has very high impedance and no current can come from the
amplifier. The only place current can come from (to maintain current continuity) is from the
5-ku resistor. But, since A is at ground, the output voltage must be +5 V (1 mA X 5 k2).
     We can therefore write, neglecting the change in polarity or phase between input and output,

                                            Y으쁘＝! 5쁘＝5
                                             V, 1 ' }(Jz

Hence, the gain is determined only by the resistor ratio.
    In a piactical amplifier the voltage gain might be 50,000 and the input resistance 500,000 fl.
With 5 V output the voltage at point A must be


                                            505沁o- 1 X io-' V
                                            5。    .。。。
This is close enough to 0 compared to the 1-V signal and the 5-V output to justify the assumption
that the voltage at A = 0. The input resistance of 500 k2 is large enough compared to I kn and
5 k2 to justify neglecting its effect (to a first degree of approximation).
     Consider Fig. 15-4, which has two inputs. By extension of the analysis applied to the circuit
of Fig. 15-3, a current of 1 mA must flow into ViflA and a current of 0.5 mA into VmB ·
      \／的t = 7.5 V = S(VinA + VmB). Point C acts as a summing point. The circuit of Fig. 15-4
can be used to add two analog signal voltages.

                                                         178

===== PAGE 194 =====
                                                         1 k2                                         5 k2
                          n^ =_1v                        MA._                                    - -－싸V`---
                           n                             imA                                         1.5 mA
                                                                                                                                                V。 ut
                                                                                                                                                +7.5 V
                     ,'    - f 二 \i
                                     1 k요                                                                      >'
                     ' 1nB - U'U V－→／V, _
                                    0.5 mA
                                                    4－
                                                               ·－---




                           Fig. 15-4. Feedback amplifier with two inputs and equal summing resistors.

    In Fig. 15-5 equal voltages are applied to summing resistors, but the resistors are not equal.
The output voltage is equal to 7.5 V, obtained as follows:

                                             .:=
                                            v.
                                            V。
                                             ut =
                                                  5kf1v,**
                                                   j     +
                                                           5kf2
                                                          j_
                                                                Vm                               =   5   (l)        + 2.     5   (1)
                                                                       VmA
The analysis of Fig. 15-5 shows, therefore, that by choice of summing resistors it is possible to
change the scale factors by which signal voltages can be multiplied and summed.

                                                                                                     5 kfl
          VjflA=           _   1V                                                          -－∼                       -----




                                                                                                     1.5 mA

                                                                                                                                             +7.5 V to V。
                                                                                                                                                        ut
                                                   2 kZ
                   V1nB= 1 V                       A44v\.

                                                 0.5 mA

                          Fig. 15-5. Feedback am미ifier with two inputs and unequal summing resistors.

     Figure 15-6 shows an op-amp with capacitor feedback between the output and the input of
the amplifier. Let the input voltage suddenly change to a negative fixed voltage at time t. At this
time current must flow from point A to Vhl with a magnitude

                                                                             I=
                                                                                   ViiiR
As in the previous examples, this current must come from the capacitor C.




                                   R
                           yin -－→＾7`Vm- -                                                                                                    V。
                                                                                                                                               ut
                                           쎄1- i




                                                                                                                                         -卜Time
                                                                                                                                       yin

                                    +                                                                                                  V。
                                                                                                                                        ut
                                    V


                                        Fig. 15-6. Feedback amplifier with capacitor feedback.

                                                                                  】79

===== PAGE 195 =====
     But current flowing for a time t means that a charge Q = It must have flown from C. But this
could only come about by an increase in output voltage VO,t given by the expression Q = C VO,t.
Combining the expression for I, and the values of Q, we obtain


                                                                    cvO,
                                                Q=
                                                     논t         =




Hence,

                                                     v。
                                                      ut- j
                                                          Vh,       RC

Equation 15-1 tells us that the output voltage will increase linearly with time, forming a ramp, and
continue until the amplifier limits. Larger values of R and C result in lower output voltages and are
to be expected. Large values of R reduce the charging rate for C and large capacitors take longer to
charge.
     The circuit of Fig. 15-6 is an integrating circuit. The voltage at the output depends upon the
summation or integral of the charge flowing into Vi, .
     In a square wave of voltage, such as is shown in Fig. 15-7, is applied to the integrator of Fig.
15-6, the applied voltage will alternately add charge and subtract charge from the capacitor at a rate
based upon Eq. 15-1, resulting in a triangular wave output.




                   yin




                 v。
                  ut




                     Fig. 匕-7. Integrator with square-wave input ai업 triangular output.


      Figure 15-8 shows an amplifier with two inputs, an inverting and a noninverting with no feed-
back-an open-loop configuration. This amplifier has a differential input and amplifies the differ-
ence in voltage between the two inputs with high gain. If the minus input is slightly negative with
respect to the plus input, the output voltage is positive (and probably limiting); and if the minus
input is slightly positive with respect to the plus input, the output voltage is negative (and probably
limiting). The configuration of Fig. 15-8 can therefore be used as an analog voltage comparator.




                         Fig. 15-8. Amplifier with two inputs, inverting and noninverting.




                                                            180

===== PAGE 196 =====
     If the amplifier limits at 10 V and has an open-loop gain of 50,000, a voltage difference in
excess of 10/50,000 = 0.2 mV is enough to drive the amplifier into its limiting region. As an analog
comparator the amplifier is quite sensitive.
     An op-amp does not always provide zero output voltage with zero input. Many amplifiers
therefore have provisions for a zero output adjustment.


EQUIPMENT REQUIRED


      Two ICs type 741 op-amp                                    Capacitor, 0.22 1jF
      Resistor, 1000 f2 1%,film 1/4W                             Zenerdiode,4.7V10%,0.5 orlW
      Resistor, 2000`2 n%, film % W                              CRO, dc coupled and calibrated
      Resistor,490 n 土1%,fi1m 14W                                dc power supply, +15 V,regulated at 50 mA
      2 resistors, 470 fi, 소10% composition                      dc power supply, -15 V, regulated at 50 mA
      Resistor, 10,000 f, 土10% composition                       dc power supply, 0 to 15 V. regulated at 50 mA; adjustable
      Resistor, 100,000 2, 士10% composition                      SWG, 200 Hz; max. output impedance 500 n at 4 V p-p
      Potentiometer, 500 f2, 3 turns, 5 W                        Sine-wave osci끄ator, 20아z, 30 V p-p
      Capacitor, 0.1' zF


                                              IC manufacturers' part numbers.

                                                                                                       Texas
              Type          Fairchild         Motoroh            Signerics        National         Instivments

              741C           74n)c          MCI741CL             N5741A         LM741CD            SN72741N
                                                                                LM741CN-14         SN72741J



EXPERIMENTAL PROCEDURE


1.
     a.   Op-Amp as an Analog Voltage Multiplier

    Using the CRO, make voltage measurements at the points indicated in Fig. 15-9, to complete
Table 15-1E. As each data point is obtained, plot it on the graph of Fig. 15-10. VA-horizontal;
Vx-vertical.


                                                                        +15 V
                                                           4.99 kl                            O        +15 V
                                                                                                       mac 一
                                                                                                    power supply
        dc      -O    』                 洲         1   小A
                                                           f.    t
                                                                       11
      power                             1kn       C
      sup이V    -o
                       그－
                                                           ff          6                              -isv
                                                                                                       dc
                                                                -15V                               power supply


                                               Fig. 15-9. Voltagemultiplier.




                                                                181

===== PAGE 197 =====
                                 Vx                                                                           Table islE.
                        】    + 20 V이ts         I                                                                               I노
                                                                                                 VA                Vc
                                                                                                (?R(7             CRt7        CR7
                                                                                               / V/div          0./ V/div    5 V/div
                                                                                                      0
                             +10
                                                                                                 +1

                                                                                                 +2
                                                                                                 +4
-20 ------- 10               0--          ' '- + 0- -          -   +20 Volts VA                  +8
                                                                                                +12
                                                                                                      1

            끼                -     10                                                             -   2
                                                                                                      ‘후
                                                                                                      8
                                                                                                 12
                                   20

                                       Fig. 巧-10. Voltage multiplier-CRO X-Y display.


      b.   야》
            －4mp asα＇' Analog Voltage Multiplier (:R(7尤γ Display

       Connect the output of a sine-wave oscillator whose signal is 30 V p-p at 200 Hz to the CR0
  horizontal input and to the l-k2 resistor input of the voltage multiplier as shown in Fig. 15-11.
  Center the horizontal display and adjust the horizontal gain so that the pattern displayed occupies
  6 horizontal divisions 三 5 V/div. View the pattern, It should agree exactly with the plot of Fig.
  15-10. If it does not, call the instructor.


                             To CRO horizontal
                                   ^                                                                            +15 V
                                                       --7一－             -－寸－   ---                               dc
            200 Hz                 A                           4.99k12                    -0
                                                                                                              power sup이y
           Sine wave    0-
           oscillator
            30 V p-p    0-
                                                                                      1
                                                                                                           X To CRC vertical 5 V/div




                                                                                                 u              1 5 `/
                                                                                                                  dc
                                                                                                 0            power supply


                                                        Fig. 巧-11.




                                                                I82

===== PAGE 198 =====
2.   Op-Amp as a Summer-Multiplier


In the circuit of Fig. 15-12 measure the voltage at point X with the CRO to complete Table 15-2E.
Use CRO sensitivities to give greatest accuracy of readings, but do not use a sensitivity below
0.1 V/div.
                                                                                                                      4.99 k




                                                                                                l
                                                                                                                       一－      -



                                                                         1 k2
                                                            -                   ----
                                                                                                              +15 V


                                                                                                          >           10
                                                                         2 k요
                                                      －∼－                              ---




                                                                                                 볍＝           -15 V




                                       Fig. 15-12. Summer-multiplier.



                                                   Table 15-2E.

                                            E4                  y8             vx
                                             0                   0
                                             0                  +1

                                            +l                       0
                                            +1                  +1


                                                                                             +15 V
3.   Op-Amp as a Voltage Comparator (Fig. 15-13)




                                70 &


                  500 o.
                  3 turn                                                                             10


                           吉；   :m

                                               dc               -o
                                             power
                                             sup이y              -o
                                                                           I



                                                                                             -15V

                                          Fig. 15.13. Comparator.

                                                            183

===== PAGE 199 =====
Use the CRO to make all measurements. For each value of VB in Table I 5-3E, vary the setting of
the potentiometer to determine the voltage at A which makes the output voltage V, change rapidly.
Measure VA to within 0.1 V and complete Table I 5-3E.

                                              Table 15-3E.

                                               VB          VA
                                               0
                                              40.5
                                              +1.0
                                              +l.5
                                              -0.5
                                              -1.0



4.   Integrator (Fig. 15-14)

                                                                                               0.22 tF

                                                                                      －니   （-              -




                               CRO EXT
                               TRIG NEG                                               1－   →         ---




                                  *                                                            100 k요
                                      10kn                             +15 V
         SWG
        4 V p-p
        200 Hz
                                                                스＼           二；
                                                                              ,.                                    X

                                                           I
                                                                5,   -,c                                       To CRO
                                                                                                               vertical
                                                                           -15V

                                         Fig. 巧.14. Integrator.

Set the SWG frequency or the CRO horizontal sweep rate for the SWG pattern shown in Fig. 15-15.
     View the voltage V, on the CRO and sketch it on the graph of Fig. 15-15. The graph should
show the voltage amplitudes for V, and the time scale.

                   +2
           SWG
               -        2



              VX
                                                                                  1




                                     Fig. 15.15. Integrator waveform.




                                                     l84

===== PAGE 200 =====
5.   Variable-Pulse-Width Generator (Fig. 15-16)


                           +15V -                       0.1
                  TO CR0
                EXT TRIG NEG
                    A                                                        470l
                                                     100 kl
                                                   -wy-     --                                     TO CR0
      SWG                                                                                          VERTICAL
                                               1
     4 V P-P                                                                                  10
     200 Hz                                                                                               X
                                                                   500 fl

                                                                                                       D 4
                                                                   3 TURNS
                                                                                                         1
                                                                                                         1 `
                                                                                                           /   v
                                                                                  0n

                                                                  '_
                                                                  -15 V

                                   Fig. 15-16. Variable-pulse-width generator.


     (a) Zener diode D1 NOT connected to pin 10 of op-amp 2.

                 1. Adjust the potentiometer to make vx a square wave. Measure vA and tabulate on line 3 of
           Table 15-4E.
                2.    Repeat I but for the most positive portion to be 25% of a cycle. Enter on line 2 of Table
           15-4E.
                3.    Repeat 1 but determine VA for the positive portion to just disappear.
                4.    Repeat 1 but for the most positive portion to be 75% of a cycle.
                 5.   Repeat 1 but for the positive portion t(巧ust occupy the complete cycle.

                                                        Table 15-4E.

                                                         ／】bSitive
                                                      Percent ofCycle        VA
                                              I               0
                                              2              25
                                              3              50 (SW)

                                              4              75

                                              5          100


     (b)   Sketch the waveform at V, for the 50% cycle (SW) on Fig. 15-17. Show voltages and
           the time scale.
     (c)   Connect the 4.7-V zener diode between point X and ground as shown in Fig. 15-16.
           Vary the potentiometer and note the effect. Sketch the waveforms at V, for the 50%
           cycle on Fig. 15-17. Show voltages.




                                                      i85,

===== PAGE 201 =====
                                                                                           I Iㄱ
                  +2
            SWG
                       -   2


                                     T
              vx
           Part 5(b)




             vx
       Part 5(c)


                               Fig. 15-17. Waveforms for variable-pulse-width generator.



DISCUSSION


1.   In part 1, what was the measured voltage gain Vx /VA for

     (a)     VA = +1 V?                                  (b)    VA = +2 V?

     (c)     VA = -l V?                                  (d)    VA =-2V?

     How does this compare with the theoretical voltage gain, and what determines the theoretical
     voltage gain and its precision?




2.   What were the positive and negative output limiting voltages in part 1? What percentage were
     these values of the respective power supply voltages?




3.   If the open-loop voltage gain of the MA741 is 100,000, what voltage would you expect at
     point C if Vx = - 10 V? Compare this with your measured voltage.




                                                         186

===== PAGE 202 =====
4.   The statement has been made that in a closed-loop operational amplifier, the input to the
     amplifier is a virtual ground when the output is not being limited. Did your data show this?
     Discuss.




5.   Compute the voltage at X.

                                                                            5000 S2
                        1 kn
                                                                    --－一－             --




               +0.1 V-－小
                        2 k2
               +0.4 V-

               -0.2 V.
                           －→∼－




                                      4 k2
                                               -1   _
                                                                            >
                                                    Fig. 巧－l8.



6.   Based on the results of part 3, what general statement can be made about the value of the input
     voltage at A compared to that at B at which the amplifier changes voltage rapidly?




7.   The switch is changed to make the voltage at A equal to +2 V. After 2.0 ms, what voltage
     should be expected at Vx? Show all calculations. Compare with the experimental change in
     integrator voltage of part 4 over a time of 2.0 ms.


                         +2 V                                  怜－
                                                             0.22 1jF
                      kㅗ          ．      lOkc2

                           b ＇떽              Wv_


                           오
                                                        二＞
                                                    Fig. 巧·l9.



8.   Explain the operation of the circuit of Fig. 15-16 with the zener diode in the circuit.




                                                        187

===== PAGE 203 =====

===== PAGE 204 =====
                                                                    ExperimenI 16



Di9iIoI-to-AnoIo9(D/A)ond
Anolog-to-Di9iEoI(A/D)
Conversion


OBJECT


     1.   To study the binary weighted ladder method of D/A conversion.
     2.   To study the comparison method of AID conversion.


INTRODUCTORY THEORY


Virtually all physical phenomena, voltage, pressure, temperature, velocity, and so on, occur in
nature on an analog basis. However, there are distinct advantages to digital representation, such as
information storage and data transmission. The requirement exists, therefore, to convert data from
an analog basis to a digital representation, AID conversion, and conversely, from digital to analog,
D/A.
     In the binary weighted ladder D/A conversion technique, a resistor network is used with values
increasing by multiples of 2. These resistors are connected between the summing junction of an
op-amp and the outputs of the counter stages. This provides currents into the summing junction
proportional to the binary weight of the counter stages. The feedback'4resistor of the op-amp can
now be selected to provide a scale factor. This will now make the op-amp output an analog output
voltage equal to the binary weighted sum of the count states of the counter multiplied by the
selected scale factor.
     The analog output voltage of the D/A converter cannot change continuously, but changes by
fixed amounts. The smallest possible change occurs when the 20: bit changes. The 20 is the least
significant bit (LSB). Each higher-order bit changes the analog output voltage by an a,lditional
multiple of 2 until the highest-order bit, called the most significant bit(MSB), changes. For exam-
pie, consider a three-stage binary counter whose maximum count state is 1 X 22 + 1 X 21 + I X

                                                    i89

===== PAGE 205 =====
2. = 7. If the scale factor of the op-amp is such that the LSB corresponds to a change in 1 V, the
analog output will progress in LSB steps of I V. The MSB = I X 4 = 4 V and the analog voltage
changes in steps of 1 V up to a maximum output of 7 V. To obtain a finer resolution in output
voltage, the number of bits must be increased and the value of the LSB decreased.
     If the output of a D/A converter is connected to the input of an op-amp connected as a
comparator and an unknown analog voltage connected to the other input of the op-amp, the
output voltage of the op-amp will be at its limiting value, positive or negative depending on the
polarity of the voltage difference between the D/A output and the unknown analog voltage. By
determining the counter count state at which the comparator output changes, the count state
equivalent to the analog voltage within one bit, the least significant bit (LSB), can be determined.
This comparison method, therefore, can be used as an A/D conversion.


EQUIPMENT RE이기RED


    CRO, dc coupled and calibrated                         Resistor, 2370 f2 士1%, % W
    SWG, 】kHz or single pulse, +5 V                        Resistor, 4530 n 소1%, %W
    Power supply, +15 V dc, regulated at 50 mA             Resistor, 4750 2 土1%, % W
    Power supply, -15 V dc, regulated at 50 mA             Resistor, 10,500 f 土1%, % W
    Power supply, +5 V dc. regulated at 50 mA              Resistor, 22,600 fl 소1%, % W
    IC type 740사Lex inverter                               Two resistors, 1kfl, 士10% composition
    IC type 7405 hex inverter, open collector              Resistor, 68 k2, 土10% composition
    IC type 7490 decade counter                            Two potentiometers, 500 2, 3 turns
    Two ICs type 74lC op-amp                               Switch bam 《， 5 switches per ba出
                                                                                          （
    Five resistors, 1.5 k요 土1%, 흥4 W


                                      IC manufacturers' part numbers.
                                                       Texas                           National
           Type       Motoro仇         Fairchild     /nstrumen惚         Signetics     Semiconductor
          741C       MC1741CL         741DC          SN72741N           N5741A        LM741CD
                                                     SN72741J                         LM741CN-14
          7404       MC7404P          7404PC         SN7404N            N7404A        DM7404N
                     MC7404L          7404DC         SN7404J            N7404F

           7405      MC7405P          7405PC         SN7405N            N7405A        DM74O5N
                     MC7405L          7405DC         SN740SJ            N7405F
           7490      MC7490P          7490PC         SN7490N            N7490A        DM7490N
                     MC7490L          7490DC         SN7490J            N7490F



EXPERIMENTAL PROCEDURE


Power supply connections:

     Type 7404 Vcc = +5 V to pin 14, 0 (ground) to pin 7
     Type 7405 vcc = +5 V to pin 14,0 (ground) to pin 7
     Type 7490 Vcc = +5 V to pin 5,0 (ground) to pin 10
     Type 741C+15 Vto pin m - 15 V to pin 6


                                                    190

===== PAGE 206 =====
1.
     a.   D/A Conversion-Decadeβα가Fig. 16-1)

     The type 7490 decade counter will count when pins 2 and 3 are connected to ground and can
be reset to zero by connecting pins 2 and 3 to +5 V. Returning pins 2 and 3 to ground will allow
the type 7490 to count.



                             SWG
                             +5 V
                          at 1000 Hz
                              or                                                                                           +5 V
                                                                                                                             -
                          single pulse
                             500 ps
                                                                                                                             ,




                                                                                                                                             5
                                                                                                                                             3~-~
                                                                                                                   여노 山
                                                                                                                      1尸     여노 띠尸   여섧 山尸
                                                            몫두땄GNEG                                       三

                                                                 " > 6ㅗ三戶_
                                                                                                  ^
                                                                                                                                              ^
                                                                                                                                                    ^
                                                                                                                                                        n
                                                                                                                                                        k
                                                                                                      m
                                                                                                  /
                                                                                                                                              Z
                                                                                                                                                    b
                                                                                                      ㅡ




                          .I
                                          14
                          ^Z
                                그         13
                          qU    R-   ^17



                          4 二
                            길
                                     Dli
                                      10
           Vcc
          = +5 V          ^b
                                                                                                                                              10.5 kn
                                      B9                                                        7405
                                      C8



                     《          Type                                                                                                          4530 `2
                 -              7490
                 -   +5
                          V

                                          zero
                                                                                                                                              1500 n
                                       reset
                                                                                                                                               一－       -1




                          If                                     !R.            =
                                                                                    4750
                                                                 l         )   see below)



                                                           1                                     CRO
                                                                                                 vertical
                                                                                                 2 V/div
                                                          1 k요

                                                                                           15                 RF   Selected to make the change
                                                                                                cdV                in output corresponding to the
                                                                                                                   LSB=1.0 volt. It may be necessary
                                                                                                                   to adjust or trim R F to make the
                                500 `2
                                                                                                                   LSB exactly equal to 1.0 volt.
                                3- turn                                1- 0+ 15 V
                                 zero          卜
                                                                       =             -     dc
                                               :1k&2.



                                                        Fig. 16-I. D/A conversion-decade BCD.



                                                                                    l91

===== PAGE 207 =====
      Set the SWG to 1000 Hz and view the output of the type 741C OP-AMP on the CRO. The
output should be a nine-step negative-going staircase waveform, with each step having the same
height. If you do not obtain the staircase, vary the zero control.
      Adjust the horizontal sweep rate so that two staircase waveforms are seen.
      Adjust the 500-&2 zero setting control so that the top step of the staircase is at 0 volts.
      With the resistor values used, the most negative step should give a vertical deflection of -9.0 V.
      Change the SWG to single pulse. Reset the type 7490 decade counter to zero by connecting
pins 2 and 3 to +5 V and then to ground. Change the CRO TRIG to INT.
      Measure the output voltage of the D/A converter 74lC pin 10. applying a single pulse at a
time and complete Table 16-1 E.
      Return the SWG to 1000 Hz and the CRO TRIG to EXT NEG. Change the horizontal sweep
rate so that one staircase is displayed. Sketch the waveform in Fig. 16-2(a).


Table 16-1 E. D/A conversion.
  /ulse        Hut(volts)
    0
     l
     2
    3
    4
    5
    6
    7
    8
    9




                                     (a)                                                   (b)

                                                 Fig. 16-2. Decade staircase waveform.




    b.    Scale-Factor Change

     Change RF to 2730 7. If necessary, adjust or trim RF to make the LSB = 0.5 V.
     Sketch on Fig. 16-2(b) and label the pattern and that of part 1(a) with the values of RF
and the scale factors for the LSB.




                                                 l92

===== PAGE 208 =====
    c.   Effect of"Opens" in D/A Converter

     Change RE to 4750 2. [Use value from part l(a)if changed from 4750 `2.]
     Open the connection between the following pins and note the effect on the staircase pattern.
In each case sketch the pattern on Fig. 16-3.

    1.    Type 7404 pm 2 and type 7405 pm 1 = 2o. Sketch on Fig. 16.3(a).
    2.    Type 7404 pin 4 and type 7405 pin 3= 21. Sketch on Fig. 16.3(b).
    3.    Type 7404 pin 6 and type 7405 pinS=2L Sketch on Fig. 16.3(c).




                (a)
                                                   (b)                          (c)

                                 ng. 16-3. Decade staircase with open errors.




                                                    l93

===== PAGE 209 =====
     d. Effect ofResistor Precision Error

      Shunt the 10.5-ku resistor on the ladder with a 68-kZ 10% resistor. Sketch on Fig. 16-4.
Remove the 68-k2 resistor. The sketch should show the pattern with and without the 68-k2
resistor.




                         Fig. 16-4, D/A binary ladder-effect of resistor precision errors.


2.
     a.   AID conversion-comparison Method

      This uses the same circuit as part 1 for the D/A conversion with the additional comparator
circuitry of Fig. 16-5.
      Change the pulse generator to single pulse. Reset the counter to a count of 0. Set the poten-
tiometer connected to pin 5 (op-amp), Fig. 16-5, to the voltage given in line 1 of Table 16-2E.
(Use CRO to measure voltage.) Monitor the output voltage of the op-amp of Fig. 16-5. Apply
single pulses to the decade counter until the monitored op-amp output changes from one limiting
 polarity to the other. Measure the counter count state at the type 7405 output pins. (Note: Con-
necting a lead from the CRO to the type 7490 counter may introduce spurious noise pulses which
can be counted by the 7490 counter, which is very fast. This is the reason for the measurement
at the type 7405.)
      Repeat this procedure for each of the pin 5 voltages of Table 16-2E, being careful to reset the
type 7490 counter to a count of zero in each case.



                                                       汐4

===== PAGE 210 =====
                    From type 741C pin 10 (Fig 16-1)

                                                                                   To CR0 vertical




                                                                                   Same
                                                                                   power supplies
                                                                                   as in Fig. 16-1.
                                Fig. 16-5. AID conversion-comparison method.


                                        Table I6-2E. A/D conversion.
                                                            yoltage Measurements αr
                                                  Type 740끄'ins after OP-AMP Output Change
                                                        (use CRO sensitivity of1 V/div)
                             Pin 5
                                                             Type 7405 Pin Voltages
                            Voltage
                          rFig. 16-5)          Pin 8          Pin 6         ^n 4           Pin2
                l            -0.5
                2            -1.5
                3            -2.5
                4            -3.5
                5            -4.5
                6            -5-5
                7            -6.5
                8            -7.5
                9            -8.5


    b.   Resolution Limits of the계／z) Converter

      Set the pin 5 potentiometer voltage to -2.5 V. Reset the counter to 0. Apply single pulses
until the op-amp output changes. Now, slowly increase the pin 5 voltage (more negative) until the
op-amp (Fig. 16-5) output just changes. Read the pin 5 voltage.

                                          v=
      Apply a single additional pulse to the counter. This should make the op-amp (Fig. 16-5) out-
put change. Now, increase the potentiometer voltage at pin 5 (more negative) until the op-amp out-
put just changes. Read the pin 5 voltage.

                                          V=
                                                       195

===== PAGE 211 =====
     Change the pulse generator to 1000 Hz and use EXT TRIG NEG (see Fig. 16-1). Check the
input to pin 4 of the op-amp (Fig. 16-5) to see if it is a 9-V negative staircase [as in part 1(a)]. Now
view the output (pin 10)of the op-amp of Fig. 16-5. Vary the potentiometer connected to pin 5 of
the op-amp of Fig. 16-5 and monitor the output of the op-amp of Fig. 16-5.

     1.   What are the output voltage levels of the wave pattern?

                        Vmax   =                             Vmin   =




      2. Does the rectangular pattern viewed change smoothly or in steps? Sketch the wave pattern for the volt-
age at pin 5 = -3.5 and -4.5 V in Fig. 16-6(two patterns). Show the time scale. Label on Fig. 16-6.




                                         Fig. 16-6. Comparator output.




REQUIRED RESULTS


Using positive logic, complete Table I 6-2R corresponding to Table I 6-2E for the NBCD equivalents
of the voltages applied to pin 5 (Fig. 16-5.) The table should have is and 0s.




                                                       l96

===== PAGE 212 =====
                                       Table 16-2R. NBCD equivalents.

                                                 Typ이405 Logic Levels
                           Pin 5
                           Voltage       /in 8      Pin 6      Pin 4    Pin2
                               -0.5
                               - 1.5
                               -2.5
                                3.5
                               -4.5
                               -5.5
                               -6.5
                               -7.5
                               -8.5



미SCUSSION


1.   Based on the data of Table 16-IE and Fig. 16-2, what is the LSB voltage value for the value of
     RF used in Fig. 16-1 for part 1(a)?




2.   Repeat I for part 1(b).




3.   For the value of RF used in part 1(a), what is the MSB voltage?




4.   The D/A converter of Fig. 16-1 has a four-step ladder. With the RF of part 1(a), the resolution
     is poor. To improve the resolution, a fifth step can be added. What resistance value should be
     used in the ladder, and what will the new value of the LSB be?




                                                   l97

===== PAGE 213 =====
5.   What will happen to the ladder resistance values as you attempt to make the value of the LSB
     smaller and smaller to give better resolution?




6.   What effect does an incorrect resistor in the binary ladder have on the precision of the D/A
     conversion (see Fig. 16-4 and compare with Fig. I 6-2a)? Discuss.




7.   In part 2(c),explain why the pattern changes in steps.




                                                l98

===== PAGE 214 =====
                                                                   Experiment 7



Comp1emen1ory SymmeIry
MOS(CMOS)-
Principles and Charoderistics




OBJECT


    1.   With complementary symmetry MOS(CMOS)to study logic operations.
    2.   With complementary symmetry MOS(CMOS)to study noise immunity.
    3.   With complementary symmetry MOS(CMOS)to study dissipation.


EQUIPMENT REQUIRED


   IC type 4007 dual complementary pair plus inverter
   Potentiometer, 500 l2, 3 turns, 5 W
   dc power supply-variable,0 to +15 V, regulated at 50 mA
    CRO,dc coupled and calibrated
    Pulse generator-variable-amplitude positive-going,0 to +15 V, ito 10 kHz
    Capacitor, 4700 pF, 100 or 200 V
    dc miiliamnieter, 1 mA
    dc microarnnieter, 100 .zA




                                                    l99

===== PAGE 215 =====
                                    IC manufacturers'part numbers.
                                                                                   National
           JType           Rc;4              Motorola            Fαirchrk/      Semiconductor

            4007      CD4007AE/BE         MCI4007UBP             F4007DC          CD4007AN
                      CD4007AF/BF         MCI4007UBL                              CD4007AD




                   VOD
                                                            11




                                           卄                                 VOD = Positive supply
                                                                               voltage to pin 14
                                                                             Vss= 0 (ground) to
                                                                               pin 7




                   vss

                             Fig. 17-I. 4007 pin and internal connections.



EXPERIMENTAL PROCEDURE


The 4007 used in this experiment is a universal gating IC with connections available so that they
can be interconnected to perform several logic functions. It will be connected in this experiment
to perform the functions of a 3-input NAND gate (positive logic), 3-input NOR gate (positive logic),
and triple inverter.
      CMOS ICs have gate input voltage limitations. The input gate voltage V1 must always satisfy
the limitation VS8 < V1 < VDD. This means that in this experiment V1 can never exceed VDD.
Otherwise, the IC can be damaged. Be careful, therefore, that VOD is applied to the IC before any
positive y0/rαge is α／7Plied to any inpur.

===== PAGE 216 =====
1.   3-Input NOR Gate


                        VDD


                         l         ,
                                                                                       Connect
                                                                                       Pin 13 to pin 2
                                                              g`
                                                                                       Pin 1 to pin 11
                                                        10                             Pin 12 to pin 5 to pin 8
                                                                                       Pin 7 to pin 4 to pin 9
                                                                                       V00 = +10 volts to
                                                                                         pin 14
                                                                                       V5s= 0(ground) to
                                                                                         pin 7

                                       Fig. 17-2. 3-input NOR gate.


     (a)   Apply voltages to the pins indicated and measure the voltage at pin 12 to complete
           Table 17-1 E.

                                                 Table 17-1E. 3-input NOR gate.

                                       Pin (i           Pin 3          Pin 10          Pin /2
                                             n                     0               0

                                             0                     0    +10
                                             0          +10                        0

                                             0          +10             +10

                                       +10                         0               0

                                       +10                         0    +10

                                       H 0              +10                        0

                                       +10              +10             H 0


     (b)   Repeat the data of part (a) in Table 17-2E, but with VDD = +5.

                                                 Table 17-2E. 3-input NOR gate.

                                       Pin 6           Pin 3           Pin 117         Pin 12

                                             0                     0               0

                                             0                     0          +5
                                             0                +5                   U

                                             0                +5              +5

                                        +5                         0               0

                                        +5                         0          +5

                                        +5                    +5
                                                                                   0

                                        +5                    +5              +5
                                                        201

===== PAGE 217 =====
2.   3-Input                 VDD
     NAND Gate

                o----.-----                p
                                                                                   Connect
                                                          6
                                                                                   Pin 1 to pin 12 to pin 13
                                                          ;3                  12   Pin 2topin l4to pin 11
                                                         10                        Pin 4 to pin 8
                                                                                   Pin 5 to pin 9
                                                                                   V。
                                                                                    。 = +l0voltsto
                                                                                    pin 14
                                                                                   Vss= U (ground) to
                                                                                     pin 7

                                               Fig. 17-3. 3-input NAND gate.

Apply voltages to the pins indicated and measure the voltage at pin 12 to complete Table I 7-3E.

                                                   Table 17-3E. 3-input NAND gate.
                                               八n 6        Pin 3      Pin /(7       Pin /2

                                                  0               0           0

                                                  0               0    +10
                                                  0        +10                0
                                                   0       H 0         +10
                                                +10               0           0

                                                H0                0     +10
                                                +10         +10               0
                                                H0         +10         +10

3.   Transfer Characteristics


The IC will be connected as a triple inverter and the transfer characteristics measured for one of the
inverter sections, the pin 6 input, pin 8 output section.


                V。
                 0

                                                                                      Connect

                                                                                      Pin 14 to pin 2 to pin 11
                                                                                      Pin 8 to pin 13
                                                                                      Pin 1 to pin 5
       500 2
                                                                                      Pin 7 to pin 4 to pin 9
       3 Turn
                                      8-
                                ：》
                        6{
                                                                                      VDD to + voltage to pin 14

                                                                                      Vss= 0 (ground) to pin 7




                                     Hg. 17-4. Inverter transfer characteristics.

                                                           202

===== PAGE 218 =====
     Measure the voltages at pin 6 and pin 8 for each value of VDD to complete Table I 7-4E. Plot
the data on the curve sheet in Fig. 17-5 as you take the data.

                                                      Table 17-4E. Transfer characteristics.

                  VDD = +3.5 γ                         γDD = +5 F/                    yDD = +10 γ                γDD = +15 y
             ／꺄兀α       （九αPLα                   ／꺄兀궁r           （九tput             Input       0utput         ／쨔'Ut     （기ltput
             V/in 6      y /in 8                 I'/ in 6         V Pin 8           y /in 6     VPin 8         F'Pin 6    VPin 8

              .   0                                    0                              0                          0
                          3.0                                       4.5                          9.0                       13
                          2.5                                       4.0                          8.0                       11
                          l .75                                     2.5                          5.0                        7.5
                          1.0                                       1.0                          2.0                        4

                          0.5                                       0.5                          1.   0                     2

             +3.5                                     +5                             +10                        +15



                                                      15




                                   ㅇ＞ 小 ＝ ㅇ＞尸그口싣ㄱ ㅇ
                                                       0




                                                       5




                                                      0                   5                10             15
                                                                          Input volts - V1
                                                           Fig. 17-S. Transfer characteristics.



4.   Dissipation


The IC interconnection for this part of the experiment is the same as for part 3.
     DO NOT connect the square-wave generator to the IC until VDD has been applied. The square-
wave voltage to be applied will be 0.9VDD . Be careful that it does not exceed VDD . Note that
VDD is being changed. Increase VDD before increasing the square-wave generator voltage. The out-
put at pin 8 should be a square wave with output between 0 and VDD.




                                                                              203

===== PAGE 219 =====
                                                                  1 ma DC



                                             To Pin 14
            Square wave



                                                           1ㅗ 土
                                                              ！
              generator
                                                                                                   VOD
         POSITIVE GOING                                                  CRO                      supply
             = 0.9 VD0
          1 kHztol0kHz                                         CL
                                                               4700 pF



                                   Fig. 17-6. Circuit for dissipation measurement.

      Apply VDD and then adjust the output voltage of the square-wave generator to 0.9VDD. Mea-
sure 'DD under the conditions indicated to complete Table 17-SE.

                                 Table 17-5E. 'DD vs. frequency and load capacity.
                                                             Frequency a
                                                             / kHz       4kHz        /0 kHz

                                          CL = 0
                        V00 = +5 V
                                          CL = 4700 pF
                                          CL = 0
                        VDD = +10V
                                          CL = 4700pF
                                          CL = 0
                        VDD = +15 V
                                          CL '4700pF
                             a If IDD exceeds 1 mA,indicate the frequency at which this occurs.



5.   Quiescent Dissipation


Disconnect the square-wave generator from pin 6.

     (a)    Ground pins 6, 3, and 10. Measure 'DO . IflDI is too small, change the 'DO meter to

            the I 00-'zA meter.                                                      1DD =

     (b) Connect pins 6, 3, and 10 to VDD. Measure '00.                              '00 =


REQUIRED RESULTS


Complete Table 17-SR for gate dissipation (PD)versus frequency and capacity based upon the data
of Table 17-SE. Dissipations are to be expressed in microwatts.




                                                         20．
                                                           叉

===== PAGE 220 =====
                                               Table 17-SR. PD vs. frequency and load capacity.

                                                                                     Free7uency
                                                                                     / ki7z       4kHz     /0 k//z

                                                                 CL = 0
                               VDD            +5 V
                                                                 CL = 4700 pF

                                                                 CL = 0
                               VDD = +10V
                                                                 CL = 4700 pF

                                                                 CL - 0
                              VDD = +15 V
                                                                 CL = 4700 pF


     Plot the results of Table 1 7-5R on the graph paper, Fig. 17-7, for the capacity value CL = 4700
pF for each of the three values of VDD. Draw a straight line on the graph for each value of VDD
and extrapolate the line out to either 200 mW or 10 MHz, whichever occurs first.

                                   106




                                   1 o5




                   口늠鷺孔I듬一Hm욘 ＂
                              쓰。
                                     0  4




                                     0  3




                                   102

                                   40


                                        o 0
                                    ^
                                    z


                                    d
                                    1

                                              m
                                              으                         寸口卜


                                                  m0" × "     n0" × 寸
                                                                                                     CoC
                                                                                                                     닐
                                                                              Frequency Hertz
                                                  旽
                                                            17-7. 긔：
                                                                   )issipation P0 (watts) vs. frequency.




                                                                               205

===== PAGE 221 =====
DISCUSSION

1.   Based upon the results of Tables 17-1 E, 1 7-2E,and 17-3E, the logic levels (in volts) for positive
     logic are:

                                        Table 17-ID. Gate logic levels.
                                                                  Voltage Levels for:
                                    Table         yi)D              I               0
                                    17.1E         +10
                                    17-2E          +5
                                    17-3E         +10




2.   Based upon the data of Table 17-iD, what can be said about CMOS gate logic levels when
     referred to VDD - V8?




3.   Using the pin numbers as the logic inputs and outputs, and for positive logic, write the Boolean
     equations for the gates of Figs. 17-2 and 17-3.
         (a) Fig. 17-2
         (b) Fig. 17-3



4.   Define the gate input transition voltage V1 as the input voltage V1 at which the gate output
     voltage = (VDD - Vss)/2. Based upon the data of Table 17-4E and the curves of Fig. 17-5,
     determine Vr and compute its proportion of VDD - v8s, and enter in Table 1 7-2D.

                                        Table 17-2D. Transition voltage.
                                                                           yr   '

                                     VDD - yss           '
                                                             ''         γi끄）- Vs8
                                            3.5
                                            5.0
                                        10.0
                                        l5.0




5.   In Table 17-3D, compute the high-level (VDD - Vr) and ground-level (Vr - V55) noise immun-
     ities for the inverter of Fig. 17-4 based upon the data of Tables 17-iD and 17-2D.




                                                        （陌
                                                        2

===== PAGE 222 =====
                                           Table 17-3D. Noise immunity.
                                                             Noise Immunity
                                               High Level                     Ground Level
                    VDD - i눙S          Volts     % (7/ yDo - Vss       nm`       % of VOD - VS5
                        3.5
                        5.0
                       10.0
                       15.0




6.   The expression for the dissipation due to gate output capacity loading may be expressed as

                                                  PD= KCLf pW

     where f is in kHz and CL in pF. There is a different value of K for each value of VDD - VSS.
     Select a value of PD at some frequency from the graph of Fig. 17-7 for each of the supply volt-
     ages and compute K. Tabulate in Table I 7-4D. Show calculations.

                                        Table I 7-4D. Dissipation constant K.

                           VDD - VSS            Pz)                      f
                            rvolts7            rpF力         CL (pF7     (kHz)        K
                                 3.5                         4700
                                 5.0                         4700
                                10.0                         4700
                                15.0                         4700



7.   (a) The input capacity of a CMOS gate is 5 pF and its input resistance is so extremely high
         (1012 f2) that resistance loading effects can be neglected. A 4007 gate is required to drive
         40 gates at a frequency of 200 kHz. VDD - v88 = 10 V. Using the value of K from
         Table 17-4D, determine the dissipation.




     (b) Repeat for f = 40 kHz.




                                                      207

===== PAGE 223 =====
     (c) Plot the results of parts (a) and (b) on Fig. 17-7. Connect them with a straight line and
         extrapolate out to either 200 mW or 10 MHz. Label with the voltage and value of CL.




8.   The rated maximum quiescent device dc input current 'L is 0.1 PA at VDD - vss = 10 V.
     This comes from the 4007 data sheet. There is no signal applied to the inverter inputs. How
     does this rating compare with your data of part 5?




                                               208

===== PAGE 224 =====
                                                            Experiment 8



(omplemenlory S9mmeIry
MOS(CMOS).-
IlL InlerFace


OBJECT

To study the problems and methods of interfacing the CMOS logic family with the bipolar TTL
logic family.


INTRODUCTORY THEORY


The CMOS logic family can be operated at the same power supply voltage as TTL but with a
sacrifice in speed. To operate the CMOS family at its maximum speed requires operation with
VDD - Vss equal to 15 V. To interface with TTL requires a level-shifting device.
     CMOS logic elements can easily drive other CMOS elements becauseof their high input re-
sistance. However, mast CMOS logic elements cannot provide the current required by a single UL
of the medium-power TTL series. To satisfy this current requirement requires higher-current CMOS
buffer elements.
      A sink is a logic element that is required to accept an external current. Convention is to
identify such a current with a minus (-) symbol. A source is a logic element that is required to
supply an external current. Convention is to identify such a current with a plus(+) symbol.


EQJIPMENT REQ(기RED

    CR0, dc coupled and calibrated
    dc power supply, 15 V variable, regulated at 50 mA
    dc power supply, 5 V, regulated at 50 mA

                                                    209

===== PAGE 225 =====
     Switch bank,5 switches per bank
     IC type 7406 hex inverter, open-collector outputs, high voltage
     IC type 4001 CMOS quad 2-input NOR gate
     IC type 4050 CMOS hex noninverting buffer
     470- 2, 土10% composition resistor
     Two 1-k2, 土10% composition resistor
     2.2.k&1, 土10% composition resistor
     4.7-k&1, 土10% composition resistor
     10-ku2, 소10% composition resistor
     15-kn, 士10% composition resistor
     47-ku, t 10% composition resistor

                                          IC manufacturers' part numbers.
                                                                                            National
             7：까7e             R(=;4                Motorola           Fairchild          Semiconductor

             4001          CD4001AE/BE           MC14001BP             F4001DC            CD4001AN
                           CD4001AF/BF           MC14001BL                                CD4001AD

              4050         CD40S0AE/BE           MCI40S0BP             F40S0DC            CD40S0AN
                           CD40S0AF/BF           MCi 40S0BL                               CD40S0AD

              7406                               MC74O6P               7406PC             DM7406N
                                                 MC7406L               7406DC             DM7406D



EXPERIMENTAL PROCEDURE


In using CMOS ICs, connect VOD and vss before applying other voltages. Disconnect them last.


1.   4001 NOR-Source (Fig. 18-1)




                                                                  VOD = + 5 volts to
                                                                    pin 14
                                                                  Vss= 0 (ground) to pin 7




                                                 Fig. 18-I. Source.


Measure V。  1t at pin 3. Use a CRO sensitivity of I V/div. Measure voltages to 0.1 V. Tabulate data
in Table 18-IE.

                                          Table 18-1E. 4001 inverter-source.

                     R           的          ／α kn      4. 7k요      2.2 kn          / kn       470 `2

                     V。
                      ut




                                                         210

===== PAGE 226 =====
2. 4001 NOR-Sink (Fig. 18-2)

                                                     VDO




                                                                 VDD = +5 volts to
                                                                   pin 14
                                                                 VsS= 0(ground) to pin 7



                                                   Fig. 18-2. Sink.

Measure V에t at pin 3. Tabulate data in Table 18-2E.

                                   Table 18-2E. CD400I inverter-sink.
                   R           여        10kn           4.7 kfz        2.2 k1      / kf      47α n

                  v。
                   ut


3.   TTL to CMOS (Fig. 18-3)


When CMOS is operated at a VO greater than the +5 V VC of TTL, a TTL gate with an open
collector having a high voltage rating (such as the 7406) can be used.
     View the wave patterns at pin 1 of the 4001 and pin 3 of the 4001. If a square wave is seen,
describe it by SW and the voltage levels. For example, SW between +10 and 0 indicates a square
wave whose levels are +10 V and 0 V. If no SW is seen, indicate as "none." The results are to be
tabulated in Table 18-3E. Do not disconnect Fig. 18-3.




              Square wave
               generator
                 +5 V
                10 kHz

                               - Vcc = +5 V to pin 14                             VOO topinl4
                               느‘ 0 (ground) to pin 7 ㅜ                        ==V55 (ground) to pin 7




                                               +
                             Vcc                                    VOD
                         Power supply                            Power supply
                          = +5 volts
                                         －그－
                                               Fig. 18-3. TTL to CMOS.

                                                        2ii

===== PAGE 227 =====
                                                         Table 18-3E. TTL to CMOS.
                                                                        SW Description
                                                                           400 八n
                                             VDD           V8      417αJ ^n /   4001八n 3
                                              +5           +5.0
                                             +15           +5.0
                                             +15          +15



      4.      CMOS to TTL (Fig. 18-4)



                To CR0
               EXT TRIG              +15 V



                                 15 kl




                                                         F>
Square wave                                          1
 generator
   +5 V                                                                                                    +5 V
                                                     2



                                               I
  10kHz
                                                                       "       "
                                 47 kZ
                                                                                   >'
                                                                                                 1k




                                     7406          Vcc= +5 volts to pin 14
                                                   0 (ground) to pin 7
                                     4001          V00 = +l5voltsto pin 14
                                                   vsS = 0 (ground) to pin 7
                                     4050          vcc = +5 volts to pin 1 (note pin number)
                                                   Vs$ = 0 (ground) to pin 8

                              Fig. 18-4. CMOS (4001) to TFL (2-7406) using CMOS (4050) buffer.


      To go from standard CMOS to TTL directly is difficult because of the limited driving capability of
      the basic CMOS gate. The 4050 is designed to drive 2 TTL loads from CMOS. It requires only a
      +5-V vcc power supply (no VDD).
           View and sketch the waveforms on Fig. 18-5 at

              (a)   4001 pin 1
              (b)   4001 pin 3
              (c)   4050 pin 2
              (d)   7406 pin 4




                                                                     2l2

===== PAGE 228 =====
              +5
      7406
      pin 1
               0



      4001
      pinl     0
                                                    (a)
      4001
      p1n3
               0
                                                   (b)


      4050
      pin2
               0
                                                     (c)
      7406
      pin4     0
                                                   (d)
                                    Fig. 18-S. CMOS/TI'L interface.


REQUIRED RESULTS

For parts I and 2, for each value of resistance and the measured output voltage, the source or sink
current can be computed. Complete Tibles 18-IR and 18-2R by computing the currents. Express
currents in milliamperes.

                                  Table 18-IR. 4001 Inverter-source.
                     R = （그（)   R = ／〃kn     R = 4.7k요     R = 2.2 k요   R = / kn   R = 47α n

         v。
          ut
         I



                                   Table 18-2R. 이沁I Inverter-sink.
                     R '= 띠     R = /0 k&2   R = 4.7kn     R = 2.2 kn   R = / kZ   R =470 n

         v。
          ut
         I


     Plot the results of parts I and 2 (Tables 18-I R and I 8-2R) on Fig. 18-6. Plot output voltage
versus current. Label each curve carefully.


                                                 2l3

===== PAGE 229 =====
                                                  I IㅣI ㅣIㅣi l I l t    -ㅣㅣㅣ ㅣI I L
                                                           4001
                                         o



                         mmㄴ ㅌm
                              =＝ㅌ`
                                 Hㄷ ㄴ＝
                                     U
               -
              -



               -


               ㅡ
              H


               ㅡ
              -




                            。
                            m      ㄴ
                                   m
                     -



                     ㅡ



                     ㅡ



                     -

                                         5
                                    ㅡ



                                    ㅡ



                                    -



                                    -




                                             ㅡ



                                             -




                                             ㄱ
                                             -




                                                  ㅣ- I ! I Iㅣl Iㅣ 1 I l i i i
                                         00      1      2     3      4        5
                                                          v。
                                                           ut - V이ts

                     Fig. 恪6. CMOS gate load characteristics, Tables I 8-IR and 18-2R.

DISCUSSION

1.   To drive a 1-UL medium-power TTL gate at the 0 state, the CMOS driver must be able to act as
     a sink and sink -1.6 mA at a voltage of 0.4 V. From the curve of Fig. 18-6, can the 4001 sink
     the required current if the 4001 is operated at the +5-V supply voltage of TTL? How much
     current can it sink?




2.   The 4001 has four separate NOR gates which can be connected in parallel. How many such
     parallel gates are required to sink I UL of TTL logic? Show calculations.




3.   The TTL type 7472 clocked J-K flip-flop clock input requires 2 UL. How many 4001 parallel
     inverters would be required to drive it at the 0 state?




4.   To drive a 1-UL TTL gate at the I state, the CMOS driver must be able to act as a source and
     source +40＇』A at a voltage of +2.4 V. Can the 4001 source this current at this output voltage?




                                                           2l4

===== PAGE 230 =====
5.   Discuss the results of part 3. Explain the amplitudes of SW voltages obtained at pins 1 and 3
     of the 4001 for each set of values for VDD and V. If no SW output is obtained, explain.
     (Note: The CMOS gate transfer voltage V. occurs at approximately 50% of VUD.)




6.   Discuss the results of part 4. Discuss the amplitude of the waveforms for each part.




                                                 2'S

===== PAGE 231 =====

===== PAGE 232 =====
                                                                                             "               EXPERIMENT
                                                                           ASTABLE MULTMBRATOR


OBJECTIVES                                                              a further increase in bias will not result in an increase in
I. To observe collector and base waveforms in a                         C이lector current. At mat bias level, collector saturation
                                                                        has been reached.
   free-running c이lecior-coupled multivibrator
2. To measure multivibrator frequency                                4. In an NPN transistor forward bias in the base-emitter
3. To synchronize the multivibrator                                     junction is increased by driving the base more positive
                                                                        r이ative to the emitter,
                                                                     5. An increase in collector current flowing in the collector
INTRODUCTORY INFORMATION-                                               load resistor causes me voltage at the collector to
                                                                        decrease. Therefore an increase in collector current in art
Classes of Multivibrators                                               NPN transistor will cause the collector voltage to go more
There is a 이ass of RC-coupled oscillators called multivibra-            negative, while an increase in collector current in a PNP
tOrs ，먀iich generate nonsinusoidal waveforms, such as                   transistor will cause the collector voltage to go more
square, rectangular, triangular, or sawtooth waves. These               positive.
waveforms find many applications. The most familiar is the           6. A decrease in current in the collector load resistor will
sawtooth wave which is employed as a time base. or sweep, in            cause the v이 【age at the collector to increase. Therefore a
oscilloscopes.                                                          decrease in collector current in an NPN transistor ,ml
   The multivibrator is one form of relaxation oscillator.              cause the collector voltage to go more positive, while
Multivibrators may be self-excited (also calledfree-running),           in a PNP transistor the collector voltage will go more
requiring no external excitation. Or they may be driven                 negative.
oscillators whose operation and frequency are controlled by          7. The voltage across a capacitor cannot change instan-
external driving or triggering voltages. Free-running multi-            taneously; that ㅈ＄, it takes time to charge or discharge a
vibrators are called astable. The frequency of astable multi-           capacitor. A measure of this time is called the time con-
vibrators may be contr이led by external synchronizing                    stant. In an RC circuit, one time constant in seconds is
p미ses.                                                                  equal to the product of the resistance R (through which the
   Driven multivibrators are not strictly oscillators, for they         capacitor is marging or discharging) in ohms times the
require external driving pulses to start their operation and            capacitance C in farads. Ohms times microfarads, of
maintain it. There are two classes of driven multivibrators:            course, yields microseconds.
the monostable (sin인e shot), which has one stable state; and
the bistable (flip-flop, or trigger), which has two stable states.   OperatIon of Collector-Coupled MultlvibratOr
   Transistors may be used as the amplifying device for              Figure 19- I is the circuit of a collector-cou미ed multivibratOr.
multivibrator circuits. Transistor multivibrators are either         c` and e2 are NPN transistors ，나iose collectors are con-
collector-coupled or emitter-coupled. In this experiment we          nected to the positive voltage source ｀뇨，through load
shall be concerned with the operation of a free-running,
collector-cou하ed multivibrator.
   The properties of transistors which cx하amn multivibrator
action are as follows:

1. An increase in base current causes an increase in collector
   current, and conversely a decrease in base current causes
   a decrease in collector current.
2. An increase in forward bias in the base-emitter junction
   increases base current; a decrease in forward bias reduces
   base current.
3. In a PNP transistor, forward bias is increased in the base-
   emitter junction as the base is driven more negative rela-
   tive to the emitter. However, a point may be reached where                   P.g 19.1. CoIIector.couped muttivibi'ator.

                                                                     217

===== PAGE 233 =====
resistors RLi and RL2. respectively. 재e bases of Q】and 口2
are biased, respectively, by resistors R1 and R,. Any 야‘ange
in voltage at the collector of C I is coupled by C큰o the base of
Q2, and similarly any voltage change at the collector of Q2 is
coupled by C콰o the base of이. It will be shown that C1 and
C2 provide regenerative feedback to sustain oscillation in 巾is
RC-coupled oscillator.
     To analyze circuit operation let us assume that the two
                                                                                             r口 J                                           rb7
circuits are symmetrical; that is, q and 口그are the same type
transistor, RLI = RL2, R` = R2, and C1 = c2; ，싸ken                    FIg.19-3. (a) Capacitor C1 discharging through R2（긔 ,$ ON, O2 is
switch 옥 is closed, power is applied to both transistors.             OFF. rb) Capacitor C2 discharging through R,. O2 `$ ON,（긔 IS OFF.
Current starts【ㅇ flow in the collectors of Q` and Q2. Since it
【＄ not conceivable that both transistors draw exactly the same        collector resistance of q and through R2 toward Vc' (see
 amount of current, assume mat the collector of 口1draws               Fig. 19-3a). Since the emitter-collector resistance of 이，
more current than that of Q,. 가erefore the voltage at the             saturated, is very low, 出e effective-discharge time constant
collector of Q` will go more negative than the collector              for C1 is R, ×（긔．The voltage vir at the base of Q2 will
 voltage of α2. 까uis negative voltage change of 口Iwill be             change as q discharges, in the manner shown in Fig. 珊4.
 coupled by c1to the base of 口2' reducing the forward bias on            When the voltage at the base of Q, has increased from
 Q2· Accordingly collector current in Q, will decrease, and           - 10 toO V to a low value of positive voltage, c2 is brought
 the collector voltage of Q-, will go more positive. This             out of cutoff to conduction, Q2 base current and c애ector
 positive duange is coupled by C, to the base of9bincreasing          current start to flow. The voltage v.2 at the collector of C2
口1base current and collector current. The voltage at the              drops, and this negative voltage change is coupled by C2 to
 collector of 의 will go more negative, driving the base of Q2         the base of의, reducing base current and collector current in
 more negative, reducing c그collector current further, thus            口rAs collector current in c` is reduced, the collector
 driving the collector voltage of Q, even more positive. In           voltage of口1, vci , rises. This positive change at the collector
 very short order this regenerative feedback from the collector
 of one transistor to the base of the next will cause 이collector                                    O, OFF             02 ON                  02
                                                                                                                                                   OFF

 current to rea야｀saturation ，나uile Q2 collector current is cut                                      O, ON              。 , OFF                O, ON


 off. We say that 이 is Or' and Q2 is OFF. 가ie action is
 practically instantaneous.                                                                                                         C
                                                                                                                                     /
                                                                                       J 。
      1-low long does Q1 remain oN and Q, OFF' 재e time
 constant GR, (approximately) determines this. 吹【 us see
 how. Assume ( ] ) that V-C = + 10 V and 12) 巾at, after power              '11


  is applied and c` saturates the collector voltage, V.1 of Q 1                                              S1
                                                                                                                  CF4ARGE           ,/q
  drops practically to 0: that us. the collector-to-emitter
                                                                                                            I                              I             ;

                                                                                                                                                             `
  resistance of 이 approaches 0. 가u`s 10-V negative mange at                                          ''- -*4-4- - 'l - - *4.* - - ,, - -.0-1
  the collector looks like a neoative 10-V battery to（긔. and ai                                             -            ㅣ                 1
  the instant of change the circuit to (1 "looks" luke that in                                              1              l               -



                                                                                                                                   r
  Fig. 19-2. Since the voltage acrocs （二 cannot changc
   instantaneously, the entire 20 V must appear across R,. and             'C 그


   the voltage with respect to ground at 냐icJunction of C1 and R,
  (point B그. the base of Q9 must measure - t0 V. cutting off
   c2. Capacitor q starts dicchareing through the emitter-
                                                                                                                                   -
                                                                                                                                   ㅣTOWARDS + V枕 Imvi
                      c1                                                                                                              -/ //



                                                                                                                                          다．ARcE


            VOLTAGE
   10 V -=- 아 ANGE AT                            b0y -ㅌ- vcc
            COLLECTOR O,
            .4-
                                                                           ' '`
                                                                                                                     C1 cH^ F1GE



                                                                                   0

     Fig.19그 Voltage c. 'sees' at the Instant that O, saiurates           Fin 19.4. V
                                                                                    《Itaae waveforms in NPN coiiector-cou이ed mu1tiv,braiOr.

                                                                    218

===== PAGE 234 =====
of 0' is cou짇ed by C1 to the base of o2' increasing Q2base             and Q2 are 1800 out of phase. Similarly, the waveforms at the
and collector current. Collector voltage at Q2 goes more               bases of c1and Q2 are 180' out o갸hase.
negative, driving the base of口1more negative. Again almost
instantaneously, as 02 starts conduc山，     g, the regenerative
                                                                       Frequency of Collector-Coupled Multivlbrator
feedback action turns o2 ON and turns q oFF. Q2 remains ON
as long as c1 is otF. The length of time c1remains OFF is              The period z of a complete cycle of the Thquare" wave at the
determined by the C2凡 time constant, for the voltage VBI at            collector of 의 or 02 is represented by the time interval AC
the base of c1 is determined by the discharge of C, through            (Fig. 19-4); that is
the emitter-collector resistance of 蝦 and through 시, as in
                                                                                                                              r = II + r2                     (19-I)
Figs. 19-3b and 19-4.
   When q starts to conduct, it switches Q2 on. When Q2                The frequencyf of the multivibrator is therefore the inverse
starts to conduct, it switches q onr. The length of time 의             of the period 1, or
conducts is determined by the length of time Q2 is on (see
waveform v82, Fig. 19-4). The length of time c2 conducts is
determined by the length of time 의 is cut off (see VBT, Fig.
                                                                                                                          =    -   1    =       긔
                                                                                                                                            1 + Z,
                                                                                                                                            h                 (19-2)

                                                                          We can approximate the time intervals :1 and ' 2 and thus
l94).
                                                                       arrive at an approximate equation for frequency.
   The idealized waveforms in Fig. 194 merit some discus-
sion. We see that as the base voltage v8, of Q2 is driven 10 V                                                  r =           1
                                                                                                                                                              (19-3)
negative during the interval t1, the c이】ector voltage v'2 ofc2                                                        O.7C1R2 + 0.7C2凡
goes 10 V positive, Vcc. We might expect that the v이tage at
                                                                       The reason for Eq. (19.3) becomes apparent when we exam-
the collector of Q, would rise to Vcc the moment Q2 is
                                                                       inc Figs. 19-3 andl94. The interval r1 is determined by the
switched oFF. However, this is not so, since capacitor C,
                                                                       time it takes C1 to discharge through R2 from a level of - 10
cannot charge up instantaneously to Vcc. Therefore v(-2 rises
                                                                       to 0 V (approx). This is a change of 10 V, out of a possible
to Vcc at the rate determined by the charge of Cnhrough 凡2
                                                                       change of 20 \/ (note mat C1 discharges from - 10 toward
in series with the emitter-base resistance of口1. See Fig.19-5
                                                                        + 10 V). This is a 50 percent change in charge. Reference to
for the charging path of C2. The exponential rise in voltage of
                                                                       the universal charge and discharge 山ne-constant chart, F培
 vc2 represents the charge of C2. At the end of the time
                                                                       19-6, 計tows that a 50 percent charge or discharge requires 0.7
interval 小 when v81 has risen from cut off to conduction, the
                                                                       of a 山ne constant. Hence
 V이【age at the collector ofc2 drops from + Vcc to a very low
 value (close to 0). At that instant q is switched oFF and the                                                                it = 0.7C1R2
 voltage v.1, at the collector of의. starts rising from 0 toward
                                                                       Simnar}y,
                                                                       Similarly,
  + vcc. The exponential rise in v.1 is the result of（二 charg-
 ing toward + vcc through RLI· At the end of period 12, when                                                                  '2 = 0.7c2시
 v81 has risen from 기0 V to a slight positive v이tage, 口1 i$
                                                                       Example. A numerical example will illustrate how the fre-
 switched ON and c2 oFF, and the cycle is repeated.
                                                                       quency of a collector-coupled transistor multivibrator may be
   It ｀〃m be noted mat the ON-OFF time of each transistor is
                                                                       calculated using Eq. (19-3).
 equal, since the circuits are symmetrical. That is, the time
                                                                         Suppose mat
 duration of the positive and negative alternations of Q1 and
 Q2 are equal, t = '2. The waveforms at the collectors ofc긔                                                      R1 = R2 = 500,000 n
                                                                                                                 c' = C2 = 0.1 pF


                                                                                                       미

                                                           RL3
                                                                                                      郞


                                                                                                      .
                                                                                                                                                      -



                                                                          山。 ＜卜J0> JJ。 ， ，。 ㅒz山Uㄸ 닛
                                                                                                                                                      1
                                                                                                      兀                                      I I
                                                                                                                               ㅓ
                                                                                                      的
                                                                                                                               A. cAPACITOR VOLTAGE .N cH^nGE
                                                                                                                               B. CAPACITOR VOLTAGE 이니OISCHARG(
                                                                                                      的
                                                                                                                                                      1
                                                                                                      凹                                          ㅣ
                                                                                                      沁


                                                                                                      加
                                                                                                                                                          r
                                                                                                      10

                                                                                                      0
                                                                                                           l_         l
                                                                                                                                             3                    6
                                                                                                                                       nMㅌ II늬〃 x c


       Fig.19-5. Charge pam tor C2. 02 is cut ofl, 01 is oi.                                               ng.19-6. Universal time-constant chart.

                                                                 219

===== PAGE 235 =====
              r1 = 0.7(0.1 x lO 't(5 X I05)                               口2 would normally have been switched in at γ in the absence
                 = 0.035 S = 3.5 × 104 S                                  of a synchronizing pulse. If the 山ne interval between pulsts
                                                                          ㅣ and 2 is slightly less than the normal period of the rnultj-
SimlaHy                  1-, = 3.5 x I0-2s
                                                                          vibrator, pulse 2, 3. etc.. will lock in the multivibrator in a
Therefore                                                                 fashion similar to pulse I.
      r= 3.5 x 10- 2 + 3.5 x 10- 2 = 7 x lO-2s
                                 iO그   ..     ,,
and     / =
              :   = 7 x
                        I
                         10- 2 =  7- = 1솩 "'y i-li
                                                                           SUMMARY
                                                                            】. Multivibrators are RC-cou이ed oscillators which gener-
Nonsymmetrical Multivibrator                                                   ate nonsinusoid비 waveforms.
The 'square" wave at the collectors of c1 and Q2 may be                     2. Multivibrators are either set戶excited (free-running,
changed to a "rectangular" wave. Here the positive and                         requiring no external triggering) or driven. Driven, or
negative alternations are not equal in time, that is t1 궂 t-..                 triggered, multivibrators require external pulses to start
This inequality is achieved by making 시C2 * 蝦Cl.                               them and keep them going.
For example. let R1 = 100,000 Il and R2 = I Mfl and                         3. Self-excited multivibrators are also called asrable
Cl = C2 = 0.001 FLF. 가1e time constant q? 2 is 10 times                        multivibrators.
the value of C,R1, and therefore the waveform will be non-                  4. Transistor astable multivibrators are either collector-
symmetrical. However, Eq. (19-3) cannot be used in comput-                     coupled or emitter-coupled.
ing the frequency of an asymmetrical multivibrator. In-                     5. Hgure 19-I is the diagram of a transistor c해ector-
dividual circuit constants and conditions must be considered.                  coupled multivibrator. Note that Q1 and Q2 are cross-
                                                                               cou미ed. The output ofcifeeds 口2' and the output of Q2
Multivibrator Synchronization                                                  feeds Q1.
                                                                            6. If the time that 01 is oFt is called t and the time c, is
An NPN collector-coupled multivibrator may be synchro-                         OFF is called 12, men 巾e 山ne z of one complete cycle is
nized by ap짇ying external negative timing pulses to the base
of ci山er transistor. 가te frequency of me synchronizing                                                        I = 11 + 12
pulses mus나）  . slightly hi帥er than that of the multivibrator,              7. The frequencyfof a multivibrator毗lose period (time of
and the amplitude of the pulse must be sufficient to switch the                one complete cycle) is t is
transistors.
   Consider Fig. 19-7a. Negative synchronizing pulses are                                                       i             !
applied through C3 to the base of c1. Assume that pulse I                                            -'   =    T    =   i ,   +   '2

appears at me 山ne that Q1 is conducting. The pulse will be                  8. A symmetrical collector-coupled multivibrator is one
amplified by Q1 and appear as a positive pulse at the collector                whose equivalent components are equal. Thus if
of 의 (there is a 180" phase shift between base and collector                   0 ' = e2' R1 = R2, RLI = RL2, and（긔 = q. Fig.
voltages in a transistor am힌ifier with resistive c이lector                      19-I is symmetrical.
load). The positive pulse is coupled by C1 to the base of 口2                9. In the symmetrical collector-coupled multivibrator of
and is superimposed on vβ2, me c' 小scharge waveform at                         Fig. 19-I, r = 0.7C1R2 = r2 = 0.7C2치·
point X (Fig. 19-7b). If the positive pulse has sufficient                 K). The frequency of the symmetrical collector-coupled
amplitude, it brings Q, out of cutoff and into conduction at X.                multivibrator in Fig. 19-1 is
                                                                                                                  l
                                                                                             r   =                                     (19-3)
                                                                                                          0.7C,R2 + 0.7C,凡
                                            `YNc PULSE
                                            ^T 帥＄E 0,
                                                          e-
                                                                               wheref is in hertz, C in farads, and R in ohms.
                                                                           11. A nonsymmetrical multivibrator is one in which
                                                                               凡C1 7스 凡C2. Therefore the times :1 and 12 of each
                                                                               秋ernation are not equ川．The outputs at the c애ectors of
                                                                               o` and c2 are rectangular, ia山er than square, waves.
                                                                           12. The frequency of a nonsymmetrical multivibrator cannot
                                                                               be calculated by Eq. (19-3). Individual circuit constants
                                                                               and conditions must be considered.
                                                                           13. Free-running multivibrators may be synchronized by
                   (aJ                              r6J                        exterl硼 negative-going pulses coupled to me base of
                                                                               either transistor. ne frequency of the synchronizing
Ftg.19.7. (a) Synchronizing a multivibrator; (b) negative synchroniz-
ing pulse is amplified by Q` and appears as a positive pulse at base of        pulses must be higher than the natural frequency of the
0=?, turning Q2 00.                                                            multivibrator.


                                                                          220

===== PAGE 236 =====
SELF-TEST

다｀eck your understanding by answering these questions.
l 」 Multivibrators are oscillators whi야｀generate sine waves.
                     (true, Jo/se)
2. In Fig. 19- I . the frequency of the multivibra
                                                 【or is deter-
    mined by 山e time constants                    and

3. For the astable multivibrator in Fig. 19- I to be symmetri-
   c毗 the I해owing conditions must be met:
   Qi =                    , CI =
   R2 =                    , RL2 =
4. 듸gure 19- I is a symmetrical astable multivibrator in
   which C1 = 0.0갸kFandR, : 100 kfl. The time of one                           Fig. 19-8. Experimental multivibrator.
   con例etc cy이eis                      S
5. The frequency of the multivibrator in question 4 is
                                                                   MATERIALS REQUIRED
                   Hz.
                                                                  口 Power supply: Variable regulated low-voltage dc source
6. As the resistance of RI in Rg. 19- I is increased, the
                                                                  ■ Equipment: Oscilloscope (with dc vertical an倒ifiers. if
   frequency of the rnultivibrator is
                                                                    possible); square-wave generator (AF range)
7. In Fig. 19-8. 새 the values are as shown except R, =
                                                                  ■Resistors: Two 6800-. 10.000-. 22.000-. 33,000-. two
   270 kfi. The time during ，아＂d1 口1 is OFF IS
                                                                     00.000-fl /:-W
                    (shorter, longer) than me time during
                                                                  ■ Capacitors: Two 0． 이-.i.F: 47-. 250-pF
   which C2 is OFF.
                                                                  U Semiconductors: Two 2N6004 transistors (other choice:
8. 가ie frequency of a synchronizing pulse delivered to me
                                                                    2N3904); 1N4154 小ode or their equivalents
   base of QI (Fig. 19-8) must be                      (higher,
                                                                  ■ Miscellaneous: SPST switch; 500.000-fl 2-W potentiom-
   lower) 山an the natural frequency of 山e multivibrator, for
                                                                    eter: two 2N6005 transistors as required for extra-credit
   effective synchronization.
                                                                    expenment




PROCEDURE

Symmetrical Multlvibrator                                              frequency; record this frequency in c이umn labeled
                                                                       "Frequency, Measured."
 I. Connect the circuit of Fig. 19-8. Power on.                     6. If the trace of your oscilloscope is not time-calibrated,
 2. Externally synchronize your oscilloscope withmesign川               measure and record the frequency of the multivibrator
    from the collector of口겯 . Use the dc vertical amplifiers of        by using (for comparison) as a frequency standard a
    your oscilloscope, if available, and set the zero level of         signal from a calibrated, variable-frequency, audio sine
    the trace.                                                         or square-wave generator.
 3. Observe the waveforms at each of the test points shown
                                                                   Asymmetrical Multivibrator
    in Table 19-I ' Draw these waveforms in proper time
    phase in the table. Measure비so the peak-to-peak ampli-          7. Power off. Re이aceR2, the c2 base bias resistor, with the
    tude of each waveform. Record the data in Table 1아 . If            series combination ofR1. a 10,000-fl resistor, and R4, a
    you are using a dc (vertical amplifier) oscilloscope.              500,000-fl potentiometer connected as a rheostat (see
    show also the polarity of voltage with reference to 0. If          Fig. 19-9). Set ／乙 for minimum resistance.
    you are using a dual-trace oscilloscope, observe and            8. Power on. Observe the waveforms at the test points
    compare the waveforms at the collector and base of？】      ;        shown in Table 19-2. Draw these waveforms in proper
    at 냐ie c이lector of c ' and c이lector of α2' and at 山e base          time phase in the table. Also measure and record the
    of 口1 and collector of c2.                                         peak-to-peak amplitude of the waveforms. Measure and
 4. Compute and record the frequency of your multivibrator             record the frequency of the multivibrator.
    in C이umn labeled "Frequency. Computed." Show your               9. Set R4 for maximum resistance. Repeat step 8. Use
    compUt at ions .                                                   Table 19-3.
 S. If the trace 이
                 「your oscilloscope is time-calibrated, mea-       10. Reset R4 for a symmetrical "square" wave. Measure and
    sure and record the time t1 and t, of a complete collector         record Its frequency: / =                  Hz. Leave R4
    cycle.｛尨ing me value of r = ti + r2. determine me                  at 什us setting


                                                                  221

===== PAGE 237 =====
TABLE 19- 1 . Symmetncal M미tivibrator Waveforms and Frequency
      了esi Pol川                                                   Wav／αrm                                                   V p-p


   Collector of Q1



   Base of QI



   Collector of Q2



   Base of c2

                                                            7"71. z기sra!ion

                                  h                                                                                             x


                                                                 Fre甲4eflCY

                             computed                                                              Measured




                                                                        14. Slowly reduce the frequency of the square-wave genera-
                                                                            tor to f Observe and record effect on shape and fre-
                                                                            quency of waveform while monitoring the output at the
                                                                            collector of Q 1 .
                                                           6V               Effect 0n waveform "

                                                    Jㅍ
                                                                              Effect 才frequencv:



                                                                        Extra Credit
                                                                        15. Experimentally determine and explain the operatton and
                                                                            purpose of 寸te components in 댜te synchronizing circuit
                                                                            of Fig. 19-10. State yourprocedure.
   Ff9.19.9. O2 base bias circuit for asymmetnc계 multivibrator          16. (a) Experimentally determine ｀나tat effect, if any. the
                                                                            level of the synchronizing pulse has on synchronization.
 Synchronizing the Multivibrator                                            Explain. (b) What is the minimum-level synchronizing
                                                                            pulse which will permit stable synchroniㅗation of the
 n· Connect the output of a square-wave generator to the
                                                                            s'vmmetrical multtvibrator?
     input of me circuit in Fig. 19-10. The output of the
                                                                                                     1N4154
     synchronizing circuit is coniected to the base of 이 as
     shown. Set the square-wave-generator frequency 200                                                                e－   →       T0 BASE 0,
                                                                                                                    2凹 pF
     Hz higher than the measured frequencyf of the multi-
     vibrator (see step 田） . Set the output of the square-wave
     generator at 6 V p-p
 12. Externally synchronize me oscilloscope with 什te output
     of the square- wave generator. Observe the waveform at
     the base of q ; at the collector of c I . at the base of Q2
     Draw these waveforms in Table 194
 13. Measure and record the frequency of the multi-
      vibrator:                 Hz                                                 티g. 19-10. Multivibrator synchronizing Circuit


                                                                        222

===== PAGE 238 =====
TABLE 19-2. 尸‘ Minimum Resistance
          Test Point                                     Waveform                                               V P-p

       Collector of 이


       Base of 이


       Collector of Q,


       Base《〕f Q2

       Frequency. Hz


TABLE 19-3. R4 Maximum Resistance                                17. Draw the circuit diagram of a symmetrical, collector-
                                                                     coupled multivibrator using 2N6005 (PNP) transistors.
          7논si Point                 Waveform
                                                                     Show polarity of battery voltage.
                                                                 18. Connect the circuit. Observe the waveforms at the col-
       Collector of 口1
                                                                     lector and base of ead, transistor. In a specially con-
                                                                     structed table draw the waveforms in proper time phase.

       Base《）
            f Qi
                                                                 TABLE 19-4. Synchronizing the Multivibrator
                                                                                                  Waveform (svnchroni:ed
       Collector of Q,                                                    Test 只〃＇n                    aif + 200J
                                                                      Base of Q1
        Base of 0그
                                                                      Collector of Q1

        Frequency: Hz                                                 Base of Q그




QUESTIONS                                                          8. How is the frequency of a collector-coupled multivibra-
                                                                      b0r varied in this experiment?
     Comment on the waveforms in Table 19-1. Do the)
                                                                   9. What other method may be used for synchronizing the
  I.
     agree with the theoretical waveforms itt Fig. 19-4?
                                                                      multivibrator in Fig. 19-9?
  2. In the circuit of Fig. 19-8 what determines how long (a)
                                                                  10. (a) Can PNP transistors be used instead of NPNs in
     cI is cut oft? How long is it oFF? (b) c1 is conducting?
                                                                      designing a multivibrator? (b) What dtanges, if any, are
     How long is it conducting?
                                                                      required in the circuit?
  3. How does me computed frequency compare with the
     measured frequency in Table 19-I? Explain any dis-           Extra Credit
     crcpancies.                                                  I I . Will the level of the synchronizing pulse affect synchro-
  4. What is the effect on frequency of the muitivibrator as凡           nization? How?
     (Fig. 19-9) is (a) increased in value, (b) decreased?        12. Is∥ possible to synchronize a multivibrator with a nega-
     ，싸iy?                                                              five pulse whose frequency is twice the frequency onhe
  5. Is your answer to question 4 confirmed by the data in              multivibrator? Explain.
     >our experiment? Refer specifically to the data on which
     sour answer is based.                                        Answers to Sell-Test
  6. Would mcrc be any appreciable d 'ange in frequency if        I . false .                  5. 357
     the voltage source of the muluvibrator in Hg. 19-8 were      2' qR-.. C,凡                 6. decreased
     reduced from 6 to 5 V ' Why?                                 3. c, .; q; 시：RLi            7. longer
  7 What is meant fly synchronization of a multivibraror?         4 2.8 x l0－〕                 8 higher

                                                                223

===== PAGE 239 =====

===== PAGE 240 =====
                                                                                                                  EXPERIMENT
                                                                                                                  FLIP-FLOP


OBJECTIVES                                                               To understand the operation of this circuit, assume that
                                                                      when power is first applied. 이 conducts somewhat more
I. Totriggera 用p-flop from one conduction state to another
                                                                      heavily than c그．This drives the collector of 이 more nega-
2. To observe the effects of a pulse input on the output of a
                                                                      tive than that of e2· 가uis negative voltage is cou이ed byR5to
   flip-flop
                                                                      the base of口2' reducing the forward base-emitter bias .「o2.
                                                                      and as a res미t. reducing Q, collector current. Accordin미y,
                                                                      the voltage at the collector of Q, is driven more positive. This
INTRODUCTORY INFORMATION                           -
                                                                      positive diange is coupled by)긱 to the base of이. increasing
                                                                      collector current in 의. driving the base of 口2 more negative.
Description and Use
                                                                      The regenerative feedback action continues, as above, and in
A flip-flop is a bistable m미tivibrator. A flip-flop is a driven       a very brief time interval 口1 is conducting at saturation, with
device. Because it is bistable. it can remain in either of two        its collector voftae close to 0. As a result the effective
sta비e states until an external signal forces it to take 山e other      voltage divider providing base-emitter bias for Q1 (see Fig
state; thus the flip-flop can be used as a digital storage device     42-2) drives the base of 口2 negative with respect to its
to retain information. Flip-flops perform many computer               emitter, and cuts off 口그．nte circuit action stops; that is, this
functions, such as acting as intermediate storage for informa-        isone stable state, with c1ON and e2 OFf.
non during me computer process and as status indicators to               It is possi비e to reverse the state of conduction. mat is. turn
indicate logical conditions existing during art operation. Flip-      c2 ON and c1oun. by ap이ying an external positive trigger-
flops can also be used in a group to function as a binary             ing pulse to the base of c2' the off transistor, of sufficient
counter.                                                              amplitude to cause（견 collector to start drawing current.
                                                                      When that happens, the cc미ector voltage at 口2 is driven in a
                                                                      negative direction. This negative voltage change is cou이ed
Flip-Flop Operation
                                                                      by R1 to the base of Q. reducing collector current in Q I and
Rgure 42- I is 小e circuit diagram of a flip-flop employing            driving the 이 collector v이tage more positive. This positive
NPN transistors, though PNP transistors may also be used.             voltage change is coupled by Rdo the base ofQ2' increasing
Examination shows that this circuit is almost iJentical with          collector current in Q,. Again, by a similar aciion to that
the collector-coupled multivibrator in Expenment 19. The              previously described, in a very brief time interval Q2 is
basic difference is that the flip-flop is direci-cou하ed,.with 凡       turned on and Q1 is turned off.
and R5 re이acing the coupling capacitors C1 and C2 found in
Fig. 19-I ,




                                                                          Fig. 42-2. VoltaQe divider provides reverse bias-emitter bias 沁r02
                  Ftg. 42-1. transistor tSp-flop                          when Q1 is conducting

                                                                    225

===== PAGE 241 =====
   Itis 出so possible to reverse the states of the two transistors    SELF-TEST
by ap미ying a negative pulse to the base of the normally on           Check 》Our understanding by answering these questions.
transistor. Thus when 0코＄ON. a negative pulse at the base of
Q코＄amplified and appears as a positive pulse at its collector.       I. In the transistor flip-flop (F培 42-1), when power is first
if this positive pulse is of sufficient am미itude, it will, when         applied o1conducts more heavily than o2' As a result,
coupled by R3 to the base of 이 , switch the two transistors.                             becomes the ON transistor,
turning 01ON and o2 OFF.                                                                 小e OFF transistor
                                                                     2. Because Fig. 42-1 is a self-excited multivibrator, the
                                                                        states of conduction of c1and c2 are reversed a니,eriodic
Transistor Switching Modes                                              intervals without any external trigger pulses.
                                                                                         (true, false)
Transistor switching circuits em미oyed in computers gener-
                                                                     3. In the circuit of Fig. 42-l, ifQ isON, a
ally fall into one of two types of operation. One is called
                                                                                         (positive, negative) pulse applied to the
voltage mode, and the other is called current switching.
                                                                         base of 이 will cause Q긔 to go off and o2 ' 0 go on.
   Voltage-mode circuits operate with relatively large swings
                                                                     4. ThecircuitofFig. 42-1. Vc' = +l0V, VB＇광 = -I0V.
in signm level. Transistors in voltage-mode circuits are usu-
                                                                         When 口1 is ON, the dc voltage at the collector of Q' is
ally driven into saturation in one operating state and are cut
                                                                         approximately                  (/0, 0, -10) V.
off in the other opera山垠 state. Voltage-mode circuits are
                                                                     5. For the conditions in question 4, the c이lector voltage of
limited in their opera山埋 speed because turnoff delay is
                                                                        口, is approximately                    V
increased｀나ten a transistor is driven into saturation. For this
reason, voltage-mode circuits are employed where speed is
not essential. The circuits in this experiment and in E시)er-
ments 19 and 22 illustrate voltage-mode operation.
                                                                     MATERIALS REQUIRED
   When high switching speed is essential, circuits using the
 current-switching technique are employed. This system per-          ■ Power supply: Regulated variable dual voltage dc source
 forms digital logic functions by switching well-defined cur-          (NorE: If a dual voltage supply is not availa비e, a single
 rents, such as 6 mA, from one part of a circuit to another.           sup미y may be used, w汕 a voltage divider across it,
                                                                       connected as in Fig. 42-3. The experimental flip-flop is
                                                                       men connected to the proper taps on the v이tage divider.)
                                                                     U Equipment: EVM; 0-l0-inA milliammeter
                                                                     U Resistors: Two 3300-, two 8200-, two 47,000-fl -W; two
SUMMARY                                                                100-fl l-W (NOTE: If a dual supply is not available, an
                                                                       additional 220-fl l-W resistor will be required.)
I . A flip-flop is a driven bistable multivibrator which
                                                                     ■ Semiconductors: Two 2N6005 transistors and two I N5625
    remains in one of two stable states until acted on by an
                                                                       diodes or equivalents
    external pulse. it is not a free-running or self-excited
                                                                     ■ Miscellaneous: SPST switch
    multivibrator.
2. The circuit of the collector-coupled flip-flop in Fig. 4지
    이osely resembles 댜ie circuit of the collector-coupled free-
    running multivibrator in Fig. 41-I . except that the flip-
    flop is direct-coupled and the free-running multivibrator
    is RC-coupled.
3. A negative pulse applied to me base of the on transistor
    changes the state of conduction of the two transistors: that
    is, it will flip the flip-flop.
4. There are large voltage changes at the collectors of me
    tW0 transistors ，판ien the flip-flop is flipped. For exam이C.
    ，따'en 口I IS ON Its collector is practically ai ground (0)
    potential. When cㅎ is OFF its collector rises to + Vc. C.
    These voltage changes 미＄《） appear, in reverse, at me
    C이lector of Q_ . It is these large voltage changes coupled
    from collector of one to the base of the other transistor that
    cause the mp小op to 拓p Therefore this type of circuit is
    called a t'o/tage-mode lr:,i1'er.
5. Flip- flop circuits find rnan\ ipplicaions in digital corn-
    puters. They ma act a, iniermcdiatc storage circuits, or
     they may be used a. logic indicators during an operation.             Fig. 42-3. Single power-supply voltage divider b.r 什p.敞'p


                                                                     226

===== PAGE 242 =====
PROCEDURE 肛－                   多冬4蜘唯졌慰戶，
                                       ---，驪뜅多볍∼＋                                              「｀겨n
                                                                                               4  ＇탤n．
                                                                                                     步啼蜘묘” －楓ij4*rrㅛ




                    LEFt 듸DE                                                                            mGItㅜ 듸DE
                     OUTPUT                                                                              OUTPUT




                                             Fig. 42-4. Experimental voltage-mode flip-flop.


1. Connect the circuit of Fig. 42-4. Power on.                         ，나tile mpplng me trigger. Does the trigger exhibit histable
                                                                       characteristics?
NOTE: If a dual supply is not available, connect the voltage
mvider of Fig. 42-3. Set me output 1ev이 of the dc supply at            6. When you have determined that the 拓p-flop is operating
21 V The negative terminal of the dc supply must not be line-             properly, fill in Table 42-2 for the conditions shown.
grounded. to eliminate 巾e possibility of con用cting grounds                Measure and record the dc output voltages.
when using other instruments in the circuit.                           7. The "signal" output level should vary between 0 (up) and
                                                                          - 5 V (down). From 艸ur preceding measurements you
2. With an EVM measure the dc voltages at the collector and
                                                                          will note that the down level is no longer - 5 V due to me
   base of 의 and c2. Record them in Table 42- I . indicate
                                                                          cross-coupling, which forms a voltage divider between
   which transistor, if any, is ON. which OFF. This is trial I.
                                                                          -5 and + II V. The output sign키 down level can be
3. Power oft. After about 1 mmn turn power on again. With
                                                                          "restored" by making the modifications in Fig. 42-5.
   an EVM measure and record for trial 2 the dc voltages at
   the base and collector of Q1 and Q2. indicate also which
   transistor is ON. which OI-'F.                                       TABLE 42-2. Flip-Flop Output Level
   Repeat step 3 for trials 3 and 4.
                                                                              Condition           Rj. ht Output        Left Output
4.
   To flip your flip-flop from one state to the other. alternat이y
   ground one transistor base and men the other.                               口ION
N(yrE: Grounding the base of the ON transistor causes the
                                                                                Q, ON
flip-flop to flip. Observe the voltage at one of the outputs


 TABLE 42-1. Transistor Flip-Flop Turn-On Slate
                                                                       DC. V                               가o,is,su'r G7ndjtion
          刀jot                 77" '" ＇ㅍ0r                 8t』
                                                             ｀e                 (:r(J//r
                                                                                       （·rOr              On                Off

           -                      q
                                  c그
           2                      《기
                                   口그

           1                      口
                                   口그
           4                       q
     --
                                   e그

                                                                      227

===== PAGE 243 =====
                                                                                                                     mT〔 REM시NㄸR
                                                                                                                     아 1R1히；E므
                                                                                                                     `^HE ^5 1N
                                                                                                                     FIG 42*'




                                                                    .`



                                                                                 Fig. 424. Flip-flop modification.
                                               -10 V
  Fig. 42.5. Voltage divider 幻rnegative supply m develop -5 V.


   Returning the collector resistor to a - 10-V source causes
                                                                   TABLE 42-3. Clamped Flip-Flop Output
   the output down level to fall below - 5 V The purpose of
   the diode connected between each output and the -5V
   source is to "clamp" the down level of the output to -5 V.
8. If you are using a dual voltage supply, connect a voltage
   divider across 小e -.10八／ source, as in Fig. 42-5. The
    - 5-V tap will be used in Fig. 42-6.
      If you are using a single voltage source, the divider of
   Fig. 423 비ready has a -5-V tap.
      When you have modified your flip-flop to conform with
   Fig. 42-6. check again me output levels and record mem
   in Table 42-3.



QUESTIONS                                                             me on transistor. Indicate polarity of voltage. Show your
                                                                      C이ㄲputations.
I. From your first four trials, steps 2 through 4, does it
                                                                   5. How does the computed value, in answer to question 4,
   appear mat me same transistor will always be an ON
                                                                      compare with the measured value? Explain any
   transistor when power is first applied in the circuit of Fig.
   42-4? Why?                                                         discrepancy.
                                                                   6. How do diodes ／기 and D2 "clamp" the down level at
2. What effect does grounding the base of the oFF transistor
                                                                      -5 V?
   have on flip-flop operation? Why?
3. What effect does grounding the base of the ON transistor
                                                                   Answers to $ Il-Test
   have on flip-flop operation? Why?
4. Assume that the ON transistor is saturated and that the         I. q; Q2            4. 0
   collector voltage is 0 measured with reference to the           2. false            5. + l0
   emitter. Compute the base voltage which would appear at         3. negative




                                                            228

===== PAGE 244 =====
                                                            -EXPERIMENT
                                                            THE ONE-SHOT(MONOSTABLE)
                                                                     MULTMBRATOR AND
                                                                      SCHMITT TRIGGER


OBJECTIVES                                                           Q.,. the base of（기 is therefore at ground potential. Note that
                                                                     the emitter of Q. is at ground. Hence, no forward bias exists
]. To dertermine experimentally the operating characteris-
                                                                     in the base emitter of《기. and Q1 is cut off. Therefore the
   tics of a monostable multivibrator
                                                                     V이tage at the collector of Q1 15 + Vc(.. the positive collector
2. To determine experimentally the operating characteristics
                                                                     source. 가is represents the stable state of the circuit: q cut
   of a 8아imitt tngger
                                                                     off and 口그conducting at saturation level.
                                                                         A positive pulse of sufficient amplitude to start current in
                                                                     Q1 is now applied to the base of Q1. Current flows in Q1, and
INTRODUCTORY INFORMATION.---------
                                                                     山e collector voltage drops. This negative change is coupled
                                                                     byC1 to the base of口2' reducing current in c2. 作e collector
One-Shot Multivibrator
                                                                      voltage of口그therefore rises, driving the base of q positive.
The one-shot mulcivibrator circuit is driven, not free-run-          More current flows in Q1, driving the collector of Q1 more
fling. Unlike the bistable trigger in Experiment 42, the mono-       negative, therefore driving the base of Q., more negative. In
stable multivibrator has one stable state to which it returns        short order. th궁regenerative action cuts off 口2. leaving c1
after an external driving pulse has caused it to execute its         conducting very heavily. The resulting change in voltage at
cycle. The one-shot multivibrator is often used to widen a           the collector of Q1. from + V' toO (approx). causes capaci-
pulse or d이ay its trailing edge.                                     tor q to discharge through 시. At the start of the discharge
    Figure 43- la shows two transistors, resistors, and a capac-     cycle, the full voltage change at the collector of이 appears as
nor connected to operate as a one-shot. c1 is connected                - Vrc at the base of Q2. As C1 continues to discharge toward
between the collector of 口1and the base input of Q,, R1 is             + Vcc (the positive voltage source to which 시 is returned),
added, and the collector of c2 is connected to the base input         the voltage at the base of .
                                                                                                 口，  rises exponentially (see wave-
of Q .                                                                form 'g2), The discharge path for C1 is shown in Fig. 43-2a.
    Study of Fig. 43-la suggests that since the Q캬）  ase-emitter         When the base of 口2 has risen above 0 V and is slightly
circuit is forward-biased (by R'). 02 will be saturated and the      positive, c2 starts conducting again. The voltage at the
collector of Q., will therefore be at, or close to, ground           collector of 口2drops, driving the base of q in a negative
potential. Since the base of Q1 is returned to the collector of       direction. Collector current through Q1 decreases, causing


                  s,
                                                                                                                              卜니
  ｀뇨 三三－ + 3万 v




                                                rα7                                                              새나

                                   Fig. 43-1. (a) Monostabie (one-shot) multivibrator: (b) waveforms

                                                                   229

===== PAGE 245 =====
                                                           수 V口




                                            ra)                                          (b)


                                            디g. 43-2. (a) Discharge; (b) charge path for C1.


the voltage at the c이lector of cL to go toward +vcc.                      In the absence of an input to Q1, the divider network R3,
Capacitor q therefore starts charging. Its charge path (see            R2, together with the collector resistor in Q1, maintains the
Fig. 43-2b) is through the emitter-base resistance of c2'              base of 口2 slightly positive relative to the emitter, and 口2
mrough R82 and mrough Rc1, toward +Vcc. The action                     operates in the saturation region. The positive v이tage devel-
rapidly turns c2 on and turns 口1off. c2 remains ON until a             이：沈 across the common-emitter resistor R4 resulting from
positive pulse causes 小e one-shot multivibrator to execute its         current flow in Q2 maintains NPN transistor Q1 cut off
cycle again.                                                           because the base of이 is at ground potential. hence negative,
   Of interest are the waveforms VB, at the base of Q2 and v.2         慟alive to its emitter (therefore reverse-biased). The stable
at the collector. Note that the positive pulse at the collector of     state in the absence of a signal, then, is 口2 ON and c1OFF.
c2 in the inter 'al t0 - ＇】 represents the time during which              When a sine wave is applied to the input circuit, cI is
Q., is cut off.                                                        turned on during the positive alternation 咐ien the base of 口1
   The positive pulse necessary to start 什ie mgger action can          is driven more positive than me positive voltage on 小e
be obtained by differentiating a square wave 1,y the circuit of        emitter, point P1 in Fig. 43-4b. Q` is driven to conduction in
Fig. 43-3.                                                             me saturation region ani is held there as long as me Input
                                                                       voltage at the base is more positive than the emitter voltage.
Schmitt Trigger                                                        Q2 is turned off. At 尸2' the voltage at the base of 이 drops
                                                                       below the emitter voltage and switching occurs, with 口2
Figure 43-4a shows an emitter-coupled binary, also called a
                                                                       being turned on and 口1 turned off.
Sch,nm trigger after its inventor. Note how the preceding
                                                                          The reason that 口2 turns off when c1goes on is that with
circuit was modified to make a trigger whose characteristics
                                                                       c1ON and saturated the collector of 口l drops to a low
are completely different from the one-shot.
                                                                       potential. 가le network R2. R3 couples this low Q1 c헤ector
   The Schmitt trigger is a binary trigger because two stable
                                                                        voltage to the base of 口2 and eliminates the forward bias on
states occur. 01may be ON and Q2 on:, or 口2 may be ON and
                                                                       c2. Therefore o2 goes off.
口1OFF.
                                                                         Figure 43-4b shows the input and output waveforms.
   Note that Hg. 43-4a differs from a collector-coupled bi-
                                                                       Between the points /\ and ／질 on the positive alternation of
nary trigger in that the usual trigger network coupling the
                                                                       the input sine wave, Q2 is cut off, and its collector is therefore
collector of Q2 to the base of Q1 is replaced by common-
                                                                       at + Vcr. Between ／느 and /b, c2is oN. and its collector
emitter coupling across R4. The switching action may be
                                                                       voltage drops close to 小C emittcr v이tage. The output wave
started by raising or lowering the bias on Q1.
                                                                       looks square (or rectang미ar). Hence the Schmitt trigger is
                                                                       called a squaring circuit.
             0.022 JJF       S2

                                                                       SUMMARY

                                                                           I. A one-shot multivibrator is monostable; that is. it has one
                                  JtL_ ,,,,,J.,,,, FIG.
                                                   TO INPUT
                                                        45-1
                                                             OF               stable slate. The one-shot remains in this stale until an
                                        V                                     external driving pulse causes it to execute its cycle, after
                                                                              which it returns to its original state. The one-shot is
                                                                              merefore a driven, nor a free-running, multi`ibrator.
                                                                           2. In the monostable MV in Fig. 43-I , 口2 is the normally o:l
                                                                              transistor. Q1 the normally off.
FIg. 43-3. The capac漱y and resistor differentiate I he square wave         3. An external positive driving pulse applied to me base of
Only the positive p이se triggers me one-탉刪 mullivubrator.                      口I turns q o！니 and Q2 OFF. The length of time that .  口，  is


                                                                     230

===== PAGE 246 =====
                  $1
  VC( 三三－ 346 V
                                                   '      (-        -




                                                         c1
                                                       .m2 'F
                                                               :        0,
                                                               J+
                                                                        2N6004
                                                                                              A3101,O

                                                                                                                        rbJ


                                             (a)


                    Fig. 43-4. (a) Schmitt tngger produces a square-wave Output故,m a sine-wave input; (b) wavetorms.

   0FF is determined by the 山ne constant (1凡 . The longer                     coupled by                  and                 to 小e
   the time constant. me wider 小e pulse developed at 山e                       base of c2.
   collector of o2 (see Fig. 43-1町 The discharge of C1                     6. In Fig. 43-Ia, 小e widm of the pulse developed at 小e
   through 凡 maintains the base of Q2 negative during the                     collector of c2 is determined by the time constant
   pulse intervaL
4. The one-shot multivibrator is often used to delay the                   7. In the Schmitt trigger (Fig. 43-4a), in the absence of an
   trailing edge of a pulse or to widen a pulse. In digital                   input signal, the base ofc2 is                   (positive.
   circuits it may be used as a no-bounce switch to enter a                   negative) relat.ive to its emitter.
   binary I into an adder.                                                 8. In Fig. 43-4a, e1is normally                     (oFF. ON)
5. The Schmitt trigger (Fig. 43-4a) is an emitter-coupled                     in the abseii=e of an input signal.
   binary circuit which converts a sine-wave input into a                  9. In Fig. 434α，when 小e input sign키 is of sufficient
   rectangular wave. It is merefore called a squaring circuit.                amplitude to switch the conduction of Qland c,, the
                                                                              collector of c2 nses to
                                                                          10. K the amplitude of the input sine wave is increased, but
SELF-TEST
                                                                              its frequency is the same, the width of the output pulse
Check your understanding by answering mese questions.                         (Fig. 43-4a) is                     (increased, decreased,
                                                                               unaffected).
 I. In Fig. 43-la, what keeps 口그ON in the absence of an
    input driving pulse is the forward bias provided 口그
    by                 and
                                                                          MATERIALS REQUIRED
 2. In Fig. 43-la, ，나1en c2 i5 0N, cI is
 3. A                 (positive, negative) pulse on the base              ■ Power supply: Variable regulated low-v이tage dc
    of Q1 (Fig. 43-la) will switch the conduction of Q1                   ■ Equipment: Oscilloscope: EVM; AF sine/square-wave
    and Q2.                                                                 generator (with ext. sync output jack, if possible)
 4. In Fig. 43-Ia, when q is Ottr. its collector voltage                  ■Resistors: 150-. two 820-. three 1000-. 10,000-, 22,000-f
    is                  When Q1 is turned on, it saturates                  比-W
    and its collector voltage drops to                     V              ■Capacitors: Two 0.022-, 100-FLF 50-V
    (approx).                                                             ■ Semiconductors: Two 2N6004 transistors (other ch이cc:
 5. In Rg. 43-la. 出c negative change in v이tage which                        2N3904); 1N5625 diode; or equivalent
     occurs at the c이lector of 口］ when QI is turned on is                 ■ Miscellaneous: Two SPST switches


PROCEDURE

One-Shot Multivibrator
                                                                              2. Externally trigger/sync yo ir oscilloscope with signal at
 1. Connect the circuits in Figs. 好Ia and 43-3. connecting                       the sync output jack on the generator, or with its square.
    ^ boA andBioB. 옥 ㄺm q are open. Set vcc at + 3.6 V.                          wave OUtDUt.
    Set square-wave generator at 500 Hz, output at 5 V p-p.                   3. With your oscilloscope, observe the square wave at tne

                                                                        231

===== PAGE 247 =====
TABLE 43.1. M아ostable Muftivibrator Characteristics


          Step                     7논引 Point                       Waveform                          V p-p                 PulseWidth
                                                          '                                 1
            3                     Generator
                                   01쨔가i'                 T
                                                          -
                                                                                            ㅣ
                                                                                                       5                                 x

                                                                                            '
                                                          -                        ㅣ        -
            4                      Across R2              1                                 -                                            x
                                                          I                         I       I
                                                          [        "                ·       `
                                                          1        I      I         1       1

            5                      Collector              I        I      I        ㅣ I
                                                          I        I      I        1 1                                                   x
                                    of Q2
                                                          I        I      I        I ㅣ
                                                           ~       1      1         1       L
                                                          '        1      l         r       1

                                                          I        -      I         I       ㅣ
            6                     Base of 02              I        I      I         I       I                                            x
                                                          1        I      l         I       I
                                                          1        1      1         1       I
                                                          '        I      T         `       1


            7                      Collector              -        -      1        - ㅣ
                                                          I        I      I        I I
                                    of Q2                 I        I      I        ㅣ l
                                                          I               L         I       I

                                                          I        I      I         I       I
            9                      Collector
                                                          1        I      I         I       I
                                     ofc2                 I        I      I         I       ㅣ
                                                          1        1      f         1       I
           10                      Collector
                                                                          x
                                     ofQ2



    output of the generator and set the oscilloscope controls                 NOTE: If there is a spike riding at me leading edge of the
    for two waveforms, properly centered, as in Table 43-I.                   output pulse. gradua따 reduce the output of the generator
 4. Swit比S2 is still open. 아iserve the waveform acrossR,.                     until me spike msappears.
    the 1000-fl input resistor. In 丘비e 43-I draw this wave
                                                                                  8. Power off. Substitute a 10,000-fl resistor for R1.
    in time 丙ase with the input square wave. Measure and
                                                                                  9. Power on. Observe and measure the am하itude and
    record the peak-to-peak amplitude of the waveform.
                                                                                     pulse widm of the output waveform at the collector of
 5. Close 옥 . applying power to the circuit. S2 is still open.
                                                                                     Q2. Draw the waveform in proper phase with the input.
    Observe the waveform, if any. at the collector of Q2 and
                                                                                     Record its amplitude and pulse width.
    record in Table 43-1.
 6. Close S2. Both switches are now closed. Observe, mea-                     NOTE: If you do not have an oscilloscope with a calibrated
    sure, and record the waveform at the base of Q2. in                       time base, measure the pulse width in centimeters or inches.
    proper phase with me input.
                                                                              10. Reduce me frequency of the square-wave generator to
 7. Observe, measure, and record the output waveform at
                                                                                  350 Hz. Measure and record the width of the positive
    the collector of c2' in proper phase with the input.
                                                                                  output p미Se. Has me pulse widm changed from mat in
    Measure and record the width of the positive pulse.
                                                                                  step 9? ，싸tat has manged?


TABLE 43-2. Characteristics of a Schmitt Trigger

                                                                                                                                        Puls,
           Step                    7es! 尸oinl                          Wat'eform                     V p-p                                  tdiWe
                                                                                                                                             h

            口


            14
                                   cenerator
                                    Output

                                    C'川ector
                                                      아J\J
                                                      '

                                                      l
                                                      I
                                                               '

                                                               I         -
                                                                         I
                                                                          1             '

                                                                                        I
                                                                                        I
                                                                                                1

                                                                                                I
                                                                                                -
                                                                                                       K)                                 x



                                      of Q,           l        -         ㅣ              1       l
                                                      1                   i             l       1


            ＇빅                      C이lector          ㅣ        ㅣ              i         1       ;
                                                      1                       -         1
                                     of Q,            ㅣ                                 1       `




                                                                   232

===== PAGE 248 =====
Schmitt Trigger                                                       tr이｀for two waveforms, properly centered as in Table
                                                                      43-2.
11. Connect the circuit of Fig. 43-4a. Vc is set at + 3.6 V.      14. Observe the output waveform (c이lector of Q2). Measure
    Close 옥，   applying power to the circuit. Set the sine-           and record in Table 43-2, in proper phase w油 the input,
    wave generator frequency at 1000 Hz, output at 10 V p-p.          its peak-to-peak amplitude and the width of the positive
12. Externa따 trigger/sync the oscilloscope as in step 2.              pulse.
13. With your oscilloscope observe me sine wave at me             15. Reduce me sine-wave generator output to 4 V p-p and
    output of the generator and adjust the oscilloscope con-          repeat step 14.




QUESTIONS                                                         6. IntheSdㄱLmitt trigger, what effect does me amplitude of
                                                                     me input sine wave have on the width of the positive
I. Why is the waveform across ／乙．, step 4, Table 43-I. no
                                                                     alternation at the collector of Q2in Fig. 43-4a? Why?
   longer a square wave?
                                                                  7 ，싸iat effect does me frequency of the input sine wave
2. In which step of the procedure did you determine that the
                                                                     have on 小e width of the positive 키ternation at mcc이lee-
   circuit of Fig. 43- I is not a free-running multivibrator?
                                                                      tor of Q2 (Fig. 43-4a)? Why?
   Refer specifically to the data in Table 4꾀 ，나tich confirm
   y)ur answer.
3. In the one-shot multivibrator. which time constant yielded
   a wider pulse: 0.022 .F x 10,000 fl or 0.022 1iF
                                                                  Answers to Self-Test
     x 22.000 fl? Why?
4. What is me「이ations川：》 between 巾e waveform on 小e                I . RBI: R1             6. C1 x R1
   base of Q2 and the width of the pulse at the collector of Q,   2. oFF                  7. positive
    in Fig. 43- la? Why?                                          3. positive             8. OFF
5.（α）In Fig. 43- la. what turns 口2off' (b) Why doesn"t it         4. +V.c; 0              9. +vcc
   remain off all the time?                                       5. C1; R1              K). increased




                                                                  233

===== PAGE 249 =====

===== PAGE 250 =====
                                                                                                      "        EXPERIMENT
                                                                   MIXERS, MODULATORS, AND
                                                                             DEMODULATORS




                                                                                                            ㅢㅢ거
                                                                                                                       +H
OBJECTIVES
l . To observe the difference frequency out of a mixer                                                         FILTER               ,ㄷ7
2. To amplitude-modulate a carrier using a bip이ar
    modulator                                                                                                  , 21
3. To demodulate an AM signal                                                                                  FILTER               2!
                                                                                         NONLINEAR
                                                                                          CIRCUIT
                                                                                                                    `/
                                                                                                                    y
INTRODUCTORY INFORMATION-                                          d커
                                                                                                               F 1ILTER
                                                                                                                   ㄴㅜE

Nonlinear Distortion
Rgure 44-I shows the iransconductance curve of a bip이ar
transistor. This graph of collector current versus base-emitter
                                                                                                          L       n/
                                                                                                               디 LTER              wwv
voltage is nonlinear. Notice how a sinusoidal VBE voltage
produces a nonsinusoidal collector current. In other words.             ng. 44-2. Nonlinear distortion produces harmonics whi햐r can be
                                                                        m이ed.
me 갉tape of the output current is no longer a true duplication
of댜te input 計tape. Since me collector current flows through a
load resistance, me output voltage will also have nonlinear             linear circuit is a distorted sine wave, which contains bar-
distortion.                                                             monics. A bank of filters can separate each harmonic from
   Nonlinear distortion produces harmonics (multiples of the            the others to get frequencies off 2f 3f . . . , nf As you see.
input frequency). For instance, if the base-emitter voltage is a        nonlinear distortion creates new sinusoidal signals.
pure sine wave with a frequency of I kHz, then the c이lector
current in Fig. 44-1 is a distorted sine wave with afundamen.           Mixer
to! (lowest) frequency of I kHz and harmonic frequencies of
                                                                        A mixer is a nonlinear circuit with two input signals and one
2 kHz, 3 kHz, 4 kHz. . . . .and so on. In general. iff is the
                                                                        output signal. The output signal is a distorted combination of
 fundamental frequency. the output contains frequencies off
                                                                        the two input signals. In Fig. 44-3, the input signals have
극f 3f . . . , 4f
                                                                        frequencies off andf,. Because of the nonlinear distortion,
    Figure 44-2 illustrates the idea behind harmonics. A pure
                                                                        the output signal contains the original input frequencies, plus
 sine wave drives a nonlinear circuit. The output of the non-
                                                                        meir harmonics. For instance, if me two input frequencies
                                                                        are 100 and 101 kHz, the output signal contains these fre-
                                                                        quencies: 100 kHz, 101 kHz, 200 kHz, 202 kHz. 300 kHz,
                                                                        303 kHz. . . . .and so on.
                                                                           A detailed mathematical analysis reveals a startling prop-




           ／뇨
                                                                        city of a mixer. In addition to the harmonics that are pro-
                                                                        duced, newfrequencies appear in the output that are equal to



                                                                                                                            '1




                                                                                                                          ＇ 〃 /J
                                                                                                    MIXER

                                                                                    I,                                    /`




                                                                        디g. 44.3』 A mixer produces the original frequencies. the sum, and
         ng. 4ㅅJ Transconductarice curve of ttans｀針《》
                                                   「                    th. 轍＇te1꾀ce

                                                               235

===== PAGE 251 =====
                  MIXER             FILTER                                                                                V。
                                                                                                                           ..,


                                                                                                                                 rjV\J
                                                                                                                                 f    -   a.,



디g. 44-4. Mixer output is tittered to get difference frequency only


the sum and difference of the two input frequencies. 1ff and
f. are the input frequencies, the new frequencies are
                        Sum = f      + /1                   (4-I)

                        Diff = /, - .r.                      (44-2)

As an exan 미e, if the two input frcquencies are 100 and 101
난1z. 小e output of a mixer like FIg. -14-3 contains 100 and
101 kHz, their harmonics, and ness frequencies given by                                   FIg. 44-5, Bipolar mixer.

         Sum = 101 kHz -4- 100 kHz = 201 kHz
                                                                       AM waveform of Fig. 44-7b; the amplitude of the high-
         Diff = 101 kHz - 100 kHz = 1 kHz
                                                                       frequency signal is varying at a low-frequency rate.
  Usually, the output of a mixer is filtered as shown in Fig.             The high-frequency signal is called the cart'ier, and the
的4 to allow only the difference frequency to rcad나he fin川              low-frequency signal is the mc汕slating signal. Hundreds of
output. For instance. iffy = 1455 kHz andf = 1000 kHr,                 carrier cycles normally occur during one c，   이e of the modu-
then on!s the 巾fference frequency                                      lating signal. For this reason, an AM waveform on an oscillo-
                                                                       scope looks like the signal of Fig.44-7c沚ue positive peaks of
         Diff = 1455 kHz - 1000 kHz = 455 kHz
                                                                       the carrier are so 이osely spaced they form a solid upper
reaches the final output of Fig. 4午4                                   boundary known as the upper envelope; similarly, the nega-
   Figure 44-5 is an exam히e of a transistor mixer. One signal          tive peaks form the lower envelope.
dr汁es the base; the other drives the emitter. One of the input            Figure 44-8 is an example of a transistor modulator. The
signals is large; 口＂` is necessary to ensure nonlinear opera-          carrier signal yr is the input to a common-emitter amplifier.
tion. The other input signal is usually small. One of the               The circuit amplifies the carrier by a factor of A, so that the
reasons this signal is small is because it often is a weak signal       output us Av . 가ae modulating signal is part of the biasing;
coming from an antenna.                                                 therefore, it produces low-frequency vanations in emitter
   가1e C이lector tank circuit is usually tuned to 山e difference          current. As shown elsewhere. 山e voltage gain is proportional
frequency. Because of mis. me two original frequencies.                 to emitter current. For this reason, the amplified carrier
their harmonics, and me sum frequency are filtered out of               signal looks like the AM waveform shown; the peaks of the
the output. Only the mfference frequency reaches the final              output signal vary sinusoidally with the modulating signal.
output.                                                                 Stated another way, me upper and lower envelopes have me
    Field-effect transistors (FETs) are also used in mixers.            shape of the modulating signal.
티gure 44-6o shows a junction field-effect transistor (JFET)
 mixer, and Fig. 44-6b is a dual-gate MOSFET mixer. In each            Percent Modulation
 drcu比 the output tank circuit is tuned to the difference
                                                                       In Fig. 44-9a, the AM waveform has a maximum peak-to-
 frequency. This suppresses me two original frequencies,
                                                                       peak value of 2V。 ,. , and a minimum peak-to-peak value of
 mcit harmonics, and me sum frequency. so 山at only the
                                                                       2Vm.n. The modulation coefficient is given by
 difference frequency appears at me final output.
                                                                                                    ㄳ／ma, - 2 V, ,r
                                                                                            '71 =                                    (44-3)
 Amplitude Modulation                                                                               2Vmㅄ + 2V, ,,
 Radio, television, and many other electronic systems would             and the percent modulation b
 be impossible without modulation: it refers to a low-fre-
                                                                                     Percent modulation = m X l00%                   (44-4)
 quency signal contr에ing the am이itude, frequency, or phase
 of a high-frequency signal. When the low-frequency signal               For instance, suppose we see an AM waveform m:e F唯
 contr이5the amplitude of the high-frequency signal. we get             44-9h on an oscilloscope. This waveform has
 amplitude modulation (AM)
                                                                                                    i6 - 4 = na.
    티gure44-7a shows a simple modulator. 사ugh-frequency                                     '7i =
                                                                                                    16+ 4    V∼
 signal v, is the input to a potentiometer: therefore, the am비b
 tude of the output sign비 depends on the position of the wiper.         and
 If we move the wiper up and down sinusoidally. we get the                               Percent modulation = ＆〕％


                                                                      236

===== PAGE 252 =====
                                               +
                                                   V00                                                          +voo




                                                         Fig. 44-6. (aJ JFET mixer; (bJ MOSFET mixer.




                                                                                     Side Frequencies
                                                                                     A modulator like Fig. 44-8 is a nonlinear circuit. Because of
                                                    빼                  ll∥
                                                                                     this, we get sum and difference frequencies, similar to a
  "   IllhlIlilIlfihlUlIll그   ,;01
                                                                                     mixer. As an example. suppose the modulating frequency is
                                                                                     I kHz and the carrier is I MHz. Then.
                  (a)
                                                              )b)
                                                                                                         Sum = 1.001 MHz
                                          UPPER ENVELOPE                                                 Diff = 999 kHz
                                                                                 ne new frequencies are called sidefrequencies. 가1e sum is
                                                                                 me upper side frequency, and the difference is th이ower side
                                                                                 frequency.
                                                                                    Like a mixer, a modulator produces the two original fre-
                  LOWER ENVELOPE                                                 quencies. me sum, and the difference frequency. Unlike a
                                          棺)                                     mixer, however, the final output of Fig. 44-8 contains the
                                                                                 carrier and the two side frequencies.
Fig. 44-7. (a) Potentiometer can proouce AM; (b) AM signal; (c) AM
envelopes.



                                                                             + vcc




                                     /.
                                                             ng. 44-8. Bipolar amplitude modulator.

                                                                                     237

===== PAGE 253 =====
                                                                      envelope to foliov. Occurs at β in Fig. 44- l0b: at this point,
                                                                      the en.ckipe is decreasing at its fastest ra【e. With advanced
                                                                      mathematics, we can derive this formula for the cutoff fre-
                                                                      quency 0nhe envelope detector:

                                                                                                                              (44-t)
                                                                                                    =
                                                                                           ／→m
                                                                                                            'rrRCni
                                                                                                        2
                                                                      where '" is the modulation coefficient. If the envelope
                                                                      frequency is greater than 八∼）      , the detected output drops
             躇）                                   (b)                 20 dR/decade.
                    n9. 44·9. AM signals                                 By adding a low-pass filter to the output .nhe Fig. 47-I0a,
                                                                      we can remove the small RF rip미e that remains on the
                                                                      detected signal (Fig. 44-l0b).
Radio Frequencies

For an antenna `(, be efti . tent. its minimum lcnttth should be
                                                                      SUMMARY
                        t - 75n0b
                                                         (44-5)         l. The I- versus VBE graph of a bipolar transistor is
                              r
                                                                           nonlinear.
咐tere length I. is in meters and frequency / in hertt. "                2. A sinusoidal VBF signal produces a nonsinusoidal c이‘
an antenna is shorter than mis. it ，〃m not radiate sienals                 lector current. 가ie（十arige in sign비 shape is C키led
efficiently.                                                               ,tonlinear dbfortiOfl.
   Antennas would be immense at audio frequencies (20 to                3. Nonlinear distortion produces hormonicsf 2j 3f . . . .
20,000 Hz). For instance, to radiate 100() Hz efhciently. we
                                                                           nf
would need an antenna leng댜 ＇of                                         4. A mixer is a nonlinear circuit with two input signals. The
   .   7.5 ' (0'           . .              .                              output of the mixer contains the original frequencies.
                 " = 7.5 x l0' meters (m) = 47 mi                           their harmonics, the sum frequency, and the difference
   L = ' ."1 000
                                                                            frequency
This is mu야，too loni . For this reason, it is impractical to            5. Usually. the mixer output is filtered so that 이ㅟy the
transmit audio frequencies directly into space hstead, corn-                difference frequency reaches me fin비 output.
munication systems transmit radio frequencies (RF); these               6. One of the mixer input signals must be large enou얏，to
are frequencies greater than 20 k거z. With RF signals. rea-                  produce nonlinear distortion. The other signal. typically
sonable antenna lengths are possible                                        from an antenna, is small.
                                                                        7. Modulation refers to a low-frequency signal contr애ing
Envelope Detector                                                           the amplitude, frequency. or phase of a high-frequency
AM broadcast signals use carrier frequencies between 540                    signal,
and 1600 kHz. In the studio an audio signal modulates the               8. 가ie high-frequency signal is called the carrier, and the
carrier to produce an AM signal. A iransrnitting antenna of                 low-frequency signal is the modulating signal.
suitable length then radiates this AM signal into space Miles           9. To produce an AM signal the modulating signal contr이S
away. a receiving antenna picks up the modulated RF signal.                  the gain of an RF amplifier.
After being amplified, this signal is demodulatenme audio              10. An AM signal contains a carrier and two side frequen-
is recovered).                                                              cies. 재e upper side frequency equals the sum of mC
   티gure44-loa 나iows one type of demodulator. Basically, it                  earner and modulating frequencies; the lower side fre-
is a peak detector (Experiment 34). Ideally, the peaks of the               quency equals 山e difference.
input signal are detected to recover me upper envelope For             II . After an AM signal is received, it is amplified and
나its reason. 出e circuit is called an envelope detector.                      demodulated.
    During each earner cycle. t e 이ode turns on briefly and            12. One way to demodulate an AM signal is with an ens'e-
比arges me capacitor to the peak voltage of me particular                     lope detector.
carrier cycle. Between peaks, 나ie capacitor disdtarges
throu帥 the resistor. By making the RC time constant much
greater than the period of the carrier, we get only a slight           SELF-TEST
discharge between cycles. In this way. most of the carrier
                                                                       Check your understanding by answering these questions.
 signal is removed. The output then looks like the upper
env비ope with a small ripple as shown in Fig. 44-l0b.                   l . If a sine wave wima frequency of 5 kHz drives a nonlinear
    Bu다iere is a crucial idea. Between points A and c m Fig                circuit. ＼나tat are 山e frequencies appearing tn me output?
 44- 10b, ead` carner peak is smaller than me preceding one            2. A mixer has these input frequenctes: / , = 32 MHz and
 If the RC time constant is too long. me circuit cannot detect             /. = 28 N州z. What do the sum and difference frequen-
 the next carrier peak (see Fig. ‘뀌- I 0c. The hardest part of the         cies equal7

                                                                     238

===== PAGE 254 =====
                                                         〃
                                                                 c




                                                                                                                     （키

                              '"        '




                                                                                                                                                TOO LONG A
                                                                        ( "                                                                     DISCHARGE
                                            aIIllIIll;
                                                              IIlIIIII

                                                                                   .,..,.01】


                                                                                               ·：：···．.....,
                                                                              8.
                                                                              c
                                                                                                               ~ r




                                            伯)                                                  (ci
                  Fig. 44-10. (a) Envelope detector; (b) envelope with small ca,r,er ripple: (c) envelope frequency 柏. high.


3. If the mixer output is filtered in question 2. what is the                                                             8. What is the minimum lengm for the transmitting antenna
   usu키 frequency at the output of the filter?                                                                               of a radio station whose frequency is 1080 kHz?
4. In an AM radio the weak signal to a mixer has a frequency                                                              9. An envelope detector has R = 10 kfl, c = m00 pF,
   between 540 and 1600 kHz. 재e strong signal comes                                                                          and m = 0.5. What does f1nu" equal?
   from a local oscillator (LO), a circuit inside the radio. The
   LU signal has n1igher frequency than the weak signal. If
   the 山fference frequency always equals 455 kHz, ，나lat is
                                                                                                                          MATERIALS REQUIRED
   the frequency of me local oscillator when the other fre-
   quency is 540 kHz? When it is 1600 kHz?                                                                                ■ Two power sup힌ies: IS-V
5.
   가1e                   sign비 of Fig. 44-8 varies the voltage                                                            ■ Equipment: Oscmoscope. two sign키 generators
   gain of the circuit. This varies the amplitude of the                                                                    (100 to 500 kHz). one audio generator
                                                                                                                          U Resistors: Two I-UI. one 4.7-kfl. four 10-kf1.
6.    An AM signal has a maximum peak-to-peak voltage of                                                                    one 22-kn, four 100-kn t -W
      10 V and a minimum peak-to-peak voltage of 0 V. What is                                                             U Capacitors: Three 0.0이-p.F. one 0.01- ㅗF. two 0. l- F
      the percent modulation?                                                                                             U Diode: lN9l
7.
      The modulating signal has a frequency between 20 Hz                                                                 U Transistors: Two 2N3904 (other choice: 2N6005)
      and 20 kHz. The carrier has a frequency of 1080 kHz.                                                                lOp amp: 741C
      What are me lower side frequencies for 20 Hz? For                                                                   U Speaker: 3.2-fl
      20 kHz?


PROCEDURE



     1. IfL = 101 kHz andf = 100 kHz in Fig. 44-ha, what                                                                   3. Connect the circuit of Fig. 44-I Ia.
        does dIC 小fference frequency equ비？ Record answer                                                                   4. Turn v, down to 0. With the oscilloscope, adjust v'.r t0
        here:                                                                                                                 0.1 V p-p. Set the frequeney to 101 kHz.
                    /;- /;     =                                                                                           5. Next adjust v. to I V p-p and 100 났仇
                                                                                                                           6. Look at the final output signal with a vertical sensitiv따
     2. The mixer output of Fig. 44-I Ia is filtered by two low-
                                                                                                                              of 0.1 V/cm (ac input) and a sweep time of 02 ms/cm.
        pass RC circuits. The approximate cutoff frequency of
                                                                                                                              Vary the frequency of the v, generator slowly in the
        each is given by
                                                                                                                              vicin心 of 101 나(z until 》｀iu get a I -kHz output signal.
                                                                                                                           7. Look at point B, me input to the final RC fitter. Notice the
                                                                                                                              ripple on the 나Ha sign펴*
                                             =

                                                         4 .ITflL.
                                                         근，        =;
                                   /,
                                                                                                                           8. Look at point A. the input to the first RC filter. Use a
        Calculatef. and record the answer here:
                                                                                                                              vertical seflsltlv따 of 2 V/cm. Notice how large the
                         ft   =                                                                                               ripple is here.

                                                                                                                      239

===== PAGE 255 =====
                        i-15 v

                                                                                                         +15 V

                                 A       1에kn   8    100 kn
                                                                                                                                그．2 n
                                                                                                                                5PEAKER

                                 ?N3여
                                         0.001"Fㅜ 0.001"FT
                                                －ㄴ            ＝」－




                                     佃                                                                          伯)
                                                 FIg. 44-11. (a) Mixer: (b) beat-note detector



Beat Note                                                                 20. Look at me output of me envelope detector. You should
                                                                              have art audio signal.
 9. Connect the filtered mixer output (Fig. 44- h la) to the
                                                                          21. Vary the frequency of 小e audio generator and notice
    input of the 이：) amp circuit (Fig. 44-I 沁） .
                                                                              what happens to 小e output of the envelope detector.
10. Vary the frequency of either ac generator and notice what
    happens to the beat note (difference frequency) out of
    巾e speaker.

                                                                                                                 +15 V
Amplitude Modulator

11. In Fig. 44-I2a, what are the side frequencies? Record
    your answers here:

         Upper side frequency =
         Lower side frequency =

12. Connect the circuit of Fig. 44-12a.
13. Set the audio generator to 200 Hz and the RF generator                  RF
                                                                            5凹 l나 z
    to 500 kHz.
14. Turn the audio generator down to 0 (do not disconnect).
    Mjust the RF generator to get a final output Vc,｀』＇of
    0.3 V p-p.
15. Use a sweep speed of 1 ms/cm. Turn up the audio signal
    and y)u will see amplitude modulation.
16. Increase and decrease the audio 1ev이 and notice how the
                                                                                                          (a)
    percent modulation 比anges.

Envelope Detector                                                                                +15 V



17. In Fig. 44-12b, work out me highest frequency the
    envelope detector can follow without attenuation for a
    modulation of lOG percent. Record it here:

                 人1m.   :'   =

18. Connect the output of the am이itude modulator (Fig.
    44-12a) to the circuit 이Fig. 44-12b.
19. Use the oscilloscope to look at the input to the envelope
    detector (across the lower I-kn resistor of Fig. 'q-l2b)                                            伯）
    Mjust the modulation to 100 percent.                                       Fig 4412. (a) Amplitude modulator: (b) envelope detector


                                                                      240

===== PAGE 256 =====
QUESTIONS                                                      8. Explain why the output of the envelope detector (Fig.
                                                                  44-12b) changed frequency when the audio frequency of
I What did you calculate for the approximate cutoff fre-
                                                                  F培． 44-12a was varied.
   quency in step 2?
2. In Fig. 44-1 la, why do you not see the original frequen-
                                                               Answers to Self-Test
   cies (100 and 101 kHz) at the output?
3. Explain why the beat note from the speaker of Fig.          1. 5kHz, 10kHz,              6. 100 percent
   44-I lb changed frequency when you varied one of me            15 kHz. . . .             7. 1.07998 and 1.08002
   generators.                                                    n(5 kHz)                     MHz for 20 Hz;
4. nme beat note out ofme speaker isO in Fig.44-I比，     what   2. 玖〕MHz; 4 MHz                 I.
                                                                                                （拓 and I .1 MHz
   can you say about the two input frequencies in Hg.          3. 4MHz                         for 20 kHz
   44d k2?                                                     4. 995 kHz; 2055 kHz         8. 69.4 meters
5. What were the side frequencies recorded in step 11?         5. modulating (or low        9. 31.8kHz
6. ，싸＾at is the frequency of the envelope in Fig. 44-12a?         frequency); carrier
7. What was the frequency recorded in step 17?                    (or high frequency)




                                                               241

===== PAGE 257 =====

===== PAGE 258 =====
                                                                                          . ∼－· :: ,           EXPERIMENT
                                                                                      PHASE-LOCKED LOOP


OBJECTIVES                                                           inputs are in phase. the dc output is 10 V. When the inputs are
                                                                     90' out of phase. the dc output is 7.5 V. ，싸ten me inputs
I. To adjust the center frequency of a 地ase-locked loop
                                                                     are 180' 0ut o댜thase. the dc output is 5 V. The key idea is the
2. To observe the lock range
                                                                     dc output decreases when 巾e phase angle increases.
3. To measure the maximum and minimum capture
   frequencies
4. To measure the dc voltage from the FM output                      VCO

                                                                     Experiment showed how .a 555 timer「could bet operated as
                                                                     a voltage-controlled oscillator (VCO) by ap이ying a dc volt-
INTRODUCTORY INFORMATION-
                                                                     age to the contr이 input. Recall the idea. When the dc v이tage
                                                                     in Fig. 45-2a increases. me frequency of me output signal
Phase Detector
                                                                     decreases. In other words, a dc v이tage controls the oscillator
Suppose we have a mixer with input frequencies of 50 Hz and          frequency. Typically. the frequency decreases linearly with
50k거1. 가ten the difference frequency is0, 咐iich represents           an increase in dc voltage (see Hg. 45-2b).
dc. In other words, a dc voltage comes out of a mixer ，나ten              Many other designs are possible for VCOs. For example.
the input frequencies are equal.                                     one approach uses an Lc oscillator with a varactor (voltage-
   A 帥ase detector is a mixer optimized for use with equal           1controlled capacitor). By , varying1the dc'voltage applied
input frequencies. It is called a 地ase detector (or 帥ase              to the varactor. we can change th티capacitance and control
comparator) because the amount of dc voltage depends on the            the resonant frequency.
phase angle 小 between 巾e input signals. As the phase angle               The important thing to remember about any VCO is this:
changes, so too does the dc voltage.                                  An input dc voltage contr이S me output frequency. In this
   듸gure 45dα mustrates me phase angle between two                   experiment, an increase in dc control voltage causes the VCO
sinusoidal signals. 'When these signals drive the 한tase detec-        frequency to decrease.
b0r of Fig. 45- lb. a dc voltage comes out. One type of 한｀ase
detector has a dc output voltage that vanes as shown in Fig.
                                                                     Phase-Locked Loop
45-Ic. When the 的ase angle 4, is 0. the dc voltage is
maximum. As the 的ase an미e increases from 0 to 180', the              Figure 45-3 !$ the block diagram of a 꺄a,ce-locked loop
dc voltage decreases to a minimum value. ，파ten 小 is 90', the         (PLL). An input signal with a frequency o나, is one of the
 dc output is the average of the maximum and minimum                 tnputs to a 야iase detector. 가te other input comes from a
 outputs.                                                            VCO. The output of the 地ase detector is filtered by a low-
   For example. suppose a phase detector has a maximum               pass filter 가*`` removes the origin비 frequencies, mcit har-
 output of 10 V and a minimum output of 5 V. When the two            monics. and the sum frequency. Only the mfference fre-

                                                                                                     ｀自
                                                                                                      （




                                                               PHASE
                                           히N(Jt + 0) -                  -           J,
                                                             DETECTOR
                                                                                v.
                                                                 ㅣ
                                                                 히N u八




               lat                                           沁                                                   （이
                      Fig. 45-1. (aJ F가，ase angle between ＄四nals: (b) phase detector: (c) output of phase detector

                                                                   243

===== PAGE 259 =====
                                                                                   乙


                                                            乙
                    V,   ,                vCo     -      Jijiji



                  FIg. 45-2. (a) DC input controls VCO output. (b) VCO frequency inversely proportional to dc input.

quency (dc voltage) comes out of the low-pass filter. This dc                  phase detector sends more dc voltage to the VCO and
voltage then contr이＄ me frequency of the VCO.                                  decreases its frequency to 49 난iz. In either case, 小e feed-
    This feedback system locks the VCO frequency on to the                     back automatically adjusts the phase angle to produce a dc
input frequency. When the system is working correctly, the                     voltage that locks the VCO frequency on to the input
VCO frequency equals /,. the same as the input signal.                         frequency.
Therefore, the 地ase detector has two inputs with equal                            The lock range BL is the range of frequencies the VCO
frequency; the phase angle between these inputs determines                     can produce, given by
the amount of dc output. Figure 45-3b shows the phasors for
the input signal and the VCO.                                                                      BL = fmll,i - fmin                 (4 5-1)
   If the input frequency changes. me VCO frequency will                       wheref．   乂 and/n111` are the maximum and minimum VCO
track it. For instance, if the input frequency /, increases                    frequencies. For example, if the VCO frequency can vary
slightly, its phasor rotates faster and the phase angle increases              from 40 to 60 kHz, the lock range equals
as shown in Fig. 45-3c·. This means less dc voltage will come
                                                                                          BL = 60 kHz - 40 kHz = 20 kHz
out of the 地ase detector. The lower dc voltage forces the
 VCO frequency to increase until it equals!,.                                  Once the PLL is locked on, the input frequencyf can vary
    On the other hand, if the input frequency decreases, its                   from 40 to 60 kHz; the VCO will track this input frequency
phasor slows down and 냐ie phase angle decreases as 計1own in                    and the locked output will equalf.
Fig. 45-3d. Now more dc voltage will come out of the phase
detector; this causes the VCO frequency to decrease unm It
                                                                               Free-Running Mode
equals the input frequency. In other words, the PLL auto-
matically corrects the VCO frequency and phase angle.                          Recall the astable 555 timer with no control v이tage. It
    Here is a numerical example. Suppose the VCO is locked                     oscillated at a natural frequency determined by the circuit
on to an input frequency of 50 kHz. If the input frequency                     components. 자ie same is true of the VCO in Fig. 45-3a. If
 increases to 51 kHz. the phase detector immediately sends                     the input signal is disconnected, the VCO oscillates in a free-
 less voltage to the VCO and increases its frequency to 51                     running mode with its frequency determined by its circuit
lmz. If the input frequency later decreases to 49 kHz. the                     elements.


                                                                           DC OUTPUT

                             INPUT                PHASE -       LOW-PASS -                 vcO          LOCKED
                             SIGNALf      －→    DETECTOR         FILT ER                           －→－-OUTPUTt

                                                   -
                                                                         佃)

                                                                 INPUT
                                          INPUT

                                                                                                       INPUT




                                     ：스
                                                   vco                           vCO                           vCO
                                           （川                            Ic)                           呵｝
                         Fig. 45·3. (a) Phase-locked loop. (b) phasor diagram. (C) increase in input frequency increases
                         phase angle; (d) decrease in input Ireguency decreases 帥ase angle.

                                                                     244

===== PAGE 260 =====
Capture and Lock                                                    ers. If the modulating signal is music, the signal out of the
                                                                    FM output will be the same music.
Assume the PLL is free-running or unlocked. The PLL can
lock on to the input frequency if it lies within the capture
                                                                    The 565
range, a band of frequencies centered on the free-running
frequency. The formula for capture range is                         The NE565 from Signetics is a 14-pin IC that can be con-
                                                                    nected to extert汕 components to form a PLL. Figure 45-5
                        Bc = /2 - /1                     (45-2)
                                                                    shows a simplified block diagram. Pins 2 and 3 are a differen-
where f2 and f1 are the highest and lowest frequencies the          tial input to the phase detector. If a single-ended input is
PLL can lock into. The capture range is always less than or         preferred, pin 3 is grounded and the input signal is applied to
equal to the lock range and is related to the cutoff frequency      pin 2. Pins 4 and 5 are usually connected together. In this
of the low-pass filter. The lower the cutoff frequency, the         way, the VCO output becomes an input to the phase detector.
smaller 巾e capture range.                                           In those ap하ications where the locked output is desired, pin
   Here is an example. Suppose the PLL can initially lock           4 is 山e output pin.
into a frequency as high as 52 kHz or as low as 48 kHz.                An exteri녜 山ning resistor `$ connected to pin 8. and an
Then 小e capture range is 4 kHz. with a center frequency of          external 山ning capacitor to 힌n 9. 재ese two components
50 kHz. If the lock range is 20 kHz and lock has been               determine me free-running frequency of the VCO. given by
acquired, then the input frequency can vary gradually from
                                                                                                             0.3
40 to 60 kHz without losing lock.                                                               r =                         (45.3)
                                                                                                             R7다
Locked Output                                                       차 and C. are selected to produce a free-running VCO
                                                                    frequency at me center of the input frequency range. If you
One use for the locked outputf, of a PLL is to synchronize
                                                                    want to kick on to an input frequency between 40 and 60 kHz,
the horizontal and vertical oscillators of TV receivers to the
                                                                    you chobse RT and C. to produce a free-running VCO fre-
incoming sync pulses. PLLs can also automatically tune each
                                                                    quency of 50 kHj
TV channel by locking on to the channel frequency. Still
                                                                       Pin 7 is me FM output. used only ，나ten an R4 signal is
another use for PLLs is locking on to weak signals from
                                                                    driving the phase detector. In FM receivers, a demodulated
satellites and other distant sources; this improves the signal-
                                                                    signal comes out of mis pin. 가uis signal then goes to other
to-noise ratio.
                                                                    amplifiers and eventually comes out the loudspeaker.
   In general, the locked output is a signal with the same
                                                                        Notice the filter capacitor CF between pin 7 and ground.
frequency as the input signal. Even though the input signal
                                                                    This capacitor and the internal 3.6-k1 resistor form a low-
may drift over a rather large frequency range. the output
                                                                    pass RC filter to remove the original frequencies, their har-
frequency will remain locked on; this eliminates the need to
                                                                    monies, and the sum frequency. The cutoff frequency of this
tune a resonant circuit for maximum output.
                                                                    filter is 뀀yen by
FM Output                                                                                                          ,        (45-4)
                                                                                            /   =     2iR,         C
Hgure 45-4a shows an LC oscillator with a variable tuning
                                                                    재e lower me cutoff frequency of this filter. me smaller 什ie
capacitor. If the capacitance is varied, the oscillation fre-
                                                                    capture range. In some applications, the filter capacitor is
quency changes. Hgure45劫 illustrates the output signal.
                                                                    omitted and the capture range equals 山e lock range.
자lis is an example of frequency modulation (FM). If the
capacitance of Fig. 45-4a varies sinusoidally at a rate of
I kHz, the modulation frequency is I kHz.                            SUMMARY
   When an FM signal like Fig. 45-4b is the input to a PLL
                                                                     L. When the input frequencies to a mixer are equal. the
like Fig. 45-3a. the VCO will track the input frequency as it
                                                                        output is a dc voltage.
changes. As a result, a fluctuating voltage comes out of the
                                                                        Given equal frequency inputs, 巾e output of a phase
low-pass filter. This voltage has the same frequency as the
                                                                        dereaor is a dc voltage that depends on the phase angle
modulating signal. in other words, the dc output now repre-
                                                                        between me input signals.
sents a demodulated FM output. This is useful in FM receiv-
                                                                        The control voltage to a VCO determines the output
                                                                        frequency.
                                                                        The low-pass filter of a phase-it漱ed 幻op removes the
                                                                        original frequencies. the harmonics, and the sum fre-
                                                                        quency. Thus allows the difference frequency. usu지lyadc
                                                                        V이ta2C, to contr이【he VCO.
                                                                        The phase an휀e between the input signal and the VCO
                                                                        sign비 determines the dc v이sage out of the phase detector.
ng. 45-4. Freguency modulation. (a) Varying capacitor varies Ire-       When a PLL. is locked on. the VCO frequency equals the
quency. (b) FM signai                                                    input frequency.

===== PAGE 261 =====
                           2

                     mPUT 3                                                                       FM OUTPUT


                           5
                 VCO INPUT "


                   LOCKED 괘
                   OUTPUT




                                                          1T
                                                          -vcc




                                            ng.45-5. Block &agram 이 the 565 PLL.


7. The lock range is the band of frequencies the VCO can             frequency of415 kHz and a minimum input frequency of
   generate.                                                         385 kHz. The capture range equals
8. The capture range, always less man or equ이 to lock             5. A 565 has a timing resistor of 10 kn and a timing
   range, is the band of frequencies that the PLL can lock on        capacitor of 0.01 p.F. The free-running frequency is
   when lock does not yet exist.
9. When the input signal is an FM signal, the PLL produces        6. The low-pass filter used with a 565 has art external ca-
   a demodulated audio signal at its FM output.                      pacitor of 0.01 pF. The cutoff frequency of the filter is


SELF-TEST

Check your understanding by answering these questions.            MATERIALS REQUIRED

1. In the phase detector discussed earlier, a decrease in         ■ Two power supplies: 9-V
   phase an햅e produces an                     in dc output        U Equipment: Oscilloscope, audio generator. electronic
    v《기tage.                                                        counter, voltmeter (digital if availa비e)
2. In the VCO discussed earlier, an increase in dc control        ■ Resistors: Two l-kft one 4.7-kfl [ -W
   voltage produces a                 in frequency.               ■ Potentiometer: 5-ku
3. If the maximum and minimum VCO frequencies are 450             U Capacitors: Two 0.01-p.F, one 0.47-1iF, two 0.I-1iF.
   and 350 kHz, the lock range is                                   one l- .`F
4. A PLL can acquire initial lock for a maximum input             ■ PLL: NE565


PROCEDURE

Free-Running Frequency
                                                                   5. Measure the minimum and maximum free-running fre-
 1. If the ac signal generator of Fig. 45-6 is disconnected.
                                                                      quencies with an electronic counter. (If not available,
    the 565 is in the free-runnir g mode of operation. What is
                                                                      usef = lIT where T is the period seen on the oscillo-
    the VCO frequency if the wiper of the potentiometer is
                                                                      scope.) Record the measured frequencies in Table 48-I ·
    all the way up? All me way down? Record the calculated
                                                                   6. Adjust the potentiometer to get a center frequency of
    frequencies in 聽비e 45-I.
                                                                      approximately 5 k汨z.
 2. Connect the circuit of Fig. 45-6 w油 a C,. of 0.2 " F
    (use two 0.l-pF capacitors in parallel).
                                                                   Lock Range
 3. Temporar啣 disconnect the ac signal generator to get
     free-running operation.                                       7. Reconnect the ac signal generator. Look at the signal on
 4. With the oscilloscope look at the VCO output (pin 4.              pin 2. Adjust the generator to get 0.5 V p-p at 5 난lz.
     Use a vertical sensitivity of 5 V/cm and a time base of       8. Look at the output (pin 4). Vary the frequency of the
     0.1 ms/cm. Vary the potentiometer and notice how the             generator from 4 to 6 kHz. Notice how the I'LL output is
     frequency changes.                                               locked ' nt ' me input signal.

                                                                 246

===== PAGE 262 =====
                                                                           +9 V




                                 1 〃F

                                                                                                   LOCKED OUTPUT


                                                                                                   FM OUTPUT


                                                           0.   01〃 F   小 CT
                                                                        J·      -9 V

                                                   FIg. 45-6. Experimental PLL circuit.


TABLE 45- 1. Free-Running Operation                                            12. Repeat step II for the other values of CF shown in Table
                                                                                   45→3.
      w:ptr               L.... kHz                  亡.S. kHz
                                                  1fl，
                                                                             FM Output
      Up
                                                                               13. Measure the dc voltage (digital voltmeter if available) at
      Down                                                                         the FM output (pin 7) for an input frequency of 4 kHz.
                                                                                   Record me dc voltage in Table 45-4.
                                                                               14. Repeat step 13 for me remaining frequencies in Ta벼C
                                                                                   45-4.
 9. Measure maximum and minimum lock frequencies.
    Record these values in Table 45-2.
                                                                               Extra Credit

Capture Range                                                                  15. Figure out how you can get a free-running frequency of
                                                                                   50 1Hz. Modify me circuit as needed. Then test it by
10. Calculate the cutoff frequencies onhe low-pass filter for
                                                                                   locking me PLL on art input signal.
    the values of’이 given in TabIc453. Record the results.
】I. Measure the maxinlum and minimum capture frequen-
    cie:,. Record in Table 45옰 Calc미ate and record mC                           TABLE 45-4. FM Output
    capture range. 하·뺨
                                                                                       Fr('quencv. I거z                     VdC, V

                                                                                              4
TABLE 45-2. Lock Ranqe

           /1,,.`,.kHi.                       ,. kHz
                                             人，                                                S

                                                                                              (,
TABLE 45-3. Capture Range

                                  /.,.1,,". kHz                         /n,a,.kHz                                            βr. kHz

           (1. 2

         〔Lㅣ

           () O47




                                                                         247

===== PAGE 263 =====
QUESTIONS                                                      Extra Credit

`. What did you calculate for the minimum and maximum          7. What change did you make to get a free-running fre-
   free-running frequencies in step -'?                           quency of 50 kHz?
2. Explain briefly how a PLL works.
3. Use the data of Table 45그 to work out the lock range.       Answers to Sell-Test
4. What is the capture range for CF = 0.2 띠＝'?
                                                               1. increase       4. 30 kHz
5. ，싸tat e仟ect does the filter capacitor have on the capture
                                                               2. decrease       5. , lJ1z
   range?
                                                               3. 100kHz         6. 4.42 kHz
6. The data of Table 45-4 proves a PLL can produce a
   demodulated FM output. Ex미amn why this is so.




                                                        248

===== PAGE 264 =====
                                                                                                                      ‘, ∼ , 1 EXPERIMENT
                                                                                THE SILICON CONTROLLED
                                                                                          RECTIFIER (SCR)




                                                                                    F
OBJECTIVES
1. To observe how gate current is used to switch an SCR on
   and off
2. To verify that gate current levels may be used to contr이                                               GATE
   collector load current levels                                                                                                                 GATE



INTRODUCTORY INFORMATION . __-

The silicon controlled rectifier is a four-layer NPNP solid-
state rectifier which has three electrodes: an anode, a cath-
ode, and a gate, which serves as a contr이 element. The SCR
differs from the two-element-diode rectifier in that it will not
                                                                                              ra)                                   rz刃
pass any appreciable current, though forward-biased, until
me anode voltage equals or exceeds a value called the for-                          FIg. 46-2. (a) SCR circuit symbol: (b) four-layer representation.
1`nrd breakover voltage. VBRF. ，싸ten VRRF is reached, me
SCR is switched on; that is, it becomes highly conductive.
The value of VBRF can be controlled by the level of gate                        Voltage-Current Characteristic
current. The gate then provides a new dimension in rectifier
                                                                                Hgure 46-3 is the v이tage-current characteristic of an SCR
operation in 咐tich low levels of gate current control hi帥
                                                                                whose gate is not connected (open). When the anode-cathode
levels of anode or load current.
                                                                                circuit is reverse-biased, there is a slight revers려eakage
   Various-capacity SCRs are manufactured today. Low-
                                                                                current called 小e reverse blocking current. ㄲ＂` current
current SCRs can provide anode currents less than I A.
                                                                                remains small until the peak reverse voltage V.ROM is
High-current 네icon contr애ed rectifiers pass anode or load
                                                                                exceeded. At that point the reverse avalanche region begins,
currents in the hundreds of amperes. The low-current SCR
                                                                                and the leakage current increases shat꾸ly.
resembles a transistor in physical appearance, with three
                                                                                   When the SCR is forward-biased, there is a small forward-
leads issuing from a hermetic캐y sealed housing. The hi助－
                                                                                leakage current, called the for'4nrd blocking current. 따tich
current SCR looks like a stud-mounted silicon rectifier with
                                                                                remains small un미 the forward breakover voltage is reached.
an added terminal (Fig. 46-I). The circuit symbol for an SCR
and its four-layer representation are shown in Fig. 46-2.


                                          0.V50 MAX                                                                             ucn. ＇댈
                                                                                                                       H1Gㅒc f4r》
                                                              0070 iSA                                                 ㄷuRRENT
                                                              (CAT((ODEI




                                                                                             REVEn$E
                                                                                                                          ／샐8＝유INGENT
                                                                                             BLOCKING CURRENT
                                                                                                     쵯

                                                                                                      ,




                                                                                                                              '


                                                                                                                              '             卜＼
  ONE PHOP40R BRONZE.
  McKEL-PL^!E0. Exㅜ
  '  TX LOCKWASI4ER AND
                                                T。
                                                 X몲 。.。40
                                                       DIA                          REvERsE
                                                                                    AVALAN(거0
                                                                                              4∼ PE^K REvERSE
                                                                                                                       F0nw^RD
                                                                                                                       BLOCKING CURRENT
                                                                                                                                           F R나＾n0
                                                                                                                                           RREAKOVER
                                  .l210                 1G^ TE}                                  VOLTAGE                                   v이．T^GE
  .ㅐE ·R^:" NfcKEl*=Pㄴ
                     ＾rE.                                                           cUn nE＇냄ㅜ
  NUT SUP'LIED w TX EACI

  UNIT,
      : INSI
  AVAII.
       .ARL섦.     N
                  TING
                    REOUEST
                       HARDWARE             ∼                                                                    '1
                                                m1i ^` L 마H[HSIONS ~" ～ㅐ
                                                                       （＞在｀
                                                                                Fig. 46-3. Voltage-current charactenstic of an SCR whose gate is
                F19. 46-1. A stud-mounted SCR, GE-type C20

                                                                              249

===== PAGE 265 =====
This is the forward avalanche region. At that point the current                         '01 >lR
                                                                                                       1R, > '. 1
                                                                                                          /          i ‘ㅎ >In·

jumps rapidly to the high-conduction level. Here the anode-
to-cathode resistance of 轍e SCR becomes very small, and
the SCR acts like a closed switch. h this high forward-
conduction region, the voltage across the SCR drops to a very
low value, and to all intents and purposes almost me entire
source voltage appears across me load which is in series with
me rectifier (Fig. 46-4). It is the extcrl녜 load resistance.
then, which must limit the current throu합，     the SCR and hold                                                       V.-,


it within the rated value of the SCR.
   가te two operating stages of the silicon controlled rectifier            Fig. 貂-5. Etfect 이 gate current on lorward voltage breakOver 1ev히·
correspond to the two states of an on-off switch. When the
 applied voltage is below me breakover point. me switch is
                                                                             The gate circuit is rated as to its power dissipation and Its
 OFF. When the voltage increases to a value equ키 to or greater
                                                                           forward and reverse gate-voltage capabilities.
 man 山e breakovcr voltage, the rectifier is turned on. The
 rectifier remains ot' . that is. in "` hi助-current state, as long
 as me current stays above a certain v시ue called the "h이ding"              SCR Ratings
 current. ，싸ten the v이tage across the rectifier drops to a value
                                                                           To ensure trouble-free operation, the manufacturer's max-
 too low 〔《）sustain the holding current, the rectifier turns off.
                                                                           imum ratings should not be exceeded. Permanent damage to
                                                                           the rectifier may result if operation beyond these ratings is
Gate Control of Forward Breakover Voltage
                                                                           attempted. SCR ratings include:
When 山e gate-cathode junction is forward-biased, the rec-
                                                                           PFV          repetitive peak forward v이tage, gate open




                                                                            b盼喀乙凡蝦지rJ
tifier is turned on at a lower anode-v이tage 1ev이 than w따i the
                                                                                        rms forward current. ON state
gate open. That is. the value of forward breakover voltage is
                                                                                        average forward current, ON state
                                                                                  今p
reduced with forward bias. This is evident from the charac-
                                                                                        peak reverse voltage, gate open
teristic curves itt Fig. 46-5. The maximum forward breakover
                                                                                  ^     peak gate power dissipation
V이tage VRRI.。occurs when me gate is open: that is. ，나1en
                                                                                        average gate power dissipation
                                                                                  αR
gate current 'Gil = 0. When there is gate current at the level
                                                                                        peak reverse gate voltage
1(7 ). the 化rward breakover v이tage VRRFI is lower 山an
                                                                                  g     storage temperature
 V8F(Fn' 도milarlv VARE,. which is determined by ' (72 which is
                                                                                        operating junction temperature
greater than1(7 ) . is lower than Vfip . and VRR/.1is lower than
 `"BRP2.
    AS the gate current b increa.ced, thiIe ScR Z)egins to act Ii如         SCR Used As a Rectifier
 αn ordinary silicon rectifier.                                            Silicon controlled rectifiers are very useful in ac circuits
    After the SCR has been turned on by gate current, the gate             where they may serve as rectifiers whose output current can
 loses control, and reducing gate current has no effect on                 be controlled by controlling 小cir gate current. An esample of
 anode current. The SCR remains on until anode forward                     this type of application is the use of SCRs to operate and
 voltage has been removed or until the anode forward-voltage               control dc motors or any dc load from an ac supply.
 level is below that required to maintain the holding current.                Refer to Fig. 46-4. In this circuit the SCR is connected as a
 When the anode source is 曲ernating current, the rectifier                 half-wave rectifier supplying current to R,. The gate is open.
 turns off during the negative alternation, when the anode'                The SCR switches on when me forward breakover V이tage is
 cathode is reverse-biased.                                                reached, at point V,IR() on the positive alternation of the
    Since they are contr （川ed by forward gate bias, silicon                applied sine wave. During the interval VRR0 throu맞1V, the
 Conir애ed rectifiers are operated below the maximum for-                   SCR conducts, ，싸ten the anode voltage drops to V.Y. whi야Its
  ward breakover point.                                                    b리ow the holding current potential, the SCR turns 이'f. It
                                                                           remains off during the negative alternation. Current through
                                                                            the load flows during the interval V,IR。through V.Y. 가IC
                                                                           ap미icd voltage, anode-to-cathode vohage. load voltage, and
                                                                           current waveforms observed in the preceding Circuit are


  巨二)
                                                                            shnwn in Fig. 46.6.
                                                  TO OSCILLOSCOPE
                                                  VERTICAL INPUT               In Hg. 46-7 the voltaee V,,,,.,.,1 at ｀나tich the S아之 " turned
                                                                            on is contr이led by the gate current. ,｀倆d, in turn is deter-


                                             S
                                                      I                     mined by the setting 可 t'(·．(,. the gate current source, and R,.
                                                                            `'/1∼is lower than t ",1,。, Therefore the period during which
                                                                            mc load draws current t "(fRIIi mrough t ' t is increased, and
      Fig.46-4. AC source driving an SCR and load, gate open                more current is d이isered hs mc recOtier to mc iiad 'the


                                                                     250

===== PAGE 266 =====
   ANODE
   $u叩Lv                                                                                                                        1DA》
   v《）
     LT^GE                                                                                                                 〃‘   VOLTAGE
               0




                                     /v   '

                                                                                  Rg. 46-8. SCA controlled by ac gate current.
  ANODE- TO-
  CATHODE
  VOLTAGE      .

                                                                         resistance R,. were re미aced by a light bulb, or by a bank of
                                                                         bulbs, the circuit of Fig. 46-8 could serve as a light dimmer.

                                                                         NOTE: For a sizable load, full-wave rather man half-wave



                        1
                                                                         rectification would be employed. A full-wave contr이］  ed
 LOAO CURRE Nㅜ                                                           rectifier wo미d require two or more SCRs.
      &
 LOAD VOLTAGE 《）                                                         CAUTION: 7加 peak reverse gaze volta舒？ must not be
                                                                         exc·eeded.
               Fig. 46-6. Wavelorms in SCR circuit.


                                                                         SUMMARY
conductom period can he further increased by increasing gate
current he ond the 1eve! in the preceding exam힌e.                         1. 재e silicon contr이led rectifier (SCR) is a four-layer
    Note that c'ate current can be and " relatively low corn-                NPNP solid-state rectifier which contains an anode, a
pared with aflodC current, In the circuit of Fig. 46-7. a dc                 cathode, and a gate.                      .
milliammeter M. is used to measure the gate contr이 current.               2. Unlike the diode rectifier, the SCR will not conduct.
The average load current throu만｀ R1 may measure many                         mough its anode-to-cathode is forward-biased, until the
 amperes. depending on the am이itude of갸ic applied v이tage                     anode voltage equals or exceeds a value called me
 and on mC si/c ol R, ; However. me average anode current                    forward breakover voltage (v〃RF〕    ，
 should not exceed the average anode-current rating of the                l 什e hreakover voltage can be contr이led by the value of
「c（·nhc「                                                                     gate current.
    Control of' anode current hy 山reet gate current was iIlus-            4. SCRs vary from low- to high-current devices.
 truted in Fij. 4h-7. The circuit of' Fin. 46-s mustrate.s ac             5 The forward and reverse voltaee-current characteristics
 contri比 whid, is more trequen小 em힌oved than dc contr이．                      ot an SCR are shown in Fifl. 46-3.
 In this circuit 山e anode-to-c,1ihode viltage bnr the SCR is              6 가ie forward hreakover voliage " affected by me level of
 supplied hy the high- voltage secondary ol transformer T. 가IC               eate current. Fieure 46-5 쟈05'.'S mat as gate current is
 gate Current is d이ivered hv me bow-voltage secondary ，써nd-                  increased. V,?RF is decreased: that is. the forward anode-
 ing. Rheostat ／헌 is used to adjust the les이 of gate current.                io-cathode voltaL'e required to fire me SCR is reduced.
 hence me conduction period of the SCR. ∥’ me load                        7. Alter an SCR has been turned on the eale loses contr이．



                                                   A


                                     !




                      三그
                                                                                                    RL



                                              CT                                      T   '
                                                                +                                                LOAD
                                                                                              S2                vㅇL ㅜ＾GE
                                                                                                   +
                                                                    A1           R2




                                                       c




                                n0. 46·7, Voitaoe at wriici' SCR is turned on is controSed by ac gate Current

                                                                     251

===== PAGE 267 =====
      Inereasine or deere iistne eate current ssull men not 相I-ct           lorssard-s川I.ig. e l cs이 is belay that required to maintain
      anode current.                                                        什is, 加1.1mn;g i'i,rrp'nt
 & An 5CR. therefore. is like an on-otf sㄳ itch ，싸ten it                 5 W'hen :he anode source of an SCR " 汕ernating voltage.
                                                                              .




      tires. it is us(. Otherwise ii is o,-i'.                              me rectmer turns                         during the negative
 9, 가te SCR can be connected as a rectifier supplying                       汕emation.
      unfiltered dc current to a load as in Fig 46-7. Here dc               In Fig. 46毛 山e point on me anode-to-cathode voltage
      gate current contr이S 山e firing point. Figure 46-6 寸11)55 S            waveform at ，나tich 山e SCR tires is                         It
      the waveforms sshid, V.m be seen in this circuit.                     reniains conducting until me anode-to-cahodc voltage
10. The firing point of an S(斗乙can also he controlled by ac                                     is reai갸ted. ，싸ten it turns 이1
      gate current, as in Fic. 46-8. II me load in this circuit          7.
                                                                            The current waveform in Fig. 46-6 shows mat load
      were a light bi批）   . varsing R,. the gate current control            current remains constant during the time that the SCR is
      would affect the brightness of the bulb. This circuit may             애．                        (m1r. false)
      therefore be used as a Ii아tt-dtnimine Circuit                      8.
                                                                            The gale current source of an SCR mas be either
I I . 가ieS아之is use&nn 이ectronics ii) suppk rectified current                                    or
      to a load. The lI".el of' the rectified current ``` determined     9.
                                                                            가te forward-bias voltage of an SCR. anode to cathode,
      by the sttInt o gate current control and by the param-                 is dc. The 1ev이 of gate current is adjusted to fire the
      eters of 什ic circ네I.                                                   SCR. Once it has fired the SCR may be turned off by
                                                                             reducing the gate current.                      (true, 五小기
                                                                        10. The holding current is the                      嫩ate, anode)
SELF-TEST                                                                    current b이ow which the SCR turns off.

Check sour understanding hs ansV.ering these questions.

 l . An SCR is a more versatile device than the diode silicon           MATERIALS REQUIRED
     rectifier because anode current can be contr에ed by the
                                                                        ■ Power supply: Variable reg미ated 0-50- V dc source
     1ev이 of                    current
                                                                        U Equipment: DC oscilloscope; EVM; 0-10-mA dc mdli-
 2. The forward breakover soltage (VflR戶) of a particular
                                                                          ammeter: 0-I 00-mAde milliammeter or equivalent ranges
     SCR is 150 V. anode to cathode, when there is 1.5 m.A of
                                                                          on a VOM
     gate current. If the gate current is increased to 2.5 mA.
                                                                        ■Resistors: 220-, 1000-. 5100-fl Y:-W: 500-fl 5-W
     me forward breakover voltage will become
                                                                        ■ Semiconductors: 2Nl596 SCR or equivalent, with heat
                      (/]＇이ier, lower) than IS0 V
                                                                          sink; IN5625 or equivalent
 3. An SCR may be used as an alternating-current                        ■Miscellaneous: Power transformer 120-V primary. 25-V
                                                                          I-A secondary (Triad F-40X or equivalentl: 2-W 5000-fl
 4. Once an SCR fires, it remains ON unm the anode forward                potentiometer; two SPST switches
    voltage has been                  . or until 什te anode




PROCEDURE 祗i                                                                                    a毗－            크竹y2牡｝s贓珊．
                                                                                                                        -：淡盛＝,


NOTE: The 2N1596 low-current SCR is rated at 1.6 A rms                  w1tage. ')r to reduce the anode current below the holding
anode current, peak positive gate current 100 mA. peak gate             current level.
voltage 츠 6 V. nese ratings should not be exceeded
   The gate current required to turn on the SCR may vary
widely. Moreover, the dc gate currents required to trigger the           DC Anode Voltage. DC Gate Current
2Nl596 over the range of anode supply voltages which this                     1. Connect the circuit of Fig. 46-9. Switches 옥 and 옥 are
SCR can handle mas be grouped very closely together. The                         both open. VAA is a variable regulated power source.
first part of this experiment will therefore be exploratory. The              2. Set V,)A at IS V as measured across the power sup이V
student will determine the dc gate current required to turn on                   with 옥 open. Do not vary VAA again until instructed to
the SCR when the anode supply is first set at 口 V dc, then at                    do so. ＾쐬 measures anode cu누rent after the SCR turns
40 V dc.                                                                         on; ^h measures gate current V1 measures anode-to-
    After the flnng characteristics of 山e SCR are observed.                      cathode voltage. When the S아   （ has fired. me voltage
小e student will study the rectification characteristics of the                   across me SCR will drop to a very low value (about 0. 1
2N1596. using an ac anode supply.                                                to 3 V) and the anode current 'A will be limited by V,.A
    The experitnental zechnique.s are carefully ,sez forth "i rite               and me size of R1 . For with the SCR ON
following i,tstructio,i.c. Th1ese should bt? 7ollowed precisely.
Note that w.hen using an anoded("suppl.y, the n川vst,ay to turn
 硼〃n? SCR after it has fired " to turn 町 the anode supply
                                                                                                 /,   A=   知   (approx)



                                                                       252

===== PAGE 268 =====
                                                                                            Fig. 46-9. Experiment키 dc circuit to
                                                                                            determine SCA characteristics.

 3. Set R,(gate current contr이）output at 0 V. Close S.,.                  record anode voltage VI)F across the SCR after it has
    Close S1. `$ the SCR oN?                                              turned on. Measure and record anode current 'A after the
 4. Adjust R, very' gradually, monitoring gate current, just              SCR is ON.
    to the point ，나iere the SCR is ON.                                 5. Open 옥 . Readjust R2 `() that gate voltage is again 0 \/.
                                                                          Repeat step 4 and record your res미ts under trial 2
Nore: If the SCR does not turn on, it may be necessary to
                                                                       6. Repeat step 5 for trial 3.
reduce the value of the 5100-n resistor in the gate circuit, or
                                                                       7. After the SCR has fired, in step 6. open 이．     removing
to 이iminate ‘【 altogether.
                                                                          gate current. Observe and record in Table 46-1 the
    Measure and record itt Table 46-I . under trial 나he gate              effect, if any, on anode current, after the SCR is ON, of
    current required to turn on the SCR. Measure also and                 opening gate swit야，   옥．
                                                                          Open 옥 . Now both 옥 and 옥 are open
TABLE 46- 1. DC Anode Voltage. DC Gate Current                         g:
                                                                          Set VAA at 40 ,/ as measured across 小e power supply
                                                                           with 옥 open. Set R, gate current control at 0 V. Close S
  VAA. V     1c. mA      VpF. v     'A. mA        Trial Number            and S1. Determine in three trials the gate current
                                                       ㅣ                  required to trigger the SCR. following me procedure
                                                                          oumned in steps 4 and 5. Record your results in Ta비e
    경5                                                  2
                                                                          46- l .
                                                        3             10. Repeat step 7 after me mird trial,
                                                        1
                                                                      DC Gate Control and AC Anode Source
    40                                                  2
                                                                      11. Connect the circuit of Fig. 46-ID. S1 and S, are off
                                                        3                 T is the power transformer used in early power-supply
Effect on anode current, after SCR is 아냄. of opening gate switchS2:       experiments. Set VGG, the dc gate supply, at 6 V. .
Step 7                                                                12. S1 on. S2 remains ‘赤 Set your oscilloscope on line
Step K)                                                                   trigger/sync. Observe the waveform from A to C. Adjust
                                                                          the oscilloscope controls un미 this reference waveform




                                                                                                          enment히 circuit using tic
                                                                                            Fig. 46-10. E지〕
                                                                                            gate conir이．

                                                                      253

===== PAGE 269 =====
TABLE 46·2, AC Anode Source. DC Gate Control
                                                            `bIts.
     Wav介rm No.                 밗2veform                 Peak 尸Ositive         'L' mA         1c, mA         Conduction Angle
                        /／콘
      Reference                \                                                  x                 x                x
                                    \,
                                              }
       I (max.)


      2 (mmn.)




    appears as in Table 46-2. Measure and record in Table             AC Gate Control and AC Anode Source
    46-2 its peak-to-peak voltage.
                                                                      14. Power of!. Modify the preceding experimental circuit to
       Observe the waveform across the SCR, points B to C.
                                                                          conform with 山at in Fig. 46-11. Note that an ac gate
    This should be me same as the reference waveform as
                                                                          source is used, rectified so that the positive alternations
    long as the SCR is oF1. When the SCR iS ON, the anode-
                                                                          appear on 由e gate.
    to-cathode voltage waveform (Fig. 46-6) will appear on
                                                                      15. Power on. With an oscilloscope connected across the
    the oscilloscope.
                                                                          load resistor (VBC) observe the load voltage waveform as
13. Close S,. 引owly vary R2. the gate current contr이，over
                                                                          R2, the gate current control, is varied from minimum to
    its entire range and observe me effect on 小e waveform
                                                                          maximum. Record in Table 46-3 the minimum and max-
    from ano六＇α cathode 恪'8C).
                                                                          imum conduction angles, and the corresponding load
       In Table 46-2 draw in proper-phase with the reference
                                                                           waveforms.
     waveform VBC for maximum conduction period (wave-
                                                                      16. In Table 46-3 also record the measured values of gate
     form 1) and minimum conduction period (waveform 2)
                                                                          current IG and load current 'L for me minimum and
    Measure for each the peak positive aniplitude of the
                                                                          maximum conduction angles.
     waveform, the load current 'L, the gate current 1c. and
    the conduction angle (duration in degrees of the on
    interval in any one cycle). Record the data in Table 46-2.




                                         F닙. 46-11. Expenmental ac circuit usln9 ac gate control.

                                                                  254

===== PAGE 270 =====
TABLE 46-3. AC Anode Source. AC Gate Control
                                                      conduction ^＇섕／e.
     Wav/brm No.               Waveform                    Degrees                   V p-p        /L. mA        /c. mA

                              \
                        ／十
      keference                                                x                                     x             x
                                             /
                                   `
                                       \\`

      Maximum (D


      洲nimum (2)




QUESTIONS                                                          7. What triggering/synchronizing arrangement in this cx-
                                                                      periment makes it possible for you to observe the load
1. What are the differences between an ordinary smcon
                                                                      waveforms in proper 山ne phase with me reference
   rectifier and an SCR?
                                                                      waveform?
2. After the rectifier turned on. what effect did the anode
                                                                   8. Compare the effectiveness of the ac versus the dc gate
   voltage supply have on anode current?
                                                                      triggering source on control of anode current in this
3. Will the size of load resistance affect the level of load
                                                                      experiment.
   current in the citcuit of Fig. 46-9? How?
4. How does the forward breakover voltage vary with bias
                                                                   Answers to Self-Test
   current? Refer specifically to your data【《〕confirm your
   answer.                                                         1. gate              6. 匕RFO' VX
5. How does load current vary with conduction angle? Refer         2. lower             7. false
   to your data in Table 46-2.                                     3. rectifier         8. dc: ac
6. Refer to waveform I Table 46-2. Identify the forward            4. removed           9. false
   breakover voltage point.                                        5. off              10. anode




                                                               255

===== PAGE 271 =====

===== PAGE 272 =====
                                                                             Appendix A



(o1hode-Roy Oscilloscope(CRO)*




CRO GAIN CALIBRATION AND POWER SUPPLY VOLTAGE CHECK


The basic measuring instrument used in these experiments is the CRO. It is used to observe and
measure waveforms, but in particular it is used as a dc voltmeter. With proper care paid to the gain
calibration of its vertical amplifiers, it can be used as an accurate laboratory measurement instru-
ment. Since the ICs used in these experiments are fragile and have a very small voltage-overload
factor, the CRO can be and must be used to check power supply voltages before power is applied
to the ICs.
     Connect the output of the CRO internal calibrating voltage to the vertical input of the CRO.
If a multirange calibrator is available, use a 10-V p-p voltage and set the vertical gain to 2 V/div.
This will provide a p-p deflection of exactly 5 divisions. If 10 V is not available, use a combination
of calibrating voltage and vertical amplifier calibration to give a deflection of 4 or S divisions. Now
obtain a steady pattern using the CRO triggering and horizontal TIME/DIV controls and check the
voltage calibration of the vertical amplifier. If the deflection does not agree with the calibrating
voltage, call the instructor. Then set the CRO vertical amplifier for I V/DIV.
     Important: Before connecting power to the ICs, check the power supply voltage against the
calibrated CRO. If the measurement with the CRO agrees with the output voltage of the power
supply,'power can be applied to the ICs and the experiment can proceed. If it does not agree, call
the instructor.


      *lt is assumed that the student has had some previous exposure to the CRO and is familiar with its basic opera-
tion and the function and operation of its controls.


                                                       257

===== PAGE 273 =====

===== PAGE 274 =====
                                                                    Appendix B



Lo9ic Symbols




Logic functions are two-valued: ONE or ZERO, I or 0; HIGH or LOW, H or L;TRUE or FALSE,
T or F; ON or OFF. Although the functions can be implemented in many different physical ways,
the net effect is that of identical logic performance. To show that identical logic is being performed,
sets of graphic logic symbols have been developed to depict the various logic functions.
      The logic symbols used in this manual are those based on the distinctive-shaped symbols of
American National Standard, ANSI Y32-14 1973, IEEE Std. 91-1973. These symbols are recom-
mended by the semiconductor standardizing committees of the Electronics Industry Association
(EIA) for registration of microelectronics logic functions. Virtually all integrated circuit (IC) manu-
facturers' published engineering data specifying dual-state logic functions use these symbols. Figure
B-l shows the symbols used in this manual.
      Logic functions may be simple or complex. A type of complexity that frequently occurs is
the requirement that a gate be controlled by more inputs than can be provided by the number of
available terminals of the case in which the gate is packaged. To provide additional gating capabil-
ity, gates can be provided with an expander input. The symbol for this is shown in Fig. B-2.
      Figure B-3 shows the application of these logic symbols to circuits such as those used in
Experiment I. Integrated circuits that perform these functions are called AND and OR gates.
      Although AND and OR circuits have many applications in logic circuitry, they do not have
complete versatility. The NAND (AND plus inverter) and the NOR (OR plus inverter) have much
greater usefulness. Logic symbols for NAND and NOR functions and INVERT are shown in Fig. B-4.
      Frequently, a function is controlled by a gate as part of a complex IC function. A typical illus-
tration might be the control of the set input to a flip-flop by means of a 3-input AND gate. Figure
 B-S illustrates the logic-symbol method of illustrating this function.




                                                 259

===== PAGE 275 =====
                                                                                                      0
                                                                                             (c) NOT (small circle)
               (a) AND                                           (b) OR




          (d) NON INVERT
                                                   工）(e) EXCLUSIVE-OR


                       1
                       1  干
                       i TF


                                                    H
               , ,,T
                                                                   SS
           7
           S     FF, , , C
           l。r O   O。  rQ                                        J;==l-
               I              I
            (f) FLIP-FLOP                                 (g) SINGLE SHOT




               (h) Amplifier
                                          －《
                                                         1'is


                                               (i) Time delay
                                                                   )             H(j) General logic symbol for
                                                                                      unspecified function

                                                F杻. B-I. U)gic symb이S.




                                                                        Two-input AND              Three-input OR
Expande                                                                     AB = C                  A+ B+ C= D

Fig. B-2. Expander input symb이．                                        Fig. B-3. Logic symbols for AND and OR functions.




    Two-input NAND
                                                  B즐DO-D Three-input NOR
                                                                                                          INVERTER

          C = AB                                           0 = A+B+C

                   Fig. B-4. Logic symbols for NAND, NOR, and INVERT functions and applications.




                                                ss S니＜
                                                 1
                                                 1 ^
                                                   z n

                                                            )5
                          Fig. B-5. Flip-fl이】
                                            1with SET function controlled by a 3-input AND gate.

                                                                 260

===== PAGE 276 =====
                                                                              Appendix C



The UNIT-LOAD Concept




To simplify output fan-out and input fan-in design, the unit load (UL) concept has been devel-
oped. A UL has significance only for its own logic family and for compatible logic families, but
not for noncompatible families.
     A UL is the load presented by a standard gate input. For example, in the TTL gate of Fig.
4-1, a UL would be the current flowing out of input A when input A is at a low potential and
input B is at a high potential. From Fig. 4-I this is

                                           (5-
                                                   0.  V7)
                                                         斗
                                                 4.。kfl
                                                                   l.   1mA
Now, let us suppose that output transistor Q3 of Fig. 4-1 is capable of sinking 11 mA. We can
express this on a UL basis as 10 UL.
      UL values are shown on IC gate specification sheets as values in parentheses next to the IC
package pin numbers. For example, suppose that we looked at the logic diagram for the gate of
Fig. 4-1 on a data sheet. It would be shown as in Fig. C-i.




                       Fig. C-I. Logic diagram of the 2-input NAND gate of Fig. 4-I.

     In Fig. C-i, the two gate inputs are at pins I and 2 and the output is at pin 3. The input load-
ing, shown in parentheses, acts as I UL in TTL logic and the output can drive 10 UL (1TL unit
loads), as shown in parentheses at the output terminal.

                                                             261

===== PAGE 277 =====

===== PAGE 278 =====
                                                                         Appendix D



IC Lo9ic Dio9roms
and Pin Connedions
(Top View)*t4


555




                                                                                       V PACKAGE
                                                                                       (Top View)

                                                                                      1. G und
                                                                                      2. 1igqr
                                                                                      3 0UtpU'
                                                                                      4. R.＄·t
                                                                                      5 Contr이 v It.9·
                                                                                      6. Th
                                                                                          ＇·thOId
                                                                                      7. D,,6. rg.
                                                                                      8. Vcc
                                                                    ORDER PART NOS S5555V/NE555V




      *555 reprinted from the Signetic Data Book. Permission to reprint granted by Signetics Corporation, a sub-
sidiary of U.S. Philips Corp., 811 E. Arques Avenue, Sunnyvale, CA 94086.
      tCD4001A, CD4007AD, CD4007AF, CD4007AE, CD4007AK, CD4049A and CD40SOA courtesy of RCA
Solid State.
       t 00, 02, 03, 04, 05, 06, 10, 14, 20, 32, SN5447A, SN7447A, 51, 72, 76, 5N5483A, SN54LS83, SN7483A,
SN74LS83, SN5447A, SN7447A, SN5483A, SN54LS83, SN7483A, SN74LS83, SN5486, SN7486, SN7489,
5N5490, SN7490, SN5496, SN54L96, SN7496, SN74L96, 121, 122, SN74141, SN5274l and SN7274l courtesy
of Texas Instruments Incorporated.

                                                     263

===== PAGE 279 =====
                                                 V凶
CD4001 A
COS/MOS NOR GATES
(POSITIVE LOGIC)




                                                                              9 2C 5 侈 ，《）
                                                                                         n
                                           vs$




CD4007AD. CD4007AF
CD4007AE, CD4007AK
COS/MOS DUAL COMPLEMENTARY
PAIR PLUS INVERTER


                                4可輒
                                     H? LJ
                                     u            1크        N3         L
                                     Terrnrnal No, 14 = V00

                                     Terr rraI No.                    7 = Vss




        00
        QUADRUPLE 2- INPUT
        POSITIVE NANO GATES




        P h1I』ve 陌9띠
        V    AB


                              SNS400fSN7400IJ, N)                                            SN5400/SN 7400> WI
                              SNS4I-400/SN74HOOIJ, NI                                        SN54HOO/SN74HO이WI
                              SNB4LOO/SN74LOOIJ N>                                           SNS4LOO/SN74LOOIT)
                              SN54LSOO/SN74L5001J, N, WI
                              SN54SOO!SN74SO(기J N w}




                                      :;
                                                 ㄴ쎄 ㅏ            l     t
        QUADRUPLE 2-INPUT
        POSITIVE NOR GATES            L<＝亡. L＜그1 」
        POilIly. Ia91C
         Y = A +B
                                戶百
                                1Y    `'     1·        'Y        7t    7·   GN.                `^


                              5N5402/5N74021J. NI                                            $N54
                                                                                                （〕2 ISN741〕
                                                                                                          2( W I
                              SNS4L02/SNY4L02IJ, NI                                          SNS4L02/SN74L02IT>
                              SNS4 LS02/SN74 LS02IJ, ＂』w)
                              SN54S02/SN74S02나』＇니． WI




                                             264

===== PAGE 280 =====
                                                     蠶g
CD4049A. CO4050A                                                                      래
                                                                                      ,

COS/MOS HEX BUFFER/CONVERTER                                                          m
                                                                                      H

                                                                                      叱
                                                                                      1


                                                                                      .
                                                                                      J
                                                                .

                                               늬                                      래
                                               ［＞」,"                놔＞므
                                                                                      ■


                                           ,   스｛
                                                     :/c.   r   ,   쁘｛   ＞브
                                                                                      J
                                                                                      `


                                          叱ㄷ 」－                 낟ㄸ －스－
                                          딩，̀ J-                V,$ J-
                                           "C ' '`              K. ,`
                                           떼c 1 '     r·l       `. · .         l11
                                                                              ·K`    오m

                                               c0404.A              CD40EOA




                                                                                           v     ．·   1^   1Y     月    l^    1Y


        .3                                                                                                                   ·

        QUADRUPLE 2-INPUT
        P SITIVE川AND GATES
        WITH OPEN-COLLECTOR OUTPUTS
                                                                                                                  〔》」
                                                                                            -
        mtilive logic:.
        V = AB                                                                              `^   1·   1Y   21     7B   7Y   c` .


                                                                                          $N54.3/$N1403U. N1
                                                                                          SN54L03/5N74L03(J. N》
                                                                                          SN54LS03/SN74LS03(J, N. WI
                                                                                          SN54503/SN745031J. N. w)

                                                                                            1r   6^   ‘γ   GNl)   §Y   `^    ·，
                                                                                                                  0
        04                                                                                  H


        HEX INVERTERS                                                                            N                吐4 1
                                                                                          △                                 蠟＼
                                                                                                 「日
        Pm1)1W. 1(3만C
        V =A                                                                                                      N
                                                                                            `^   교v   2^   vㄸ     3^   ]Y    '^


                                       SN5404/SN74041J. NI                                SN5404/5N7404(WI
                                       SN54H04/SN74H04IJ, N)                              SNS4H04/SN74H04(WI
                                       SN54L04/SNT4L04(J. ＂》                              SN54104/5N74L04(T)
                                       SNS4LS04ISN74LS04IJ. N, WI
                                       SN54504/SN74S04IJ. N. w)

                                                                                            1Y   .'   6Y   GND    5V   5'   ·＇


        05
        HEX INVERTERS
        WITH OPEN-COLLECTOR OUTPUTS



        p)NCiti＇· 황에比：                                                                                            N
        V= A
                                                                                            1^   ?'   ?^   vㄸ     】＾   ］γ   .^


                                       SN5406觸N7405U. ＇니1                                 引녘54.5/$N74《｀5
                                                                                                       《w)
                                       S"5새（)5/$N7하 ()6
                                                      （』'．寸I                              SNS4HOS/SNT4HOSIW)
                                       `N54L505/SN74LSOSIJ. '.. w)
                                       SNS4SOSISN74SOSIJ. N. WI



        06
        HEX INVERTER BUFFERS/DRIVERS
        WITH .PㅌN·COLLEcT."
        HIGH-VOLTAGE OUTPUTS


       "sitios I여FC:
        Y=A


                                                                                          SNS40B/5N7406". N. n1




                                                     265

===== PAGE 281 =====
10
TRIPLE 3-INPUT                                                                    m
POSITIVE-NAND GATES
                                                                                            0
'."'t1멩1log.-
Y 蜜 ^Bc
                           II   2k    2$   IC    2'   CCC     ``    ＇·   ''     vCC   2'    '^    ?1
                      sN541이3N741이』  ．"l                    $N5410眉춰74｀ 《Hw1
                      SNS4H10/5N74P41이』  . N)               SPdS4H10iSN74U10)W)
                      SN54L I0/SN74LI0(J. N)                $N54L 1CV$N74L10)T)
                      $N541S10/SN74LS10∥. " . WI
                      $N54$1. /$"74S1이』 ．" . 배1




                                                               1D

                      ㅂ꼽닙＜｝尸骨；니퓽∼背，背l－十:.
                                       ，
                                                                    `'   뱁■     cHD   rY    z1)   』《


20
DUAL. 4-INPUT
POSITIVENAND GATES                         녘그
                                                〔＝)-
mIsilICe I여鮮
V = ABCD              河三스H노已‘논닌〕
                               끄〕1츠츠                          닌－HaJl그J1꽈긴J七J1JJ→
                                                               `'   `'   NC     kCC    2C   20    2?


                      SN5`20人N742.{J. N》                    $N5420唇N7`2《川w)
                      $"54H2이＄N74M2CHJ. N1                  SN54H20/5N74H2이w》
                      $N54L20唇N74L2이』  . N'                 針154L20/SN74L20(T)
                      $N54LS20/SN741S2이』  . N. WI
                      s'd54s2이＄N74s2이J. N. wl               NC - NO ", ttInaI    0000CClIOn




                                     266

===== PAGE 282 =====
SN5447A,SN7447A                                                                                   TYPES 5N5483A. SN541583. SN7483A, SN741S83
BCD-TO-SEVEN-SEGMENT DECODERS/DRIVERS                                                             4-BIT BINARY FULL ADDERS


          '46A '47A . ' 』．N. OR w PACKAGE                                                                                                             ·1. F H. i `'＇·H^1. 더）
                                                                                                                                                                           써H/c'1며
                                                                                                                                                      ..             -^－小       `.
            '146. '147 ; ' . 』OR N PACKAGE
                      I TOP VIEW)




                                                                                                                                                 `＇나545'擢N7451(J. N)
                                                                                                                                                 sH5．ㅐ5I唇N7'H5HJ. NI
                                                                                                                                                 $N54弱"SN74`5`U, N. W1




SN5447A. SN7447A
BCD.TO-SEVEN-SEGMENT DECODERS/DRIVERS



                                                AND-GATED J-K MASTER-SLAVE FLIP- FLOPS WITH PRESET AND CLEAR
      72                    EUNCTION TABLE                                           형       ＇月       .K       .J         `?   .1   .            K3        .=   .    ‘」
                                                                                                                                                                      “P    .      즈“ 스－
                                                                                                                                                                                 ! ·ㅣ l
                            INPUTS                          OUTPUTS
                                                                                                                                                                                        'I
       PRESET CLEAR CLOcK                        』     K     O      O
            L           H            x            x    K     H      L
            H           L            X           x     X        L   H
            L           I            K           IC    X    H*      H*
            H           H           .11.         1     L    ().     00
            H           H           」1           H     I     H       I
            H           H           J1.           I    H        L   H
           H         H            Il      H   H   TOGGLE                           $N5472'SN7472나 r바                                           SN54 72 /$＇나74721w1
       Pos,I.Y. mg1': .J                    （2-K3
                              Jl "J2·J3. Ki 래                                      5N54H7215N74H12)J. N)                                       5N54H72/SN74H72I WI
                                                                                   5N541721SN74L721J. Nl                                       5N541721SN741721T)

                                                                                                                                               NC- No ,nt. ,nal ㄷ nneㄷ맬1.n




                                                           ．기JA). J-K FLIP-FLOPS WITH PRESET AND CLEAR
       구6

                       ' 76. ' H76                                               ' LS76
                    FUNCTION TABLE                                           FUNCTION TABLE
                        ~NP1J T`                      OUTPUTS                    *NmJ' `                            .1J' 'uT`
       ＇쵭‘` ' 1   l沚E ^n cL여E              』     K    0     0       PRESET CItE只 CLOCE            』        `         0     0
           L        H          X           x      x   H     L            L   H           x        X        x         *4        ㄴ
          H         I          H           0     0    L     H            H   1           `        `        X         L         H

           L        L          `           X     X    H-     1           L   L           x        `        X        H1         H1         cK     "      뱁       ｀」   Vcㄷ   江1 2 P日    7
                                                                                                                                                      c4 n                           ㄷ1 ·
          H         H         J1.          L     L                       "   H                    1        〔        00
                                                      아， 《）
                                                          o                                                                     o
          H        ㅐ          J`           I4    t    H     L            H   H                    H        〔        H          L        SN5476/5N74761J. N. WI

          H         H         J1.          L     H    L     H            H   H                    L        H         L         H        5N54H76/5N74H761비 N. WI
          H         H         丁l.          H     H    TOGG L [           니   ㅐ                    H        H        n)GG L E            SN54L576/SN74LS7EIJ. N. WI
                                                                         H   H           H        겨        ㅈ        0() %




                                                                                    267

===== PAGE 283 =====
TYPES SN5483A,SN54LS83,SN7483A, SN74LSB3
4-BIT BINARY FULL ADDERS

                                                                     .1 0R N DUAL-IN-LINE
                                                                OR W FLAT PACKAGE (TOP VIEW)



                                                           B1        La      〔,      c.        G'VO           B1        ^ `        i ]


                                                       -
                                                           1i - 15 = 14 m n m `2 - "                                -
                                                                                                                        札 m ,            -


                                                    ㅣ
                                                    I ■■■■■■■I -

                                                      -                                                                       1-
                                                                 14          c'      c0                       . 1       ^1

                                                                B·                                                            =1


                                                                04                                                            a?


                                                           II    [ ]          A3     B〕                       12        B2


                                                       -UU. .■■U. U-
                                                                         2    3      *             `          '          7         1
                                                           A'        工〕      ＾〕      B]            v｛工   【 2            B7         ^2




                                                                                                              w                                                                            J OR N
CIRCUIT TYPES. SN5486,                                                            FLAT PACKAGE (TOP VIEW)                                                                DUAL-IN-LINE PACKAGE (TOP VIE WI
SN7486 QUADRUPLE 2-INPUT
EXCLUSIVE-OR GATES                                              @) (D ([D 巨）匣）C) (D 』“l戶lF기Jㅠlf而lf,l仄－
                                                                             n:：丁rㄱ
                                                                     I        I_ _        I         - 1_ __L                  __I_           _             I

                                                                니
logic                                                            -
                                                                             i큐귀
                                                                                ㅣ             L_                              n-
                                                                                                                                   -/             -
                                                                                                                                                      ㅗ』
                                                                                                                                                                    길 易」n48J\
              TRUTH TABLE                                       "I t二＝=1- r -- - 1=-
                                                                                                         「和                              ㅣ＇ //1筐놈 咫） d
                                                                                                                                         ==＝」I
                                                                                                                                                      一
        A
            INPUTS
                  B
                        OUTPU니
                          Y                                     ① 巨）(i:) α）① ① (Z) ㄴ1샤t긴
                                                                                       ＂J끄flJIiTh
        0         0            0
        0         1            1
        1         0            1                                positive 沁gic: Y = ^ o B
        1         1            0




TYPE SN7489                                                                                                                                    J OR N DUAL-IN- LINE
                                                                                                                                         OR w FLAT PACKAGE (TI긔）VIEW)t
64-BIT READ/WRITE MEMORY
                                                                                                                                                 5EL EㄷT m1PU巧                  {)＾ㅜA   또N5E     .^1A          드E卜1또
                                                                                                                                                           _J '_    __   _ _\   sLut    OuTput   p4eur        OUTPUI
                                                                                                                                        f_       __
                                                                                                                              ,,


                                                                                                                    - 16 , 15 ,. 14 콘 13 뻐 12 . " - 札 m 숄 .-
                                   FUNCTION TABLE
                                                                                                                                             B                 c         D      .4
                                                                                                                                                                                          ㅗ
                                                                                                                                                                                         ｀』       . 3

             ME   wE   OPERATION          CONE기TION OF OUTPUTS
             L    L    write             Complement of Data Inputs                                                                 ^                                                                     `]

             L    H    Re繃               Complement of Seleoted Word
             H    L    Inh,b,t Storage   Complement of Data Inputs                                                                       ME                    nE        . `     `1       D2      $2



                                                                                                                                                                                 ㅜ                早
             H    H    Do Nothing        비gh                                                                                             Il                    tL


                                                                                                                    -      ` ㄴ 2 . 3 뻐 4 ' 5 H 6 ` 7 - 8 '-
                                                                                                                         衢；:=: 업므寸＝=/ ：첩’，零 갇．
                                                                                                                                             :;"，
                                                                                                                                               ．磊.’측 .땅뱐：
                                                                                                                                                        , "' "


                                                                                      268

===== PAGE 284 =====
CIRCUIT TYPES. SN5490. SN7490
DECADE COUNTERS
                        』.Ft N
           DUAL.IN.LINE PACKAGE (TOP VIEW(                                                                                                 TRU꺼 TABLES
        l NPu ㅜ                                                                                          BCD COUNT SEQUENU
           A    NC   A     D   (aND 8    C                                                                    S.. Not. 1)                                   RESET, COUNT 峰cc Note 2)




       i日，·；,,I-雹
              '4            1] 「교 "               m          9            B                          COUNT
                                                                                                              0
                                                                                                                   ㅇ TPUT
                                                                                                                   C      8 A
                                                                                                                                                              RE5r ＂나PUㅜ｀    0u＂려J'
                                                                                                                                                                                     D C 8^
                                                                                                       0      0    0    （〕  0                             80)1) 80)2) 홧9n] R9'2]
              -
                                                       --
                                                                                                       1          0         0          0        -           `       1    0       S   C 0G 0
                                                                                                       2          0         0          1        0           `       ]    x       0   0 000
                                                                                                       3          0         0          '        1           x       x    1       I   I 00 1
                                                                                                       4          0         ㅣ          0        0           x       0    x       0   COUNT

                                                                                                       5          0           1        0    ㅣ               0       x    0       x      니ㅜ
                                                                                                                                                                                     COU！
                                                                                                       6          0           1        `        C           0       x    x       0   COUNT
                  WI-                                                --




                             2      3       4     5          6 J」                                      7           0          `        1        `           x       0    0       x   COUNT

                                                                                                       8           】        0          0        0         Nc    ＇寸‘) 1n히
                                                                                                                                                                       ＇n'   c   1`＾吐don
         INPUT 8CII)
                 m p0(2)                    NC   "CC        89( () 89(a                                                                         `
         縕m
                                                                                                       9           `          0        0


                                                                                                 NOTES:      I.   Outoot ^ connactid h) input ..                   ＇야 日CO eetaflt.

                                                                                                             2. x lndlc.tfl thet .1Ot.re I에1O.1 1 or · 1에Ical 0 may
                                                                                                                  be pr.tant.




TYPES SN5496, SN54L96. 5N7496, 5N74L96
5-BIT SHIFT REGISTERS

                                                                                         FUNCTION TABLE
                                                                          INPUTS                                                       OUTPUTS
                                                 PRESET                   PRESET
                                     CLEAR                                                    CLOCK SERIAL             OA         O8       OC       OD      OE
                                                 ENABLE          A        B   C     D     E
                                        L          L             x        x   x      x    x      x           x          L          L        L        L         L
                                        L          x             L        L   L      L    L      x           x          L          L        L        L         L
                                        H          H             H        H   H     H     H      x           x         H          H        H        H          H
                                        H          H             L        L   L     L     L     L            x         OA0 O80 OC0 아）
                                                                                                                                    () QE0
                                        H          H             H        L   닉     L     H     L            x         H          QB0      H        QD0        H
                                        H          L             x x x x x                      L            x         OA0 O80  C0 QoO OE0
                                        H          L             x x x X x                       t           H          H  OAn O8n 0cn ODn
                                        H          L             x x x x x                       '           L          L         OAn O8n OCn 00n

                        H = higti level (Steady StateL L = mWIcy이 (steady state)
                        x = irrelevant (any input, including transition引
                        ' = transit. . from mw t. m9h level
                        《그AC, QB0』·＇ㄷ = th. level of Q A' Qg. etc. respectively before 卄｀· indicated steady-stat, input conditions weFe established
                         OAn, QB',; etc = the level 이 0 A. Og. etc. respectively betor. the moat-recent ' treniltion .' the clock




                                                                                  '96 . . . J. N. OR W PACKAGE
                                                                                   'L96. . .JORNPACKAGE
                                                                                             (TOP 써EW)

                                                                                     OUTPUTS                      OUTPUTS




                                                                                                       vcc     D  E                P0(50r
                                                                                                             ,--,－걀               EN'\BLL
                                                                                                                  PR E sE T


                                                                                  paoitine Iogic: see function table




                                                                                                269

===== PAGE 285 =====
                                                                                                                                                                                            MONOSTABLE MULTIVIBRATORS
       121
                           FUNCTION TABLE                                                                                                                                                                                             崑血上世j立苾극
           mPUTs   ·OUTPUTS




                                                                                                                      LLLA끄nR
                                                                                                                                                       6




                                                                                                                                                       HHHHuVvVv
        Al  A2   B   a




                            x L x H ,H ,x L
        L x x H H , ,L x
                                                                      H H LXH HH
                                                                                                                                                                                                                                      뇨펴.
                                                                                                                                                                                                                                      멱IJ{
                                                                                                                                                                                                                                       S
                                                                                                                                                                                                                                                弓균｛고긍
                                                                                                                                                                                                                                           J1LhEHif琶苞
                                                                                                                                                                                                                                          .c Al A? S 0 000
                                                                                                                                                                                                                                      SN5412115N74121)J. N. WI
                                                                                                                                                                                                                                      SN54L121/5N74L121)J, N. TI
                                                                                                                                                                                                                                       121     F키01 = 2 kl) NOM
                                                                                                                                                                                                                                      'L121 ' ; A,,,1 = 4 k!l NOM

                                                                                                                                                                                                                                       Nc             N. t n?t,00ltofl,,ect On

                                                                                                                                                                           RETRIGGERABLE MONOSTABLE MULTIVIBRATORS WITH CLEAR
       122
                                      FUNCTION TABLE
                                    'N'uT$                                                                                                             OUTPUTS                                                                         f1。  -   -.?          _ r A_   ?   - -'




                                              Al *2 SI 52                                                                                               0                   0
                                                                                                                                                                                                                                      n1I
                                                                                                                                                                                                                                                                      기1
                                                                           x H X x X x , L L L




                                                                                                 x , L X H ' H H * H H H H H H
                                                                                                                                 X x X L H H ! H H 二
                                              X ∥ x x L L L X x x H
                                                                                                                                                                            H H H H HU U
                                                                                                                                                                                                                                                       =D,
                                                                                                                                                          LLLnn Lnn八nn
                                                                                                                                                                     끄 n
                                                                                                                                                                                                                                      인Hi小f{j珏；죠ㅍ｛：구


                                                                                                                                                                            ㅐU U U U Uv v
                                                                                                                                                                                                                                       SN54l22fSN74l22)J. N. w}
                                                                                                                                                                                                                                       SN54L122/SN74L122(J. N. 1)
                                                                                                                                                                                                                                       j22    fl ,,, = 10 ku NOM




                                                                           1 1H X L
                                                                                                                                                                                                                                        L122  . 1키ft = 20 k11 NOM
                                                                                                                                 H H


                                              * ㅎ! X
                                                                                                                                 " H




                                                                                                                                                                                                                                       NC -No ,n,e,nal C Onvec non




 TYPE SN74141                                                                                                                                                                                             JON N DUAL-IN LINE                                                      FUNCTION TABLE
                                                                                                                                                                                                     OR W FLAT PACKAGE 1 TOP VIEW)
:BCD-TO-DECIMAL DECODER/DRIVER                                                                                                                                                                          머＇'PU'S                   0u! Pu' s
                                                                                                                                                                                                                                                                                 T= NPUT                   OUTPUT
                                                                                                                                                                                                     -m→   －-,.｀        。。。   〃－→－-
                                                                                                                                                                                                                                                                                 「n C ' B ^                    ONt
                                                                                                                                                                                                                                                                                      十     +  r           -
                                                                                                                                                                                                                                                                                  L       . :L   L              0




                                                                                                                                                                                                                   즌硼，
                                                                                                                                                                                                     言＝亡 4ㄱ，÷ " ' 슥． ∥
                                                                                                                                                                                                                                                                                  닐H
                                                                                                                                                                                                                                                                                                   旴
                                                                                                                                                                                                          P이'liv, ～四'C; see trum table
                                                                                                                                                                                                                                                                                                   m
                                                                                                                                                                                                                                                                                  H H
                                                                                                                                                                                                                                                                                          -4   L       H       NONE
                                                                                                                                                                                                                                                                                          H    H       L       NONE
                                                                                                                                                                                                                                                                                          H    H       H       NONE

                                                                                                                                                                                                                                                                                 H - h,gh level L - low level
CIRCUIT TYPES, SN52741. SN72741                                                                                                                                                                                                                                                  t ^＇· .n, e
                                                                                                                                                                                                                                                                                           『 .｀』1p`J1` are 이＇
                                                                                                                                                                                                              JOR N DUAL-IN-LINE
0PERATIONAL AMPLIFIERS                                                                                                                                                                                        PACKAGE (TOP VIEW)




                                                                                                                                                                                                           F1巨l皿1듀1IEif,－丁rLㄱ




                                                                                                                                                                                                     NC   N. ' nlernal coon口
                                                                                                                                                                                                                           「t'0"


                                                                                                                                                                                                      270

===== PAGE 286 =====
                                                                             Appendix E



Glossary of Logic
and lntegroled-(ircuil
Terminolo9y


Access Time. Time required to obtain information stored in a memory.
Accumulator. Section of a computer which performs the operation of addition and stores the sum.
A/D Converter. Analog-to-digital converter. Circuitry that converts an analog voltage or current to an equivalent
     digital output.
Adder. Circuitry that performs the operation of adding two numbers.
Amplifier. Circuits that increase the amplitude and power level of an incoming signal.
Analog Switch. In D/A conversion, the circuitry that switches the binary information into the summing circuitry.
AND. Logic function whose output is a I when a끄 inputs are equal to 1.
Astable Multivibrator. An oscillator having two outputs. The outputs levels are-complementary; when one output is
     mgh, me other is low.
Asynchronous Input. Inputs to a flip-flop which affect the output of the flip.flop independent of all other inputs.
Asynchronous Operation. An operation that proceeds independently within a system independent of any clock
     signals.
BCD. Abbreviation for binary-coded decimal. 8421 code is commonly called BCD, although the 8421 code is some-
     times called NBCD. All other codes are referred by their weighting: for example, 4221.
Binary. See Flip-Flop.
Binary-Coded Decimal. A 4.bit binary code covering the decimal numbers 0, 1, 2. . . . .9. Each digit requires a
      grouping of 4 bits.
Bipolar Device. A device in which current flow occurs with both minority and majority carriers. npn and pnp tran-
      sistors are examples of su야i devices.
Bistable. A circuit having two stable states.
Bit. A binary digit, either a 1 or a 0.
Boolean Algebra. The algebraic rules of logic.


                                                       271

===== PAGE 287 =====
Borrow. In subtraction, when the subtrahend is larger than the minuend, a borrow is required from the next more
     significant column.
Breakdown Voltage. The voltage at which a semiconductor device undergoes a sharp change in its current-voltage
     characteristic. There is a -sharp increase in current at this voltage.
Byte. An8bit word.              -
Carry. In addition, when the sum exceeds the radix a carry is generated for addition in the next more significant
      column.
Clear. Set a binary to the 0 state.
Clock. In a digital system, a timing pulse for controlling the timing of operations.
Comparator, Analog. A circuit that compares two analog voltages and indicates which is greater than or less than
     the other.
Comparator, Binary. M arrangement of logic gates for comparing two binary numbers for equality, less than, or
     more than. See also Exclusive-OR.
Complement. (a) The sum of a number and its complement is equJ to one less than a power of the radix.- For
     example, in decimal me 9s complement of 57 equals 42. In binary the is complement of 1 is 0 and 0 is 1.
     Binary Is complements are available from the opposite side of a FF. (b)The sum of a number and its corn-
     미ement is equal to a power of the radix. The I Os corn힌ernent of 57 is equal to 43. In binary the 2s 인？甲pie-
     ment is obtained readily by adding one to the is complement. (c) The inverse of a logic function. A is the
     complement of A.
Complementary MOS. Also CMOS and COS/MOS. A series arrangement of n-channel and p-channel enhancement-
    mode transistors with the drains tied together. The output is taken from the common drain terminal.
Counter. Digital circuitry for counting incoming pulses and indicating the number of incoming pulses by the states
     of output terminal.
Counter, Binary. Count states are represented in binary notation.
Counter, Johnson. See Counter, Twisted-Ring.
Counter, Mod-N. Modified binary counter with N distinct count states. Returns to original state after N pulses are
     counted.
Counter, Ring. A counter with output returned to input to form a continuous ring. One stage of the counter is in
     a different state from all other stages.
Counter, Ripple. A counter in which a count change progresses from one stage to the next so that a change ripples
     through the counter.
Counter, Synchronous. A counter in which all stages change state at an identical time determined by a clock pulse.
Counter, Twisted-Ring. A ring counter in which the state of the input stage is the complement of the final stage.
Diode. Two-terminal device with high conduction in the forward voltage direction and essentially zero conduction
     in the reverse voltage direction.
Divider (Frequency). The output frequency is 1/N of the incoming frequency, where N is the number of different
     count states of the counter before returning to its initial state. See also Counter.
DOT-AND. Logic output of wired collector logic resulting in an AND function. Frequently called Wired-OR.
DOT-OR. Logic output of wired collector logic resulting in an OR function.
DTL. Diode transistor logic.
Exclusive-OR. Digital circuit for two inputs that results in a 1 if one input is a 1 and the other is a 0. If both inputs
      are alike the output is a 0. It acts as a digital comparator, giving a 0 for like inputs and I for nonalike inputs.
FALSE. Equivalent of a 0 or an OFF.
Fan-In. Number of inputs to a gate.
Flip-Flop (FF). A circuit having two stable states. Its state can be changed upon the application of a signal and will
      remain indefinitely in the new state after removal of the signal.
      (a) R-S. Two inputs, R for reset and S for set. When the R input is activated, the FF is placed into the 0
          state. When the S input is activated, the FF is placed into the 1 state. Activating both R and S simulta-
          neously is not allowed.
      (b) T. Upon application of a clock pulse to the T input the FF toggles.
      (c) RST. Combination of R-S and T.



                                                         272

===== PAGE 288 =====
      (d) J-K. Similar to RST, but clocked. J = R, K = S. In addition, when both J and K are activated the FF
          toggles. When J and K are not activated no change takes place when a clock pulse is applied.
      (e) D(Data). Information is presented to the D input in digital form and appears at the output after a clock
          pulse.
Full-Adder. Provides sum S and carry out CO information for three inputs X, Y, and the carry in C1 information
      from the next least significant column. Performs the operation X + Y + C1.
Full-Subtractor. Provides difference D and borrow out B。   information for three inputs X, Y, and the borrow in B
      information from the next least significant column. Performs the operation X - Y - B1.
Gate. Logic operator or circuit.
      (a) AND. Output is 1 if all inputs are 1.
      (b) NAND. AND followed by INVERT.
      (c) NOR. OR followed by INVERT.
      (d) OR. Output is 1if any input is a I.
Half-Adder. Performs the addition operation for the least significant bit and provides the sum S and carry out CO
      for the operation X + Y.
Half-Subtractor. Performs the subtraction operation for the least significant bit and provides the difference D and
      borrow out BO for the operation X - Y.
Hexadecimal. Number system based upon radix 16.
High Level. More positive of the logic levels in a binary system.
Integrated Circuit (IC). An assembly of circuit components intended for operation as an electronic circuit. In a
      monolithic IC, all components are fabricated simultaneously on a single silicon substrate. In a hybrid IC,
      multiple substrates, individual semiconductors, and film components are combined.
INVERT. To perform the NOT function. Provides A when input A is applied.
Isolation Diode. A p-n junction, normally reverse-biased, which surrounds components in a monolithic IC to pro-
       vide isolation from other components. Care must be taken in circuit operation to prevent the diodes from
      becoming forward-biased.
Karnaugh Map. A map for logic equations arranged in a manner so that logic and circuit simplifications become
     readily apparent.
Ladder. In D/A conversion, resistor network for converting binary outputs on a weighted basis.
Latch. A simple R-S flip-flop constructed with either two NAND or two NOR gates.
Logic Delay. Speed of signal propagation through a gate. Frequently expressed as pair delay, which is the delay
      through a pair of inverting gates.
Logic Diagram. A diagram using logic symbols to show the signal flow relationships in a system.
Logic Swing. Difference in voltage between the high voltage level and the low voltage level.
Logic Symbol. Graphic representatioi of basic logic function.
Low Level. More negative of the logic levels in a binary system.
LSB. Least significant bit.
LSI. Large-scale integration. A complex integrated circuit with more than 100 gates.
Master-Slave. A flip-flop with two separate clocked flip-flops. Information is first transferred into the master and
     then information from the master is transferred into the slave.
Memory. Information storage.                                                                                    ;,
Mon이ithic. See Integrated Circuit.
Monostable. Single shot, one shot. A circuit normally in a stable state. Upon application of a signal it is triggered
    into a quasistable state and remains in the quasistable state for a time determined by an RC time constant. It
    then reverts to its stable state.
MOS. Metal oxide semiconductor. Field-effect transistor in which the gate is isolated from the channel by an oxide
    film.
MSL. Medium-scale integration. A complex IC having between 12 and 100 gates.
NAND. AND followed by INVERT.
Negative Logic. The 1 level is more negative than the 0 level.
Nibble. A 4-bit word.


                                                        273

===== PAGE 289 =====
Noise Immunity-Noise Margin. Difference between lo昏c level and gate mreshold voltage. Represents the maximum
      allowable spurious signal beyond M1ich an undesired gate output level can occur.
NOR. OR followed by INVERT.
NOT. See Invert.
Octal Numbers. Number system based upon radix 8.
One Shot. See Monostable.
Operational Amplifier. High-voltage-gain, hi鱗.input-impedance, dc.wideband, amplifier with output voltage level 0
      volts when input voltage is zero. Single-input amplifier is inverting. With dual differential inputs, amplifier
      amplifies differential input.
Pair Delay. See Logic Delay.
Parallel Adder. An adder in which all bits are added simultaneously. See also Serial Adder.
Parallel In-Serial Out. In a shift register, method of introducing parallel information into the register and retrieving
      information in serial form. See also Shift Register and Serial In-Parallel Out.
Parasitic Element. Undesired circuit components. Stray capacitances and lead inductances. In monolithic ICs, the
      isolation diodes.
Parity. Error-checking method applied to a word which checks by counting the number of ls. A parity bit is added
      to convert all words in the system to ODD parity or EVEN parity as required.
Passive. A resistor is used between the output terminal and supply voltage.
Positive Logic. The I level is more positive than the 0 level.
PRESET. See Set.
Pull-Down Resistor. A resistor connected to ground or to a negative voltage.
Pull-Up Active. A transistor is used between the output terminal and supply voltage to lower the output source
      impedance.
Pull-Up Resistor. A resistor cor.nected to the positive supply voltage.
Pulse. rA signal of short duration.
Q Output. Flip-flop output terminal corresponding to the TRUE output.
Q Output. Flip.flop output terminal corresponding to the FALSE output.
Race. A timing conflict that occurs when two signals are coincidentally applied to a logic element.
RAM. Random access memory. A memory in which stored information can be retrieved within a time period inde-
     pendent of the location of the memory element within the memory. See also Scratch Pad Memory.
rRegister. Storage location for binary information.
      Shift. A register in which all information can be transferred one stage at a time by shift or clock pulses.
      Circulating 와iift. A register in which 小e final stage is returned to the first stage so that information circu-
             lates within the register.
 RESET. See CLEAR.
Ring Counter. See Counter, Ring.
Ripple. See Counter, Ripple.
R自pple Counter. See Counter, Ripple.
ROM. Read.only memory. A memory in which information is permanently stored and cannot be altered.
RTL. kesistor-transistor logic.
Scratch Pad Memory. A R M for temporary information storage.
Serial Adder. An adder in which each pair of bits is added one pair at a time. Requires less equipment than the
      Parallel Adder but requires more time to perform the operation.
Serial In-Parallel Out. In a shift register, introduction of information into the register in serial form and retrieval
       of information in parallel form. See also Parallel In-Serial Out.
SET. In a flip-flop, to set into the I state. Opposite of RESET.
Shift. In a register, to transfer all information by one stage upon application of a clock or shift pulse.
Shift Register. See kegister, Shift.
SSI. Small.scale integration. An IC with less than 10 gates.
Strobe. To clock or gate.


                                                          274

===== PAGE 290 =====
Synchronous. A digital system in which all operations occur simultaneously at a time determined by a clock pulse.
Synchronous Inputs. Inputs to a flip-flop which control the output but only after the application of a clock pulse.
     For example,J-K inputs in J-K flip-flop.
Threshold Voltage. Gate voltage at which the output level transfers from Hi鱗 Level to Low Level.
TRUE. ONE state. Opposite of FALSE.
Truth Table. Tabulation of output level for all possible valid input combinations.
TTL, T2L. Transistor-transistor logic.
Turn-Off Time. Delay time after pulse initiation to cut off current in a transistor.
Turn-On Time. Delay time after pulse initiation for transistor current conduction.
Up-Down Counter. Capable of being reversible with respect to its count state procedure.
Wired Collector Logic. External connection of outputs of logic gates, to provide additional order of logic gating.
     Also called Wired-OR, Phantom-OR, Collector-OR. See also DOT-AND and DOT-OR.
Word. A grouping of bits treated as an entity in a computer.
Zener Diode. Diode with operation in the current region beyond reverse voltage breakdown.
ZERO. Logic level opposite to ONE. Equivalent to FALSE.




                                                         275

===== PAGE 291 =====

===== PAGE 292 =====
                                                                             Appendix F



References




TEXTBOOKS


Barna, A., and D. I. Porat. Integrated Circuits in Digital Electronics. Wiley, New York, 1978.
Bartee, nlomas. Digital Computer Fundamentals.4th ed. McGraw.Hill, New York, 1977.
Blakslee, 1. R. Digital Design with Standard MSI and LSI. Wiley, New York, 1979.
Cirovic, Michael. Integrated Circuits: A User's Handbook. Reston Publishing Co., Reston, Va., 1977.
Deem, W., K. Muchow, and A. Zeppa. Digital Computer Circuits and Concepts, 3rd ed. Reston Publishing Co.,
    Reston, Va., 1980.
Gothmann, w. H. Digital Electronics: An Introduction to Theory and Practice. PrenticeH毗 Englewood Cliffs,
    N.J., 1977.
Greenfield, J. PracticalDigital Design UsingICs. Wiley, New York, 1976.
Grinich, V. H., and H. G. Jackson. Introduction to Integrated Circuits. McGraw.Hill, New York, 1975.
Lancaster, Don. CMOS Cookbook. Bobbs.Merrill, Indianapolis, mnd., 1977.
Lancaster, Don. TTL Cookbook. Bobbs.Merrill, Indianapolis. Ind., 1974.
Levine, Morris E. Digital Theory and 什actice Using Integrated Circuits. Prentice.Hall, Englewood Cliffs, N.J.,
     1978.
Strangio, C. E. Digital Electronics: Fundamental Concepts α＇'(/ Applications. Prentice.Hall, En미ewood Cliffs, N.J.,
      1980.
Tobey, G., J. Graeme, and L. Huelsman. Operational Amp!ifiers-Design and쟈,plication. McGraw-Hill, New York,
      1971.
Tocci, Ronald J. Digital Systems: Principles and Applications. Prentice.H毗 Englewood Cliffs, N.J., 1980.
Wakerly, J. Logic Design Using Standard Integrated Circuits. Wiley, New York. 1976.




                                                       277

===== PAGE 293 =====
TECHNICAL PUBLICATIONS


Fairdmd Semicond1J.t0r
     APP-107 Diode Transistor Micrologic.
     Linear Integrated Circuits, Applications Handbook.
Motorola Semiconductor Products, Inc.
     AN-235     Using the Motorola MDTL Line of Integrated Circuits.
     AN-262A Decade Counters Using MDTL Integrated Circuits.
     AN.284 MDTL K〕Shift Registers.
     AN.409 MDTL Multivibrator Circuits.
     AN.464 MTFL Designer's Note-The MC4004/MC4005. A 16.Bit Random Access Memory.
     AN.707 Noise Immunity Comparison of CMOS versus Popular Bipolar Families.
     AN-768     CMOS Schmitt Triggers.
      &N.772 CMOS Monostable Multivibrators.
     McMOS Handbook.
National Semiconductor
     AN-20 Applications Guide for Operational Amplifiers.
RCA
     COS/MOS Integrated Circuits Manual
Texas Instruments
     CA.102 TTL Integrated Circuits: Counters and Registers.
     CA.112 Logic Design with Series 54/74 Gates.


TECHNICAL ARTICLES


Garrett, Lane S. "Integrated.Circuit 以gital Logic Families."
     IEEE Spectrum, Oct. 1970, Part 1, pp. 46-58.
     IEEE Spectrum, Nov. 1970, Part 2, pp. 63-72.
     IEEE Spectrum, Dec. 1970, Part 3, pp. 30-42.
      A compr랴iensive summary and comparison of the di瘢tal logic families.




                                                      278

===== PAGE 294 =====
                                                                 Appendix G



K Socket,
Switch Bank,and Equipment




This appendix gives the Construction details of a laboratory IC socket and switch bank for use in
the experiments of the manual. The socket is a 16-pin dual-in-line socket and is used with both the
14-pin and 16-pin ICs used for the experiments.
      To minimize damage to the IC pins when extracting the ICs from the socket, use the AUGAT
dual-in-line extractor tool TI 14-I.
      The POMONA banana plug patch cord series Model B mates with the five-way binding'posts
and are stackable. The 8-in, length is the most useful for intersocket connections and for discrete
components. The 4-in, length has limited usefulness and can be used only between adjacent pins.
The 12-in, length is needed for the more complex setups. For connections to power supplies, the
CRO, signal sources, and other equipment, lengths up to 60 in. are available. Model HB is an ex-
tension stacking series that can be used for extension to longer length. Pomona also has available
five-way binding posts to BNC and double binding posts to BNC adapters.
      The CRO used for the experiments should be a triggered sweep CRO. A dual-beam or dual-
trace CRO, although not essential, can be helpful in the analysis of sequential patterns.
      Many of the experiments require a pulse generator or square-wave generator (SWG) with
positive-going output and voltage capabilities up to +5 V. The frequency range is from 1 Hz to
approximately 50 kHz. Single-pulse capability is essential. The output impedance can be between
50 and 500 `7. If the generator output goes both positive and negative, the negative portion can be
clipped with a small-signal diode, Care must be taken to ensure that the positive-going voltage
applied to the IC does not exceed Vcc at any time.
      Several experiments require an audio oscillator.
      Power supply requirements can be found in the individual experiments. The supplies should
be well regulated and have low RF output impedance to minimize interaction and noise generation.


                                               279

===== PAGE 295 =====
LABORATORY IC SOCKET




                         -
                                                                                                                         `，띨＼ 尸ㅡ
                                                             ＝
      ·                                                          ㅢ
                                                                                                             H
                                                             띨
                                                             ｀
                                                             ㅡ                                               -
                                                                 ―
                                                             =




                       ， ㅗ ： 寸 丙 *,^I` ，
                                       寸＼ m1*+,', ｀ 寸 丙 ＋ㅗ
                                                             -




                                                             -
                   !
                   i
                   尸
                                                                                                                                   - ^ m
                                                                                                                                       \" ㄴ
                                                                                                                                          0 N寸杜   니으0= "
                                                                                                                                                                                    …
                                                                                                  T罷七0mㅇ l
                                                                         T
                                                                             ～
                                                                         ㅇ
                                                                             그
                                                                     느
                                                                     口8一
                                                                       L커
                                                                         ㅇ
      ,                                                                  미
                                                                                                                                                                                          -




                                                                                                                                                                                              一m一…

                                                                       1                          卜
                                                                     믄
                                                                     ○
                                                                                                                 一0山 c
                                                                                                                                                                                              小
                                                                             l
                                                                                 α
                                                                     -

                                                                                 1
                                                                                 1
                        m
                        *H4
                          J
                          뉵＼m
                            +
          J ㅋ *1： m*

                     ＼뉵
                ＼寸
                                                                                                                                                                                           PARTS 니ST
                                                                                                                                                                      i             IC Socket Augat No. 316-AG3A
                                                                                                                                                                                    Jermyn No. A1229AM



                                                                                                                                                                      ^b ^z n, ^/




                    ·
                    1
                                                                                                                                                                .`1
                                                                                                                                                                                    5-Way Binding Posts
                                                                                                                                                                                    RH #2 Machine Screws x'/2'
                                                                                                                                                                                    #2 Hex Nuts




                                                                                     으ㅇ 工 0 ： 인
                                                                                                                                                                                    #2 Lock Washers
                                                                                                                                                                ~
                                                                                                                                                                d
                                                                                                                                                                                    Aluminum channel 8"x2'/2"xl '/2"x
                                                                                                                                                                                    1/8' , #6063T5 or equivalent
                                                                                                                                                                                    Peter Frassee, Inc.
  '                                                                                                                                                                                 17 Grand St., New York . N.Y. 10013
                                                                             24"
                                                                                                                                                  H
                 Note - Mount socket below.




                                                                                                                                                           2羽

===== PAGE 296 =====
SWITCH BANK



  1




                                      PARTS 니ST
                        7   5-Way Binding Posts
                        5   SPDT Toggle Switches
                            Cutler-Hammer 8Z82K14 or equivalent
                        1   Aluminum channel 8"X2Y2"xl '/2"x
                            1/8" #6063T5 or equivalent
                            Peter Frassee. Inc.
                            17 Grand Street, New York, N.Y.
                            10013

  '

      H_      ㅢ


                  281

===== PAGE 297 =====
-

===== PAGE 298 =====


