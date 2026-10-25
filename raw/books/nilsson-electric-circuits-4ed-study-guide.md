---
source_url: /run/media/yutae/Data/해답_ElectricCircuits.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 0be60197923314b7cb132917ba5d4307e91bf48c181c3cb905c8917ae83d56ea
---

# Electric Circuits (4th ed. Study Guide) (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출. 일부 토큰은 원서 원형과 미묘히 다름 (인식 오류 아님, text-layer 원본). 원문 PDF 로컬 대조 권장.

## Book metadata
- title: Electric Circuits (4th ed. Study Guide)
- authors: James W. Nilsson
- edition: 4th ed. study guide
- year: 1993
- pages: 441

## Original text (all 441 pages)

  James W. Nilsson
    Study Guide
ELECTRIC CIRCUITS
    FOUR자-I EDITIO／니




                       =a
                   FOURTH EDITION


             STUDY GUIDE

ELECTRIC CIRCUITS
               James W. Nilsson
                 Professor Emeritus
                Iowa State University




                              A
                             VT
    ADDISON-WESLEY PUBLISHING COMPANY

  Reading, Massachusetts· Menlo Park, California · New York
 Don Mills, Ontario · Wokingham, England' Amsterdam · Bonn
 Sydney · Singapore ' Tokyo. Madrid · San Juan · Milan · Paris
C叩舛ght @ 1993 by Addi羽n-We없ey Publi帥dng Company, Inc.

All rights reserved. No part of this publication may be reproduced, stored in a re七ieval
system, or transmitted, in any form or by any means, electronic, mechanical, photocopying,
recording, or otherwise, without the prior written permission of the publisher. Printed in
the United States of America.

ISBN 0-201-52700而

12 345 6 78 9 10-AL- 96959493
To the Student

This study guide was written to accompany Electric Circuits, Fourth Edition; its goal is to give
you additional insight and experience in solving circuit problems.

The study guide contains illustrative drill exercises and problems that are similar to but not
identical to the drill exercises and problems in the textbook. A discussion of each solution is
given so that you can trace the analysis of the problem at hand. Hopefully these discussions
will also help you develop and sharpen your own skills so that you can solve other circuit
analysis and design problems. I have endeavored to select a good cross-section of
representative drill exercises and problems that illustrate the range of skills needed to
successfully analyze circuits.

A selection of supplementary problems is provided for each chapter as well; these are in
addition to the problems available in the text itself. They will give you additional practice in
problem solving. S이utions to the supplementary problems are printed at the back of the
study guide so that you can check your work.

I hope this manual will help you approach circuit analysis from the point of view of
understanding the fundamental principles involved and at the same time steer you away
from the "let's plug into an equation and see if it works" approach.

                                                                                  J. W. Nilsson




                                                                                             111
                                   Coi毗ents


Chapter 1     Circuit Variables                             1

Chapter 2     Circuit Elements                              9
Chapter 3     Simple Resistive Circuits                     21
Chapter 4     Techniques of Circuit Analysis                35
Chapter 5     Topology in Circuit Analysis                  57
Chapter 6     The Operational幻plifier                       69
Chapter 7     Inductance and Capacitance                    87
Chapter 8     Response of First-Order RL and RC Circuits   101
Chapter 9     Natural and Step Responses of RLC Circuits   133
Chapter 10    Sinusoidal Steady-State Analysis             149
Chapter 11    Sinusoidal Steady-State Power Calculations   167
Chapter 12    Balanced Three-Phase Circuits                181
Chapter 13    Mutual Inductance                            195
Chapter 14    Series and Parallel Resonance                209
Chapter 15    Introduction to the Laplace Transform        227
Chapter 16    The Laplace Transform in Circuit Analysis    243
Chapter 17    The Transfer Function                        263
Chapter 18    Fourier Series                               281
Chapter 19    The Fourier Transform                        303
Chapter 20    Two-Port Circuits                            321
Solutions to Supplementary Problems                        341




                                                             V
                                       Chapter 1
                                    Circuit Variables


Part A: Representative Drill Exercises with Solutions

Drill Exercise 1.1
The current at the terminals of the element in the accompanying figure is

         i= O,       t< O;


          i= ic匕-2어恥A,         t之a

Calculate the total charge (in microcoulombs) entering the element at its upper terminal.


                                      V




Solution

Since i = dq/dt it follows that idt = (dq/dt) dt = dq.
Therefore




or




            = 尸. lOe크띠ydt = 50(刃／sC.
                 U




                                                                                            1
 2                                                                               Chapter 1/Circuit Variables



 Drill Exercise 1.2
 Assume the voltage at the terminals of the element in the figure corresponding to the current in Drill
 Exercise 1.1is

           v= 0,     t< 0;


          p= 5J_2어Xtv,          t之0.

C삯culate the total 口妃rgy (in mill加ules) delivered to the circuit ele毗nt.


Solution
The reference for the current in the figure is in the direction of the voltage drop across the element.
Therefore we use the positive sign in the expression for the power. The expressions for v and i are
given, and hence we have

          p= 0,      t< 0

and

          끄＝Soc匕-4띠yW,            0St5eo.

It follows from the defmition of power that


          W=   f:
                    500e'4여X 'dt = 125     mJ.
Drill Exercise 1.3
A high-voltage direct-current transmission line between Celilo, Oregon, and Sylmar, California, is
operating at 800 kV and carrying 1800 A, as illustrated in the accompanying figure.
       Calculate the power (in megawatts) at the Oregon end of the line and state the direction of
power flow.

                                         1.8 kA


                                       +
                             Celilo.                                S닌mar,
                             Oregon    800 kV                      Calif a rn治
Part B: Representative Problems with Solutions                                                             3




Solution
In determining the power flow in the line between Cello, Oregon, and Sylmar, California, we have
two choices. We can either look toward Sy佃ar or toward Cello. If we look toward Syhnar, we writep
 = vi because the reference for i is in the direction of the voltage 小op across the line. It follows that if
we look toward Cello we must writep = -vi. Either calculation leads us to the conclusion that 1440
MW flows from Celilo to Sylmar.
        Looking toward Sy노lar gives

             r1』
               ＼』1 . . 4r13 . . 4 1l . . 4r\3 4 1 1r1 . . dr16 4 1 1r뇨 1 1111
          p= a只Jx Lu x l· ox LU = 1'l'44ix Lu = i 'i'iuiviw;


therefore Sylmar is absorbing 1440 MW.
       Looking toward Cello gives


          p = -&jo x l03 x 1.8 x 103 = -1恥0MW;

therefore Celilo is delivering 1440 MW.



Part B: Representative Problems with Solutions

Pr야)lem 1.1
A current of 1400 A exists in rectangular (0.6-by-9-cm) copper bus bar. The current is due to free
electrons moviur throurh the bus bar at an average velocity of v meters/second. If the concentration
or tree electrons is itr' electrons per cuDic meter ana II tney are unuormiy wspersea uirougnout mne
bus bar, then what is the average velocity of an electron?


Solution


船쌉덮泮onx滯un。r黑ly2凸鰐叩，黜繫業빻빴客心望恥，뚫：밗各冒‘"
5.4 x i014 square meters; hence the charge per meter is 8.65 x 106 coulombs/meter. The average
charge per second passing perpendicular to the cross-sectional area of the bus bar is

          8.65 x 106 x (average velocity of an electron).
4                                                                                         Chapter 1/Circuit Variables




Since the average charge per second is the current we have

                    . .           .                   1400
          average velocity ot an electron =                                 or 161.814um/s.
                                                   8.65 x 106 '


Pro川em 1.2
The voltage and current at the terminals of an automobile battery during a charge cycle are shown in
the accompanying figure.
       a) Calculate the total charge transferred to the battery.
       b) Calculate the total energy transferred to the battery.

                           v)V)




                                  I   I   1    I      I     I    !                     t(k引
                     (a)     0        4        8           12         16          20
                                                   Vottage vs. time
                           1(A)




                             4

                             2

                                          I    I      I          I    _I_     I        r(k引
                     )b)              4        8           12         16          20
                                              Charging current vs. time

Solution
       a) The charge transferred to the battery is the area under the i versus t plot. Thus


          q = 12.5 x 4 x l03 + 8 x 8 x iO3 + 3 x 3 x 103 = 123,000 coulombs.
          叩＝J12,000pdt= 674.53kJ
          w= f



Part B: Representative Problems with Solutions                                                       S




       b) The total energy transferred to the battery equals the area under the power versus time plot
between 0 and 15 ks. To find this area we must derive the analytical expressions for the power and
then integrate over the appropriate intervals. Note that 小fferent expressions for power result from
the fact that the expression for the current changes during the charging interval.

          v= 9+ 0.2x10e3tV,                     0 5t 515ks


          i= 15- 1.25x10H3tA,                   0 5t 54ks


            =12- 0.5x10e3tA,                    4 5t 5l2ks


            =30- 2x10e3tA,                      12 5t 515ks

            =0,                                 t 2l5ks

          0 5 t 5 4000 s:


          p = vi = 135- 8.25 x 1013t -0.25 x 10H6t2W


          w =   f0mpdt=      468.67kJ



          4000 5 t 5 12,000 s:


          p = vi = 108 - 2.1 x l0H3t - 0.1 x 1o_6 t2 w




          12,000 5 t 5 15,000 s:

               .   八nn      m八 . . d rl-3.   』＼ 1 -. .,-6 . 2 117
          p = VI = 乙／u-     I乙 7( 끄J i-      U.'4. XIU    r w



          叩＝I：蠶p dt= 104.40 kJ
6                                                                           Chapter 1/Circuit Variables



          叩FOT = 468.67 + 674.53 + 104.40 = 1247.60 kJ



Part C: Supplementary Problems

Supplementary Problem 1.1
Two electrical circuits, represented by boxes A and B, are connected as shown in the figure. The
reference direction for the current i in the interconnection and the reference polarity for the voltage
                                                                                                        v
across the interconnection are as shown. For each of the following sets of numerical values, calculate
the power in the interconnection and state whether the power is flowing from A to B or vice versa.

          a)
               i= 15A, v = 20V              b) i= -5A, v= 100V

          c)
               i= 4A, v= -50V               d) i= -16A, v= -25V

                                                   /
                                                  +
                                  A               v              B




Supplementary Problem 1.2
The voltage and current at the terminals of the circuit element in the figure are zero fort < 0. For
t 之 0 they are


          V= 98，어X比中b0ooty, t之0,


          i= 24.5te小1어XyA, t之0.

       a) Find the time (in microseconds) when the power delivered to the circuit element is
          maximum.
       b) Find the maximum value ofp in milliwatts.
       c) Find the total energy delivered to the circuit element in microjoules.
Part C: Supplementary Problems                                                                           7




                                          V




Supplementary Problem 13
The voltage and current at the terminals of the circuit element in the figure shown with the preceding
problem are zero for t < 0. For t 之 0 they are

          V = 1＆
               匕-8& S.
                    sin 6仕V, t 之 0,


          i= 160e中80'sin60tmA, t 之0.

       a) Find the power absorbed by the element at t = 12.5 ms.
       b) Find the total energy (in millijoules) absorbed by the element.


Supplementary Problem 1.4
One method of checking calculations involving interconnected circuit elements is to see that the total
power delivered equals the total power absorbed (conservation of energy principle). With this
thought in mind, check the interconnection in the figure and state whether it satisfies this power check.


                                                                2A


                                                                     d

                                 5                         2A   +    40V        2
                           +                         +

                          60V           。+v        60V




Supplementary Problem 1.5
       a) Repeat Supplementary Problem 1.4 for the interconnection in the figure.
8                                                                            Chapter 1/Circuit Variables



    b) Repeat part (a) if the polarity of the voltage across element d is reversed.

                                -   12V    +           +     28V



                 +
                                      b

                                    2.4A        +
                                                              d

                                                            2.8A
                                                                   1    +     +

               20V       2.4A                  32V   O.4A              60V   60V     4
                                        Chapter 2
                                     Circuit Elem이毗S


Part A: Representative Drill Exercises with Solutions

Drill Exercise 2.1
For the circuit shown, calculate (a) i5; (b) v1; (c) v2; (d) v5; and (e) the power delivered by the 24-V
source.

                                                    2n



                             24V                                         5U



                                                    1U



Solution

       a) Applying Kirchhoff's voltage law around the closed path generates the following equation:

           -24 + v2 + v5 - v1 = 0.

Now use Ohm's law to e血llinate v1, v2, and v5, thus:

           -24+ 2i5+ 5i5- (- ii5) =0.

Therefore i5 = 24/8 = 3 A.

       From Ohm's law we have
       b) v1= -1i5= -3V,
       c) v2 = 2i5 = 6 V,
        d) v5 = 5i5 = 15 V.
        e) The power delivered by the 24-V source can be calculated several ways.




                                                                                                           9
10                                                                         Chapter 2/Circuit Elements



      If we visua血的urselves standii略 to 血아渺t of the sour此 an기00岫rig 的ward 小e source, the
power equation is

               p = - vi = - (24) (3) = 72W.

The mu叫邸油i tells us U妃 source is deliver뇨g 72W.
     If, on the other hand, we look away from the source, the power equation is

              p = vi = 24 (3) = 72W.

The plus sign te小 us the circ毗 to 小釘뇹ht of the source is absorbii娼 72W, w砥沚 毗ans the so毗e
is delivering 72W.
        Finally we calculate the power delivered by the source by summing the power absorbed by the
three resistors, thus:

                  /n\2 ,1 . ／八＼2 尸 . /n\ 2 /4\ ,m八 i1,
              p = (JJ 乙 十 (i) 그 十 （刃 (JJ = ／乙 w.



Drill Exercise 2.2
            The current i   in the circuit shown    in
                                                         fi엣re A is 5 A.
            a) v3;                                         Calculate:
        b) the power absorbed by the independent voltage source;
            c) the power delivered by the independent current source;
            d) the power delivered by the controlled current source;
        e) the total power dissipated in the two resistors.

                                             6id)




                                                                            5A




      (a)
Part A: Representative Drill Exercises with Solutions                                                   11




Solution

        a) Since i中 is known to be 5 A, it follows that 6i中 is 30 A. Kirchhoff's current law can be used to
establish the current in every branch of the circuit. The branch currents are shown on figure B.
        To fmd v, summarize the voltages around the closed path abcd; i.e.,

             v- 20 (5) + 10 (5) =0; orv= 50V.




       (b)

       b) The power absorbed by the independent voltage source equals 10 v5 since the branch
current is in the direction of the voltage drop across v . Thusp = (50)(10) = 500 W.

       c) To find the power delivered by the independent current source first fmd the voltage across
the source. This voltage has been labeled v0 on figure B. Note that v0 is the same as the voltage across
the 10-Q resistor. Thus v0 = (5) (10) = 50 V.
       Now observe that the source current is in the direction of the voltage drop across the source.
Therefore the independent current source is absorbing (5)(50) or 250 W. This is the same as saying
the source is delivering a negative 250 W.

       d) Using v1 to denote the voltage across the dependent current source we have

             v1 =20 (5) = 100 V.

It follows that the dependent current source is delivering 30刃 W to the circuit connected to its
terminals.

        Hint: It is sometimes helpful when deciding on whether a source is delivering or absorbing
power to represent the circuit connected to the source as a box without worrying about the
connections inside the box. Thus when concentrating on the dependent current source we could
visualize the circuit as shown in figure C.
 12                                                                                 Chapter 2/Circuit Elements




                                                    .irw+（刃力nee十e<{ {<>
                           功A                      .4中년．＋巴nn吹1s 口f翔e
                                                     de芦m巴n+ 配／(V帥 f1
                                                         站q比e.


         (c)
        e) The total power dissipated in the two resistors is

               p = (20)2 5 + (5)2 (10) = 2250W.

We can check our calculations by checking to see if the total power absorbed equals the total
                                                                                               power
delivered. In this circuit only the dependent current source is delivering power. The total
                                                                                            power
absorbed is 500 + 250 + 2250, or 3000 W. This agrees with the power delivered by the dependent
current source.



Part B: Representative Problems with Solutions

Problem 2.1
The voltage v0 in the circuit shown in the figure is 60 V. Find (a) i1; (b) vg; and (c) the power
delivered by the independent voltage source.

                                            211                 511
                                                                 W
                                                                        尸＋




                                                       ;,4511
                                                                        呵    1211

                                            311                 111




Solution

        a) Since v0 is given, use Ohm's law to find the current in the 12-Q resistor. This current also
exists in the 5-Q and 1-O resistors; therefore the total voltage across the three resistors is 90 V [i.e.,
5(5) + 60 + 5(1)], positive at the left terminal of the 5-O resistor. This is also the voltage across the
45-O resistor, positive at the upper terminal. Therefore i1 = 90/45 = 2 A.
Part B: Representative Problems with Solutions                                                                   13




,   .   . First use Kirchhoffs current law to fi the current through Vg
            .
                                                                nd
                                                                                     the reference
                                                                                       .   Assume
                                                           ii. INOW use 八lrcnnoiis voitage taw to sum
                b)
utrecuon is up tnrougn tne source; tnen LfliS current is i
the voltages around a closed path that includes 노                    ·



        One such summation is

                       -v뇽 + 2 (7) + 90 + 3 (7) 口 0 ·

Therefore v。= 125 V.

                 c) Standing to the right of the source and looking toward the source yields the equation

                       p = -125 (7) = -875W.

The minus sign tells us the source is delivering power to the circuit connected to its terminals. Thus

                       Pdelivered = 875 W.


Problem 2.2
The voltages v1 and v2 in the circuit in the figure are 480 and -420 V, respectively.
                     a) Find the power supplied by each voltage source.
                     b) Show that the total power supplied equals the total power dissipated in the resistors.

                                                         2 fl



                                        585V

                                                                                      4011


                                        585V




    Solution

          a) Assume 11 is the current in the upper source and i2 is the current in the lower source.
    Assume further that the reference for either i1 or i2 is through the source from minus to plus.
           To find i1 apply Kirchhoff's voltage law around the closed ioop made up of the upper 585-V
    source, the top 2-O resistor, and v1. Thus
14                                                                            Chapter 2/Circuit Elements



             -585 + 2ii + V1 = 0.

 Therefore 2i1 = 585 - v1 = 585 - 480 = 105, or i1 = 52.5 A.
        To find i2 apply Kirchho作s voltage law around the closed ioop made up of the lower 585-V
 source, v2, and the lower 2-Q resistor. Thus

            -585 - V2 + 2s2 = 0;

therefore

            2i2= '2+ 585 = -420+ 585= 165

or

            12 = 82.5 A.

The power supplied by the upper 585-V source is

          Pupper (supplied) = (585) (52.5) = 30,712.50 W.

The power supplied by the lower 585-V source is

          Pupper (supplied) = (585) (82.5) = 48,262.50 W.


        b) To find the total power 小ssipated in the resistors, first find all the branch currents. Let
            a be the current down through the 20-a resistor;
            tb be the current down through the 5-c2 resistor;
            c be the current down through the 40-Q resistor;
and
          i3 be the current in the 中（2 resistor, oriented left to right.
First find i by applying Kirchhoff's voltage law around a closed path where i, is the only unknown;
thus

            - V1 + 4아C + V2 = 0.

Hence

          4位C= v1 - v2 = 900
Part B: Representative Problems with Solutions        15




or

          iC = 22.5 A.

Using Kirchhoff's current law we have

          1a == il m iC = 52.5 m 22.5 = 30A,


          ib = i2 - iC = 82.5- 22.5 = 60A,


          i3 = ib 尸 i口 = 60- 30 = 30A.

Now calculate the power dissipated in each resistor


          P2 Q upper = (52.5)' (2) = 5,512.50 W,


          끄4 Q       = (30）口 (4) = 3,600.00 W,


                wer = (82.5)e (2) = 13,612.50 W,
          P2 Q l。


          P2。52      = (30)2 (20) = 18,000.00 W,


          PSQ        =(60)25= 18,000.OOW,


          끄40Q       = (22.5)2 40 = 20,250 W.

It follows that

           XPdiss = 78,975 W.

 From the calculations of part (a)

           기Pdel = 78,975 W.
16                                                                            Chapter 2/Circuit Elements



Problem 23
       a) Find the voltage v, in the circuit in the figure.
       b) Show that the total power generated in the circuit equals the total power absorbed.

                                            0.75 V            391A
                                 15kfi     ／小＼                /\     0.4kfl




                     7V                                                         12 V




Solution

      a) Using Kirchhoff's current law the current down through the 0.25-kc resistor is '1位A . Using
Kirchhoff's voltage law to sum the voltages around a closed path generates the following equation:

          -7 + '5iA + 0.75 + 40i1 (0.25) = 0

where i is measured in milliamperes (mA). Therefore i A = 025 mA and 39i八 = 9.75 mA.
       Now use Kirchhoff's voltage law to find v,, thus:

          H7 + 15i1 + 0.75 - Vy - 0.4 (39iA) + 12 = 0,

from which Vy = 5.日：1 V.

      b) From the solution to part (a) of this problem we note both independent voltage sources are
generating power and all the other elements in the circuit are absorbing power. Therefore

         Pgen = 7 (0.25) + 12 (9.75) = 118.75 mW,


         Pabs = (0.25)2 (15) + 0.75 (0.25) + 9.75 (5.6) + (9.75)2 (0.4) + (10)2 (0.25) = 118.75 mW.
Part C: Supplementary Problems                                                                    17




Part C: Supplementary Problems

Supplementary Problem 2.1
Given the circuit shown in the figure, find each of the following:
       a) the value of 13;
       b) the value of i6;
       c) the value of v;
       d) the power dissipated in each resistor;
       e) the power delivered by the 12-A source.



                        12A      卜；
                                             3fl     i3           6c!   +,i6
Supplementary Problem 2.2
The currents 1a and 1b in the circuit in the figure are 2 A and -4 A.
       a) Find iC.
       b) Find the power dissipated in each resistor.
       c) Findv.
       d) Show that the power delivered by the current source is equal to the power absorbed by all
          the other circuit elements.

                                                   6fl



                                 j
                                                   八 八 八




                             5 '｝듣


                                       in                   2fl
                                                            vv



                        90V1                   V1111 )AA                       'C1   3O




                                      ii 0                 4O
18                                                                          Chapter 2/Circuit Elements



Supplementary Problem 2.3
The voltages v1, v2, and v3 i口 the circuit in the figure are 2.16, -24, and -2꽈 V, respectively.
       a) Find the power supplied by each voltage source.
       b) Show that the total power supplied equals the total power 小ssipated in the resistors.


                                               ]




Supplementary Problem 2.4
Given the circuit shown in the figure, calculate each of the following:




                                  b 0oy




      a) i1,i2, i3, i4, and i5;
      b) v2, v3, v4, and v5;
       c) the power supplied by the source;
      d) the power dissipated in each resistor.
      e) Does the power supplied by the source equal the total power dissipated?
Part C: Supplementary Problems                                                                   19




Supplementary Problem 2.5
For the circuit shown in the figure, find (a) R and (b) the power supplied by the 30-V source.


                                                                        8O

                                                                       伊
                                                                 \<r

                                                                           怨
                                                                        Y Y Y




                                                     > >>   :,
                                                                                  1.25O

                                                                       0.75O
                                                                        w




Supplementary Problem 2.6
       a) Find the voltage v), in the circuit in the figure.
       b) Show that the total power generated in the circuit equals the total power absorbed.


                                              0.7V                      491A
                                   25kO      ／戶＼\                       /.\     ikfl




                       5.7V                                                               了0v
                                    Chapter 3
                             Simple Resistive Circuits


Part A: Representative Drill Exercises with Solutions

Drill Exercise 3.1
For the circuit shown, find (a) the voltage v; (b) the power delivered to the circuit by the current
source; and (c) the power dissipated in the 10-Q resistor.

                                                  7.2 Il       6n



                            5A                                          10 f




Solution
       a) First find the equivalent resistance connected to the terminals of the independent current
source. Starting at the right-hand end of the circuit, we have 16 ohms in parallel 毗h 64 ohms or
12.8 c. This 12.8-Q resistor is in series with 7.2 Q, which yields a 20-Q resistor. Now the 20 ohms in
parallel with 30 ohms gives an equivalent resistance of 12 C. It follows from Ohm's law that

          v= 5 (12) =60V.

       b) The power delivered to the resistive network is (5) (160) or 300 W. [Note this can also be
calculated using (5)2 (12) or 300 W.]

       c) First calculate the current in the 7.2-Q resistor. Assume the reference for the current is
from left to right. Then

          .          60
          i7.2 = 7.2 + 12.8 = i A.

Now use Ohm's law to calculate the voltage across the 12.8-O equivalent resistor:



                                                                                                         21
22                                                                   Chapter 3/Simple Resistive Circuits




          v12.8 = 3 (12.8) = 38.4 V.

This is also the voltage across the 64-Q resistor, positive at the top. It follows that the current in the
10-Q resistor is


          小6꺾0               =   2.   4 A·

Therefore the power dissipated in the 10-Q resistor is

          Pl。= (2.4)2 (10) = 57.6 W.


Drill Exercise 3.2
In the ohmmeter circuit sho帥, the voltage drop across the 50-1uA ammeter and the internal
resistance of the 1.5-V battery are negligible. The variable resistor R is adjusted to give full-scale
deflection of the microammeter when R is zero.
       a) What is the numerical value of R?
       b) What is the midscale reading of the ohmmeter in ohms?
       c) If the variable resistor R can be reduced to zero, how low can the battery voltage drop
          before the ohmmeter cannot be adjusted to read 0 Q when R is zero?
                                 50 iA
                                             23 ku    A




                   +
                  1.5 V -m                                                             ／구X




Solution
      a) When R is zero, the voltage across the branch containing the 50-MA ammeter is 1.5 V.
Therefore the total resistance in the branch corresponding to full-scale deflection is


          Rt。ta，극和 106=30kc.
Part A: Representative Drill Exercises with Solutions                                                    23



ItfollowsthatR = 30- 23 = 7kg.

. .. .b).When.the ohmmeter re沙．빤望고．닫t.he voltage di띤p acros迪e 프프肛咬으叩75V.
Lixewise tne voi[age crop across 八工 is u. i그 V. I ne curreni mK win oe L) x iuV + (U. />/11) or
68,206.82 4uA. It follows from O뇨ll's law that

                        0.75      106
             R                  x     ! 11O.
             凡＝   =   68.2。6.82

Note that the current in the ammeter is negligible compared to the current in the 11-O resistor. Thus
the resistance in the branch parallel to the branch containing the ammeter determines the midscale
rea小ng, providing it is very small compared to 30 kO.

       c) The minimum value of the battery voltage for a zero-ohm rea面g when R is zero is

              VBB = (23 x 103) (50 x lo_6) = 1.15V.


Drill Exercise 3.3
       a) Use a 스寸o-Y transformation to find the current i in the circuit shown in figure A.
       b) Find v1 and v2. (Hint: Use the circuit that exists after the i- to-Y transformation has been
          made.)

                                                 15 n




                                    24 V                        50 1




       (a)
Solution

       a) Convert the delta connection in the lower right portion of the circuit to obtain the
equivalent circuit shown in figure B.
24                                                                  Chapter 3/Simple Resistive Circuits




                         忍V




       (b)

Using series-parallel simplifications the equivalent resistance connected to the terminals of the 2牛V
source is 24O. It follows from Ohm's law that i = 24/24 = 1A.

       b) Use current division to calculate i1 and j2, thus:



          Ii =     (1)   （針跏＼       ·




and



             72=   (1)   （卦啣A.
It follows directly from the circuit diagram in figure B that

             v1= 4i2+ 201= 3.2+ 20= 23.2V

alld
and

             V2 = 5i1 + 201 = 1.0 + 20 = 21.0 V.



Part B: Representative Problems with Solutions

Problem 3.1
The current in the 15-O resistor in the circuit in the figure is 3 A, as shown.
       a) Find Vab.
Part B: Representative Problems with Solutions                                                          25




       b) Find the power dissipated in the 41-O resistor.
       c) What percentage of the total power delivered to the terminals a, b is dissipated in the 26-O
          resistor?

                                                       26 Ii




                                                                                 15U




                               3.6 U



Solution

      a) To find Vab we start on the right end of the circuit where the current is known and work our
way back through the circuit using a combination of Ohm's law, Kirchhoff's laws, and series-parallel
sin呵坂C欲油好．We reason as follows:
       1.   the voltage across the 30-O resistor is 3(20) or 60 V;
       2.   the current in the 30-O resistor is 2 A;
       3.   the 26-O resistor in parallel with the 104-O resistor can be replaced with a 20.8-O resistor;
       4.   the 20.8-O resistor is carrying 3 + 2 or 5 A;
       5.   the voltage across the 20.8-O resistor is 104 V;
       6.   the voltage across the 41-O resistor is 104 + 60 or 164 V;
       7.   the current in the 41-O resistor is 4 A;
       8.   the current in the 164-O resistor is 1 A;
       9.   using Kirchhoff's current law we find the current in the 3.6-O resistor is 10 A from right to
            left;
      10.   the voltage across the 40-O resistor is 164 + 10(3.6) or 200 V, positive at the upper
            terminal;
      11.   the current down through the 40-O resistor is 5 A;
      12.   the current, right to left, in the 8-O resistor is 10 + 5 or 15 A;
and
      13.   the voltage Vab is 8(15) + 200 or 320 V.

       b) The power dissipated in the 41-O resistor is (164)2/41 = 656 W.
26                                                                             Chapter 3/Simple Resistive Circuits




       c) The power delivered to the terminals a, b tSPab = (320) (15) = 4800 W. The power
dissipated in the 26-Q resistor is


           P26 = (104)2/26 = 416 W.

The percentage of the total power delivered to the terminals a, b dissipated in the 26-Q resistor is
(416/4800) x 100 or 8.67%


Problem 3.2
Two d'Arsonval ammeters are connected in parallel as shown in the figure. Ammeter 1uses a 1-mA,
50-mV movement and has a full-scale reading of 10 mA. Ammeter 2 uses a 1-mA, 100-mV movement
and has a full-scale reading of 5 mA. Calculate the reading of each ammeter.




                             1.6v                                                       196 ci




Solution
m기14 n n H=－二．n1戶‘41 .-Hn!n1.,== hm mr m小小 八1n小 4 :n /=r) \/ 4rl小3/ .-. 1/ 4 1le3\ '14 - r入 nm J 11= n n n . . = . n1md
'Ilie  eauivalent resistance 01 ammeter 1 is (>(J X 10 나/iU X 10 q ) or > sJ. ana tue eauivaient
.-nm!n1,= Hm .J ,,.44=14 ',1.1小 八 !n /mJln 뇨 . .--  \/ -.-'- 3\ 八小 nr｝ 入 -'. '= M 1.4n nm=m4n1nmn nmn ..4 =4n小dLJ 1L,1:=.
resistance     01 계［llmeter 2 is (100 X 10 나／.-> X     10 ') or LU LJ . since the ammeters are in parallel, tneir
equivalent resistance is 4 Q. It follows that the total current in the circuit is 1.6/200 or 8 mA. Using
current division the ammeter readings are calculated to be


            小＝     8   （쁩）     =    6.    4   mA
and


            A2=    8   （읗）     =     1.   6毗
Part B: Representative Problems with Solutions                                                         27




Problem 3.3
A 15-kc resistor is connected from the 150-V terminal to the common terminal of a dual-scale
voltmeter as shown in figure panel (a). This modified voltmeter is then used to measure the voltage
across the 25-kQ resistor in the circuit in figure panel (b). What is the readi띵 on the 6再V scale of
the meter?




                                                                    기11



                                                         Modified
                                                         V이tn杷ter




                                  (b)
Solution
The equivalent resistance of the modified voltmeter with respect to the 600-V terminal is 90 +
(30)(15)/(45) or 100 k(2.
        When the modified voltmeter is connected across the 25-kQ resistor in figure B the voltage
applied to the meter is 1500(20/25), or 1200 V.
       It follows that the current into the 600-V terminal is 1200/100, or 12 mA.
       ［川雎 이玎rent division the n妃ter-movemez址 current is 12(15/4斗 or 4 mA.
        駐nce 5 mA corresponds t야he 600＼岫ark on a un迂orm scah 4 mA쎄1卽e a scale rea面ig
of (4/5)(600), or 480 V.
28                                                                   Chapter 3/Simple Resistive Circuits




Problem 3.4
Resistor networks are sometimes used as volume-control circuits. In this application, they are
referred to as "resistance attenuators" or "pads." A typical fixed-attenuator pad is shown in the
figure. In designing an attenuation pad, the circuit designer will select the values of R1 and R2 so that
the ratio of vWvi has a specified value and at the same time the resistance seen by the input voltage
source Rab has a specified value.
        a) Show that if Rab = RL, then


          샤＝4R1 (시＋凡）

and


           % 까
                      R2
                 2R1 + R2 + RL


       b) Select the values of R1 and R2 so that Rab = RL = 50 (2 and vO/v = 0.5.


                                   r                           켜



                                                                      으
                          EH中m八1＋小，V                                  +

                                   !1                m
                                   1
                                                 /
                                                 <                    V.    등月L


                                                               11口
                          ;＝小그H,                           ,
                                                                      d

                                              Attenuator



Solution

        a) First note that Rab can be expressed as a function ofR1, R2, and RL by straightforward
series-parallel equivalents. Thus

                      凡 (RL + 2R1)
          Rab = 2Rl + R2 +
                           2R1 + RL

By hy山thesis Rab = RL1 ; therefore

                       凡 (RL + 2R1)
                 2R1 + R2 + 2R1 + RL
Part B: Representative Problems with Solutions                                                        29




Now multiply both sides of this equation by (R2 + 2R1 + RL) and simplify to get


         毗 = 4R1 (시 + 凡）·

When Rab = RL the current into terminal a is v1/RL and by using current division the current out of
terminal c is

                        (v. 'l         R1
          '0
                    -   (RJ) R2 + 2R1 + RL
Now since vO = RLiO it follows that

                  yR2
          %= 2Rl + R2 + RL

or

           vO                    R2
               vi       2R1+ R2+ RL


       b) For the given values of RL and vO/v1 we have

          2500 = 4R1 (R1 + R2)

and


          nc=      R2
           '  2R1 + 凡 + 50

Using the second equation above we can express R2 as a function of R1, thus:

          7?2 = 2R1 + 50.

When this expression is substituted into the first equation we generate the quadratic expression

               R              R       2500
                          型
                                       12
                                                 u.
                                             =
                          3
30                                                                      Chapter 3/Simple Resistive Circuits



Solving for R1 yields

           -     -25
                             型
          l 'Ci = H= 1
                     土
                  3          3
Only the positive value is realizable in a passive circuit; therefore

                         Q            ,1    20() 八
                   亞
          R1 =               and      K-, = m=H SJ.
                   3
                                          -  3




Part C: Supplementary Problems

Supplementary Problem 3.1
       a) Find the voltage drop across the 50-O resistor in the circuit shown in the figure.
       b) Find the voltage drop across the 60-O resistor in the circuit shown in the figure.


                                                      30 1




                                   50 L                                   30 1




Supplementary Problem 3.2
For the circuit shown in the figure,
       a) calculate / o;
       b) calculate the power dissipated in the 14-O resistor.
Part C: Supplementary Problems                                                                      31




                             33 V                                        14 {I




Supplementary Problem 3.3
The current in the 2-Q resistor in the circuit in the figure is 8 A as shown.
       a) Find the voltage Vab.
       b) Find the power dissipated in the 20-Q resistor.
       c) Wha印ercentage 可the t야alpo＼叱r delivered to the ter的姐ls 斗 b is 曲如ated in the 2-Q
          resistor?

                                                            3 {2




                                                                          2n




Supplementary Problem 3.4
       a) Calculate the current i in the circuit shown in the figure.
       b) What will the 10-mA ammeter of Example 3.4 read if it is inserted in series with the voltage
          source?
32                                                                 Chapter 3/Simple Resistive Circuits



       c) Repeat parts (a) and (b) for the circuit panel (b) of the figure.
       d) Why is it important to know how much resistance in panel (b) of the meter inserts into the
          circuit?



                               90 mV



                               (a)                    (b)




Supplementary Problem 3.5
A d'Arsonval ammeter having a full-scale reading of 100 mA is used to measure the current in the
3- 2 branch in the circuit shown in the figure. The d'Arsonval movement is rated 10 mA and 100 mY.
       a) What is the a帥妃ter readi叩？
       b) What is the current in the 3-Q branch with the ammeter removed?
       c) What is the percent error in the measured current based on the actual current?


                                             600 ((




Supplementary Problem 3.6
The voltage divider circuit shown in the figure is designed so that the no-load output voltage is
six-tenths of the input voltage. A d'Arsonval voltmeter having a sensitivity of 1000 Q/Y and a f네［-scale
rating of 30 V is used to check the operation of the circuit.
       a) What will the voltmeter read if it is placed across the 25-V source?
       b) What will the voltmeter read if it is placed across the 15-kQ resistor?
       c) What will the voltmeter read if it is placed across the 10士Q resistor?
Part C: Supplementary Problems                                                                    33




      d) Will the voltmeter readings obt面ed in parts (b) and (c) add to the reading recorded in
         part (a)? Explain why.




Supplementary Problem 3.7
A multirange voltmeter consisting of a 200-mV, 10-mA meter movement and three resistances, R1, R2,
and R3, is sho帥 in the figure. The desired voltage ranges are 15 V, 150 V, and 300 V. The 15-V,
150-V, and 300-V terminals are as shown.
       a) DetermineR1, R2, and R3.
      b) Assume that a 1500-Q resistor is connected between the 15-V terminal and the common
         terminal. The voltmeter is then connected to an unknown voltage using the common
         terminal and the 300-V terminal. The voltmeter reads 250 V. What is the unkno팎n voltage?

                                                       300 V




                                                       150 V




                                                       15V




                                                       Corn rnon
 34                                                                   Chapter 3/Simple Resistive Circuits



 Supplementary Problem 3.8
The figure shows two possible ways of connecting a voltmeter and an ammeter in order to determine
the unknown resistance Rt. State which method of connecting the voltmeter and the ammeter you
would recommend if you knew the following:
           The meters are d'Arsonval types with movements rated at 1 mA and 50 mV.
           The voltmeter is designed to read 300 V at full scale.
           The ammeter is designed to read 5 mA at full scale.
           The supply voltage is 150 V.
           The resistor is known to be greater than 50 kQ.
           The power rating of the resistor is 0.5 W.
      J出的your answer by show旽 出e error ar帥평 in each 毗比Lod for (a) 凡 = 50 k(2 and
(b) R = 100 kQ.




                     Method 1                            Me hod 2




Supplementary Problem 3.9
For the circuit shown in the figure, find (a) i1, (b) i2, (c) v, and (d) the power supplied by the current
source.



                                              4n
                                              vvv-

                                                     m
                                                     <




                                             n n A
                                                                                 24 fl
                                          Chapter 4
                                 Techniques of Circuit Analysis


Part A: Representative Drill Exercises with Solutions

Drill Exercise 4.1
Use the node-voltage method to find v in the circuit shown in the figure.

                                                                 6O      2O             411
                                                             1H＝小＼      \/＼人



                     4.5 A                                    111
                                                                               3 1211         30 V




Solution

Select the lower node in the circuit as the reference. Define v1 as the node voltage across the 1-Q
resistor, positive at the top. Define v2 as the node-voltage across the 12- 2 resistor, positive at the top.
The two node-voltage equations are
            브
                     V       e
                                 V
                                                             0                                            +=
                             8
                                                                                                          1
                                                 <
                                         4
                                             1
                                                     U
                l
                쁘b   v2- 30 . v2- v1                                n                                              +
                         .           十                   n    = U.
                         4                               8



Solving the two simultaneous equations yields v1 = 6 V and v2 = 18 V. It follows that the current
away from node 2 through the 2-Q resistor is

          i2 = (18- 6) 18 = 1.5A.

Therefore the drop across the 2-Q resistor is 3 V and v = v2 - 3 = 18 - 3 = 15 V.




                                                                                                              35
36                                                                           Chapter 4/Techniques of Circuit Analysis



Drill Exercise 4.2
Use the node-voltage method to fmd v1 in the circuit shown in figure A.

                                                           15佃

                                                         \7/

                                             25f                              40n
                                             w            1+
                                                               [
                        150 V                            <<<111    三80
                                                                         1                 33 f3

                                                          비


        (a)
Solution

The reference node along with nodes 1, 2, and 3 are shown in figure B. Note that v2 is a known voltage
(150 V) and the dependent voltage source places a constraint




                                                                             如Jt
                                                                             小人／


                        1요키／                                                    晦

        (b)

between v2 and v3; i.e., v3 = v2 - (150 - lsi中) = 150 - 15i中 . Therefore v1 can be found by writing a
single node-voltage equation at node 1, namely


               h而   Vi - 150        v1 - (150 小 15i中）
                      25        +          40           =U,

where

               .   150 小 V1
              i中 =    25
Part A: Representative Drill Exercises with Solutions                                             37




Solving for v1 gives v1 = 120 V.


Drill Exercise 4.3
       a) Use the expression b - (n - 1) to determine the number of mesh-current equations
          needed to solve the circuit shown in figure A.
       b) Repeat using bC = (nC - 1).
       c) Use the mesh-current method to find how much power is being delivered to the dependent
          voltage source.


                                                    3v小




                                       25 V                            n




       (a)
Solution
     a) There are 8 branches and 6 nodes; therefore the number of mesh-current equations is
8- (6- 1),0r3.

       b) There are 6 essential branches and 4 essential nodes; thus the number of mesh-current
equations is 6 - (4 - 1), or 3.

       c) A set of mesh currents is defined in figure B.



                                                                札N 4
                                                                  皿/
                                                          口

                                          口
                                                                  P
                                                                  m
                                                              'V"/
                                                               3J2m


                            I      '   느 "    oVC
       (b)
38                                                               Chapter 4/Techniques of Circuit Analysis




The mesh-current equations are

             -(- 3v41) + 1411+ 2 (i1- i2) +3 (i1- 13) =O,


             -25+ 2 (i2- i1) +5 (i2- 13) +10= O,


             -10+ 5 (i3- i2) +3 (13- i1) =O.

The constraint equation is

             Vt, = 3 (j3 - i1) .

       To fmd the power delivered to the dependent voltage source we need the values of i1 and v中.
Since v1, = 3 (i3 - i1) , our problem reduces to fmding i1 and i3; i.e.,

             p3『中 = 小 (- 3v中）il = 9i1 (i3 - i1) ·

The solutions for i1 and i3 are i1 = - 1A and i3 = 3A; therefore

             p3『中 = 9（中1) (4) = -36W ·

The 岫毗 sign tells 出 the dependent voltage soi玎ce is d吐叱ring 36 W to 由毗ircuit connected t이ts
terminals; therefore the power delivered to the dependent voltage source is -36 W.
       Note: With the h奴 give的ri the solution to I뇨쿄［Exercise 2.꾸he solution to I뇨皿 歐ercise
4.3 can be represented as shown in figure C.

                                                了乙V J뇨
                                                             .
                                                         띠卜H ／거




                                            乙啣7


       (c)
Drill Exercise 4.4
Use the mesh-current method to find the mesh current i a in the circuit shown.
Part A: Representative Drill Exercises with Solutions                                                  39




                                                                                       30A


                                                                                 ＼匕／
                                                            i .n                                  3n




                     』，三＝                                                 ,}:H                    "




Solution
In studying this circuit note the two current sources reduce the number of unknown mesh currents to
one, namely 1a. Thus the single mesh-current equation that describes the circuit is



           －加+       1      (fa－        』）『2          [ia            (刊：                     『
where


           vc    2   (ia+          午)          or v          =     4ia.

Solving for i a yields i a = 10 A.


Drill Exercise 4.5
Find the power delivered to the circuit by the 牛A current source.

                                                                                             4A




                                                            128 V
40                                                           Chapter 4/Techniques of Circuit Analysis



Solution

In studying the circuit illustrated, note that to fmd the voltage across the 牛A source requires solving
three node-voltage equations but only t팎o mesh-current equations. (The 中A current source yields a
known mesh current.) Define il and i2 as the mesh currents in the lower left and right windows,
respectively. The two mesh equations are

             -128+ 4 (i1- 4) +6 (i1- i2) +211= O

and

             6 (i2- ii) +3 (i2- 4) +30ir+ 5i2= 0,

where ir = i1 = 4. The solutions for i1 and i2 are i1 = 9 A and i2 = -6 A.
       The voltage drop across the 4-A current source, positive on the left is

             V4A =4 (i1 卞4) +3 (i2 -4) = -10V.

Therefore

             P4A =4 (H 10) = -40W.

The n恤us 毗nt네s us the 千A source is delivering 40 W to the circ山．


Drill Exercise 4.6
Find the Th6venin equivalent circuit with respect to the terminals a, b.




                      40 V




       (a)
Part A: Representative Drill Exercises with Solutions                                                    41




Solution
The Th6venin voltage can be found by writing a single node-voltage equation. Let V1 = Vab; then

          V1   V1- 4AJ
          1尸8+ ' 5                     21工＝ 0,


where it = (40 - v1)/5 . Therefore V1 = 20 V.
       To find the Th6venin resistan氾 we can either find the short-circuit current or use the
test-source method. We will do it both ways.
       First we will find R1by finding the short-circuit current. With a short circuit across a, b the
short-circuit current from a to b will be

          iab = iSC = 8 + 3i ,

where i = 40/5 = 8 A. Therefore iSC = 32 A and R = 20/32 = 0.625 (2.
       If we use the test-source method, we apply a test source across a, b after remo岫ng all
independent sources. The resulting circuit is shown in figure B.




                                                                     二7
        他）

From figure B we have
                          브
                  브
                                  O乙
                                                                                                              H
                                                                                                              小




           iT=        l
                              5
                                         킁）
                                              ,




 or t'r / Pr = 8/5, hence R = VT / 1T = 0.625 Q . The Thevenin equivalent circuit is shown in figure C.
 42                                                         Chapter 4fFechniques of Circuit Analysis




       （이


Drill Exercise 4.7
Assume that the circuit in the figure is delivering ma虹mum power to the load resistor R.
        a) How much power is the 100-V source delivering to the network?
       b) Repeat part (a) for the dependent voltage source.
        c) What percentage of the total power generated by these two sources is delivered to the load
           resistor R?




Solution

        a) For ma虹mum power transfer R = 32. When R is 3 Q the voltage across R 毗l be one-half
the Th6venin voltage, or 60 V.
       Let v1 be the node voltage across the essential branch containing the 20-V source and the 4-Q
resistor, positive at the top. The circuit can be described in terms of a sin멤e node-voltage equation
because the voltage across the 3-Q resistor is known. Hence


          "'二100* "' -4 20『 "' 少＝0，叫＝印V.
                                                                                                     43
Part B: Representative Problems with Solutions




It follows directly from the circuit sho꿔n in the figure that v中 = 60 - 20 = 40 V, and the current out
of the positive terminal of the 100-V source is

                 100       60 * 140- 60
          hm=
                       -
                              +               30A.
            。=         4
                                          =
          11。


Thus the 10아V source is delive如g3仄刃 W to the circu九

       b) The current out of the positive terminal of the dependent voltage source is (140 - 60)14, or
20 A; hence the dependent voltage source is delivering 800 W to the circuit.

       c) The power delivered to the load is 1200 W; therefore the percent of the developed power
delivered to the load is (1200/3800) x 100, or 31.58%.



Part B: Representative Problems with Solutions

Problem 4.1
Use the node-voltage method to find v1 in the circuit shown in figure A.

                                     5n                     iOf1




        （미


 S아ution

 In studying the circuit in figure A note there are 5 nodes and therefore we anticipate writing 5 - 1 or
 4 n에e-voltage equations. However, further inspection reveals two independent voltage sources
 connected directly between nodes and hence the number of unknown node voltages is reduced to two.
         In selecting a reference node, note that the node in the center of the circuit diagram is an
 attractive choice because then the desired unknown voltage v1 becomes one of the unknown node
 44                                                                 Chapter 4lFechniques of Circuit Analysis



voltages. The circuit showing the reference node along 꿔ith the assignment of the node numbers is
shown in figure B.


                                                         2.
                                                              45Y
                                                                                        '
                                                                                       1
                                                                                  3,
                                                                                       1
                                                                                       1
                                                                                       1


       (b)

       Since the current in the 270-V source is unknown, we form a supernode as shown by the
面tted line in fi멧re B.
       Now note from the circuit that v2 is a known node voltage, i.e., v2 = 45 V; and the node
voltages v3 and v4 are constrained by the 270-V source, n쏘ely v3 = v4 + 270.
       Summing the currents away from node 1generates the equation

             v1             1/ -45
         三計乳＋ '5                     = 0.

Summing the currents away from the supernode gives

             v3 - 45        브和   V3 - 270
                                          .1- tn = 0                                           +
                10                   60    " V그l     '

Now when we use the constraint

          .       45 小 V3
         1A=
          LI           10   '

the preceding equations are reduced to two unknowns. Solving for v1 yields v1 = 54 V.


Problem 4.2
      a) Find the branch currents i a and i, for the circuit shown in figure A.
      b) Check your answers by showing that the total power generated equals the total power
         小ssipated.
                                                                                                              45
Part B: Representative Problems with Solutions



                                                           1 ] /b




                          2.7 A                                                             135 V




       (a)
Solution
                                                                                                   it
In studying the circuit in figure A we note there are 4 nodes and 4 meshes. Hence at first glance
                                                   equations 찌ill be needed to describe the circuit.
appears either 3 node-voltage or 4 mesh-current
However, further study reveals 2 voltage sources are connected between nodes; hence the
                                                                                                      will
node-voltage method will reduce to a single equation. Likewise the presence of 2 current sources
reduce the mesh-current method to a pair of simultaneous equations.
         The computation of the branch currents from mesh currents involves addition, whereas the
computation of branch currents from node voltages involves division. We shall opt for the
mesh-current approach. The mesh currents are defined as shown in figure B. Since we do not know
 the voltage across the dependent current source, we shall use the supermesh shown as a dotted path
in figure B.

                                                          /／乙力




                                                                                                   .:
                                                                                                1砧1yI
                                                                                                i3,
                          그口A
                                                                                                          J
                                                                                                          1
                                                                                =m   戶느   ==1    小    戶
                                                                    =m尸   日m1




             (b)
             Summing the voltages around mesh 3 gives

                   e1lib + 5 (i3 -i4) + 1 (i3- i2) = 0.
46                                                          Chapter 4/Techniques of Circuit Analysis



       Summing the voltages around the supermesh gives

          10 (i2 - 2.7) + 1 (i2 - i3) + 5 (14 - i3) + 135 = 0.

       The currents tb and i4 can be eliminated from the equations by noting tb = i3 - i2 and 14 -
                                                                                                   i2
= 0.8 1d = 0.814 or i4 = Si2. When these substitutions are made, we get the following pair of
equations:

          -1512 m 513 = 0,


          3（可2 - 613 = -108.

It follows that 12 = -2 A, 13 = 6 A, and i4 = -10 A.The branch currents are

         i a = 2.7 寸12 =4.7A,


         i b = i 3 Hi2 =8.0A,


         IC =i3- i4= 16.OA,


         i d =14= -10A,


         ie =13= 6A.

      b) The voltage across the 2.7-A source, positive at the top is 101a = 47 V.
      The voltage across the dependent current source, positive at the top is 101a + 1ib = 55 V.
      The power delivered by the 2.7-A source is

         p2.7A(del) = (2.7) (47) = 126.90 W.

      The power delivered by the 135-V source is

         P135 (del) = 135 (10) = 1350 W.

      The power delivered by the dependent source is

        P11Ib (del) = 88 (6) = 528W.
                                                                                                       47
Part B: Representative Problems with Solutions



       The power absorbed by the dependent current source is

              PO.旽 (abs) = (8) (55) = 440 W.

       The power 小ssipated in the three resistors is

              PR = (8)2 (1) + (4.7)2 (10) + (16)2 (5) = 1564.9明 W.

       Therefore the total power generated is

              X尸gen = 126.90 + 1350.0 + 528.0 = 2004.9 W.

       The total power dissipated is

              1 "diss = 1564.9 + 440 = 2004.9 W.


Problem 43
Determine i。and vO in the circuit shown in figure A when R is 0, 2, 6, 10, 14, 20, 30, 40, 50, and 70 Q.


                                                   3.76 fl           2n




                    10 A




        (a)
 Solution
 Since R。is being varied over a range of values, it is worth first finding the Thevenin equivalent with re-
 spect to the terminals of RO. In this circuit successive source transformations afford a straightforward
 method for arriving at the Th6venin equivalent. Several intermediate circuits that are produced by
 successive source transformations are shown in figures B-E.
 48                                                                      Chapter 4/Techniques of Circuit Analysis




                                                 I Ofl           2끄1
                                                 ＼人／            /\d/
                                                                  1HyH
                                                                                  H




                          ez.4V

                                                                             스        i
                                                                                          "
         (b)   First transformation




                     1,24-A中 '.4 5,e,z.:44I 극小a《
                                                                                 之CL




       (c)
               Second transformation


                                                                 乞4之



                                       44
                                                         {=＝十
                                                                                              ，

       (d)     Third transformation




                                            口V



       (e) P配比fin equ如a把nt



The determination ofi。and vO has been reduced to the analysis of the circuit shown in figure E. It
follows that

              .      24                          24RO
                                and         V"= 10
             'O = 10 + RO                          + RO
Part B: Representative Problems with Solutions                                                           49




Problem 4.4
When a voltmeter is used to measure the voltage ye in figure A, it reads 4 V. What is the resistance of
the meter?

                                                        0.70 V
                                                                        24i.
                                40k(          1.25kf)   1               뇨d     4kf)




                       12 V                                                            12V




       (a)
Solution

One approach to this problem is to first find the Th6venin equivalent with respect to the terminals of
the 2.24 kQ resistor, assuming the resistor is an internal component of the circuit. We begin the
analysis by first replacing that part of the circuit to the left of the 2.24-kQ resistor 꿔ith its Th6venin
equivalent! We get the circuit shown in figure B.

                                  긋5. 25乞2.              口．      品4乙b
                                         ／戶
                                       -b=    (t>
                        (>.5V



       (b)

       Recognizing that the current do帥 through the 2.24-kQ resistor is 25gb leads us to the equation

             6.5 = 25.25db + 25ib (2.24)

orib = 0.08 mA = 80uA.
      It follows that

             Vth = Vab = (0.08) (25) (2.24) = 4.48 V.

       Placing a short circuit across a, b and then calculating the short-circuit current yields



             뇨＝    （崗如毗
                  25
50                                                           Chapter 4/Techniques of Circuit Analysis



Therefore the Thevenin resistance is

             R = 까 / isc 七 696.12Q .

The Th6venin equivalent is shown in figure C, where we have also shown the voltmeter as an external
load.

                                         (4石. /‘之／그4

                                              ／山1그
                            캬彷V                         4V
                                                                    中    『

       (c)
We know from the statement of the problem that when the voltmeter is attached it reads 4 V.
Therefore it follows from figure C that the current drawn by the voltmeter is (4.48 - 4.00)1696.12, or
approximately 0.69 mA. Hence the resistance of the meter is (4/0.69) or approximately 5.8 k(2.


Problem 4.5
Use the principle of superposition to find vO in the circuit shown in figure A.




                    13 V




       (a)
Solution

In applying superposition to a circuit that contains dependent sources we must remember to keep the
dependent sources in the circuit at all times.
Part B: Representative Problems with Solutions                                                        51



        For the circuit in figure A the dependent voltage source stays in the circuit as we consider the
contribution from each independent source. To find the contribution of the 13-V source we solve the
circuit in figure B for vO' and to find the contribution of the 6-A source we solve the circ山 in fi햇re C
for vO"

                                                                     f( a.
                                                                    八八／          1
                                                         2노2.            5:i乙    I (5fL
                                                                     4小I'八／
                                                                     寸m
                                                                            mH1十H八人／
                                                                                기r
                                                                                          r
                                                                                          1

                      '3V
                                                                     色'            트      朴
       (b)




       (c)
The node-voltage equations for the circuit in figure B are

             v1- 13 . v1- v2 . v1- v2 n
               m    十   ,m   十   4 / = U
               3         /      ic

and

             V2   -   33 1
                       (므
                                -   v2   )   /7 + V2: V1 + V2   :
                                                                     V1
                            d                        /
                                                                              0.
                                                                          =
                                                                lO


Solving for v1 and v2 gives v1 = 12 V and v2 = 10.37 V. It follows that

              .         2 (v1 - v力
                                    11.53 V.
             V'O = V1 -    " '7 " =
52                                                           Chapter 4lFechniques of Circuit Analysis



       The mesh-current equations for the circuit in fi엣re C are

          161i + 5 Eli - (12 - 6) 1 + 2 (i1 - i2) = 0,


          312+ 2 (12- il) +5[ (i2- 6) -i1] +8 (i2- 6) +33 (i2- i1) =0.

Solving for i1 and i2 yields ii = -1.10 A and i2 = 0.67 A. It follows that

          v"。=5[ (i2- 6) -i1] +8 (i-          6) +33 (12- ii)

               = -5.53V

Therefore v。= vO' + vO1' = 11.53 - 5.53 = 6.00 V.



Part C: Supplementary Problems

Supplementary Problem 4.1
Use the node-voltage method to find the branch currents i a through td in the circuit in the figure.

                                         in          2 fi



                                                                             2




Supplementary Problem 4.2
       a) Use the node-voltage method to find v in the circuit in the figure.
       b) Find the power source associated 꿔ith each source in the circuit and state whether the
          source is delivering power to, or absorbing power from, the circuit.
Part C: Supplementary Problems                                                                     53




                                                ioc




                               50 V
                                                                5/m




Supplementary Problem 43
      a) Use the node-voltage method to find vi in the circuit in the figure.
      b) How much power is dissipated in the 55-Q resistor?
      c) How much power does the 125-V source deliver?
      d) Repeat part(c) when the 55-(2 resistor is changed to 110 Q.




Supplementary Problem 4.4
      a) Use the mesh-current method to find the voltage v in the circuit in the figure.
      b) Find the power associated with each source in the circuit.
      c) State whether the source is extracting power from, or delivering power to, the circuit.
54                                                          Chapter 4/Techniques of Circuit Analysis




                                                3A




                                                                50 V
                               136 V




Supplementary Problem 4.5
Use the mesh-current method to calculate the power associated with each element in the circuit in the
figure.




                         3n




                                       2c1




Supplementary Problem 4.6
Determine the Th6venin equivalent with respect to the terminals a, b for the circuit hi the figure.
Part C: Supplementary Problems                                                                         55




Supplementary Problem 4.7
The resistor R in the circuit shown in the figure is adjusted until ma址mum power is delivered to the
resistor.
       a) Wha出 the vat出 of R?
       b) What is the power delivered to R in milliwatts?
       c) 硼at percentage of the total power delivered by the sources in the circuit is delivered to R?


                                  bK1i                   1.0kg




                     40 V


                            口20          k【1    令    ·   751     .       +   8




Supplementary Problem 4.8
The load resistor RL in the circuit in the figure is adjusted until ma址mum power is delivered to RL.
       a) 꿔hat is the vat出 of RL?
       b) What is the ma址mum p이妃r?
       c) What percentage of the power delivered by the 100-V source reaches RL?
56                                                             Chapter 4lFechniques of Circuit Analysis




                        1伉）V




Supplementary Problem 4.9
Use a Th6venin equivalent to find iO in the circuit sho싸n.



                                             5c           4c




                                  30V                             6f




Supplementary Problem 4.10
Use the principle of superposition to find y八 in the circuit in the figure.




                           10 V
                                 Chapter 5
                         Topology in Circuit Analysis


Part A: Representative Drill Exercises with Solutions

Drill Exercise 5.1
       a) Find the power associated자ith each branch of the circuit in the figure.
       b) Verify that the power generated is equal to the power absorbed.
                                                   5／口




                      149 V




Solution

       a) Using the tree defined in Fig. 5.13 and the solution for the tree-branch voltages given in
Eqs. (5.4) we first calculate the link voltages, thus

          Va = Vd 中 VC - Ve = 149- 4- 134 = 11V,


          Vb = VC- Vd = 134- 149= -15V,


          Vf =Yg mVc = 40 中4 =36V,


          Vh =Vc HVc mVg =l34+卜40 =98V.




                                                                                                       57
58                                                       Chapter SIT아川ogy in 아cuit Analysis




Now all the branch currents can be calculated.

         ia = 54= 5i1= 5 (1.8) = 9.OA,


         ib= Vb/ 2= -7.5A,


          iC = vCI4 = 1.OA,


         i d = i b H i a = e 7.5 e 9 = H16.SA,


         ie = VeI20 = 6.7A,


         If = VI20 = 1.8A,


         ig = Vg 15 = 8 A,


         ih = Vh I 10 = 9.8 A.

The branch powers are now determined using the power equationp = vi. The results are summarized
in the following table:

        BRANCH                   VO／工4GE (V)        CUR]？五NT (A)             POWER (W)
            a                         11                   9.0                   99.00

           b                        -15                  -7.5                   112.50

            C                          4                   1.0                    4.00

            d                        149                -16.5                -2458.50

            e                        134                  6.7                   897.80

            f                         36                   1.8                   64.80

            g                         40                  8                     320.00

           h                          98                  9.8                   960.40
Part A: Representative Drill Exercises with Solutions                                                      59




       b) From the table we can see that

          1尸gen = 2458.50W

          刀'dis =99+ 112.50+ 4+ 897.80+ 64.80+ 320+ 960.40

                     = 2458.50 W


Drill Exercise 5.2
       a) Use node 4 as the reference node in the circuit shown with Drill Exercise 5.7 and calculate
          the numerical values of the node voltages v1, v2, v3, and v5 via the node-voltage method.
       b) Check the answers to part (a) by using the numerical values of the tree-branch voltages vC,
          Vd, Ve, and Vg obtained in Drill Exercise 5.6(b).

Solution

       a) Refer to the figure in Drill Exercise 5.7 and note that when node 4 is used as a reference
there are three unknown node voltages, namely v2, v3, and v5, since v1 is known to be 149 V.
       The three node voltage equations are
                             的
           브加
                                             V     V           出
                        e

                                     V2 小
                                             }
                                                       }
                                                           中

                                                                   0                      +=
                        2                4                 加
                                             U         e
                                             y   出
          v3- V2 . v3- v5                5       r加            0                                       =
                 十
            4        >
                .            =       1




           V5       . V5- V2 . V5- V3             ,,
          五0十          2()       十       5       =u.

       The solutions are v2 = 134 V; v3 = 138 V; and v5 = 98 V.

       b) From Drill Exercise 5.6(b) the tree-branch voltages are vC = 4 V, Vd = 149 V, Ve = 134 V,
and Vg = 40 V. Using the tree-branch voltages to obtain the node voltages yields

          V1 = Vd = 149 V,

          V2 = ye = 134 V,
60                                                               Chapter 5/Topology in Circuit Analysis



           v3= ve+ vC= 134+ 4= 138V,


           VS = Ve+ Vc eVg= 134+ 4- 40= 98V.

These values agree 꿔ith the values obtained in part (a).


Drill Exercise 53
In the circuit in the figure. v. is increased to 10 V and all the resistors are set eoual to 1Q. Use the
Loop-current metnoo 10 nno
       a) the branch currents and
       b) the total power dissipated in the circuit.


                                                   0.5 1




                    叫                                                            in




Solution
       a) Using the same tree given in Fig. 5.17 and the identification 기ld orientation of the loop
currents in each tree branch as given in Fig. 5.18, the six fundamental-loop equations are

          10 = ta + (ia + i b + 1f H id 小e) !


          10 = tb + (1b + 1c - Ie) + (ib + i c + f - id 中 'e) + (a + i b + f - id - ie) ,


          0 == 1c+ (Ib+ 1c H1e) +(jb+ Ic+ 1f e1d m1e) ,


         0 = 1d+ (1d+ te Hja Hjb mjf) +(jd+ je ejb Ujc ejf) ,
Part A: Representative Drill Exercises with Solutions                                                    61



          0 = ie+ (ld+ ie eia Hib mif) +(Id+ Ie Hib 小ic eif) +(Ie 中ib HIc) ,


          10 = if + 伉 + ic + f 小 m 니e) + 偏 + ib + if - b 니e) ·

(Note: Since all resistors are equal to 1 ohm the dimension of each term on the right-hand side of
these equations is volts.)
       A computer solution of these six equations yieldsia = 5 A; tb = 5 A; iC = 0 A; i d = 5 A; i e =
5A; and if = 5A.
       Using the cut-set equations, the remaining branch equations are found. Thus

          1g =ia+ lb+ if= lSA,

          ih =ta+ 1b+ 1f U1d H ie= SA,
                                            A
           1
           LJ    1i
                  d
                          1
                              b   C
                                      f
                                      1i쏘
                                            0                     +=
                                                                  1
                                                                  H



                          匕
                                  A
                 1i
                                  0                               +=
          ik = tb + i c - ie
                  b                                                      =




        b) Since the circuit contains a single source, we can use the generated power to calculate the
total dissipated power. Therefore

          ZPdiss =Pgen = 10 (15) = 150W.

Note that this result agrees with the observation that 25 W is dissipated in branches a, b, d, e, f, and h
and no power is dissipated in branches c, j, or k.


Drill Exercise 5.4
Are the following three equations independent?

                       6v1 - 3v2 + 4v3 = 15.

                      2v1 + 8v2 - 10v3 = 0.

                -4v1 + 11v2 中 14v3 = -15.
62                                                              Chapter 5/Topoiogy in Circuit Analysis



Solution
The question is whether we can find three constants c1, c2, and c3, all of which are not zero, so that

             c1 (6v1 - 3v2 + 4v3 - 15) + c2 (2v1 + 8v2 - 10v3) + c3 (- 4v1 + 11v2 - 14v3 + 15) = 0.

First collect the coefficients of v1, v2, and v3 to get

             (&i + 2C2 H 4c3) v1 + (- 3c1 + &2 + 11c3) v2 + (4c1 小 10c2 - 14c3) v3 - 15C1 + 15C3 = 0.


Now make c1 = c3, as this will eliminate the terms - 15c1 + 15c3. Now our equation reduces to

             (2C1 + 2C2) v1 + (&i + &2) v2 + (- 10cr - 10C2) V3 = 0.

Now observe that if c1 = -c2 each coefficient in the above expression is zero. Therefore we conclude
the equations are not independent. In other words one equation in the set is a linear combination of
the other two. For example if we multiply the first equation by -1 and then add it to the second
equation we 찌ill generate the third equation.



Part B: Representative Problems with Solutions

Pr아)lem 5.1
Use the tree-branch method to find vO in the circuit seen in figure A. In selecting the tree, use the
recommendations made in Section 5.2.




       (a)
Part B: Representative Problems with Solutions                                                        63




Solution
Whenever po弱ible we place a branch in a tree if it contai哨 a voltage sou毗 or if the branch voltage
controls a dependent source. At the same time, if possible, we place a branch in a cotree if it contai口s
a current source or if the branch current controls a dependent source. The tree shown in figure B
sati呱es these recommendations.




       (b)

       It follows from the tree in figure B that the fundamental cut-set equations are

             la+ tb+ tc              =0,


             te+ ig尸1dH1b            =0,

             ih m ie H iC            =0,


             lc+ ib+ id+ If =0.

Now since 1h and i f cannot be expressed in terms of Vh and Vf, we focus on the first two cut-set
equations. In other words Vh and Vf are known tree-branch voltages and therefore we have only two

unkn"삡盆烈’olt筏＼”，삡出哉匹9;i,: v/5;id = V41/20:i,;ie = ,, = ,,;andi, =
v므/40. It follows that cut-set equations (1) and (2) become

              노m    9       느5
                             =   0
                                                                                                Chap妃r5ff아川四如lCircuit Analysis




                 左    노
                      m          m
                                 面
                                 +
                             e
                                         - (- 9) =O.


Now express the link voltages vC and vd in terms of tree-branch voltages. Thus


             V- = Vt 十 V. 小 1노" = 4') 十 V.. 小 7.25 I 亡1 '-
                                                                               .
                       .                             .   .             h   八       (vd\
              " -- - - -- ---      -- - -- --- !20) -

But Vd = Vf - Vg = 40 - Vg. Therefore


            %=
                     40+ Va          -
                                         等     (40
                                                             -   Vg)


and the first cut-set equation becomes

                 쁘
                 m    l
                      e5                       14.5。+
                                                                       等           d이     9         +=
                       I'
                       (4。
                                 + V.      -
                                                                                               3Va + O.725Vg = 39.

The second cut-set equation reduces to

                    v。 (40- v。)
                    40H ' 20 " - e9,
                 a+

or 4伽a + 3Vg = -280 . It follows that Vg = VO = 120 V.


Problem 5.2
Use the loop-current method to find the power developed by the independent voltage source in the
circuit shown in figure A. In selecting the tree, use recommendations made in Section 5.2.



                                                                                          各

                                         125
                                          V三牛480O" r55O
                                                                   25O                        40O




      (a)
                                                                                                         긔



Part C: Supplementary Problems                                                                      65



Solution
A tree that follows the recommendations given in Section 5.2 is graphed in figure B. Here the graph is
simple enough to show the loop currents in their entirety.




       (b)
       Referring to the circuit in figure A, we generate the three loop-current equations.

             Loop a:
             -15i中 + 40 (ia + 'b) + 251a = 0 , i中 = i口 ·


             I乂兀pb:
              -125- lSia+ 40 (ia+ ib) +80jb =0.


             Loop C:
             中125- l5ia+ 55ic =0.

The solution to the three loop equations gives 1a = -1 A; 1b = 1.25 A; and iC = 2.0 A. The power
developed by the independent voltage source is

             P125 = 125 (ib + iC) = 406.25 W.



Part C: Supplementary Problems

Supplementary Problem 5.1
Use the tree-branch method to find the output voltage vO in the circuit shown in the fi햇re.
 66                                                               Chapter 5/Topoiogy in Circuit Analysis




                                                  5A




                            15V




Supplementary Problem 5.2
Use the loop-current method to find i1in the circuit shown in the figure.




                            6V                                           12V




Supplementary Problem 5.3
Use the tree-branch method to find v中 in the circuit shown in the figure.


                                        2 kfl              1 ku




                                                                            10 V
Part C: Supplementary Problems                                                                      67




Supplementary Problem 5.4
Use the loop-current method to fmd it in the circuit shown in the figure.




Supplementary Problem 5.5
Use the tree-branch method to find the power associated with each element shown in the circuit in
the fi암ire.
                                    5O         ion
                                                M


                         20 V                         二50O     11    4A




Supplementary Problem 5.6
Use the loop-current method to find the power delivered to the circuit by the dependent current
source in the circuit shown in the fi암lre.




                                                                      3.4／中
68                                                          Chapter 5/F아)01四y in Circuit Analy前S



Supplementary Problem 5.7
Use the tree-branch method to find the power delivered by the independent current source in
                                                                                            the
circuit shown in the figure.


                                               15 A
                                           Chapter 6
                                    The Operational Amplifier


Part A: Representative Drill Exercises with Solutions

Drill Exercise 6.1
Assui毗 that the 叩erational ammfier in the circt血 誼叫n is ideal.
      a) Calculate vO for the following values of v3: 0.4, 0.72, 2.0, -0.6, -0.8, and -2.0 V.
      b) Specify the range of v5 such that the amplifier does not saturate.
                                                                    100 kfl




Solution

       a) To obtain an expression for vO as a function of v, sum the currents away from the inverting
input terminal, thus

          "'   ;   "'   + V1
                            。
                           1。
                                -   VO
                                         +i1=                  0.
Now take advantage of the characteristics of an ideal operational amplifier. First i1 = 0 and second
v1 = 0 because v2 = 0. Therefore our equation reduces to

                        100 v. = -12 5v.
          VO =     -
                         8 a'
                                         4e   '   V   '   )'
We must also rec雎nize that vO lies bet吼en -10 V and +15 V. For the given values of v the
corresponding values of vO are



                                                                                                        69
 70                                                                   Chapter 6/The Operational Amplifier




            v
                  (J)
                                                   v。(V)            v5 (V)                     v (V)
                -2.0                                15 (sat)         0.4                  -5
                -0.8                                10               0.6                  中9
             -0.6                                       7.5          2.0                卞10 (sat)


       b) v。reaches negative saturation when v is 0.8 V and vO reaches positive saturation when v =
 -1.2 V. Therefore the linear operating range corresponds to -1.2 V 5 v 5 0.8 V.


Drill Exercise 6.2
        a) Find vO in the circuit shown if Va = 0.1 V and Vb = 0.25 V.
        b) Ifyb = 0.25 V, how large can Va be before the op amp saturates?
        c) IfVa = 0.10V, h이기arge can Vb be before the 아m叩 鋌turates?
        d) Repeat parts (a), (b), and (c) with the polarity of vb reversed.


                                                                       250 kfi




Solution
     a) We begin our analysis by finding vO as a function of Va and Vb. This relationship is derived by
summing the currents away from the inverting input terminal. Thus

          "vl';           ' +
                        "va     V1   ;;Vb   * V12; VO
                                                    +i1=
                                     25     +   25。
                                                               0.
Now we invoke the properties of the ideal op amp; i.e., i1 = 0 and v1 is zero because v2 is zero. (Note:
v2 is zero by virtue of an external connection.)
Part A: Representative Drill Exercises with Solutions                                                  71




       Solving for vO gives us the desired expression

          VO = -50巾a - 10巾b .

When Va = 0.1 V and vb = 0.25 V, vO = -7.5 V. We note this value lies within the linear ra叩e of
operation.

       b) When Vb = 0.25 V our expression for v。isvO = 小50 Va - 2.5. The op 仙p reaches
saturation at -10 V; therefore the largest value of Va is -7.5/-SO, or 0.1.5 V.

     c) When Va = 0.10 V, vO = -5- 10 Vb. Now the op amp reaches saturation when Vb =
-51-10, or 0.5 V.

       d) With the polarity of vb reversed our expression for v。is VO = -50 Va + 10 Vb. When Va =
0.1 V and vb = 0.25 V, Vb iS -2.5 V. We note this value lies within the linear range of operation.
When Vb = 0.25 V, V。= -50 Va + 2.5. Since the op amp saturates at -10 V the largest value of Va is
小12.51-50, or 0.25 V.
       When Va = 0.10 V, 1'O = -5 + 10 vb. As Vb increases, the op amp will saturate at +15 V;
therefore the largest value of Vb is 2 V.


Drill Exercise 6.3
       a) In the difference 키llplifier shown, Vb = 6.0 V. What range of values for Va will result in
          linear 아心硝on?
       b) Repeat part (a) with the 20-kg) resistor decreased to 5 kQ.

                                                                40 k1)




 Solution
       a) First note that since the op 缸p is ideal i2 = 0 and v2 = (20/25) Vb = 0.80 Vb = v1. Now
 sum the currents away from the inverting input terminal using the fact that i1 = 0. Thus
72                                                                  Chapter 6/The Operational Amplifier



           V1 小Va . V1 HVt9           ,\
             10    十         40   =U '

Replacing v1 with 0.8 Vb and solving for v。gives v。= 4(v, - Va).
      When Vb = 6 V, V。= 24 - 'a. To find the limits on Va we first note the limits on v。are t 10 V.
Therefore

          4v口 = 24 土 10 ! or v口 == 14/4 == 3.5 V and


          Va = 34/ 4 = 8.5 V. Thus 3.5V 5 Va 5 83V.

        b) When the 20次Q resistor is decreased to 5 k , v2 = v1 = 0.5 vb and the e사）ression for vO
becomes v。= 25vb - 4Va. When Vb = 6 V, vO = 15 - 4va or 4Va = 15 t 10 V. The limiting values of
Va are 1.25 V and 6.25 V. Thus

          1.25 V 5 Va 5 6.25 V.


Drill Exercise 6.4
In the bridge circuit in the figure, the circuit parameters are Vdc = 1.5 V, VC = 20 V, R1 = 10 kQ,R2
 =2kc,R4= 1k , andA =2x10.
       a) Find v1 - v2 in microvolts when R is larger than its balance value by 1C.
       b) Specit ' the range of R工 such that the operational amplifier does not saturate.


                                                                     + vcc


                                                                겨

                       Vdc
                                  +         \   /   +
                                                                     寸 vcc        V0
                                  ]
                                       수＝
                                                    V2
                                                        " ' "




Solution
      a) By definition vC = (v1 + v2) = 104uV and vd = v2 - v1 = - 11.2uV.
Part B: Representative Problems with Solutions                                                        73




                                        Ad
       b) CMRR =20 log10                     = 20 log10 1000 = 60dB.
                                        aC
       c) By definition

          4 = Al + A2 }

            d
                           2
                          le
            a                                    =
                           (A2 尸Al) ·

Therefore
            al   = {Ac- Ad= e 999,500

and

            d七
             ）
                           AC +Ad = 1,000,500.
                  n
                      2
         미
            VO = AC vC + Ad Vd
                 = i03 10 x 10_ 6 + 106 (- 11.2 x 10_6) = -11.19 V.

        e) When v1 = v2 = 15.6 4叱 vC = 15.6 4uV and vd = 0. Therefore vO = 15.6 mV.
        When v1 = v2 = 4.41uV; ve = 4.4uV and Vd = 0. Therefore v。= 4.4 mV.



Part B: Representative Problems with Solutions

Pr야)Iem 6.1
 The operational amplifier in the circuit shown in the figure is ideal. Calculate the output voltage when
 the input voltage v, is 25 mV.

                                                     50 kO         40 kfl




                                                                                 30 kcl
 74                                                             Chapter 6及he Opera如nal Am川豌r



 Solution
In this 血cult we can fi川 the 에聊t voltage V加y sumn血g the currents at the invert血g 蜘ut
terminal 키ld at the node formed by the connection of the 5卜, 10-, and 40-ku resistors. Let us denote
this as node "a" and assign Va as the voltage across the 10-kQ resistor, positive at the top. (Note: We
do not sum the currents at the output node of the op 缸llp because the current into the output
terminal is unknown.) Our two node-voltage equations are

                          '               Va
                                  +                0
           0;
                      V
                              "
                                      0
                     45
                                               =
                1.
and

           Va . Va mVO . Va m0
           10十                    40      十        50   =U '

When v, = 25 mV the first node-voltage equation gives us Va = -25/29 V and the second
node-voltage equation yields vO = -5 V.


Problem 6.2
The variable resistor RO in the circuit in the figure is adjusted until the source current ig is zero.
Assume the ideal operational at叩lifi야5 are 아比rati叩 in their linear r踞jot蟠．What is the va岫 of凡？




Solution
Let v。 1be the output voltage of the first op amp and v。
                                                       2 be the output voltage of the second op amp.
Now by summing the currents at the inverting input terminal of the first op amp we get vO1 = -3v.
S山曲ing the currents at the inverting input terminal of the second op amp yields v。   2 = -1.6 v。1=
4.8v,.
Part B: Representative Problems with Solutions                                                         75



      It follows 小rectly from the circuit 小agr缸ll that

          .       vi . vi - V。
                             2  vi  3.8vi
          1.'n = ！느 + ' 1 != = t느 e =1. '
          'g   l5 '    RO       15     R。．'

By h卯othesis 1g = 0; therefore RO = (3.8)(15) = 57 k(2.


Pr야)lem 6.3
Assume that the ideal op 帥p in the circuit in the figure is 아比rati叩 in 奴 血ear r叩油．
       a) Calculate the power delivered to the 4.7-kc resistor.
       b) Repeat part (a) with the 아心ational ai叩l小er removed from the circ旼，that 奴毗뇨he
          4.7-kc resistor connected in the series with the voltage source and the 43.5-k(2 resistor.
       c) Find the ratio of the power found in part (a) to that found in part (b).




Solution
      a) Because the op amp is ideal i2 = 0, and therefore v2 = 235 mV. It also follows that v1 = v2
= 235 mV. Finally we observe vO = v1 = 235 mV.
      The power delivered to the 4.7-kQ resistor is (235 x i0日)214700 or 11.75 UW.

      b) With the op amp removed the voltage across the 4.7-kQ resistor is (4.7/50)(235) or 22.09
mV. In this case the power delivered to the load is (22.09 x i0H3 )214700 or 0.1038uW.

       C)Pa巾b 七 113.17.

      d) Yes, the op amp acts as a buffer and enables the 235-mV source to control 113.17 times as
much power to the load.
 76                                                                              Chapter 6/The Operational Amplifier



Pr야)lem 6.4
The operational amplifier in the adder-subtractor circ山 sho帥 in the figure is ideal.
        a) Find vO when Va = 2.5 V, Vb = 5 V, VC = 15 V, and Vd = 10 V.
        b) If Vb, vC, and vd are held constant, what values of Va will saturate the op amp?

                                 十            5 kfl                            40 kf2
                               VaS1           V＼小／HH叫                          八／/VH1



                                    +         8k{)
                               Vb




                                 +            30kfl
                               Vc卜H1\          /V\                                           33 kf I

                                  +           60kfl
                               Vd e           \＼人

                                                                     120 kf3



                                    V


Solution

      a) First find vO as a function of Va, vb, vC, and vd. Start by summing the currents at the
noninverting input terminal

           V2    . V2 HVd . V2- Vc . . ,,
          正0十        日） 十    30   十i2= U.

But i2 = 0, therefore we can write

                 2
          y2=    ; (2vC + Vd) .
Also note that v1 = v2 because the op amp is ideal. Now sum the currents at the inverting input
terminal; i.e.,

          V1 HVa     .   V1 eVb         .   V1-    VO   .   .   -'
             5       十     8            十     40        十i1 = U.
Part B: Representative Problems with Solutions                                                       77




Since i1 = 0 and v1 = (2I7)(2vC + Vd), we solve directly for vO. Hence

              VO = 8VC + 4Vd - 8Va - SVb

Now substitute the given numerical values for Va, Vb, vC, and vd to get

              vO = 12+ 40- 20- 25= 7 V.

       b) VO = 12 + 40 - 8Va - 25,
             = 27 - 8Va.

The op a叩 saturates at 土 15 V; therefore we solve for Va such that

              吃 =    (27!
                            15)


Therefore Va = 1.5 V at positive saturation and Va = 5.25 V at negative saturation. For linear
operation 1.5 V 5 Va 5 5.25 V.


Pr야)lem 6.5
       a) Find the Th6venin equivalent circuit with respect to the output terminals a, b for the
          inverting amplifier of figure A.
       b) 싸hat is the output resistance of the amplifier?
       c) What is the input resistance seen by the source v when the load at the terminals a, b is 600
          (2?

                                                     100 kCI




        (a)
78                                                                            Chapter 6/The Operational Amplifier



Solution

        a) We begin by fm小ng the Th6venin voltage v, = Vab. Summing the currents at the inverting
input terminal gives


                 Vl-4 Vs + V'-1。
                               。     V
                                             +希

Summing the currents at the output terminal yields

                 yi- v1 . v1 - 104 (v2 - v1)
                  10()     十                 1               =I) '

After observing v2 = 0, solve this set of equations for v1. We get v, - -24.93 v.
       Using the test-source method to find the Th6venin resistance reduces to solving the circuit
shown in figure B. Note in dra痂g the circ山 we have used the fact that v2 = 0.

                                                                     k29k乙2




                                                                                          V.누


       (b)
      It follows directly from the circuit in figure B that the test current 1T in milliamperes is

             .       少r+
                               10伊？1 +
             LT =              1



But

                               1力F               1600       41方r
             V1 =                .       .        月,.' .1 = =;; ·

                    1叫醫
                                         )
                                                 'Ii)
                                                        '.
                                                              1W
Part B: Representative Problems with Solutions                                                         79




Now substitute v1 into the expression for i T and solve for the ratio VT/iT. Thus


              VT＝凡：4꼼g몲1/ 10" 七2.62(2·
       The Thvenin equivalent is shown in figure C.

                                                          乞 (2. a.


                                     그4.43匹



       (c)
       b) The output resistance is the same as the Th6venin resistance; i.e., RO = R 二口 2.62 Q.

        c) We can use the Th6ve而 equivalent to predict the value of the output voltage when a 600-(
resistor is connected across the terminals a, b. It follows directly from figure C that


             「b＝        2.62 (
                       6。
                       品0          24.93v5)

                   斗 -24.83 v .

       Now we can sum the currents at the inverting input terminal of the circuit in figure A when a
600-Q resistor is connected across a, b because we know vO in this case is -24.83 v5. Thus


                              h伽
               V1 -    V5 .         v1+ 24.83                                                               +
                          十                     "s = 0.
                   4                     100

       Solving for v1 gives

              V1 브 0.0066 v5.

It follows that the current supplied by the source is

             .   Vs - 0.0066 v5
             Is=      4（乂乂1     '
80                                                                                    Chapter 6/The Operational Amplifier



The resistance seen by the source is v/i3; therefore



                 凡vsis
                                    =   1聲；
                                                      66   =
                                                               4026.76 C   ·




Problem 6.6
Find v。in the circuit shown in the figure.

                                                                               5 (1




                                 3V




Solution

We must assu毗 the 아）帥ps are ideal beca出e we have no 河Ormation to the contr기ry. I力tv可
represent the output voltage of the first op a叩. Now sum the currents at the inverting input terminal
of the first op amp. In writing the expression take into account that at the inverting input terminal of
the first op amp that v1 is zero because v2 is zero. Thus

                               3* 0- vO1              0- v0
                                                  1
                                                  +                 0
            0-
                                +             4
                                                                -
                         。.5
                                                                -
       or

            vO1 = - 0.8 vO 小 24.
Part C: Supplementary Problems                                                                      Si



Now observe that the output voltage of the first op amp shows up across the 8-c) resistor, which is
connected to the inverting input terminal of the second op amp. Summing the currents away from the
top terminal of the 8-Q resistor yields

                              0     +
                                   % =
                      e
            브
                      2
            8
or

                    1 = 1.25 (- 0.8 vO - 24) .
          v。= 1.25 v。

Now solve for v。to get

          vo= -15V.

Check to make sure the first op amp is not saturated. This check is necessary because our analysis was
pre小cated on the assun叩tion the op ai叩s are 아比rating in their linear re蜘n

          vO = - 0.8 (- 15) - 24 = -12 V.

Since the first op 카np saturates at 土 15 V our analysis holds up.



Part C: Supplementary Problems

Supplementary Problem 6.1
The operational amplifier in the circuit in the figure is ideal.
       a) Calculatev。ifva = 4Vandvb = OV.
       b) Calculate vO if Va = 2 V and Vb = 0 V.
       c) Calculate vO if Va = 2 V and Vb = 1V.
       d) Calculate vO if Va = 1V and Vb = 2 V.
       e) If vb = 1.6 V, specify the range of Va such that the amplifier does not saturate.
82                                                                     Chapter 6/The Operational Amplifier




                                                             100 kfl




Supplementary Problem 6.2
The operational amplifier in the circuit in the figure is ideal.
       a) CalculatevO.
       b) Calculate i 。



                                                    40 kfl




                        2.5 V
                                                                         5 kf




Supplementary Problem 6.3
The op amp in the circuit in the figure is ideal.
Part C: Supplementary Problems                                                                        83




       a) CalculatevO.
       b) State whether the amplifier is inverting or noninverting.


Supplementary Problem 6.4
The inverting amplifier in the circuit in the figure has an input resistance of 500 k(2, 기l output
resistance of 5 kQ, and an open-loop g曲 of 300,000. Assume that the amplifier is operating in its
linear region. Calculate the follo耐ng:
       a) the voltage gain (vdv3) of the amplifier;
       b) the value of v1 in millivolts when v = 1V;
       c) the resistance seen by the signal source (vi).
       d) Repeat parts（毗 他工 and (c) 出ing the ideal model for the 아）amp.


                                                      100 kfl




Supplementary Problem 6.5
Repeat Supplementary Problem 6.4 given that the inverting amplifier is loaded with a 1-kg resistor.
84                                                               Chapter 6/The Operational Amplifier



Supplementary Problem 6.6
       a) Find the Thevenin equivalent circuit with respect to the output terminals a, b for the
          inverting amplifier in the figure.

                                                    50 kul




       b) What is the output resistance of the amplifier?
       c) What is the input resistance seen by the source v when the load at the ter曲als a, b is 20目
          (2?


Supplementary Problem 6.7
The operational amplifier in the noninverting amplifier circuit in the fi암lre has an input resistance of
吼0 k52, an output resistance of 5 ks), and an open-loop gain of 20,0刃. Assume that the op amp is
operating in its linear region. Calculate the following:
       a) the voltage gain (vo/vg);
       b) the inverting and noninverting input voltages v1 and v2 if Yg = 1 V;
       c) the difference (v2 - v1) in microvolts when Vg = 1V;
       d) the current drain in picoamperes on the signal source Vg.
       e) Repeat parts (a卜U江ssuming an ideal 아）카叩．


                                                         80 kU




                                                                       4 kfi
Part C: Supplementary Problems                                                                                85




Supplementary Problem 6.8
The circuit in the fi암lre is an ideal linear differential amplifier in which the gain of the amplifier is a
function of the external resi如心 사，R2,1b and 凡．
       a) Show that

                R4 (R1+ R2)          R2
          VO = R1（凡 + 凡）Vb H 瓦Va '

       b) What is the expression for vO if R3 = R1 and R4 = R2?




Supplementary Problem 6.9
Select values of RB, Rc, and RD in the amplifier circuit in the figure such that vO = 8(yb - Va) and the
voltage source Vb sees an input resistance of 4500 (2. Use the ideal model for the operational amplifier.




                                                                               10 k1I
86                                                              Chapter 6/The Operational Amplifier




Supplementary Problem 6.10
The two ideal operational amplifiers in the circuit in the figure are known to be operati培 in their
血tear reg幻n.
       a) Calculate vO1.
       b) Calculate v。
                     2.


                           5V




                           3V
                                   Chapter 7
                           Inductance and Capacitance


Part A: Representative Drill Exercises with Solutions

Drill Exercise 7.1
The current source in the circuit shown generates the current pulse

          ig (t) = 0,      t <0;

                 =5eH2어i小5ee8qyA,           t之0.
          拓（t)

Find (a) v(0); (b) the instant of time, greater than zero, when the voltage v passes through zero; (c)
the expression for the power delivered to the inductor; (d) the instant when the power delivered to
the inductor is ma虹mum; (d) the maximum power; (f) the ma虹mum energy stored in the inductor;
and (g) the instant of time when the stored energy is ma址mum.




Solution

       a) The reference for the current in the inductor is in the direction of the voltage drop across
the inductor; hence


                   V= L竺＝2><10카-1以Xkm2어y+ 4000e小800t1
                       at                                                   t> 0
                              L                     J

                        =8e4800tH2em2어t       t> 0

              v(o+) =8 m2 =6V.



                                                                                                         87
88                                                                         Chapter 7/Inductance and Capacitance



       b) When t > 0, the voltage will be zero when 8e18어y = 2em2어노, or t = (노4) /600 = 231ms.

        c) The expression for the instantaneous power at the terminals of the inductor is vi; therefore
for t > 0,

                          '
                                               (5eH2以t             800t)
         p =
                                                             5e_
                (8e1800
                              -   2e   _2어y)
                                                         -




            = 5me1여Xt e40e-l텨Xy 1 伽니어)CW.

       d) We know from calculus that whenp is passing through a ma址mum its fi心t derivative with
respect to time will be zero. Thus

           立4  = 0 = - 50,00C匕-1어Xy + 64,侃（匕-160i + 40C（匕中긔xt.


To fmd the values of t where dp/dt is zero, we multiply by e1텨X노 and divide by 4000. Thus

          e120노 =.
                -1l 2.5e600'+ 16= 0.

Now let x = e60 '. This produces the quadratic equation

         工2- 12.5x + 16 = 0.

Solving for the roots of the quadratic equation yie1dsx1 二已1.45 andx2 斗 11.05. The corresponding
values of time are

          rl= (In 1.45) 1600 = 616.58ps

and

          t2= (lnll.05) /600= 4ms.

Now refer to the expression forp obtained in part (c) and note the smallest value oft that is greater
than zero will give the largest value ofp. Therefore the power is ma虹mum at ll or 616.58 bus.

       e) Substituting the value oft1 into the expression forp gives

          P (t) = 5(匕e 0.61858 - 10e_0"4 (0.61858) - 4C匕-1.6 (10.61858) = 4.26 W.
Part A: Representative Drill Exercises with Solutions                                                     89



       11 The easiest way to fmd the maximum ener2v is to first fmd the ma址［llum current and then
use the energy equation w = (112)Li2. We can deduce the time of maximum current as follows. First
note the expression for ig tells us the current starts at zero, rises to a positive peak, and then decays to
zero. The positive peak corresponds to (di8/dt) = 0, which in turn implies the voltage is zero. Thus we
can use the time found in part (b), i.e. 2.31 ms, to fmd the ma虹mum current. We get

          i max = 5e 小0.2 (2.31) - Sc中0.8 (2.31) 七 2.36 A.

It follows that

                                         36)2 勺
           叩m缸
                    =   {(2   x 10H3) (2.     5.58   mJ      .




    g) The ma虹mum energy coincides with maximum current; hence the stored energy is
ma址mum at 2.31 ms.


Drill Exercise 7.2
The current in the capacitor is 0 for t < 0 and 2 cos 50,000t A for t 之 0. Find (a) v(t); (b) the
maximum power delivered to the capacitor at any one instant of time; and (c) the ma虹mum energy
stored in the capacitor at any one instant of time.

                                                          0.5 肛F

                                                   F니ea
Solution

       a) Since the current is known, we use the integral relationship to find the voltage; thus
                    l
           v = 스f '_ idr+ v (o)
                   c- U



                 = 2 x 106 f     _2 cos50,어X뇨dr + 0 = 80 s1n50,어0tV,        (t 之 0).
90                                                             Chapter 7/Inductance and Capacitance



       b) The reference for the current is in the direction of the voltage drop; therefore

          p = vi = (80 sin 50,0001) (2 cos 50,00目

            = 160 sin 50,000t cos 50,000t

            =80sin1000,000tW          t 之0.

It follows that the ma疝num power delivered to the capacitor is 80 W.

       c) The maximum energy stored will coincide with maximum voltage, or 80 V. Therefore

          Wm., = } (0.5 X 10_6) (80)2 = 1600/{J.



Drill Exercise 73
The current at the terminals of the two capacitors shown is 240e - 1位／iA for 1 之 0 . The initial values
of v1 and v2 are -10 and -5 V, respectively. Calculate the total energy trapped in the capacitors as t
approaches infinity.




Solution

To fmd the energy trapped in the capacitors at t = m, we need to determine the voltage on each
capacitor at t = oo. The current and the initial capacitor voltages are specified; hence we use the
integral relationship to calculate the voltages v1 and v2. We have

          v1= 0.5 x i06 fi + 240 x 10H6e11야 dx - 10


            = - 12eH10'+ 2V.
Part B: Representative Problems with Solutions                                                                                                                 91




          v2= 0.125X 106fi
                        , + dx 巾 S


              = -3ee10'- 2V.

It follows that v1(oo) = 2 V and v2(끼 = -2 V. Therefore the trapped energy is

                                             lo_                                              10'                                  2
          叩=        글        （2
                                         x          6)
                                                               (22) +    글         （8
                                                                                          x          6)   (U            2)
                                                                                                                                       =   20肛J.




Part B: Representative Problems with Solutions

Problem 7.1
The current in a 2-H inductor is

          i= SA, t 50;


          i= (B1cos1.日+ B2sin1.&)e寸0'41A, t之0.

The voltage across the inductor is 28 V at t = 0. Calculate the power at the terminals of the inductor
at t = 5 s. State whether the inductor is absorbing or delivering power.


Solution

To find the power at the terminals of the inductor at t = 5 s we need the numerical values of v and i at
5 s. To fmd the numerical expression for the current i we must determine the values of the coefficients
B1 and B2. The values of B1 and B2 can be determined from the statements that the initial value of the
current is 5 A and the initial value of the voltage is 28 V. From the expression for the current we have
i (0) = B1 = 5A.
        Assuming the reference for the current is in the五rection of the voltage drop across the
inductor we have

                                  di               d
          v                                                      cos               6t + B2 sin
                                             2-
                                                                                                                              e'
                                  dt               dt                                                                                  0A]
              =L-                        =
                                                                         1.
                                                         [(5                                              1.
                                                                                                                   6)
                                                                                                                                                          O巾
                                                  + 0.8B2)                              61 +         2B2                           cos
                                                                                                                                                     c_
              =         [-
                                   (16
                                                                   sin
                                                                              1.
                                                                                               (3.
                                                                                                               -         4)
                                                                                                                                           1.   日]
       Then v(0) = 3.2 B2 - 4 = 28 or B2 = 10. Thus the expressions for v and i are
 92                                                                                                       Chapter 7/Inductance 기ld Capacitance




               yv= (-
                   (m24Sin
                      24sin1.6t+
                           l 日 28cos1.
                                 COS l 61)
                                       日）e -0.4: V

 and


               i = (5COS
                      cos l .
                          1.61
                            日+ 10
                               l0 Sbl
                                  sin l .
                                      1.61)
                                        日）e -0.4: A.

At t = 5 s the numerical values of v and i are -3.76 V and 1.24 A, respectively.
       It follows that at t = 5 s

          p = (- 3.76) (1.24) 二已 - 4.67W.

The minus sign tells us the inductor is delivering power to the circuit connected to its terminals.
       Note: If the reference direction for the current is assumed in the direction of the voltage rise
across the inductor the thought process for findingp(5) is the same. In this case the voltage across the
inductor is v = -Ldi/dt and the power expression isp = -vi. The numerical results are

          B1= SA;                                   B2= -7.SA;


          「＝
                =             [12
                              [l25i.
                                       sin
                                              1.
                                              l·
                                                   日＋28m8
                                                   61 + 28 cos l·61   1.
                                                                           Q]
                                                                                ]   e
                                                                                        -0.
                                                                                              4:   A,
                    r尸                       4 』，           m 尸 . m 』已 1 -0.4: -
          i=        [Dcosl.
                                                   oi   -   I.
                                                                 Ds1nI.(YJ e                   /\ ; ana


          p = -(1.06) (- 1.10) = 1.16W.

In this case the inductor is absorbing power from the circuit connected to its terminals.


Problem 7.2
The three inductors in the circuit shown in the figure are connected across the terminals of a black
box at t = 0. The resulting voltage for t 之 0 is known to be


          Vb = 16匕44iV.
Part B: Representative Problems with Solutions                                                          93




                                                                            그




                                                                 曾，   ckx

                            3H




                                                                            J

If i1(O) = 1A and i2(O) = 3 A, find
       a) i。
           (O);
       b) iO(t),        t 之 0;
       c) 11(t),        t 之 0;
       d) 12(t),        t 之 0;
       e) the initial energy stored in the three inductors;
       t) the total energy delivered to the black box;
       g) the energy trapped in the ideal inductors.


Solution

       a) To find i。we first replace the original inductors with an equivalent inductor. The para끄［el
inductors can be replaced by a 2-H inductor carrying an initial current of 4 A. This 2-H inductor c出
then be combined with the 8-H inductor so that the original array of three inductors is reduced to a
1（下H induc帥 carrying 4 A in the dir吼如n of i口 Th小 M이 = 4 A.

       b) The voltage across the equivalent inductor is vb. Since vb is a voltage rise with respect to the
reference direction for i。the expression for iO(t) is

                        1 ,4
                                     1 (o)
                   = e I뎌 J。Vb tir 十
                       -eq

                   ==   H




                     . -4t .         n
                   ='e     A,    I 亡 U.
94                                                                                                Chapter 7/Inductance and Capacitance




       c) To fmd i1(t) we first fmd the voltage across the parallel inductors. Let this voltage be
denoted as v1, positive at the top. To fmd v1 we first find the voltage across the 8-H inductor. Let this
voltage be called vO, positive at the top. Then

          v。= -8 (di。/dt) = 128ee4'V,                                          t之O.

Now

          Vl= VbHV。
                  ＝32e寸4iV,                                           t之O.

and


          il= 긍工‘ 32e’缸m+ 1
                         8H 3
                                         七      A
                             e
                                              5小 3
                                                                                              H




                                                             t 之 0.                               =
                                                                                                  小




       d) Since v1 is also the voltage across the 6-H inductor, it follows 小rectly that


          b=         －       층工          ‘   3勿’缸血*             3


                         4H 3
                                         屯     A
                             e                5e3
                                                                                                                     H

                                                                                                                         +=
                                                             t 之 0.



啣品黑粘罪"熬眈inusall '"'"" ""'""'""" "'" "'"' " "" """' " "
          w    (o)       =        {(8)
                                             (4)2+    {(3)
                                                                (1)2+   {(6)
                                                                               (3)   2=
                                                                                          92.50J.

       f) The total energy delivered to the black box is the same as the initial energy stored in the
equivalent inductor; therefore

          Wdj:. = f (10) (4)2 = 80J .
Part C: Supplementary Problems                                                                          95




Note: An alternate calculation is to first fmd the e사ression forp(t) and then integrate from t = 0 to t
= cc. Thus


          p   (t)   =   VbiO =   (16伽e41)         (4e小4          ') = 6伽U앉W

                        r的   / . ,\ -8t ,                 n八 1
          叩di弱＝ J。 64侁 나dt= 80J·


        g) The total energy trapped in the t뇨ee inductors can be found by using the final values of 。,


                                                                   (
i, and i2. Hence


                                            引引口                        5e3
                                                                             4{
                                                              6    r              \
                                                                                      L
          ...trapped - l /l\                                lH 2
                                                                                      +=
                                                                                      l八乙  <
                     e2＼  刀
                                                                                       e




          ry
                                                                                           U
                                                                                  J
Part C: Supplementary Problems

Supplementary Problem 7.1
The triangular current pulse shown in the fi암lre is applied to a 20-mH inductor.
       a) Write the expressions that describe i (t) in the four intervals t < 0, 0 5 t 5 5 ms, 5 ms 5 t 5
          10 ms, and t> 10 ms.




                                                                                               10




       b) Derive the expressions for the inductor voltage, power, and energy. Use the passive sign
          convention.


Supplementary Problem 7.2
The current in a 160-mH inductor is known to be

              ／八       i=m\ . 4 i日 . 尸nn八 -250t .                                       , ,1
          i = ( .) cos J1人fit 十 I· 그 sm >（凡片) e /\ )                                  ( = U.
96                                                             Chapter 7/Inductance and Capacitance



       What is the ma疝mum magnitude of the inductor voltage? Assume the passive sign convention.


Supplementary Problem 7.3
The current in a 10-H inductor is

          i= 4A,      t 50.


          i=
           = (BlC0S0．
                 cos 0.8t + B2 sin
                       秘＋B2Sin0旼）e-0.61
                                   0.&) A,           t之 0.

The voltage across the inductor is 16 V at t = 0. Calculate the power at the terminals of the inductor
at t = 4 s. State whether the inductor is absorbing or delivering power.


Supplementary Problem 7.4
The rectangular-shaped current pulse shown in the figure is applied to a 2.5-uF capacitor. The initial
voltage on the capacitor is a 6-V drop in the reference direction of the current. Assume the passive
sign convention. Specify the capacitor voltage at 5, 10, 20, and 30 gus.




                           5




                                        1       1      0       I      I            r似引
                           0           10      15             25     30

                       -   2




Supplementary Problem 7.5
The trapezoidal current pulse shown in the figure is applied to a 0.5-1uF capacitor.
       a) How much energy is stored in the capacitor by the current pulse?
Part C: Supplementary Problems                                                                            97




       b) How much charge is on the capacitor at t = 15 1us?
       c) Calculate the voltage on the capacitor at t = 23/iS.




                                            10      15        20    25      30




Supp佃nentary Pr야)lem 7.6
The three inductors in the circuit in the figure are connected across the terminals of a black box at t
= 0. The resulting voltage for t 之 0 is known to be

          VO =2어：
                匕尸4tV.

If i1(0) = 5A, find
       a) i3(t),      t 之 0;
       b) i1(t),      t 之 0;
       c) i2(t),      t 之 0;
       d) the initial energy stored in the three inductors;
       e) the total energy delivered to the black box; and
       f) the energy trapped in each of the ideal inductors.
98                                                                  Chapter 7/Inductance and Capacitance




                                                                         +




                             三5H
                                                   20 H


                                                            )7
                                              ，寸
                                                                "
                                                                        V0
                                                                             탁땄

                                   ，』十   6H




Supplementary Problem 7.7
For the circuit in Supplementary Problem 7.6, what percentage of the total energy delivered to the
black box has been delivered when t = 150 ms?


Supplementary Problem 7.8
The three capacitors in the circuit in the figure are connected across the terminals of a black box at t
= 0. The resulting current 4, for t 之 0 is known to be

           i。(t) =3.2eH10'mA.

If v1(O) = 25 V and v2(0) = 15 V, find (fort 之 0) (a) vO(t); (b) v1(t); (c) v2(t); (d) i1(t); and (e) i2(t).
Part C: Supplementary Problems                                                                  99




                                 +




                   "'"丁十."' h"""
                           10 卜LF／戶＼V2




Supplementary Problem 7.9
For the circuit in Supplementary Problem 7.8, calculate

       a) the initial energy stored in the capacitors;
       b) the fmal energy stored in the capacitors;
       c) the total energy delivered to the black box;
       d) the percentage of the initial energy stored that is delivered to the black box; and
       e) the percentage of the total energy delivered that is delivered in 40 ms.
                          Chapter 8
         Response of First-Order RL and RC Circuits


Part A: Representative Drill Exercises with Solutions

Drill Exercise 8.1
The switch in the circuit shown has been closed for a long time and is opened at t = 0.
       a) Calculate the initial value of i.
       b) Calculate the initial energy stored in the inductor.
       c) What is the time constant of the circuit for t > 0?
       d) What is the numeric川 ex마明如nf야 i (t) for I 之 0?
       e) What percentage of the initial energy stored has been 小ssipated in the 44 resistor 5 ms
          after the switch has been opened?
                                                           t= o




                      100 V




Solution
       a) For t < 0 the inductor is a short circuit; therefore there will be no current in the 午Q resistor
before the switch is opened. Prior to opening the switch the current out of the positive terminal of the
100-V source is 100/[1 + (5)(20)/25] or 20 A. The current in the 5-Q resistor (left to right) is
(20/25)(20) or 16 A. It follows that the initial value of i is -16 A.

       b加＠ 카 (10 x 可가- 1寸 = 1.28J .

        c) r = L/R = 10 x 10 3/4 = 2.5 ms

        d) i= /‘戶-1t= -1命e4어yA ,          t之0



                                                                                                       101
 102                                                               Chapter 8/Response of First-Order RL and RC Circuits




:,,,,,?，曾弩眈中，咎，然出：黑，火，is1.
                      current
                         28e畔盜“,"，‘客煮＝盒：뇨
中O resistor is the difference between the initial stored energy and the energy stored at t = 5
                                                                                               ms;
therefore


           w鈿 = 町이 - w (5 ms) = 1.28 (1- 戶）J.

It follows that the percentage of the initial energy stored that is dissipated after the switch has been
open for 5 ms is

                                                     4
           %di55:            28                  e
           % diss =
                                            -



                                                             100 = 98.
                        1.
                                  (1
                                                         x
                                            28                        17.
                                                     )
                                       1.
Drill Exercise 8.2
The switch in the following circuit has been closed for a long time before opening at t = 0.
       a) Find v0(t) for t 之 0.
       b) What percentage of the initial energy stored in the circuit has been dissipated after the
          switch has been open for 60 ms?




                 15 V                                                                            40 kfl




Solution

        a) Inst此沖培 the circi血 no妃 that after the switch is opei妃d the 5／小 capacit아 wi11 址由arge
into the 20-kO resistor and the l-duF capacitor will discharge into the 吼）-kO resistor. Therefore the
voltage across the 5-uF capacitor can be found independent of the voltage across the 1-MF capacitor
and vice versa.
        Before the switch is open the capacitors act like open circuits and the current out of the
positive terminal of the 15-V source is (15/75) or 0.20 mA.
Part A: Representative Drill Exercises with Solutions                                                                                                 103




       Let v5 be the voltage across the 5-MF capacitor, positive on the left, and let v1 be the voltage
across the 1-uF capacitor positive at the top. Then v5(0) = 20(0.20) = 4 V and v1(0) = 40(0.20) =
8V.
.     .The time constant associated        the 4uF capacitor. r.5               x
                                                                                  10'3 = 100 ms and
                                                                                     with
                                                                                                                         is       . =   (20)
                                                                                                                                               ,(5之
                                                                                                       5-
tue time constant associated witii me i-ur capacitor is 11 = (4(J) (1) X LU V = 40 ms.
       We can now write the expressions for v5 and v1, namely

             v5= 4em1mV,                                          f之0

and

             v1= 8em25iV,                                          t之0.

From our definitions of v5 and v1 we see that

             v。=v5+ v1= 4eH10t+ 8ee25rV,                                                                    t之0.

          b) First calculate the total ener目stored in the two capacitors, thus:

             w   (0)            =   {5
                                              (4)
                                                    2+           {(1)
                                                                          (8)   2=
                                                                                                   72肛J.

Next calculate the total energy stored at t = 60 ms. The voltages v5 and v1 at 60 ms are v5 斗 2.20 V
and v1 二＝1.79 V. Therefore

             叩
                       （60ms)
                                         七｛
                                                    (5)          (2.20)2 +                  {(1)     (1.79)   2斗
                                                                                                                   13.64肛J    .




It follows that

             wdiSS (60 ms) = w (0) - w (60 ms) 七 58.364uJ.

The percent dissipated is

             % dissipated =                               [58.          36/72] 100 = 81.05


Drill Exercise 8.3
The switch in the circuit shown has been in position a for a long time. At t = 0 the switch is moved to
position b. Calculate (a) the initial voltage on the capacitor; (b) the fmal voltage on the capacitor; (c)
104                                                   Chapter 8/Response of First-Order RL and RC Circuits



the time constant (in microseconds) for t > 0; and (d) the length of time (in microseconds) that it
takes the capacitor voltage to reach zero after the switch is moved to position b.

                                                                    1.25 k{1
                                                                      VW
                                                         t =0

                                  3.5 kf3


                     60 V                                                                         8 mA
                                                                               壬6.
                                                                                     75 kfl
                                                                +

                                 11.5 kfl


                                                 0 05 " FT
                                                  .
                                                                VC




Solution

        a) Since the switch has been in position a for a long time the capacitor acts like an open circuit
for t < 0. Therefore the initial value of vc is the same as the voltage across the 11.5-kQ resistor.
Therefore
                                  l
                                  l              V
                                            <
                                            1U
                                                 拓
          yC(0U) = vc(0
          v (0     yC(0+)        型巧                                                           =




       b) After the switch has been in position b the capacitor again appears as an open circuit
                                                                                                 and
therefore the final v고ue of vc is the same as the voltage across the 6.75-kO resistor. Hence

          vc(的) = -8 x 1013 (6.75 x 103) = -54V.

mP c
capacit。
      就n"撰烈咨群恕沙，：隙砦，恕cen micr。 ，捏싻繇絮）,,,
                         seenIs少，
400.

        d) Since we computed the initial and final values of vC along with the time constant of the
circuit fort > 0, we can write down the expression for vc(t); thus

          vyC(0 卜54+
             (t) =       (46+ 54)e-25어t
                   -54 + (46


                = -54+ 1伉匕-25以yV ,               t之0.
Part B: Representative Problems with Solutions                                                          105




vc(t) will equal zero when

              10匕m250Y =54

or

                     i     .    (ioo'
              t ＝云面in（찌

               = 246.47 4us.




Part B: Representative Problems with Solutions

Problem 8.1
The switch in the circuit seen in the figure has been closed for a long time before opening at t = 0.
Find, for t 之 0,
        a) 包（r),
        b) VL(t),
        c) ii (t).


                                        30 i




                                 1
                                                                                                              1
                         400V                  』！1    20mH    :
                                                                  y     90f1i；   」＼
                                                                                      lOU1
                                                                                                                  1
        (a)
 Solution
         a) To find iL(t) for t 之 0 we need to find the initial value ofiL and the time constant of the
 circuit. We find the initial value of L by calculating 1L in the circuit just before the switch is opened.
 Prior to opening the switch the inductor acts like a short circuit; therefore that portion of the circuit
 to the right of the inductor has no effect on z. for t < 0. For t < 0 the Thevenin equivalent of the
 106                                                                     Chapter 8/ 之esponse of First-Order RL and RC Circuits



circuit to the left of the inductor is a 280-V source in series with a 25-O resistor. Therefore iL(o) =
280/25 or 11.20 A.
        To fmd the time constant after the switch is open it is necessary to fmd the Th6venin
equivalent of the circuit to the right of the inductor. By using the test-source method, the Th6venin
resistance is found to be 52.50 O. This method is shown in figure B and the following calculations; the
기比yen노 equ如alent is shown in figure C.

                                               H中＝ L丁                  勿I스



                                                                                                       111qL
                                                                                                               二
                                                                                               >>> r
                                                                                         느寸4

                                                                                <22{2.                   八

                  (b)




                        h=
                                    3位‘*   h（싹6。       (70)
                                                       塑拓     h
                                   70奸
                             =(30) -   +


                    Rt= 甘1/iT= 52i0Q.




            (c)
It follows that the time constant is (21/52.5) or 0.40 ms. Therefore

                    q (t) =11.20匕-25여yA ,                         t之0.


       b)
                    vL =      L쁘＝
                                           m
                                               娩小어yV
                                                                   ,
                                                                        I之0.
                                     UI

       c) Using current division, the expression for iA(t) is found to be


                    jL(t)：금L (t) =-4．어尸啣A, t 0.
Part B: Representative Problems with Solutions                                                                  107




Problem 8.2
At the time the switch is closed in the circuit shown in the figure, the voltage across the paralleled
capacitors 1120 V and the voltage on the 5-4uF capacitor is 10 V.
       a) What percentage of the initial energy stored in the three capacitors is dissipated 如 the
          10-kQ resistor?
       b) Repeat part (a) for the 2- and 40-k(2 resistors.
       c) What percentage of the initial energy is trapped in the capacitors?




                         4 나F
                                                                                      10 kfl




Solution
       a) To find the energy dissipated in the 10-kQ resistor we first find the expression for the power
dissipated in the resistor. The energy can then be found by integrating the power. To find the power
we will first find the current. To find the current we reduce the circuit to an equivalent capacitor in
series with an equivalent resistance. The equivalent capacitance is (20)(5)I (25), or 44uF, charged to 50
V. positive at the unoer terminal. The eciuivalent resistance is 2 + (400I50).                  or 10 kQ. The time
                                                                                                    1 느 11 n  !=m1  1
                                               ')
h4h八1hH1 八r 114 m 八： ,1J1 = 1r\ 4 /J 1/ m r..-Ic
constant 01 the circuit   is 1(1  (4 X  10
                                                  h小 4r\ '4= n 11 Jy八11 小小4 114 1 11 n
                                                  or 4U  ms.   It bOlows    that  the    114 느4
                                                                                       voltage  across the equivalent
resistance is

           v= 50eH2StV,          t之0,

 where v is positive at the upper terminal of the resistor.
        The current into the upper terminal of the equivalent resistance is

           i= v/104= 5em25tmA,             t之0.

 Using current division, the current into the upper terminal of the 10-kQ resistor is (40/50)i, or

             kQ= 4eH25imA,
           :l。                         t之0.
108                                                                                                               Chapter 8/ 之esponse of First-Order RL and RC Circuits



The power 小ssipated in the 10-kg resistor is

             P1。
               kQ = (11。kQ)2 l04 = 0.16eU5m W.


The energy dissipated in the 10-k(2 resistor is

             叩10kQ= J。 끄kQ dt=                                                                     3.
                                                                                                        2   mJ·
The initial energy stored in the three capacitors is


             叩（이 카（16x 106) (44J)2+ {(4x10已 (44)2 +{ (5 x 1丁뇨10)2

                                 = 16.25mJ.

        Therefore


            %d帥a妃d＝금知 100= 19.69.
       b)
            i2k{2            =i = 5eU25imA.


            P2k{2 =i 2 (2000) = 50eU50' mW.


            W2kQ                        i尸
                                                            P2kcdt=
                                                                                       1mW.
            』나   .   .       .                                              1
             7o ci's없p缸ea = ＝二；)< I（大J = (Ll> ·
                                             .                                                     』 ，，八




                                                                          'U. 乙J




            .                     1.                                      -25t     .
            i40kQ        =
                                  3i=
                                                                      C          mA.


            P4。
              kQ = (i40kQ)2 (40,000) = 4匕H5아 mW.


            W40k(2       =
                                  J              P4okQdt=
                                                                                              0.
                                                                                                        80mJ.
Part B: Representative Problems with Solutions                                                                                                109




          ,,1 .. . . .     0.80    dnn . nm
          'ro cussiparea = =;=;i x wu = 4.YL.
                                                 J1J1二J




       c) Let v2 be the voltage across the 5-uF capacitor, positive at the upper terminal; then


          , ,：二귿止j.5x1戶少公* 10
                          _,       V




            =40eH25i-30V,                                       t之0..

Tht好V2（미 = 中30V.
      Let v1 be the voltage across the paralleled capacitors, positive at the top; then


          V1 =
                     뿌J                     s／       可＝           凡 『的
            =10ee25'+ 30V,                                      t 之0.

Thu鉀K끼 = 30V.
    The energy trapped is

                               =   {             X
                                                     lo_        (30)2 +글         X
                                                                                     10_        (30)2 + {        X
                                                                                                                     10_
                                                                                                                                (_   羽)   2
          Wti.
             apped
                                       (4
                                                           6)              (16
                                                                                           6)               (5             6)
                               = 11.25mJ.

It 向표ows that


          ％啣小                               (｝       雀）         100= 69.23

To check the calculations note that 69.23 + 4.92 + 6.15 + 19.69 = 100%.


Problem 8.3
The switch in the circuit shown in the figure has been in the ON position for a long time. At t = 0 the
switch is moved to the orv position.
       a) Find the numerical expression for iO(t) when t 之 0.
       b) Find the numerical expression for vO(t) when t 之 0.
 110                                                     Chapter 8/Response of First-Order R乙 and RC Circuits




                                       4O          ON


                                                                                   밋L
                                                         t= o
                     96V                                                                81 mH



                                                                            l
                                                        16.2 A   vO   (f)   多36O
Solution

        a) For t < 0 the inductor acts like a short circuit. The initial value of iO is


          iO(0") =iO(0')=(4즈끄） 賈 = 4A.
After the switch is in the 아下 posi的i for 키ong time, the 如uctor aga뇨 acts like a short circu丸
Therefore the final value of iO(t) is

           .. .        -162                .
          i ( 的) =          = ,1   =-9A.       .
            '              l8


[Note: In calculating i (이）) we first found the equivalent resistance of the parallel combination of the
60百2, 36-Q, and 1842 resistors; i.e., Re = 10 Q.]
        With the switch in the OFF position the Th6venin resistance seen from the terminals of the
inductor is 18 + (60)(36)/96 or 40.50 O; therefore the time constant for the circuit is


          r= 81 x 10H3/405= 2ms.

       It follows that the numerical expression for iO(t) is

          iO (t) 卜9+               [4- (- 9) ]e中5어y


                     = -9 + 13eH5어yA ,             t 之 0.

       b) From the circuit we note that the voltage across the 36-O resistor is the same as the voltage
across the 18-O resistor plus the voltage across the 81-mH inductor. Thus

                                  나4 di
          vO   (t)
                     18i + 81 X 10   dt
Part B: Representative Problems with Solutions                                                          111




                          = -162 - 292.5em5어 ' V,   t之 0.

It is worth noting that if we had not found iO(t) first, we could find vO(t) directly by using the technique
of finding the initial value of vO(t), the final value of vO(t), and the time constant.

node-, 沙，“出沙，客쁘，낍빠낱升，黑瓢띠，少，心瓷：就然乳：,
like a 午A current source since there cannot be an instantaneous change in inductor current. Thus at t
 = 0+ we have


           vO     『 vO
                6。 +                 +16.2+ 4= 0
                     ')
                (0
                               (0)
or

           vO(O+) = -454.50 V.

At t = co the inductor acts like a short circuit; so

           VO（的） == -16.2 (10) == 中162 V .

The time constant is the same as above; i.e., 2 ms. It follows then that


          vO(t) = 162
          %(0            1454.60+ 162]e
                  l62+ [-454.60   l62]e -500


                          =-162- 2925ee500'V,       t 之0.



Problem 8.4
The s毗ch in the circuit seen in figure A has been open a long time. The switch closes at t = 0. Find
iO(t) fort 之 0.
 112                                               Chapter 8/Response of First-Order RL and RC Circuits




                                     100 mU        8O         2O




                              14O                                            240V




        (a)
Solution

Prior to closing the switch at t = 0 the inductor acts like a short circuit. The initial value of iO(t) can
be found using the node-voltage method. Using the lower node as the reference node 缸ld letting v1
denote the voltage across the branch containing the 5-(2 resistor and the dependent voltage source,
we can write the equation


               h正丁
                    . V1 - 1位中 , v1 - 240 -
                               丁          = U
                          5         10

Now use the fact that i中 = (v1 - 240)110 to find v1 = -140 V.
      It follows that

              iO(0m) = iO(0+) = -v1/14 = 10 A.

We can obt小n both the final value of iO and the time constant of the circuit by finding the Thevenin
equivalent circuit with respect to the terminals of the 100-mH inductor after the switch is closed. The
Th6venin resistance is 25 (2 and the Th6venin voltage is 264 V as shown in figure B. From the circuit
shown, the fmal value of iO(t) and the time constant are easily determined; thus

                                     k>On4나  긋5:r2=
                                .   ＞니勿工1H>1구人／
                                              ()                               //
                                                                        在，4\
                                      H牛乞
       (b)
Part B: Representative Problems with Solutions                                                           113




             i。
              (oo) = 264/25 = 10.56 A

and

             r = 100 x 10e3/25 = 4 nlS.

       The expression for iO(t) is

             iO(t)
             匈 （0     l0.56+ (10 -
                     = 10.56 (l0el0.
                                   10.56)e -25(


                     =10.56H0.56e小25OtA,       t之0.


Problem 8.5
The switch in the circuit seen in figure A has been in position a for a long time. At t = 0 the switch
moves instantaneously to position b. Find v。 (t) and i。(t) for t 之 0.




                            4.8 mA




       (a)
Solution

Before operating the switch the capacitor acts like an open circuit. Therefore fort < 0 the current
iO(t) is

             iO(0 ) = 4.8 [ 100/160] = 3 mA.

The voltage across the capacitor at I = 0e is

             v。
              (0小) =(40x 103) (3x 10小3) =120V.
114                                              Chapter 8/Response of First-Order RL and RC Circuits



Since there cannot be an instantaneous change in the capacitor voltage we have

             v。
              (0+)=v。
                    (0小) = 120V.

After the switch is operated, we can find the final value of v。along with the time constant by fmding
the Theve小n equ如alent 毗h res恥ct to the tern恤als of the capacitor. We 丘rid 凡 = 羽 k and Vt =
80 V. The circuit is shown in figure B.

                                              쿄＞坦- 2-
                                              人＼/H
                                                          +
                                                                        工弘   尸F
                                 艮八／
                                                         弩 T
       (b)

      From figure B we see that the final value of v。
                                                    (t) is -80 V and the time constant is (30 X
103)(1乃0) x 10-6 or 1 ms. Therefore for t 之 0,

             y. h80 + (l20 + 80)eH1어


               = -80+ 200ee1어XyV ,            r之0.

It follows directly from the circuit diagram in figure A that

             . -.           i',,(t)
                                  . l0H6 dv。
             i叭U    =           }十
                        40 )< 10나    .)u 口1



                    :   -   2－    和   '蜘mA,    t20.




Problem 8.6
In the circuit seen in the accompanying figure switch 1has been in position a, and switch 2 has been
closed, for a long time. At t = 0, switch 1moves instantaneously to position b. Two hundred
microseconds after switch 1moves to position b switch 2 opens. Find vO 450 1us after switch 1 moves to
position b.
Part B: Representative Problems with Solutions                                                            115




                                                                         t = 0 + 200 1L s

                                                                                       2




                          50 V




Solution
Before switches 1 and 2 operate, the capacitor acts like an open circuit and the initial voltage on the
capacitor is

          v (0) = (30/ 40) (24) = 18 V,

positive at the upper terminal. In calculating vC(0), replace that portion of the circuit to the left of vO
with its Th6venin equivalent (v1 = 30 V and R = 12 kg).
         At t = 450 4us both switches will have operated; therefore we must first solve for the capacitor
voltage during the interval of 0 5 t 5 200 1us. In this interval the capacitor is shunted by the 24-kQ
resistor and the series combination of the 4-kQ and 8-kQ resistors. Thus the equivalent resistance
across the terminals of the caoacitor is (12)(24)/(36). or 8 kQ. The time constant of the circuit is
八｝ 뇨／ -rl3) /m rn月＼ 1. mr\＝小 h小 /i /n\ '44 = 11 n11 小小＋ 11 小1 !
(8X   il口 (11Z4) X 1U ' , or (113) ms. It tollows that in 11      ! 1!
                                                                this      ! 1    1 1t
                                                                     time interval          !1
                                                                                   the capacitor   11
                                                                                                 voltage !
                                                                                                         is

          vV, = 18e
                l8e -3000 V,                   057S2004us.

At t = 200ps the capacitor voltage is


          v,(20Qus) = 18ee0'6 仁 9.85 V.


capa孟鷺紫謐： 忿烈謐謂韶指毗持쌌8-kQ'""'""" shunthe
       The voltage across the capacitor in the time interval 200 1us 5 t 5 m is

                          88eH2000
                                                      10_
                                              200 x
          V,=                                                    v.
                                     (1
                                          -
                                                            6)
                 9.
       Since vO is the voltage across the 8-kQ resistor, it can be related to vC by voltage division; i.e.,

                                              200 x 10 6)
                           y, 勺6.59ee2000 (1小
                      8
          VO =
                      而
       whent = 4501us, v。二＝3.99V.
 116                                             Chapter 8/Response of First-Order RL and RC Circuits



 Pro川em 8.7
 The voltage waveform shown in figure A (left) is applied to the circuit of figure A (right). The initial
 voltage on the capacitor is zero.
          a) Calculate v。
                        (f).
        b) Make a sketch of v。
                             (t) versus t.


                                                            0.05 F




                                                 t (n倒

        (a)
Solution

       a) The recta叩ular voltage pulse can be viewed as a constant voltage source that is turned ON
at t = 0 and then turned on 2 ms later. Thus we have a circuit where sequential switc址ng takes pla凹.
       Since the initial charge on the capacitor is zero and cannot change instantaneously the initial
value of vO is 40 V. As the capacitor charges toward 40 V the output voltage approaches zero. The
time constant of the circuit is

              r = RC = (0.05 x 10_6) (200 x 103) = 10 ms.

Therefore

              v。
               = 0+ (40 - 0)eml어y


                =4（匕-1여)CV ,     0드t5 2nlS.

At t = 2 ms the value of the output voltage is

              v(2 ms) = 4C匕 -0.20 斗 32.75 V

and the voltage on the capacitor is 40 - 32.75, or approximately 7.25 V, positive reference on the left
terminal of the capacitor.
Part B: Representative Problems with Solutions                                                           117



        At t = 2 ms the source voltage drops to zero, and since the capacitor voltage ca끄lot change
instantaneously, the output voltage becomes -7.25 V. The capacitor now discharges toward zero at a
time constant of 10 ms. That is,

             vO(t) =m7.25e-1凹（1 - 0.002) V,    0.002드 t5m .

       b)
                                  v。(v)
                                  4O
                                  3O
                                  2O
                                  IO
                                   O
                                  니0




Problem 8.8
The gap in the circuit seen in figure 8.8A 꿔ill arc over whenever the voltage across the gap reaches
18,000 V. The initial current in the inductor is zero. The value of u is adjusted so that the Thevenin
resistance with respect to the terminals of the inductor is -8 Q. How many milliseconds after the
switch has been closed will the gap arc over?




                                                                                 Gap




       (a)
Solution

First find the expression for the Th6venin resistance as seen from the terminals of the inductor. Using
the test-source method, construct the circuit shown in figure B.
118                                                  Chapter 8/Response of First-Order RL and RC Circuits




                                          IC）느r之            丁乞스       며中 乙丁


                                      쓰二그二＜>                               4b
                                                                                U:
                                                                                     ;
                                                                       스



       (b)

       Figure B gives

                     .   . ,400 \
             1方r = mm八 + iT ( ；人尸 ) )
                             \   JU   /



where i1 = (40/50)IT.
       Solving for the ratio vT/iT gives

              브h=8- 0.80' = Rr.


By hypothesis R = -8 O; hence a = 20 V/A.
      Now the Th6venin voltage can be obtained from an analysis of the circuit shown in figure C.

                                            1C2r2느



                       奴引／



      （이

       From figure C we have iA = - 125/50 or -2.5 A, and v1 = -40 iA - 20 iA or 150 V. Therefore
the problem has been reduced to solving the circuit shown in figure D.

                                              -8a.

                         r요力／



      (d)
Part B: Representative Problems with Solutions                                                        119




       The differential equation that describes the circuit in figure D is

                           1각di(t')
          150= -&(t) +40x10 V =.=1.
                               at

Separating the variables 甘ves



            '   (   ')   {（쑈．    乃＝        枷dt·

Therefore


          上（') , 磊．寸二 200力，
or

                   4 n 기尸 . 4 n m尸 200 :            ' ,\
          t () = - 16. ID 十 Jd. IDC    A,         I 크 U.


       The voltage across the inductor is

                    di(t') -- flflt
          VL(t) = L- ：윽 = 15山＝q나 V )              r 之 0.
                                      UI



VL will reach 18,000 V when

          C2仗느 =
                                120,

or

          t = 23.94ms.


Pr야)lem 8.9
At the instant the switch of the figure is closed, the voltage on the capacitor is 55 V. Assume an ideal
operational amplifier. How many milliseconds after the switch is closed will the output voltage vO
equal zero?
120                                            Chapter 8/Response of First-Order RL and RC Circuits




                                                                +   1(
                                                                    55 V
                                                                           -




                                                                         10 F1F


                                75 kfl


                                                                                   +

                       35 V
                                                                                   v,,




                                                                                   V




Solution
The problem is to derive the e사：)ression for the output voltage vO as a function of time. The
differential equation governing the behavior of v。is obtained by summing the currents at the inverting
input node. Begin by first noting from the figure that v1 = v2 = (60/100)25 or 15 V. Note that v1 = v2
because the op amp is ideal. Therefore the differential equation is


            立謐『10 x 1丁' 붊小－%)                    却


or

            dv。
             dt= 50.


To solve this differential equation requires knowing the initial value of vO. The circuit diagram in the
figure reveals that


          v。
           (0+)= -55+ v1= -40V.


Therefore


          心神山g句
Part B: Representative Problems with Solutions                                                                 121




or


             v。=501- 40 V.


It follows that v。will pass through zero when t = 800 ms. (Note: The op a叩 will saturate when v。=
40Vort = 1.6s.)


Problem 8.10
        a) At the time the switch makes contact with terminal a in the circuit seen in the figure, the
charge on the capacitor is zero. The switch remains at terminal a for 3 ms and then moves
instantaneously to terminal b. How long after the switch makes contact 꿔ith terminal a is the output
voltage zero?
       b) If the switch remains in contact with terminal b, how many milliseconds after making
contact with termina比 d配s the 아）띠np sa恤ate?

                                                                            0.04 F




                         8V




Solution

         a) The initial value of v。is zero since the initial charge on the capacitor is zero. The fmal value
of％小(500/4.0) 8.y- 1어）V.（枷e: In pre小ctin酊卜．e final value of v0, ignore.th얏ossib夢的캇e
op amp saturating.) I tie time constant governing the uiscnarge or tne capacitor is (>uu x 1(T) U.U4 x
mr노b6\ 八＝1 n1l m= . mLmmmrmmm == .14m4 1 L. .. =1= J .小l ! .. !.4 =4 4＝뇨！m4 n it. ... ＝八I. . 1!._ C. 日 -. !=
LU   J1 UI LU U1 . I UGICLUIC WUCI1 LUC SWILcIL IS III 1 USILIU1I 4, LIIC SUIUIIUU 101 V0 15




             v,3= -100+ 10匕e5mV,                    05t53ms.

at t = 3 ms, v。= -13.93 V. Observe that the op amp has not reached saturation; hence at the instant
the s刃itch moves to position b vO is -13.93 V.
 122                                           Chapter 8/ 之esponse of First-Order RL and RC Circuits



        When the switch is in position b the final value of vO is + 100 V. (As before we ignore the
 possibility of the op amp saturating when predicting the fmal value of vO.) The time constant is still 20
 ms; therefore the expression for vO when t lies bet吼en 3 ms and the time the op amp saturates is

           vO = 100 + (- 13.93 - 100)eH50 (t小 0.003)


              = 100 - 113.93ee50 (t-0.어）3) V,     3 ms 5 t 5 t。,

where tO represents the instant the op amp saturates.
       The output voltage equals zero when

           113.93e小50 (t-0.凹3) = 100,

or

           t = 5.61 ms.

     b) When the switch is in position b, the op amp 네l saturate when vO reaches 15 V. To fmd out
how many milliseconds after the switch makes contact with terminal b, solve the equation

           100 - 113.93e小50A1 = 15,

where & represents the elapsed time after contact with terminal b has been made; i.e., & = t - 0.003.
      The elapsed time is thus

          & = 5.86ms.



Part C: Supplementary Problems

Supplementary Problem 8.1
In the circuit shown in the figure, the current and voltage expressions for t 2 0 are

          i= &e20甘A,        t 之0·
                               ，


          v= 240eH20V,        t 之0.
Part C: Supplementary Problems                                                                         123




                                         尸른
Find (a) 凡 (b) L, (c) T (ms), (d) the initial energy stored in the inductor, and (e) the amount of
energy that has been dissipated in the resistor 100 ms after the current has begun to decay.


Supplementary Problem 8.2
The switch in the circuit in the figure has been closed a long time. At t = 0 it is opened. Find vO(t) for
t 之 0.




                      54V                                                         9011




                                2n




Supplementary Problem 8.3
For the circuit in the figure, what percentage of the initial energy stored in the inductor is eventu세y
dissipated in
       a) the 5-Q resistor;
       b) the 40-Q resistor; and
       c) the 10- 2 resistor?
124                                                 Chapter 8/Response of First-Order RL and RC Circuits




                                                              1011



                                       1
                                                        511
                                                        八八




                                             \!=.
                                                                     40 11   v。(t)
                                                    2




Supplementary Problem 8.4
In the circuit shown in the figure, the switch has been in position a for a long time. At t = 0, it moves
instantaneously from a to b.
       a) Find i (t) for t 之 0.
       b) Find the total energy dissipated in the 牛（2 resistor.




Supplementary Problem 8.5
The switch in the circuit in the figure has been closed for a long time. At t = 0 it is opened.
       a) Find SL(t) fort 之 0.
       b) Find VL(t) fort 之 0.
       c) Find i (t) fort 之 0.
                                                                                                       125
Part C: Supplementary Problems




Supplementary Problem 8.6
In the preceding problem, what percentage of the initial energy stored in the 100-mH inductor is
小ssipated in
       a) The 60-C resistor;
       b) The 20- 2 resistor; and
       c) The dependent voltage source?



Supplementary Problem 8.7
Both switches in the circuit in the figure have been closed for a long time. At t = 0, both switches
open simultaneously.
                (t) for t 之 0.
       a) Find 1。
       b) Find vO(t) fort 之 0.
       c) Calculate the energy (in microjoules) trapped in the circuit.

                                           (=0                         (=0
                               lOkfl                      5kfl




                  100 V                                                           4 kfl
 126                                           Chapter 8/Response of First-Order RL and RC Circuits



 Supplementary Problem 8.8
 The switch in the circuit in the figure has been in positionx for a long time. At t = 0, the switch
                                                                                                     moves
 instantaneously to positiony.
        a) Find vC(t) fort 之 0.
        b) Find V中（t) for t 之 0.




                                                                                  8 kfl




Supplementary Problem 8.9
In the preceding problem, what percentage of the initial energy stored in the 0.5-4uF capacitor is
eventually dissipated in
       a) the 8-kO resistor;
       b) the 160-kO resistor; and
       c) the dependent current source?



Supplementary Problem 8.10
The switch in the circuit shown has been in the on position for a long time. At t = 0 the switch is
moved to the ON position.
       a) Find the numerical expression for i (t) when t 之 0.
       b) Find the numerical expression for v(t) when t 之 0.
       c) Find the numerical expression for i3(t) when I 之 0.
Part C: Supplementary Problems                                                                       127




                                                                         2H




Supplementary Problem 8.11
The switch in the circuit in the figure has been closed for a long time. At t = 0 the switch is opened.
Find the numerical expression for i (t) when t 之 0.




 Supplementary Problem 8.12
The switch in the circuit in the figure has been closed for a long time. The switch opens at t = 0. Find
the numerical expressions for i (t) and v(t) when r 2 0.
128                                                  Chapter 8/Response of First-Order RL and RC Circuits




Supplementary Problem 8.13
The switch in the circuit in the figure has been open a long time. The switch closes at t = 0. Find v1(t)
for t 之 0.


                                          2fl            4n            2.6 H




                       74 V




Supplementary Problem 8.14
The switch in the circuit in the figure has been open for a long time. The switch closes at t = 0.
       a) Find the numerical expression for the voltage across the terminals of the capacitor for t 之 0.
       b) Find the numerical expression for the source current i (t) for t 之 0.


                                                        20 kf)




                                          「     “「         『O
                                                           8 0k1      +
                                                                      Vc7h5o   f


                              12+ ,   i
Supplementary Problem 8.15
The s꿔it比 노 the circt血 血 the f蜘re has been in posi如n a for a lo叩的e. At t = 0 the switch is
moved to position b. Find VC(t) when t 之 0.
Part C: Supplementary Problems                                                                           129




Supplementary Problem 8.16
The switch in the circuit in the figure has been closed for a long time. At t = 0 the switch is opened.
       a) 찌hat is the initial value of i (t)?
       b) What is the final value of 1(t)?
       c) What is the 由妃 constant of the circ山 fort 之 0?
       d) What is the numerical expression for 1(t) when t > 0?
       e) What is the numerical expression for v(t) when t > 0?


                                            2 kfl                                        800 c



                             b 0y                                                                2 ／工F




 Supplementary Problem 8.17
The switch in the circuit in the figure has been in position b for a long time. At t = 0, it moves
instantaneously from b to a. Find vC(t) for t 5 0.


                                    25k11           l6kfl




                     300 V                      60 kn

                                                            0.25 1iF   가
                                                                       1
                                                                                   (t)
                                                                               v
                                                                           1
 130                                           Chapter 8/Response of First-Order RL and RC Circuits



 Supplementary Problem 8.18
 The s析tch in the circuit in the figure has been closed for a long time. Find the capacitor voltage v
                                                                                                      (t)
 for t 之 0.


                                                          5n         10 fl



                                                                               15／小




Supplementary Problem 8.19
The switch in the circuit shown in the figure has been in position a for a long time. At t = 0 the switch
is moved to position b, where it remains for 10 ms. The switch is then moved to position c, where it
remains inde凡血啣．
        a) Findi (0+).
        b) Find i (8 ms).
        c) Find i (16 ms).
        d) F油d 町1丁 邱）.
        e) Fmd
           F뇨dyv (l0
                   (10 + ms).

                                                                     9c




Supplementary Problem 8.20
In the circuit in the figure, switch 1has been in position a for a long time and switch 2 is open. At t =
0, switch 1 moves instantaneously to position b while switch 2 remains open. Eight milliseconds after
switch 1o心ates, switch 2 closes.
       a) Find vC for 0 5 t 5 8 ms.
       b) Find v for 8 ms 5 r 5 oo.
Part C: Supplementary Problems                                                                      131




Supplementary Problem 8.21
The gap in the circuit in the figure will arc over whenever the voltage across the gap reaches 12,000 V.
The initial current in the inductor is zero. How many milliseconds after the s꿔itch has been closed
will the gap arc over?




                        100 V
                          Chapter 9
          Natural and Step Responses of RLC Circuits


Part A: Representative Drill Exercises with Solutions

Drill Exercise 9.1
The element values in the circuit in the figure are R = 400 Q,L = 50 mH, and C = 50 nF. The initial
current in the inductor is -4 A, and the initial voltage on the capacitor is 0 V. The output signal is the
voltage v. Find（旬 IR(O); (b) ic(O); (이 加（0)／꺄 (d）山；(e) A2; and (f) 叩) whent 之 0.

                                                                                                        +
                                                                기                           卜   m
                                                                                                1
                                                                                                    +



                                                                                                             l
                                                                                        t
                                                                                                1
                                                                             『
                                                                                                        >>
                                                                                                    V
                                                                                                尸
                                                                C   TVO
Solution
        a) There cannot be an instantaneous change in the capacitor voltage or the inductor current.
Therefore the initial voltage across the resistance is zero and it follows the initial current in the
resistor is zero, thus iR(O) = 0.
       b) There can be an instantaneous change in the capacitor current. Since iC + iL + iR must
sum to zero at every instant of time it follows that iC(O+ ) = 4 A.
        c) Since the initial capacitor current is known we have


                                                        ) 凹 x 1。
                                                               6
                                                                                    V
                                       =    'C   (Q
                                                                                    S
          dv           (O
                                  ')
                                                            =
                       a                              c
                                                                                    e
                                                       '
       d), e), and 1) For the given values of尺 L, and C we find the roots of the characteristic
equation to be sl = -10,000 rad/s and s2 = -40,000 rad/s. Therefore the voltage response is
overdamped. That is,

                                           10,어01                            0001
          v=
          y                                                +a2e
                                                           +A2e
                                                                      -40,
               =Ale-
                            A1e
                                                                                                                 133
 134                                                                                                                   Chapter 9/Natural and Step Responses of RLC Circuits



 We fmdA1 andA2 from the initial conditions

                   v(0+) =A1+ A2 = 0,

 and

                   dv(0+)                        . nnnn .                                      . nn,,n .                    nn ' . . n6
               =     -.1m = - IU.UWA1 -                                                        '11J.U.RJA) = 5U X IU
                     di         "   1                                                              "     H


        The solutions forA1 andA2 are


              小＝짹29V                                           and A2= U앉，刃o v.
                                 3                                                                        3



Substituting the values ofA1 andA2 into the e시：)ression for v gives



              「＝
                         빻
                                     ［
                                             『
                                                 “       '"'   的－
                                                                                   .‘的，
                                                                                                     曲］
                                                                                                                  v,
                                                                                                                                    (20.


Drill Exercise 9.2
In the circuit shown in the figure, R = 250 c2, L = 0.32 H, C = 21tsF, Jo = = 0.5 A, V0 = 80 V, and
I = -1.5 A. Find (a) iR(O+); (b) i (0+); (c) diL(0+)/dt; (d) s1,s2; and (e) IL(t) fort 之 0.



                                                                              r=
                                                                                                                       il   _
                                                                                                                                    C      "
                                                                                                                                               '}
                                                                                                                                                    L   A
                                                                                                                                                            니m




                                                                                                                                                            V



                                                                                                                                                            1



Solution
        a) The initial voltage across the resistor is 80 V and it cannot change instantaneously because it
is the same as the capacitor voltage. Therefore the initial value of the resistor current is iR(O +) =
80/250, or 320 mA.
        b) From Kirchhoff's current law we know 1L + iR + 1c = I at every instant of time.
Furthermore we know the inductor current cannot change instantaneously; hence

          .        ／八＋       \           d           戶              』1   八八               '1    戶n


          'C(U ) = 中lD 中 (Li乙 - U.NI = H乙3乙 /\ ·
                                                                                                              1        44       .
Part A: Representative Drill Exercises with Solutions                                                    135




       c) The initial voltage across the inductor is the same as the capacitor voltage; therefore

         LdL
           L               )          ,       , ,        L    0
                                                                               25。A/
                                    8。
                                    凹
                                                              (.
                                                         .
                                                              (O
                                                    dI
                                                                   +
         L
                 (,
            d1
                 (O
                                                                           =
                                                             口(
                                      .

             nr
                  .             =
                                                                                       s.
                                                                       )
                                              。r
                                ＝
                           )
                      0+
       d) For the g如en va佃es of尺 LandC

          s1= -1띠）+j750rad/s                             and               s2= -1伉乂）-j750rad/s.

      e) Since the roots of the characteristic equation are complex, we know the current response is
underdamped; therefore iL(t) will have the form


          iL(r) = ir+ De     coswdt/ + i)2e
                      i)le-atCOSW             smwd,
                                       D2e -atS.
where a = 1000 rad/s and wd = 750 rad/s.
      The final value of iL(t) will be the source current, or -1.5 A. The values of D1 andD2 are
determined from the initial conditions, namely

          'L (O+) = 0.5 = lf+ D1

and

          dL(O+) = 250 = -10001기 + 750D2

We fmd D1 = 2 A and D2 = 3 A; therefore the numerical expression for IL(t) is

          LL(t) = -1.5 + 2e小1以0tcos750t + 3ee1000tsin750tA,                                  t之 0.



Drill Exercise 93
       a) Find the equation for vO(t) for 0 5 t 5 t Sat in the circuit shown in the figure if vO1(0) = 2 V
          and vO(0) = 8V.
       b) How long does it take the circuit to reach saturation?
                                                             0.1 FLF




                                    250 kfl



                           V9




                                                                                                     V
136                                                                          Chapter 9/Natural and Step Responses of RLC Circuits



Solution

        a) The analysis of the circuit in the figure is discussed in Section 9.5 of the text. The
relationship between,the output voltage vO and the input si叩al Yg is given by Eq. (9.78). For the
numericai vaiues 01八l, Ll, 八2, ana L2 we nave


           d2v。
                               =
                   乙
           =11=            m             乙．
                      1．

                  口I

The solution of this second-order differential equation is discussed in Example 9.13, where the
notation g(t) = dvO/dt is introduced. We have from Example 9.13 that

          g(t) = 2t +g(O),

whereg(O) = dvO(O)/dt.
        The first step in the solution of the problem is to find dvO(O)/dt when vO1 = 2 V. From the
circuit diagram in the figure we see that at t = 0 the current in the l-d小 capacitor will be the same as
the current in the 500-kQ resistor. Assuming the reference for both currents is from left to right, we
have


          1500 k2                  (O)
                                              :
                                                  ii胛  （0)
                                                             ＝
                                                                 욺／
                                                                      io "
                                                                        "    :
                                                                                 4肛A·

The capacitor current is related to the output voltage via the expression

          .         , dvO
          11uF == m吐／二e
                  "                               Ui



       Note the minus sign is in agreement with the reference direction of ii/{F and the polarity
reference for vO. It follows that

          dvO
          二I'口 (U) == -4 == g(U)
          Ut



and

                  쁘m
                           =21- 4.
Part A: Representative Drill Exercises with Solutions                                             137




The solut白noftli心 血計order d姸erential equation can be 面帥妃d by separ玳旽 variables a끄（I
integrating. We get

          小b = 21dt 小 4dt,

or

                                                .    .       .        /，뇨＼


          VO = I                        -'卜r 十 已式Ii)
                               .2
vO(O) is given as 8 V; therefore

          vO=
          %=r2t -4t+ 8                                                   05t5f凹t.

        b) From the circuit in the figure, we see that the second 아）카I叩 毗Li sa曲ate wh이I v1, rea比es
 + 9 V. Therefore we solve the quadratic equation

                               1    -   .       』m               1l


          I             -'It            十6 = y}
              .2
or

           t =2 t \T. S.

Negative values oft have no physical significance; therefore

           rSat = 2 + V3 斗 4.245.

 Also note no real values oft will cause the op amp to saturate at -9 V.
       Finally we must check and see if the first op amp saturates before 4.24 s because our solution
 assumes that each op amp operates within its linear region. From the solution of Example 9.13 we
 know

                   dvO1 =                   -
                                                    1
                    出
                                                         '




 Therefore

                   dvO1 = -dt
138                                                           Chapter 9/ 寸atural and Step Responses of RLC Circuits



and

           vol    = -1+ v0l(0)


                  = -t +2.

At t = 4.24 s, v。
                1 equals -2.24 V, and since the first op amp saturates at -5.0 V, the second op amp
reaches saturation first.



Part B: Representative Problems with Solutions

Problem 9.1
The natural voltage response of the circuit of the fi엣re is

          v = 50e1凹'000' (cos 80,0001 - 1.2 sin 80,0001) V,                          t之 0.




                                                                                 i
when the capacitor is 0.02pF. Find (a) R; (b) L; (c) V0; (d) / o; and (e) iL(t).


                                                             91L
                              c_
                                        [+.
                                              V。
                                                   「
                                                   L
                                                       r7.
                                                                   1。
                                                                        '"   i
                                                                                                    1
                                                   L
                                                                                                中
                                                                                        +V
                                                             111
                               C_
                                    r
Solution

       a) From the expression for v we know a is 60,000 rad/s. Therefore [1J(2RC)J = 60,000 and
since C = 0.02pF it follows that R = 416.67 Q.


,，乙 茄岑豁xCpre穹
          。)4. f ：烈然뺏，
            and叱“，   ，『必急，‘喆쓰沽"" "" """
       c) It follows directly from the expression for v that v(0) = 50 V.

       d) The initial current in the capacitor equals qdv(o)/dtj. The derivative (dv/dt) is found to be

           쁘
           m = 50 x l03e卞印，여Xy [ -156 cos 80,0001 - 8 sin 80,0001] ,
                                                                                                          139
Part B: Representative Problems with Solutions




fr。m which Edv(0)/dtl = -7.8 x 106 V/s. It follows that the initial canacitor current is (0.02 x
                           1 <dr ==4 A
lu  ")(- 기
mrle6\ /
               X 1U") or -1>b mA.
             0 뇨／ 11)6\ 八；
          'i.S
         From part (c) we know the initial voltage across the resistor is 50 V; therefore the initial
resistor current is 50/416.6工 or 120 mA. 助 defi血如n, i is the 油tial curren山 the induc恤．Since
                                                                                               for the
七(0) and iR(O) have been determined we can use Kirchhoff's current law to establish that
circuit in the figure

          10 = H'R(O) - ic(0)


              = -120 + 156 = 36 mA.

       e) As noted in (d) the inductor current in the circuit in the figure is

          包（1) = 中'R(t) - i (t) .

But iR(t) = v(t)IR and i7(t) = qdv(t)/dt] and v(t), R1 and C are known. Thus we can compute jL(t).
We qet

                                    尸
                       -風）.0001 r -'』    nr1 J\J\i＼』 . 4 尸八 . n1\ r\r뇨r1. 1 1   . 느 r1
           ii人1) = e      '     L Jo cos ou,u1月丑 十 1:）乙 sin 6U,(R只JtJmA,        t =u.




Problem 9.2
 The two switches in the circuit seen in the figure operate s押chronously. When switch 1 is in position
 a, s꿔itch 2 is in position d. When switch 1 moves to position b, switch 2 moves to position c, and vice
 versa. Switch 1 has been in position a for a long time. At t = 0 the switches move to their alternate
 positions. Find vO(t) for t 之 0.



                                                                                         1 kfl
                       40 V




 Solution
 With the two switches in the circuit in the figure in their initial position, the capacitor acts like an
 open circuit and the inductor acts like a short circuit. This follows because the switches have been in
 their initial position a long time. It follows that the initial voltage on the capacitor is 40 V, positive at
 the upper tern如毗 and the initial current in the induct야 is 20 m人 야妃nted from t아tO bott帥．
         After the switches operate, the capacitor, resistor, and inductor are placed in parallel. The
 numerical values of R, L, and C are known, so the roots of the characteristic can be calculated for
 140                                                  Chapter 9/Natural and Step Responses of RLC Circuits



 t > 0. The roots are -20 radjs and -80 rad/s. Since the roots are real and 小stinct, we know the
 solution for vO is of the form

                             201
           %
           vO=                     +a2e
                                   +A2e
               =4le-
                                          -801
                       A1e
Now the initial conditions are used to findA1 andA2.
       The initial current in the resistor, oriented down, is 40/500 or 80 mA. The initial inductor
current is 加 mA; therefore the initial current in the capacitor is -100 mA. The minus sign me帥s the
reference direction for the capacitor current is down.
       Once ic(0) is known, we can find dvO(0)/dt; i.e.,

           吼,(0)＝쁘 = 1照刃V/s.
            口t               C


We can now write

           vO(0) =A1 +A2 = 40

and

           dvr)(0)
              ." = -2th41 - 804, = -5000.
             at         -      日

鈿lvi昭的r月land A2 gives小 = 羽 VandA2 = 70 V; therefore

           v (t) = -3'J匕-20t+ 7C匕-80'V ,              t之0.


Pr야)lem 9.3
In the circuit in the figure, the resistor is adjusted for critical damping. The initial capacitor voltage is
50 V, and the initial inductor current is 200 mA.
       a) Find the numerical value of R.
       b) Find the numerical values of i and dt/dt immediately after the switch is closed.
       c) Find vC(t) for I 之 0.




                                                 V+
                                                  C
Part B: Representative Problems with Solutions                                                       141




Solution

       a) In the series circuit shown in the accompanying figure, critical damping occurs when a2 =
w02, where  a (R/2L) and w0 = (1/LC). For the given values of L 띠ld C we findR = 100O.

         b) The initial inductor current is 旦iven as 200 mA and therefore 1(0k ') = 200 mA. To find the
initial value of di(0 + )/dt we first fmd the voltage across the inductor at t = 0+.
         Since the initial capacitor voltage is known to be 50 V we can use Kirchho什s voltage law to
fmd the voltage across the inductor. If we reference the inductor voltage positive at the left terminal
of the inductor, we find

          VL(0+)= 50- 100 (0.2) =30V.

But vL(0+) = L[di(0+)/dt]; hence


          二：
               (0+)
          di二二그 =      v,(0+)        ..
                        U : ' = 1fl1 A/ c.'
               dt         L              '.

       c) To find vC(t) for t 之 0 we first find 1(t), and then u鈿g Kirchho作s voltage law we can w虹e

            ..    , di(t)
          VcI() = L 寸； 1 十 入mJ ·
                           U'



By hypothesis the circuit is critically damped, so we know i (t) is of the form

          i (t)
            (r) = D1te
                  Dlie中s어Xy +i)
                             D2e2e -sooc

D1 and D2 are found from the initial conditions. Specifically,

          1(0) =D2 = 0.20 A

and


          뽕＝          D,   －    跏따30   (刃·

Therefore D1 = 4000 A/s andD2 = 0.20 A.
      The expression for 1(t) becomes

          1(1) = (400t +0.20)e牛5띠iA,          t 之 0.
 142                                                        Chapter 9/Natural and Step Responses of RLC Circuits



 Substituting this equation into the equation for VC(t) gives

           vC(t) =(2X 1Q5t+ 50)e15띠iA,                        t之O.


 Pr야)lem 9.4
 The switch in the circuit of the figure has been in position a for a long time. At t = 0 the switch moves
 instantaneously to position b.
        a) Find vO(0+).
        b) Find dvO(0+)/dt.
        c) Find vO(t) fort 之 0.

                                                                b    1 kft




                           400 mA




Solution

        a) Since the switch has been in position a for a long time just prior to moving to position b the
capacitor acts like an open circuit and the inductor looks like a short circuit. Let vc be the voltage
across the 1.75-kQ resistor, positive at the top. Now sum the currents away from the upper terminal of
the 1.75-kg) resistor. Then at t = 0e we have



           -0.4* "얹 )。* v"(O늚꾜刃：..
Solving for VC(0h) gives 350 V.
       Now let IL represent the current, left to right, in the 10-mH inductor. Then at t = 0中

                     ) = 350           00
                                                     20A.
               (0'
                               ;
                                   /
          'L
                           2
                                                0.
                                            =
When the switch moves to position (b), neither the voltage on the capacitor nor the current in the
inductor can change instantaneously; therefore vC(0+) = 350 V and iL(0+) = 0.20 A. Also note that
when the switch is in position b the equivalent resistance in the circuit is (100이(250)/1250, or 2002.
Now the value of vO(t) at t = 0+ can be computed. Thus
Part B: Representative Problems with Solutions                                                           143




          vO(0+) = 350 - 200 (0.20) = 310 V.

       b) When the switch is in position b, Kirchhoff's voltage law tells us that

          vO(t) = VC(t) - 200 ZL(t) ,

where vC(t) is the voltage across the capacitor, positive at the upper terminal, and IL(t) is as defmed
before. It follows directly that

                                                        diL
                                            )
                          =
                                                    2。。
                                                    200
                   (t)                                      (t
                                       (t
            dvO
                              dvc
                  at                 at                   at
                                                H
                                                -                )
Therefore

          小C(0+
           c(0 =                     丸 （0') -2。
                                              。旽 （0') .
            at                         at        at

The value of [dvC(0 + )/dt] can be easily determined because the initial current in the capacitor is
identical to the initial current in the inductor; thus

           dyC(0+) -.．二으2 = e2
           dvc(O            -2 Xx 10
                                  l05 V/s.
                   dt         尸 10小

The minus sign in the expression for [dvC(0 + )/dtj reflects the fact that the reference for iL(t) is in the
direction of the voltage rise across the capacitor.
       To find [diL(O + )Idt] we use Kirchhoff's voltage law to find the voltage across the inductor at
t = 0+. If the polarity reference for this voltage is positive at the left terminal we can write

             -350 + 0.2 (200) + vL(0+) + 300 = 0,

or

                  . 八＋.             .n, ,           , diL . 八＋.
           VL(U ) ==1UV ==L ==(U                                 ).
                             UI


It follows that

            d1L(0+)                  10 x i03
                                              = 1000 A/s.
               dt                       10
144                                                      Chapter 9/Natural and Step Responses of RLC Circuits



       When the numerical values of dvC(O + )/dt and diL(0 + )/dt are substituted into the expression
for dv。
      (O+ )/dt, we find

          dvO(O+) -          A1V (VV,FI
                        -   H 1W少八八J vIa.
               dt

       c) To find the numerical expression for v。 (t) fort 之 0 we must first find the roots of the
characteristic equation when t > 0. For the circuit in the figure a = R/2L = i04 and w8 = 1/LC =
lOs. Thus a2 = w弓 and the response is critically damped. The form of the solution for vO(t) is


          vO(t)   V/ (D1'
          V, (r) =vf+ (Z기’ +D2')e
                            Z万） -104t

After the switch has been in position b for a long time, we see from the figure that v。
                                                                                      (t) is 300 V;
therefore vf = 300 V. The constants D '1 and D '2 can now be computed because vO(0 +) and
dvO(0 + )/di are both known. We find

          vO(0+) = 300 + D2' = 310

and



          ""‘芬 = -10뇨' *D1' = -400，어刃·
               m+   \




Therefore D'1 = -3 x i05 V/s andD'2 = 10 V. It follows that

           . ..       . r. .,.           八   , n5J -104t, ,
          V叭t) = J（人J 十        [1U   m   iX1U   (J   C                 '




Part C: Supplementary Problems

Supplementary Problem 9.1
The natural response of the circuit shown in the figure is known to be

          V= 5（匕-St小9fJm4StV ,                  t 之0.

Find iL(0+).
Part C: Supplementary Problems                                                                      145




                                                                         +
                                 H

                               쁘9             尸
                                                                         V

                               \／之／7111       >>\11
                                                         T2   .   5 mf   1




Supplementary Problem 9.2
In the circuit in the fi햇re, a 50-mH inductor is shunted by an 80-pF capacitor; the resistor R is
adjusted for critical damping; and V0 = 5 V and I = -0.4 mA.
       a) Calculate the numerical value of R.
       b) Calculate v(t) for t 之 0.
       c) Plot v(t) vs. t for 0 5 t 5 10us.
       d) What percentage of the total energy stored in the inductor and capacitor remains 5 Aus after
          the initially stored energy has begun to dissipate?




Supplementary Problem 9.3
In the circuit in the figure, the initial energy stored in the inductor is zero, and the initial energy
stored in the capacitor is 153.6 4uJ. The circuit elements are R = 5 kQ,L = 120 H, and C = (10/3) uF.
       a) Find jL(t) fort 之 0 if the dc current source is 4 mA.
       b) Find the ma址mum value of IL(t).
       c) Find the time (in milliseconds) at which the ma虹mum 어：curs.




                       上m了                        1내六l
                                                                                  .
 146                                              Chapter 9/Natural and Step Responses of RLC Circuits



 Supplementary Problem 9.4
 Switches 1 and 2 in the circuit in the figure operate sync뇨onou啣. When switch 1o꺄뗘 switch 2
 closes and vice versa. Switch 1has been closed for a long time. At t = 0, switch 1 opens. Find


        b) dva(0+)/dt;
        c) Va(t) fort 之 0.


                             50011                    t==0


                                                                                 0.25 H
                                                             山nn붇   55 P, FF 小            r+
                                                   "그 「'
                  150 V



                          7 "J                                                    1.0H논
Supplementary Problem 9.5
The initial energy stored in the circuit in the figure is zero.
        a) Find the roots of the characteristic equation.
       b) Find the capacitor voltage for t 之 0.
        c) Find the inductor current for t 2 0.




                                                                           +
                                                                            VC




Supplementary Problem 9.6
The switch in the circuit in the figure has been closed for a long time. At t = 0, the switch moves
instantaneously from a to b. Find vC(t) for t 之 0.
Part C: Supplementary Problems                                                                        147




                                                    1t)        125 (1




                  50 V                                                                      137.5 V




Supplementary Problem 9.7
The switch in the circuit in the figure has been in the ON position for a long time. The switch is moved
to the on position at t = 0. Find the numerical expression for VC(t) when t 2 0.

                                               0N
                                20 (1                                              240 (1
                                A 八 八




                         1 kV       480 (1 二




Supplementary Problem 9.8
The switch in the circuit in the figure has been closed for a long time. Time is measured from the
instant when the switch is opened.
       a) Find the numerical expression for VL(t) when t 之 0.
       b) Find the ma虹mum value vjjt).

                                                             t =0



                                                                        2.6 (1


                                                    0.5 尸F                         +
                                   T    1


                                12 V =e                                   5.8 mH
                               Chapter 10
                     Sinusoidal Steady-State Analysis


Part A: Representative Drill Exercises with Solutions

Drill Exercise 10.1
A sinusoidal voltage is given by the expression

          v = 40 cos (2513.27t + 36.8尹) .

       Find (a)f in hertz; (b) Tin milliseconds; (c) Vm; (d) v(0); (e) 中 in degrees and radians; (f) the
smallest positive value oft at which v = 0; and (g) the smallest positive value oft at which dy/dr = 0.


Solution

       a) From the given expression for v, cv = 2513.27 rad/s; thereforef = 2513.27/2ir or 4伉）Hz.

       b) Since T = 1/f the period is 2.5 ms.

       c) The ma虹mum value of v is the coefficient of the cosine function; hence Vm = 40 V.

       d) v(0) = 40 cos 36.870 = 32 V.

       e) From the given expression for v, 中 = 36.87' or 0.6435 rad.

       f) The first time v will equal zero fort > 0 will occur when the argument of the cosine is 90" or
1.57 rad. Therefore we find t such that 2513.27t + 0.6435 = 1.57, or t = 368.96 us.

       g) The first time (t > 0) that the derivative of the cosine function is zero is at the time the
voltage is at its mi如um value. This will occur one-quarter of a cycle after the voltage passes t뇨ough
zero. Therefore

          t = 368.96 + (1/4) (2500) = 993.961us.




                                                                                                     149
150                                                          Chapter 10/Sinusoidal Steady-State Analysis



Drill Exercise 10.2
The voltage across the terminals of the 0.2-4uF capacitor is 40 cos (105t - 50O) V. Calculate (a) the
capacitive reactance; (b) the impedance of the capacitor; (c) the phasor current I; and (d) the
steady-state e사｝ression for 1(r).


                                                75 mA
                                             11Y＼ 사＼  11=+
                                             +    V      寸


                                                  ＝卜
Solution

.     . . 咐叩햐蜜．en e柳쓰如for v we have cv = ios耐s. T岫efo【야he capac姓ye reactance
is -ij나rU. 乙 X It) V)J, or -)() 5J.


        b) The impedance of the capacitor isj x (capacitive reactance) or -j50 (2.

        c) I = V/(- j50). From the expression for v we see that V = 40 i -50g. J follows that I =
0.8 /    A.

        d) To inverse transform the phasor current note that it has the same frequency and waveform
as the voltage. The amplitude and phase an밈e of the current are given by its phasor. Thus

              江 0.8 cos (10斗 + 的DA.


Drill Exercise 10.3
Find the steady-state expression for vc. in the circuit shown in figure A if j口 = 0.8 COS 的0t A.
                 r      1             1/
                                                                   느尸       0




        (a)
Part A: Representative Drill Exercises with Solutions                                                151




Solution

The first step in finding vO is to fmd the phasor-domain equivalent circuit. From the expression for ig,
note w = 4000 rad/s. Therefore the impedance of the capacitor is -j40 Q and the impedance of the
inductor isj70 Q. The phasor transform of the current source is 0.8 LQ A. The phasor-domain circuit
is shown in figure B.

                                                               2;
                                                      多二나之                 匕J2-
                             O.81 "4                                +

                                                   -44&r?.          15

       (b)

       Current division can be used to find the phasor current lo; thus

                 [o.   8四：     ] [30-   140]
                                               j70) =0.8j크0A
             10= (30H j40+ 10+

The phasor voltage V0 isj70 10 or 56 LQ V. It follows that

             v。= 56 cos 4000 V.


Drill Exercise 10.4
The parameters in the circuit in the figure are R1 = 0.1C, wL1 = 0.8 ), R2 = 24 C, wL2 = 32 Q,
andVL = 240 +jOV.
       a) Calculate the phasor voltage V.
       b) Connect a capacitor in parallel with the inductor, hold L constant, and adjust the
          capacitor until the ma留itude of I is a minimum. What is the capacitive reactance? 찌hat is
          the value of V5?
       c) Find the value of the capacitive reactance that will keep the magnitude of I as small as
          possible and at the same time make 1 V3 I = I Vi. I = 240 V.
 152                                                       Chapter 10/Sinusoidal Steady-State Analysis




        (a)
Solution

        a) For the given values of the circuit parameters in the figure we get

                  240 / 伊
              L= 24匣＝10／으A,


              已援＝7·斗卯'A·
It follows from the figure that

              1= 'a + 1b = 10 - j7.5 A,

and

              艮= VL + (R1 + jwL1) 1


                = 24이Q + (0.1 +10.8) (10 -17.5)

                = 247 +j7.25 = 247.11/ 1.68 V.

        b) The magnitude of I can be minimized by using the capacitor to balance out the current in
the inductive branch. Referring to figure B we see that L must equal j7.5 A because then I = 10 -
j7.5 + j7.5 = 10 LQ A . It follows that the impedance of the capacitive branch must be 240/Q7.5) or
 -j32 Q. Thus the capacitive reactance is -32 (2.
Part A: Representative Drill Exercises with Solutions                                                    153




                                          H+
                                                                                        'b     ]
                                                               VL                joL2
                                                                                             jo,C ／戶＼\


                                                                .


       (b)

       The new value of V is

             V = 204 LQ + (0.1+ j0.8) 10 匹

                  = 241 +j8 + 241.13i1.90으V.

       c) Refer to figure B and let 'm denote the magnitude of the current in the capacitor branch.
Using this notation, the line current can be written

             I = [10 +j (Im - 7.5) ]A.

By hypothesis the magnitude of the source voltage is 240 V. If we let a denote its phase angle we can
write

             V5 = 240 坦 =240+ (0.1+ j0.8) E10+ j (Im+ 7.5) ]


                  = (247 m 0.8Jm) + j (7.25 + 0.1(m)

It follows that

                                                                             l
              .       r .八.n n ,, 1 .) . .月八尸 . ,, . 1 .ni
             2的 =    [   (247   -   0.   8 1mJ +
                                               .   '   (7.   25 + 0.11rnY]   '




       Now square each side of this equation to generate the following quadratic equation

          ／刃i2 - 605.771m + 5325.48 = 0,

or

             7r7i= 302.88 士 293.96.

The smallest value 0 'm is 8.92 A. We have then that ZC = 240Ij8.92 = -j26.90 Q. The capacitive
reactance is -26.90 c.
154                                                                                        Chapter 10/Sinusoidal Steady-State Analysis



Part B: Representative Problems with Solutions

Problem 10.1
Find Zab in the circuit shown in figure A when 由e circuit is operating at a frequency of 10 krad/s.

                                                       -            V.,   +


                                                           1.6mH  530fl
                                   a e1/                    YY＼入山／ 八H




                                   bs                                             T
                                                                                      2.
                                                                                           5" F        令
                                                                                                                   08v.
                                                                                                                      ,



       (a)
Solution
To fmd Zab we first construct the phasor-domain equivalent circuit and then apply a test source
across the terminals a, b. At 10 krad/s the phasor-domain circuit, with the test source, is as shown in
figure B.
                                                                              K

                           I：
                                                                              +   5又）J2.
                                                                          27戶     f人／
                                                  仄＝
                      V ( t)
                               了
                                       '                                  小뇨1            {                 .




                                                                                  仁7" "y'尸I그吼뇨
                                                                                                               .
                                                                                                  그．
                       T   T
                                                       二
                                                                                                                          4
                                                                                                                              o.
       (b)

       From the circuit in figure B we have

                VT = (530 +jl6)1T + (- j40) [IT + 0.8V,] ·

But V = -j16 'T. (Note: The minus sign is necessary because the reference for 'T is in the direction
of the voltage rise Vs.)
        Now we can solve for the ratio VT/IT, which by definition is Zab; thus



             午z小18
                                   -       j24＝
                                                           羽스3建O·
Part B: Representative Problems with Solutions                                                           155



Problem 10.2
The frequency of the sinusoidal current source in the circuit seen in the figure is adjusted until the
voltage vO is in phase with ig. Find the frequency in ra小ans per second.




Solution

The voltage vO 꿔ill be in phase with the current 1g when the equivalent impedance seen by the current
source is purely resistive. Because the branches are in parallel, it is easier to work with the equivalent
admittance. The admittance will be purely conductive when會 is in phase with v0.
       The admittance seen by the current source is

                     1        . ..\ n ' . 4八m6
          y = 御胱1 +j8C匕) 十JU      'm)   X Lu


             =     印00.- j80wh뉘啣x                i0 6
                 36x100+ 6400w' '

The admittance will be purely conductive when

                  8.Ow      ' = 0.8w X i0_6
          36 )< 100 + 640C뇨J二

or w = 100 rad/s.


Problem 10.3
The ex江essions for the steady-state voltage and current at the terminals of the circuit seen in the
figure are

          Vg = 300 cos (500Qrt + 78') V
 156                                                         Chapter 10/Sinusoidal Steady-State Analysis



 and

               ig = 6 sin (500071t + 123') A.

             a) What is the impedance seen by the source?
             b) By how many microseconds is the current out of phase with the voltage?


                                                9




                                                               Circu仕




Solution

      a) The phasor transform of Vg is 3伉）L그竺 V. Before finding the phasor transform of 1g we must
change to the cosine format; i.e., ig = 6 cos (5000.ir t + 33') A. The phasor transform of ig is 6 L望 V.
The impedance seen by the voltage source is 300 /j / 6／至 , or 50 쓰望 Q.

      b) The current lags behind the voltage by 45'. The period of the sinusoidal functions is
2t/5000.ir or似야is. Now 45' is one-eighth of a period; therefore ig lags Vg by (1/8)(400) or 501us.


Problem 10.4
Use the node-voltage method to find the steady-state expression for v。
                                                                     (t) in the circuit seen in figure
AifL = 1.5mH, C = 200/31uF, Vgi = 400cos1仄0tV, andv2 = 300sin (1000 + 53.13') V.

                                 10 U                                     2O




                                                                                         2




       (a)
                                                                                                      157
Part B: Representative Problems with Solutions



Solution
The first step in finding vO is to construct the phasor-domain equivalent circuit for the circuit shown in
figure A. The circuit is shown in figure B where Vgi = 4兀世 uid Vg2 = 300 /                 V.




                      好4)
       (b)

       Observe that b = (V0 = 400)110 A; then the node-voltage equation can be written as

              V+ 4仄0        V    V   2 (V+ 400) V - 300 i- 36.870
                         + =＝느+ -f= + " 1,,   ' + V    -          = 0.
                 10        J1.> -)D      10            2

Solving for V0 gives

              V0= 90 /         V.

It follows that the steady-state solution for v。is

              vO(t) = 90 cos (l00河 - 53.13') V.


Problem 10.5
Use the mesh-current method to find the steady-state expression for vO in the circuit seen in fi햇re A
江 Vg equals 400 cos 5000t V.




        (a)
 158                                                              Chapter 10/Sinusoidal Steady-State Analysis



 Solution
 To fmd vO by the mesh-current method, we first construct the phasor-domain equivalent circuit. The
 circuit is sho지Vn in figure B where we have defmed the mesh currents Il 缸ld 12. Note from the figure
 that V0 = 100 12 and 1夕 = I1 HI2.




             (b)
                                      二1 牛口
             The two mesh-current equations are
                                                                              牛
                   400 / 0 = /300 L + 50 (I1 - In - 150 (I1 - I,')


                           = 150 (1i - 12) + 50 (12 - I) + (100 - 1100)12

Note that to fmd V0 we only need 12. Solving for 12 gives -1.6 + j0.8 A; therefore

               Vl = 100Im = -160 + 180 = 178.89 / 153.430 V.

The steady-state expression for vO is

               vO(t) = 178.89 cos (500t + 153.43') V.


Problem 10.6
Find the Th6venin equivalent circuit with respect to the terminals a, b of the circuit shown in figure A.

                                                            ion


                                     5L2



       (a)
                                                                                                      159
Part B: Representative Problems with Solutions



Solution

Let V1 be the node voltage across the dependent current source in the circuit in fi昏lre A. Observe
that the Thevenin voltage is V0 and that once V1 is known V0 is easily obtained. Specifically


          %=M=，커小
when the reference for V1 is positive at the upper terminal of the dependent current source.
       Summing the currents away from the upper terminal of the dependent current source
generates the equation



           -0.3[：크二：]* "; " + 1。-Vij2。＝『
SolvingforV1weget4 +j22 'VandhenceVt = 12 +j16 = 20/ 53.13V.
        When a short circuit is placed across the terminals a, b in the circ岫 in figure A, V0 becomes
zero, the dependent current is therefore zero and the short circuit current from a to b is

                   25 /00
              'Sc = 10 示 = 2- fl A '
It follows that the Thevenin impedance is

              Z1= V1/ISC = 1.6 +/8.8Q.

 The Thevenin equivalent is shown in figure B.

                                                   "7끄      J"8;8J乙


                              ；勿／奭宣／

        (b)


 Problem 10.7
 The operational amplifier in the circuit shown in the figure is ideal. The voltage of the ideal sinusoidal
 source iSVg = JCOSIU ( V.
 160                                                      Chapter 10/Sinusoidal Steady-State Analysis



        a) How large can RO be before the steady-state output voltage no longer has a pure sinusoidal
           waveform?
       b) For the value of RO found in part (a), write the steady-state e사）ression for vO.

                                                               80O




Solution

        a) The circuit is analyzed in the phasor domain by summing the currents away from the
inverting input terminal of the op amp. This gives the phasor output voltage V0 as a function of RO,
from which the critical value of RO can be ascertained.
       In the phasor 面main the voltage source becon妃s5 四으，the 2.S-M1그 capacit아 is a的叩edance
of -j40 Q, and the 5-uF capacitor is an impedance of -/20 Q. The phasor value of V2 is

          v ' = (5／으凡）
           '    R。-j20

Because the op amp is ideal, V1 = V2.
      The node-voltage equation at the inverting input terminal is

           Vi     V] -V
          布6+ '80 "=0 '
       When V1 is replaced by the expression for V2 the solution for VO as a func如n of RO is




      We see from the figure that the op amp will saturate when the amplitude of vO reaches 10 V.
Therefore saturation will occur when



         Iv기m
           = 10= VR.已
                                                                                                   161
Part C: Supplementary Problems



Sol油［lg for RO gives 40 Q.

       b) When R。= 40 Q, VO = 10 /        V; therefore the steady-state expression for vO is

          v。= 10 cos (104t + 900) V.



Part C: Supplementary Problems

Supplementary Problem 10.1
At t = -2 ms a sinusoidal voltage is known to be zero and becoming positive. This occurs next at + 8
ins. It is also known that the voltage is 80.90 V at t = 0.
       a) What is the frequency of v in hertz?
       b) What is the expression for v?


Supplementary Problem 10.2
Use the concept of the phasor to combine the following sinusoidal functions into a single
trigonometric expressions.
        a) y = 100 cos (800t + 120") + 60 cos (8001 - 150O)
        b) y = 50cos (300t + 30) -20sin (300t + 210)


 Supplementary Problem 10.3
 Find the impedance Zab in the circuit in the figure. Express Zab in both polar and rectan암llar form.




                                                           20 n
162                                                          Chapter 10/Sinusoidal Steady-State Analysis



Supplementary Problem 10.4
       a) For the 由cuit showi山 the fi昏ire, fmd the frequency (in ra小叩s per secon미 at w蜘h the
          impedance Zab is purely resistive.
       b) Find the value of Zab at the frequency of part (a).




Supplementary Problem 10.5
The phasor current I in the circuit in the figure is 3LQ A.
       a) Find 12, 13, and V.
       b) If w = iO5 rad/s, write the expressions for i2(t), i3(t), and v5(t).


                                       211




                                                                           6罕
Supplementary Problem 10.6
FindI0andZinthecircuitinthefigureifV2 = 40 +j30VandI = 6 匹亡A.
                                                                                                       163
Part C: Supplementary Problems




Supplementary Problem 10.7
Use the technique of source transformations to fmd the steady-state expression for v(t) in the circuit
in the figure. The sinusoidal voltage sources are given by the expressions

          v1 = 180 cos (400 - 36.87) V

and

           V2 = 150 sin 400t V.




 Supplementary Problem 10.8
 Find the Thevenin equivalent with respect to the terminals a, b of the circuit shown in the fi암｝re.
 164
                                                                    Chapter 10/Sinusoidal Steady-State Analysis




                                                      5c
                                                  十




                                                               啞｛1 1 人 戶（ \1
                                                           印


                                     n<
                                     0
                                              /
                                                  니
                      \＼二／ A                                                   -j2 L ：二   V2
                     (715&
                                          \
                                                                 >
                                      \
                                                       4V1


                                                                                               1b




 Supplementary Problem 10.9
In the circuit in the figure, v5 = 20 sin i04t V and i = 5 cos
                                                                (104t 卞 60O) A. Use the node-voltage
method to determine the steady-state expressions
                                                      for v1 and v2.




Supplementary Problem 10.10
Use the mesh-current method to find the steady-state
                                                     expression for y中 in the circuit in the figure ii Vg
= 400 cos 4000t V.




                                                                                  500
Part C: Supplementary Problems                                                                          165




Supplementary Problem 10.11
       a) Find the phasor voltage VO in the circuit in the figure.
       b) Does VO lead or lag the source voltage?

                                        ] O         j10 O




                          220世 V




Supplementary Problem 10.12
Find the Norton equivalent circuit with respect to the terminals a, b for the circuit shown in the figure.




                              5罕
Supplementary Problem 10.13
The operational amplifier in the circuit in the figure is ideal. The circuit is excited from an ideal
sinusoidal voltage source where Vg = 10 cos l0乂k V.
       a) Find the value of Rf that will make vO lag Vg by 90'.
       b) For the value of Rf found in part (a), write the steady-state expression for vO.




                          0.1 H
                          Chapter 11
          Sinusoidal Steady-State Power Calculations


Part A: Representative Drill Exercises with Solutions

Drill Exercise 11.1
Find the phasor voltage V (rms) in the circuit shown if loads L1 and L2 are 13 kVA at 0.8-pF lag and
10 kVA at 0.%-pF lead, respectively. Express V in polar form.

                                           厄5 f




Solution
To find the source voltage we must first find the source current. Once the source current is known,
出e voltage across the inductor can be computed. The voltage across the inductor pl出 the voltage
across the loads L1 and L2 equals the source voltage.
       First express the loads in terms of their complex powers. For load 1 the power factor is 0.8 lag;
hence the reactive factor is 0.6 and the complex power is

          Sl = 13 (0.8) + j13 (0.6) = 10.4 + j7.8 kVA.

For load 2 the power factor is 0.96 lead; hence the reactive factor is 0.28 and the complex power is

          S2 = 10 (0.96) 小 j10 (0.28) = 9.6 中 j2.8 kVA.

The complex power of the combined loads is

          ST ==51+ 52 ==20+ j5kVA.




                                                                                                       167
 168                                                 Chapter 11/Sinusoidal Steady-State Power Calculations



 The load current can be computed from the expres
                                                           sion

                 了T = (250 四) I.

 We get


                    = (20 +j
                           乙-'U
                               5) l0"= 8。+j2。

and therefore

                 I = 80 -j20A.

The load current is the same as the source current out
                                                       of the positive terminal.
       The source voltage can be found using Kirchhoff's voltage
                                                                   law, namely

                vs =250 亡뜨+ j0.5I


                   = 260 +j44J = 263.06 p8그5 V.


Drill Exercise 11.2
The source current in the circuit shown in figure A is 5 cos
                                                                  80001 A.
             a) What i叩edance should be connected across the terminals
                                                                       a, b for ma虹 um average
                power transfer?
             b) What is the average power that is transferred to the imped
                                                                            ance in part (a)?
             c) Assume that the load is restricted to pure resistance. What
                                                                             size resistor connected across a,
                b will result in the most average power transferred?
             d) What is the average power transferred to the resisto
                                                                     r in part (c)?




                                                                    1n
       (a)
Part A: Representative Drill Exercises with Solutions                                               169




Solution

        a) The impedance for maximum average power transfer to the terminals a, b is equal to the
conjugate of the Th6venin impedance seen from the terminals a, b. At the given frequency of 8000
rad/s the capacitor has an impedance of -j和 Q and the inductor has an impedance ofj8 Q. The
Thevenin impedance is


          乙＝j8+ 1앞크犁＋
                 Lu
                     1 = 10 + j5 Q.
                                   -J. :%)


Therefore for ma虹mum average power transfer the load impedance is 10 寸 j5 Q.

       b) To find the average power transferred we use the Th6venin equivalent. The Th6venin
voltage (positive at terminal a) is


          M=(5出片硼邱- j1和47·山크望？·
Therefore our problem is reduced to analyzing the circuit in figure B.

                                             /C)Jt   스 !>J2小   工




                                                                   b

        (b)

 The load current is

                  M而   幻                                                                                  =

              I = 굶 = 2.37＝그＆쏘은 A.
                           n
                               /
 The average power delivered to the load is

                       2

          니胃'10=28125W.
 170                                                      Chapter 11/Sinusoidal Steady-State Power Calculations



        c) If the load is restricted to a pure resistance the phase angle
                                                                           of the load impedance is fixed at
 zero degrees. In this case the best we can do is set the ma多li
                                                                 tude of the load impedance equal to the
 ma多litude of the Tbevenin impedance; hence

           R=
                     IztI
                                           =
                                                11.18Q.

       d) 꿔hen a load impedance of 11.18 + JO (2 is connected across
                                                                     the terminals a, b in fi因lre B
the load current is

                                Vt
                           18乙코1.7工A
           I= 21.18'+j5 口2.

and the average power is

                                          \ 2

          p=（三引 ".18:26.56W.
                /4
                            '        .-




We observe this is less than the power computed in part
                                                                   (b), as it must be.



Part B: Representative Problems with Solutions

Problem 11.1
The current source in the phasor-domain circuit shown
                                                         in the figure delivers 10.4 LQ A (rms).
       a) Find the average and reactive powers at the terminals of
                                                                     the current source.
       b) Is the current source absorbing or delivering averag
                                                               e power?
       c) Is the current source absorbing or delivering
                                                        magnetizing vars?
       d) Find the average and reactive powers associated with each
                                                                       impedance branch in the circuit.
       e) Check the balance between delivered and absorbed
                                                                average power.
       f) Check the balance between delivered and absorb
                                                             ed magnetizing vars.




                                                  4
                                                                   16 fl
Part B: Representative Problems with Solutions                                                       171




Solution
        a) To fmd the average and reactive powers at the terminals of the current source we first fmd
the voltage across the terminals of the source. The voltage can be found either by writing a single
n에e-voltage equation or by finding the equivalent admittance seen by the source and then using the
relationship V = IIY We shall use the later method. We have

             1 . 1 .    1      .n,, .,m』1.   . d3
         y = 三0 勻而 十 16 -j12 = 們J  -jIU)   X IU

and

          V:
                 [10.
                        4世7
                              （卯－
                                j70)
                                        /1丁 ']   =
                                                     72* I弱V,

where the reference polarity for V is positive at the upper terminal of the current source.
       Looking into the source from the right side of the source, the expression for the complex
power is

          S = -Yf = - (72 +156) (10.4)

               = -748.80 - j582.40 VA.

Therefore P = -748.80W and Q = -582.40 VAR.

       b) The minus sign tells us the current source is delivering average power.

       c) The minus sign tells us the current source is delivering ma多letizing vars.

       d) In the calculations that follow the reference direction for each branch current is down.
          res泣ive br口nc方

          ID =Y120 = 3.6 + 12.8 A


          SR = (72 + 156) (3.6 -12.8) = 416 + JO VA

Therefore the resistive branch is absorbing 416 W and no reactive power.
          inductive br口nc九

          li, = YIj10 = 5.6 - j7.2 A,


          Si』= (72 + j56) (5.6 + j7.2) = 0 + j832 VA.
172                                                                        Chapter 11/Sinusoidal Steady-State Power Calculations



 Therefore the inductive branch is absorbing no real power and 832 magnetizing vars.

mcan, ,use
        ,If w
          the畔，肥，崙受斗弗：黑뜹乷諱客ted뇨""'" ' "'"弱'h' 冊V的따凹出' " '"
                                        (660)
                                                 2     -




                                                       =   y· 乙斗 -   /l.   3乙 !
                           砥200 + j6,600

or

               Z= 9.24 +jl. 32Q.

If we assume the resistor and the inductive reactance are in parallel across the 660-V source, the

                                        2
          R = 岩읊）= 9.43)
                      //    /,1\




and

                             J)
                                                66Q.
          ,=
                  (
                      （乂乂JU
                                   2=
Problem 11.2
The circuit shown in the figure represents a residential distribution circuit in which the impedances of
the service conductors are n으liuible and V,1 = V) = 120 /00 V (rms). The three loads in the circuit
are L1, a coltee maker and a trying pan; L2, a room air conditioner, a flair aryer, ana a ruDe-type coior
TV set; and L3, a clothes dryer, a quick-recovery water heater, and a range with a se作cleaning oven.
Assume that all these appliances are in operation at the same time. The service conductors are
protected with 100-A circuit breakers. Will the service to this residence be interrupted? Explain.
Part B: Representative Problems with Solutions                                                       173




Solution
We begin by e사）ressing each load in terms of its complex power. In this circ血 all the loads absorb
real power, thus

         S1= (12刃 + 1196) +10 = 2396 +jOVA,


          S2 = (860 + 600 + 240) + JO = 1700 + JO VA,

          S3 = (4850 + 4474 + 12,200) +J0 = 21,530 +JOVA.

Let I, 12, and 13 be the currents, oriented down, throu합1L1, L2, and L3 respectively. Then

          I1 =2쬘姓뿌＝10.
             -
                     '07＋氾A,'
                120 LQ: -    -'. '         ',


         I,- ＝쭈， 악뿌小．17+JO A,
               1LUL L.

and

               21,530.+ j9
          13 = 二丙血
                1-1,. ,f0 = 89.71 +jOA.

In writing the expressio酊or 11, 12, and 13 we have taken advantage of kno的lg thej components are
zero ana [nereiore I = I
        Now define 1g1 and2 to be the current out of the positive terminal ofVg1 and V2 respectively.
Using Kirchhoff's current law we have

          181= 11+ 13 = 109.68 +JOA

and

          'g2 = 12 + 13 ’『 103.88 + JO A

Therefore the service will be interrupted because the service conductors are carrying more than
100 A.


Problem 113
A factory has an electrical load of 800 kW at a lagging power factor of 0.8. An additional variable
power factor load is to be added to the factory. The new load will add 160 kW to the real power load
174                                                Chapter 11/Sinusoidal Steady-State Power Calculations




of the factory. The power factor of the added load is to be adjusted so that the overall power factor of
the factory is 0.96 lagging.
       a) Specify the reactive power associated with the added load.
       b) Does the added load absorb or deliver magnetizing vars?
       c) What is the power factor of the ad小tional load?
       d) Assume that the rms voltage at the input to the factory is 2400 V. What is the rms
          magnitude of the current into the factory before the variable power factor load is added?
       e) What is the rms ma帥tude of the current i如 the factory after the variable power factor
          load has been added?

Solution
       a) Let S0 represent the initial value of the complex power delivered to the plant and S
represent the fmal value of the complex power delivered to the plant. Then from the statement of the
problem we have

          ,m    八，,n . . 800 . n /.       n八八 . .／八八． ,.
          )0 = out) 十 ) ;;; (U.t) = 猷人J 十 it乂只) KVA,
                         u.o

and

          ,1    ,,n, . .960 .,, 八，1.       ,,/n . .八，,n. , .
          햐 =   Ju 十 / ;;:;; (U.20) = ！灼U 十 )乙芍U KVA,
           1           iJ17U


Therefore the reactive power of the added load is

          Qadded = 280 - 600 = H320 kVAR.

       b) The added load delivers magnetizing vars to the plant.

       c) The complex power of the added load is

          Sadded = 160 中j320 = 357.77 乙姮3크望 kVA.

Therefore the power factor of the added load is

          Pfadded = cos (- 63.43') = 0.4472 (leading).

        d) Before the load is added, the current into the factory can be determined from the
relationshin 2400I二,..,= (800 + 160(fli03. Solving for Ic, . ,.,,, gives 333.33 - 1250 or 416.67 / -36.870
A.         '       啣J
                           '          "                V       ' M   "U   "   나   '             r
Part C: Supplementary Problems                                                                                                   175




                  Therefore the rms ma凹litude of the current into the factory is 416.67 A.

                  e) After the variable-power-factor load has been added, the factory current can be determined
rrnm mne rernmuncnin 乙u시u..口nhMm. = I?UII -I- 灼illi ii尸1 Or I. mtrM勺 Pnh1aIc 4 Ih .'hi / e 1f.. )h" A ." Iheretrs,e
껸 '---- .-V 1V---':'----'---t- - ' VV= lactory '니1J" -. J'-'-'-I11J ' '-- 11acrOiy 1/111114-口- --'.'." I= ====1 工 1.' 工1上1/11/11J11/
we rms magmtuae or mne current into mne tactory is again 'Ut.bI A.
      Note that in this case power-factor correction has allowed a 20% increase in average power
consumption without any increase in the magnitude of the line current into the plant.



Part C: Supplementary Problems

Supplementary Problem 11.1
The following sets of values for v and i pertain to the circuit in the figure. For each set of values,
calculate P and Q and state whether the circuit inside the box is absorbing or delivering (a) average
power and (b) magnetizing vars.

             a)
                    1J= 100 cos (口t + 3(JO) V,
                    i= 10 cos (cot + 60) A
        b)
                    17= 100 cos (cot - 450) \ T}
                    i = 10 cos (c玎 - 750) A
                  이 v = 100 cos (cot + 135) V,
                    i = 10 sin （口兀 - 95") A
                  m y= 100 cos (cot - 160) V,
                    i = 10 sin （口玎 + 45") A
                  이 y= 100 sin (cot + 140) V,
                    i = 10 cos （口기‘ + 95") A


                                                      十뇨
176                                          Chapter 11/Sinusoidal Steady-State Power Calculations




Supplementary Problem 11.2
A load consisting of a 6.254) resistor in parallel with a 513-mH inductor is connected across the
terminals of a sinusoidal voltage source vg, where Vg = 100 COS 5000t V.

       a) What is the peak value of the instantaneous power delivered by the source?
       b) What is the peak value of the instantaneous power absorbed by the so毗e?
       c) What is the average power delivered to the load?
       d) What is the reactive power?
       e) Does the load absorb or generate magnetizing vars?
       I) What is the power factor of the load?
       g) What is the react如e fact야 of th이oad?


Supplementary Problem 113
The current source in the phasor-domain circuit in the figure delivers 26立 A (rms).




                                                                        /5 n




       a) Find the average and reactive powers at the terminals of the current source.
       b) Is the current source absorbing or delivering average power?
       c) Is the current source absorbing or delivering magnetizing vars?
       d) Find the real (average) and reactive powers associated with each impedance branch in the
          circuit.
       e) Check the balance between delivered and absorbed average power.
       I) Check the balance between delivered and absorbed magnetizing vars.


Supplementary Problem 11.4
Find the average power dissipated in the 404) resistor in the circuit in the figure 江 Vg = 240 cos
反xx \/.
Part C: Supplementary Problems                                                                      177




Supplementary I 'roblem 11.5
The inductive load impedance in the figure has a magnitude of 26 Q and absorbs an average power of
13 kW. The sinusoidal voltage source supplies an average power of 13.50 kW.
      a) Find the effective value of the load current.
      b) Find the inductive reactance of the load.
      c) Find the inductive reactance of the line.
      d) Find the magnetizing reactive power supplied by the source.



                                               1
                                               1 O.8fl       jX




                               67司少 V (rrns)




Supplementary Problem 11.6
      a) Find V (rms) and 0 for the circuit in the figure if the load absorbs 600 VA at a lagging
         power factor of 0.8

      b) Construct a phasor diagram of each solution obtained in part (a).
178                                              Chapter 11/Sinusoidal Steady-State Power Calculations




                                          1n          j2 U

                                  니




                             120／쓰 \/ (rrT）引




Supplementary Problem 11.7
In the circuit shown in the figure the load resistance can be varied from 0 to 4000 Q. The load
capacitor can be varied from 0.1to 0.5 pF.
       a) Calculate the average power delivered to a load when RL = 2000 Q and CL = O.21uF.
       b) Determine the settings of RL and CL that will result in the most average power being
          transferred to RL.
       c) What is the most average power in part (b)? Is it greater than the power in part (a)?
       d) If there are no constraints of RL and CL, what is the ma虹mum average power that can be
          delivered to a load?
       e) What are the values of RL and CL for the condition of part (d)?
       f) Is the average power calculated in part (d) larger than that calculated in part (c)?




                                                                    三
                                          6 kU         0.6 H




                                                   12* "       .
                                      1
                                          v= 180 cos 5000tV
Part C: Supplementary Problems                                                                        179



Supplementary Problem 11.8
The operational amplifier in the circuit in the fi昏lre is ideal. Calculate the average power delivered to
the 50-Q resistor when Vg = cos 50,000t V.


                                                     0.04 尸F




                                                                         50 n
                                Chapter 12
                       Balanced Three-Phase Circuits


Part A: Representative Drill Exercises with Solutions

Drill Exercise 12.,1
The voltage from B to N in a balanced three-phase circuit is 120 LfQ V. If the phase sequence is
positive, what is the value of VBC?


Solution

In a positive sequence set of voltages the line-to-line voltages lead the line-to-neutral voltages by 300
and the amplitude of a line-to-line voltage is '厚 times the amplitude of a line-to-neutral voltage.
Therefore

          VBC = ['匹Q] VBN = 207.85 ,i             V.


Drill Exercise 12,.2
The current 'CA in a balanced, three-phase, 八connected load is 15 d墜 A. If the phase sequence is
positive, what is the value of 1cc9


Solution

In a positive sequence set of currents the line currents lag the delta currents by 30" and the amplitude
of a line current is 月 times the amplitude of a delta current. Therefore

          'CC = [v' L Q] 'CA = 25.98世 V.


Drill Exercise 12.3
The complex power associated with each phase of a balanced load is 384 j288 kVA. The line voltage
at the terminals of the load is 4160 V.



                                                                                                        181
182                                                                                              Chapter 12/Balanced Three-Phase Circuits




       a) What is the magnitude of the line current feeding the load?
       b) Given that the load is connected in delta and the impedance of each phase consists of a
          resistance in parallel with a reactance, calculate R and X.


Solution

The capacitor bank is a source of magnetizing vars. Therefore the magnitude of the line current will
be minimized when the capacitor bank is used to supply all the magnetizing vars demanded by the
load. In other words the 3中 bank of capacitors is designed to furnish 864 kV사t of reactive power.
        a) If the capacitor bank is connected in delta the rms ma多litude of the voltage across each
cariacitor is 4160 V. The reactive nower suonlied by each canacitor is 288 kVAR. Therefore the
capacitive reactance or eacn capacitor is - [41에)-I乙亡5히以시Jor -에J月／뇨2. /\[ 에 i-iz tne capacitance is


          C=         12。
                     ,2m .m
                                (1
                                                        )   ＝
                                                                꺾·
                                                                     14肛F
                                (6。       .。9
       b) If the capacitors are connected in wye the rms magnitude of the voltage across each
capacitor is 4160/V3 V. Each capacitor must still supply 288 kVAR; hence the capacitive reactance is
now -20.03 Q. At 60 Hz this requires a capacitance of 132.43pF.

       c) With the capacitor bank installed the complex power per phase is reduced to

          S中 = 384 +jo kVA.

If we use the line-to-neutral voltage VAN as the reference the rms line current is



           1aA
           L4    '   =   1aA
                         !64=         =         (416。
                                                (;      ，言4,000世
                                                          /v's)             -
                                                                            -   159.88 LQ   A.
Note: If we use the line voltage VAB as the reference, then the phase current 1AB is


          I48BA*='AB＝器쁠＝92.31LQ A.
The magnitude of the line current is＼厚 'AB or 159.88 A.
Part B: Representative Problems with Solutions                                                     183




Part B: Representative Problems with Solutions

Problem 12.1
       a) Is the circuit in the figure a balanced or unbalanced three-phase system? Explain.

       b) Find 1。
                .




                                                    \  }R    b
                                                    =1VVVH !

                                         24아二끄또V

                                  )24.
                                          聊：V




Solution

       a) The system is unbalanced because the load impedances are not identical.

       b) Because the impedance of the neutral conductor is zero, the three line currents are easily
obtained. Thus

              240 / 00
                       12/j                                   A,
          'aA= 21 =



         ！比：'      끎/   -   j4。           =    4.    8느뜨旦7八
and

                  240/ 1200
          'cC =   80 +j60 =               2.   4/ 83.130           A,
184                                                          Chapter 12/Balanced Three-Phase Circuits




The neutral conductor current is

          1(7= 'aA + 1bB + 'cC = 14.32 /_-8.16:A.



Problem 12.2
The magnitude of the phase voltage of an ideal balanced, t뇨ee-phase, Y- 刃nnected source is 125 V.
The source is connected to a bal띠lced Y-connected load by a distribution line that has an impedance
of 0.1 + j0.8 Q/ . The load impedance is 19.9 + j14.2 (2／中．The phase sequence of the source is acb.
Use the a-phase voltage of the source as the reference. Specify the magnitude and phase angle of the
following quantities: (a) the three line currents, (b) the three line voltages at the source, (c) the three
phase voltages at the load, and (d) the three line voltages at the load.


Solution

The first step is to construct the single-phase equivalent circuit sho찌n in the figure.




                ias勾
                  V            十
                                fr _




       a) First calculate 'aA. Thus

                  125/ 00
          'aA= 2아jls= 5/                  A.

Because the phase sequence is known the expressions for 1bB and ICC are known, namely

          'bB = 5/ 83.130 A and 'cC =      /_=156.8즈 A.

       b) Since the phase sequence is negative the set of line voltages lag the set of line-to-neutral
voltages by 34J'. The magnitude of a line voltage is 月 times the magnitude of a line-to-neutral voltage.
Therefore

          V的 = [V互／二塑：] V口n = 216.51／二翌n/,


          VC= 216.511         V,
Part B: Representative Problems with Solutions                                                       185



and V口 = 216.51 /_- 150 V.

       c) First calculate VN using the circuit in the fi昏lre. Th好, V 寸 = (19.9 + I 14.2)IaA =
122.23 /         V. It follows that VBN = 122.23 / 118.64' V and CN = 122.23 / -121.36' V.

       d) The line voltages at the load end are calculated directly from the line-to-neutral voltages at
the load end, thus Vj = 211.72/ -31.36' V, VBC = 211.72 (88.64' V, and VCA = 211.72/ -151.36"
V.


Problem 12.3
A balanced 八connected load having an impedance of 24 + j18 ci is connected in parallel with a
balanced Y-connected load having an impedance of 20匹亡 ( 2/ b . The paralleled loads are fed from a
line having an impedance of 0.1 + jO.5 Q/ . The ma多litude of the line-to-neutral voltage of the
Y-load is 680 V.
       a) Calculate the magnitude of the current in the line feeding the loads.
       b) Calculate the magnitude of the phase current in the s-connected load.
       c) Calculate the magnitude of the phase current in the Y-connected load.
       d) Calculate the mnagnitude of the voltage at the sending end of the line.


Solution

      First construct a single-phase equivalent circuit. In doing so note that the line-to-neutral
impedance of the is-connected load is 8 + j6 (2. The circuit is shown in the figure.




                       0----쓰도夕a1瓦；下-：뇨
                      目                             ／了
       a) It follows directly from the circuit in the figure that

          'aA    = I ' + 12


                   680dt . 680{j2으
                 = 而血 十 (8 + j6)

                 =88.40- j40.80= 97.36 /                 A.
186                                                               Chapter 12/Balanced Three-Phase Circuits



Therefore the magnitude of the line current is 97.36 A.

        b) The magnitude of the phase current in the s-connected load is

                       IIAI
                              =         680V        =
                                                        39.26A.
                                  124
                                            +j18J


An alternative calculation for the magnitude of L is to first calculate the phase current in the
Y－叫岫毗nt 由cuit of the i\-load and then divide the ma帥恤de of this current by＼厚 辰om the
circuit in the figure we have

                     680/ 00     --
                I勺 == ', H．二口 = 68 / -36.87" A.
                      ?5 +JO        -나

Therefore



                I -I
                II八1
                              =   單
                                  V3
                                     39.26 A.
                                        =




       c) From the circuit in the figure we have

            .   680 四으     . . .
                       = .j4／브／\'
           11 = 20匹亡

       Therefore Ilyl = liii = 34A.

        d) The line-to-neutral voltage at the sending end of the line can be calculated from the circuit
in the figure. Thus

          Van
                              = VAN + (0.10 + J0·50)'aA

                              = 709.24 + j40.12 = 710.37 厓.24 V

The magnitude of the line voltage at the sending end is 1 ab I = \/3 I Van I = 1230.40 V.


Problem 12.4
A three-phase, is-connected generator has an internal impedance of 0.9 + j9 Q/*'. When the load is
removed from the generator, the magnitude of the terminal voltage is 13,200 V. The generator feeds a
Part B: Representative Problems with Solutions                                                         187




s-connected load through a transmission line with an i呻edance of 1 + j9 Q/ . The per-phase
impedance of the load is 92.1 - j12 (2.
       a) Construct a single-phase equivalent circuit.
       b) Calculate the magnitude of the line current.
       c) Calculate the ma多litude of the line voltage at the terminals of the load.
       d) Calculate the magnitude of the line voltage at the terminals of the source.
       e) Calculate the magnitude of the phase current in the load.
       t) Calculate the ma얍litude of the phase current in the source.


Solution

       a) With no load on the generator the terminal voltage is identical to the internal voltage. Using
the a-phase voltage Va'n as the reference the single-phase equivalent circuit is as shown in the figure.
The figure is constructed with a Y-equivalent circuit for both the generator and the load.

                                         口，.3皿    43끄            兀    뇨Z       그q꾸 겨      3D·7J之
                                         싸羽까＝寸二弩1HW小
                                                         vcirl                 "'   W/W       T거4"
                                                                                                   1


       b) From the circuit in the figure observe that

                             200W    ) LQ        231.05 /         14.04
          L*     =   (13,
          '。   A =          (32
                                  +18)      -
                                            -
                                                             -
                                                        _______           A.

The magnitude of the line current is the of 1aA, i.e., 231.05 A.

       c) The line-to-neutral voltage at the terminals of the load is

          VAN = (30.7 小幷凡A = 7153.07느끄竺 V.

Therefore the magnitude of the line voltage at the load end is 月 (7153.07), or 12,389.49 V.

       d) The line-to-neutral voltage at the terminals of the source is

          V口12 = (31.7 +j5)I口A = 7414.71（二：塑'7으 V.
 188                                                               Chapter 12/Balanced Three-Phase Circuits



 The magnitude of the line voltage at the source is therefore '厚 (7414.71) or 12,842.66 V.

       e) The magnitude of the phase current in the s-connected load is the magnitude of the line
current d如ided by＼匡 or (231.四月工 꿔hich is 133.39 A.

       1) The ma多itude of the phase current in the 八connected so毗e is also the ma凹litude of the
line current divided by \／互， or 133.39 A.


Problem 12.5
A balanced three-phase distribution line has an impedance of 1 + j5 c2/ 5. This line is used to supply
three balanced three-phase loads that are connected in parallel. The three loads are

          Ll= 75 kVA at 0.96 pf lead,

          L2 = 150 kVA at 0.80 pf lag,

          L3 = 168 kW and 36 kVAR (magnetizing).

The mag血ude of the line voltage at the terminals of the loads is 2500 '/ V.
       a) What is the ma多血tide of 毗 line voltage at the sen小昭 end 可the line?
       b) What is the percent efficiency of the distribution line with respect to average power?


Solution

       a) We be帥I 切 first fin曲g the equivalent 鈿恥巾hase load. The complex po吼叩er phase
for each of the given loads is
                     0
          S         兀코                    U    羽   겨           人
                                                               V                                              %=
                                                                                                         m1




          '1  150,_, -  . -
          )2 =＝二(U.s 十 /U.b) = <1U 十 j34,) KVA,
                    J


and

           曷   l
             = ;(lb8 + 戶이 = >b + )12 kVA,
                    .   '   /,,   .   4   戶．       .   .   .




               17
The total complex power per phase is S1 + S2 + S3 or 120 + j35 kVA.
Part B: Representative Problems with Solutions                                                       189



       Using VdJ.4 as the reference we can calculate 'aA from the complex power formula. That is

          "AN 'aA = (120 +J35)103,

or


          (*= ‘加'몇詩臺塑＝明*j14.
It follows that I口A = 48j14 = 50／二프근르 A.
        Now the line-to-neutral voltage at the source end can be found since we know both the line
impedance and the line current. We have

          V口n = 2500LQ + (1 +15) (48 小j14) = 2627.74／쯔으至 V.

The magnitude of the line voltage at the sending end of the line is '手 (2627.74), or 4551.37 V.

       b) The average power lost per phase in the line is


         p： 呻니     'aA1     2   ·上   :   2500 W

It follows that the average power input per phase is 120,0刃 + 2500, or 122,500 W. The percent
efficiency of the line is

          %刃 =egTxi예
                          PIN



                 嗤辯x 100= 97.96
Problem 12.6
       a) Calculate the reading of each wattmeter in the circuit shown in the figure. The value of Z, is
          40L      c .

       b) Verify that the sum of the wattmeter readin多 equals the total average power delivered to
          the 八connected load.
 190                                                                           Chapter 12/Balanced Three-Phase Circuits




                                                                                     A




Solution

       a) From study of the circuit in the figure, observe that the reading of wattmeter 1 is

          W1 =   JVBA1
                             11bB1   COS           (0VBA
                                                               -
                                                                   0IbB)

and the reading of wattmeter 2 is


          w2= 'cA1
                 I
                             II뇌     邸
                                           （0VCA
                                                           -       91cC)
In these e사：1ressions eVBA is the phase angle of 'BA' e1bB is the phase angle of 'bB' 0vCA is the phase
angle Of VCA, and 0!cC is the phase angle of 1cc.
        Several other observations are necessary before we start our calculations. First, the phase
sequence is negative; second there is no impedance in the line between the source and the load; and
third the load is delta-connected. Based on these observations we make the followi昭 calc岫tions.

                         240 /00
          'aA = (40/3) T jo = 18LQA.
Therefore tbB = 18 jj竺 A and IC = 18亡二드00 A.

          VAB =＼厚느3竺VAN= 24小厚／                                             V

It follows that\/BA = 240v手 JQ V andVcA = 240v'互 /           - V.
        We now have all the values needed to compute the wattmeter readings. Thus

          w1 = (244Jv' ) (18) cos (1500 - 150') = 7482.46 W
Part C: Supplementary Problems                                                                         191




and

          w2 = (240V) (18) cos [e150' - (- 90')1 = 3741.23W.

       b) The sum of the two wattmeter readin多 is 11,223.69 W.
       The power per phase can be calculated using the a-phase voltage and current, thus

          j7中 = (240) (18) cos (0 - 300) = 3741.乃 W.

Therefore the total power is

         PT = 3p中 = 11,223.69W.



Part C: Supplementary Problems

Supplementary Problem 12.1
The ma多litude of the phase voltage of an ideal balanced, three-phase, Y-connected source is 120 V.
The source is connected to a balanced Y-connected load by a distribution line that has an impedance
of 0.2 + j0.8 Q/ . The load impedance is 15.8 + j11.2 Q/ . The phase sequence of the source is abc.
Use the a-phase voltage of the source as the reference. Speci勺 the magnitude and phase 帥gle of the
following quantities: (a) the three line currents, (b) the three line voltages at the source, (c) the three
phase voltages at the load, and (d) the three line voltages at the load.


 Supplementary Problem 12.2
The magnitude of the line voltage at the terminals of a balanced Y-connected load is 440 V. The load
impedance is 3.387 c/ b. The load is fed from a line that has an impedance of 0.0693 + j0.04 c2ftP.
       a) What is the magnitude of the line current?
       b) What is the ma帥tude of the line voltage at the source?


 Supplementary Problem 12.3
 A balanced s-connected load has an impedance of 60 + j45 ci . The load is fed through a line
 having an impedance of 0.8 + j0.6 Q/ . The phase voltage at the terminals of the load is 480 V. The
 phase sequence is negative. Use VAB as the reference.
        a) Calculate the three phase currents of the load.
 192                                                        Chapter 12/Balanced Three-Phase Circuits



        b) Calculate the three line currents.
        c) Calculate the three line voltages at the sending end of the line.


 Supplementary Problem 12.4
A balanced A-connected load having an impedance of 72 + j54 (2/ b is connected in parallel 꿔ith a
bala皿氾d Y-connected load having an impedance of 50 世 Q / . The paralleled loads are fed from a
line having an impedance of 0.5 + j1.5 Q/ . The magnitude of the line-to-neutral voltage of the
Y-load is 1200 V.

        a) Calculate the magnitude of the current in the line feeding the loads.
        b) Calculate the magnitude of the phase current in the A-connected load.
        c) Calculate the magnitude of the phase current in the Y-connected load.
        d) Calculate the ma多litude of the line voltage at the sending end of the line.


Supplementary Problem 12.5
A three-phase, A-connected generator has an internal impedance of 0.009 + j0.09 (2/ b. 砥／hen the
load is removed from the generator, the magnitude of the terminal voltage is 13,800 V. The generator
feeds a A-connected load through a transmission line with an impedance of 0.02 + j0.18 (2Ib. The
per-phase impedance of the load is 7.056 + j3.417 (2.
        a) Construct a single-phase equivalent circuit.
        b) Calculate the magnitude of the line current.
        c) Calculate the magnitude of the line voltage at the terminals of the load.
       d) Calculate the magnitude of the line voltage at the terminals of the source.
       e) Calculate the magnitude of the phase current in the load.
       f) Calculate the magnitude of the phase current in the source.


Supplementary Problem 12.6
A three-phase line has an impedance of 1 + j3 (2/& The line feeds two balanced three-phase loads
that are connected in parallel. The first load is absorbing a total of 7.2 kW and 5.4 kVAR magnetizing
vars. The second load is A-connected and has an impedance of 11.52 - j8.64 (21#. The line-to-neutral
voltage at the load end of the line is 120 V. What is the magnitude of the line voltage at the source end
of the line?
Part C: Supplementary Problems                                                                         193




Supplementary Problem 12.7
Three balanced three-phase loads are connected in parallel. Load 1is Y-connected with an
impedance of 400 + J3(xJc肋load 2 is 八connected 싸ith 띠Ii呻edance of 2的0- 月81i0 I弘 and
load 3 is 172.8 + j2203.2 kVA. The loads are fed from a 小stribution line with an impedance of 2 +
j16 Q/p. The magnitude of the line voltage at the load end of the 丘ne is 24v'. kV. Calculate the total
complex power at the sen小ng end of the line.


Supplementary Problem 12.8
       a) Determine the reading of each wattmeter in the circuit in the f哥lre if the phase sequence is
          negative, the magnitude of the line voltage is 4160 V, and the load impedance is
          208 /      . Q/ .

       b) Repeat part (a) given that the phase sequence is positive.




Supplementary Problem 12.9
The line voltage in the circuit in the figure is 600 V, the phase sequence is positive, and the load
impedance is 8 + j6 Q/中.
       a) Calculate the wattmeter reading.
       b) Calculate the total reactive power associated with the load.
194   Chapter 12/Balanced T뇨ee-Phase Circuits
                                            Chapter 13
                                         Mutual Inductance


Part A: Representative Drill Exercises with Solutions

Drill Exercise 13.1
                                                                                                  1 is 6
Two magnetically coupled coils are wound on a nonmagnetic core. The self-inductance of coil
H, the mutual inductance is 9.6 H, the coefficient of coupling is 0.8, and the physical structure of the
coils is such that the permeances P11 and尸22 are equal.
       a) Find L2 and the turns ratio N1/N2.
       b) If N1 = 800, what is the value of P1 and P2?


Solution

        a) From the relationship M = k vTL고巧 we have



          L2去，山a24H.
The se珏-inductances are related to the permeances by the expressions L1 = NP1 andL2 = NP2 . By
hypothesis P11 = P22 . Hence for a nonmagnetic core P1 = P2 and (L11L2) = (N11N2)2. Therefore we
have


             M而            찌
                           n
                           lm 2
                                  le 2
                                                                                                                 =




        b) Given that N1 = 800 turns it follows from part (a) that

                L]            小仄
           P1 = 근 = 9.375 x 10 V Wb/A = P-, .
                  1
                      1=                         1d
             -

                  八1




                                                                                                           195
196                                                                    Chapter 13/Mutual Inductance



Drill Exercise 13.2
A linear transformer is used to couple a load consisting of a 360-c resistor in series 꿔ith a 0.25-H
inductor to a sinusoidal voltage source, as shown in the figure. The voltage source has an internal
impedance of 184 + JO Q and a ma仙um voltage of 245.20 V, and is operating at 800 rad/s. The
tran計ormer parameters are R1 = 100 c, L1 = 0.5 H, R2 = 40 c, L2 = 0.125 H, and k = 0.4.
Calculate (a) the reflected impedance; (b) the primary current; (c) the secondary current; and (d)
the average power delivered to the primary terminals of the transformer.


                                                           /(U力丁
                                                       /   小＼
                                            Source   Transformer   d       Load



Solution

       a) For the given values of the transformer parameters we have

         入{    = 0.4V6面2了 = 0.10 H,

         wM =800 (O.1) =80Q,

         Z22 =40+ j800 (O.125) +360+ j800 (O.25)

               =400+ j300 Q

           Z221             =
                                    500Q
and

         Z;2                =400- J300C .

      It follows that the reflected impedance is

                        /   小   n   \   2
         2戶 1黑1 (4（刃- J300) =10.24 -J7.68Q
               \)fiJ/
Part A: Representative 1)rill Exercises with Solutions                                              197




       b) The se끄-impedance of the primary 毗nding is 100 + j400 Q and the internal impedance of
the source is 184 + JO. Therefore the prim缸y current is

          11
                   =             2缸20／쁘
               '       184+ 1어［) +j吼0+ 10.24- j7.68

                   = 0.50 /       }.l30A.

The steady-state expression for i1 is

          ii (t) = 0.50 cos (8001 - 53.130) A.

       c) The phasor-dornain expression for the secondary current is

          1 _j口)凡t1 UJ80     .
                               塑꼬D
           12 ＝들7尸 500區立（0.5이＝
                   = 0.08 LQA.

       The steady-state expression for i2 is

           b (0 = 80 cos 8001 mA.

        d) The resistive component of the impedance seen looking into the primary termin심s of the
 transformer is 100 + 10.24 or 110.24 c. The rms value of the primary current is 0.50/V A. It follows
 that the average power delivered to the primary winding of the transformer is

                              2
                            .24 = 13.78W.
               尸= r9흐9) ' 11。
                       (V2J


 Drill Exercise 13.3
 Use the T-equivalent circuit for the linear transformer in figure A to fmd Il and 12. The phasor
 currents Il and 12 are defined in the figure A.
 198
                                                                        Chapter 13/Mutual Inductance




                                                Jw月才
                                               J= \
                                                 H=




                        Source              Transformer        d       Load



        (a)
 Solution
For the given parameters of the transformer L1 = 0.5 H,L2 = 0.125 H,
                                                                     andM = 0.10 H. Therefore
L1 - M = 0.4 H and L2 - M = 0.025 H. At 800 rad/s w(L1 - M) = 320
                                                                      C, w(L2 叫 M) = 20 Q, and
wM = 80O. The phasor-domain equivalent circuit using the T-equivalent
                                                                       circuit for the tr키lsformer
is sho치Vn in figure B where the voltage source is V3 is 245.20世 V.




       (b)

The mesh-current equations for the circuit in the figure are

              (284 + j400)Il - 18012 = 245.20 je - 1801i + (400 +1300)12 =
                                                                              0.

The solutions for Il and 12 are

              Ii = 500亡스3꼬으mA         and    12 = 80 匹h沮·
                                                                                                                         199
Part B: Representative Problems with Solutions



Part B: Representative Problems with Solutions

Problem 13.1
Find the value of k in the circuit shown in the figure so that Zab is purely resistive when w = 4 krad/s.

                                                                                 2011                    511




                                                                                                               12.5 .F




Solution

Using the concept of reflected imllpedance the expression for Zab at 4 krad/s is

                                                                             r    = = -2
                                               " " '" '                          WM
                                               20+    +
                                                                  '
                          "'
           "
           Zab                                              j50
where

          口小／= wk'/Ej石 = 40k

 and

           Z22 = 5 + j32 尸 j20 = 5 + j12 = 13／흐7흐望 Q .

 substituting the values into the expression for Zab gives



               786＝
                      『j5. *+
                     加+
               Zab = 20                                           j50
                                                                             （쒸2        (5-
                                                                                              112)
                                                                                                     .




 Zab will be purely resistive when the j term is zero, or when

                                               2

               鬪
                      /        .   n   .   \



                                                   (
                                                       ")
                                                                        :＝   乳

 Solving for k gives k = 0.6634.
 200
                                                                          Chapter 13/Mutual Inductance



 Problem 13.2
 The load in the circuit shown in the f蜘re is adj出妃d for
                                                            曲血l네rn average po吼r transfer.
        a) Calculate the steady-state expression for i1if Vg iS 300 COS 4000t
                                                                              V.
        b) 砥hat percentage of the average power developed by
                                                                   the ideal sinusoidal voltage source is
           delivered to the load?


                                                                5 mH
                                        511     1mH   10O   1       뇨   24O




Solution

         a) The impedance of the load for maximum average power
                                                                  transfer to the load equals the
conjugate of the Th6venin impedance as seen from the termin
                                                              毗 of the load. We can use the conc아t
of refi凹妃dii叩edan凹 to find the Th6ve恤 in叩edanc已
                                                       At a frequency of 4仄刃 rad/s we have 口兀1 =
16 Q, a兀2 = 28.8Q, w凡I = 20 Q, and口兀g = 42.1加king m
                                                              t아he circ岫 from the load term노als
with the independent voltage source removed, we calcula
                                                        te the total impedance on the primary side
of the transformer thus:

          Z11 = (5 + 10) + j (4 + 16) = 15 + j20 = 25 / 53.13 Q.

It follows that Zl1 = 15 - j20 (2 and the Th6venin
                                                      impedance is

                               ,_
                                    .   '   2
          Z = 2.4 +j28.8 + i의 (15 -j20)
                           \--'/
             = 12+ j16 Q.

The load impedance is therefore 12 - j16 Q.
                                                                                                    201
Part B: Representative Problems with Solutions



      Now that we know the load impedance we can calculate the impedance reflected into the
primary side of the transformer. After first noting that Z22 = 14.40 + j12.8 = 19.27 / 41.63 Q we
write

                /   4   n        .   2
          Zr = 卜，뿌니 (14.40小j12.80)
                \ I-工乙
                            //




             = 15.52 - j13.79 (2 .

Since the source voltage is 3凹 亡Q V the current out of the positive ter岫nal of the source is

                                     300 iO0
          h = 15 +j20+ 15.52 -j13.79 = 9.63/                 A.

The steady-state expression for i1(t) is i1(t) = 9.63 cos (4000t - 11.50O) A.

       b) The average power developed by the independent voltage source is

          Pg = (300) (9.63) COS (0 + 11.50) = 1416 W.

       To calculate the average power delivered to the load we first calculate the load current 12. Thus


          I-I＝철프II =10/ 36.8尹A.
              乙22 '   나H

The resistance component of the load impedance is 12 Q; therefore

          尸L = {(10)2 (12) = 6(刃w.

 The percentage of the developed power delivered to the load is


           % delivered = 擘L x 100 = 42.37.
                                         1416



 Problem 13.3
 Find Rab in the circuit seen in figure A if N1 = 100 turns and N2 = 200 turns.
 202                                                                                                 Chapter 13/Mutual Inductance




                                                                                        12
                                                    a1




                                                                         1 d e a1
                                                    尸ab+
                                                                                            .
                                                                                        ;
                                                         >
                                                                                            사2   80 fl


                                                    b1

         (a)
 Solution
The phasor-domain equivalent circuit of the circuit shown in figure A is shown in figure B. From the
figure we see that Rab is the ratio Yat,/Ii. In finding this ratio we first note the ideal transformer
imposes the following constraints: 10011 = 20012; and (V1/100) = (V2/200).




        (b)

        To find \Tab as a function of Il we use the following relationships:

                           끼                                         d                                                          %
                                         느
                                                                                                                                +
               Vab                   2
                                                                                    !
                                                                                                                                =




and

                                             (                  i\
               V2=   (1+
                           I2) 80=           (11+
                                                           才)
                                                                     80= 12011.
It follows that

               Vab = 1.5 (120)Ii = 1801i
Part B: Representative Problems with Solutions                                                        203




or

          ,,
             ' =        . nn ，八
          I（口I   ==m= = lou 뇨d
                 Vab
                  11




Problem 13.4
The following measurements were made on a lossless linear transformer. With the low-voltage side
open, the inductance measured looking i如 the high-voltage side is 12 H. With a 125-V rms
sinusoidal voltage applied to the high-voltage 꿔inding, the open-circuit voltage measured on the
low-voltage winding is 50 V rms. With a 15-V rms sinusoidal voltage applied to the low-voltage side,
the open-circuit voltage measured on the high-voltage side is 24 V.
       a) Speci勺 the numerical values of L1, L2, M, and k for the transformer.
       b) Calculate the turns ratio of the transformer.
       c) Construct two possible equivalent circuits for the linear transformer if a is chosen to equal
          1%
           ／兀1
       d) Repeat part (c), given that a is chosen equal to L2JM.


Solution
       a) Let L1 represent the self-inductance of the high-voltage winding. Then by hypothesis L1is
12 H. With the low-voltage side open while the high-voltage side is energized we know the voltage
ratio VLV/VHV is equal to M/L1; therefore (50/125) = M/L1, or M = 4.8 H.
       With the high-voltage side open while the low-voltage side is energized, we knowVL.v/Vuv is
equal to LilM, where La is the self-inductance of the low-voltage winding. Thus (15/24) = L2/M or
L2 = 3H.
       The coefficient of coupling is M/vTj15j, or 0.8.

       b) The turns ratio NilNi can be calculated from the voltage ratios as given by Eq. (14.104);
therefore

                                  1
                                  2
                                      = 0.5


    c) If we choose a = M/L1, or 0.4 we get L1 [(hR)2 - 1] = 6.75 H, k2L2 = 1.92 H, and (1 -
r戶2= l.uo i工 i ne two possiDie equivaient circuits are as snown in ngures A and Ii.

      d) If we choose a = L2JM, or 0.625, we have k2L1 = 7.68 H, (1 - k2)L1 = 4.32 H, and [(1/k)2
- ilL2 = 1.6875 H. The two possible equivalent circuits are shown in figures C and D.
204                                                                           Chapter 13/Mutual Inductance




                                     乙／                       LC.4-          +e C2

                                                              U言H三，
                   中＋            ＝
                                                               1
                        L;
                                                                              m=




      (a)
                   目' 万m二
                c:j；
                             ,       '.     f   . ,,J




      (b)




                                          43'2,c                 I :Oh,Z5m    寸中e.之




       (c)
                                                                  1 盲1三
                                                                /,G875刀
                                                                                         1

                                                                                         Z
                                                    : 口6251




                                                                          卜 三
                                                                                     ／
                                                        旨
                                                                nm))n
                                                                                     나
                                                                               寸戶
                                                                                             +
                                                                                             1
                                                                                             石
                                                                                             中


                                                                 ""   "                      U


       (d)                                               "
Part C: Supplementary Problems

Supplementary Problem 13.1
Two magnetically coupled coils have self-inductances of 27 mH and 3 mEl, respectively. The mutual
inductance between the coils is 7.2 mH.
        a) What is the coeff也呱 of co叩li叩？
Part C: Supplementary Problems                                                                        205



       b) For these two coils, what is the largest value that M can have?
       c) Assume that the physical structure of these coupled coils is such that P1 = P2. What is the
          turns ratio N1/N2 if Nl is the number of turns on the 27-mH coil?


Supplementary Problem 13.2
A 3000-Q resistor is connected to a sinusoidal voltage source by a linear transformer. The internal
impedance of the source is 10.44 + j13.92 Q when the source is operating at a frequency of 1600
rad/s. The rms voltage at the terminals of the source is 15 V when the source is not loaded. The
parameters of the li 妃ar transformer are primary winding R1 = 13.12 Q;L1 = 30 mH; secondary
windingR2 = 600 C; L2 = 3 H; mutual inductance of the tr기lsformer = 75 mH.
       a) What is the numerical value of k?
       b) What is the value of the impedance reflected into the primary?
       c) What is the value of the impedance seen by the source?
       d) What is the rms ma曾itude of the voltage across the 3士C resistor?
       e) What percentage of the average power developed by the source is delivered to the input of
          the transformer?
       1) What percentage of the average power developed by the source is delivered to the 3-kQ
          load resistor?


Supplementary Problem 13.3
In the circuit shown the frequency of the sinusoidal source is 4000 rad/s and the rms value of the
internal voltage is 45 V.
       a) Find the Th6venin equivalent circuit with respect to the terminals c, d.
       b) What load 油pedance would result in ma血恤i average power be뇨g trax好ferred t야he
          terminals c, d?
       c) What is the ma血um average power than can be transferred?
       d) What比rcentage of the average power delivered to the tr카lsformer is delivered to the load
          in part (c)?

                                      5 (1       10 i             160 il
206                                                                       Chapter 13/Mutual Inductance




Supplementary Problem 13.4
The values of the parameters in the circuit in the figure are L1 = 0.2 H;L2 = 0.8 H;M = 03 H;Rg
= 20 (2; and RL = 560 Q. If Vg = 480 cos 中毗 V, find
       a) The ma多litude of v。
                            ;
       b) the average power delivered to RL;
       c) the percentage of the average power generated by the ideal voltage source that is delivered
          toRL.




                                                         >
                                                         >          尻




Supplementary Problem 13.5
The source voltage Vg in the circuit in the figure is equal to 480 cos 4乂t V; find
       a) the amplitude of vO;
       b) the average power delivered to the soo-c load resistor;
       c) the percentage of the average power generated by the ideal voltage source that is delivered
          to the load resistor.




                                                                   二 560 [1
Part C: Supplementary Problems                                                                    207




Supplementary 'Problem 13.6
What percentage of the average power delivered to the石 y terminals in the circuit in the figure
reaches the 9卜Q resistor?




                                                                        90 fl


                          125／르V
                            (rm引




Supplementary Problem 13.7
The parameters in the circuit in the figure are N1 = 1000 turns, N2 = 5어：) turns, R1 = 2 Q, L1 = 20
mH, and RL = 18 Q. If Vg = 150 cos 500 V, what percentage of the average power delivered by the
ideal voltage source is dissipated in the 18- 2 resistor?




Supplementary Problem 13.8
Find the average power delivered in the i-c resistor in the circuit in the figure.
208                                                                       Chapter 13/Mutual Inductance




                                                   4n




                             烈                                       in




Supplementary Problem 13.9
      a) Determine the turns ratio a of the ideal transformer in the circuit in the figure so that
         maximum average power is transferred to the 200-a resistor.
      b) What is the ma血um power that can be transferred?
      c) What is the rms voltage across the 200-a resistor when ma抽um power is bei培 delivered?


                                 5 kfl     ] k1)



                                                                             200 n
                    (r二Vs)
                     3
                                Chapter 14
                       Series and Parallel Resonance


Part A: Representative Drill Exercises with Solutions

Drill Exercise 14.1
The following components are available to construct a parallel-resonance circuit: L1 = 7.5 mH, L2 =
15 mH, C1 = 6 uF, C2 = 3 uF, and R = 2 k(. Design a circuit that will have the highest possible
resonant frequency. Specify (a) 口）o; (b) fi; (c) Q; (d) w1; and (e) o2.


Solution
       a) To obtain the highest possible resonant frequency we want L and C as small as possible;
therefore we place the inductors in parallel and the capacitors in series. The equivalent inductance is
5 mH and the equivalent capacitance is 2pF. The resonant frequency is


          ii v'l0 x l0U9 ; or 10 krad/s.

       b) The bandwidth of the circuit is 1仄RC), or 250 rad/s.

       c) The quality factor of the circuit is the resonant frequency divided by the bandwidth or 40.
       The corner frequencies w1 and w2 can be computed from Eqs. (15.7) and (15.8), respectively.

Ther'湍八們，‘，才，烈，땁，“ndca앉닯，＝詐8。烈：町,, = , , *加，.,＝婦佃，.)
Drill Exercise 14.2
A sinusoidal current source delivers a current having an amplitude of 100 uA. The internal
impedance of the source is 750 + JO kQ. This current source is used with a 40-mH inductor and a
500-k(2 resistor to form a parallel-resonant circuit. The resonant frequency is 250 krad/s.
       a) Specify the numerical value of the circuit capacitor.
       b) What is the Q of the circuit without the source?
       c) What is the Q of the circuit with the source?
       d) What is the bandwidth of the circuit with and without the source?

                                                                                                     2們
210                                                          Chapter 14/Series and Parallel Resonance




       e) What is the maximum output voltage that the source can deliver?
       f) What is the ma血um value of the capacitor current at resonance?


Solution

. . 2. . 맏L andw0缸e spe師ed; theref呼．如． V쁘印fCQ C帥be ob帥ed from the expre蜘nC=
I/ WOL). ror LflC given vaiues OIL ana w0 L is u.'+ nr.


       b) The quality factor of the parallel structure without the source connected is obtained from
the expression w0 RC, where R is 500 kQ. Thus

          JN   ／八r＝』m ' m n3\ ／尸n』
                                 ＼ ' d -'3' /1노 1 4 -'- 9\ 尸1\
          1/ = ZDu X Lu ) (DW X LU ) (u.'I X Lu ) = DO.


        c) When the source is connected to the circuit the effective resistance is the parallel
combination of the 500-kc and 750-kQ resistors. The effective resistance is 300 kQ and hence the
quality factor is reduced to 30.

      d) Since the bandwidth equals the resonant frequency divided by the quality factor, the
bandwidth is 5 krad/s before the source is connected and 8.33 krad/s after the source is connected.

       e) At resonance the maximum amplitude of the output voltage equals the peak current of the
source times the effective resistance. Therefore

                mr\ J\ . . m r\H6\ mm\ . ' d n3S nr1 1 r
           Vm = （끄人ixiu J (J（人I X Lu) = j (_, V.


       f) At resonance the current in the capacitive branch is the quality factor times the source
current. Hence


          'mc =30 (100x 10_6) =3 mA.



Drill Exercise 14.3
The components in the circuit in the figure are R = 10 c, L = 0.2 mH, and C = 5 nF. Calculate (a)
coo; (b) Q; (c) fi; and (d) the frequencies where the amplitude of the current is 80% of its ma姓nlum
value.
 Part A: Representative Drill Exercises with Solutions                                                  211




                                      Vs= VmCOSot          i= I,,COS ({U + 비




 Solution

          a) The resonant frequency of the series circuit in the figure is iivT三, or 106 rad/s.

          b) The quality factor of the circuit is w0 LIR, or 20.

          c) The bandwidth equals the resonant frequency divided by the quality factor; hence ft = 50
krad/s.

      d) The amplitude of the current will be 80% of its ma址mum value when the impedance is
125% of its minimum value R. Therefore we want to find the frequencies when


                   1+)j
                          Q (w- wo) (w+ w
             11*
                                            o)   = 1.25.

       For the known values of Q and w0 the above requirement generates the quadratic equation

            (02 士 37,500w - 1012 = 0.

       Solving for the positive values of w gives

            （刃l = 981,425.77 radls
and

            m2= 1,018,925.77 rad/s.


Drill Exercise 14.4
A para끄el-resonant structure as shown in the figure is to satis勺 the following specifications: fo = 200
kHz, Z(f0) = 40 k(2, I Z(f, ) I = 32 (2, andfa = 186 kHz.
       a) Specify凡乙 and C.
       b) What is the Q of the circuit?
212                                                         Chapter 14/Series and Parallel Resonance



        c) What is the bandwidth of the circuit?
        d) If this circuit is driven by a sinusoidal current source having an internal impedance of 360
            + J0 kQ, what is the Q of the energized circuit?
        e) What is the bandwidth of the energized circ山?




Solution
                      'S
                 (1m COS rot)



                                1     8i           I
                                                   CT          L
                                                               卜      V。=
                                                                        ＝   7
                                                                            V   mCOS
                                                                                』 .+   (wf+   O




        a) At resonance the impedance of the parallel circuit is equal to the resistance; therefore R =
40kO.
       To fmdL and C we first find the quality factor of the circuit. The quality factor can be found
from the specification that the magnitude of the i叩edance at 186 kHz is 32 kQ. In general


          ,：去［1+JQ（針쒸］
꿔hich can also be 싸ritten




For the problem at hand we have


          古喘［卜미蠶－副］·
        Solving for Q gives

           0 = 5.16.

Now

          C = Q/w0R = 102.71pF
and

          L = 1／切긍C = 6.17mH.
 Part A: Representative Drill Exercises with Solutions                                                  213



        b) The value of Q was found in part (a); i.e., Q = 5.16.

        c) The bandwidth is the resonant frequency divided by the quality factor, or

                4.   八八／.   4』
                             ＼3

          肝十싸；/" = 38,738.35Hz.
        d) After the source is connected to the parallel circuit, the equivalent resist띠lce is 36 kQ.
Therefore the quality factor of the circuit is reduced by a factor of (36/40), or 0.9. ThusQ =
(0.9)(5.16) = 4.65.

      e) The bandwidth of the energized circuit is increased by a factor of 11(0.9), or 1.11. Hence the
bandwidth increases to 43,042.61 Hz.


Drill Exercise 14.5
The circuit elements in the figure are R = 80 Q, L = 50 mH, and C = 0.2MF.
       a) If the circuit is excited from a sinusoidal voltage source 20 cos 口）0 t V, what is the rms value
          of vO(t)?
       b) The rms value of vO is measured with a digital voltmeter that has a resistance of 500 kQ.
          What is the rms reading of the voltmeter?




Solution

        a) For the given circuit elements the resonant frequency is i04 rad/s. At resonance the current
out of the positive terminal of the voltage source is 加 ..Q/80, or 0.25 LQ A. The capacitive reactance
at resonance is -500 Q; therefore VO is (- j500 )(0.25四) or 125 /_-90 V. Thus the rms value of v。is
125/V or 8839 V.

       b) With the voltmeter in parallel with the capacitor, the Q of the parallel combination is

          Q = w。
               RmC =: (104) (500 X 103) (0.2 >< 10-6) = l0C目1.
214                                                            Chapter 14/Series and Parallel Resonance




         Therefore the series equivalent circuit of the parallel combination consists of a resistor of (500
x 1下I  (1  + 106) or. 50 Q and a ca.
                         0.                  of 0.20
                                        pacitor          + 10- ,. or 20戶．
                                                          (1   6)    0.    F.
        ror an practicai purposes rue resonant irequency is srui iii - rauis; rnereiore m1le current m tne
                                                                                                       .
                                                                                .,        ,   ..   .       ..




circuit is (20/80.5) LQ A, and the value of VO is

               .      20 . n 戶
               VU == ;;;；二 (U.) -p （大J) = I乙4／乙／二흐츠브'V V.
                     OO. J


The rms reading of the voltmeter is 124.22/v工 or 87.84 V.



Part B: Representative Problems with Solutions

Problem 14.1
The current source in the circuit sho팎n in the figure is generating a sinusoidal current of 420 cos wt
mA. Calculate
            a) the unity power-factor resonant frequency;
            b) the peak amplitude of v。at unity power-factor resonance;
            c) the Q of the circuit;
            d) the bandwidth of the circuit;
            e) the frequency at which the peak amplitude of v。is ma虹mum;
            t) the ma虹mum value of the peak amplitude.

                                                                                     0
                                                                                     +

                                                          5H
                                                  1 kt1                              VO


                                                          5。
                                                                                     1



Solution

       a) For the parallel circuit in the figure the unity power-factor resonant frequency is given by
Eq. (14.63). For the circuit values given in the figure 口J0 is 3 rad/s.
      b) At unity power-factor resonance the impedance of the parallel circuit as seen from the
terminals of the current source is given by Eq. (14.66). For the given values of R多 R,L, and C we have
 Part B: Representative Problems with Solutions                                                          215



 Z(w0) is (5000/105) or approximately 47.62 (2. The peak amplitude of vO is the peak amplitude of the
 current source times Z(cv o). Hence



           Vm
                   圈
                                (4加／
                                                                    1丁   ')
                                                                              =
                                                                                  20V.
        c) To find the Q of the circuit, first replace the inductive branch with its parallel equivalent at
the unity power-factor resonant frequency. The equivalent resistance is given by Eq. (14.73), and the
equivalent inductance is given by Eq. (14.74). The Q of the coil at resonance is

           ,      1 므（)1-. () _.,
           VcoiI H j     ='                    5               小 .).

It follows that

          R2= 5 (1+ 9;) = 50c
and


                         d
                         l小 0
                            /
                                                                    H                    +=
                                                           型
                                                       9
The so-c resistor is in parallel with the 1000-Q resistor; therefore the equivalent resistance of the
circuit at resonance is

          .1      (1000) (50)                                  1000 ,-,
          Ke = 411=：느于HJ= = m＝二1 $J .
                  iU>(J      21


Now Q is found from the expression

                                                                    師
                                           끄
                                                               八乙
          Q = w0ReC =
                                                   勺

                                       7
       d) The bandwidth is w0/Q, or 1.05 rad/s.

       e) The frequency corresponding to the ma址mum peak amplitude of vO is given by Eq. (14.68).
For the given circuit parameters we get

          wm = v-ris' 勺 3,16 rad/s.
216                                                                                       Chapter 14/Series and Parallel Resonance



       t) To 丘nd the ma址mum peak 缸llplitude of v。at the frequency Wm, first fmd the admittance
Y(口Jm) and then use the phasor-domain relationship

          ir
          v         卜         I
           'o_          ,..I_.. \'
                        .r "4勺n)


The equation is

           . .    1 .       1     . .VI
          Y0m) = 1000 十 5 +j5Viil 幻百

                         = 19.18 + j5.75 = 20.02 /고6.69 mV.

It follows that

                              420, 00 x i0-
          V11= 끼r       八11
                                 -八八   4   J戶   ／八11   d   11中J
                                                                  m = 20.97/ 1 16.69口 V
                                                                           느H11

                        乙U.'.,乙 / 10.
                                    （力rxl')


Therefore the peak amplitude of v。at 3.16 rad/s is 20.97 V.


Problem 14.2
In the circuit in the figure, the peak amplitude and frequency of the sinusoidal voltage source are
constant. The capacitor is adjusted until the peak amplitude of v。has its ma址mum value.
       a) What is the expression for C in terms of R,L, and w?
       b) What is the value of 1 V。1max?
       c) What va岫 of C싸ill 叫 the circ山 奴o series resonance?
       d) How do the answers for parts (a) and (c) compare for a high-Q circuit?
                                           (v0) I for a high-Q circuit?
       e) How does I '1。1max compare to I V。




                                                   닉7, cos 口寸
 Part B: Representative Problems with Solutions                                                      217



 Solution
       a) To find the value of capacitance that will m血ize the peak amplitude of vO we de小e the
expres如n for the am메tude 可％ as a f山iction of C. Using phasor－面main analy前s we can wri妃 the
expression for V。as

                V=                        F뇨四으                                 口n
                     U            /                           I    \           1 I0乂:1
                                 IR+ iwL+ 1w;
                                          rd                                           /
                                  \                                /



                                              F今1 四으
                                 (1- w2LC) +jwRC '

        Let V,,口 represent the amplitude of VO. Then


                I乙4n =
                                                         Vm
                     "W V下 w2LC)2 + w2R2C2
In the expression for I'4口 C is v缸iable and w, R, andL are fixed.
        Ne虹 we find the value of C where the derivative of V, m with respect to C is zero. We find
dV,,,,/dC is zero when

                                      L
                C-
                戶，


                     =           八        m'         .
                                11二 1   二r 二
                                八   十 口J J乙




Let Cm represent this critical value; i.e.,

                                          U
                 m=              R2+c。2i
                                      L2

       b) When C = Cm we find the denominator in the expression for V, i, reduces to

                 2! ／져       .   2 ,2. ..2                               八
                                                                                  n2
                ) L.L771 - 1 十 口) 八
                                      L771                        == ,,2 . 2. 2 ·
                                                                     八 十 口) L.


Therefore,
                                                                           드
                                                                                VR2 + w2L2.
          Vmc
                         (m缸）
                                      =   N
                                               'OI       카    =        R
218                                                         Chapter 14/Series and Parallel Resonance




       c) Let CO represent the capacitance corresponding to unity power-factor resonance. Then

               -                1
          LO= -:;-.
                            ofL

       d) In comparing Cm to CO it is convenient to re싸rite Cm in the following form:

               -                              L
          Cm =
                                      I           2r2\
                            n2 1 4 .WI- .               I
                            PC II 十 =-I
                                      I
                                      I   '
                                                  11=
                                                  PC    )
                                                        I




But w2L2/R2 is Q2 for a series resonant circuit. Hence

          C-            =                     L
                   ''       R 2 (l
                                (1 + 0
                                     Q)2

For a high口 circuit, Q2 >> 1, and the expression for Cm becomes

               -L
          Cm 勺 m1 )
               0e／之e
or

                                          1
          Cm
                            쌉구L三

                            七   CO.
Therefore for a high-Q circuit the capacitance that maximizes the peak amplitude of vO is very near
equal to the capacitance that results in unity power-factor resonance.

       e) When C is adjusted for unity power-factor resonance, the amplitude of vO is Q times the
amplitude of the source voltage; i.e.,

           V뇨o(max)（口）o) = QVm ·

The expression for Vmo(maX) S


                     .22 =VmVi;：万2.
          吼（蜘）＝智VR2* 。iL
Part B: Representative Problems with Solutions                                                      219




Therefore when Q is high, the expression for V, O(maX) can be approximated as

          V油伽x) 仁 QV,加

Thus in 址gh-Q circuits

          Vmo(maX) 七 P io(wo)



Problem 14.3
Scale the circuit in the figure so that the unity power-factor resonant frequency is 1,583,571.69 Hz and
the impedance seen by the ideal sinusoidal current source at resonance is 400 kQ. Specify the scaled
values of Rg，尺乙 and C.




Solution
For the circuit in the figure the resonant frequency of the unscaled circuit is

                                    lH2
                              m
                              匠＼
                                ）
                                日
                                       = V100 -1 = v'9rad/s.
          wO1 = [iZ
                  11
                                                                                                           H




The resonant frequency of the scaled circuit is specified to be 1,583,571.69 Hz, or

          nb2 = 27r (1,583,571.69) = 9,949,874.38 rad/s.

The frequency scaling factor, kf, is

          .     nJo2   . n6
          KcJ = =:11
                wO1
                     = IUI
220                                                                   Chapter 14/Series and Parallel Resonance



       To fmd the impedance scaling factor we first calculate the impedance at resonance seen by the
current source in the unscaled circuit. From Eq. (14.66) we have


           Z(wO1) = , , 三L. , = ., 三쨌刃）5) =400Q.
                           八gi\ U   丁L         ( LUUU) ( J)
                                                              .1- c
                                                  500          "

The impedance seen by the current source at the scaled resonant frequency w。
                                                                           2 is s們cified to be
400 kC; therefore the ma얍litude scaling factor is

                  1J\ 11     d』13




          km＝ 耿川協' "                =
                                        ix凡·

 . . . 여놘小ndk伊e kn애n, the values可如毗uit paramete心뇨the scaled circuit缸e ea出y
ooLalneu. I nus


          Rg = 2000km = 2Mg,

          R = 5km =5kQ,


          L = (km/kj) 5 =5mH,
and

          C = (1/kmkf) (1/500) = 2 pF.


Problem 14.4
The operational amplifier in the circuit shown in the figure is ideal. If Vg = 30 cos wt mV, at what
frequency will the operational amplifier saturate?
Part B: Representative Problems with Solutions                                                     221




                                                   5k11            5kO




                              Vg
                                                                               10 kfl




Solution

Finding the frequency that causes the operational amplifier to saturate requires deriving the
expression for the output voltage as a function of w. The derivation is done in the phasor domain. Let
Va represent the phasor voltage across the capacitor, positive at the upper terminal. Now write two
node voltage equations. The first equation sums the currents away from the inverting input terminal
of the op amp, and the second equation sums the currents away from the upper terminal of the
capacitor. The two equations are

          0 mVq      O HV
            100 "+ 50三0 = 0
and



          뇨0+v小叩／1丁'小느값" 却．
whereVg = 30 X 10e3L9V.
     Solving for VO gives

          VO = -1.5 (2 +j0.75w x 10m3) V.

        The operational amplifier saturates when the magnitude of VO is 12 V; therefore the value of w
is such that

                                         l
          . 尸 / , . ,, 尸／戶．尸 2
          1.J \4十U
                     '그O乙xo
                                      7
                                 . ,,-6\ 2
                               x iu        =
                                             .八
                                             I乙，
 222                                                          Chapter 14/Series and Parallel Resonance



 or

           w = 10,327.96 rad/s.



Part C: Supplementary Problems

Supplementary Problem 14.1
The frequency of the sinusoidal voltage source in the circuit in the figure is adjusted until the
amplitude of the sinusoidal output voltage is ma虹mum. The ma虹mum amplitude of the source
voltage is 400 V.

        a) What is the frequency of v5 in hertz?
        b) What is the amplitude of vO at the frequency given in part (a)?
        c) What is the bandwidth of the circuit?




Supplementary Problem 14.2
Select the circuit values for the parallel-resonant structure in the figure so that 口0 = 500,000 rad/s,
fi = 20,000 rad/s, Vm(Wo) = 200 V, and II (wo) I = 20 A. Give the values of R, L, C, and Im.




                                           11<
                                             <<1
                                               11
                           Is            尸           I
                                                     T
                    (I,,, COS (1Jt)                               L     V。= Vm COS (wf + 0)



                                                      1                         S
Part C: Supplementary Problems                                                                     223




Supplementary Problem 14.3
A parallel RLC circuit is designed to have an impedance ma多litude of 5 kc at the resonant frequency
and 4 k(2 at a frequency of 25 krad/s below resonance. If the resonant frequency is 10 Mrad/s,
calculate the value of C in nanofarads.


Supplementary Problem 14.4
The frequency of the sinusoidal voltage source in the circuit in the figure is adjusted to unity
power- factor resonance.
       a) What is the Q of the coil at the resonant frequency?
       b) What is the peak amplitude of v。at the resonant frequency?
       c) What is the Q of the circuit?
       d) What is the bandwidth of the circuit?


                                              150 k[1




                                    V9                               20 pF

                            (40 cos w0t V (




Supplementary Problem 14.5
A 20-mH coil with a Q of 25 at 10 Mrad/s is used in the circuit in the figure to design a
parallel-resonant circuit. The resonant frequency is specified to be 10 Mrad/s.
        a) Specify the value of C in picofarads.
        b) Specify the value of R so that the Q of the circuit is equal to 20.
        c) Specify the bandwidth of the circuit in kiloradians per second.
224                                                              Chapter 14/Series and Parallel Resonance



Supplementary Problem 14.6
The internal impedance of the sinusoidal voltage source in the figure is 40 + JO Q. The frequency of
the source is set at the unity power-factor resonant frequency of the circuit. The amplitude of the
source voltage is set to yield an rms value of 500 mV.
                          町芦“斗擢州努；芯
                                                               40mH
                          虹累＼"규득V子．
                                                lofi

                          r， j
                           口．r.
                          忖근堪灘                                        0.25尸F不   V0




                          立二．,；료                                          1 '
       a) What is the rms value of vO at resonance?
       b) If v。is measured by an rms voltmeter having a resistance of 10 kQ, what 的l the voltmeter
          read?
       c) Repeat part (b) given that the meter resistance is 100 kQ.


SunDlementarv Problem 14.7
The frequency of the sinusoidal voltage source in the circuit in the fi凹lre is adjusted until the circuit is
operating at unity power factor.
       a) Calculate w0.
       b) Calculate vO at the unity power-factor frequency.
       c) Calculate v。at w = 0 rad/s.
       d) Calculate vO at cv = m rad/s.
       e) I沁 you t뇨nk the a卿litude of v小 ma血ium at 口J = w0?
       I) Calculate v。when口J = 1.384 Mrad/s.

                                                       lookn




                       10 cos u寸
Part C: Supplementary Problems                                                                     225




Supplementary Problem 14.8
The op amp in the circuit in the figure is ideal.
       a) Find the value of R so that vO is 180' out of phase with Vg at 800 Hz.
       b) When R has the value calculated in part(a),what is the steady-state expression for vO if Vg
          = 7.07 cos 160Uirt V?
                             Chapter 15
               Introduction to the Laplace Transform


Part A: Representative Drill Exercises with Solutions

Drill Exercise 15.1
Use step functions to \\Tite the expression for each of the functions shown.

                                                              ' ,
                                                                仕）


                                                                            10 닯n 町t (0드 r드 2)


                                                  r（引                                                   r（引
(a)
                                                              -10
                                                        (b)



                                   썲
                                       1/
                                              /                              f(s)

                           (c)
Solution

       a) For t 5 Of(t) is zero and for 0 5 t 5 2,1(t) is a straight line with a slope of 5. Hence the step
function u(t) can be used to turn the ramp function 5t on at t = 0. Thus

          f (t) = 5ru(t)         0 드 r 5 2.

From 2 5 t 5 6,f (t) is constant; therefore, if a ramp function starts with a slope of -5 at t = 2 and is
added to the ramp 5t u(t),f(t) will be constant fort 之 2s. Thus the function

          f (t) = 5t uQ) .. 5 (t - 2) u(t - 2)




                                                                                                        227
 228                                                                                       Chapter 15/Introduction to the Laplace Transform



is a ramp with a slope of 5 for 0 5 t 5 2 and a constant 10 fort 之 2.
        For 6 5 t 5 8,1(t) is a decreasing ramp function with a slope of -5. To generate this portion
off(t), add the term 中5(t 中 6)u(t - 6) to the previous function; thus

          f (t) = St u(t) - 5 (t - 2) u(t - 2) - SQ 卞 6) u(t - 6).

        Testing the function at t = 6, 7, and 8 s, respectively, yields

          f (6) = 30 - 20 - 0 = 10,

          f (7) = 35 - 25 - 5 = 5,
and

          f (8) =40 - 30 - 10 =0.

      Note that all these values agree with the givenf(t).
      Finally the function is zero for 8 5 t 5 oo. Force the function to zero in this time interval by
adding a ramp function with a slope of 5 at t = 8. Thus the complete expression forf(t) becomes

          f (t) = St u(t) - SQ - 2) uQ - 2) - SQ - 6) u(t - 6) + 5Q - 8) u(t 中 8) .

        b) Heref(t) is a sinusoidal function for 0 5 t 5 2 and zero elsewhere. Therefore step functions
can be used to turn the sine wave on at t = 0 and off at t = 2. The difference between u(t) and u(t -
2) will be 1when 0 < t < 2 and zero when t is less than 0 or greater than 2. Hence we expressf(t)
                                                                                                  as

          f(t)   =   [u
                           (t)
                                       小       u
                                                   (t
                                                             -
                                                                 2)
                                                                      ]    sin兀L
       c) There are two ways of using step functions to generate an analytical expression for the ramp
function given in figure (c). The two methods are summarized as follows.
       In the first method: (1) turn on a ramp function with a slope of 4 at t = 0; (2) add a ramp with
a slope of -4 at t = 5 s; and add in a constant of -20 at t = 5 s. This approach leads to the expression

         f (t) = 4t u(t) - 4(t - 5) u(t - 5) - 20u(t - 5).

      In the second method turn on the ramp function 中 at t = 0 and turn it off at t = 5 s. This is
done by creating the rectangular pulse [uQ) - uQ - 5)]. Using this pulse,

         f(t)    =   屯    [u
                                 (I)
                                           -            u
                                                            (t
                                                                  -   5)
                                                                                   ]   ·
                                                                                                       229
Part A: Representative Drill Exercises with Solutions




Drill Exercise 15.2
Findf(t) if

          f(t)：去f!, F(w).加dw
and


        「呼詩昏6(w).
Solution

Usi邱 the s蹄雎 pr아心口 of the ii叩毗e fu耐帥，

          -. . 1 r的 (3 + jw) , - . . 7r ,.o+ (3 + jw) , . . . 1 3 3
          Jt)＝石J이4＋川兀아叩m= 石k (4+ ]이叩坦cv＝三 ' 4＝죵 '



Drill Exercise 15.3
In the circuit in the figure, the dc current source is replaced 꿔ith a sinusoidal source that delivers a
current of 1.2 cos t A. The circuit components are R = 1 Q, C = 0.625 F, andL = 1.6 H. Find the
numerical expression for V.




                   1dc
                                  )                                   C
                                                                          '
 Solution

 When ig(t) = 1.2 cost

              衣1) 七 1.2
                  了2+        ,i
 and Eq. (16.42) reduces to



                         \
                          ,
              V(s)= 小加小 夕入．           /   3   거r. I느
 230                                                                                                     Chapter 15/Introduction to the Laplace Transform



 For the given numerical values of R,L, and C,

                                                                  2
                          yrr) =                             1.yzs
                                                             d   ,＼八




                                ' '         (s
                                            (S2 +1.6s+ 1) (s2+ 1) '


Drill Exercise 15.4
                                            :*, )(1.92s2
 m4
 Findv                if
                                              + 1)(s2 + 1.65 + 1)
       「
           （
                 《）
                      『
                           『，
                                  :
                                      (:
           (t)
                           v5
                                  =
                                      (s2
 Solution

First we note that V(s) is a proper rational function and therefore it can be expressed as a sum of
partial fractions. The partial fraction expansion requires the denominator polynomial be written in
factored form. The roots of the denominator polynomial are

                          (s2 + 1.6s + 1) = (s + 0.8 - j0.6) (s + 0.8 + j0.6)

and

                      (s2 + 1) = （了 H月）(s ＋月）.

Therefore V(s) is

                                                                                         =     』＼m
                                                                                             I .Ll乙I.
                                                                                                     2
                      V(s) =(s + 0.8 - jO.6) (s + 0.8 + j0.6) (s - jl) (s + j1) '

The partial fraction expansion of V(s) is


                                                   K1                                              心           K1        蚣
                      V(s) = (s
                             (H0.
                                + 0.81j0.6)
                                     -j0.6) + (s
                                              0+ 仙．
                                                  0.8+
                                                    nj0.6)
                                                       j0.6) + (s
                                                               0加 -j1) + (s +j1)
It follows that

                                               d   』＼八   /       ,1    ,1   .   . ,1   /\2




                      局 乙1.2（茹닦뀨鼎加尸幽프至
Part A: Representative Drill Exercises with Solutions                                                                                                                                                  231




and

                                                                                 d    r1八     /.4\                     2
                                                                                       #L
                                                                                                                                                 (j2)
         K2
                                                               j0.
                                                                                 1.
                                                                                                                                                                 印
                                    (0.8*                                              (。 +
                                                                                                                                                        =
                                                                                              V
         K什
                                                                                                                                                            0.
                                                                                                                                                                          ..Q:   v.
                                        +
                                                                                                            I)
            =                           (。
                                                     .8
                                                               j。
                                                                           .4)
                                                                                                  .8
                                                                                                                           jl.
                                                                                                                                      6)
BydefmitionK; = 1／二233.13' andK2 = o.6o匹.
     A direct application of Eq. (16.67) leads to

                  ..                         I八 -Il.Ri                                            . n / . 八八八 . 八, . . . 八                                                            1 . . ..
                                                                                                      6 + 233.130) + 1.
                                                                 "   . 나

          v
                  (t)
                                =            L2e
                                                                                      cos         (0.
                                                                                                                                                                 2c051]
                                                                                                                                                                                        u
                                                                                                                                                                                            (t)
                                                                                                                                                                                                  V.
Drill Exercise 15.5
Findf(t) if

          F(s) = (2s3 + 8s2 + 2f 日) /(S2 + 5s + 4) .


Solution
Start the analysis by observing that F(s) is a improper rational function. Before finding the inverse
Laplace transform ofF(s), express F(s) as a polynomial plus a proper rational function. This is done
by dividing the denominator polynomial into the numerator poiynomial. This division yields

                                                                     2*                                                          + 1
                                                     얌
                                                                                                        4
                                                                                        (:
                                                                                                                 (s)
                                                                     2+                                 + 1) (s + 4) ,
                                                                                                                                             )
                                                     2s
                                    ＝
                                    =
                        (5)
                        (s)
              F
              F
                                                                                        (s
 or


                                    =                                2
                                                                                 +                      + 4)
              F
                          (s)
                                                      2s
                                                           -

                                                                                         (s
                                                                                                                                  ·




 The polynomial terms can be inverse transformed using the transform pair given in Eq. (15.9). Thus


              f(t)              =            2祭小4e
                                                                                                                             tu        (t)
                                                                                                                                                 .




 Note the polynomial terms in the s-domain generate impulse functions and derivatives of impulse
 functions in the time domain.
 232                                                                                          Chapter 15/Introduction to the Laplace Transform



 Drill Exercise 15.6
        a) Use the initial-value theorem to find the initial value of v in Drill Exercise 15.4.
        b) Can the final-value theorem be used to find the steady-state value of v? Why?


 Solution

 From page 618 of the text we have

               - -, .            1.92s2
               r （刃 =     )               )
                        (s日 + 1.6s + 1) (s勺 + 1)

Therefore


          了V1（刃 =
                         1   l
                                  S
                                      프
                                          l
                                          De
                                          O


                                          d
                                          l
                                          +
                                           /


                                           12
                                            1
                                          1H 了        1
                                                          1
                                                              1
                                                                  \
                                                                          1
                                                                              l
                                                                                      2
                                                                                          !
                                                                                                      1
                                                                                                      /
                                                                                                          +
                                                  J
                                                                                  S
                                                                      1
                                              /
and

               Un까
                     寸 （了） = 0.
          S.
                .



It follows from the initial value theorem that v(0+ ) = 0.
        Observe that this result is in agreement 꿔ith the discussion of the circuit in Fig. 15.16 (see p. 618
of the te肛book) where it is stated there is no energy stored in the circuit at the time the switch is
opened.

       b) No, V(s) has a pair of poles (s - j1)(s + j1) on the imaginary a疵.



Part B: Representative Problems with Solutions

Problem 15.1
In Section 15.3, we used the sifting property of the impulse function to show that L{6(t)} = 1. Show
that we can obtain the same result by finding the Laplace tr缸lsform of the rectangular pulse that
exists between 土 e in the figure and then fmding the limit of this transform as e - 0.
                                                                                                 233
Part B: Representative Problems with Solutions




                                               尸（t)

                                       2



                                           냐        0            i


                                                                     _ae_8(t_ t)


                                                -
                                                    8




Solution
From the figure and the definition of the Laplace tra好form, the transform of the rectangular pulse
between 士e is


         뺘亡仁卜小 "';:'"
Using L'H6pitals' rule yields


          limit
          빻枷戶   F(s)=-   limit      +se"-SE
                         e-'O 'Is"eSE,1
                    士12s 呵'                             =   1.
Problem 15.2
 Show that


          L 何勺(t) } =F(s ＋口）.

 Solution
 Using the definition of the Laplace transform we have


             L{e f아寸，- e 'f(t)e "dt

                       玎弘t)e （了' a)t dt
                       = F(s + a).
 234                                                         Chapter 15/Introduction to the Laplace Transform



 入rote: If


                           F(s) =J;f(t)e'" dt
 then


                 耶回玎和（加如 ' "ydi·


Problem 153
The make-before-break s팎itch in the circuit shown in the figure has been in position a for a long
                                                                                                  time.
At t = 0 the switch moves instantaneously to position b.

         a) Derive the integrodifferential equation that governs the behavior of the voltage v for I > 0.
        b) Show that


                             나勺小＋(1的］
             V
                       =
                            s2 +         RC) +         LC)
                 (s)
                                   (s/
                                                 (1/
Solution
         a) Since the switch has been in position a for a long time prior to moving to position b, the
capacitor looks like an open circuit and the inductor looks like a short circuit at t = 0 . Therefore the
initial voltage on the capacitor is VdC, positive at the left terminal of the capacitor. The initial current
in the inductor is (VdC/R) into the upper terminal of the inductor. The differential equation that
governs the behavior of the voltage v for t > 0 is

                 dv . v . 1 ,:               .         Vj
             勺간 R 十 E J 0+ var 十 下- = U.
Part B: Representative Problems with Solutions                                                    235




      b) The Laplace transform of the equation in part (a) is


          c    [sV尸
                           (_
                                V1c)
                                             ]     V. V .Vdc
                                                 + R 十 L計 而 = U,

or



         唯『加c]                                    = ＝叱Ic   ［未
Solving for V gives

                      -Vdc (s + 1/RC)
          V=
                      (2 .             S     .    l \
                      (S
                           十RC；十L司




Problem 15.4
       a) Write the two simultaneous differential equations that describe the circuit sho끼l in the
          figure in terms of the mesh currents i1 and i2.
       b) Laplace-transform the equations derived in part (a). Assume that initial energy stored in
           the circuit is zero.
       c) Solve the equations in part (b) for ri (了) and/2(s).
       d) Find i1(t) and i2(t).
        e) Find j1(미 and[ i2(oo).
        f) Do the solutions for i1 and i-, make sense? Explain.

                                                                5H




                                           180u(t) V




 Solution

        a) For the circuit in the figure the two mesh-current equations for t > 0+ are
 236                                                                                                       Chapter 15/Introduction to the Laplace Transform



                                                                              m
                             跏       m
                                     +                                奭꺄    d(i1-, i2) + 154,,( i1 -                     h而
                                                                                   e

                              =
                                                                                   m                 b)           + Sd
                                                                                                      U'




                                         . 尸 d ..     .                                戶 di1 ．八．
                                     U = l> U1.-(1, -1i '-                             D----+ 1(J, .
                                                                  at ' H      -,         at                -
These equations can be simplified to

                     dii  di,
          180u(t) =30- -20- -
              "      at    at

                                            dii
                                                                                                  竺
                                     0 = 叫20-二 + 101, + 15
                                            at      e                                         m
      b) Since the initial energy stored in the circuit is zero, i1(0+ ) = L2(0+ ) = 0. Therefore the
Laplace transforms of the differential equations derived in part (a) are

                             180
                                            = 30sf1 - 20512,
                             S


                                     0 = -20s11 + (10 + 155)12.

       c) Using Cramer's method for solving simultaneous equations gives

           (5)                          18                      s+
          n
                                 -                (
                                                            3
                                            s2
                              -                       (s+
                                                                      6)
                                                                       2)

and

                                                  72
               (5)
                              :
          '2
          72
                                      :(:
               (5)
                              =       s      (s
                                                            + 6)       ·




      d) The expressions for 'i (s) and 12(s) are proper rational functions; hence they can be
expanded into sums of partial fractions. We get


                                            6
                                            H2S                 8
                                                                H S
                         臼
                                                                        8
                                                                       s+ 6
                     ＼
and

           . .                        12                          12
         i2(SJ = m小 e
                  S   s+ 6
Part B: Representative Problems with Solutions                                                            237




It follows directly that


           i1   (t)   =       [&    +8   -   8e小                        (t)        A
and


          b(0=                [12    -   12e小                (t)              A

        e) i1
            （끼 = 00                      and                  b (m) = 12A.

        f) Do not be too surprised to find i1(t) -, 的 as t 斗 oo since the linear transformer has no
resistance in its coils. It is not immediately obvious that i2 should approach a constant value of 12 A.
However, we can test this result as follows. The voltage across the 15-H coil is

                  』尸 d . .    . . . 戶（刃I
                       ,(1 叫 i 2) 十 > 二1
           V15H = l:) 二m
                                    Ui                                        Ui




                      = (120- 12C匕U日）u(t) V.

Thus as t -, 的, yl5H 斗 120 V, and i2 斗 (120/10), or 12 A. In other words as t - 00 both i1 and (i1 - i2)
approach m at a linear rate; i.e.,

           il- . & + 8 as t -,

出ld (i1 - i2) - 6 中 4 as t - m. Therefore v1511 - 120 Vast-. 的
       Also note that

                                             d 1        -          i
                              5di14·
                                  +5 5                                 2)
                                                   (i
           V511
                               dt                       dt
                          =
                          =    5-
           ,m
                      = (60 + i20eH ') u(t) V

Therefore v1511 -* 60 V as t - 00
       Thus at t = 00 the source voltage is balanced by the sum of VSH + V1SH.
       Note further that i1 can still approach infinity as t -. 띠 since the circuit resistance is zero; i.e.,
(180 - 180)/0 is an indeterminate form.
       Finally note that v1511(0+ ) = 0 and v5H(O+ ) = 180 V are in agreement with the results that
i1(0) = 0andi2(0) = 0.
238                                                            Chapter 15/Introduction to the Laplace Tr띠lsform



Part C: Supplementary Problems

Supplementary Problem 15.1
Use step functions to write the expression for each of the functions shown in the figure.


                                         f)t)

                                         10



                                                                                      r（引

                                                         r（引
                               -10              10

                         (a)                                    )b)




Supplementary Problem 15.2
There is no energy stored in the circuit shown in the figure at the time when the switch is closed.
       a) Derive the integrodifferential equation that governs the behavior of the current i.
       b) Show that


           (,      [dC               l
          f
              )=
                                                     .




            ' '     L    2 .R               . 1 '
                         S 十 =-S 十 :=
                             L     I乂／




Supplementary Problem 15.3
The current in the inductor and the voltage across the capacitor are zero at the time when the switch
is closed in the circuit shown in the figure.
Part C: Supplementary Problems                                                                        239




       a) Derive the integrodifferential equation that governs the behavior of the voltage v.




Supplementary Problem 15.4
There is no energy stored in the circuit shown in the figure at the time when the switch is closed.
       a) Derive the integrodifferential equations that govern the behavior of the mesh currents i1
          andi2.
       b) Show that


                                      (s2L2C + R2Cs + 1) Vg
          1.   =




          "        了3L1L2C + 了2C (R1L2 + R2工i) + S（사凡C + L1 + L2) + 사 + 凡 '




Supplementary Problem 15.5
The values of the circuit parameters in the circuit in the figure are R1 = R2 = 1(2, L1 = L2 = 1 H,
afldC = 1F. Ifvg = l0ui(t) V, findi1(t) fort >0.
240                                                                                                Chapter 15/Introduction to the Laplace Transform




Supplementary Problem 15.6
Findf(t) for each of the following functions:


          a) 胸乙（』
                誓(s2）
                   꺾，),
                    (s)   =          .    30       ('   ..+.         1)   .   (s.   + 2)   .   ,
               F
          b)
                              了 (5 十 .)) (,S                              十 yS 十 乙U)




          .)
          c)   " 0) =
               F    (s)       s
                              ,     (s2       500
                                               + 1 ++6)1呵  (s
          ') 耶）= '므：'*긍므）
                        ,
                                              * 800s
          e)
                                      2                                   125)2
               F
          0)   『
                                              + lOs +
                   （5)        (s2
                              (:
                          :
                                                  :
                          =
                   (s)
                                              s2
                   (s)    :   10          (   , (+              9s
                                                                      +
                                                                     5) 18)
          0F
                          -                   s
                                                  (s+
Supplementary Problem 15.7
Apply the initial- and final-value theorems to each transform pair in Supplementary Problem 15.6.


Supplementary Problem 15.8
Use the initial- and final-value theorems to check the initial and final values of the current in the
circuit in Supplementary Problem 15.2.
Part C: Supplementary Problems                                                                         241



Supplementary Probjem 15.9
Use the initial- and final-value theorems to check the initial and fmal values of the voltage in the
circuit in Supplementary Problem 15.3.
                          Chapter 16
           The Laplace Transform in Circuit Analysis


Part A: Representative Drill Exercises with Solutions

Drill Exercise 16.1
A 125-Q resistor, a 4-mH inductor, and a O.1-4uF capacitor are connected in parallel.
       a) Express the admittance of this parallel combination of elements as a rational function of s.
       b) Compute the numerical values of the zeros and poles.


Solution
        a) In the s domain the admittance of a resistor is (1/R), an inductor is (1/SL), and a capacitor
is sC. Since these three branches are in parallel,


          Y(s) =
                          lR
                           十 二：=m 十 Sc
                               1
                                             .   -




                             )iJ




                =
                    1늦*
                                   笙，
                                        9+
                                                     O.1x10   s


                      7S2                 8
                    1。    + 80,00小 + 25x10
                           -
                =
                                                       S


       b) After factoring the numerator polynomial, the expression for Y(s) is


           Y(s)=l르으『띠）,x刃－j羽，어y) (5* 40,cx刃* j30,O(劤．         S


It follows directly that the zeros of Y(s) are

           -z1 = -40,000 + j30,000,




                                                                                                       243
244                                            Chapter 16/The Laplace Transform in Circuit Analysis



and

             e22= -40,000 -j30,000.

Y(s) has a simple pole at the origin; i.e.,P1 = 0.


Drill Exercise 16.2
The dc current and voltage sources are applied simultaneously to the circuit shown in figure A.There
is no energy stored in the circuit at the instant of application.
       a) Derive the s-domain expressions for V1 and V2.
       b) Derive,for t> 0, the time-domain expressions for v1 and v2.
       c)
       C) CalCUlate
          Calculate v1
                    Vl(C      V2(0+).
                      (0+)and v2
       d)Compute the steady-state values of v1 and v2.




       (a)
Solution

       a)Since there is no energy stored in the circuit prior to applying the dc sources, the s-domain
equivalent circuit that applies for t > 0e is as shown in figure B.




       (b)
The two node-voltage equations are


                                   51 S
             V1 - V2
                       +   ViS =
               S
Part A: Representative Drill Exercises with Solutions                                              245



and
                                                         助
                    吃               V                    0 巧
                            U


                                            卜                                     0
           브
                                                 H




                            S                             +=
           3
鈿lvi雎 for V1 and j;今 蜘es

          v1 =1孕G브쓰1.
               1
                =                           戶1       .   =   \


                   S (S 十 乙＞S 十 I)
                       /        .   八




and

                           2.5 (2 + 6)
          V2 = =1m          '
               S (f + 2.5s + 1)


       b) The expressions for V1 and V2 are proper rational functions. The partial fraction expansions
for V1 and V2 are

              15                 (      . (5/3)
          v1= s                 s'+ 0.5 十 s+ 2 '
and

                   15           (                                (25/3)
          v, = m11 =m 1 " n m + 斗m寸＝.
           日    S     S + U.>   了+ 2


The inverse transforms of V1 and V2 are

                                        m了               코
                                                                                      m   V
                                                                          m
                                                                                                             +
                                                                   5
                                                                                  n
                                                                                                         4
                                                                                                         1


                                                                          川
                                                                   于
                                                                          ］
and

                                                                       희r                 m
                                                                                          V
                                                                              m
                1. ,  125 -0.5:                                                       n
          V-) = I U - m1七
                                                                              川
                   L                    0                                     1
                                                                              J
       c) From the expressions for v1 and v2,

         v1(0+) = 0 and v2(0+) = 2.5 V.
246                                                        Chapter 16/The Laplace Transform in Circuit Analysis



These values make sense, as can be seen from the circuit in figure A. For t < 0 the capacitor is
short-circuited by a switch; hence v1(0e) is zero. In this circuit there cannot be an instantaneous
change in the capacitor voltage; therefore vi(0+) is also zero.
       The inductor current is zero at t = 0+: hence the inductor looks like an ooen circuit at t =
0+. Therefore when the switches operate, the 3-Q and 15-Q resistors form a voltage divider across
the 15-V source. It follows that

                 ,    /3
                     .+.


             V2(U ) = (i司 I) = 乙'> V.
                                     \.            ,   .




        d) From the ex마essions for v1 and v2, it follows that v1( ) = v2(미 = 15 V.
        Note that these values make sense in terms of known circuit behavior. After a long time the
inductor behaves like a short circuit and the capacitor acts like an open circuit. Therefore at t = 口）
the circuit appears as shown in figure C. It follows from this figure that



                                                   十匠
                                     5-4                                           (5V
                                            中！
       (c)
                           V2 - 15                                                       +
             立
                                     - c = (1 tr 1,八 = 174 = i cv
             3
                             15        V   ' ' ' -'    ' 1 1V "



Drill Exercise 16.3
The switch in the circuit shown in figure A has been in position a for a long time. At t = 0 the switch
moves to position b. Compute (a) v1(0e); (b) v2(0m); (c) v3(0e); (d) i (t); (e) v1(0+); (f) v2(0+); and
(g) V3(0十）.




                                           100 V




       (a)
Part A: Representative Drill Exercises with Solutions                                                  247



Solution

       a) After the switch has been in position a for a long time, the sum of the voltages v1 띠ld v2
must be 100 V. Because the capacitors are in series, the charge on each capacitor is the same;
therefore

             v1C1 = v2C2,
or

                     q可 l   l
                            H4
                             l
                             V                     =
             V2 =



It follows that
                             0
             V   0          l社       m                           1
                                                                 H

                                                                     +=


or

             v1(0 )=80V.


       b) From part (a) we have
                          朗      V
                                 加                                                               =

             v2(0 ) =   le 4                                                                    \1/




       c) By hypothesis there is no charge on the 1.6-4uF capacitor at t = 0 ; therefore v3(0) = 0 V.

       d) The s-domain equivalent circuit for the circuit shown in figure A that applies for t > 0U is
shown in figure B.




                                 誓
       (b)
248                                                                          Chapter 16/The Laplace Transform in Circuit Analysis




The expression for I is obtained by dividing the total voltage by the total impedance. Thus

                                        00/                                  iO-
            I
                =


                    4   八O
                            -     (1
                                                s
                                                    )             =   32 x
                                                                                   6.
                    프- (2 + 0.5 + 0.625)
                        S

Taking the inverse Laplace transform yields

            i = 326(t)1uA.

       e) Because there is an impulsive current, there can be an instantaneous change in a capacitor
voltage. The change can be found using the integral relationship between v and i. Thus

                                                6             +

                v1(O') =능---f- 32x 10'66(t)dt+ 80
                                        d   ,




                                = 16V.

       0
                                        4   ,   6             +
                v2(0+) = ---                        fU.- 32 )< lo_66(t) dt + 20
                                        乙               I.,




                                = 4V.

       g)
                                        d   ,   6             +
                v3(O+) = -,-
                          I                         1U.- 32 x 10H66(t) dt + 0
                                       1. O             '.1




                                =20V.

These values of v1(O +), v2(O +), and v3(O +) are consistent with the conservation-of-charge principle.
That is, at t = 丁, the charge in the system is

            q1 = q2 = 40uC.

At t = O+ the charge in the system is also 中C) /{C; i.e.,

            q1 = q2 = 81uC
Part B: Representative Problems with Solutions                                                     249




and

               q3 = 32AuC.



Part B: Representative Problems with Solutions

Problem 16.1
Find the poles and zeros of the impedance seen looking into the terminals a, b of the circuit shown in
fi昏ire A.




                                                                 iF




                                                                 iF




       (a)
Solution
The s-domain circuit is shown in figure B.

                             比




             (b)

Either the upper or lower delta connection can be replaced by an equivalent wye. We shall replace
the lower delta. The circuit reduces to that shown in figure C, where
250                                                                                                    Chapter 16/The Laplace Transform in Circuit Analysis



                                                  2
                        -.                        S
              乙1
                                 =     2 . . .
                                      S 十了 十 I



                                 =
                             1
                   Z4
                                      S2S +s+ 1 '

and

                    -                             1
             乙3=
                                            S2 + , + 1




                                                                                                                           吉皿
       (c)
       The impedance Zab can now be found by series-parallel reductions. Thus

             z1+                      1       쑈       2f2+                    1 +l
                                                  了2 +                   I.   +      ]   ,




                                     l
                                     H S
                                                             寸+ S + 1
             z2+
                                                  了          (2S         + S + 1)            '




Let Z4 represent the parallel combination of (Z1 + 1) and [Z2 + (its)]; then

                                                                   ／八 2 .                    . m. 2
             z4=                                                   （乙S         .     十S十I)                .
                                                                                                              .




                                                      5+ 1)                              『       52+ 25+ h]
                                                                               L얌3
                                     (52+
Part B: Representative Problems with Solutions                                                        251



The impedance seen looking into the terminals a, b is

             Zab == Z3+ 'Z4


                                     2 (s2+ s + 1) (2s2+ s + 1)
                                   (s2+ s+ 1) (2s3+ 3s2+ 2s+ 1)

                                     2
                                   (s+ 1) '

        From the expression for Zab, observe that there are no zeros in the finite s-plane and there is a
first-order pole at -1.

       a) The s-domain equivalent circuit is shown in figure D.

                                                                  (4X/o) 后



                                                                                定J之




       (d)

       The node-voltage equation for the solution of V0 is

               . ,                  (5／노） 了             -




               V0 . n 4 - . L U ' V ' " ' J'
                                                              ］
                                                              '
                                                  1v
             八n小，\ + (12／   甲 + 月 \/ 1r노6<   = 0'
             乙＼    (X)0 V 'Hr
             20J,..UUU          4)< 10"

The relationship between I                        and V0 is

             ,        =   [(51s)       -   0.   5 v0]
                 Y/                   4000


The solution for V0 is
252                                                                  Chapter 16/The Laplace Transform in Circuit Analysis



Expressing V0 as a sum of partial fractions yields

             .,   -10 .   15
             V0 = 二二 十 了 + 100

It f에ows that the ti毗＜lomain expres如nf아 % is


             % = (- 10 + 1知-1어y）呻）V.



       b) After the switch has been closed for a long time, vO is -10 V. The voltage across the
capacitor is 5 - (- 10), or 15 V. Therefore the final charge on the capacitor is

                       /r\   八尸   d   nH
             q "oo) = ('U·乙：) >( lu
                                                 /4   -\   八   尸1尸   r\
                                                )(I기 = 工／)/iU.
                                           6\
Problem 16.2
The initial energy in the circuit in figure A is zero and vg(t) = 6004u(t).
         a) Find I (s).
        b) Use the initial- and final-value theorems to find i (0) and i (oo).
        c) Do the values obtained in part (b) agree with kno꿔n circuit behavior?
        d) Find i (t).


                                                                          0.25v4,




                                                                                          140 n



       (a)
S아ution

       a) The s-domain equivalent circuit with the mesh currents defined is shown in figure B.
Part B: Representative Problems with Solutions                                                                                                                    253




       (b)

       Summing the voltages around the 'b and I meshes gives
                                                                                                                         m
                                                트四= 10 (lb + 'a) +                                                           1
                                                                                                                                 S
                                                    S



                                                        0=
                                                                     ]9 (/                       H
                                                                                                     /b) +205                        (I+
                                                                                                                                                    la) + 1401.


Now eliminate 'a from the equations by noting



             'a
                                =       .·乃／
                                                                 中   =       0.
                                                                                           25        (뀌            (ib
                                                                                                                                 -         1)
                                                                                                                                                .




After eliminating 'a the two simultaneous equations are solved for 工 The result is

             /= -150（了                                                                           )
                                    s                        + 8s+ 25)
                                               (2
                                                                                                     '




       b) It follows from the solution in part (a) that

                    (s) = -150 (                                                                             ).
                  sI        二   \   /                        /           .    rl                 .   八   尸＼


                                                             (S      十 5S 十 乙그)



 Applying the initial-value theorem gives


                  S
                  ,limit如
                            -       。O                               =            i
                                                                                      (0
                                                                                            ')
                                                                                                         =    0.
 254                                            Chapter 16/The Laplace Transform in Circuit Analysis



 Applying the fmal-value theorem gives

              1;m;t
              茗bsI(s) = j(co) = 1.2 A.


        c) To check the initial value of i, construct the circuit at t = 0+. The dependent current source
is zero because by hypothesis v甲(0+ ) is zero. The inductor acts like an open circuit because the initial
inductor current is zero. Therefore at t = 0 + the circuit is as shown in figure C. It is
apparent from figure C that i (0+ ) is zero.




                        a刃V

        (c)
       To check the final value of i, construct the circuit at t = 的. After a long time has elapsed the
inductor acts like a short circuit and the capacitor acts like an open circuit. Therefore the circuit is as
就山wn in figure I工
       Now v甲 can be found by writing a single node-voltage equation; hence

              vm- 600     vi,
                        +i布＋0.25v甲＝ 0.
              ' 10

                                                   口25呵




                           Ei) 기／



       (d)

It follows that v, = 168 V and i (的) is (168/140), or 1.2 A.
Part B: Representative Problems with Solutions                                                       255




       d) Factoring the denominator polynomial in the expression for I gives

                    r             - 150 (s- O.2)
                    J   =
                            s (s + 4 -.j3) (s + 4 +13) '

A partial-fraction expansion generates


                    I＝프亡뽀予科喘半
It follows that

                        =   [1.
                                  2 + 51.61e   ' cos   (3t
                                                                     ]
                                                             + 91.330)   u
                                                                             (t)
                                                                                   A



Problem 16.3
The two switches of fi엣re A 아比rate sync뇨onou啣．When switch 1is 叩en, swit比 2 is in position a.
When switch 1is closed, switch 2 moves to position b. Switch 1has been open for a long time and then
closes at t = 0. Find i 2 for t 之 0.

                                                                                       5c



                                                                                            5v
                                     8V




        (a)
 Solution

 From the statement of the problem, the initial current in the 1-H inductor is zero and the initial value
 ofi2 is -1 A. Using the T-equivalent circuit for the magnetically coupled coils, the s-domain
 equivalent circuit fort > 0小 is given in figure B.




              (b)
256                                                                                                              Chapter 16/The Laplace Transform in Circuit Analysis



        In studying the circuit in figure B, note that L1 - Mis zero, L2 - Mis 4 H, andM is 1H. Also
note the mitial current in the vertical leg of the T-equivalent circuit is the same as the initial value of i2
since the initial value of i1 is zero.
        The s-domain mesh-current equations that describe the circuit in figure B are

                                    8       .              八．



                       1+ H= (S+ 8) Ii -SI2,
                          S                     -               -       -                     -




                                   -5= -s11+ (5s+ 24)I2.

Solving for '2 yields

          r-      -(s+ 8)
          '2- (s + 4) (s + 12) '

A partial-fraction expansion of '2 generates

          /,
                   =         5
                             -0.
                                                      0.5                   '




               乙         (s+ 4)                      s+ 12 '

from which

          i2=          -0.
                       '0·
                                   51
                                   5
                                        -
                                                41
                                                         +
                                                         *6e
                                                                    -
                                                                        i2tl
                                                                                j   u
                                                                                        (t)
                                                                                                  A.
Problem 16.4
The magnetically coupled coils in the circuit seen in the figure carry initial currents of 3 and 2A, as
shown.
       a) Find the initial energy stored in the circuit.
       b) Find '1 and '2
       c) Find i1 and i2.
       d) Find the total energy dissipated in the 6- and the 13.5-(2 resistors.
       e) Repeat parts (a) through (d), with the current in the 9-H inductor reversed.
                                                                                                                 3H
                                                                                                       1



                                                                                                                       애］
                                                                                                                        中r
                                                                                n
                                                                                                            ／八
                                                                                                       4H


                                                                                                       1
                                                    6l                                                                               13.5fl

                                                                                                       3A
Part B: Representative Problems with Solutions                                                         257




Solution
       a) First note from the figure that one current enters a dotted terminal and the other current
leaves a dotted terminal; therefore from Eq. (13.39)


          叩나L1i三* 4L2i글－Ml2
For the values given in the figure we get


          叩＝
                   글
                           （4)
                                 (9汁｛ (4) 3
                                         (9)
                                                     -
                                                           (3)
                                                                 (2)   =   18J.



       b) The s-domain mesh-current equations for the circuit in the figure are

          61i+ 4sli- 12+ 3512+ 6= 0,

           13.512 + 9s12 + 18 + 3sli 中 9 = 0.

Solving for Il and '2 we get

                3                    .         1     尸2
          11 = H1=                 ana         i, = ＝卜＝ .
               s+ i                              -  s+ 3



        c) It follows directly from the solutions for I and '2 that

               .    ,1 e3r . .
               11 =iC UflA                     ana       i2 = 中2e 꼬u(t) A.



        d) The instantaneous power dissipated in the circuit is

           p = 硝 + 13.5i弘 10茁& w.

 The total energy dissipated is

               w= 1 108e 臼dt =18J.
                       -
                           U
258                                                 Chapter 16/The Laplace Transform in Circuit Analysis




       e) When the current in the 9-H inductor is reversed, we have
                    2h
                     +l
                      =
                             L                      J
                     L
                                  )e ）日
           叩        lH2     le2
                              1

                              y
                                          Mi1i2 =
                                                    외



          '1 = 3/(s + 1),

          '2 = 2/(s + 1),


          ii =3ee'u(t) A,


          i2= 2e_tu(t) A,


               =108ee갇W,
         p
and

               rm di\n 12i 1. 尸．1 1
          w =j.   iuoe    ar= J4j.
                u
                -
Part C: Supplementary Problems

Supplementary Problem 16.1
A 480-C resistor is in series with an 80-mH inductor. This series combination is in parallel with a
0.5-pF capacitor.
       a) Express the equivalent s-domain impedance of these paralleled branches as a rational
          function.
       b) Determine the numerical values of the poles and zeros.


Supplementary Problem 16.2
Find the poles and zeros of the admittance seen looking into the terminals a, b of the circuit shown in
the figure.
Part C: Supplementary Problems                                                                          259




                                              F161 극41 (1
                                          4IjU下
                                   a0


                                                            H



                                   b.




Supplementary Problem 16.3
Find VO and v, in the circuit shown in the figure if the initial energy is zero and the switch is closed at
r= 0.




                            24 V




Supplementary Problem 16.4
The energy stored in the circuit shown in the figure is zero at the time when switch is closed.

        a) FindvC.
        b) Find ic.
 260                                            Chapter 16/The Laplace Transform in Circuit Analysis



 Supplementary Problem 16.5
 There is no energy stored in the circuit in the figure at the time the current source jumps to 50 A.
        a) Find I (s).
        b) Use the initial- and final-value theorems to find i (0 ) and i (的).
        c) Do the results in part (b) agree with known circuit behavior?
        d) Findi(t).




                              in




Supplementary Problem 16.6
Scale the circuit in Supplementary Problem 16.5 so that the resistors become 1kQ and 5 k(2,
respectively, and the capacitor reduces to 0.02/i F.
       a) Specify the scaling factors km and kf.
       b) Construct the s-domain equivalent circuit of the scaled circuit.
       c) Find 1(1) for the scaled circuit.


Supplementary Problem 16.7
The switch in the circuit in the figure has been closed for a long time before opening at t = 0. Use the
Laplace transform method of analysis to find
      a) i1 fort 之 0;
       b) i2 fort 之 0.
Part C: Supplementary Problems                                                                          261




                                                                                 iOfl




Supplementary Problem 16.8
The switch in the circuit shown in the figure has been closed for a long time. The s꿔itch opens at t =
0. Find (a) i1; (b) i2; (c) i0; and (d) v.




                          12 V




 Supplementary Problem 16.9
 The ideal operational amlplifier in the circuit shown in the figure is operating in its linear range. Find
 vO(t) for r > 0 if the switch closes at t = 0.
262                                            Chapter 16/The Laplace Transform in Circuit Analysis




                                lv




Supplementary Problem 16.10
The voltage source in the circuit shown in the figure is the unit ramp function tu(t). How long after the
r缸lp is turned on will the ideal op amp saturate?




                               tu(t)
                                        Chapter 17
                                   The Transfer Function


Part A: Representative Drill Exercises with Solutions

Drill Exercise 17.1
The energy stored in the circuit shown in figure A is zero at the instant when the two sources are
turned on.
       a) Find the component of v, for t > 0, due to the voltage source.
       b) Find the component of v, for t > 0, due to the current source.
       c) Find the expression for v when t > 0.




                                 ,/nn: l.,,
                               ,,，《，
                                           0.4 n




                                                        L
                               V



                                                        I   '



       (a)
Solution

       a) The s-domain equivalent circuit with the current source removed is shown in figure B.

                                           口．4-rJ-

                                                            4-
                                                                 VI
       (b)
                                                   ：극
       The node-voltage equation that describes the circuit shown in figure B is

             V ' , V 's , V ' - (15/s) - 1)
             :＝卞 기＝ =H    了1       八   .    -   1J1
             U.>s    '2            0.4



                                                                                                     263
264                                                                             Chapter 17/The Transfer Function



Solving for V ' gives

                       ,.            75             25        25
                            =
                                (s+ 1) (s+ 4)     (s+ l)    (s+ 4) '
                  V.
It follows that


                  V1 =25 (e_t_ e_4) u(t) V.


       b) The s-domain equivalent circuit with the voltage source removed is shown in figure C.

                                           O. 4...a.
                                        HH小叭／                +
                                                                   그1
                                                                            ,
                                                                            了     (）軍
                                                                        T
                                                              V布
                                                                                   TS
       (c)
The node-voltage equation that describes the circuit in figure C is

             V " . V"                . V "s     7.5    』，
             =:Ue 十 === 十 1= H                me 1m = U.
             U.4    U.>s    2                     S


Solving for V " generates

             - , ,,                  15             5         5
                            =
                                (s+ 1) (s+ 4)
                        .



                                                  (s+ 1)    (s+ 4) '
             V,
The expression for 1/ " becomes


             v" = 5 (e_t - e14i) u(t) V.


       c) It follows directly from the principle of superposition that

             v = v' + v" = 30 (eHt - 4em U) u(t) V.
Part A: Representative Drill Exercises with Solutions                                               265




Drill Exercise 17,,2
The unit impulse response of a circuit is known to be

            .           1 -70:
                 m ,\ nn』          ／八 . ,L . r1\ 1, 1   -  'S    - .八．
          V叭t) = 'U"人八- e      cos （乙'out 十 (1) v, wneretantl == /／乙14


       a) Find the transfer function of the circuit.
       b) Find the unit step response of the circuit.


Solution
         a) Because the circuit is driven by a unit impulse function, we know the Laplace transform of
vO(t) is the same as the transfer function. That is,

          L{
                  vo   (t)
                             } V0
                              =      (s)
                                            =H
                                                  (s)
                                                        .




Using the trigonometric identity cos (24& + 6) = cos 240t cos 9 - 2甘［Y sinO and noting that cos 6 =
(24/25) and sin6 = (7/25) we have

           v (t) = 960目匕叫701c。s 2띠)t - 2800匕-70: sin 240.

The Laplace transform of vO(t) is

               ,,, .              96CK) (s + 70)                    2800 (240)
               Vo(S) = . . . .n.2 . .1.n. 2                     . . 거n. 2 -. . 八 . ,,. 2!
                       "S 十 八J) 十 （乙'IU)                        ( s 十 /U) 十 （乙（Ok))

or

                 . .                       960k
           Il (S) =           八                             .
                 "           (S'+ 140s + 62,500)


         b) Now that we have the transfer function of the circuit, we can fmd the response to any given
 input. For a unit step input we have
                              l                         아qY)
               V0(s) = 三H(s') = )     '
                               sH + 14小 + 62,500
 266                                                                                                                   Chapter 17/The Transfer Function



        A partial缸配如n expansion of 乙이 gives

           !   r         /   \                 K1J卜                                       K
                                                                       +
                                                   _                   1                           J1
           V叭刃 =
                                       S + /0 -jZ4kJ
                                           _   _       _   _   _   _                 -        小



                                                                           S + /0 +j24O
                                                                                                   -




where局 = 20 /                              and셔 = 20／쯔L It fo如ws that

           v。                                  伽sin 2仰］
                                     ［伽’
                   (t)
                                 :                                         u
                                                                               (t)
                                                                                         V.
Drill Exercise 17.3
        a) For the circuit shown, fmd the steady-state expression for vO when Vg = 10 cos 50,000t V.
        b) Replace the 50-kQ resistor with a variable resistor and compute the value of resistance
           necessary to cause vO to lead Vg by 120.

                                                                                                  10 kfl       10 kO




Solution
       a) First find the transfer function of the circuit. Let R1 represent the 10-kQ resistors, R2 the
50-kQ resistor, and C the 400-pF capacitor. Summing the currents away from the inverting input
terminal gives

          V1- v, V1 卞 VA
          =;,4 + ' r, V =0, or v。=2V1- Vf.
                   八1                          八1                                                          U


       Summing the currents away from the noninverting input terminal gives

         ！今                                                                                             烏C아食
         i; +(V2mVg) SC= O, or P2= (l; /?2E노）'
Part A: Representative Drill Exercises with Solutions                                            267




But V1 = V2 since the op 帥p is ideal; hence we can solve for the ratio VG/Vg. We get

         ！흐= H (s         '   ＝       下t2C노 1         中   .




          1舍            ' '           R2Cs + 1

For the given values of R2 and C we have




       To find the steady-state expression for vO first find H (j50,000); i.e.,


          H (j50,0凹）=，뉴 , 키1 = 1/     ./ 丁        I
                                                                  .

Now we can write down the steady-state expression for vO,

          vO = (10) (1) cos (50,0001 + 90') .


       b) Let R2 be a variable resistor and express H (s) as a function of R2; thus

          枷）= 凡帥 x 10 '2) s 小 I
                        凡 (400X
                                                  10Hl2）了 + I '
 and



           月
               (j50,
                   毗）
                                  ＝
                                      二： :’，岩｝
                                             二：
                                             ：
 Note from the transfer function that the angle of the denominator term is the negative of the
 numerator term. Therefore vO will lead Vg by 120" when

           響，世＝帥0 = 1.7321,

 or

           R2 = 28,867.51 c .
268                                                                Chapter 17/The Transfer Function



Drill Exercise 17.4
The numerical expression for a voltage transfer function is

                        V0=               .   32x.105
          H
              (5)
                    =
                                 ,:
                                      2
          4
                                                        , i。
                                                           ；·
              (s)
                    =
                         -
                             =
       a) Use a str小帥내ne ai叩litude p奴 to find the frequency where the ai叩血ude of H (泗）
          equals unity.
       b) What is the actual amplitude at the frequency found in part (a)?
       c) What is the peak a呻litu出 可H伽) in d凹小els?
       d) At what frequency does the output voltage reach its peak amplitude?
       e) If the amplitude of the source voltage is 10 V, what is the peak amplitude of the output
          voltage in V?


Solution

        a) First we write HOw) in the form convenient for making a Bode amplitude or phase angle
plot. Thus

                     5
          nUmJ = l 나2
                 1- u +j2tu

where u = w/800 and : = 0.25.
       The straight-line Bode amplitude diagram is constant at 20 log10 5 or 13.98 dB for w less than
800 rad/s, and then drops off at 40 dB/decade for w greater than 800 rad/s. The straight-line
amplitude plot will cross the zero-dB axis at 1800 rad/s.

       b) When w = 1800 rad/s, u is 2.25; therefore H (11800) = 1.1861／二프쏘笙 . The ai叩血ude in
decibels is 20 log10 1.1861, or 3.41.

       c) The peak amplitude of H如) in decibels is


         凡B伽毗）=13.98* 小岫小'(1刊｝
                        = 20.28 dB.
Part B: Representative Problems with Solutions                                                        269




       d) The frequency at which the peak occurs is

              蜘 = 口뇨 'I二石乎 = 800 V而云 = 748.33 rad/s

      e) Since 20 log10田伽) j= 20.28 we have log10田伽。          )I equal to 1.014 and therefore the
peak magnitude of H (j口）) is 10L014, or 10.328. When the amplitude of the input signal is 10 V, the
peak amplitude of the output voltage is 103.28 V.



Part B: Representative Problems with Solutions

Problem 17.1
The voltage source in the circuit in Example 17.1is changed to a unit impulse, that is Vg = 5(t).
       a) How much energy does the impulsive voltage source store in the capacitor?
       b) How much energy does it store in the inductor?
                                             (t).
       c) Use the transfer function to find v。
       d) Show that the response found in part (c) is identical with the response generated by first
          charging the capacitor to 1000 V and then releasing the charge to the circuit, as shown in
          figure A.




                                                               +
                                                               1000 V




        (a)
         a) After a source transformation the circuit appears as shown in figure B. The initial energy in
 the circuit is zero, hence the capacitor appears as a short circuit at t = 0 . Thus the impulsive current



                       5（亡）                                                 Ip. F

          (b)
270                                                                                                                                              Chapter 17/The Transfer Function



passes t뇨ough the capacitor. The voltage on the capacitor at t = 0 + iS
                                                                          + i/ . \

              『b(0+) = lOO片湍dt= 10(刃V.
                                                          .          ',




               v
The energy stored in the capacitor at t = 0 + is
                                              0                                0
                                                                                                    J
                      /1\
               w,t, ) =
                            +\
                                              l
                                             le2
                                                                               l
                                                                               氏
                                                                               J     6
                                                                                     H


                                                                                         =
                                                                                          (
                                                                                          )        le2



        b) Since the impulsive current passes through the capacitive branch there is no energy stored
in the inductor att = 0+.

             c) From Example 17.1the transfer function (VdVg) iS

                                     ,:          1000
                                                  +5
               壯                                      000,
                                                                          (s
                                                     25x1。
               H
                                 =
                                                                                             )
                                           s2 +6。
                                                。。r+
                     (s)
                                                                                                          6·
When vg(t) is a unit impulse, J舍 is 1.0 and therefore

               Vo = H (s)

                                            1000 (s + 5000)
                                 (s + 3000 - j4000) (s + 3000 + j4000) '

A partial-fraction expansion gives

                                                              K1
               V0 = (s + 羽00 - j4000) + (s + 3000 +j 40(Xi)

where K1 = 559.02 /                                                            . It follows that

               vO
                    ..
                    (t)
                                 =
                                     r. . . ,, n八 -30以y
                                     Ll.
                                            l.
                                                 l.
                                                      8
                                                              '03e
                                                                               如         cos
                                                                                                  . . 八八八』 八／ 尸n. .1 . . ,,
                                                                                                 (4000t
                                                                                                          小. 57 .'   )
                                                                                                                         ]   u
                                                                                                                                 (t)
                                                                                                                                       V.
       d) The s-domain equivalent circuit for the circuit shown in figure A is shown in fi암lre C.

                                                                                                                                            +1
       (c)
                                                                                                               T
Part B: Representative Problems with Solutions                                                                                                 271




The node-voltage equation that describes the circuit in figure C is

                       V0        V0
                                1。。。 l0 '
                 + 250
                   25。+ 。.。5s
                          05, 『
                              +l
                                                                                                     "
                                                                                          =
          工1J
          V0s*
                                            .
S아ving for 끼）yields

           . = - 1附）(s + 5000)
          L;
          vn=
          " U      2 . 』戶1\r뇨n . 八i= . . m1而 '
                  S 十 （乂人人is 十 乙；) X IU


This is identical to the expression obtained in part (c).


Problem 17.2
The input voltage in the circuit seen in the figure is

          까 = i0           [U   (t)   ' .       u   (t
                                                              -   0.       1)         ]       V.
Use the convolution integral to find vO.

                                                                                          4Q                 0.4H
                                                         eHH1尸a＼ 人V11YYY\
                                                                                                                                中         .
                                                                                                                                          +


                                                         '
                                                         V1                                                              1 F,             VO
                                                                                                                           l-
                                                                                                                    0.          1-   .,




                                                                                                                                I         1



Solution

In order to use the convolution integral we first find the impulse response of the circuit. The impulse
response can be found from the transfer function. The transfer function is


          月（s)＝속＝4*.然）(10幼
                                      25                                                      25
                                                                                                5)
                                      1뇨 +25
                                                                                                   2     '


                     s2+
                 H
                                                                                (s+
                                                                       e
272                                                                                                            Chapter 17/The Transfer Function



The impulse function is


          姻玎' k(s)] =25Ae"'iu(A).
The input voltage is a rectangular pulse with an 띠nplitude of 10 V and a width of 0.10 s. Thus in using
the convolution integral we break up the integration into two time intervals, namely 0 5 t 5 0.1 s and
0.1 S 드 r 5 m.
       In the first time interval we have


               V。
                        =   j4lO
                                                     [2ste
                                                                            ]   a




                                                                                            }
                                        L- sA                                       t

                    "25아들了（-5才－1) 0
                    = 10 - 10ee5' (5t + 1)                                                  05 t5 0.10.


In the second time interval we have


          vO
                    =       250f, 。1Ae'52d       －
                                        I                    -s4                        i
                                        i
                                                                   아十1)
                            4      戶八       -e
                                                                   /   戶1




                                                             25
                    =


                            z1u1



                    = 10e5(1 - 0.10)(5r + 0.5) - b0匕巾5' (5t + 1)                                          0.1드 t5m .


Problem 17.3
      a) Find the impulse response of the circuit in figure A (Part a) If Vg is the input signal and iO is
         the output signal.
      b) Given that Vg has the waveform shown in figure A (Part b), use the convolution integral to
         find iO.
      c) Does 4, have the same waveform as Vg? Why?
Part B: Representative Problems with Solutions                                                     273




                                                                         6fl   小- 1卜＝ 0




                                                                     0   0.5     1.0      f(s)



                                                                  -100


                                                            (b)

       (a)
Solution

       a) The resistance seen by the voltage source is 6 + 24, or 30 Q. Therefore the current out of
the positive terminal of the voltage source is VgI30. The output current I can be found using current
小vision; therefore




It f에O吼 that 川s) is a constant; i.e.,

                        -   .

             Il                                       UZ,
                                        '。
                  (S)           =   -        =   U.
and the impulse response is an impulse function, namely

             h(t) = 0.02 6(t) .
274                                                                                Chapter 17/The Transfer Function




  .   . b) In applying the convolution integral, visua也e rotating and s뇨fting the input signal Vg.
I neretore ior t < u, i1) is zero.
        For 0 < t < 0.5 s we have
                            +
             1。= f- 100 (0.02) cQ) d. = 2A.

For 0.5 < t < 1.0 we have
                                      +
             1O=        -   1-            100   (o.   02)   o   (A)   da=   -2A.
For 1.0 < t 5 00,
                            +

             b＝片0姻m =0A.
Thus iO has the waveform shown in figure B.




       (b)

        c) Yes, the purely resistive network has no memory. The absence of energy storage elements
means the currents and voltages in the circuit can respond instantaneously to any changes in the input
signal.


Problem 17.4
Given the following current transfer function:

             F뀨，   \＝       뇨                  106
               "                 'i       s2+ 400s+ 106 '
Part B: Representative Problems with Solutions                                                                                         275




       a) At what frequencies (in radians per second) is the ratio of 'O/li equal to unity?
      b) At what frequency is the ratio maximum?
      c) What is the ma姓mum value of the ratio?


Solution

       a) To find the frequencies when the ratio J/I is unity, we use the results obtained from an
analysis of Bode diagrams when H (s) contains complex poles. Therefore we begin by puttingH (jw) in
the form conducive to Bode analysis, as follows:




         ""' " "[(i．崗：j0.4（崗］'
where: = 0.2 and w, == 1000 rad/s.

，啣忠'黑瑞：
      ::：쌌湍黑絮齬，‘er1쁜乷：黑胃忿'如""'"" '""
b,     b) The ratio s max
                       ,i                imum
                                                when the dB amplitude                  is
                                                                                            maximum. This occurs at w, ,   which
                                                                                                                                   is given
by the expressi。n w,                 -




       Thus

          Wp = 10刃 VI - 0.08 = 959.17 rad/s.


       c) The peak amplitude in decibels is


          AdB   (WP)        =   -
                                     10 log10
                                                 [叱2
                                                        (1
                                                                   -
                                                                             C2)   ]
                            =   --   10 log10    [0.
                                                       16    (0.       %)]
                            = 8.14dB.

An amplitude of 8.14 decibels corresponds to a ratio of 2.55. Therefore the maximum ratio of!O!!, is
2.55.
276                                                                  Chapter 17/The Transfer Function



Part C: Supplementary Problems

Supplementary Problem 17.1
The s찌itch in the circuit shown in the figure moves from position a to position b at t = 0. Use the
principle of superposition to find v。(t) for t > 0.




                          30 V
                                                                                  2N




Supplementary Problem 17.2
There is no energy stored in the circuit in the figure at the time the switch is closed. The sinusoidal
voltage source is generating the signal 1000 cos 1어刃 V弧 V. The response signal is the voltage v。     .
       a) Find the transfer function Vo/Vg.
       b) Find J/。(s).
       c) Describe the nature of the transient component of v。
                                                             (t) without solving for v。
                                                                                      (t).
       d) Describe the nature of the steady-state component of v。
                                                                (t) without solving for v。
                                                                                         (t).
       e) Verify the observations made in parts (c) and (d) by finding v。
                                                                        (t).
Part C: Supplementary Problems                                                                       277




Supplementary Problem 17.3
       a) Find the transfer function V/Vg as a function of k for the circuit in the figure.
       b) Find the largest value of k that will produce a bounded output signal for a bounded input
          signal.
       c) Find vO(t) fork = 0, 20, 40, 50, and 80 if vg(t) = 10뇨(t) V.




Supplementary Problem 17.4
Use the convolution integral to evaluatey(t) at 3, 6, 9, 12, 15, and 18 s if

          y(t) = 力（t) 卞 工（t) = 工（t) 卞 /i(t)

and h(t) andx(t) have the waveforms shown in the figure.




Supplementary Problem 17.5
       a) Use the convolution integral to findy(t) if h(t) and x(t) have the waveform shown in the
          figure.
       b) Sketch the waveform of y(t) for -5 5 r 5 20 s.
278                                                                   Chapter 17/The Transfer Function




                             h노x(t)
                               (s):h t(s)
Supplementary Problem 17.6
The transfer function for a linear time-invariant circuit is



          H(s）수나茗．빠，00·
If ii(t) = 4 cos (50 + 60O), what is the steady-state expression for v。
                                                                      (t)?


S마叩佃nentary I노야)lem 17.7
The operational amplifier in the circuit in the figure is ideal and operating within its linear region.
       a) Calculate the transfer function VO/V5.
       b) If v = 1.25 cos 200t V, what is the steady-state expression for v。
                                                                           ?


                                                         500 kfl
Part C: Supplementary Problems                                                   279




Supplementary Problem 17.8
The o壯ational amplifier in the circ吐 in the figure is ideal.
       a) Find the transfer function Vo/Vg.
       b) Find v。江Vg = 1山（i) \／·
       c) If Vg = Vm cos t V, how large can Vm be before the op amp saturates?




                              in            2fl




                         vg




                         V          T'   "                TIF
Supplementary Problem 17.9
The unit step response of a circuit is known to be

          vO = 50e   0' Xi sin 40,000t V.


       a) What is the transfer function of the circuit?
       b) What is the impulse response of the circuit?
       c) If the input sinusoidal voltage source is


          Vg = 5 COS (40,0001 + 少) mV,

what is the steady-state expression for vO?
                                                                                    Chapter 18
                                                                                   Fourier Series


Part A: Representative Drill Exercises with Solutions

Drill Exercise 18.1
Derive the expressions for ay, ak, and bk for the periodic voltage function shown if Vm = 607r V.

                                                            v(t)

                                                            Vm
                                                  Vm/            2



                                                                                                 I           1               I             I    I    I   r
                                                                                               刃4            刀2          3刃4               T   5刀4


Solution

For the given periodic function, the expressions for ay, ak, and bk are found from the defining
equations (19.3), (19.4), and (19.5). In using these relationships note that the optimum choice for t0 is
zero and that the integration over one period must be broken into the intervals 0 to T/4 and T/4 to T.
The expressions are

                         l
                         eT                                               lT
                                      L
                                                                                   Tm
                                                  꺄                                                          m                                                     +
                                                                                                     드
              따                 n1J   m0     戶m                             n11J

                                                                                                     2
                                ,       八m    尸         ，

               = ;; Vm = iI. )J( V,
                    5.
                 0


          ,         21                T14                                                                T              Vm
          ak   =-
                         ;1f。                /\..5
                                             Vmcos               (,
                                                                 (kwot)    0/      )*J
                                                                                               +fT
                                                                                                                  -j-        cos   (kwc)       dt}


                  Vm    . kr   30 .
               = =1二；sin       == sin
                 凡口'0 '   二4
                           乙 = 人                                                         （弩）             ,



and

                                                                                                                                                             281
282                                                                                                                      Chapter 18/ 고ourier Series




                                               T/4
          bk=                                            Vmsifl                         dt+ T14     sin
          小2                                                                                   IT
                                                                                                                   dt}
                                    1f。
                                                                         (kwot)
                                                                                                          (kwOt)
                                          1J
                                                                                                          佃나나＼
                              Vm L                                       /k7r\ ]                    毗
                                                                                           型
                                                     =

                 키I- """ （了) ]
               ＝而；
                                                     1




                                                                                           k
Drill Exercise 18.2
Derive the Fourier series for the following periodic voltage.




Solution

In studying the given periodic function, note that it is odd and has both half- and quarter-wave
symmetry. Therefore ay is zero and ak is zero for all k. We also know that bk is zero for even values of
k. For odd values of k we have

               까
               =       T O 4 f(t)
                       8      fT/                              sin   tkw/) dt.


        The integration called for in the expression for bk must be broken into two intervals, one from
0 to T/6 and then from T/6 to T/4. For 0 5 t 5 T16 the expression for Vg is

                                          r
                   四
          Vg       j                t            O 5t 5T/6.
                   T
For T/6 5 t 5 T/4, Vg is a constant equal to 1뇨j We have then that



             (TI" 牛如t) di +片加小岫*}
          .，궈JO
                       12Vm .                            (kr\                     . .     ..
               =       k2兀2                    " "       （了)         ,            k " " dd      '
Part A: Representative Drill Exercises with Solutions                                                     283




The Fourier series for V (t) is

                                的
             vJt' = 쁘뇨                   1
                                2
                                                                .        ,   ..   ,   ,
                                               .
                                                   rri7r\
             ’占V/        2               三 Sm '三기 Sm W따刃 V.
                    Jr                   ,2            \ =r /
                             n = 1, 35


Drill Exercise 18.3
The trapezoidal voltage function in Dri끄 Exercise 18.2 is applied to the circuit shown in figure A. If
l2Vm = 986.96 Vand T = 6283.19 ms, estimate the average power delivered to the 1-Q resistor.




                                                                                                    111




       (a)
Solution

To estimate the average power delivered to the i-c resistor, calculate the rms value of each harmonic
voltage across the resistor. The average power for each harmonic voltage is the rms value of the
voltage squared divided by 1 c. The total average power is obtained by adding the powers associated
with each harmonic voltage.
       To fmd a harmonic voltage across the 1-Q resistor we first find the transfer function 1乙？/1乙
wnere yR is me voirage across rue resistor. I ne s-aomain circuit is snown in ligure li .

                                               S



                             呻
                                                                         ,

                                              ／扮了1
                                                                    J.
                                                                                          4-
                                                                                               ＼七
       (b)

       Summing the currents away from node 1 gives



             如，牛* 쏙뇨0.
284                                                                              Chapter 18/Fourier Series




S아毗rig for Vj亡 gives


           VR-
           yk-
                        ,2S +s+           1

Hence


           Hi.c\ =！느                                1
          1= \m/              V_           2 . .
                              ' S         S 十S 十 上


The value of H (s) as a function of the kth harmonic is


          H (j
                 (jkw0)
                                              ,,1
                                          -
                         ):
                  "0.               (,
                                               2 2
                                                  )
          H
                               =
                                    (1-       k w。        +jkv。
But u。is (2兀 x 103/6283.19) or 1rad/s. Therefore


          H (jkcv。
                 ) = H (jk) =                                l,    .
                                                        (1- k) + 恥

        From the solution to Drill Exercise 18.3, the Fourier series for Vg is

           Vg =86.6051flt - 3.46s1n51 + 1.77sin7t +' "

        From the transfer function,

          H（月） = 1／二四


          H (j5) = 40.79 x 10已- 1堅끄으，

and


          H (j7) = 20.62 x i0                            / _171.700.

        Now write the corresponding terms in the Fourier series of the voltage across the resistor:

           yR = 86.60 sin (t - 900) - 0.141 sin (51 - 168.23) + 0.036 sin (71 - 171.70) +' "
Part A: Representative Drill Exercises with Solutions                                                                       285



        At this point observe that the amplitudes of the harmonic voltages are very small compared to
the fundamental. Since the average power is proportional to the square of the amplitude of the
voltage across the resistor notice that a good estimate of the average power delivered to the 1-O
resistor can be obtained from the fundamental component of yR. Thus


            尸＝堡竺끄／'/乙三斗3750 W.
                         I


Drill Exercise 18.4
         a) Calculate the mnean-square error if the periodic current in Example 18.2 is approximated by
            the first term in its Fourier series and 'm = 10 A.
        b) Repeat part (a), given that the periodic current is approximated by 10 sin 口J0t. (Hint:
            Observe that because of symmetry the computation of구 can be made by integrating from 0
            to T/4 and then 小vid旽 this res山 by T/4.


Solution

         a) Take advantage of symmetry to find the mean square error. The interval of integration can
be chanced to 0 to T/4 orovided the result of the integration is divided by T14. From Examnle 18.2 the
lirst term in the l ourier series representation Ott is L?iImIJrI
1크4a 1八미44 :-4 114 ,. n ', . . m: nm n 八－': 八n 山UH八m八41.,1: 八－1 八r .· :n r (} r
                                                                                    Sin (W(,t). In the interval O1 U 5 t 5 1114
                                                                                口2] n!H ／』. 4\ !4 114 n 느1h小m1 hr il ；戶 i / m／月


the expression for i is 回, I기t. It follows that the error function in this interval is

              ..     4'm       8'm . .         .
            以t) =    =;；나 H H;        없fl (O)（刃·
                                7re



The error function squared becomes

              2... 16／立 . 64J且 , . . ,. . 64J丘． . ..
            E ( (J = 1H[          =1      i Sl1l [ 0갸Y J 十 H            Sl1l 1 nnV ) 1
                      거n二           二r月r1         \ 1J /            4        \ 11 /
                      I           )T I                         7r

By definition the mean-square error is



          「나1T/J。4"""지｝려！"·"""
286                                                                             Chapter 18/Fourier Series




       b) If the periodic function is approximated by 10 sin o0t then the error function in the interval
0 5 t 5 T/4 is


                             砥T
                   蛔                       =
                             1
                                 r- /77i 前n (（呵）.


It follows that


          \
          0E
                             l
                                  거
                                  M r 4)
                                       q
                                                         )
                                                   區
                                           r
                                                 ＝努鈿 (wot) ＋耶in느町）,
               ）
                                             ）
               日
                             e
                                             日
                                                        =

                                                   T
and the mean-square error is


          石＝亭f"4e2(t)d'지긍긔                                       = 2.2764 A2.




Part B: Representative Problems with Solutions

Problem 18.1
Derive the Fourier series for the periodic voltage shown in the figure, given that


           「   （   ()   :   lm9i.          푸t,              05 t5 T/2;


         「（()＝印Si.푸나）                                       T/2 5 t < T.


                            v(t) (V)

                                 100

                                 80
Part B: Representative Problems with Solutions                                                                                        287




Solution
Observe that v(f) can be thoug뇨 of as the sum of two ha正wave rectified sine functions. Thus we can
describe v(t) over one period as

           v(t) = v1(t) + v2(t),

where

                 ..                 .         f2兀 \                     .            e．'
           v1   (t)       =   100sin          (;            9,          0         t5T/ 2;

           v1(t) =0,                    T/2 5t 5T;


           v2(t) = 0,                   0 5 t 드 T/2;

and

            , ..
           V-,(t) = 0(J sin I - =
                                   . 127r
                                                       (t
                                                                   T\1
                                                                 _:_I I,
                                                                                    m.4
                                                                                    ifZ 5t 5i.
                                                                                                  m
                      "        '         Li                        乙／J

       Use the Fourier series for the half-wave rectified sine function tabulated on the end pages of
the textbook. Thus


        「仰戶響구知（岫． 7r
                                                                                          的                   .




                                                                            르쁘            夕       COS (flWt)
                                                                                      1'           nl2 H ]\ '
                                                                                    n= 2, 4, 6,    V'    -/


      The Fourier series for v2(t) can be derived by simply shifting the Fourier series 曾ven on the
end pages by 刃2 units to 由釘뇹ht. Thus

                              쁘兀        旦2             尸
                                                       hL                                          mq
                                                                                                    口
                                                                                                                                                )
                                                                            7尸2
                                                                                                                                            =




                                                                                                             cos [nwo(t - T/2)]                  +
                                                                              \
           V                                  S                  r 1\
                                                                                          塑
                      n
                                                   1
                                                                                                                                                )=
                                                                                                                                                4   H
                                                                                                                                                    e



                                                                 加
            ）
                                                                              1
                                                   n
            느
                      \
                                                                                          兀
                                                                                              n = 2, 4, 6,
                                                                              J                                                             ]
                                                                                                                                  '
                                                                              /
                                                                                                                  (n2   U   k)
        Next, simplify the series for v2(t) by using the following trigonometric relationships:

           sin [nJ0(r - T/2')] = sin (wot 中 7工） = -sin wj,

and

           cos nw0(t - T/2) = cos (nwot - nJr) = cos n7r cos nw0t.
288                                                                                     Chapter 18/Fourier Series



      The cos n7r is always unity since n is an even integer in the summation term. Therefore we have

             02
             V         쁘兀    )4』
                               1 .           120       mq口        cos nw0t
                            e 未) Sin W0t
                            =
                                           - 二mV                  r                 '

                                                                  (7i       == 1)
                                                                        2
                                                   n == 긱 4厄


       Adding v1(t) and v2(t) gives the Fourier series for v(t); thus

             岫              + 20 sin w。t-3罕             m q口
                   塑
                                               =
                   兀
                                                   n = 2, 4, 6,



Problem 18.2
The periodic function shown in figure A is even and has both half-wave and quarter-wave symmetry.
      a) Sketch one full cycle of the function over the interval - T/4 5 t 5 3T/4.
      b) Derive the expression of the Fourier coefficients ak.
      c) Write the first three nonzero terms in the Fourier expansion off(t).
      d) Use the first three nonzero terms to estimatef(T/8).




       (a)
Solution

       a) Figure B is a sketch of one cycle off(t).
Part B: Representative Problems with Solutions                                                         289




        (b)

      b) Because the periodic function is even and has both half-wave and quarter-wave s戶llmetry
we know that bk is zero for all k; aV = 0; and ak is zero for even values of k. For odd values of k we
have


          .,：引伊
              l v
                  固*
                  \i
                     n,/ 邸（kw/) dt日刀， :1큭의* 4)/ c。s(kw。t)dtj.J
                                    J iO \ 1

        In studying the expression for aj, note that the integrals are consistent with the fact that

                                               \        0 5 t 5 T/8,
          J(t) = （了 t + 1)
               .        .       (8         .




and



              /(   ()       =   （半    「4)
                                     （·                       刃85               (< 기4.

        The expression for ak can be 꽈ritten as the sum of four integrals; i.e.,

              口k = '1 + '2 + 13 + 14,
where

                   64 r T/8 ,   /27rk \ .
              '1 = -:;i' U (Cos t -=--ti at.
                   T                                                        "




                                     少
                                                   "I               )
               b                흐T            (27rk .\ ,.
                                          Cos I- =-rI 口1.
                                              \ 1         )             "
290                                                                                                   Chapter 18/Fourier Series




           b      H
                       塑尸    戶1J
                                   m跳   t cos（뿌如，
and

           n      翌T  n11V   恥m
                                       /27rk \ .
                                   cos 1 - -ti at.
                                        \ 1 )
Carrying out the integrations yields

                                                              16          . 4
                                                             =1== 十 1=m Sin
                                                             mr白. 乙
                                                             It, !,
                                                                           兀k
                                                                                （쒸，
                                                              32                       .

                                                                      cos       十 H=1 sin
                                                                                   8
                                                                                  兀k
                                                         -     --


                                                                                                  ,
                                                         21k
                                                                                            （警）
and

           ,   16 .            (兀k\
          14 "i Sifl （了) -；瓦 " "
                                             16 .
                                                              （쒸·
It follows that


          따＝돐卜미쒸긔，k = 1,3,5,·
                      It, 凡        L         \       /               -J




        c) From the equation derived in part (b),


           a1＝푤，[3 cos（升中1.82,
           幻＝듣卜미쮜 긔 !-0.56,
                       I1I         L     "       '                  .i
Part B: Representative Problems with Solutions                                                       291



and


          .，근，늬3미퓌 긔 :-0.20,
                  乙그兀     L           \   ' /        -j


The Fourier series forf(t) is

          f (t) = 1.82cosw0t- O.56cos3w0t- O.20cos5w01+ - · ·

       d) Using the first t뇨ee terms of the Fourier series we have

          . . n,.,,.     . n八         /7r\         n ,,         (37r\       八4八   /5兀＼
          八．
           T/8) 斗‘．.82「”' (i尸0.56 ""'（히- 0.四cos（히
                       之 1.83


Problem 18.3
The peri어ic voltage shown in figure (a) is applied to the circuit sho吼 in fi昏lre (b). Derive the first
four nonzero terms in the Fourier series representation of the steady-state output voltage vO.


                                          vg (V)


                                           30ir




                                                                        2



                                                   寸30w



                                                      100 k[l
                                (0)
                                (b)
292                                                                                                  Chapter 18/Fourier Series



Solution

We begin by finding the Fourier series representation of vg(t). Because the function is odd we know
that ay = 0 and ak = 0 for all k. The expression for bk is

                                                         m0
                                 4
                                                          -3
                                 r            戶11V               30兀 sin (kwot) dt
                                                                         =
              1
                  1              H
              D
                  K
                                     쁘
                                                                                =

                                     k
From the expression forbkwe haveb1 = 60V, b2 = 60V, b3 = 20V, b4 = 0, andb5 = 12V.
Therefore the first four nonvanishing terms in the Fourier series representation of the input voltage
are

          Vg(t) = 60 cos (w0t) + 60 cos (2w伊) + 20 cos (3w01) + 12 cos (5w0t) +' "

where a幻 = 500兀 rad/s.
        Next, derive the transfer function 1'0/V5. The s-domain node-voltage equation for the circuit in
the figure is

                            V0            .          + VOH    +2。 1。9
                                                                    Ji   .           _   v, =   。.
          25x103                                      100x10J

From this node-voltage equation, it follows that

          - -. .   V。     500
         Il      =   = s + 2500
                      (S)                i}
Thus


          H           (j，帥）                          =         2500器00,rk·

Now evaluate H (jkw0) at the first four nonvanishing frequencies:

          H (jwo) = 0.17/ -32.14,

          H (j2w0) = 0.12／二흐1竺尤


          H (j3w0) = 0.09／二二흐2.C匡，
Part B: Representative Problems with Solutions                                                       293



and

          H（戶如）= 0.06 느：72코쏘 .

Now we can evaluate the Fourier series for vO(t). We get

          vO = 10.16 sin (w0t - 32.14') + 7.47 sin (2w0t - 51.49') + 1.87 sin (3w0t - 62.05")
                + 0.73 sin (5cv( ( - 72.34') +' "


Problem 18.4
The Fourier coefficients for the periodic voltage shown in the figure are

                 Vm
          口V =   了;
                                             竺r
          따＝哲外如朴畔,
                 71 凡     \     e /      =
                                                     allk;
          .      4F今1 /.       幻r\
                                                     all k.
          Dk = : 2, 2
                 Jt, 入r   \
                              了卜  /




       a) Given Vm = 244.95 V, find the rms value of Vg.
       b) Using the first three nonzero terms of its Fourier series, estimate the rms value of Vg.




Solution

      a) The area under the squared voltage function for one period can be found by integrating the
squared voltage from 0 to T/4 and then multiplying by 2. Thus
294                                                                                              Chapter 18/Fourier Series




         月，弘＝2J:'" '喀'dt =字．
 .,      ..    4Vm
        （
ivote: v뇽 () = 二戶L              0 5 t 5 T/4.] It follows that the rms value of vg(t) iS

                                      l
                                            丘
         ，呻，
          ufl'
               = ［三
                 LT
                    回2
                    6 ]

For the given value of Vm,

          Vrms 立 100V.

       b) From the given expressions for the Fourier coefficients,

          aV = 61.2375,


          a1 = 0,


         口2 勺 -49.6372,


          b1 斗 99.2745,


          b2 = 0.

Therefore

                                                                                             l
                                                             2                               2
                                 2375)2 +             2745
                                                                 十2          6372
                                                                                    21
                        L(61.                                                            j
                                                                                )
                                                         )
                                                  .                   (49.
                                            (99
            Vrms
                    :   1
                            "




                    쌉 99.55 \/.


Problem 18.5
Assume the periodic function described in Problem 18.2 is a current with a peak amplitude of 2 A.
       a) Find the rms value of the current.
Part B: Representative Problems with Solutions                                                        295



       b) If this current exists in 54-Q resistor, what is the average power 小ssipated in the resistor?
       c) What percentage of the total power 小ssipated in the resistor is associated with the
          fundamental component of i?


Solution
       a) The area under i2(t) for 0 5 t 드 T/8

               -
                             H.4 n . 2 . .ltY
                       r1/8 It3I(
                                            , . J11 .                                ,,,,,
                                     口：可十下十 II 口(＝玉'
                                                  II
          A1 =J0
                                     L'      J
The area under 12(1) for T/8 5 t 5 T/4 is

                                            2

                                                                            ]
                                 4                  128t                                 4T
                                     F25&
           .           rT/
                                                               '   ,   ,]        .




          A2       =
                       J T/8         ［二二＝
                                                           "           "        "'       24

The area under i2(t) for 0 5 t 5 T/4 is

                                            liT
          A = A1 + 月2 :=
                                             24 '

The mean value of i2(t) is therefore


         而＝雨푸
and the rms value is



         'rms=               f
                                            l35A

      b) The average power dissipated in the 54-Q resistor is

         =1    .2   -.   :11
         // = 1;시mt >4 = =＝中 (54) = 99W.
                          b


      c) The rms value of the fundamental component of i (t) is


         'rms1＝솥円(3cos45'- 1)1 ! i.29A.
                             V 乙 1 7[                                       1
296                                                                                                  Chapter 18/Fourier Series




The power associated with the fundamental component is (1.29)2(54) or appro血lately 89.22W. This
is (89.22/99)(100) or 90.12% of the total power dissipated.


Problem 18.6
A periodic function is represented by a Fourier series that has a fmite number of terms. The
amplitude and phase spectra are shown in figure A parts (a) and (b), respectively.

            a) Write the expression for the periodic current u鈿g the form given by Eq. (18.38).
            b) Is the current an even or odd function of t?
            c) Does the current have half-wave s戶nmetry?
            d) Calculate the rms value of the current in miffiamperes.
            e) Write the exponential form of the Fourier series.
            0 Make the amplitude- and phase-spectra plots on the basis of the exponential series.


                                              月, (mA)




                                                              1
                                                              툴
                                                              i
                                                                  而으




                                                                       小8N二 1
                                                              l
                                                              /
                                                                       5        而나 1 7      krad/s
                                                              ]

                                        (a)
                                                 卞   8,   ,




                                                                       11
                                                     90口



                                                                       5
                                                                                         kradls
                                                                  1
                                                                  3             7




      (a)
Part B: Representative Problems with Solutions                                                                297




Solution

       a) From Eq. (18.38),


            i (t) = ay +                     2 An cos (nw0t - 0) .
                                             n= 1

Using the values given in figure A gives

            {iy = 0,


            A1= 441,                                    e1                =90";


            A3= 49,                                     03                = e900;


            A5 = 17.64,                                 e5                = 900;

and

            A7= 9,                                      97                = e 900.

The expression for 1(t) is

            1(t) = 441 cos (w伊 - 90') + 49 cos (3w01 + 90) + 17.64 cos (5w0t - 90)
                   + 9 cos (7w(t - 90")


                             = 441 sin 10001 - 49 sin 30001 + 17.64 sin 50001 - 9 sin 7000t mA.


       b) The function is odd because i (- t) = -i (t).

       c) Yes, because bk is zero when k is even.

       d)

                                                                                                          l
                                              2      9)2                           2                      "
                                                  + 4                      7.64        +
                                                                                           (9)   21
                                                                               )
                                     (441)
                                 L                                                                    ]
            /m           ,   =   1                  (        -       (1
                 "   "   "                                       2

                             = 314.07 mA
298                                                                       Chapter 18/Fourier Series



       e) From the definition of C we have
                   q=
           q               力            = 血 d9. .
                 lH 2  1
                                n
                                          2   느HmH




Using the values given in figure A we have

          -     441                         .      .
          Ul   == /                     = -j22u.> mA,
                   乙




          C_1 = j220.5 m八


          C3 ：孚쁘＝j24鈿A,
          C_3 = -j24.5 mA.

                               _900: -j8.82 mA,
          Cs :1誓4/
          C巧 =j8.親m八


                  9U 2
           q               쁘
                                            mA,                                       =
                                        <
                                    d
                                        1
                                                                                      =
                                    1
                                        口
and

          C_7 = -j4.5 mA.

The exponential form of the series is

          i =1220.5e1(0' -j2邪e加 ' +j24.5e -j知0t         J24.5e)鈿Ot +j8.82e -j&00t         .8.82ej50t

               -j4.5e -j7w0t +14.5e17W0t mA.

       f) The amplitude and phase plots are shown in figures B and C, respectively.
Part C: Supplementary Problems                                                                      299




                                                   /d시

                                      r
                                          "        "初




                                                   似7




                                나5-   中3            ＝戶 / 0           1
                      -
                            7
       (b)
                                              日7
                                                         勿
                                                             '




                                                                 I           5-
                :：乙1寸小十
                                 -3
                                                                         3        7
                          -5-
                                          m兄7.

       （이



Part C: Supplementary Problems

 Supplementary Problem 18.1
 The perio玉c square-wave voltage in figure (a) is applied to the circuit shown in figure (b). Derive the
 first four nonzero terms in the Fourier series that represents the steady-state current.
      300                                                                         Chapter 18/Fourier Series




                                 v9 (V)

                                 1057T
                                   4

                                                     /1S                             0.0159 /1F
                                     0    50   100
                                }057r .
                                  4
                        (a)                                Ib)




Supplementary Problem 18.2
The periodic triangular waveform shown in figure (a) is applied to the bridge circuit shown in figure
(b)
        .




            a) Determine the first three nonzero terms in the Fourier series representation of vO.
            b) If the bridge circuit is regarded as a filter, what frequency component present in the input
               voltage is eliminated from the output voltage?




                                                                 S




                          (a)
                                                                     (b)




Supplementary Problem 183
The periodic sawtooth voltage shown in figure (a) is applied to the circuit shown in figure (b). Derive
the first four nonzero terms in the Fourier series representation of the steady-state output voltage vO.
Part C: Supplementary Problems                                                                         301




                                            S
                                   0.02
                                                (b)



Supplementary Problem 18.4
The Fourier series for the triangular current shown in the figure is


          i (t) =5兀- 10      2       -1 s蜘100rt.
                            n= 1


       a) Estimate the rms value of i using the first four terms of the Fourier series.
       b) Repeat part (a) using the first six terms.
       c) Repeat part (a) using the first eight terms.
       d) Calculate the true rms value of i.




                                                                             ms




 Supplementary Problem 18.5
 The square-wave voltage shown in figure (a) is applied to the circuit shown in figure (b). Find the
 average power associated with the fifth harmonic of the source voltage.
302                                                                                Chapter 18/Fourier Series




                      v9 (V)
                       50ir

                                             ms                                    200 n
                                 ,r/2   if




                                                  (b)




Supplementary Problem 18.6
The periodic current source in the circuit shown in figure (a) has the waveform shown in figure (b). If
the period of i is 628.3185 ps, estimate the average power delivered to the 5-kQ resistor.



                                                                       (A)
                                                                       -     。.2
                                                                             刃8
                                5kfli        25mH
                                                                  H 刀8                T

                                                                       0.2r
                                                                 )b)
                                   Chapter 19
                              The Fourier Transform


Part A: Representative Drill Exercises with Solutions

Drill Exercise 19.1
The Fourier transform off(t) is given by the following expressions:

         F(w) = Qrco 5 co < -2;

         F(w) = 2,-2 <w < -1;

          只이 = 1! 尸1 < a) < 1;

         F(w) =2,       1< w< 2;

         F(w) =O,      2< w 5oo.


Solution
A sketch of F(w) is shown in the figure. Using the inversion integral given in Eq. (19.9) yields
                                         F?kJ7 '




                                            Z

                              中그
                                           工


                                                                                 口그




          f(r) 금仁戶"' 加* J!, 1e"' 伽『f：勿itwd『}

                                                                                                   303
 304                                                                                                Chapter 19/The Fourier Transform




                                                                      押了
                                                                                                }
                                                             l             l                2
                   ＝그_ .1可으
               寸
                                                                                        止
                            +
                                  2兀 [ it                    )
                                                             e                 +l
                                                                                            1
               e
                                                                           H        戶
                   乙듦{2(.e -it .6
                   = ------    -e -j2 )+
                                     ）『（6eit -e
                                             -.-ft*
                                                 )+2(e
                                                    2(6J2
                                                       "--e6it)J



Drill Exercise 19.2
Given thatf(t) is a real, odd function oft, show that the inversion integral reduces to


          f(t) = -                         f! , B(w) sinwtdw.

Solution

Drill Exercise 19.5 shows that whenf(t) is real the inversion integral reduces to


          f(t) =굶f!, [A(co) coswt- B(w) sinwt] dw.
Given thatf(t) is a real, odd function oft then by hypothesisf(t) = -f( -t). From the result obtain
from Drill Exercise 19.5


         ．小）＝打！, 卜A(w) cos cot - B(co) sin cot]dco.
Butf(t) can equal -f (나) only if the integral

          f        A
                           (co)
                                           coswtdw =             0.
It f에ows then that if只t) is a re毗 odd fu耐油 oft, the mnyers油 integral beco毗S

           m                      1
                       -r--J                    li (w) sintcoaw.
                       -
                                      ,.
                                                =.   .   .   .         .




                       乙兀 !                e的      \     /
Part A: Representative Drill Exercises with Solutions                                                  305




Drill Exercise 193
The voltage source in the circuit shown is generating the voltage

                                             V.
            Vg = e'u(- t) + u(t)

          a) Use the Fourier transform method to find Va.
          b) Compute v口(0) , va(0+), and va(ci).

                                                               1 fl




Solution
          a) To find Va, first find the Fourier transform of the voltage source Vg. The Fourier transform
of v뇽is

                               1
                                                       l
             노＝
                          (,
                                jw
                                     ) +i6   (w)
                                                   +
                          (l
                                                           石
Next find the s-domain transfer function Va/J슝 for the circuit in Drill Exercise 19.10. The s-domain
node-voltage equation that is generated by summing the currents away from the upper terminal of the
o.5- 2 resistor is


             노쓰근 뇨V,,s=
                     H
                        0.
              I U. >


 From this equation we find

                   .. .        1a      1
                  /i (S ) = =m = 十．
                     "      Vg   S+ 3


 Therefore

                  W( i,,\ =
                                   1
                  "\ J' 1        3 ＋加 '
 306                                                                                                                                                   Chapter 19/The Fourier Transform



 From Eq. (19.55) the Fourier transform of V。
                                            (w) is as follows:


           乙（0)                 =
                                         (,
                                                    .
                                                        j.
                                                               )1
                                                                    (.
                                                                               *j.         ）『j
                                                                                                       ,    (3
                                                                                                                      1j.        ）『궁
                                                                                                                                                  三)
                                                                                                                                                   ·




 The first two terms on the right-hand side of the expression can be expressed in terms of partial
 fractions. Hence

                                  (
                Va(w)=（此) +(요知쀼 (3玘 ，+ .7V
                                      (3貂
or


          乙回＝（心뇨*쁩 (3(1/+：介詐名·
The time-domain expression for va(t) is found by inverse transforming the first three terms by
inspection and using the inversion integral to evaluate the fourth term. This yields

                                                                                                                                             V
                                         '.                    +U                                                      u               +   l小 6
                                                                                     （r)
                                                                                                 m
                                                                                                                 -갚
           ,h
                (r)
                           :=       }e
                                                                                                       1e
                                                                                                                           (t)
                                    斗
                                              （나）
                                                                         }：恥
                                                                                                      l乙




       b) Using the expression derived in part (a) yields

                                                         l16                     lH 6
                    1                                                    0                             V
                .     八-


          Va(tJ ) ==7 m
                           .


                                                                                                     lH 4                                                               +=
                                         1f


                                                                            V
                                                        l
                                                        H6
                                                                           1
                                                                           l 4
          va(0+) = 0 +                                                     H
                                                                           l
                                                                           l五
                                                                             6                                                                                                  +=


and


                                                        lH 6
                                                                                                   V
                                                                                lH 6
                                                                    0
          乙佃）= 0 +                                                                               lH 3                                                                                     =




Note that va(0 +) = va(0m) as it should because there is no impulsive current in the capacitor. Also
observe from the circuit that at t = m the value of Va must be (0.5/1.5)vg or (i/3)vg. Since Vg = 1 V at
t = 00, it follows that V口 = (i/3)V at I = m.
Part A: Representative Drill Exercises with Solutions                                                                                             307




Drill Exercise 19.4
Assume that the magnitude of the Fourier transform of v(t) is as shown. Given that this voltage is
applied to a 6-kQ resistor, calc岫te the total ener町 delivered to the resi如r.

                                                                                                            1V(/w)I (V- s)
                                                                                                                 6




                                                                                                                                      c (rad/s)
                                                                                                        2000町    0           2000,T


Solution
First note from the figure that V(jw)1 is an even function of叫 therefore in appl艸g Parseval's
theorem we use the form of the integral given in Eq. (19.63); i.e.,

            .   ,




           w1w = ;iJ0
                                        1
                                                .
                                                    oo
                                                                    1y
                                                                                  (m)
                                                                                                1 dm·
                                                                                                '



It follows from the figure that

                    .    .    .                         -                (
                                                                                            6
                                                                                                    \       O 5w 52C以材，
           'V（叫1                            =
                                                    0
                                                            "   '        (2仄Xh尸
and


           Iv
                        (w)
                                  H0,
                                                                                        2000r5w5的.
Thus

                                                li
                                                                         們
                                                                                        卜d侃）" 냐，너"]dw
                                                                                                                                                        =
           W1(,)


                                  = 24kJ.

 Since the voltage is applied to a 6-kQ resistor the total energy delivered is



           W6kQ=
           m*
                 x。。
             中246。 "'                                           J                       =
                                                                                                4J.
308                                                                                     Chapter 19/The Fourier Transform



Part B: Representative Problems with Solutions

Problem 19.1
Use the de＆的rig integral to f뇨dii妃 Fouri아 transform of the fo끄O岫ig fu耐ions:

             a)       f(t)   =Asin               t,                -2 5 t 5 2,

                      f (t) =0;                                毗妃＼where;

                                                                          I
       b）只卜쭈H及                                                            三5t
                                                                              5 U,
                                                                                  -




                  f(t) =2尹f +A,                                           0 5 t 5 r／긱

                  f (t) = 0,                                   elsewhere.


Solution

       a) Figure A is a sketch off(t).




       (a)
       The Fourier transform off(t) is


                  徊= ［」S唯小"wtdt·
Using entry number 5 in the Abbreviated Table of Integrals in Appendix D of the te址book to
evaluate this integral yields

                  F   (w)            =     可航d        ,   sin2w.

                                         (2rH - 4w)
Part B: Representative Problems with Solutions                                 309




         b) Figure B is a sketch off(t).


                                                                   和f)
                                                                         2三小
         (b)
         The Fourier transform off(t) is


               F(w)＝之；[（쒸！미／iwtdt+ 4尸 [（半卜미／""』·
Combining entry number 1in Appendix D 꿔ith the integral




yields




                                                               ]
                             . .
                             I.
                                   .   .\   I
                                            mm8
                                            fi-
                                                  cos It0 w)
                                                           \
                                                               1
                                                     2
               "
                   (
                   ')
                        ＋긔
                                                   .2



Problem 19.2
 Show that iff(t) is an odd function,

               A(w) = 0

 and

               B(w) = -2 f;: f(t) sin WI dl.

 Solution

 By definition
 310                                                                  Chapter 19,The Fourier Transform




           A(w) = f       f(f) coswtdt.
Now break the interval of integration into two segments, from - cc to 0 and 0 to co. Thus

           A佃）= 尸         cos口玎dt + I甲 f) coswtdt.
                   r 4m               -o

Butf(t) is given to be an odd function; therefore the integral from -cc to 0 is the negative of the
integral from 0 to cc. To see this, make the following ch帥ge in the variable of integration in the
interval- co to0. Lett = -x, thenx = oowhent = -co;x = 0whent = 0; anddt = -dx. Therefore

           fD, f(-k) m5（小m:) (H血）= 可：f(x) cos姓毗

It follows thatA(w) = 0.
        By definition

          B(w) = -f！的 f(t) sin wt dt.
Once again break the integration into the intervals - cc to 0 and 0 to co. Then

          B(w) = -1!: f(t) sin wt dt - f: f(t) sin wt dt.
But becausef(t) is odd the first integral is identical to the second integral; therefore

          B(w) = -2f: f(t) sinwtdt.

Problem 19.3
G加eny(t) 玎二 珣九（t 쿄) d show that如）=F{y(t)} =X佃쎄마毗比X(w戶斗(t)}
andH(w) = F{h(t)}. (Hint: Use the defining integral to write Fly(t)} = f！的[f! m x(A)h(t - A) ILa]
e艸 dt. Next, reverse the order of integration and then make a change in the variable of integration;
that is, let (u = t - A.)


Solution
Using the hint given in the statement of the problem we have
Part B: Representative Problems with Solutions                                                                                                                                                            311




          F{              y
                                   (t)     }   =    Y
                                                            (w)             =        f!          .   [i
                                                                                                                            xQ)                  h          (t
                                                                                                                                                                     -
                                                                                                                                                                          ))       d]       e
                                                                                                                                                                                                "   '小.


Next, reverse the order of integration; that is, first integrate 꿔ith respect to t and then with respect to
又．Thus you c띠1 write

                                                                                                                                                 .
                                                                                                                                                                          dtjcL.
                                                                                                                                                                               1
                                                                                          ff00
                                                                                                                                                 e
                                                                                                                                                     -jwt
                                                        .
                                                                                                                                  2)
           Y
                    (w)                   =    f!                 x
                                                                      (A)
                                                                                                 -            h
                                                                                                                  (t-   -         2)                                                    .




To evaluate the integral inside the brackets, make the follo싸ng change in variable: let u = t - 又 and
then note that du =玄 and u = 士 oo when t = 土 OO. It follows then that

       f二 h(t 小又）e_.ia)i dt                                                                               =       C!        m          九   （u)                   e   “加    （" +i) du

                                                                                                          = e 'm f！的 九（u)eUodu
                                                                                                          = eU加i H (w) .

Substituting this result into the expression for Y(w) gives


               Y(co) =5巴, 工（2) eU' 노回d兀

                                           ＝丹（w·．) 500, 工（又）e_jO ld丸

                                               = 月＠)X佃）.

Thus the Fourier tr缸lsform of the output [Y(w)J equals the pr어iuct of the transfer function [H(w)J
and the Fourier transform of the input [X(w)1.


Problem 19.4
The current source in the circuit in figure A is given by the expression
           .                             4 戶 -A I 'r 1 .
           L, -                          1知 j ' ' 1A.
               1g             1中         1VV                                    .'
312                                                                                                          Chapter 19/The Fourier Transform



        a) Find vO(t).
       b) What is the value of vO(0) ?
        c) What
        C) \Vhat is
                 iS the value
                        ValUe of
                              Ofy0(O+
                                 vO(O )?
        d) Use the Laplace transform method to find vO(t) for I > O+.
        e) Does the solution obtained in part (d) agree with vO(t) for v > 0 + from part (a)?




        (a)
Solution

       a) Begin 切 飾如g the 民岫er transform of vO(t) u鈿g the relations노pV如） = I了（w)Ig(cu).
The s-domain transfer function Vo/Ig is the impedance seen by the current source in figure A. Thus

              ,7                      R(1/sC) -     R
              i: 1         =
                                     R + (1/sC) (1 + RCs)

For the numerical values given in figure A we have

                       -         '             -.                5
              I-I (S) = 乙 = H1.
                     '                                          s+ 1

It follows that



              H      (w)              ＝月                 (jw)    =   ，乙，
The Fourier transform of the given input current is

                . .      15     .  15
              /g（叫 = (-
                        jw + 4) 十（抑 + 4) '

Thus the Fourier transform of the output voltage is

                                                                 *75                      * ; 75
              乙
              VO                                                       (jw+ ,)         (jw+ 4) (jw+ 1)
                                                          j.
               （0)         (w)             =
                                           :        (-
                                                    (-
                                                          jw+
                                                                     4)（加*  1)   +
                                                                                 *（加
                                                                                                         ·
Part B: Representative Problems with Solutions                                                         313




A partial fraction expansion of J'O(w) gives

              , . .       15    .  40                           25
              V0(W) =(- jc9+ 4） 十（抑 ＋1)                       （加＋4) '

The inverse Fourier transform gives the time-domain expression for the output voltage,

               (t) = 15e4'u(- t) + (40eHt - 25eH中)u(t) V.
              v。


       b) From the expression derived in part (a) we have

              vO(O ) = 15V.


       c) From part (a) we get

               (0+) = 15 V.
              v。

Note that because there is no current impulse in the capacitor, the voltage across the capacitor cannot
change abruptly.

       d) In using the Laplace transform method to find v。    (t) for t > 0+, note from the solution
obtained in part (a) that the initial voltage on the 0.2-F capacitor is 15 V. Therefore the s-domain
equivalent circuit is as shown in figure B. The s-domain node-voltage equation that describes the
circuit in figure B is

                 . V。.V。 s    15
              -3 十 了 十 =S = (s+ 4Y

                         晶     小
                                   口
                                               돠   ］多룐   5-
                                                                  그．
                                                                       H
                                                                                   +
                                                                                   屹
                                                         百皿 T
                                       1
                                                                           겨＞
                                           1
        (b)
        S아ving for l今 gives

                ,       15s+ 135                 40             25
               VO =
                      (s+ 1) (s+ 4)            (s+ 1)         (s+ 4) '
314                                                                      Chapter 19/The Fourier Transform



       The inverse Laplace transform of the output voltage is

          % = (4C/'        ＆巧叩）V.

       e) Yes they agree.


Problem 19.5
It is given that F(w) = enJu(Hw) + enJ u(w).
       a) Findf(t).
       b) Find the 1-(2 energy associated withf(t) via time-domain integration.
       c) Repeat part (b) using frequency-domain integration.
       d) Find the value of w1 iff(t) has 90% of the energy in the frequency band 0 5 w 5 w1.


Solution

       a) A direct application of the Fourier inversion integral yieldsf(t); thus
                                               rJ
                                                的 0
          n/ .    1   .的
         八Ii =；긴小 ee'
                              i上） jt(O .   .   l石     e
                                                          H&) Jt(J) -,
                                                             e     口w
                                     口w十

                  1／兀
                 1 + r2 '

       b) Becausef(t) is an even function the 1-Q energy associated withf(t) can be found by
integrating over the interval of 0 to m and multiplying the result by 2. Therefore


         才m＝玎口咤肝亡J.    ＼上 ]   1 J


       c) The magnitude of F(w) is an even function. For 0 5 w 5 m, IF(w)I2 equals eH20). Thus

         까m극月／뇨 급J.
       d) From the statement of the problem we want to find the value of w1 such that


         記1 2(Od山仕｝
Part B: Representative Problems with Solutions                                                       315




It follows that

           1 - e12(J1 = 0.9,

or


           Wi =                       {inl0:             :         1.
                                                                        15 ta可s.



Problem 19.6
The input voltage to the high-pass RC filter circuit in the figure is

           v,   (t)         =AeHatu                          (t)        .




Let a denote the corner frequency of the filter, that is, a = 1/RC.
        a) What percentage of the energ戶n the signal at the output of the filter is associated with the
           frequencybandO 5 cv 5 aifa = a?
        b) Repeat part (a), given that a = v' a.
        c) Repeat part (a), 曾ven that a = a/v'3.




Solution

        a) Begin by finding the Fourier transform of the output voltage vO. This is done by using the
relationship VO(w) = H (w)匕(w). The input voltage is given; therefore V1(w) is known. Specifically

           （0)                                     ( A
          匕
                                               =
          V,
                      (w)                      =   (a
                                                        +Jw)                ·




꿔e fmd月（cv) by first finding the s-domain transfer func如미乙川）Fr恤 the cisc毗 in the figure we
have
316                                                                                                                                    Chapter 19/The Fourier Transform



                                                      R                                -   -




                   VO
                                  =       (／
                                                   之 + 노C)        (1／
                                                                                               '




Therefore


              I兀n＝                                                            RC노 =
                "  V1                                                        1+ RCs s+ (1/RC)
                                                                                                                                   .
                                                   丘＝
                                                                                                                      S
By definition a = (1/RC); therefore


                     그孚＝.
          月回 = H（加）= JI上J 丁 ({



The expression for VO(w) is


          乙
          V。                                                                      j A
                                                                                    (a
                                                                                  w
           （0)              (w)
                                               =
                                               =
                                                        (a
                                                        (.
                                                                   +jw)
                                                                   *j                          +jw)               .




The ma凹litude of VO(cv) squared is

                                                                                   2 .2
                       =                                                        口) JI
              IIL乙n,n尸                                                       2+
                  "
                                                                                    (a2+
                                                                              +a 2))（口      2
                        "
                                      n
                                          'I
                                                                        (a
                                                                                        +w)                                    '




When口 == 口 we have

                                                                                      2d2

              1乙
                            （"            샤
                                                             乙／
                                                                                  :",2)
                                                                                  +    w
                                                                                               )
                                                                                                   2   ·




The total 1-C energy content of the output signal is

                                                                                        2 d2                             12
          w . . = 三 rm                                                                口'4侄                       'I!,) ＝쓰－=
          "' oal  7r ' 0                                                     (a
                                                                             （口
                                                                                      2++w)
                                                                                          m 2)             2HH
                                                                                                                          4a
The energy content in the frequency range from 0 to a is

                                                                                      2 .2

          Wa                          "                 j    。          (a
                                                                        J;
                                                                             2 +w)
                                                                                ', 222dw
                                                                                   2)
Part B: Representative Problems with Solutions                                                                                                      317



                                                                                                                    a2
                        =A2h dw 7V I                      0
                                                                                                    尸                 dw
                                                                                                                          n)2)
                                                                          2+ m
                                                                             w)
                                                                              2)                                     +co)
                                                                                                                                 2
                                                    '
                                                                                                            (e2+
                                                                                                    '
                                                                    (a                                      (a
                                                   ,                       '
                                J吐                 1)l                    = 1
                                     d2
                        = =141 I -r - II .
                          4va \2        )


Therefore the percentage of the total is

                   Wa                . 八八                           1 127;                그             . nn         』n . m』
                                                                                                                           ，』
                             xl （乂) == =                                  1:        -II        Xl （八) 勺 l8. lf "/o.
                                                                          L乙              ]
               Wt。
                 tai                                                '1

        b) When口 d配sn아 equal口 we have


                                          lH兀
                                                                的                   w A dw
                                                                                    m2d2
                                                  月11V



                                                                                          )（口2 + w2)
                                                         0
          까otal=
                                                                                +
                                                                                    w2
                                                                    （口2
                                                   I
                                                                                          均
                                                                    尸
                                                                    m
                                              /
                                              兀
                                              1
                                                                                          m
                                                                                    n
                                                                                                긱
                                                                                          +
                                                                                                        +          , 2 +w)2
                                                                                                J
                                                                                                                                     卜｝
                                                                                                              (a
where

                                          2                                                                           2
                                 口                                                              , =                1口
                                                                          and
              !r


          人1 =                                                                                k
                             2   2                                                            =1L            2   2'
                            口 e 口                                                                           口 H 口


Carrying out the integration gives

                                                  A:Z
            w           .   =


            "                        2（口 + 口） '


In the frequency range from 0 to a we have


                        =                                                           A
                                                                                    d2dw
                                77; " 0
                                                                                        （口2+ nJ2w)
                                1尸
            刃.                                                                 띠2
                                                         （口2+                  m2w)




                        긔『：[，乙2) *,,:’시                                                                                                   dw
                                                                                                                                               },
318                                                                 Chapter 19/The Fourier Transform



where K1 and K2 are as given above.
      After integrating we get

                      .2     r          /   \     기

         吼乙（，亡, 2) '寸'（計卦
The ratio (Wa/Wt。
                tai) becomes


         금누 2r(a2-小an （升쒸·
When a = a'V this ratio reduces to 0.2723. Therefore 27.23% of the total energy content in the
output voltage lies in the frequency band between 0 and a厚.

      c) When口 = （口1'I手 ) 出e ra如 found in part (b) is 0.1057. Thus 10.57% of the total ener目
content in the output voltage signal lies in the frequency band between 0 and (可月).



Part C: Supplementary Problems

Supplementary Problem 19.1
       a) Use the Fourier transform method to find i (t) in the circuit shown in the fi留lre. The initial
          value of 1(t) is zero and the source current is 1(hi(t) A.
      b) Sketch 1(t) versus t.

                                                          3n



                                                                  ]H




Supplementary Problem 19.2
      a) Use the Fourier transform method to find v(t) in the circuit shown in the figure if vg(t) = 40
         sgnt.
      b) Sketch v(t) versus t.
Part C: Supplementary Problems                                                                 319




                                               80 ku




Supplementary Problem 19.3
The current source in the circuit in the figure is given by the expression

                        2: 1
          i17 = e        " /\.
                    中
           O




       a) Find vO(t).
       b) What is the value of vO(0 )?
       C)      iS the value
       c) What is     Vahle of vO(O + )?
                            0fV0(0
        d) Use the Laplace transform method to find vO(t) fort> ot
        e) Does the solution obtained in pard (d) agree with vO(t) fort > 0 + from part (a)?




 Supplementary Problem 19.4
 The amplitude spectrum of the input voltage to the high-pass RC filter in the fi암lre is

           .,. .    100
           V小U) == 1H1           100 5 ln기 드 200 rad/s,
                    'WI



          匕（叫 = 0,               elsewhere.
320                                                                  Chapter 19/The Fourier Transform



      a) Sketch IV (w) I2 for -羽0 5 cv 5 300 rad/s.
      b) Sketch I VO(w) J2 for -300 5 口J 5 300 rad/s.
      c) Calculate the 1-(2 energy in the signal at the input of the filter.
      d) Calculate the 1-c) 이比r町 in the sig耐 at the O啣Ut of the filter.
      e) What percentage of the input energy is available at the output?
      f) Repeat parts (d) and (e) given that R is changed to 5 k(2.
                                                Chapter 20
                                              Two-Port Circuits


Part A: Representative Drill Exercises with Solutions

Drill Exercise 20.1
Find they-parameters for the circuit in figure A.




       (a)
Solution
From the defining equations for they parameters we nOtey11 andy21 are found when port 2 is
short-circuited andy12 andy22 are found when port 1 is short-circuited. The circuit in fi햇re A 呱h
port 2 short-circuited is shown in figure B.

                                                      L A之
                                                                  aH
                                                                       -z-z
                                                I-   IV\ .f   1
                                +     77
                           二
                           VI
                                               吉初n            自도皿
      (b)
An analysis of the circuit in figure B gives

                 Vi   V1
                                    0.25 V1
             '1 = 而 + . . =

and



                                                                                                321
322                                                                         Chapter 20/Two-Port Circuits



                   V1
             /) = m1;
                  -> =-0. 2 V1


From the defmition ofy11 andy21 we have

                           V1
             Yii =                        = 0.25U
                                匕= 0
                         -'1
and

                               h百         = 0.25 U
             Y21 =
                                匕= 0

The circuit in figure A with port 1 short-circuited is shown in figure C.

                                                               5그2m
                                                         ]    小人／
                                                         三寸



       (c)
From figure C observe that


             /,'2 = l5
                    V2 +' 므
                          5
                            = 但）
                              \
                                 T7           15) V2

and

             /,
                      卜V2= >        -0.
                                          2匕．  H




By definition

                               h瓦                  U
                                                   0八乙

             Y12 =                  匕     0


and
Part A: Representative Drill Exercises with Solutions                                                                                       323




                              b瓦
                                                                )                        口匹       U
         Y22 =                                 匕                印




Drill Exercise 20.2
The following n妃asure毗nts were made on a two下山rt re前曲ye circ毗 With 10 mV applied to port 2
and port 1open, the current into port 2 is 0.25肛A and the voltage across port 1is 5 isV. With port 2
short-circuited and 50 mV applied to port 1, the current into port 1 is 50 uA and the current into port
2 is 2 mA. Find the h-parameters of the network.


Solution
From the equations that define the h parameters we have

                     l                 hn                                                m                立h                   =
                     l
                                                                                                                       匕
                                                                                          1
                                                            匕
                                                                                                  1
             1
                 n
                                                                         0
                                                                                              d
                                                                                                      n
                                                                                                                           0        =
                                                                                                                                   e1




                                       匕瓦                                         and 1222 =
                                                                                                          b瓦
          /il2            =                                                                                                0
                                                                                                                           1




                                                                         却                                     L
                                                                                                                                        =

                                                                                                                   1
Therefore with port 1 open (Ii = 0) we can determine h12 and h22. From the data given in the
statement of the exercise we have

                     :=            s
                                                            ,
                                       x
                                                        0
          h12=
          九；
                                                                             =
                                                                                  5x10
                                                                -
                                                   ,'
                              1。x

 and


           方끄： 1。，“ ,
                25            0.
                                                                    으；
                                                                             ':          251ut.


 With port 2 short-circuited (V2 = 0) we can use the given data to find h11 and h21. Thus

                               r1\         .   .    m1＼尸3


            hll= J1JXl1J .=ioooc
                     --       50x10m

 and
 324                                                                     Chapter 20/Two-Port Circuits




                   =   2x
             h21          ,',
                            "
                                :
                                    =
                       5。x              的.
Drill Exercise 203
The b-parameters of the two-port network in figure A are b11 = 20日/3, b12 = MQ, b21 = 去U,
and b22 = 中100/3. The network is driven by a sinusoidal current source having a ma址nlum曲plitude
of 100 MA and an internal impedance of 1000 + JO . The network is terminated in a resistive load of
10kQ.
       a) Calculate the average power delivered to the load resistor.
       b) Calculate the load resistance for maximum average power.
       c) Calculate the maximum average power delivered to the resistor in part (b).


                                                                    ；二
                                                  Two-port model
                                                       of a
                                                     network




       佃）

Solution

       a) After making a source transformation at the input port, the phasor-domain circuit is as
shown in figure B.


                                             三；
                                             +                            ]
                                                                          L＜下1
                       口ild                                                    D
                                                                                   蚣
                        V                                                 十帖 +
                                                           [b]
                                             1{
       (b)

From Table 20.2 we have

             V2                AbZL
             V8    B12 + biiZg + b22ZL + b21ZgZL'

where ZL = (10 + JO) kQ, Zg = (1 + JO) kQ, and Vg = 0.lLQ V.
Part B: Representative Problems with Solutions                                          325




       For the given values of the b parameters we get


               트Vg

or

          V2 = (- 中昑)(0.1匹D = 尸40 四 = 40L쯔竺 V.

       The average power delivered to ZL 15

                          . n2 \
                     . f '4U
          -          I       I  I                             尸1八

          p＝         三       (io而j)
                                                          ＝
                                                              刈mw.


       b) From Table 20.2 we have



          7:
                 =
                           ：告
                         :：二：
       For the given values of the parameters we find Z1 = 40 k(2.

     c) When ZL = 2:i = (40 + JO) kQ, the ratio (V2IVg) becomes -1000. Therefore V2 =
100／완；亡 V and the average power delivered to the 40-k(2 resistor is

                                      /               \
          "’推匐’ "'"
                         .                .   ,,,,2




Part B: Representative Problems with Solutions

 Problem 20.1
 Find the b-parameters for the circuit shown in figure A.
 326                                                                             Chapter 20/Two-Port Circuits




        (a)
 Solution

To fmd b11 we must determine the ratio (V7JV1) whenIl is zero. To find this ratio we analyze the
circuit shown in figure B.

                                                               妃그1之＋毛   寸- .1노




                                                      亡染三
                                                                             十
                                                                             t色

                                                               1O-n--
        (b)

        Since '1is zero the currents 'a and 'b are

                                                      V2
                                   and
                    ,


                        ;;;
                        ［色
                                                      40
              /a=
                        141J
                                                /b=
        The voltage 1q is

               Vl = 30I - 101b


                             和     m
                                   而     0
                                         l      似
                                                而＼
                                                           즈
                                                       2
It follows that


              b11 =          丘 匕       0
                                   l
                                           2.
Part B: Representative Problems with Solutions                                                   327




       We also find b21 whenIl is zero. That is,



                               '1 = 0


       From the 由Cu止in 旽出eBn야야hat

              ,      ,       . ,        2172          V2
              i2=    'a 十 ib = ==                = ;;;
                                        나V            二U




and since V1 = { V2, we have


              b21= (끎니針듦 = o.1o ty.
                                                                                                      in
       To find b12 and b22 we short-circuit the input port. Hence we must analyze the circuit shown
fi凹ire C.




        (c)
 With the short circuit in place the port 2 current is


              '2 =                                                           15
                                                  130 (10)1
                         r         -




                         1旦9Xl9기             +    1 1:
                                                      )1＝二 1

                         [     40       j         L 4o J
 The current at port 1is


                  '1= /.-/.닉응'2－졺／:=－글'2·
 By definition

                                   트h                        - 1Sf,
                                                                             和c
                  b12 = -               匕        0=      H    (12/
                                                                     2
                                                                     )
                                                                         =
328                                                                        Chapter 20/Two-Port Circuits



and


                                  =
                                      2.
                          v1= o


Problem 20.2
Find the s-domain expressions for the a-parameters of the two-port circuit shown in figure A.




            (a)
Solution

The par缸neters a11 and a21 are found with port 2 open. The s-domain equivalent circuit with port 2
open is shown in figure B. When '2 is zero, j1 is



                  11=[f(s+1)1)+*(}(i1) =IL(s2으겊2）
                        (5+2)]
                  "1 [(5r, (V1]                卜·
                                              g Jlm




                                                                     寸Hm
                                                                             乙   =<:
                                                                                       :;
                                                                                +
                                                                                  1／노

      (b)
Part B: Representative Problems with Solutions                                                                                   329




The current 'a is found using current division, thus


              'a
                    =
                         1 1 ] ,
                         [(s
                                         +2
                                                   )
                                                       ]   1F



The port 2 voltage is



              n＝玩* (})'1＝除끔］'1
                        = r2（브土- )1F 如 +2) ] V.
                               LS
                                    (S
                                              + 2)         J    [S2
                                                                          + 2r + 2]     '           "




By definition
                                                b
                                                                                 + Zr + 2)
                                                                          (s2
                   l
                                              竺巧
                                                                      -                                              =

                                                                0
                   口
                                                                                2(s + 1)                                 =




                   )
                   1
                   n                          h瓦                - s(s + 2)                                           =

                                                       伊    0     2(s+ 1) '


       The parameters a12 and a22 are found by placing a short circuit across port 2. Thus we must
analyze the circuit shown in figure C.
                                                                                                             二
                                                                                                        缸仰
                                                                                                                             +
                                                                                                                 시


                                                                                            茂
                                                                                                크
                                                                                                         T
        (c)
 In particular we determine the ratios

                                              V1
                   口12         =         二；
                                                           V2 = 0


 and
 330                                                                                                           Chapter 20/Two-Port Circuits




             a22 =                            =
                                                  쯔b              匕   0


From the circuit in figure C we have

                                                           V1                   回421vl.
                                                                                L(S'+ 2)J "
                                   1*［굡缶］
            'a
                                     rl)
                                     \S/ H
                                                      /,
                                                                      I         ]       ]            V1
                                                                                    1
                                                                                    )
                                       L ks)]
                                                                          (s+
            '"
                                                                                        jia_
                                                                                               (s+
                                                                                                          2)
                                                       1,
                                                            )］가
                                       [11{
                             '
                                       11+
                                                  (
                                                            'i1
and

                                   1二
            '1   t
                     '       ==   二＝
                                       S      .




Now note that

                            Ii 1 1_ -
            '2= e1b -/ ' = 下＋규万］v1,
and therefore

                 ,, m 奭브：22
                 '                     2（了 + 1)'

Also note



         '1 ='a*'C= 皓H｝匕
                         =
                                 （夕’
                                  ，：弦 '）匕·

But
Part B: Representative Problems with Solutions                                                              331




              匕＝
                       -a1212=
                                           :   긺
                                                   '+
                                                            2)72,
                                                        + ,1)

therefore

                                 S2 + 2s
                                       4- 2
              C22=                耶 + 11) '


Problem 20.3
The linear transformer in the circuit sho싸n in figure A has a coefficient of coup血g of 0.65. The
transformer is driven by a sinusoidal voltane sour尤 whose internal voltane is v'. = 100 cos 200i V.
'["tie internal impedance 01 the source is 1U + jO L2.
       a) Find the phasor-domain z-parameters of the linear transformer.
       b) Use the z-parameters to derive the Th6venin equivalent circuit with respect to the terminals
          of the 400-Q load.
       c) Derive the steady-state time-domain expression for v2.

                                                                                                -
                                                                    I-
                                                        IOU         1    201i   kY       160U       1
                                                                                          八 八 m;        =
                                                                                     1                  十

                                                                                     的   H
                                                                                         m              m

                                                                                                        1




                                                                                                        1
                                                                                                그
       (a)
 Solution
       a) The z-parameter equations in the phasor-domain are

                   Vi = ZllI1 + Zl2I 2

 and

                   V2 = Z2lI1 + z2212.

             The transformer Phasor-domain circuit is shown in figure B.
 332                                                                        Chapter 20月wo-Port Circuits




                                                   反口J之          d52Jt   m＜느之    十l三



                                                                 言   旨료'＝그．
                                    H＋万
                                      {
                                                   1\




                                          S+            A/   ＝
       (b)

In constructing the circuit in figure B we have used the fact that w is 2000 rad/s andMis 26 mH. The z
parameters are


               z11                         = (20 + 120) c ;
                                  12 = 0




              z21                          = J52 Q;
                                  '2 = 0




              2l2                          = j52 c ;
                                 Ii = 0

and


                                           = (160 +j320) c .
          7::
                                 'I = 0
                     푸，
       b) From the statement of the problem we know Zg = (10 + JO) Q and Vg = 100／으 V. Using
Table 20 1we find

              ,-                  Z12Z21
         乙'= ' 22
                                 zii + Zg

and



                               Zii + Zg
         \=
                          [:
                                ,,'므乙卜．

The nuz玭rica! values 可乙 and＼乙 缸e

         Z1= 222.4 + j278.40 Q
Part B: Representative Problems with Solutions                                                     333




and

             V1 = 80 +j120 = 144.22 L5쏘1 V.

Using the Thevenin equi'valent the circuit in figure A can be reduced to that shown in fi암lre C.

                                      규？乏4_17_       j27日4皿
                                         小人／HHH8?m
                    佯4.22
                         V

       (c)
       c) From the circuit in figure C we have

                  1 144.22 / 56.31. 1
                       －;;；互而）] 44刃
             "『 1(622.4」
                = 84.61 /32.21' V.

The time-domain expression for v2 is

             v2(t) = 84.61 cos (2000t + 32.21') V.



Problem 20.4
The follo岫lg dc measurements were made on the reciprocal, resistive, two-port circuit shown in the
figure.




                       176 V (Jc)
 334                                                                   Chapter 20/Two-Port Circuits




        加匹4SURE人lENT!                                MEASUREMENT 2           MEASUR万兀lENT 3

   V1 = 50＼乙                                     Vi = 0 V,           '1 = 0 八

  '1 = 5 人                                       Ii = -8A,           '2 = 5 八

  '2 = OA;                                       1今 = 20V;            V2 = 42V.



A variable resistor RO is connected across port 2 and adjusted for ma油um power transfer to RO.
Find the ma疝mum po＼叱r.


Solution
In studying the measurements made on the resistive two port we note measurement 1is made with
port 2 open and measurement 3 is made with port 1 open. Hence z11 and z22 are readily obtained.
Spec小떼ly

           m    旦h                   = 훨 = 10 '
                                 L
                                     0   >                               =
                             1
and

                즈b
                                             끄
                                                 Q
                                                 4
                                                 8
          Z22            L
                                                                                     =

                                                                                         =
                                         5
                     1
Since the two port is reciprocal we know z12 = z21. Therefore if we express the data in measurement 2
in terms of the z-parameter equations we have enough information to compute z12. Kno刃ing z11
                                                                                               and
z22 we can 찌rite

          Vi = loul + z1212

and

          V2 = z1211 + 8.412.

       In terms of measurement 2 the equations become

         0= -80+ z1212

and
Part B: Representative Problems with Solutions                                                 335



          20 = -8z12 + 8.412

      From the first of these equations we have 12 = (801z12), and hence the second equation
reduces to the quadratic expression


          z2 + 2.5zl2 - 84 = 0

The solutions for z12 are

          2l2 = -1.25 土 9.25.

Since the network is a reciprocal, resistive circuit z12 is positive. Therefore

          2l2 = 8.0 c.

       Now using Table 20.2 on pages 841召42 of the te虹 along毗h the data in the fig出e, we get

          .,         z21V    8..,.._.            .
           vt= 2ll
               Z11+ Zg = -j (IIO) =ooV
                   +2g
and

          尸1    ,1
                              Z12Z 21    .   ,   ,－뇨

          乙1 = 八i = 222     -    1 '7 ='1·（1 bd.
                            '11 기＝ 乙g


For maximum power transfer RO must equal 4.4 Q. From the Th6venin equivalent we know the
voltage across RO will be 44 V and therefore the ma虹mum power is




Problem 20.5
Derive the equivalent circuit that is satisfied by the g-parameter equations.


Solution
The g-parameter equations are

          'i =g11V1 +g1212
336                                                                    Chapter 20/Two-Port Ciicuits



and

             V2 = g2i "i + g2212

In visualizing a circuit that is described by these equations, note the following.Il is made up of如
components, one determined by V1 and the other determined by '2. Therefore at the input port we
have two branches in parallel. One branch carries the current g11V1 and the second branch carrie:; the
current g1212. Therefore at the input port we have the arrangement depicted in figure A. Note that g11
is an admittance and g12 is the current gain when V1 = 0.

                                              그/
                                                        m
                                        1H누




                                    +
                                                       1륭그
                                                                        2
                                    vL                                   工z



       (a)
       Focusing on the equation for V2, note it is also made up of two components. The first depends
on V1 and the second depends on '2. Therefore at the output port there are two branches in series.
One branch is an impedance g22 carrying '2 and the second is a dependent voltage source g21V1. The
two voltages are additive. Thus port 2 has the arrangement shown in figure C.

                                                       日22




                                              和匕
       (b)

Note that g21 is the voltage gain when '2 is zero.
       Finally we can combine figures A and B to get the g-parameter circuit shown in figure C.

                        -       .                                 2

                            /                  1   1
                            .드                吉97 令孔石 「921 4
                                                                            4
       (c)
Part C: Supplementary Problems                                                                       337




Part C: Supplementary Problems

Supplementary Problem 20.1
Find the z-parameters for the circuit shown in the figure.




Supplementary Problem 20.2
Find the a-parameters of the circuit shown in the figure.




Supplementary Problem 203
The following measurements pertain to a two-port resistive circuit. With port 2short-circuited and
20 V applied to port 1, the current into port 1 is 2 A and the current into port 2 is -0.8 A. With port 1
short-circuited and 25 V applied to port 2, the current into port 2 is 1.4 A and the current into port 1
is -1.0 A.Find they-parameters of the two-port.


Supplementary Problem 20.4
Find the phasor-domain values of the a-parameters for the two-port circuit shown in the figure.
338                                                                     Chapter 20/Two-Port Circuits




Supplementary Problem 20.5
The operational amplifier in the circuit shown in the figure is ideal. Find the h-para毗ters of the
circuit.




Supplementary Problem 20.6
Find the s-domain expressions for the a-parameters of the two-port circuit shown in the figure.
Part C: Supplementary Problems                                                                       339




                               如
                                    甕難        驪     瀜茁




                                                                    셔
                                                                    固1m
                                                                      m
                                                                          ；二
                                                             노                 +


                         V1                                                    V2
                                               ?
                                                    毋崙
                                                             月




                                                   膊轉皺 j


Supplementary Problem 20.7
In the circuit in the figure the g-parameters of the two-port are

          g11 = -20 x i0-4 5,        g12= 3X 102,         g21= 2000,                g22= -20,000Q.

The internal impedance of the source is 1000 + JO c 기ld the load impedance is 10,000 + JO c.
       a) Find V2.
       b) Find the average power delivered to ZL in mW.
       c) Find the load impedance ZL that will result in ma如um average power tr瑯fer to ZL.
       d) Find the ma虹nium average power in part (c).
       e) Find V1 and Il under conditions of maximum power transfer.
       f) How much average power is delivered to port 1when maximum average power is delivered
          tOZL?




                        自｛多
340                                                                    Chapter 20/Two-Port Circuits




Supplementary Problem 20.8
      The z-parameters for the resistive two-ports in the figure are

        2'll= 100 C ,                     z11 = 80 (2 ,


        2 ' l2= -500 Q,                   2l2= H400 c ,


        z'21 = 1000 Q,                    22l= 2o00 c ,


        2 ' 22= 10,000 Q,                 z22 = 16,000 c .

      Find the input resistance Z1n = V1! 1.




                                                                          5 k1)
                  Solutions for Supplementary Problems


Chapter 1
l4   a) p = (15)(20) = 300 W, AtoB.

     b) p = 100(- 5) = -500W, B to A.

     c) p = -50(4) = -200W, B to A.

     d) p = -24(- 16) = 400 W, Ato B.

l名   a) j)
        p=       2401x10te
             vi= 240l X
           = yi         l03 2e -2띠1W.

           字 48.02 105te-
            (Si
                  =            x        2aX '   (1   -   bOOt) W/   s.
           뽀=0                 when     t = 0, t = ims;                  PmaxOCCtt1satt = ims.
           at
               八 1 r1.1 . d n5/mr뇨r뇨』
                                    ＼ ' m nH6그 -2   八八 1 ,1. .
     D) Pmax = 乙＜1.ui x lu ( jt人人Jx1u )e          = 3乙4스／4 mw.

                                    的
     c)
           叩＝ 24.01 x 105 f              t2匕-2띠idt= d刃．254uJ.
                          0

L3   a) v(12.5 ms) 브 40.12 V,                   1(12.5 ms) 브 40.12 mA.

           p = vi 斗 1.61W.


                      m 戶1J0
            W
                               25.可1a' sin260t dt = 28.8 mJ.                                           =
     b)
꾜          Pa = -5 x 60 = -300 W (del),                       Pb = 1 x 60 = 60 W (abs),

           Pc = 2 x 60 = 120W (abs),                       Pd = 2 x 40 = 80W (abs),
           Pc = 2(20) =' 40W (abs),                       Pabs = 60 + 120 + 80 + 40 = 300W,

          Therefore,pdeljvered = Pabs。
                                     thed.


                                                                                                 341
342                                                                      Chapter 1




工巨    a) Pa = 20(2.4) = 48 W (abs),     Pb = 12(2.4) = 28.8 W (abs),

         Pc = 32(0.4) = 12.8 W (abs),    pj = -28(2.8) = -78.4W (del),

         Pe = 60(1.2) = 72W (abs),      Pf= -60(4) = -240W (abs),

          Pabs = 48 + 28.8 + 12.8 + 72 = 161.6 W,

          Pde1 = -78.4 - 240 = -318.4 W. Does not check.

      b) Pabs = 161.6 + 78.4 = 240 W,

         Pdel = 240 W. Checks.
Solutions for Supplementary Problems                                              343



Chapter 2
꾜          a) i3 + i 6 = 12,,   313 = 日6;    therefore, i3 = 8 A.

           b) 16= (112) i3= 4A.

           (:) V노 = 갚3 = 日6 = 24V.

           d) P312 = (8)23 = 192W, P6(2 = (4)2(6) = 96 W.

           e) P12A= 288W.

2교         a) i a + 'd m 'b = 0; therefore, id = i b m 1a = -6A.

               i d + i e + 20 = 0; therefore, i = m 20 H id = -14A.

               i e + i c 卞 i a = 0; therefore, i = i口 - ie = 16 A.

      b) p5Q= (2)2x5= 20W,                   p6f2= (2)2X6= 24W,

              P1Q = (巾6)2 > i = 36 w,          P2Q = (_14)2 x 2 = 392W,

              Piif2 = (_ 4)2 x 11 = 176W,          j73f2= (16)2 x 3 = 768W,

              p4Q = (16)2 .x 14 = 1024W.

      c)
               -90 + i d + V + 11gb = 0,        V = 90 m id 叫 11ib,   v = 140V.

     d) p20A(del) = (140)(20) = 2800W.

              II 'R =20+ 24+ 36+ 392+ 176+ 768+ 1024= 24中［) W.

              P의）v = e 90i6 = -90(- 4) = 360 W.

              Therefore, 1P(abso巾ed) = 2440 + 360 = 2800 W = PdeI·
344                                                                                                               Chapter 2




2쿄    a)
                                                        1小1
                                                       WV -

                                               디
                                      )
                                          H+                                          1
                             그6I V                                                    1
                                          냐
                                                                                      노
                                               ｛뇨
                             그 '1 V




                i1 = (261- 216)/i = 45A,                      i3 = (- 204 + 261)/i = 57A.

               Pupper = -261(45) = -11,745W (delivered),
                 wer = - 261(57) = -14,877 W (delivered).
               Pl。

      b) 1Pde加ered = 11,745 + 14,877 = 26,622 W,

                EPdissipated

                       = i}(1) + i글（2) + i궁（1) + i三（10) + i}(5) + i릉（20).

               i2= -v2/2 = -(- 24)/2 = 12 A,

                i4 = (216 + 24)/lO = 24 A,

                i5 = (- 24 + 204)/S = 36A,
                i6 = (216 + 204)/20 = 21 A.




           1 勺
             1   白
                 1
2A    a)                 = 40/10 = 4A,                                      b) v2    =100- 40= 60V,




           h
                         = 60/6 = 10 A,                                         V3   =213= 12V,


               b
               1   b
                   1
                         = i2 - i1 = 6A,                                        v4   =40- 12= 28V,
                         = 28/4 = 7A,                                           v5   =72i5= 72V.
                         = i4 - i3 = 1 A.

      c) is = j2 + i5 = 11 A,                       Ps = - 100iS = -1100 W,
         p5(delivered) = 100 W

      d) P6Q = 102(6) = 600W,                           Q = (4)210 = 1印W,
                                                      P1。                            P2Q == (O) Z = ／乙 w,
                                                                                            //\2八   -m   11   r




               P4Q = (7)24 = 196W,                   肋2Q = (1)272 = 32W.
Solutions for Supplementary Problems                                                                345




      e) Yes, pdISS= 600+ l60+ 72+ l96+ 72= ll00W.

 2亞                                                                   B.n.
                                                                      44
                                                                       Mv-
                                                                                        1




                                                                                            d d d
                                                                                        +

                                                                                        느
                                                                                    1
                                              나5A
                                                                                    1
                                                    -.,3I         出1.1.
                     aov4)
                                                                + '
                                                                戶V/
                                                                             =   n 뇨“.a
                                                    쓰／      才     .     V.
                                                                 寸VV\

                                                                 O.75..n.

      a) v = 20- 12 = 8V,                b) i5 = 5 + 1= 6A,

         ja =8/2 =4A,                        P3ov =-30(6)

         jb = 13+ 4 ==1A,                                =-180W,


         (R + 8)1, = 30 - 8 = 22 V,      Therefore,pdel = 180 W.


         Therefore, R + 8 = 22/1 = 22 (2 ,

                orR = 14 Q.

？亞    a) Summing voltages around the left closed path yields
          5.7 = 25i八 + 0.70 + 0.5(! + 49iA).
          Therefore 1A = 0.1lllA.

          Summing the voltages around the right closed path yields
          10 = 49(0.1)(1) + v, + 0.5(50)(0.1).
          Therefore v, = 10 - 7.4 = 2.6 V.

      b) PS.T. ' = -5.7(0.1) = -0.57mW = -570uW,
          P25k    = (25 x 103)(0.01) x 10小 = 250MW,
           .5k = 500(5 x 10_3)2 = 12,500 4uW,
          P。
          P1k     = 1000(4.9 X l 113)2 = 24,010 1uW,
                                (:
346                                                 Chapter 2



      Pl。
        y = -10(49)(O.1) x iO4 = -49,00QuW,

      P4아八 = 2.6(4.9) x iO43 = 12,740pW,

      PO.7V = 0.7(0.1) x i0H3 = 70 AUW.
      Z尸generated = 570 + 49,000 = 49,570川V,

      3Pabs。
           rbed = 250 + 12,500 + 24,010 + 12,740

                   + 70 = 49,570/
                               1W.        Checks.
Solutions for Supplementary Problems                                                           347



Chapter 3
  J,   a) The equivalent resistance across the千A source is 25 ; therefore, v50Q = 4(25) = 1어）V.

       b) v텨） = (20/50)(100) = 40 V.

 1Z    a) 51 120= 4Q,         6l I18l I18= 3.6(2,    IO =33I6.6= 5A.

       b) 61 118 = 4.5Q,       i14 = 5(4.5)122.5 = 1A,     P14 = (1)214 = 14 W.

3쿄     a)




       Vb= 8(5) = 40 V,        2이180+ 4= 20c, i= 40/20= 2八

       ix = 8 + i = b0A,       v   = 20i)? + 6b = 100 V.

즈크     a) i = 90 mV/10 = 9 mA.

       b) i m = 90 mV/ IS = 6 mA.

       c)
            i = 9/1000 = 9 mA,      im = 9/1005 = 8.96 mA.

3亞     a) The ammeter resistance is 1Q. The resistance seen by the 60 V source is 603 C. Therefore,

            imeas = (60/603)(12/16) = 74.63 iiiA.

       b) The resistance seen by the source is 602.4 (2. Therefore,

            i3Q = (60/602.4)(12/15) = 79.68 mA.

       c) Percent error = [(meas - actual)/actualj x 100 = -6.34%.

3垣     a) 25V.
348                                                                                       Chapter 3




      b) Rm = 30 k(2, 30 kQ, 30 k（기 1 15 kQ = 10 kQ,

           Vmeter = (10/20)(25) = 12.5 V.

      c)
           301 110 = 7.5 k(2,   Vmeter = (7.5/22.5)(25) = 8.33 V.

      d) No, because of the meter loading.

玉2    a) 15-V terminal: R1 + Rm = (1S/10)10J = 1500 C.

           Therefore, R1 = 1500 - 20 = 1480 Q.

           150-V terminal: R1 + R2 + Rm = 15,000 (2.

           Therefore, R2 = 15,000 - 1480 - 20 = 13,500 Q.

           300-V terminal: R1 + R2 + R3 + Rm = 30,000 Q.

           Therefore, R3 = 15,000 c.

玉旦    Use method 1because the ammeter resistan氾 of 10Q is negigible compared to R. 기：is
      m啣始 the voltmeter will read very cbs아아he true voltage across凡．S뇨ce 小e ammeter is
      reading the true current in凡the ratio of the volt毗ter rea函昭 to the ammeter rea曲培 w찌［
      be the best measurement of R. Note in method 2 that since the resistance of the voltmeter is
      of the same order of magnitude as R, the error in the ammeter reading will be appreciable.

      a) 凡 = 50kQ.


           Method 1: Am = (150/50,010) A,

           匕i = 150 V,      Rmeas = 1／뇨二4?月 = 50.01k(2.

           Error = [(50.01 - 50)/SO] x 100 = 0.02%.


           Method 2: Am = 150/{10 + [(300)(50)/350J103} = (105/30,어）7) A,

           Vm = 150 - 10(105)/30,007 V,      R = Vm/Am 斗 42.86 k52.

           Error = [(42.86 - 50)/SO] x 100 = - 14.29%.
Solutions for Supplementary Problems                                                               349




      b) R = 100kQ.

            Method 1: V,n/Am = 100.01 kQ. Error = 0.01%.

           Method 2: V7 IA77i 斗 75 kQ. Error = -25%.


玉9




                                     그5A




        戶   n
            乙
                q
                    1
                        <
                                ＠
                                    日    M       戶         乃
                                                               學    = 1.5 A,
                            乃
      v24 = 24(i2 + i3) :== 60 V,

     吻= rl.2 +(l꼬．의 (i2 +b\' = 6(2.5)
        \n         )                乙，
                                     0
                                      = 15 V."   -   .3)   "   .'   "   寸   ’   ．




                                                           + sv -                   4   1 0V   -




     a) i1 = 7.5/6 = 1.25 A.
350                                                                          Chapter 3




      b) i2 = 1.OA.

      c)   -v + 10- 7.5 = 0,   v = 2.5V.

      d) P2.SA = -(2.5)(75) = -187.5 W;    therefore, p23A(del) = 187.5 W.
Solutions for Supplementary Problems                                                              351



Chapter 4
jj,    Use the bottom node as the reference. Let v1 = node voltage across the 5 C resistor, let v2 =
       node voltage across the 10 (2 resistor. Then

       "';10* 긍* '"' ; "' =0 V1＝끅므：9．們v,
       V2- V1 . V2   -. -'             840    . ,, ,,d !,
         八   十 ;:; 小 L =U,        V2 = 二二＝ == 上u.11 v,
           乙       LU                    / /


      i口= (10 - v1)I1 = 0.91 A,      i b = (v1 - v2)/2 = -0.91 A,

      iC= vl/5 = 1.82 A,     b= v2/10 = 1.09 A.

4.2   a) Use the bottom node as the reference node. Thus

            v- 50 v  v- 15iO n .        .＝八 n-.   .         '－寸－ .
              尸 +: +    .   = U, s, = vfZU. I'heretore. V = 32 V and In = 1.O A.
               그        LU    4                中             '                 V


      b) The current delivered by the 50 V source is (50 卞 v)/5 + (50 - 15iO)/10, or 6.2 A.
         Therefore,p4.;0y(del) = 310 W. The current into the + terminal of the dependent source
         is (v - 15i)/4 + (50 - 15iO)/10 = 4.6 A. Therefore, the dependent source is absorbing
         (24)(4.6), or 110.40 W.

玉쿄    a) Let v2 be the node voltage across the 55-Q resistor. Then
           v1- 125 - yl . v1 小v2
             25   十面十 40                                         v1   =100V
           V2 = 125 + 15i中                                            = 110V
                                                                 V2
            . v1 - 125
           i中＝ 25

      b'          ..2
               2= V2
       '   P55{ =
           pss        = 220W.


      c) The current directed up through the 125-V source will be


           Is：諍늉 3.25A,               Pi25v = -125(3.25) = -406.25W,

           orp125y(delivered) = 406.25 W.
352                                                                                           Chapter 4




        d) v1 = 100 V (unchanged),           v2 = 110 V (unchanged),

            .       V1 .   V2    八 八戶 ．
            'S = 苗 十 茄 = 2.25八
            p125(de1ivered) = 125(2.25) = 281.25 W.

4.4    Defme 1a andib as clockwise mesh currents in the lower left기d lower right windows respec-
       tively.

       a)
            -136 + 2ia + 8(ja - 3) + 40(ia - ib) = 0,

            40(ib- ia) + 10(ib - 3) + 50 = 0.

            Therefore, i a = 8A,      i b = 6A,    V = 40(ia m i b) = 80V.

      b) p136(del) = 1361a = 1088 W, p50(abs) = 501b = 300W,

            V3A = (8 - 3)(8) + (6 - 3)(10) = 70 V,          P3A(abs) = 210W.

쏘     Let i1 = cw mesh current in lower left mesh, i2 = cw mesh current in upper mesh,
                                                                                              i3 '= cw
      mesh current in lower right mesh. Then:

      51i + 10(i - i2) - 3(- 15i2) + i3 = 0,                        ii   =4A

      15i2 + 3(- 15i2) + 10(12 - 1) = 0,                            i2   = -2A

      i3- i1= 6.                                                    i3   = 10 A

      P1sQ=   '2 · 15= 60W,
      Pl552 =.2                                                       Q = (i1 - i2)2 · 10 = 360 W,
                                                                    Pi。

      Pic2 =i孕 ·1= 100W,
                                                                    P3{2= i三 . 3= 48W,

      P2Q = i三 · 2 = 32 W,                                          yA =-15i2= 30V,

      3vA = 90V,                                                    P3vA = 卯侮 - 13) = -10凹W.

      VA        = voltage rise across 6-A source in the direction of the 6-A current

                = 10(i2- i1) -5i1 = -80V.
Solutions for Supplementary Problems                                                                   353




       P6A = H6VA = 480W.

       >Pabs = 60 + 360 + 100 + 48 + 32 + 480 = 1080W,

       1Pde1 = 1080 W. Checks.

 또亞    Vt = v2 = -SO,OOO(40)ib = H2 x lobib,                           1b = (0.1 - 4 x 10中'v2)/1080;

                       （刃肛八 Vt = -200 V.
       therefore,i b = 1

       To find R (see the figure):




                         1    1   .   m ,S-   5      I
              VT         I 14X1U                  VT 1            -
                         l
                                                                       VT     戶. . 八
                   +40                                            /<i= =.1 = : 4 k51
       iT= 50,0刃                  1080             -   I   '           'F'
 4.7   First find the Thevenin equivalent with respect to the terminals of the resistor; Vt = 35 V and
       Ri = 3.5 kQ.

       a) R= R1= 35kQ

       b) p = (5 x 10""3)2(3.5 x 103) = 87.5 mW

       c) With R set at 3.5 kQ (see the figure), the following equations hold:

                                      $kJt1

                                                                       +
                       H口 V                                    .2Ok.n. ＝乙夕／
                                                                                             落

       p40v(de1) = 40(3旬 = 140 mW,

       po.751(del) = (22.5)(3.5)(0.75) = 59.0625 mW,

       Percent = (87.5/199.0625)100 = 43.96%.
354                                                                                             ChaPter 4




塑          a) First find the Thevenin equivalent with respect to the terminals of RL. Let v1 be the node
              voltage across the 100-Q resistor with the lower node as the reference node. Then:

               v]'- 100       Vi           Vi
                ' 50      +j高- 05-j友j= 0; thereforevi= 얹）V.

              》小娜小凹* 1喘小？·
               No꽈 됴nd 凡 (see the figure):




                ..        . . .4,   5000.       .      .. . 八 戶. . 50
      VT = (IT + (J.:l8)(2U + -:;- ;;-),        18 = ('T 十 U.:)I8) 二；
                                                                    ;!
                          '         J_JU        "              "   iJ, J


      Therefore, i少0．屯： and 切＝(iT* 0·刀：)(20구學）·
      R1 = VT/iT = 64 52. Therefore, RL = 64 (2.

      b) Pm.x= 442/64= 引그1.25W


                                                    口" 5 1P
      c)
                              好
1!
     嗣



     Solutions for Supplementary Problems                  355




     포으    V = (80/3) V,     R1 = (22/3) c;   therefore,

           .      80/3     80    .
            0 = 6 + 22/3 = 而 = 乙／\'
     玉l9



                             b y




                1考：0, 吐 =8V.
           咨* VA- 10




           小2111升印，],                 畦= 12V,
                  L\      "I 3J
           Therefore, v八= 1v乂 +v{ =8+ 12= 20V.
356                                                           Chapter 5



Chapter 5
且l    Circuit diagram




                                   百V




      Graph, with selected tree




      The fund카llental cut-set equations are

      i口 + ig = 0,

      mig+ i b + iC + 1f = 0,

      ig+ Ic - ib = 0,

      d + 1b - ig = 0.

      Va is known; hence use the last three equations. Thus
      -Vi,        Vh         V,.
      才＋言 + ; + 5 = 0,
      1노     I노        v',
      寸＋盲e言＝0,
                                                                                     357
Solutions for Supplementary Problems




      쁑＋쁨숑：0.
      Eliminate the link voltages Vg and vb:

       Vg =l5 HVc 1Vd+ Ve,

       Vb = V + Vd - ye.

       After substituting and multiplying all equations by 6, there results:

       6ve + 3Vd - 3ve = 0,

       -3vC - 3vd + 6v, = -30,

       3vC + 6vd - 3ve := 30.

       Solving for Vd giVeS
            Nd 中540 = 5v,
       Vd = 百 = 尸108

       VO = Vd = 5 V.

 끄     Circuit小agram




                                                                               (ZV
358                                                                                             Chapter 5




           Graph with selected tree and loop currents




      N야e that
       .   il   i a +ib +1c
      IC = 二m =       n     ) or
           J          3
                         lb
                                    ii = 3iC.
               'a+
                              and
      凡＝
                     2
      Now observe there are only two unknown loop currents; hence, sum around fundamental
      loops a and b:

      6 = 2ia + 1(ja + ib)

      6 = 4ib + 2(ia + ib) + 3ib + ia + ib

      Solving foria and 1b gives 1a = 2 A       and 1b = 0. It follows that iC = 1 A   and i1 = 3A..

꼬     Circuit diagram




                                                                          回／
             -              --U




Solutions for Supplementary Problems                                                                   359




      Graph with selected tree




                                       2 匠   +


                                       l
                                       小




      Note that there are only two unknown tree-branch voltages, namely vb and Ve. The fundamen-
      tal cut-set equations are

      ta + i f = 0,

      1f + 1, = 0,

      ig- iC = 0,

      ig+ d - tf = 0,

      ig+ ie - If = 0.

      Do not use the first, third, or the fourth equations to find vb and Ve because 1a' 1d' and iC cannot
      be expressed in terms of tree-branch voltages. Using equations (2) and (5) gives
      Vf . Vb   ,1
      == 十 근＝ = 0.'
      2 ' 1            '.
      v旦 . ye     Vf    ,,
      ＝于 十 H:1 口- =:= = U.
       2    1     乙

      Now eliminate the link voltages Vf and vg:

      Vf =       m Ve + Vb -      5,


      Vg = Ve + 10 - 6yb·
360                                                                                        Chapter 5




       Thus

           Vb 小 ye _5
                             +    VL. =        (I
                 2            "   '   i/




                                           %+=
                                             l             九2
                                                     V
           Ve + 10 - 6Vb              H
                                      e
                                                     1 b
                                                                      日 ＼q
                                                                             0
                                           e



                 2

      Therefore, Vb = V = 1 V.

흐d    Circuit小agram



                                                     3工2
                             /25V                               !，冗
                                                                                 }7』
                                                                                  4

      Graph with selected tree and ioop currents

                                               .1.                    z




                                                                                       4

      Note: Ic = 5ix = e 51a; hence sum around meshes a and b only.

      -125 + 3ia + 9(ia 小 'b) = 0,

      9(ib - i a) + 61b + 18(ib - q) = 0.

      It follows that

      l2ia- 9ib = 125,

      8lia + 33ib = 0,
                         A
                     프
           a

                 3
Solutions for Supplementary Problems                                                        361




            re, i = -- 끄 = -3.67 A.
      Theref。
                                3

 흐亞   Circuit diagram

                                                  2



                                              뇨
                                                              力끄－        3
                                                              戶人／


                           V
                                              J                          }
                                                                    L:
                                                                                   우
                                                                                       ‘"
                                                  4

       Graph 꿔ith selected tree

                                             t厦       小   +   似                了

                                                                         +\<
                                                          1 mJ
                                                          2              <
                                                          峰
                                                               =




                                             任              +
                                        +m
                                                               1




                                                          +


                                                               1
                                                                               H




       The fundamental cut-set equations are

       i1 + i4 + is + i 6 == 0,

       - i2 + i4 + is + io = 0,

       尸 13 + i 5 + i6 = a

       Using the equations (2) and (3) yields
       -V2 . V4 . V5   .  ,1
       =H 十 :   十 = --4 = U.
         >       u    >u            '
        -.-v3 . v5     .       '\
        1'了 十 而 -4 = U.
       Now eliminate the link voltages v4 and v5

       V4 = 20 - v2 and v5 = 20 - v2 - v3.
362                                                                               Chapter 5




      It fo표ows that
      -v,          20 - v,                20 - v, - v
              +        n,    .    e   +
          >            8U                     >U                      '
                                               戶:
      -                                                     =    4.
      -v    20- v, -vA
       '1 +     戶：   寸 = 4.
       10      >U         "
      from which

      -93v2 - 8v3 = 1340,

      - v2 - 6v3 = 180.

      Thus v2 = -12 V                      and v3 = -28 V. Also

      V4 = 20- v2 = 32 V,

      v5 = 20- v2 - v3 = 60 V,
      .       V4        -.
      14 =    面    =    0.       4 A,

      Therefore, i1 = -i4 - i5 - i6 = -0.4 - 1.2 + 4 = 2.4 A.

      끄5(2= v;/5 = 28.8 W                     (abs)

      P10Q = v/10 = 78.4 W                          Cabs)

      P2oQ = v二/80 = 12.8 W                         (abs)

        Q = v/50 = 72 W
      P5。                                     (abs)

      P20V = Vui1 = 20(2.4) = 48 W                              (abs)

      尸4A= V516 = 60(- 4) = -240 W                                        (del)




                                                                                        ,d止山1山m山
                                                                                        363
Solutions for Supplementary Problems




 互血    Circuit小agram
                                                           7   ／口




                                 1         FHLH/
                                                   22. V
                                                               \／尸




                                                           下
                                                           2
                             .




                                                                     三4白
                         ,       1＝
                                                               4
                                  1mHHHHHH1a1H
       Graph with selected tree and loop currents




       The fundamental loop current i b is known. So sum around loops a and c only.

        -22 + 6(ia - tb) + lOla = 0,

       2(ib + iC) + 屯c + 22 = 0.

       Nowi    = e jaardib = 中3·4i中 = 3·翁a. 1t10ll0 'St1U1t1a = -5A; ib = -l7A; andiC = 2A.

        V34 = 4iC + 6(ja - 'b) = 80 V.

        Thus,p3.41小 = -8아3·屯中） = -1360W.

        Therefore,p3.4j小(delivered) = 1360 W.
364                                                                 Chapter 5




끄     Circuit小agram

                                                 15目




      Graph with selected tree




                                  土




      The fundamental cut-set equations are

      ia + i d + i f = 0)

       f + d - ib - ie = 0)

      ie + i c - i f = 0.

      The unknown tree-branch voltages are vb and vC. Also note
                       V八   1'b       .   e Vb     1      . ,1 1,
      if= iSA;
                      了= 了；           ie = i1    ana Va = 끄J V.
Solutions for Supplementary Problems




      Thus Eqs. (2) and (3) become

           Vd-   Vb
      l> + 1:m e =:= eI H1=eI =ti.
       』                   nVb\
            I     乙     \ (1 /     "
            V.
      m==4. --1        S = 0.'
       -Vh
                   ‘   戶          ,,




       4 " 3               -.

      Eliminate the link voltage Vd, i.e., Vd = 10 - Vb and find Vb = v八 = 20 V and vC = 60 V. Now
      V1 = Vd - VC = 10 小 vb - vC = -70 V. Therefore,

      P1SA = 15(- 70) = -1050 W        and plsA(delivered) = 1050W.
366                                                                                 Chapter 6



Chapter 6
6.1   a) (v1 - Va)/20 + (v1 - vO)/100 = 0; therefore, vO = 6v1 - SVa.

            Va = 4, vb = v2 = v1 = 0 V, vO = 6(0) - 5(4) = -20 V, but -15 5 vO 5 15 V,
            therefore, vO = -15 V (saturated).

      b) Va= 2V,          Vb = V1 =   v2= 0, v。=6(0) -5 (2) = 小10V.

      c)    Va =2V,       Vb = V1 =   v2= 1V, v。=6(1) -5 (2) =-4V.

      d) Va = 1V,         Vb = V1 =   v2 = 2V, vO = 6(2) -5(1) = 7V.

      e) 6(1.6) - Sva = vO; therefore, Va = -1.08 V when vO = + 15 V.

            Va = 4.92 V when vO = -15 V; therefore -1.08 V 5 V口 5 4.92 V.


亘교    a)    VO = G邱R5)v5 = (- 中아10)(2.5) = -10 V.

      b) iO + (vO/5) + (vO/40) = 0; therefore, iO = 2.25 mA.

亘쿄    a) v1= v2 =3V, (v1/40) + (vi- vO)/80 = 0, vO =9V.

      b) Noninverting.


            쁘 뉵
亘포    a)                         -300.0凹 + 0.05                                 =
                   0.01[1
                   0.0l[l++ 3어）
                            300,000
                               ，以）0+ 0.01]
                                     0.0l] +[l+
                                            [1 + 0．
                                                 0.002]
                                                   어） +0.05
                                                        0.05 =      少J.9t> .



      비 0
            h
              = [RO + Rj)/(R。- ARf)]V。= [1o5/(3 x 10)](99.965) = 349.88 1uV.

           R1n = v31i5,     is = (v5 - v1)/1000,

           R1 = [v5/(v5 - v1)]1000 = 1000.35 Q.



      m 旬
           VO =卜邱民］V노 = -100v5,              v1 = 0,    1릭n = 1000Q.
 啞
            쁘匕
                                     -300,000 + 0.05
                    0.01[1 + 300,000 + 0.01 + 5] + 6(1 + 0.002) + 0.05

                  = -299,999.95/3006.1221 = -99.796.
Solutions for Supplement띠y Problems                                                                      367




      b) [(v1 - v5)/RJ] + [v1/R] + [(v1 - vO)/R4 = 0,

                v1[1 + (11500) + (1/100)] = v + (vO/100),

                506v1 = 500v5 + 5(- 99.796v5); therefore, v1 = 2.012 mW.

           c)
                Rin=卜5/(v5 - v1)]1000 = 1002.02 (2.

       d) vO = -100v5,               V1 = 0,     R1ll1000c2.

亘血    a) Vt = VO,

                VO                         -5000 + (200/50)                        . m.
                     = ,d .戶n. . = ' 戶八八，,   八nn ,m八1' r』 ' 』 .=n1 .1,,n .日，,. = -41.4tx
                1눙     (.[/DU) [1 十 >uuU 十 2UO／乙UI 十 [I 十 i/ 2UJ 十 (2UU/:)U)            '


                therefore, Vt = -47.46 vs. To find the Th6venin resistance, we apply a test voltage source
                at the output terminals with the independent source deactivated, as shown in the figure.
                                                   So kj.


                                        1 kJL               aOOKJ1m


                                                            gOOO (-vi)




                iT = VT/ES0 + (20/21)] + [VT + 5000v1]/200 mA.

                V1 = [v7(21)/1070][20/21] = (2/l07)VT. Solving for the ratio VT/iT gives R 斗 2.033 kQ.

      b) ROUt = R = 2.033 k(2.

      c)        Write the node-voltage equations at the input and output nodes to get

                [(V1 中 v5)/1] + [V1/20J + [(V1 - VO)/50] = 0,

                [vO/2] + [VO + 500th'1]/200 + [VO - Vi]/50 = 0.

                Solving for VJ[ yields v1 = 0.4947v5. Now find i5; thus i = (V5 - v1)/1000 and

                R1ll = V5/i5 = 10007(1 - 0.4947) = 1978.84 C.

亘그    a) Replacing the op-amp with its equivalent circuit gives the circuit shown in the figure.
368                                                                                            Chapter 6




          Writing the node-voltage equations at nodesx andy gives

          [v1/4이 + [(v1 - vg)/500] + [(v1 - vO)/80] = 0,

          [v。
            /4] + [(v。- v1)/80] + [(v。
                                     /5) - 2 x 104(v2 - v1)/5] = 0.

          Also note that (v2 - v1) = O.8(vg 中 v1). Solve these equations for Vo/Vg = 2.9986.

      b) From the equations derived in (a), v1 = O.9996Vg = 0.9996 V and V2 = O.9999Vg
         = 0.9999 V.

      c) From (b) it follows that v1 - v2 = 343.59,uV.

      d) i = (v - v2)/10> = 858.99 pA

      e) v1 = v2 = Vg,      [vgl40] + L(vg - vO)/80] = 0; therefore, (vo/vg) = 3

          v1= v2= 1V,           v2- v1= 0,    i5= 0.

亘흐    a) From the circuit in the figure for the problem, we have

          V2 = R4v叭凡 + 凡） = v1 and

          [(1/R1) + (1/R2)]v1 - (11R2)v。= (1/Ri)va.

          Solving for v。gives

          VO = [(R1 + 凡）仄dyl- (R2／사）Va

          [(R1 + R2)R41R1(R3R4)]vb - (RilRi)va.

      b) If R3 = R1 andR2 = R4,        V。= (RilRl)EVb - Va].
Solutions for Supplementary Problems                                                              369




亘은    From the circuit shown with the problem, (Rc + RD) = 4500 Q,

      V2 = LRril(Rc + RD)]vb = v1, and (v1 - va)/1S00 + (v1 - VO)/RB = 0.

      Solving for vO gives



           IRn        1          1R。1      IRn       11 Rrs         1      1R。1
      "" '[i3而 " ] "' 小列 "" '[i3面 "] L(R小D)J "" [i3茄］""'

      The specifications required that the coefficient of vb and Va must each equal 8, therefore RB =
      8(1500) = 12 k(2 and 9RD/4SOO = 8, or RD = 4 kQ. It follows directly that Rc = 500 (2.

丘1Q




                             M
                 3
          i1 =   而
          .  5- 3        .
                  =U'U> m八
          i2= 40

          i3= il - i2 =: o.25 mA,

         V02 = 2位3 + 3 = 7 V,




口
370                                Chapter 6




       .   5- 7
                = eU'l m八
       '4 = 20

       i5 =14 + i 2 = m0.05 nlA,

      v01 = 5 + 1아5 = 4.5 V.
II口

 Solutions for Supplementary Problems                                                                                    371




 Chapter 7
  Z4 a)          00
            1i
                      I 드 0;    i = 5叱 0 5 I 5 = 0.005 s;
                                =
                                 )
                                                                                      i = 0.5 - 5此 0.005 드 I 5 0.01 s;
            1i
                      t 之 0.0ls =
                                 }




        b) v = 乙玎叱therefore,

           y= 0, t < 0.    v = 1 V,      0 < t < 0.005 s; v = -1 V, 0.005 <t < 0.01 s;
           v= 0. t> 0.0ls.    p= vi: therefore.p= 0. t< 0·.     p= 50t. 0< t< 0.005s;
           p = -0.5 + S0t, 0.005 < t "< 0.01 s; " ' p =0,  t > 0.01 s. w = 0.5Li2; therefore,

            w= 0, (< 0;         w = 2512,                          0 드 t 5 0.005 s;

            w = 25(乙 - 0.5t + 2.5 x l0 s,                           0.005 5 I 5 0.01 s;

            w= 0,        t 之0.0ls

  Z교    v= Ldildt= -300e H나sin500tV,

        dv/dt = -300eeZ> t[500cos500t - 25osin500l];

        dv/dt = 0 when tan500 = 2;

        the first peak occurs when I = 2214.3 1us,

        v(2214.3 4us) = -154.26 V; therefore, Iy7Z1nt1 = 154.26 V.

  7.3   i (0) = B1 = 4A,       竺，'. (0) =프．= 0.8B2 - 0.6B1; therefore,B2 = 5
                                    I                        It)


        and i = [4cos0.& + 5sin0.&le_U"& A,

        y = L16cos0.&
            [l6C0S0.81 -m 62Sin0.81]e
                          62sin0.&]e -0.61 V,                       i (4) = -388.73 mA,

        v(4) = - 1.121 V,     p(4) 프 435.65 mW (absorbing).

 14 v,(5Ms) =。.4x1。
                  6f5.-<10 '5dt+ 6= 1。+6= 16V,
                                .       n   .   .   .   n1   6

        %(l0/iS)
        i'c(10us) = 0.4 x
                        >: 10
                           l06 J.-IU x.,-6
                                        ju - 741+ 16 = -4 + 16 = 12V,




                                                                                                                         371
372                                                                                                                                                                                         Chapter 7




      v
      , ,   (2。
            (20/    us) ='S)                       。.4
                                                   0.    4X
                                                          X l06
                                                            1。 J2,0八x.10
                                                                     iv
                                                                         6         f                       -   2d + 16中 12 + 16 = 4 V,


                                                                                       二U 八 'U



7.5   a)                            1.         . .       .
-      ' V                        = - (area unuer i vs. t)
                                        c




                                      = 2 x 106[2 나 (5 x 10_6)(0.1) + 15 x 10e6(0.1)] = 4 V,

                    才
                                  =    {     Cv2
                                                                  =    {    (0.    5 x 10_            6)   (16)   =            41uJ.
                   q
      b)                          = area under i vs. t

                                  = f (5 X 10_6)(0.1) + (15 - 5)10_6(0.1) = 1.25 uC.

      c) @t = 231us,

                   q              = [2 - f (2 x 0.4 x 0.1)110-6= 1.96 uc,                                                                                               v = qIC = 3.92 V.

 血    a) Reduce the original inductors to an equivalent inductor of 10 H carrying an initial current
         of 5 A. Then


                   i3   (t)       =          -           솖.             t          2 fj_ 4xth + 5 =                                    5e'    4A,                   t     0.

      b) Calculate the voltage across the 6 H inductor:

                                                              di                   - - _d,
                                                                                                               t 之 0.
                   V6H=                小才＝                                        120e     " '   V,
                   Therefore, voltage across paralleled inductors is

                   V511 = 200匕141- 120匕놔4: = 80匕-4:                                                                               V,
                                                                                                                                                      t 之 0.

                   It follows that

                   ii(t) = -4 11 80eH4dx + 5 = (4ee4i+ 1) A.                                                                                                              t 之0.
                             >yU
                              "                                                                                       S                                    -




                                                                       4
                                                                       1
                                                                       1m
                                                              l
       c)          b(r)
                   :2   (t)       -          -           +.
                                                              而
                                                                      r .         80e4 dr + 0 =                           (e                 4:   -   1)       A,         t之 0.
Solutions for Supplementary Problems                                                                                                                          373




                                                      +              l
                                                                     H2
      d) 叩（0) 나 ' 5                                                                      52 = 137.5 J.
                                                        ）
                                                  <                             /
                                                        日
                                                  U                             0
      e)/ Pb。
          j7bO,x= y.
                  v。
                   13   lOOOe
                   i3 = lmm-&                                                            Wbox =               J:    i어)Oe      ‘缸m=              125 J.
                                    l                            J
                                                                                                                   加    2
                                                                                                                        l              m
                         l
                         12                                                                            l
                                                                                                       m2
                                    夕                                                     加
                                              )
                                                                 2                         =
                                                                                                                               크
                                                                                                                                            J,   w6= OJ.
                                                                                          叩1
                                                                 <
      f)        w5=
                                              H
                                                                 U
 2교 札ci＝ 上； 1어蚣뇨= 125(1 -戶）,

      Wdel(O.1S) = 125(1 - em1'2) 브 8735 J.

      Percent delivered = (87.35/125)100 = 69.88%.

 7旦   a) Reduce the original capacitors to an equivalent capacitance of 8 uF with an initial voltage
         of 40 V. Then

                                d 』而
                          lu I.'
                VO =    e 二；H J 1\                    3.2 x 10e3eHl0rdr
                                                                e    dr+ 40 = 40e
                                                                              吼匕小lmV
                                                                                   V,                                                                r 之 o.
                           o -u


      b)                        1n6 ,
                                工U
                                                      3.2 x 1013eU1伽dr + 25 = (8eU1m + 17) V, t 之 0.
                                        j '
                Vi =    - 11 I
                           44.
                             ) 'J 0


      c) v2(t) = vO(t) - v1(t) = (32e_10t 卞 17) v,

                                 _&cdvi          -inf
                ii (t) = -24 X 10 '- 1.- = 1.92e
       d)
                   ''               at


      ") 12(t) = -16《1丁畔뇨1.28戶）mA,
                       Ut

  끄             旬                   게     巧                      l
                                                                 42                 (25)2 + {                      (15)2
                        111m1
                    叩
                                                  )
                                                             +                                                                        13,625pJ.
                                                  e
                                                                     (16)                              (10)
                                                                                                                           =




            1
            b
                    竹    l
                         U2
                                    겨         l       AJM/           e
                                                                     l2     ·
                                                                                16   ·
                                                                                         172
                                                                                                   +   { 10 172·    ·          =       7,   225자J.

                    砥
                        = w, 尸 wj = 13,625 - 7,225 = 6,400 1uJ.

      d) Percent delivered = (6.4/13.625)· 100 = 46.97%.

       e)
                叩 = 128r1 ／枷公mJ = 6.4(1 - em20') mJ.
                                -   U                                                          .
374                                                       Chapter 7




      w(40 ms) = 6.4(1 - e10"8) 브 3.52 mJ;

      therefore % wdel(40 ms) = (3.5216.4)100 = 55.07%.
Solutions for Supplementary Problems                                                                                        375



Chapter 8
84     a) v(0) = 240 := i (0)R = 8R; therefore, R = 30 (.

      b) v = H乙刃／di = 160比e小20t; therefore, 1印山, L = 1.5 H.

      c) i= 1J20= 50ms.

      d) w(0) = O.5(i.5)(8)2 = 48J.


      『)
                 w
                     (diss)
                                        =   f1
                                                      (30)
                                                                 64e   "40
                                                                             ' dl = 47.12 J.


蚤귿    For t < 0, fmd the Thevenin equivalent w.r.t. the inductor terminals. V = 30 V, Ri = 5 Q.


      ij   (O'
                     )        =   -꼼
                                            =    -6
                                                             A
      'L(O+) = -6A



                                                                                                      1
                                                                                                      LL   (D)
                 Fort > 0, see the second figure.
                                                                             佃幼n.


                                                                                                                 三qo-j7-




                                       訃텍署아＝40Q; theref야.!= 0.4／和 =0.01S.
                  qe
                 R

                 l/T = 100; therefore i = 可lakA,                                           I 之 0.


                 %=4；旨) 可'띠= 236.2珂'田v,                                                             I 之0




                                                                                                                           375
376                                                                                                                          Chapter 8




8쿄    a)   p5Q = 5i三 = 4500e 어yw,                                               叩SQ=      J:              45me_5어ydt= 9 J,
                        1 ／尸八 ' . m 八-3' ／』＼』＼』＼\ 八八 1n 1
                   Wi = 弘그乙 >( LU      )(八天-I) = 乙工'Hi J.


          Percent 小ssipated in 5 ) = (9/23.4) x 100 = 38.46%.
                    2
      ..          VO   d . . ,, -to뇽.1.            戶m J . . ,. -coot
                                        ' W.Ar = fn   144伽 J小戶 dt = 2.R8J.
         r斗J.C         - - - -- V小戶 W
      b) flAnQ = 亡 = 1440
                  4.0                ' " " .t,fl1 J 0 - - m!         h' ---甘 -
              Percent dissipated in 40 c = (2.88/23.40)100 = 12.31%.
                       2
      .)
      c)   Pl0Q=
           P1QQ             =        VO         =   5760e   "5어       'W, W1。
                                                                            Q =      f:              5760e'5여'dt = 11.52J.

              Percent dissipated in 10 c = (11.52/23.40)100 = 49.23%.

                   Check:                       38.46 + 12.31 + 49.23 = 100%.


  포   a) Fort< 0,


            如(0         "       )=        (藎)        （和）          ＝   加A；
                                                                       A;【h0
                                                                          therefore
                                                                            「   「. 71.
                                                                              0fb   'i。         (.
                                                                                                (O    +   )＝   加A.

              i40(0m) = i4。
                          (0+) = 0.

                                                                                               그O J '



                                                                      a5=            :.8O小．
                                                                       A
                                                                      a{
      For t > 0,




                                          朴，           .                   ?
            Leq = (10)(40)/50 = 8 mH,                                           i (0) = 20 + 0 = 20 A,

               T= (8/4)1013 = 2 ms,                                         lit = 500,
                                                                                                                                               m1



Solutions for Supplementary Problems                                                                                                                377



           therefore i(t) = 20e15어i A,                                                                       t之 0.

      b) The energy dissipated in千（2 resistor equals the energy stored in the eq出valent inductor:
                岫
                m      =          {         (8
                                                   x
                                                         10_
                                                                   3)
                                                                        (20)2    =    1.    6 J.

 쵸亞   a) Fort < 0, i = 0 A, IL(0) = 20 A. Fort > 0, fmd the Th6venin equivalent w.r.t. the
         terminals of the inductor:


           놔＝     0,         凡＝                    2瑜毗                   『ef야er＝                              響／         io '
                                                                                                                           "     :   4邱·
           hr = 250; therefore, iL(t) = 20em20t A,                                                                              I 之 0.




                                                                                                                                           나
                                                                                                             .-LL    (O4) = 그 OA
                                                                                 1
                                                                                 1中뇨


                                                                                           1 d 1 1 r 1 1 1
                                                                                 +丘
                                                                                                 卜O口r,              d4




      b)   也＝          L穹＝                               -500e25                 V,
      c) i中 = mi .
      C)        :L=:= 15e
                      -5e -25w A,

 邑亘

      a) p凹（2＝ 텨y旨＝15以km5여yW，叩凹Q= Jm, 15毗-5o꺄＝3 J;
           WStOltd =                             글 (0.1)(400) = 20 J;

            therefore % dissipated in 60 Q = 15%.



      b)   , 加,        ＝          字＝
                                        w
                                                    =    (60i中，
                                                                  日J
                                                                        )'   =   45毗．5咐w,

           叩20Q=                       J:                45毗’S어y과＝ 9 J;

            therefore % dissipated in 20 Q = 45%.

      .) p4往中 = -401.夕L = 的00e'5어yw.
378                                                                                                                                  Chapter 8




且Z     a) Fort< 0,

                                                      q kJ11                          S MJL.

                                                                 +            -         (          4

                                    40V
                                             )                  뇨（0')                           吃佃'): 1{ kJL
                                                                 1



           .   90       .
           2 = =:= = D mA.                   v3(0 ) = 5(9) = 45 V,                              v6(0 )=5 (4) =20V.
               18         '
           恥rt > 0,

                                                          5kJt口                                        5kJt
                                       Hmm小사／              1
                                                                         +             4
                                    +                -卜    1e        '




                                LIS 二；< 3J4F                    그0 =;=            '     V口


                                     기                                   -        14F




           T= (5 x 103)(2x 10                       ) = lOms,                lit = 100,

           吻 =25e小1여iV,                      t之0; therefore i , =See1어)tmA,                                  t之0.

                               d如                                                                  附                    汕
                    迂
                                                                                                               V                %=
                                                                                                                                +
                                                                                                         墮
                                                                                            篁
                                    5 >< 10
                                                                                                                            e
      b)
                                         l0-3e -1어뇨dr + 20 =                                                        t           1




                    6
                                                                                                         3
                                                                                            3
      c) 叩尸拍）(45)2+ {(6)(20）乙4237.5싸
           Wdj. =       f (25)2
                         (2)
                                        =   625肛J,

           WtrapPed = 4237.5 - 625 = 3612.5pJ.

蚤量    a) 恥rt <0,

           v,(0) = v,(0+) = 끅三 x 80 = b0Oy. I-'人J


           For t > 0, fmd the Th6venin equivalent w.r.t. the capacitor terminals: V = 0, R = 40 kQ.
           (See the figure.)
           r = RC = (44) x 103)(0.5 x 10                        )

            = 20 ms.
               I.
Solutions for Supplementary Problems                                                                                379




                     lit = 50; therefore v = iQ匕15아 V,                                  t > 0.




          b)
                      V小            크』노-4       V功 -vc            -' -.       '.        -八       =/             八
                     瓦KO e 上（J V中 十 ii능而i6= u; tneretore zuv中 - b0y中 十 邱 - vc = U,
                     5邱 = V口                 邱 = 20匕’S位v,                  t 之 0.

晏으        a)                    2
                    P8＝ 石無＝0.05e 1어)tW,
                           어八flu
                                                                      叩8= I的
                                                                           . 0.05e叫1어ydt= 0.5 mJ,
                                                                                   1J



                     Wi 카邸 x 可如叫2 = 2.5 mJ;
                    therefore, percent dissipated in 8 kQ = (0.5/2.5) x 100 = 20%.

      b) Let vd equal I:he voltage across the 160 kQ resistor. Then

                    Vd = vc - 邱 = 卽／抑VI
                                    2
                    P，印：몲>< io =0·旽"떠
                    Wi60= f:                 p160d卜0.4毗
                    percent dissipated in 160 kQ resistor = 16%.

                                                                l어y
                    Pd =             10 4v中 =         16e
                                        "'



                           Vd                                         W,                         p杉t = 1.6mJ;
                                                            "
     c)
                                ·
                                                                              Wd =
                                                 0.
                                                                                          f0
                    percent dissipated in the dependent source = 64%.

                    Check: 20 + 16 + 64 = 100%.

JQ a) i (0) = i (0+') = -5 A. Fort > 0, the Th6venin equivalent circuit w.r.t. the 2 H inductor
      isvr = 180VandR1= 22;

                    therefore, r = L/R = 2/20 = 0.1 s and i (oo) = 180/20 = 9 A. Thus

                    i (t) = 9 - 14eHiOtA, t之 0+.
38m1                                                                                                            Chapter 8




                d 』八』
                   ＼  d 八. Jm八 . 4 』，,\ -1（노 1 ,                     』 = n+
       D)   V ==1d(J- L1 = ／乙 十 I이妃          v,                     r =u


       c)
            'S = i + i羽Q = i + v/30 = 11.4 - 8.4e小101人                                t 之 0+.

 晏꾜 i (0) = i (0+) = 40/8 = 5A. Fort > 0+,thecfrcuitsimplifiestoi(oo) = -24/12 = -2A,
    r = LiR = 24/12 = 2 ms, lit = 500. (See figure.)



                                                a4V



       i = -2
           m2 + [5 -e (-           [-2 + 7e1500]A,
                      (H2)]e -5여1 =卜2                                             rt 之 0 +

旦끄 i (0) = i (O+) = 40/5 = 8 A,                     r = 4/20 = 1/5 s,

       i (oo) = 40/20 = 2 A,            i = 2 + (8 - 2)e_St A,                    I 之 0+,

       V = L(di/dt) = 4(- 枷小 = -12t匕e身V,                                r 之 0+.

 昱1크 For t < 0, let v1 be the voltage across the 8 Q - iA branch, positive at the top of the branch.
     Then
               l
               y           4   l
                               y       A
                                                                 V1 = 14 V                              +
                                       1
                                       i
                       n
                   1               m
                                            브
                   6               8                0
                       /
                                                =
                                            2
                                                                 iL(O) = 14/2= 7A
               . v1 - 74
              i八＝ 6                                              (current left-to-right
                                                                 in the 2.6-H inductor)
       For I > 0, find the Thevenin equivalent with respect to the terminals of the 2.6-H inductor
       when the switch is closed.

       vt = 52V. R, = 5.2c: thereforeir.n스i = 10A.                               r = 2.6/52 = 0.5s. Thusi, ==
       1』N   m e2r . '             n"                   " " H'          -                                -
       it) - 韶     /\}         I 之 U.
                                                                            2. 6 14




                                           兵/
                           1

Solutions for Supplementary Problems                                                                 381




      v1 (t)
                =   刀L+ 2,  6字
                                  山小e            2' + 2.
                                                       6
                                                           (6e
                                                                              )
                =20+ 9.6eH2tV,           t 之0.

量고또 a) v (0) = v (0+ ) = 0. Find the Th6venin equivalent w.r.t. the terminals of the capacitor.
       We get v1 = 200 V,R = 16kQ;

               thereforet = (16 x 10)(50 x 10-6) = 0.8 s, voo) = 100 V.

               And thus v, = (1凹- ic町匕m1.2St) v ,                     t之0+

      b) i = Cdv,/dr = 6.25eHl"25imA,                 ( =u
                                                                 11   +
                                                                          ;
                          1r기n   d 八戶     d 八尸 -1.25t  1                      . ' 』m+
               i80kQ = vC／亡乂J == I·乙：) ＝느 I· 二：玘      mA,                     ( = U ;

               q= i c + 180kQ = 1.25 + 5e_1'251mA,                        t 之 0+.


量꼬 v (0) = v.(0+) = (9/12)(- 60) = -45V.Fort > 0+,thecircuitreducestoT = (15 x io3)
   [(2/3) x 10-6] = 10 ms, vc(끼 = 75 V; therefore

      vc = 75 + (- 45 小 75)em1以y = [75 - 120e卞1以y]V,                                I 之 0+.
                                                           1S k_


                                                                                        V



量교亘 a) First replace the circuit to the left of the switch with its Thevenin equivalent; thus J' =
       6VandR1= 1200Q.

               i(0) = 0Aandi(0+ ) = 6/2000 = 3mA.

     b) i（的） = OA.

      c) r = (20炚2 x lo_6) = 4 x 10H3 = 4ms.

     d) i (t) = 0 + (:3 - 0)em25 ' mA = 3em25m mA,                                t 之 0+.

     e) v = 6 - (1.2)(3)eH25侄 = 6 - 3.6ee250 V, t 之 0+.
382                                                                                       Chapter 8




꾜Z  F0:i
 fl F。rt <0, v
             ,,(0H)
                (0) =-300
                       ,,.., 60 = -1凹 V = v (0+).
                      1八J



      For t > 0, fmd the Th6venin equivalent w.r.t. the terminals of the capacitor: J' = 160 V,
      R = 16 kQ; therefore,

      T= (0.25 x 10巾6)(16 x iO3) = 4ms,           h/r = 250.

      vco = 1; = 160V;

                     （刃- 34C匕-25但v,
      therefore v, = 1                          r之0.

毖1晏 v (0) = v (0+ ) = 0. With the switch open, find the Thevenin equivalent w.r.t. the terminals
    of the capacitor. We get

      Vt = 25 V andRt = 20 Q. Therefore, v (oo) = 25 V and

      T= 20(500) x i0H6 = 10ms. Thus, v = 2S- 25eH1어노 V, r 之 01+.

量42 a) 91 118 = 6c; therefore, i(0) = i (0+) = 10(6)115 = 4A.

      b) 0 + 5 t 5 10 ms:       61 118 = 4.5 Q, r = 0.27/135 = 0.02 s,

           i = 4emSOt A; therefore, i (8 ms) = 4e -0.4 = 2.68 A.

      c)
           lOms 5 t 5 m:       i (10 ms) = 4e -03 = 2.43 A,

           r = 0.27/9 = 0.03S, i = 2.43e-(t - O.01)(100/3) A,

           1(16 ms) = 2.43em0"2 = 1.99 A.

           v(10) = 0.27[d(4em501)/dt]t - 1。ms = m54eU03 = -32.75 V

           v(10+) = 0.27[d2.43eUl凹（r -0"01)'3Idt]i = 1。ms = -21.84 V


           恥rt(0: 116k2=（喘伊＝5毗
           v (0) = VC(0+) = (s)(16) = 80V.

           For 0 5 t 5 8 ms (see the figure):

           r = (50)(0.2)1043 = 10 ms,
                                                                                          m小小




Solutions for Supplementary Problems                                                              383



           h/r = 100,

           v (t) = 朗匕-1여i V,

           0 5 t 5 8ms.


                                          +


                                         t智


      b) 8 ms 5 r 5 oo (see the figure):                  v (0.008) = 80匕-0.8 = 35.95 V
                                                         Ic KJL
                        4
                                              4
                        '4   a,
                                  .s.   Vqs:  -




                                                         WJ



          Req = 10 + 15 [(25)(37.5)/(625)J = 40 kQ,

          t = (40)(0.2)10小3 = 8 ms,                    工／r = 125,

          y,=35.95e"l25(i - 0.008) v,                  0.008 5 r 5 00.

&2j, :Find the Tbevenin equivalent w.r.t. the terminals of the 50-mH inductor. Thus, Vt = 120 V and
     R = -2 (2. The circuit becomes as shown in the figure. The differential equation that de-
     scribes this circuit is -120 - 2i + 0.05玄/dt = 0. Senaratin으 variables uives Fdi/(60 + fli = 40
       . - .    ..   1 .1 . 1    . 11
     at. mt昭ratmg 1)Oth sides 弘elcis:. =卜wr ,.,1 . /,1 40t      . :+
                                                 十 oue JA, r 之 (1 ' ;
                                                                            느7


      V = Ldildz = 120e10'V, t 之 01 ; V = 12,000 whent = 115.l3ms




                                                  1甲
384                                                                                                                                           Chapter 9



Chapter 9
                                                        l
                                                        12
                                                      기이J
                                                                                                                   l

gl    了1 牛 m口 +                                   m                                                                      = -45;
                                                                  <
                                                                           s2=
                                    =
                                    e


                                                                                                                   '
                                        12
                                                                                        -a-
                                                                  U
                                                                                               [a2_          w三]   "
      毗比for.                  伽：                －乳           .=       25：        赤，           and     R= 8Q.
      v(0+) = 50- 卯1 = -40V; therefore,iR(0) = -S人

         (0+ ) = 2.5 x 10U3 [-250 + 的5이 = 9.5人
      k'c(O

      iL(O+) = -9.5 + 5 = 4.5A.

2교    a) 口O = 5 )< 10干, 口 = 口J, = (L끼？C), thereforeR = 12.5 kQ.
                                                 A2Jeem,
      b) v(t) = [A1t +                                                v(0+) = A2 = 5,

               IR(O+) = v(0+)/R = 5/12.5 = 0.4 m人                                              iL(O+) = -0.4 m人

               ic(0+ ) = - ['R(O+ ) + IL(O+ )] = 0; therefore, [dv(0 + )/dt] = 0.

               [dv/dt] = [t4i - A1at - qd2Jemm. ThusA1 - 口42 = 0;

               A1                            2 = 23 x i06,                            5 x 106t+ 5)                       'V,      t之 0+
                                                                                                      ee5m         '여X
                       =
                               口4                                     v=
                                                                           (2.                                                            .




      c) t(us) v(t)




                d l2345678
                         9m
                                                 5.0
                                                 4.55
                                                 3.68
                                                 2.79
                                                 2.03
                                                 1.44
                                                 1.00
                                                 0.68
                                                 0.46
                                                 031
                                                 0.20
                                                                              mm小




Solutions for Supplementary Problems                                                385




      d) w(0 ) = 0.5qv(O十)]二 + 0.5L[iL(0十)]t = 5nJ,

          jR(5/is) = v(5us)/R = 140匕

          ic(5,4s) = C[dv(5,us)/dt} = -500e 乙 '4uA,
          包（5/iS) = -EiR(S1us) + ic(5i{s)] = -900e123uA.
          Therefore, w(5 dus) = 0.5(80 X 10H12)(17.5ee2"5)2

          + 0.5(50 x 10m3)(900 x 10e6e小2"5)2 = 32.5e寸5 nJ.
          Percent = [32.5e15/5J100 쓰 4.38%.

2쿄    a) 口
         a = (l/2RC
             (1/2RC') =30
                       30,,      nJ2
                                 w。= 1/LC = 2500,           o。= 50,

          underdamped,       Wd = v9i666 = 40 rad/s,

         iL = I／比 + D1e
                    』DleU口iC0Sn
                         at cos wdt
                                 Jdr + i)2e
                                       D2e -at sin Wdt,

          wC(0) = 156.3 x 10e6 = 0.5C[v(0+)]2; therefore, v(0+) = 9.6 V.

         'R(O+) = v(0+)/R = 1.92 mA,         iL(0+) = 0 = 1k + D1,

          therefore, D1 = -4 mA,       L[diL(0+)/dtJ = v (0+) = 9.6 V.

         [dL(0+ )/dt] = wdD2 - aD1 = 9.6/120 = 80 mA/s,

         therefore, 40D2 - 30(- 4) = 80,      D2 = -1 mA,
         iL = 4 - eH3m [4 cos 401 + sin 401] mA,       t之0+.

     b) [diL/dt] = e "3m [190 sin 40t + 80 cos 401] mA/s,      (djL/dt) = 0
         when tan 40' = -8/19; therefore the first peak occurs

         when 401 = 2.74 rad, or t = 68.58 ms,
386                                                                                                                                    Chapter 9




            iL(ma지 = IL(0.06858) = 4.42 mA.

      c) t= 68.58ms.

으냔    a) Au = 0+,thecircuitbecomesasshowninthefigure.
                                                                                       o.as.
                                                                                       十＋                  'I.
                         300 mA ID        그OO. n.                                                                      tH i



                  L
                         呼
            y                                                       =


                                 0; therefo比，                       and th出，

                      鈿
                                                              0,
                                                    字＝                                          (0k)               =
                            =                                                                                            0.
                                                                                       吻
                  0
                                      =0.8劣， 劣（0')＝뻗');
             吃
                                dVa                                 =


                                dt
      b)
                          쁘m                        Th出，
                  b                                                                                        +
             血                  0             104
                                                                                            )
                 e   e
                 e   r
                                          6/x 10 V/ Thus,                              +                           8 x 10
                                                                                                                       l0 V/
                                                                                                                              4
                                                                        dVa
                                      =
                                      =
                                                         s.
                                                         5.             -     -   (0
                                                                                  (0
                                                                                                       =
                                                                                                       =    418/
                                                                                                            4.
                                                                                                                                  s.
      C) 口＝ 1二＝ 500,
                 乙八I.-
                                          口2= 25 x 1o4,                        二卜 = 16/ l0'
                                                                              2w。
             2'   2.
            a > coo, tnus overaampeu;                    3i = -200 rad/s,

            S2 = 叫8어）rad/s,               'a（끼 = 0,

            y, (0 = 0 +A,le-20y +A ,2e -8어i,                             (0+) =A '1 +A '2 = 0,
                                                                        v。

             쁘m  (0k) = 小2oQ,4 ' - 8004 '2 = 4.8 x 1o4;

            therefore,A '1 = -A ' 乃             A '1 = 80,

            吻(t) = [80ee20(노- 80e 얹Xi] V,                          t之0.

으亞     a) a (R/2L) = 25,000,                w0 = VI兀乙 = 20,000,                                            overdainped,

            S1 = -10,000,             S2 = -40)000.

       b)   vV, = l5 d卞-iO,여0t+
                  15+ Aie    + , p e-40.凹0:,                            %(0+) = 0;
                                                                        v,
Solutions for Supplement缸y Problems                                                        387




            therefore, 15 + A '1 +A '2 = 0.

            [dv.(0+)/dt] = -10,000A '1 - 40,毗4'2 = 0;

            A '1 = -20 V andA '2 = 5 V. Thus,

            % = ［巧 -炬10 '어Xy + 可的'여Xl] V,                     t 之 0+.
                            ee10，여XUe
                                   - e -40'여)0t] mA.
      c) iL= iC= C(d以幻＝ 2.5[

 2亘   For t < 0 (see figure),
                                                         1 a S1Jm
                                                  1=1HHeW呻1


                                 30o. .n.                 so0JL                (   （丁）
                                                  +

                                                  v (O)



      i (0) = (137.5 小 37.5)18目 = 0.125A = i (0+),

      v (0) = 37.5 + 300(0.125) = 75V = vC(0+).

      恥rt :> 0,

                                            100       -
      125 I 1500 = 100 c,
                                   口 = 瓦而 = ＞내A) raws,
        2     1     尸n    d,,6         a2 = 25 x i06,         2   2
                                                             a c m0,        unoeraampeu,
      (00 = iZ = )U X IU,
      vC(的) = 137.5 V,          s1,2 = -5000 土 j5000 rad/s;
                                                     B;em5어0t
      therefore, v%(i)
      theref.Jre   (t) = 137.5
                         l37.5 + B1e
                                 Bie-5000COS
                                         cos.50001 + B2e      sin50町1,

      v (0+) = 137.5 + B1 = 75,             B1 = -62.5 V,

      C쁘 (0k) =K0*) = 0.125.                  쁘 (。
                                                 k) = 62.5。
                                                          。 V/s.
        口t ' "          "                  at "                "        "
      dvC . n+.                              .
      - -(0 ' ) = 500092,          B2 = -50V,
388                                                                                               Chapier 9




      %(r)
      v (t) = [l37.5
              [137.5 -H 62.5ee5어XyCOS
                                   0S50001 - 50eU5여Xy sin 50001]V,              1 之 0.


끄     %(0 ) = v
              %(0
                (O + ) = （明0/5（目）1000 = 呱）v,

          11 .八r  ／八 .，노, . ,\\ 4 n』
                                   ＼n   ／八n八         2   d .! Jm  m 八8           dr14
      a = 入／乙L == （乙'44J1'44J) I （大只J = 에 （八,,      wo = Ill乂／ == 'U )     (00 = 'U )

      underdamped, 0d= (w訃기"= 8q刃『a田5,
      v. = [B1- cos 80001 + B2 - sin 8000t]eH&XX ',            vc(0+) = B1 = 960V,

      [dv (o +)/dt] = 8어0B2卞 6000B1 = 0; therefore, B2- = 0.75B1- = 720 V.

      Thus, v. = [960 cos 8어걋 + 720 sin 8以） ee6000 v.
                                           01]
으旦    a) a = (R/2L) = 224.14 Np/s,               m0 = ii/ EC = 18,569.53 rad/s,

          underdamped,          wd = 18,568.18 rad/s.

          Thus, i = ij + [A 'l cosw/ + Al2wdt]e at,            i/ = 0.

          i (0) = i (0+) = 12/2.6 = 4.62A = A '1,            [di(0+)/dtJ = 0.

          Therefore, COdA '2 - q4 ' 2 = 0,         4   = (a/wd)A 'l = 55.71mA.

          vL
          VL = L(di/dr)
                    dt) = -m [LA lm自md]e-at sin COdl
                            [ia,'lwWwd]e

             = -497.1
               m497.l3e-22
                      3e   4.14t sin 18,568.181 V, 1 之 0+.

      b) (dvL/dt) = 0 when tan WdI = wd/a = 165.69;

          therefore, 口Jdt = 89.310 + n(180'),          n = 0,1,2.... .The first peak will yield
          vL(max), i.e., n = 0; therefore
          rmax = l.56/wd = 83.95 dus (89.31' 立 1.56 rad),
          v(83.95as) = -487.83 V,            I1JnlaX1 = 487.83 V
Solutions for Supplementary Problems                                                                        389




Chapter 10

i2     a) T = 8 - (- 2) = 10 ms,                       f = lIT = 200 Hz.

       b)   V = Vm COS (wt + 0),                    10 ms - 3600; therefore 2 ms - 72已

            0 = Vm COS (- 72 + 0),                     -72 + 0 = -90,       0 = -18,
            Vm = 80.9/ COS 18' = 85.06,                   V = 85.06 COS (200 Jrt - 18') V.


프묘     a) y = 100c0s (8어t + 120) + 60cos (800t- 1500),

            Y = 100LjO + 60 /                           = = -50 +j86.6 + (- 51.96 -j30)

                       = -101.96 + J56.60 = 116.62 Li흐（）으흐으； therefore

            y = 116.62 cos (800t + 150.96').

       b) y = 50 Cos (3刃t + 30) - 20sin(300t + 2100);

            therefore Y = 50 jQ - 20LJ2Q = 43.30 + j25.00 - (- 10.00 + J17.32)

                                        = 53.30 + j7.68 = 53.85 / 8.20. Thus,y = 53.85 cos (30甘 + 8.20').

10.3   Z1 = (5 -110) I I (4 + 122) = 16.67亡 -玉87으 = (13.33 - jlO) Q,

       Z2 = 101 120 = 20/3 = (6.67 + JO) Q,

       Zab = 40 +J55 + Z1+ Z2 = (60 +j45) Q or                           75/ 36.87c.

10.4
                            ，끊느搗.
                        乙而느措訊
       a)
            Zab

                                       &U2      .1 250w            sol
                            =                +/ 1          )       ;；기
                                25以）+w"
                                                               m




                                                 L2SOo+ w'         -1
                                        1=
            Zab is resistive when the f-term vanishes'
            therefore, w = 25 rad/s.


                 , .    =     = iQ.
            m=ab
                                 5呵＝
            '7
                  八尸nn . m戶2    + ==.'
                  2500 十 25日
            Let V = voltage across the impedance (3 + j4) (2, positive at the top node. Then
            V= (3 +J4)I = 9+ /12 = 15/ 53.13V. ThusI3 =V/(4- J3) =J3A,
3卯                                                                                         Chapter 10



             12= 6- 11- 13= 3- 13= 4.24 /                A,

             VS = (V- 212) = 9 +j12- 2(3- j3) = 3 +j18 = 18.25i80.54 V.

       b) i 2 = 4.24 cos (105t - 45.) A,      i3 = 3 cos (105t +이）.) A, and
             v = 18.25 cos (10t + 80.54.) V.

iQ亘          V4 =12+ j24

                  = 26.83 / 63.430 V

             z    = (V/L)
                  = 1.66/ 83.66" Q




                                                     十   ' 1b '    0뇨1
                                               !1/                I3    .


                                                                  그.Jt. :




             V    = (j5)(6) = j30 V,      V1 = 40 + j30 - j30 = 40 V,

             Ii   = 40/(8 -16) = (3.2 + j2.4) A,

             12   = 3.2 + j2.4 - 6 = (- 2.8 + j2.4) A,        V2 = 1012 = (- 28 +j24) V,
             V3 =V- V2= j30+ 28- j24= (28+ j6) V,
             13   = [(28 + j6)/(2 + j1)] = (12.4 - j3.2) A,
             14   = 13 - 12 = 12.4 - j3.2 - (- 2.8 + j2.4) = (15.2 - j5.6) A,
             10   = Il + 14 = 3.2 +j2.4 + 15.2- j5.6 = (18.4- 13.2) A

                  = 18.68 i- 9.870A.
10.7
                                                                   4山n=




                          I 8O/-3(.. 97
                                                                             V
                                 V


       (a)
                                                                                                   391
Solutions for Supplementary Problems



      After two source transmissions, the phasor-domain circuit shown in figure A reduces to the
      circuit shown in figure B.



                                                                             l
                                                                             1丁l
                                                                       +V


                                                        11二口弓1
                                                  口4
                                                                 百4
                                                                      t1重1
                                                  1

                                                   d
                                函
                                    A
                                        （士）
                                              l                         =




       (b)
       Combining the two current sources into a sin합e source and the para끄el branches into a single
       admittance (figure C) gives

                   I   = (- 24 小月2) A,

                   Y   = 0.15 / e 63.430 A,

                   V   = 'ly = 180亡二凶으）

                       = 180 cos (400 - 9()0) V.




                                                      (-.aq- 'a)
                                                            A
             (c)
10쿄          it follows directly from the circuit that

             15 = [V1/10] + [V2/2J + [(V1 巾 V2)I5]

             and

             0 = [玖- j2)J 4' [(V2 - 4V1)I50] + L('2 - V1)/5]. Solving for V2 gives V2 = V =
             (14 -j14) V = 19.80 /＝크巨으 V. App蜘띵 a test voltage sourc아아k ter씨n毗 a,b (a如r re-
             moving the independent current sources) gives the circuit shown.


                                                                      !SO.ii.


                                                                      汁14
                                                                                   S
392                                                                                                   Chapter 10



           Therefore, 'T = FVT/(-12)1 + [VT - 4V1)/5이 + [(VT - V1)/5]; also
           [V1/10J + EVT!21 + [(V1 - VT)!5] = 0. Thus, V1 = -VT and
           (IT/VT) = [1/(- j2)] + [5/50] + [215], and so
           Z = (VT/IT) = (1 -jl)           ) = \/i /       c.

1啞     The phasor＜如main equ如alent circuit is as shown in the fi目표e. The帥asor-doma血node volt-
       age equations are as follows:



                        aO
                        스8으'
                          V




                  -j2。心午"
      多而' 玆4)j20)+ Vi                                                    thus V1 = 23.06 /_-76.97 V

                                                                         th出V2 = 24.38 느里里 V
          +(1+ j2) -5/
       v1 = 23.06 cos (104t - 76.970)            v2 = 24.38 cos (104t - 63.42.) V.

lQ끄 Construct the phasor-domain circuit.

                                                 430o.




       400 = 13001A - 11001B + 501B,

       뇨나뇽， 兀= 501B
JQJ1 a) Let V1 be the node voltage across the 中j30- 2 capacitor, positive at the top node. Theii

            V1     V1- 220              Vi- VO                       ]
                                                                                     264-
           下6+ _ 1               + ' j10 '=0
                                                                     1   '   "   =            j明
           VO      VO
           二亡느 + H三：+
                           VO- V1
                               V . ",    4 = 0
                                                                     ]           = 268.33 /二
                                                                                 =
                                                                                       '33／
                                                                                           中10300 V
           IOU   -J) U          flU
Solutions for Supplementary Problems                                                                   393




       h) V0 la多 Vg by 10.30'.

1QJ_2 After transforming the 5-A current source and the子（2 resistor to a 15-V source in series with
      a 3-(2 resistor, the circuit reduces to a sin멤e mesh structure. From this circuit we have:
           V1 = Vab = [15(110)/(3 - i4)1 = 30느368.87 V and

           Zr= [(- jlO)(3 + j6)/(3 - i4)1 = 12 + j6 = 13.42 / 26.5工 Q;

           therefore, 'N = [(30 / -36.87 )/(13.24 /                   )] = 1 - j2 = 2.24 / -63.43 A,

           ZN = 乙．

끄꼬 a) Construct the phasor-domain circuit.




       V2=     -j105 , 1。
                        四으＝ (5mj5) V= V1,
             10V 小 jl0尸


       ,，寸"二＝「 口(崗                                              Vl;



        theref。
              re,        =   5 v' 느45
                                                        iuuJ
                                             -


                                        L
                                                 I無1.
                                        [1
                    VO
        ForVotolagVgby90', Rf= 100Q.

        b) WhenRf= IOOQ,

            VO = 5vi／二：쏘O(1 小I') = 10 /                        \/;

            therefore, vO = 10 cos (b（乂Ot - 90') V = 10 sin l000t V.
394                                                                    Chapter 11



Chapter 11
a'
           a) P = (1/2)(100)(10) cos (30' - 60') = 433.01 W (abs),

              Q = 500 sin (- 30) = -250 VAR (del).

      b) P = 500 cos (- 45' + 75') = 433.01 (abs),

              Q = 500 sin (30') = 250 VAR (abs).

              P = 500 cos (1350 + 185) = 383.02 W (abs),

              Q = 500 sin 3200 = -321.39 VAR (del).

              P = 500 cos (- 1600 + 45) = -211.31W (del),

              Q = 500 sin (- 115) = -453.15 VA之 (del).

              P = 500 cos (50' - 95) = 353.55 W (abs),

              Q = 500 sin (- 45) = -353.55 VAR      (del).

              P = [100/a 12,6.25 = 8刃 W;

              Q = {[100W ]2/(25/3)} = 600 VAR;

              thereforej)m카 = 800 + f8(n2 + 御02 = 1800 W.

      b) Pmin =800 m1000 = U200W;

              therefore, peak power absorbed by the source is 200 W.

      c)
              尸 == 800W.

      d) Q= 600VAR.

      e)
              Absorbs magnetizing VAR.

      O       s = 尸 + jQ = 800 + j600 = 1伉乂）／쪼世끄 VA;

              pf = cos 36.870 = 0.8.
Solutions for Supplementary Problems                                                  395




       g) if = sin 36.87 = 0.6.

fl 쿄   a) y = [1/10] + [1/(8 + j6)] + [1/(-i5)1 = (0.18 + jO.14) U,

            Z = 11Y = 4.39/ -37.8즈 Q. Let V = voltage across the parallel branches,
            positive at the top. Then

            V = I5,Z = (26 匹 )(4.39 / -37.87 ) = 114.02 /_-37.87 V (rms).

            S (delivered) = vI: = (2340 - j1820) VA.

       b) The source is delivering an average power of 2340 W.

       c)   The source is absorbing 1820 magnetizing VAR.

       d) Resistive branch: P = (114.02)2/10 = 1300 W.

            Inductive branch: 'L = [(114.02 / -37.87 )/(10 /        )]

            = 11．띠力      主'7뽀A(rms). Therefore, 尸I. = (11.4)28 = 1040W;

            QL = (11.4)2(6) = 780 VAR.

            Capacitive branch: Q = (114.02)2/(_5) = -2600 VAR.

       e)
                rbed = 1300 + 1040 = 2340 W,
            "abs。                                     Pdel = 2340 W.

       f)   Q(abs) = 1820 + 780 = 2600 VAR,           Q(del) = 2600 VAR.

끄d     Construct the phasor-domain equivalent circuit.
                                    4力O Jt.               -i '0On




                                              40I1그
       240 = 17201A HJ4001B       'B - 'A -    。r )
                                               0J


       Thus, 1B = 3 + j3 = 31 껸Z A,           尸40 = 1 (317 )2 (40) =3d) w.
396                                                                                                                                    Chapiter 11




d   J   戶    \   =1       r,       ,m   1   =        1   2      J   m   戶八n           d   m   nnn            戶八八

프교          a)   "Ioss = U·dt l 1                            = I乞：)U(J - I3M工J = >（久J;

                                    1   .       12             ／八戶            1   1       1         A尸   1          !         八尸   ．

                 inerelore 1 I I                             = 0乙：),          1 I 1 = 乙：) /\)                      1eff = 乙그 /＼·


            b)   III2RL = 13,以）0; therefore, RL = 20.80 Q,

                 XL = V2(2                               20.82 = 15.6c.

            c) 675 = 1 20.8 + j15.6 + 0.8 + jXj 1 (25); therefore, X1 = 0.60 Q.

            d)   -      675/ 0
                          +j16.2 = 25／二흐쁘工A (rms),
                 I = 21.6

                 Sg = -(675四)'                                      = -13,500 -jlo, 125;

                 therefore. O口 = 10.125 VAR (delivered).
                               "    mr      O                   "




끄亞          a) Let Vm = rms magnitude of the load voltage and I = phasor line current directed from
               the source toward the load. Then I = (480 - j360)/V, , and 120i0 = V.,, /00 + [(480 -
               1360)/VmI(l + j2). We reduce this expression to 120 Vm 世 = V,i + 120(J + jO(J(J;
               theref。re. 120 V. , c。s 0 = V + 1200 and 120 V.,, sin 9 = 600. N。       w find cos9 and sin9
                          2n       . 2 r.   m '        . _ r4   d八 n』..』.._.2 . 4 1. " mr\6   ._ i기 . .  . ir2
               and set c05  & +  sin - e  = 1 to generate V,1 卞 12,Ut乂1  Vm   + 1.8  X 1U   = U. Solving b0r Vm
                 gives 11,8姻.08 and 151.92; thus the two possible values of 1뇨 are 108.85 V (rms) and
                 12.33 V (rms). If Vm = 108.85 V, I = (4.41 - j3.31) A (rms) and 0 = 2.63'. If Vm =
                 12.33 V, I = (38.94 - j29.21) A (rms) and 0 = 23.93.

            b) The phasor-diagrams are

                                                                                                    LaoL旦 , 4
                                                                                                                        7如키工
                                                                                                                   1D8.55｛르
                                                                        vvI' = to已 8SL2 V


                                                                                  J媒之．,,,
                                                                        1a. 33／오
                                                                             'In.,                  好／立 V



iLi         a) V1 = 180四으（12/18) = 120四으V,

                 乙 = j3000 + [(12)(6)(1000)/18] = (4000 + J3000) Q,
Solutions for Supplementary Problems                                                         397




            ZL = (2（刃0 -. jl伉(力 (2;

            therefore, I = [(120四)I (6000 + j2000)] = 18.97! - 18.430 mA,

             11    /d .八. /d ,1 .. n 4 '1U3. 2／八n八n. 八 ／』＼
            I-' = (1/Z)(Ib.9I X IU ) (乙UJ(J) = .xu mw.


      b) Set X to -3000 Q if possible. For given range on C, the best we can do is set X =
                                                                   (1叫2 as poss似e·師ce
         - 2000 Q. (C 크므타 Now帥 as close to 1,1(4000)2 +
         V (4m0)2 + (1어0)2 = 4123.11 C2, setR = 4000 (2.

       c:) I = [(120 /Q으/(8000 + 11000)] = 14.88 /           mA;

            therefore, P =: (0.5)(14.88)2(4) = 443.08 mW, yes.

       d) pm., = [(112)(60)21(40刃)1 = 450 mW.

       e) RL = 4000 c, CL = [11(3000w)] = 0.06671uF.

       1)   Yes.

끄쿄     V口 = - (Z11Z)Vg, where＼노 = n으v,

       午      [_11061(50，以刃）(0.04) = 尸j500 Q,

       Z, = 羽 + j (0.8>< 10H3)(50,000) = (30 + j띠）) c;

       therefore VO = [j500I(30 + j40)](1L으) = 10/그6.87 V,

       P = (1/2)(10)2I50 = 1W.
 398                                                                                              Chapter 13



 Chapter 12
끄l          a) The single-phase equivalent circuit is shown below.

                     'aA
                             = [1201(16 + j12)] = 旬＝쪼윤즈 A,

                     'bB     = 6 /-156.87A,

                     'cC     = 6/ 83.130人

                     Vab     =（月쏘巴 Van,

                             = 207.85／끄 V.

       b)
                                                           O.a二             如·1兵 A 'S.S.r.




                 Vbc = 207.85/             ＼乙         VCa = 207.85그塑으V.

       c) VN = IaAZ中 = (4.8 - j3.6)(15.8 + jll. 2) = 116.20 /                                V,

               VBN = 116.20/＝끄亞竺V,                           "CN = 116.20d堡쪼으＼/.

       d) VB = (V互쏘巴뇨N = 201.27 L2크望＼/,

               VBC = 201.27/＝으1흐쓰V,                        "RCA = 201.27d塑크笙V,

12.2           'aA
                           = (4知／
                                ＼厚）/3.387,

                           = 75LQA.

                                                    0 . 0bq3.1         戶·O니4

                                                +     -
                                                                 4
                                                                 .I.

                                                                       4A
                                                                            쁨P낱 3 . 387J11

              Van= (4中D/v手) + 75(0.0693 + jO.04) = 259.23 + j3.0

                           = 259.25 / 0.6631' V.
Solutions for Supplementary Problems                                               399




      a)    liii = IIaAI =75A

      b)    I Vj I = 月 (259.25) = 449.03 V.

j꾜     a) Ip.B = E(480四/(60 +j45)] = 6.4 /                       A;

            therefore, 'BC = 6.4 / 83.13 A,        'CA = 6.4/ -156.87A.

       b) IaA = (V3 LQ)(1AB) = 11.09 /                   A;

            therefore, 'bB = 11.09 / 113.13' A,         'cC = 11.09 I -126.87 A.

       c) Van = [(480iv' ) /      ] + (11.09 /               )(0.8 + j0.6)

                = 288.21LJ) V, therefore, Vab = 499.20 LQ V, and

            VbC = 499.20 /      V,       Vca = 499.20 /               V.

J꼬     a) Single-phase equivalent circuit
                                         O. $.n.   . 1. S八


                                          H工口A               中
                                                     口0O／삼




            IaA = [1200/(24 + 118)1 + [12刃/50] = 56 - j24 = 60.93 /_-23.2;

            therefore, I/ I = 60.93 A.

       b)    11A I = I 12어）V手/(72 + j24) = 23.09 A.

       c)    Ilyl = 1200/50 = 24A.

        d) Van = 1200 -I- (56 - j24)(0.5 + j1.5) = 1266.05旦26 V;

             therefore, I Vi. I s = V3 (1266.05) = 2192.86 V.
4伽1                                                                                                         Chapter 13




l쏘     a)

                                    口．003a. 戶.03.,.     o.oa八 戶·'B八                  A a·3$aJ1


                     I3.Bo아可                                                                        JL1iq
                                                                                                     J11
                        V了




       b) 'aA = [(13,800/I) /(2.375 + jl.349)] = 2917/ -29.60 A;

            therefore, I 1L I = 2917 A.

       c) VAJ寸 = (2.352 + j1.139)Ith = 7622.94느3.76 V;

            therefore, I VL I = v' (7622.94) = 13,203.31 V.

       d) Van = (2.372 + J1.319)IaA = 7916.93 /                            V;

            therefore, 1 Vab I = I Vj I S = \厚 (7916.93) = 13,712.52 V.

       e)   I 1 L = IaA/V'      = 1684.13 A

       f)   Same as (e).

12.6



                                                                                                    4그町
                                                                                       3

                                                                                           dH i 그

                             -I. ＋工；
                                   乙.,낟凡艸，
                                                                                       4


                           =0. fi
                                                                                           qV 1
                                                                                              L 1
                                                                                                니
                                               1＝니 卜-     I    I   1 a    .tikft
                                                  \r      H        11口   n 1 r4 11


                                                        m1 N




            Il = [(2400 - 11800)/1201 = (20 - j15) A,
            12 = [120/(3.84 - j2.88)] = (20 + j15) A,

            'aA = (ii + 12) = (40 + JO) A,
            Van = 120 + (1 + j3)40 = 160 + 1120 = 200 / 36.8끄 V;

            therefore
            IVLIs = 20小厚 = 346.41 V.
Solutions for Supplementary Problems                                                         401




끄2    S1 = [(24 x 103)21(400 - j300)] = (921.6 + j691.2) kVA,

      S2 = [(24 x 1o3)""/(8oo + j6어）)] = (460.8 - j345.6) kV人

      S3 = (57.6 + j734.4) kVA,        ST = S1 + S2 + S3 = (1440 + j1080) kVA;

      therefore, IaA = (1440 - j1080)/24 = (60 - j45) A.

      s = 11.시2(2 + j16) = (75)2(2 + 116) = (11.25 + j이）) kVA.

      Thus, SS = 1440 + j1080 + 11.25 + j90 = (1451.25 + j1170) kVA,

      S (tota1) = 3SS／中 = (4353.75 + j3510) kVA.

끄晏    a) V&j = (4160／月）匹mherefore, VAB = 4160 /                 \/,

          VBC = 4160 / +90' V        VCA = 416이 -150' V.

           'A = (4160/V중 )/[(208/3) 느竺 = 20V了／크匡A;

           therefore,

           'B = 20＼匡 L!PZ A,       VAC = 4160 /      V.

           Thus, W1 = (4160)(20V) cos (30 - 45O) = 139,196.31 W,

           W2 = (4160)(20v'3) cos (90 - 165') = 37,297.54 W.

      b) VN = (4160i汀) 匹亡 V, therefore, V1&j = 4160 /           V,

           VBC = 4160/ -90'V,        VCA = 41604j쓰V,           VAC = 4160 /        V.

           'A = 20Vi/= 5 A,       lB = 20v了 /        A; therefore,

           W1 = (4160)(20v'3) cos (- 30' - 45') = 35,297.54W,

           W2 = (4160)(2C月) cos (- 90' + 75') = 139,196.31 W.

           Note that reversing the phase sequence reverses the readings of the wattmeters.
402                                                          Chapter 13




12은   a)   I 'Ii. I = 600 V,   Zb = 8 + j6 = 10 / 36.87 Q,

           I 'Ll = [(600/V互)/10] = (60/'./J) 人

           Wm = (600)(60/'/ ) Sin 36.87 = 12,470.77 W.

      b) QT = 汀 刃'72 旨 21,＆乂）VAR.

           Check刃T = 3（印／月）2(16) = 21,6(刃VAR.
Solutions for Supplementary Problems                                                403



Chapter 13
旦.    a) k = M/'JE]:;; = 7.219 = 0.8.

      h) Mm카 = 1二仄 = 9mH.


      c)
           L1/L2 = (Ni/N2)2; therefore, N11N2 = V工7乙 = 3.


끄귿    a) k = 四／\／工；巧］ = 75/'/30(30面y = 0.25.

      b) coM = (1600)(0.075) = 120 Q,

           Z22= [(600 "4- 3000) + j (3)(1600)] = (3600 + j4800) = 6000 / 53.13 Q;

           therefore, 乙 = (120/6毗六3600 小泮叫 = (1.中I -jl. 92) C.

      c) Z = (13.12 -I- j48 + 1.44 -j1.92) = (14.56 + j46.08) Q.

      d) Il = [15/(14.56 + j46.08 + 10.44 + 113.92)] = 151(25 + j60)

              = 230.77j -67.38' mA (rms),

           12 = (jwA刃Z22)11 = 4.62／二끄竺 nm (r毗）,

           V2 = 300012 = 13.85 /          V (rms).

      e) V = [151(25 + j텨）)J(14.56 + j48.08) = 11.59 / 5.77으 V (rms),


           斗 = \71* = (11.59／立77으）(2羽．77／흐7코8D
              = (11.59 /     )(230.77 /      )

              = (775.38 + j2560.47) mVA,

           S5(delivered) = 151 " = (1331.36 + /3195.27) mVA;

           therefore, percent delivered to transformer

           = [(775.38)/(1331.36)] x 100 = 58.24%.

      1)   尸L = [(13.85)2/3000] = 63.91 mW; therefore, 刃L = 4.80%.
404                                                                                     Chapter 13




끄코    Vt = Vcd = I口小／11 = j48[45/(15 + j30)] = 64.40｛쪼亞끄미rms),

      Z, = [1印 + j480 + (48/33.54)2(15 - 30)] = (190.72 + 1418.56) Q.

      b) ZL = Z: = (190.72 - j418.56) Q.

      c) P = [64.40/2(1어）.72)12(190.72) = 5.44 W.

      d) Il = (Z22IjwM)12,       jwM = j48 Q,

          Z22 = (160 + j480 + 190.72 - j418.56) = (350.72 + j61.44) Q,

          12 = (32.20)/190.72) = 0.1688 匹r A (rms); therefore

         Il = 1.25 /          A (rms),

         P1 (transformer) = If (10) + 1了 (160) + 5.44 = 25.69 W,

          and the percent delivered to the load is

          (5.44/25.69)100 = 21.18%.


꼬넌    a) Construct the s-domain circuit.

                                                 1




                                                口尸入                           k
                                                                                  드三으
                                                          甘／
                                                               1         4/
                                                 tj꾜eM.
                                                                   工a.
          480 = 20Ii + j320(I1 - 12) -112012,

          0 = 1320(12 - Ii) + 112012 + 18012 - 1120(Ii - 12) + 56012,

         Ii = 1.6 - jl.4 A,     12 = 1.1 + JO A,

          V。= 56012 = 616dtV,            IVOI = 616 V.
Solutions for Supplementary Problems                                                            405




       b)     /m m\ 2
        ' P = l- 4I 560 = 338.80W.
              (
                V2j

       c) Sg = -          4빼 = -384 - j336 VA; therefore Pg(del) = 384 W.


             Pe   【此nt蜘red山Q                        ＝   響x         100 = 8跏％            ·




끄臣     Construct the phase-d이nain circu妃




                                                                          r    '   斗＼
                                                                   卜"二二"
             480 = 20Il + j8011 + 1120(Ii - 12) + 1320(Ii - 12) + j120I1,

             0 = 56012 + 1320(12 - Ii) - jl2oli; therefore, 12 = 0.579 四으 A,

            VO = 324.211으V.

       b)
            尸=      쉬12   12   (560)   =   93.85 W.

       c)
            S = - . 4801: = -240r욕
                                \ + j,4) = -101.05 - j176.84 VA;
                                               17            17/




             therefore, Pg(del) = 101.05 W, and


            【加們此nt delivered的m :                               ：熬    / 100 = 92.87%         .




13.6



                                                                              !e
406                                                                                             Chapt:er 13




          125 = 20li + V1 + 120(Ii - 12)
          0 = 120(12 - Ii) - V2 + 9012
          V2 = 3%'i,      Ii = 3I2.
          Therefore, Il = 1.5 LQ A (rms) and 12 = 0.5 LQ: A (rms),

          Fb= [1.5(125) - (1.5)2(20)] = 142.50W,
          P Q = (0.5)290 = 22.50 W; therefore,
          percent delivered = (22.50)/142.50)100 = 15.79%.

꾜2     Construct the phasor-d이nain circu九




           150 = 21i +j10Il + V1,       V1 + V2 = 1812,              V1 = 2V2,
           (Ii - I2)N1 = 12N2; therefore, Il = 1.512,             3V2 = 1812,
          "2 = 612, and!2 = (5- j5) = s.I      j             A,



          1'18Q   =   퓌     18 = 450W,
                           '·
                                             11= 512 =  1.           (7.   5-   j7.   5)   A,
          Sg = - { (150)(7.5 + j7.5) = e 562.5 - j562.5 VA.

13.8




           120 = 7.21i + V1,
Solutions for Supplementary Problems                                                          407




          V2 = 1(I + 13),
          120 = 413 + "2
          12 = 4Il,       Vi = 4V2.
          Solving for 12 and 13 gives
          12 = 4.8샌亡 A (rms) and 13 = 23.04 L亡 A (rms),

          12 + 13 = 27.84 L. 2 A (rms),           P1Q = (27.84)2(1) = 775.07 W.

끄스    a) Find the Th6ve血比甲加alei吐 of the circt血 to 伽 left of the ideal transformer. We get V
          = 24 LQ V (rms), Z = (5000 + JO) Q. For maximum power transfer, the impedance
         looking into the ideal transformer from the Th6venin terminals must be 5000 Q; therefore
           八八n   =2
                 /=   .   戶八八n          n   八r1

                口) = ;X人人-I}
          LI.仄JU／                口 = U.Lu.


      b) P(ma址mum) = [(12)2/5000] = 28.80 mW.

      c) V2以）0Q = 12口 = 2.4 V.
    408                                                                                                                       Chapter 14



    Chapter 14
14.1               a) w = [(103)(106)/40(6.25)] = 4 x 106; therefore co。= 2000 rad/s.


                   b) VO = (25匹 x 10H3)(3200) = 80샌e V; therefore, Vm = 凹 V.


                   c)        = (l/RC) = [(10_3)(106)/(32)(6.25)J = 50 rad/s.

                         Q = (co万) = (20刃/50) = 40.

                   d) w1 = 20刃[(-1/80)                         +Vl+
                                                                            (iJ80)
                                                                                         2   J   =   1975.16 rad/   s,
                        m2 = 2025.16 rad/s.

                   e) QnJ-j = (2)(4)(6.25) = 50; Q is lower by 20%.

14.2               (1/cooC) = (200/20) = 10 (2; therefore, C = (1/l0w0) = 0.2MF,

          L = (1/口）긍C) = 201uH,                                       Q = 500/20 = 25 = w。
                                                                                         RC; therefore, R = 250 Q.

                   I    I = QIm; therefore 'm = (20/25) = 0.8 A.

141 Y근＋Ji + i佃如如＋cv이 근(1 +jM), ｝근Vn平；
4              '        R           '   1   '                  加                     J
                                                                                         R "
                                                                                                               나         1J



           therefore, M = 土0.75,                                      w。= 107 rad/s,

          cv = cv。- 25,000 = 9.975 x 10o rad/s
                 -?6IIfl(1(1QQ'7' Y in6\    e드nrYY)
-0.75 =    口V)VV니＼+/ ' / ' V " 4V / ＝노
             月（19.975x 106)         -    月 '
fi = 50,000/0.75 = 66.67 kradJs.       O =！卑        = 150 = cv0R C,
                                           I,                          m尸




                   0          （15
                                                )
                ,,d1。)
          C= l。 x
                                                    =
          C＝
                              (5
                         可
                                                        3nF.
                                                唯）]" 눋 '宗팖'如xl이
                                                              "
Solutions for Supplementary Problems                                                                                                                               409




                  R1
                               響    x io3 = 2 x io5; therefore u。= 1.1Mrad/s,
                                         =




            0m;        ,   ＝   프퓽            =    5.   5.
       " ) Z(wo)：缸싸蒜崙"12=25。kQ, Vm＝崙（250)=25 V.
       " ) Q南＝W亦eqC, 凡，＝客烈，,
            R1         =   8000     (1
                                             +    5.
                                                       52)       =     250 kQ,                         Req
                                                                                                                      =      93.75 kf;

            therefore, Qckt = (1.1 X 106)(93.75 x lO3)(20 x lo小12) = 2.0625.

               iQc幻 = 1.1 x 106/2.0625 = 533.33 krad/s.
       d) 月 = w。



                                                                                                                                 (
l쑈     a)                                                                                                                        / == \ 二

            R = woL/QCO1i = 8 k(2,                                                                           三 小 但）"
                                                                                 (1이      ' "     珪－
                                                                                                             LC                  나7 '
                                                                                                                                       4 r1Hl2
                                         I             d nn d 』，             d nl2                ._,                                  Lu                 -
            therefore,；二 = 끄人J.IO X Lu ! anu L ==                 e} 三 u.D pr.
                      Lt'                         (100.16)(20 x 10 V)

       b) 凡q= 8刃（:1+ 252）立5M(2,                                                                        R' =RgI I凡q= 20/w0C브4入1(2,

            4 = RgI I5; thereforeRg = 20MQ

       c) fi = 口）WQ = (10 x 106)/20 = 500 krad/s.

14.6   a) 口금 = (1/LC) = [(103)(106)/(40)(0.25)] = 108;

            therefore, co。= 104 rad/s,                                                   -1/w。
                                                                                             C = -400Q,

            1rnlS= (0.50/50) = 0.01世 A,                                                           VO = (0.01)(- j400) = 4 /                                   V.

       b)
            Rmeter = 10 k(2,                                   Qp = WORmeterC = 25;

              .                     11            rd    ,1   r노n』 ＼   . r4   .         八尸2\   1              d   尸   ,＼戶1   1\              r기   』＼ 八尸   1m

            rnererore, K1 = [IU,()叭" ('I 十 乙그 )J = ID.91 bd ,                                                                               Ll 三 u·乙＞1ur.

            1rnlS= (0.5 /                        )/65.97 = 7.58／으 mA; therefore,
410                                                                                                        Chapter 14




           V0 = (15.97- f似0)(7.58 x 1戶H 3.03乙뜨7.쏘V (rms).

           Thus, Vmeter = 3.03 V.

      c) 'meter
         "m.妃： = 100k(2,                 Q! = 250,                      R1브 [10/(250)2J= 1.6C ,

           V0 = (0.5/j51.6)[1.6 - j400] = 3.88 느：89.7끄 V (rms);

           therefore, Vmeter = 3.88 V.

141   a)       -         R,
1      ' Z =Rl＋凡＋
                 jwL + 1+ j；
                           凡C

                                      R2                        . . ,     .        口JJ？글C
                = R1 + RO +
                                   1+ )LC2           碌了"
                                        碌？十JWL j1+ )LC2


                                                                                       固]
                                                   져
                                                                                                  2
                                     口'C小2'-
                                         n2／
           therefore, co0L =                                        wo = 1 ;=; m
                                                                              11
                                   1 + U)枷象？'                               U [1
            1          103. 1012
                                    1.25 x 1012,                         1    卞10l2
           LC           (40)(20)
                                                                                            =0.   5X106
                                                                        R；乙 戶 103(20)
           Thus, w0 = 1 Mrad/s.

                                    L
           乙 = 入1 十／白 +
      b)   -      .1       ,1                  .   八   八   .   戶＼




                                   瓦乙 = I내J KW,

              10/ 00 -                                         --    --
           1 =＝干 = 0.1/ 0口 mA,                                 V,. = 75 X 10I = 7.5/ 0 V.
               Iou)    -     -                                   V                 '

      c)   ＠口） =0,              Z= R1 + 凡） + 凡 = 180 k口7)


           I＝끎世＝立世mA, %＝古（75)! 4.17世V
      d)       @w= m,            Z= c가                 VO= OV

      e) Not necessarily, since both the real and imaginary components of Z vary with w.

      f)   At cv = 1.384 M rad/s,                      wL = 55.36 kQ,                 (1/wC) = 36.13 kQ,
Solutions for Supplementary Problems                                                                411



          m   =   . 戶戶 4 /   m戶      100        . ,,= ,, . .m4 . 八. . /\
          乙 = > + J:)＞·Jt) + /> + 1 1 ..n n<0 = 91.)4 + 尸三叩J K놔
                                           I   丁 ／乙· 1()0



                     10/ 00
           I =         ; m = 105.83 / -1434肛A,
                           //
           I VO I = (0.10583)(75) = 7.94 V. This demonstrates 1 VO is not maximum when w = m0,
           since IV0（口J0기 = 7.5 V.

j.4.   a) After you replace Vg, 100 k(2, 1.8 kQ, and R with a Th6venin equivalent, the
          phasor-domain circuit is as shown.

           R2 = 200kQ

           C = 0.011uF

           V = V71' / 0('




           \／口   -




             ' R1 ' +(VOmVO)JwC+ VjwC= 0
                      Vt
              , .. 小            VO    -'   .     .      ,.       - VO
           HVa(JWC) -i; = U, tnereiore, Va = jwCR2 '

           Solving for V(, yields

            .                    -iwR-,CV. ,'                  , ..,.         . .      . . .. .
           VO =                  』）' n 口 "'    .             'i7 will be out of phase with V when
                           (1- nJ "C民R2) +J口)凡C

           n2扼R,                  = 0, or when
412                                                                                                    Chapter 14




                 , 1                                       1,                              978.93 Q,
                                         卽0),                             101, ,2 =
                                                           103)(0.
                        =

                otC'R 2                                               x
           凡=                                                                         1,
                                                       x
                                                                              6)
                                            2
                                                                 01
                                                (JJJ
                            (27r·
           凡 = 쩍무．打甲 山7893;【岫而e,R = 218.88 .
           Atf = 8001妃
      b)
                                    %=      －字v뇨           '.




           Therefore: Vm' =         끽各茗）= 139.92mV,
           VO = -14.14 V = 14.14/j型fV,

           vO(t) = 14.14 cos (1600兀t + 1800) V.
Solutions for Supplementary Problems                                                                                                                                                                           413




Chapter 15
亞1     a) f (t) = (t + 10)u(t + 10) - 21u(t) + (t - 10)u(t - 10).

       b) f (t) = -8(t + 3)u(t + 3) + 8(t + 2)u(t + 2) + 8(t + 1)u(t + 1)

                   - 8(t - 1)u(t - 1) - 8(t - 2)u(t - 2) + 8(t - 3)u(t - 3).


工끄     a)
            V叱＝川＋L似幽日坰斥                                                                                                                     idt.

       b) [V/ s] = RI + L(sl) + (1/cElls]; solving for! yields

            I = (V/ L)i[s2 + (R/L)s + (1/LC)].



亞코 ") 畔* " 少*打,（
               『－V) dt:0.
       b) C(sl스 + 끼／? - (V比／R)(1/s) + (1IL)[(V/s) - ([（比／了2)] = 0;

            solving for V yields

            V = V [s 4- (R/L]/{RC[s2 + (1/RC)s + (1/LC)]}

15.4


                      R1i1 + L1                                                           +                      C)                                                     i2)
       a)
            Vg =                                        (di11dt)                                  (1/                     f-                         (i1        -             dr;
            0 =     (1/                C)   f_                         (i2        -       i1)           dr       + L2               (di2/            dt) + R2i2.

       b) V = [R1 + sL1 + (1/sc)]!1 - (1/sC)!2,

            0 = 中(1/sC)!1 + ER2 + sL2 + (1/sC)]!2,

            A = {[R1 + sL1 + (1/sC)][R2 + sL2 + (1/sC] - (1/sC)2},

            N1 = Vg[R2 + sL-, + (1/sC)],
                                                                                                               2
                          N1                                                                                 (fl-,C + R1C노 + 1,)J乙
                               .                                                                             .    .            /1    .      11             /1            .




            /] ==                                                                                                                亡）
                                                                                                             '        日                          q
                                                                                                                                                                         '                                .

                                        ===
            -I                     1             r "
                                                   그1              !         ／기       .    )" ／기 -11 1                              .       !        11             .        /!     .   1   .   11 11 .   .'
                          m=                       =                                          4




                                   스             Is"LiL2C十s'C（사L2十L1R2）十s(Li十L2十R1R2月
414                                                                                          Chapter 15




      ,            10 + s + 1
                     (52
                                 )            10           s + 1)
1쏘
           -                          -            (s2+
      11 -       . 3 . 八 2
                s(s3+ 2s2+ 3s+ 2)          s(s+ l)(s2+ s+ 2)

                               10(52 + s + 1')
                s(s + 1)(s + 0.5 -j0.5v于)(s + 0.5 +j0.5v力



      I'＝孕璹T+s+o．
                凸..5f7 + s +0.，드
                               ， o.5 '71
      天O = 5 A,             K1 = -5 A,        K2 + (5II7) /         A.

      11(t) = [5 - 5e中i + (10/v7)em0요 cos (0.5f7t - 이）.)]u(t) A

               = [5 - 5e巧 + 3.78h05' sin 1.321]u(t) A.


亞亘 ') 耶）＝孕『,s +K2) + (s且）, 小쁑＝9,
               K2 = 36(2)/(-2) = -6,           K3 = 36(- 4)/[(-8)(- 6)] = -3;

               therefore,f (t) = [9- 可2'- 3e씨町t).


      b) 殉＝孕＋孕，;＋후卄具     , 시＝（羽0,
         只s) = f 七亡 七亡 느六，    .)(1)(2)
                               s/A\
                                  I - 1,                                 U八斗八J)


               K2 = 30(- 2)(- 1)/[(-3)(1)(2)] = -10,

               K3 = 30(- 3)(- 2)I[(寸4)(- 1)(1)] = 45,

               K4 = 30(- 4)(- 3)I[(- 5)(- 2)(- 1)] = -36.
                                                                36ee5'Ju(t).
               Therefore,f (t) = [1 - 10em꼬 + 45e4i -

      c)
                           K1     K                       K卞，
               F(s) = S
                      :' + (s + 6- j8) + (s + 6+ j8)'                K1 = [500(5)1100] =和,
               K2 = 500(j8)/[( 6 +18)016)] = -15 -j25 = 25 / -126.87 ,

               K = 25 126.87,             f (t) = [30 + 50eh ' cos (& - 126.8尹)]u(t)
Solutions for Supplementary Problems                                                                                                                                                         415




      ") 耶）：三'*（上）2+（忽）, K1=響아＝凹，
            K2 = 200(5))/(-5) = -200,

            K1 = 三［200（흐끄이
                     "                   'SL            S         i   S = -5
                                                                               =     200{   [s_      (s+
                                                                                                                   10)
                                                                                                                           ]/s2}              ,_
                                                                                                                                                       -5=           -凹,
            f (t) = [80 - 20야e尸5i - 80e_Stju(t).

                     .           .                                                 K李                              K1                                            K卞，
            F                                                         +                          +                                                 +
                 n
                                                  K1
       e)
                                     =                  '     I                      '       今             /   .   r   1           ..   n .            /     ,             1,   . . ,, . 1

                                                                                                     냥 十 J U JIU)                                      낳 十 그 十flu)
                     (s)                                                                                                                                         ;
                                          (s + 5 -110)'                   (s + 5 +j10)e

            K1 = 800(- 5 + jlo)/(j20)2 = 10(1 -j2) = i0/弓／
                                                         ＝里坐으，

            ..                           n, n d1              S
            八2 == 猷工J二 1                                                                         = I = 1 亡四으，
                     mL
                                                       (s + 5 + 110)2
                                                                               5= -5+ jlO



            f (t) = [20'弓teU51 cos (lot - 63.43. + 2em51 cos (101 + 이）.)]u(t).



      t) 只《）가啞川小予小，
            K1 = (180/5) = 36,                                        K2 = [(- 200 + 180)/(- 5)] = 4,

            f (t) = lO3(t) + [36 + 4e_Stju(t)

珏7    a)    n r끼na -
                                               立Kre + d\
                                               1/V\1J 1 ' 1           中
                                                                                   그人11 + rd/ e\ ]
                                                                                   1:1J[1 1 \ 111J/1
            JJ' \JJ -
                                           (s + 2)(s + 8)                 s[l + (2/s)][l + (8/s)]'

                     liin                  m.. .   - .      -   n.八4-.
                                          st (s) = U, ttleretorej(U ') = U.
            5-             ,



                     lim                   ,m. . ,, .       -
                                          5r (S) = 9, lflereloref(叫 = 9.
            S +                      m



      b) , 口／, . -小                           ( +l) (s+ 2) -         30[l+ (1/s)][1+ (2/s)]
             "             \1U       H
                                          (s + 3)(s + 4)(s + 5) s[l + (3/s)J[l + (4/s)][l + (5/s)]'
416                                                                                                                                                                           Chapt二r 15




                                                 lim             .m. .  n '.     戶   戶. 八4-.
                                                                SJIS) = U; lflerelorej(U " ) = U.


                                                lim              ,n. .      .       . .    .
                                                                S／乂5) = I; rnerei야ej（的) == 1.


                c)                      ,,, .    500(s + 6)           500[1 + (6/s)1
                                       srisj= -           -    =         -     -   1 4
                                          "   (sZ + 12s + 100)   s[1 + (12/s) + (iOO/5Z)]'

                                            urn
                                                                sF(s) = 0; thereforef(0+) = 0.


                                           lim
                                                                StlS) = iu; tnererore八oo) = 3O.
                                                                       ,m    .       .         八n        .       .   -.            .



                                     S +               的



                                                     (S) = 200 + 10) = 200[1 +
                                                     (s)                           )]
                                                                                                                               (lOis
                                                                                         (s
                                                                                                                                            -
           d)
                                     sF
                                     :F
                                                     "       (S+ 5)Z    s[1+ (5／노）］二 '


                                                                sF(s) = 0; thereforef(0+) = 0.
                                          urn
                                了+                     00




                                                                s八S) = du; tfleretorej(力) = ?5lJ
                                          urn
                                                                                 .             八，,   .       n       戶.        .                  nn




      e)
                                                     . .                                      800s                                                     800
                                 '八刃
                                                           =
                                                                       （노2
                                                                                         + 1Qr + 125)2 =             s2
                                                                                                                          [i
                                                                                                                                       +   (10／
                                                                                                                                                       노） +   (125／
                                                                                                                                                                      노2)]2

                                          urn                    -- .    n .     -   ---.4-.
                                                                St (5) = U; ulereioref(U ' ) = U.


                                s-
                                                .。
                                                           sF
                                                                   (s)
                                                                                         =    0; thereforef(的) = 80.


      0              -.n.. . - 10(s2 + 9s + 18) - 1小[1 + (9/s) + (18/52)]
                     "' \U -        (s + 5)     1      [1 + (5/s)]        '

                     Initial-value theorem is not applicable sincef(t) contains impulses;


                     ,lirn0sF
                     s-
                                                '
                                                      。          (s)
                                                                                     =        36; thereforef(的) = 36.
                                       SV(S) = U,                                                    S-+0 SV(S) = Vdc
                                                                                                     s-.0




Solutions for Supplement幻ry Problems                                                                                                                                                                                 417




                                                                      (l今.11加
亞코        sl      (s)       =          [:
                                       [s2         2+
                                                    +      (R/
                                                           (R/             L):s +
                                                                           i)                        -        (1/        LC)]

                  h1ll
          ,urn.                        sI          (s) =              0,                         i       (0         ')       =        0,
                                                                                                                                                     checks             initial
                                                                                                                                                                                          value.




                                                                                                                                                                    【3
                                                                                                                                                                  operation of circ出t since capacitor blocks
                                                                                                                         =
                                                                                          .(m)                                   0,
          ,lim0                                                                                                                             .h凹k8.                 P.
                                !/0)                             0,
                                                      =
                        :       sI           (s)      =          0,               :(oo)                                  =       0,         checks                                ..的f.            .           dc.
                                                                                [s + (R/L)]
                                                     Is2 + (1/RC)s + (1/LC)]
                  lim                        1,. .                         .                                  lim                          ,. .               ,
          5-        .



           v(0+ ) = 0, agrees with stated initial condition.
           v(끼 = Vdc, agrees with operation of circuit.
418                                                                            Chapter 16



Chapter 16
프교     a) Zab = (R + 了L)(1／노（乃兀R + sL + (1／노（D]

                 = (1jC)[s + (R/L)]/[s2 + (R/L)了 + (1/LC)].

       b) (R/L) = 6000,       (1/LC) = 0.25 x i08,    (IJC) = 2 x 106;
          therefore Zab = 2 X 106(s + 6000)/(s2 + 600Q + 25 x 106),
          2l= 6000,       Pi = 3000 +j4000,     P2 = 3000 -j奴0

16.2




          z砂 = 小V(4 + 吐
          z日斗 = (16／노） + 2砂
                 - 4(2 + 打 + 16)
                      s(s + 4)

          y, ,- 1 ,  s(s + 4)   = 0.5(s2 +小 + 8)'
          'th 4 " 4(s2+ 4s+ l6)    (s2+ 小+ 16) '
           勺
             = 2 + j2,      z2 = 2 - j2,   P1 = 2 + j2匡       P2 = 2 - j2'厚.




                                     겋
          1/ -        (24/s)        1
          VO -
                 [R + sL + (1/sc)] sC
                         1스1IT C\

          VU乙[s2 +（說)s + (1奴긔
          (1/LC) = 1010,
          (R/L) = 120,000.
Solutions for Supplementary Problems                                                        419




         I乙 =
                                    24 x 1010
         "         s(s + 60,000 -180,000)(s + 60,000 +180,000)


                  瓦               K2                       硝
              =     =+ .    ．小 n n 1 '4 1 n n n . + . 1m = = 1 ．戶小 n 4 八．.
                  S    (s + 6UJ乂乂I -/8UJ乂乂｝) (S + （乂J!（乂xi +j8U,UU0)'

             K1 = 24,          K2 = 15 / 143.13..    K ' = 15 / -143.13;

             therefore, vO = [24 + 3(ke텨）
                                        ，어Xy cos (80,000 + 143.13')lu(t) V.

!珏     a) The s-domain node-voltage equation is

             V1-'- (30/s')                 1（尸        -- - -
                               +
                                                  ) + V 01 x 10                    =   0;
                  10,000                   +50,000
                                                        (0.               "   s)
              '            '       (lOOs
             therefore, 1C = [30,000(s + 500)15(52 + 1500s + 1.5 x 106)]

              凡              K2                 尺；
             = S + (s -I- 750 -1968.25) + (s+750 +j968.25)'

             K1 = 10,          K2 = 12.65 / -113.28'.             尺二 = 12.65 / 113.28'.

             yC = 10
             vc        25.3m-750t cos (968.25i-113.28.)]u(t) V.
                  l0 + 25.30e

       b) 'c = sCV = [3 x 10m4(s + 500)/(s2 + 1500s + 1.5 x 106)1


                                   K1                         K
                   = (s + 750 -1968.25) + (s + 750 下1968.25)'

             '1 = 154.92 x 10已끄堡으，

             iC = 309.94eH75m cos (968.25t + 14.48')u(t) uA.


16.5   a) Construct the s-domain circuit.
420                                                                                                                                                    Chapter 16




               41c + s(IA - Ic) + 5(JA - 1B) = 0,

           'B + S('B - 'A) + s(IC - IA) + 흐9/C = 0,


           ／中 = IC,
                                                    IC
                                                    7
                                                         【：
                                                                       Ig+
                                                                       7：
                                                                        『78,
                                                                           IB,                     '   7=
                                                                                                            74= 10s
                                                                                                            'A              (52
                                                                                                                            (s+
                                                                                                                                      -   .2  熬
                                                                                                                                          5)(s+ 10)
                                                                                                                                                250)

      b)             ,        10(s2 - 24s - 250) .  .
           sI=                 (s
                                  + 5)(s + 10
                                             ) tneretore,                    '
                                                                                 ;
           i
               (0+
                         )=
                                     ,
                                     s-
                                          urn
                                                ,             5/   =
                                                                           l0A,              i
                                                                                                 (m)
                                                                                                            =   s-
                                                                                                                     쁘5。
                                                                                                                       SI
                                                                                                                                  =       -   50 A.

      c) Atr
      C) Att== 0+




           (50 - i)1 - 4i = 0; therefore, i = 10 A                                                                     (Checks.)
           At t = co, the capacitor appears as an open circuit;

           therefore i中 = 0 and 4i中 = 0. The inductor appears as a short circuit, hence i = -50 A,
           since the 5- resistor is shorted.

      d) =                     50                        42            '     18
      '    1=            --           十 1느   十                                           .
                                    S   S+ >   s+                                    1 (J'



           i (t) = [-50 + 42eH5t + 18e110']u(t) A
Solutions for Supplementary Problems                                                                    421




뜨血    a) 뇨＝10叩．
              ＝흐擊＝1以)0.                         kf=           0.02         . =l以）0.
            " '    i        >          "        r     r1rlnn\ /r} n4\ \/ 1nm山
                                                      ykAu八U.')乙) 八 LU



      b) For the dependent voltage source, the coefficient of i中 has the dimensions of o뇨ls,
         therefore the coefficient of i, in the scaled circuit wi끄 be 4000. In the s-domain, the circuit
         becomes:




                                                                                      1
                                                                                 5.OXI0
                                                                                    S




      c)
           In 싸riting the solution for i (t), note: (1) all frequencies are multiplied by 1000, and (2) the
           current amplitude will be the same since the circuit is driven by a current source.
           Therefore,

           i (t) = [-50+42em5어X ' + 18eU10'어X ']u(t) A.

五．Z   a) i1(0) = i1(0+) = 12/2 = 6A,                i2(0) = i2(O+) = OA,

           L1- M= OH,           L2- M= OH,                L2- M= 2H;

           therefore the s-domain circuit becomes
                                 'is       n=       尸'.
                                                    V 口
                                                           O作）
                                                           小               d a




           Now this circuit reduces to
                                    to/S


                                                                                    to人
422
                                                                                                                    Chapter 16




             A2= rl9+ 2)/,＋감（/, e/,, e l2md
                 S              \ S          /          寸                     '


             -12 = 2s(I2 - Ii) + (2s + 10)12; therefore,

           1= 竺 (s3+ 7s2 + 15s + 25) = 三 (s + 5)(2 + 2f +5).
                         5 -                                              '        S .       "         '


            /,
                     =                   6
                                           7노＋ 5)（노2+
                 '             (s+ 5)(s+ 1- j2)(s+ 1+ j2)


                     =- L旦＋ 主7三亡왁＋ 3.75四e.. and thus
                      S+ :) s+                                  1- fz     s+ 1+ jZ'

           i1(t) = L-1.5eH5' + 7.5e_t cos 2t]u(t) A.


      b)
           '2=           (s+
                         (:
                                *)(:  )(s+
                                         *,1-               -
                                                                 j2)
                                                                       (s+ 1+     j2)
                     ＝푸｝『 ""'：瓷斗 con加艸m.
           Therefore,

            2(t) = [叫1.5e_5t + 1.5v了e4' cos (刀 + 63.43.)]u(t) A.


l塑    a)   For t < 0,                    iO(0) = b0A,                                   i1(0) = 4A,   i2(0) = 6A.

           Using the T equivalent circuit for the magnetically coupled coils gives the s-domain circuit
           sho帥 in the f蜘re. AppM昭目rchhoff's laws generates the f에owing equations 뇨 terms
           of!1 and 12:




           (12/s) = 10(!i + 幼 + s(I1 + 12) - 10 + s11 - 4 + 3/l and

           511 - 4 + 31i = 3s12 - 18 + 212. Solving for Il and 12 gives
Solutions for Supplementary Problems                                                                                                       423




            ,       (4/7)(72 - 19s + 6)                                              .           (1i7)(42s2 + 236s + 36')
            1i=     '   ' '..                                 '.                 i)          =   '     / '       -                     .
                           =                .      ,     S         '                     -                   r   乙   .   r1   .   n뇨

                                                                                                        叭S 十 di 十 6J
                -        /      .   iN

                        只S 十 55 十 S)


            We also have
                                  2
            /. =/, + , = (1/7)(7Qs" + 160s + 60).
                                     /d   , 尸4 .       /,mn            .   d   /,1           .   ／八．




                                                   s(f + 8s + 8)

            using p.f.e. to find i1, i2 and i。yields

            i1 = [0.429 + 6.83白U6"82& - 3.265e_l "lThJu(t) A.

       b) i2 = [0.643 + l.4l白e6"82秘 + 3.94le-1.17刀Ju(t) A


       c) i。= [1.071 + 8.252e_6.82앉 + O.676e_l "lTh巾i(t) A

                                                         762eel"l72]u(t) V
       d)
                 l2 -e l0i.
            yv = 12          [1.286 -e 82.524eU6.82& - 6.
                       10i。= [l.286

j亘운    Writing the s-domain node-voltage equation at the inverting i叩ut terminal gives (V1/l) + [(V1

       前器너유二胡씌잃：瑞盆叩'半叱謐ving for V,"甘' "' "" '("
垣끄 Thi뎐沖艸빤旽．        帥맷fier由cuit.; there恥21.0 = _(Zp'Zg)Vg ihere』Z1 = 프I／노）/[1 +. (1／노）]
                                                                 [1/(5 』+1月 + (l/S2jr
       . = I bd. b깬vmg r아和 giv뜨. 노. = -II[S (S 十. I月 = U(l/S ) -
   ana乙i                                                                      +e =
       tnereiorevO = (1- t -e )U(t) V. Ifleop-amp 꿔illsaturatewhenvO = -lu V ort
       11; therefore, t = 11 s.
424                                                                                                                         Chapter 17



Chapter 17
fl j,         An analysis of the circuit for t < 0 shows the value of vO(0) = -38.4 V and the current up
              through the inductor is 9.6 mA. Fort > 0, 30-V source acting alone:


              ;；百十
              乙； S , 1싱 -(30幼 .
                       1以刃
                                                        十
                                                                （2s+
                                                                            玘；
                                                                             4伏刃
                                                                                             ）
                                                                                                  =       U,
              까＝,s(s즈黑
                  (:2  才뇨，
              . ,,       KO .                       K1                                   .                         <
              VO =；느S + 1500 -戶어）
                                ）十（S+ 150띠1+ j5어）),
         KO = 24,                      K1 = -12 +j6,                                             K = -12- j6.
                                                                                                 111J\




                                                                                                                       그S




         Irntial capacitor voltage source acting alone: y = -38.4 V,

          V' s .                       V。               .              VO
         교十
                         （2f+
                                       4000）      十10
                                                                       (刃＝         _u)
                                                                                                 y,




          I,。= 2
              (s烹忿烈.6)
         v = (s*巧品：00)
                   『小盈剛，
        K2 = -19.2 + j19.2,                                            K = -19.2 - j19.2.



                                                                                                                       a$




        Imtial inductor current source acting alone:
        Pb,,
        V,"              끼尸S
                         V,"s               yV ",,-19.2 x
        mmH          +
                                   -    +     -
                                               ;,                                                              0
        d 11J\ 1\
                                                                                                      =
                                d 八0                        八          .    1 八n   r1
        1U(Rj                   IU                          1.5 十 'MJUU
Solutions for Supplementary Problems                                                                                                                                         425




                                                      ,                    96                 10

                                            甘 + 3。。。s + 2.5 x 1。6)
                                                                                 x.
                                                                            .
                            =               (2                                                                  '
                  ,＝




                                                                                                                      쯤
             「？
                                                                                                                                                                天； = j9.6,
       「3,              :              (,        *                     K3-             j跏）               *(,   *,.        +j5。       。)'     K3 =   -j9.   6,
       V, = ,L/: 미，
                  , .      , nrrr   24 , (- 3t2 + i15.6) , (- 31.2- i15.6)
                  '= 1/，了 -I- V " = 1 " 中 \ V二：= ' .1二：
                                                      :/. + . \ r：
                                                                 二 1 I巾二：. .'
       '0- '0                                                   '0               ' 0 - s ' s + 150卜戶00) ' (s + 1500 + j500)'
        - 31.2 + j15.6 出 34.88 d塑巫으；

       therefore, % = 口4 + 69.77戶烈)'cos (5幽 + 153.4功帥)V.
                                                                                                               1k二．              니 'U느 as




17.2   a) The s-domain circuit is

                                                                                                                    O.OlS            0.rX10乞／$




                                       =                 100J
                                                 100 + 0.0ls + 0.5x 107s
                  Pb=
                  v。                                                                            ':
                  4         (,         )=                 V0=              :,:               , ,,    값            x1。
                                                                                                               . 5。 6

                                                                                                                      4
                                                                                                   . , , ; 10 s, , , , , . , : . 100Qr
                  %0)
                  V。
                                 (s)             =
                                                 :4             H    (s)
                                                                            V5                 乙52 + i。 + 5。x i
                                                                                               =                           S2          i。
                                                                                                                                        6
                                                                                                                               + 5。x
       b)
                                                                     (5）
                                                                                 (s)
                                                                            蜘）
                                                                                                                                      l072
                                                                                                                                      10 5
                                                                    (s + 5000 - j5000)(s + 50目 + 15000)(s - j100(W5i )(s + j100(h'5 )

       c)         Because the poles of I如) are a 啣叩lex con加gate p缸 뇨 the left 뇨珏ofthes－아an디 the
                  transient component of vO(t) will be a damped sine wave.
426                                                                                                                     Chapter 17




        d)
              The steady-state response will follow the driving voltage, thus it will be a sinusoi由l
              function of time.

       e)
                                                     107s2
                      =
                  '       (s + 5000 + j5000)(s' + 50 x 10")
             K1
                                                                                       S = -50（刃 + j5伉刃




             K2
                          (s2 + l毗 + 50 X 106)(s +11000v'30) s =j1000V6


             Therefore, V。        (t)
                                        =       1000v  '
                                                           e'
                                                                5띠' cos   (50001
                                                                                        -    135 + 1000 cos 1000v'W V
                                                                                               ")
17.3   a) Construct the s-domain circuit.
                                                                                       kl1
                                                     니O九




                                                                                                             VI,
                             \6
                                  匕而    +   -
                                                ZU匕）
                                                 S




             匕＝乙『kI：乙*k(늑씌
             therefore

             .,    401今                  k      ,                                                                             (3)
             V1 = 40_ k                 40- k "

             When Eq. (3) is substituted into Eq. (1), there results


             恥智꼼乷）＝月（s).
       b) 160- 4k 之0; therefore4k = 160,                                           k = 40,

             and k 5 40 for a bounded output voltage if Vg is a bounded input voltage.
Solutions for Supplementary Problems                                                                                                427




                                                  20
       c)
            k= 0:              V。                                                V. =20匕e160ru(t) V
                                                                                 v。 =20e
                                                S + 160 '

            k= 20:
            k=
                            匕  vO
                                        =
                                        =
                                                ,
                                                            608。
                                                               ，                 v。
                                                                                            =   60e’ 吼(t) V

            k= 40:              VO =                                              VO        = 1어뇨（t) \/



            k= 50:              VO                                                vO        = 120e40'u(t) V


            k = 80:            1今           =       16。'
                                                S 180
                                                    ,
                                                            -                   「。          =   180e1吼     (t)
                                                                                                                  V


17.4




                                                                      三瓜二        0      6       1a     入




                 四56:               y    =
                                                f               (t-
                                                                         A)
                                                                              (3又）d7L
                                    = 0.5t3, y(3) = 13.5
                                                                      y(6) = 108;
                 6 5 t 5 10:

                 yf 꾜(t - ))d. +4 (36- 꾜）(t中兀）m
                 = m0.5P + 18t2 - lOSt + 216,

                 y(9) = 337.50;
                 10 5 t 5 12:

                 y= /,1,.               飢（re又）m+ 4 (36- 꾜）(t - A）叱
                             . = 1\  1而                         4. . . - .. .. 1.12
                 tileretore y(IZ) = J싸                          j杜lZ - 시a凡 + L                         (36- 없)(12- 2)d =584.
                                                        二                                        U




                 12드t드16: y= f6 ,.                                            M(rH凡）dA +fl,2                     (36- 3A)(t- 又）d七
                                                        4- lu                                        - U
428                                                                                                                                                            Chapter 17



          .    .    ,_ -s   .6                                                    n4 . 4 戶 . \ ..  ,12                        . 4 戶 - . . - 』- -. -. --
          inereiorey(i>J = j r                                                    j4(l> - A) L4. + J,                         (30 小 j4八l> - 4)ti4 = >34.>tJ.
                                                                    J                                           - o


          16 드 t 5 22:                              y= J12f1_1。                             (36- 꾜）(t -又）吼

          y          (18)   =       f二2             (36H                 꾜）        (18쿄）'La= 208.
                                                                                            X (t=>)




                                                                                            仕 =1口）



fl 亞   a) h(A) andx(t -)                                   are plotted below.y(t) = 0 fort 5 -2,


           小25t56:                             y=               f             2       8(10- A)da = 64i H 4i2 + 1中1.


          65t58: y= f小；                                                                8(lo- 2)da

                                              = 768 - 64i.
                                                            -       in                  .               .   .




          8 5 t 5 16: y = J.'V ,                                                      8(10 -又)c兀
          八                     .         i




                                                           V 1．卞6


                                                    = 中2 - 12& + 1024.

          16 5 r 드 00: y(t) = 0.


                                                                                            "：
                                                                                             '     卜｛            :.-,)
                                                                                                                         IO      入

                                                                                      X（七1>)

                                                                                               B

                                                                                       I 1                                        入
Solutions for Supplementary Problems                                               429




      b)
                         t          y               t             y

                    -2
                                    0              8            256

                         0       144               10           144

                         2        256              12            64

                         4        336              14            16

                         6        384              16             0




17亘   H (j50) = [625(10() + j50)/(j5000 + 12,500 - 2500)] = 6.25 LQ;

           therefore, vO = 25 cos (501 + 600) V.

工Z2        a) 月(s) = e石在元          각＝R／偈C)S + 1),             Zi =R刃라C芦 + 1);

               thereforeH(s) = -(C:/Cf)[s + (1IR,C1)]I[s + (1IRfCf)],

               (1/R,C) = 40,      (1/R1力 = 100,         C,/Cf = 12.5;

               therefore, H(s) = - 12.5(s + 40)I(s + 100).

           b) H (j200) = 11.40 i 195.260,     vO = 11.02 cos (200t + 195.26') V.


fl         a;) Construct the s-domain equivalent circuit.
 430                                                                                                                                                                           Chapter 17




                                                             Pa* Va                                   b
            Va
                                                                                            ;V
                                                            SVa+                            2
                                   Vg+
                                                                                                           =
                                                                                                                     0.
                                   41!
            乙－
            Vb                           a                                                             1'b-
                                                   + (yb
                                                                                                                              O
                           小
                               ,
                                   V
                                                                                y,
                                                                                      ):+
                                                                                                                          V
                               -                   +(Vb-
                                                                      e         V。
                                                                                                                                  =   0.
                           乙
                                                                                      )S+
                                                                                                                     -l
                                                                                                                     乙




            P江
            VOs+
               +Vo-
                  ,, Vb =0.
                  乙


                 It follows from Eqs. (2) and (3) that

                 Va = V。
                       (打2 + 4s + 1).

                 Substituting (3) and (4) into (1) yields

                 V。 , , . .
                 -
                                                                                                      0.25                                            0.25
                   = ?1I                                   (1 =

                 1슝                      " ' "'                   s3 + 2.5? + 1.5s + 0.25                                                  (s + 0.5)(s2 + 2s + 0.5)'

       b) v뇽 = 1（뇨4(1),                                                   1슝 = lOis,

                 2, = .   - -     2.5
                  U s(s + 0.5)(s + 0.293)(s+1.707)


                 - 10S (s瑥3) +出.5) (s？므6.
                                       7。7)'
             %(r)
             vO(t) = [l0
                     [10 -H 29.14e
                               l4e10"29갚
                                   O.293t + 20e0
                                            2me051 -e 0.86e
                                                      0.8白H1.707:]u(t) V.
                 Checks: vO(0) = 0,                                                                   ％佃）= 10V.


       " ) 月(jw匕.．四3+11)(0.5瑥)(1.70가j1.0) = 0.1085＝坦크Z;
             therefore, Vm(ma虹mum) = 15/0.1085 = 138.29 V.

工Z2    a)   VO = 2 x 1061(52 + 60,000s + 25 x 108),

            H        (s)
                                   =         VO/
                                                             Vg   =       VO/
                                                                                     (1/
                                                                                                 s)
                                                                                                       =       sVO
                                                                                                                              =   2 x 106s/   (s2
                                                                                                                                                    + 印,000g + 25 乂 108)   .




       b) h(t) = Lm1[H (s)]
Solutions for Supplementary Problems                                                                           431




               =L
                    -   [
                        1            K1
                            (s+ 30,00(J- j443,000)
                            .             .       .   +
                                                          (s+ 30,(XXJ+ j40,000) l '
                                                          .    =   '
                                                                       K
                                                                       -   -   -   -   -   -   -   -
                                                                                                       1
                                                                                                       I   .




           K1 = 1.25 x i06厓6.87으,             K = 1.25 x i06 /

           therefore,, h(0
           therefOre   h(r) = [2.5 x l06e -羽,어0 cos (40,000t + 36.8尹)]u(t) V.
                                   X 10

      c)   H們0,000) =: 31.21/ 20亞6;

           therefore, v。= 156.05 cos (44J,000t + 29.56') mV.
432                                                                                                     Chapt:er 19



Chapter 18
J꾜    ay = 0, ak = 0 for all k, bk = 0 for k-even, bk = 105/k for k-odd; therefore we have

                        00

      Vg= lOS       2
                               ,   -
                                       sinnw0tV
               n=1,3万


      vi = 105L으v,                                V3 = 35四으＼/!         V5 = 21／立v,        V7 = 15匹亡V.

      a)0 = 2 x io4兀rad/s,                             鈿0 = 6 >< l04兀rad/s,       知0 = 105兀rad/s,

      7w。= 14 x 10'ir radJs.

      Z1 = 800 + j250.07 - j1000.97 = 1097.20 /_-43.19 (2,

      z3 = 800 + j750.21 - j (1000.97/3) = 卯1.9旬끄亞끄 (2)

      Z5 = 1320.16 / 52.70 c,                            Z7 = 1795.56 / 63.540 ),

      Ii = (105/1097.20)（坐.1望 = 95.70（坐끄如iA,

      13 = (35/901.95) / -27.51' = 38.80 ,i -27.51' mA,

      15 = 15.91 / -52.70' mA,                            17 = 8.35 / -63.54' mA,

      i = 95.70 sin (w0 + 43.19) + 38.80 sin (3口J0 - 27.51")

         + 15.91 sin (5口J0t - 52.70') + 8.35 sin (7w(/ - 63.54') + ... mA

塑오    a) Let각 = l04+ 0.ls,                                Z2 =5000Q,         乙＝8000c,
          Z4 = (2000 + 109/5s) = [2000(s + 105)/s] C,

          :;...-        VO -                      Z2        Z4     -       -0.2(s2 + 1010)
         LL,.)) =       ;:= iii 7  1 '7                  '7 J '7 二 .. L 1 <AAAfl\ /., i 4il n1Y)＼·
                         Vg     乙1 丁 乙2                  乙3T 口4    J YIJ나小시八"- I- 乙1力'J'Ju,


          Vg is even with half- and quarter-wave s甲nmetry,

          therefore, a, = 0, bk = 0 for all k, ak = 0 for k-even, and for k-odd

              8 J4/4" . n 』 0.4r.     .      .    0.8
         口1 = 三 r' " ((1.'1 叫 늑．三）COS 奴功亡It    = 三＝느． '
              TJO ".'1         T 'YV' '' H " ' k2n.2.'
Solutions for Supplementary Problems                                                          433




                                       的

             theref。
                   re. v, =塑
                      "   O
                            .    二
                                       Y
                                      1=1
                                             4 c。
                                                s nwd v.
                                                {          V     "


                               .7V   n=1,3万 n

             m0= (力r x i06/62.8) 斗 105 rad/s,                  尸(Iwo) = 0,

            H (j3w0) = 158.66 x 10已＝1'塑互쓰，

            H (j知。
                 ) = 183.76 x 10            / - 161.010,

            月(17口J0) = 191.49 >< iom3亡二프62t,

             Vm3 = (0.8/9.ir2) = 9.01 mV,

             Vms = (0.8/25兀2) = 3.24 mV,            Vm7 = (0.8/49ir2) = 1.65 mV,

            vO = 1428.93 cos (3w0t - 149.62) + 595.79 cos (5w0 - 161.01")

                + 316.76 cos (7w0 t - 166.2尹) + ... uV

        b) w0

J,, 4   m., 1m d，勺 .       尸八 100
I꼬      rromtx. II.I, Vg = DU - 二i中           2       1sin nwOt V. Use the n。
                                                      n
                                                                            de-v。
                                                                                ltage meth。
                                                                                          d
                                             n=1
        to derive Hs); thus,

        H (s) = (Vo/Vg) = 10刃/(s + 1100),            m0= 100ir rad/s,

        月(JO) = 0.9091,       且伽o) = 0.8741／二호竺，

        月但蜘） = 0.7894 L므으.7笠                 月好如） = 0.6904/＝쁘흐望，

        月們蜘） = 0.5988 / - 48.80' ,           Vmi = (100/2V) = 31.83 V.

        Vm2 = 伍聊2兀） =: 15.92 V,              Vm3 = (100/3끼 = 10.61 V,

        'm4 = (100/4ir) =: 7.95 V,

        vO = 45.46 - 27.82 sin (w0t - 15.94") - 12.56 sin (2w0t - 29.74")

           - 7.33 sin (3w0t - 40.59') - 4.77sin (4w0t - 48.80') - ... V.
434                                                                                                                                                                                                                     Chapter 19




쑈포                                                                                                                                                                                                        l
                                                                                                                                                                                                          12
       a)                                                        r                                     /                .                     .                  .                       /       .

                                        rms-[（ "
                                              孰）벼 ' 벼 '［춰                                                                                                                                                  브 17.74 A.


      b)                                    r                                                               -小                                                                                       l
                                                                                                                                                                                                     12

                                                                                                                                                                                                      立 17.89 A.
           '
                    I
                                    .       l25J2+
                                                                                     hl0+ 25+                                (1뺍)
                                                                                                                                        2                  +(t
                                                                                                                                                                                '25)
                                                                                                                                                                                             +4]

      c) 1lllS 브 17.95 A.

      d)
                                                                                                                                                   l

                                                                                                25 x 104 2尸dt] '
                                                                          JO.
                                                                                     02
                    ／小
                                ,   =                ［그H
                         " n'                                ·02
                                                                                                                                                   "
                                                                                                                                                       l
                                                                                                                            t3 U02
                                    =          [(50)
                                                                 (25/ 10                          ")
                                                                                                                        2
                                                                                                                                    0

巫스    (V = (2劫r X 10小 = 2000 rad/s.

      From Problem 18.3,

      V55 = 40 Sfl 10,000t V,

      Z5 = 73.2 + [200(- j200)/(200 -1200)] = 173.2 -j100 = 200 /_코0 Q,

      15 = [(40四D仄200느크畇］ = 0.2旦rA,

      P5 = [40(0.2)12] cos (- 30') = 3.46 W.

18

               C,
                     戶
                            =
                                        i
                                                       j   f 戶. .
                                                            5;
                                                                     (-
                                                                                 . - U . ..,.r. .
                                                                                0.
                                                                                          2e_
                                                                                                 "1
                                                                                                           .', .   y)
                                                                                                                            dt +        'T-
                                                                                                                                              rT
                                                                                                                                                           T
                                                                                                                                                                      n = H .,,,,,,r . 1
                                                                                                                                                                     0.
                                                                                                                                                                           "' 伊dt
                                                                                                                                                                          2e'
                                                                                                                                                                                             ，
                                = j (02lnsc)[1 - cos nwot],                                                                                       VR = ZI; therefore, H (s) = V/I = Z.
               (liz) = [(IJR) + (l/sL) + sCJ,
               therefore, Z = H (s) = (1/C)s/[s2 + (1/RC)s + (1/LC)]
                                                                 = 2.5 x 106s/(s2 + 500s + 108).
               m0= 2r x 106/628.3185 = 10 krad/s,                                                                                                                                      ff010,000) = 5000LQ (Z
Solutions for Supplementary Problems                                        435




          H (J20,伉目） = 166.57乙二坐型Q,            H (j30,OC目） = 93.73乙쁘聖望Q,
          C1. = j (0.2hr)[1 - cos (r/4)] = 0.0186 L2Q A,

          therefore, C1. = (0.0186 /   )(5000四) = 93.23 /       V,

          V1(rms) = [2(93.23)/v万] = 131.85 V
          尸1 = [(131.85)2/5어刃］ = 3.48W,        C2. = (0.1r)匹人

          c2v = 5.30／끄I으V,        匕 (rn好） = 7.50 V,        尸2 = 11.25 mW,

          C3. = jO.0362 A,     C3, = 3.40j 1.0즈 V,     V3(rms) = 4.80 V,

          尸3= 4.61 mW; therefore, 尸 斗 尸1 + 尸2 + 尸3= 3.49W.
436                                                                                                Chapter 19



Chapter 19
19.1                                                                                      3+j
        a)   H
                 (s)   =   "g
                                =   [(3 + s)   /(4
                                                     + s)]; therefore,   H
                                                                             (w)     =


                                                                                         (4 +jw)
                                                                                         (
             q (w) = 10[7rd（口）) + (1加出 therefore


             1(w) = '叫았汀"니烈芻 如) + I (w),
             ii（卜亡乙 '畔援｝jw) d:wd：娑目日乃八
             , (w') = 10(3+ jw)                KO ,      K1    =1.: ,              2.c       "
             12佃．)＝風；小；乙計 4＋뇨 커計 3W
                                n.;mand
             i2(t) = 3.75sgnt + 2.5e4iu(t) A,
                                                               5ee4iu(t) A
             therefore, i = i1(t) + i2(t) = 3.75 + 3.75sg可 + 2.

                                = [7.5 + 2.5ee4iJu(t) A.




                                               斗
       b)
                                      （』   ）                      小          小               士


19고    a) H (s) = [VIVg] = (1/RC)/[s + 1/RC] = 2.5/(s + 2.5),

             月（加） = [2.51(2.5 +jw)],                    1슝 = 40(2加D = [80/f口)],

             「喘· 52b뇨貿刈＝쁨 :.5욘加
                2.
             therefore, v(t) = [40sgnt - 80em23'u(t)J V
Solutions for Supplementary Problems                                                                                                           437




       b)
                                                                     V仕）

                                                                                               90 s5r,（七）
                                                                        tv)
                                                                              10


                                                                                               /   /   +   戶




                                                      V (t)                          /
                                                                                       /k卜 - eo e.7·5t LA｛七＼               1   r




프쿄    a) Ig(W) = [1i(2 + jw)] + [1/(2 -jw)],

            H (s) = (VO/1) = R(1/sC)/[R + (1/sC)] = 1/(s + 1),

            //(／口J) = 1/(1 +I口）),                                VO(w) = 月（口))Ig(W),


            乙＠n (:+I小*寸(2如뇨I叫
                             尺9 .     K1     .   K2     ,   K3
                          = 三；I口） 十 (1+ j口J) 十 (2- f口)) 十 (1+ j叫'

            K。= [1/(小1)] = -1,                                   K1 = (1/1) = 1,                               K2 = 1/3,           K3 = 1/3,


            V0（小곰缶 (: 1
                   (2+jw)*(：凹)w) and
            %(0 = {[(4/3)e-1 小 규］n(0 + [(l/3)e刀Ju(- t)} V.

      b) vO(O ) = (1/3) V
      C)
            vO(O+) = (4/3) - 1 = (1/3) V

      d) Use superposition: Let v; = output due to the current source and vO" = output due to
         energy stored in the capacitor at t = 0-.

            Therefore, V; = H (s)Ig(s) = [1/(s + 1)][1/(s + 2)] = [1/(s + 1)] - [2/(s + 2)],

                                        ee   갇]   u    (t)   ,      v          (t)   =   (1/       3) 'u       (t)   ,   and
            v   (t)   =   [em   '   -




            %(0 = [e나 m, e끄 + (l/3)e寸i]n(0 = [(4/3)eh1 m e -刀]u(t) V

      e)    Yes
438                                                                             Chapter 19




                                                        A N.
                                                       .aoO   e   aoo   r4a(1



       b) H(s) = [V。
                   (s)/V,(s)]

                 = s/(s + 100)

           H (w) =jw/[100 +jwj

           ％佃） = 且佃）
                   匕＠).

           Therefore V。
                      (w) = [100/w][jw/(100 + jw)] = j100/(100 + jw) for

           1어） 5 口) 드 200. Thus, I V如）1 = 100/ Vio4 +;;2 for

           1어） 5 cv 5 200 and 1 V。
                                 (w) 1 2 = i0i (10 + w2).




                    l m兀
                                 跏 仙
                                               迂
                                                   如
                       4 1 1 日
      c)
           WIN
                                           2
                                                                                         H1




                                       m
                 = 15.92J


      "나OUT극瑞 (10‘已
                  ，，」』
                  = 10.24J



      e) Percent of input = (10.24/15.92)100 = 64.35%.
Solutions for Supplementary Problems                                    439




      1) H (s) = s/(s + 200),    H(w) = [jwl(200 + jw)J,

          VO(w) = (100/cu)Ijw/(200 + jw)] = [/1001(200 + jo4] and

           I V,(w) 12 = [1041(w2 + 4 x 104)] for 100 5口J 5 200 rad/s;

          11/  - 1 .200
          "our - 元 J l00        [1041(w2 + 4 x 104)]dw = 5.12 J,

          therefore, % of input = [5.12/15.92J(100) = 32.18%.
440                                                                        Chapter 20



Chapter 20
2皿    z11 = (V1/I1)12= 0 = (201 15) + 16 = 4 + 16 = 20 (2,

      Z21 = (V2J11)12 = 0 = [16!i + (5/2S)(lO)I] Ii = 18 Q,

      z12 = (V1/I) 1 = 0 = [1612 + (10/25)(5)I2]/I2 = 18 c,

      Zn = (V2J12)11= 0 = (101 115) + 16 = 6 + 16 = 22Q.

2Q2   First fmd the h-parameters: h11 = (V1/I1) v2=o = 1000 Q,

      九21 = ('7J'i) v卄0＝乳 方12 = (V1/V2)11 =0 = 10巴

      h22 (I7JV2)11 = 0 = 0 = 25u tj ,        스h = 0.025 - 0.005 = 0.02,

      口11 = (- 八h1h21) = -4 x 10며，            a12 = (h11/h21) = 20 (2,

      口21 = (- h22仄21) = 卞（).5/s U ,          口22 = (- 1.伽21) = -0.02

20쿄   Yii = (I1/V1）吃＝0 = (2／加） = 0.1U,

      Y21 (IilVi)v2=o = (- 0.8/20) = -0.04 U,

      Y12 = (Ii/V2)匕 =0 = ( 1.0/25) = -0.04 U,

      Y22 = (I7JV2)v1 = 0 = (1.4/25) = 0.056 U.

20크   With port 2 open, the node-voltage equation at port 2 is
             '/,   V, -4V] V, -Vi
      -j三＋          ' 50' + _ 5  '   =   0,
      a11＝눈 ,,: ,＝프芋느1.951匹흐쏘·
      With port 2 open we also have
Solutions for Supplementary Problems                                                                                                                                                                       441




      【尸知                '2                  i 5 V2
                                                 -




      Thus, a21 = (111V2)12 = 0 = (7.5 + /7.5)114 = 0.756 L4
                                                                 ，【50
                                                                 ,therefore,
                                                                                【6
                                                                               【. 「0, I1
                                                                                      11=             =        0.
                                                                                                               .·3          [
                                                                                                                            +j25 I V2+ 0.
                                                                                                                       3 il 14               j
                                                                                                                                                 t.
                                                                                                                                                               3V2,
      With port 2 short-circuited, we have the circuit shown in the figure.




          4\'i
      L=  -==.                        k=
       (1  50 '                        1J
      12 = ' (Ia + 1b) = (- 14/50)V1,

      a12 = (- V1/I2)v2 = 0 = (50/14) = 3.57샌e (2,

      1l= [(Vl/10) + (Vii5)1 = 0.3V1 = 0.31(- 50/14)I21,

      a22 = (- Ii/12)v2 = 0 = (15/14) = 1.071LQ.

29亞   Let Va be the voltage across the 1000-Q resistor positive at the upper terminal. Let VO equal
      the node voltage from the lower node of the circuit to the node where the 500-a resistor, the
      40-Q resistor, and the output terminal of the op-amp join. Since the op-amp is ide毗 we have
      V1 = 100011; thereforeh11 = l000candh12 = 0. WealsohaveI2 = (V2 - V。              )I40and

      Va = (2/3)J/) = 0.8V1; therefore, VO = 1.2V; thus

      '2 = (- 1.2)140) V1 + (1/40) V2 = -30Ii + 0.025 V2. It follows that h21 = -30 and h22 =
      0.025 U.

2Q血   When '2 = 0, let 'a equal the left mesh current and 'b equal the upper mesh current. Both
      mesh currents are oriented in the clockwise direction. Then Vi = 1(I - Ii,) + Sin and
      n   = /1    ! \   r4   /d . \11 1     1,   !    ／八     J\ ! r . /m 2 八 . d\   1.      1r 1r八 2
      0 = 1(Ih 尸 'a) + [1 + (l/s)Vb; therefore, 'a = (2s + 1)V1/(2se + 2s + 1) andIi, = sV1/(2sH
           =       』 \       1   r           !           d   !                   !   ,   /m      '        八＼         . rm   I   .    八                                                        .


      + 2s + 1); V2 = SIa + 14 = sV1(2s + 2)/(2s ' + 2s + 1); therefore, a11 = (V11V2)j., = 0 =
      ／八 I     m         .       d\   . r八   /       .   d   \1                           /r   11 r       \                         ／八   .   d   \   1r八   /          .   4\   1   rm띠1   .       1   .U    1

      (2s' + 2s + 1)/[2s(s + 1)], a21 = (I1/V2)12 = 0 = (Zr + 1)/[2s(s + 1)]. The network is symmet-
      rical and reciprocal; therefore a22 = a11 and a11a22 - a12口21 = 1, and thus a12 = (2s +
      1)/[2s(s + 1)].
442                                                                                      Chapter 20




2Q2    a) g21Z = 2 xl07,          (1 + giiZg) = 叫1,       (g22 + ZL) =Ul04,
            g2Jg21Zg = 6 X i04,     (V2Vg) = -400,       V2 = e 10 = 10 L쁘Q V.

       b) P = [(10/V )2/104] = 5 mW.

       c)
            乙 = 40kQ.

       d) Vt = m2000Vg =50L QV,

            "m카 = L(25/V7 )2/叩，以）())J = 7.8125 mW.

       e)
            Vi = Rc22 + Z) /g21ZJjV2 = -6.25 mV = 6.25 L쁘Q mV,

            Ii = RciiZi. + 스g)/(-g21)]I2,      12 = (5/8) mA,      Il = 31.25／으／iA.

       f)   P = (1/2)(6.25)(31.25)10    cos 1800 = -97.66 mW.

20.8   First calculate the a-parameters for each network: a1t1 = 0.1,


       口12 = 15（刃（2 ,      21 = 1mt5,
                          口’                 口力 = 10,      口； = 0.04,

       a立 = 1040Q,        a云 = 0.5 mU,        口亡 = 8.

       Now calculate the a-parameters for the cascade connection: a11 = 0.754, a12 = 12,104 (2,
       a21 = 5.04 m U,      a22 = 81.04. Finally Zin = [(a1iZL + a12)/(a2lZL + a22)] = 149.42 (2.
