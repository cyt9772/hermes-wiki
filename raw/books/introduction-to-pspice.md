---
source_url: /run/media/yutae/Data/Introduction_to_PSPICE.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: af3dad686af2bb705dbee41a5991113e1fb3098b411b1197bbbceb798cb374a5
---

# Introduction to PSpice — A Supplement to Electric Circuits (4th ed) (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출. 일부 토큰은 원서 원형과 미묘히 다름 (인식 오류 아님, text-layer 원본). 원문 PDF(`/work/wiki/raw/books/Introduction_to_PSPICE.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Introduction to PSpice — A Supplement to Electric Circuits (4th ed)
- authors: James W. Nilsson · Susan A. Riedel (McGraw-Hill)
- pages: 156 (pdfinfo)
- source file: `Introduction_to_PSPICE.pdf` (sha256: `af3dad686af2bb70…`, 134 MB)
- extract: `pdftotext -layout` @ 2026-10-25, 373,638 chars

## Original text (all 156 pages)

Introduction to PSpice
         A Supplement to
       ELECTRIC CIRCUiTS
        FOURTH EDITION


    James W. Nilsson
     Susan A. Riedel
INTRODUCTION
TO PSPICE@
A SUPPLEMENT TO

ELECTRIC CIRCUITS
FOURTH EDITION



                    JAMES W. NILSSON
                      PROFESSOR EMERITUS
                      IOWA STATE UNIVERSITY


                    SUSAN A. RIEDEL
                      MARQUETTE UNIVERSITY
INTRODUCTION
TO PSPICE@
A SUPPLEMENT TO

ELECTRIC CIRCUITS
FOURTH EDITION




                    JAMES W. NILSSON
                          PROFESSOR EMERITUS
                          IOWA STATE UNIVERSITY


                    SUSAN A. RIEDEL
                          MARQUETTE UNIVERSITY




                     A
                    VT
                    ADDISON- WESLEY PUBLISHING COMPANY

                    Reading, Massachusetts · Menlo Park, California
                    New York . Don Mills, Ontario · Wokingham, England
                    Amsterdam · Bonn · Sydney . Singapore
                    Tokyo . Madrid . San Juan · Milan · Paris
Senior Sponsoring Editor, Eileen Bernadette Moran
Production Supervisor, David Dwyer
Production Coordinator, Genevra Hanke
Copy Editor, Jerrold A. Moore
Text Designer, Sally Bindari, Designworks, Inc.
Illustrators, Capricorn Design
Cover Designer, Peter M. Blaiwas
Senior Manufacturing Manager, Roy Logan
Compositor, Interactive Composition Corporation

PSpice is a registered trademark of MicroSim Corporation. All other
MicroSim product names are 仕ademarks of MicroSim Corporation.
Representations of PSpice/Design Center screens are used by per址s-
sion of and are proprietary to MicroSim Corporation. Copyright 1992
MicroSim Cor兀ration.

Many of the designations used by manufacturers and sellers to distin-
guish their products are claimed as trademarks. Where those designa-
tions appear in this book, and Addison-Wesley was aware of a trade-
mark claim, the designations have been printed in initial caps or all
caps.

The programs and applications presented in this book have been in-
cluded for their instructional value. They have been tested with care,
but are not guaranteed for any particular purpose. The publisher does
not offer any warranties or representations, nor does it accept any li-
abilities with respect to the programs or applications.

Copyright C) 1993 by Addison-Wesley Publishing Company, Inc.

All rights reserved. No part of this publication may be reproduced,
stored in a retrieval system, or transmitted, in any form or by any
means, electronic, mechanical, photocopying, recording, or otherwise,
without the prior written permission of the publisher. Printed in the
United States of America.

ISBN 0-201-51318-8

3 4 5 6 7 8 9 10-DO-959493
                                                                       'Ii




PREFACE

ABOUT THIS MANUAL

In什O加Ct加n to P旬兀ce回 expressly supports the use of PSpice回
(or SPICE) as part of an introductory course in electric circuit
 analysis based on the textbook Electric Circuits, Fourth 晟ition.
This supplement focuses on three things: (1) learning to write
PSpice programs; (2) constructing circuit models of basic devices
 such as op amps and transformers; and (3) learning to challenge
 computer output data as a means of rein向rcing confidence in
 simulation. Because PSpice is designed to simulate networks
 containing integrated circuit devices, its range of application
 goes well beyond the topics covered in the textbook. Even
 though we do not exploit the full power of PSpice, we begin the
 introduction to this widely used simulation program at a level
 that you can use to test the computer solutions.
     The use of PSpice involves learning a significant new technical
  vocabulary and a number of specialized techniques. Hence, we
  designed this supplement to stand on its own as an instructional
  unit. Our decision to separate this material from the parent text-
  book also is a service to you: The portable format greatly 包cili-
  tates your use of the supplement at a computer terminal. In this
  format the supplement adds value, but not cost, to your study.
  This supplement is provided to purchasers of the text without
  any adjustment to the price of the textbook.
     Introduction to PSpice contains 67 problems. We designed
  these problems with two objectives in mind: (1) to teach you
  how to construct PSpice source files; and (2) to teach you the im-
  portance of checking the output from PSpice simulation to en-
   sure that the computer-generated solution makes sense in terms
   of known circuit behavior. Complete solutions to these problems
iv    PREFACE


      a七 included in the solutions manual for Electric Circuits. You
      may also use PSpice to solve many of the textbook's Drill Exer-
      cises and chapter Problems.




      INTEGRATING PSPIcE INTO INTRODUCTORY
      CIRCUITS COURSES

      Although some circuits courses cover PSpice as an independent
      topic, many instructors prefer to integrate computer solutions
      with the course. We used the following methods to support such
      integration: (1) notations in the margin of the textbook (marked
     in color by a logo and the acronym PSpice) refer to sections in
      the supplement that relate to the topic under study in the text-
     book; (2) topics appear in this supplement in the same order in
     which they are presented in the text; (3) notations in the margin
     of this manual (marked in color by a logo and the name Nilsson)
     refer to sections in the textbook that relate to the topic described
     in the manual; and (4) the accompanying table relates topics in
     the supplement to topics in the textbook.




     ABOUT PS이任

      SPICE is a computer-aided simulation program that enables you
      to design a circuit and then simulate the design on a computer.
      SPICE is the acronym for a Simulation Program with Integrated
     Circuit Emphasis. The Electronics Research Laboratory of the
     University of California developed SPICE and made it available
      to the public in 1975.
        Many different software packages are available that imple-
     ment SPICE on personal computers or workstations. Among
     them, PSpice, from MicroSim Corporation, is the most popular.
     PSpice's popularity can be attributed to many factors, including
     its user-friendly interface, extensions to Spice that support mod-
     eling of digital circuits and much more, and its no-cost student
     version. This manual focuses on how to use PSpice, a superset of
     SPICE. We summarize differences between PSpice and SPICE
     in Appendix C and also mention them as appropriate in this sup-
     히ement.
                                                                     PREFACE   V


      We limited our applications of PSpice to the types of circuit
   problems discussed in the textbook. Although PSpice is a general
   purpose program designed for a wide range of circuit simula-
   tion-including the simulation of nonlinear circuits, transmis-
   sion lines, noise and distortion-here we discuss the use of
   PSpice only for dc analysis, transient analysis, steady-state sinu-
   soidal (ac) analysis, and Fourier Series analysis.



   八ANUAL                                                             TEXT
   CHAFfER                             TOPIC              PROBLEMS   CHAPTER
   2-4                         DC Analysis and Output       1-8         2
   5                           Op Amps                      9-10        6
   6刀                          Transient Analysis          11口         乙8




8 llllllll
                               Sw如hes                      18中23        8
                               Step Response               24-32       8, 9




       0 l n二 그1V 41 5U 6 m/
                               Varying Component Values    33-34        9
                               AC Steady-State Analysis    35-39        10
                               AC Power                    的42          11




 /
 0
                               Mutual Inductance           43-46        13
                               Ideal Transformers          47-48        13
                               Frequency Response          49-56      14, 17
                               F뇨lsed Sources              57寸64        18
                               Fourier Series Analysis     65-67        18
                                                       VII




CONTENTS

CHAPTER 1   PSPI E IN GENERAL 1
    1. 1 The Data Statements 4
    1.2 The Control Statements 4
    1.3 The Output Statements 5

CHAPTER 2   DATA STATEMENTS FOR DC ANALYSIS 7
   2.1 Independent DC Sources 7
   2.2 Dependent DC Sources 8
   2.3 Resistors 11

CHAPTER 3   CONTROL STATEMENTS FOR DC ANALYSIS 15
   3.1 The .OP Control Statement 15
   3.2 The .DC Control Statement 16
   3.3 The .TF Control Statement 17
   3.4 The .SENS Control Statement 21

CHAPTER 4   0UTPUT STATEMENTS FOR DC ANALYSIS 23

CHAPTER 5   0PERATIONAL AMPLIFIERS 29
   5.1 Modeling Op Amps with Resistors and Dependent
       Sources 29
   5.2 Modeling Op Amps with Subcircuits 31
   5.3 Using Op Amps Library Models 34

CHAPTER 6   INDUCTORS AND CAPACITORS 37
viii   CONTENTS


       CHAPTER 7    TIME-DEPENDENT CIRCUIT RESPONSE 39
           7.1 Exponential Pulse Sources 39
           7.2 Transient Analysis 40
           7.3 Time-Response Output 41
           7.4 Natural Response 43

       CHAPTER 8    SWITCHES 49
           8.1 Piecewise Linear Source 49
           8.2 Voltage- and Current-Controlled Switches 51

       CHAPTER 9    STEP RESPONSE 53


       CHAPTER 10 VARYING COMPONENT VALUES 57


       CHAPTER 11   SINUSOIDAL STEADY-STATE ANALYSIS 61
          11.1 Sinusoidal Sources 61
          11.2 Sinusoidal Steady-State Response 62

       CHAPTER 12 COMPUTING AC POWER WITH PROBE 67


       CHAPTER 13 MUTUAL INDUCTANCE 71


       CHAPTER 14 IDEAL TRANSFORMERS 73


       CHAPTER 15   FREQUENCY RESPONSE 75
          15.1 Selecting Frequency Variation and Number   75
          15.2 Frequency Response Output 77
          15.3 Bode Plots with PROBE 80

       CHAPTER 16 PULSED SOURCES 85


       CHAPTER 17 FOURIER SERIES 89


       CHAPTER 18 SUMMARY 97
                                              CONTENTS   Ix



APPENDIX A   GUIDE TO PSPICE CONTROL SHELL AND PROBE
             MENUS 99


APPENDIX B   SPECIFYING PSPIcE SIMULATION
             PARAMETERS 111


APPENDIX C   DIFFERENCES BETWEEN SPICE AND PSPICE 113


APPENDIX D   QUICK REFERENCE TO PSPICE 115


PROBLEMS 131

ANSWERS TO SELECTED PROBLEMS 149

IND태 153
                                                                                1




CHAPTER 1


PSPICE IN GENERAL

I he general procedure for using PSpice consists of t뇨ee basic
steps. In the first step the user creates a source file for the circuit
to be simulated or analyzed. In the second step the user enters
the source file into the computer, which then runs the program
and creates an output file. In the third and final step the user in-
structs the computer to print or plot the results of the output file.
   Before we discuss creation of the source file, some general
comments about the PSpice format are in order.t
1. Each statement in the source file may have several constituent
parts. These parts, called fields, must be in a specific order but
may appear anywhere in the line. Fields may be separated by one
or more blanks, a comma, or a tab. In certain instances, equal
signs or left and right parentheses are used as separators.
2. A statement in the source file cannot be longer than the 80
characters that fit in a single line on the computer display. A
longer statement may be continued on the next line by including
a plus sign (+) in column 1 of the next line, followed by the re-
mainder of the statement.
3. PSpice does not distinguish between uppercase and lowercase
characters. For example, "yIN", "Vin", and "yin" are equiva-
lent. This usage does not hold for SPICE, where all characters in
the source file must be uppercase-lowercase characters are not
permitted. In this manual we use the convention of uppercase
for PSpice keywords and lowercase for all other words. Thus if



tA. Vladiniirescu, K. Zhang, A. R: Newton, D. 0. Pederson, and A. Sangio-
vanni-Vincentelli, SPICE Version 2G User's Guide, University of California at
Berkeley, unpublished; PSpice Circuit Analysis, Version 5.0. MicroSim Corpo-
ration, Irvine, Calif., 1991.
2    PSF니（正 IN GENERAL


     you attempt to use any of the example programs in this manual
     as inputs to SPICE, you must first convert characters to upper-
     case.

     4. A name field must begin with a letter "a" through "z" (or "A"
     through "Z"), but the characters that follow may be letters, num-
     bers, or any of the following: "$", " -", ", "I", and "%".
     Names may be up to 131 characters long, but choosing a more
     reasonable length (say, 8 characters) is preferable. In SPICE,
     name fields may not contain any delimiters, and only the first 8
     characters of the name are used.

    5. A number field may be an integer (4, 12, -8) or a real num-
    ber (2.5, 3.14159, -1.414). Integers and real numbers may be
    followed by either an integer exponent (7E-6, 2. 136e3) or a
    symbolic scale factor (7U, 2.136k). Table 1 summarizes the
    symbolic scale factors used in PSpice and their corresponding ex-
    ponential forms. Letters immediately following a number that
    are not scale factors are ignored, and so are letters immediately
    following a scale factor. For example, 10, l0v, 10HZ, and l0A
    all represent the same number, as do 2.5m, 2.5MA, 2.5msec,
    and 2.5MOhms.

    6. The first statement in the source file is the title line, which
    may contain any type of text. The title line is ignored by PSpice,
    except to label the output upon completion of the analysis.

    7. The last statement in the source file must be . END. Note that
    the period is part of the statement.

    8. An " 永" in the first column marks comment lines. Comments
    may contain any text and are ignored by PSpice.

    9. Except for the title line, subcircuit definitions, the
    .OPTIONS statement with the . NOECHO parameter, and the
    . END statement, the order of the statements in the source file
    does not matter.

       In creating a source file to direct PSpice to analyze a circuit,
    you must do three things. First, you must describe the circuit to
    be analyzed; second, you must state the type of analysis to be
    performed; and, third, you must specify the desired output. For
    convenience you should therefore divide the source file into
    three major subdivisions.
                                              PSPICE IN GENERAL         3


TABLE 1
PSPICE S址E FACTORS
SYMBOL                  EXPONENTIAL FORM                     VALUE
F (orf)                         le-15                         101's
P (or p)                        le-12                         10U12
N (orn)                          le円                          10四
U 佃ru)                           le小                          10小
卜vi 佃r m)                        le-3                         10日
K (or k)                          1e3                         io3
MEG (or meg)                      1e6                         106
G (or g)                          1e9                         109
T (or t)                         1e12                          1012



   One subdivision consists of data statements that describe the
circuit being simulated. Another comprises control statements
that describe the type of analysis to be performed. The other
contains the output specification statements, which control what
outputs are to be printed or plotted. Although these subdivisions
may be placed in any order in the source file, we will adopt the
following convention in this manual: the data statements will ap-
pear first, followed by the control statements, followed by the
output statements.
   In addition to these major statement subdivisions, the source
file must include two other statements. The first line of the
source file must be a title statement and the last line of the source
file must be an end statement.
   You may create the source file with any text editor available
on your system, so long as this editor does not insert any control
characters. Most word processors make extensive use of control
characters and so are generally not suited for creating PSpice
source files. If your word processor has a configuration in which
text can be created without the usual control characters, you may
then create PSpice source files by using this configuration.
   Also, if you are using PSpice within the Control Shell, the
Files menu contains a text editor that you may use to create the
source file. Working within the Control Shell has other
significant advantages, such as the online help manual, which
can assist in creating and modifying source files. See Appendix
A for a detailed explanation of the Control Shell.
   We now take a closer look at the three major subdivisions
within a PSpice source file: the data statements, which describe
the circuit; control statements, which specify the type of analysis
and the output statements, which describe the type and format of
the output.
 4                                                      PSPICE IN GENERAL


                                                        Li THE DATA STATEMENTS

                                                         PSpice is based on nodal analysis. Therefore the first step in de-
                                                         scribing a circuit to PSpice is to number all the nodes in the cir-
                                                         cuit. The reference node must be numbered zero (0). The re-
                                                         maining nodes must be numbered with nonnegative integers but
                                                         they need not be sequential. After numbering all the nodes in a
                                                         circuit, you can describe a circuit completely by identifying the
                                                         type of element connected to the nodes. In addition to describing
                                                         the type of element, you must also specify its numerical charac-
                                                         teristics. PSpice places several restrictions on the topological
                                                         characteristics of a circuit. Therefore, when describing a circuit,
                                                        you must make sure that (1) every node has at least two connec-
                                                         tions; (2) each node in the circuit has a dc path to the reference
                                                        node; (3) the circuit does not contain loops of either voltage
                                                        sources or inductors; and (4) the circuit does not contain cut sets
                                                        of either current sources or capacitors.
                                                            The description of each passive circuit element and each inde-
                                                        pendent source must contain three pieces of information: the
                                                        type of element, two nodes to which it is connected, and its nu-
                                                        merical value. The description of each controlled or dependent
                                                        source must contain four pieces of information: the type of ele-
                                                       ment, the two nodes to which it is connected, the controlling
                                                       nodes, and its numerical value. The format for each element data
                                                        statement consists of (1) the element name, (2) the circuit nodes
                                                        to which the element is connected, and (3) the values of the
                                                       parameters that describe the behavior of the element. The ele-
                                                       ment name must start with a letter of the alphabet.
                                                           Before concluding this overview of data statements, we need
                                                       to pause and comment on polarity references. In PSpice, when
 NnSSOn
 1끼11:5 b(J11    Polarity references for voltage and   polarity is relevant to the behavior of the element, the first node
current: Section 1.6, p. 15
                                                       is positive with respect to the second node. T址s condition im-
                                                       plies that the current reference direction is from the first-named
                                                       node to the second-named node.




                                                       1.2 THE CONTROL STATEMENTS

                                                       As we mentioned earlier, PSpice was developed to analyze cir-
                                                       cuits containing integrated-circuit devices. One of the important
                                                       aspects of such analysis is to determine the dc operating point, or
                                                       bias level, of the circuit. As a result, PSpice automatically per-
                                                       forms a dc analysis prior to both transient and ac analysis.
                                  1 . 3 THE OUTPUT STATEMENTS            5


Therefore you may obtain a dc solution by just describing the
circuit.
   When other than simple dc analysis is desired, a control state-
ment is used. The control statement consists of a PSpice com-
mand followed by fields that describe the parameters of the de-
sired analysis. The number and type of these parameter fields
depend on the type of analysis to be performed. The analysis
commands described in this manual include . DC for complete dc
analysis, . AC for ac analysis (frequency response), . TRAN for
transient analysis (time response), . FOUR for Fourier Series
analysis, . OF나o co呻ute the dc operati璡 point of a circ毗 皿ior
to other analysis, and . TF to compute the gain, input resistance,
and output resistance (the transfer function). We present detailed
descriptions of these commands later in this manual.




1.3 THE OUTPUT STATEMENTS

PSpice output has several constituent parts. The presence of each
of these parts and the format used in the presentation is con-
trolled by the output statements in the source file. We briefly de-
scribe these statements here and discuss them in more detail
later in this manual.
   The first section of the output file is the description of the cir-
cuit itself. At a minimum this section includes a listing of the
source file created for PSpice to use in analysis.
   The second section contains the default output from some of
the analysis commands, which generate output without any spe-
cific directions from the source file. For example, the . TF corn-
mand always causes the gain, the input resistance, and the output
resistance to be printed in the output file after analysis is com-
히ete.
   The third section contains the printout and line printer plots
that have been explicitly requested in the source file. You use the
.PRI町 command to print data from the analysis. This state-
ment includes fields that specify the type of analysis that gener-
ated the data and a list of the circuit variables whose values are
to be printed. You use the . PLOT command to create line print-
er plots of data generated during PSpice analysis. The plot state-
ment includes the same fields as the print statement.
   The fourth section contains information that summarizes some
statistical information describing the execution of PSpice. This
information includes the memory requirements and the execu-
tion time and may be used in conjunction with the specification
6   PSPICE IN GENERAL


    of some optional parameters to make your analysis more
    efficient.
       In addition, the PSpice software is packaged with a graphics
    postprocessor called PROBE. It permits you to plot virtually any
    value of interest after PSpice has analyzed the circuit you have
    described. PROBE needs access to a special data file in order to
    function properly. You may generate this data file during PSpice
    analysis by including the . PROBE command in your source file.
    After PSpice has completed an error-free analysis of your cir-
    cuit, you may activate PROBE either at the operating systems
    level or from the Command Shell. We describe PROBE in more
    detail later in this manual.
CHAPTER 2


DATA STATEMENTS
FOR DC ANALYSIS
We begin our description of PSpice data statements with those
that specify dc current and voltage sources. First, we present in-
dependent sources and then dependent sources. Whether inde-
pendent or dependent, these sources are described in data state-
ments consisting of four fields. The specific purpose of each field
varies with the type of source being specified. We conclude with
resistors, for which the data statements consist of three fields.




2.1 INDEPENDENT DC SOURCES

Data statements used for specifying independent dc sources in-
dlude four fields. The first field is the element name, which must
consist of a unique string of characters, the first letter of which         NnSSOn Ideal independent voltage and cur
                                                                            IHbbUtI
identifies whether the element is a voltage source or a current       rent sources: Section 2.1, pp. 26-27
source. If we let xxx denote an arbitrary alphanumeric string,
then element names for independent sources must conform to the
following convention:

                                             恕岫
                                                  n   m   m
       Type of Element
       Independent voltage source
       Independent current source
  The second field contains the node numbers identifying the
branch in which the dc source is located. The order in which the
nodes are listed determines the polarity of the source. For a
voltage source, the first node is positive with respect to the sec-
ond node. For a current source, the current direction through the
source is from the first node to the second node.
 8                                                     DATA STATEMENTS FOR DC ANALYSIS


                                                         The third field identifies whether the source is constant or time
                                                       varying, with a dc source indicated by DC in this field. Finally,
                                                       the value of the dc source goes in the fourth field. For a voltage
                                                       source, this value has the units volts, and for a current source the
                                                       units are amperes.
               100 V(dc)                                 For instance, the data statement for a 100-V dc voltage source
                                  1 ]                  named Vsourcel connected to nodes 1 and 0, as shown in Fig. 1,
                                                       would be:
FIGURE 1 A 100-V dc source connected to nodes
1 and 0, with node 1 positive with respect to                  Vsourcel
                                                               나尸／
                                                                                      1 0                DC         100             t
                                                                                     니4尸／              뇨＝小尸／       니m戶／


node 0.                                                           Name              Node               Type of     Value
                                                                                 connections            source
                                                        If we reverse the order of the nodes in the description of the
                                                      source in Fig. 1, we enter the value as a negative number:
                                                                        Vsourcel            0 1   DC     -100.
                                                        In PSpice you may use an independent voltage source of zero
                                                      value as an ammeter. That is, in order to measure a current, you
                                                      may insert a zero-valued voltage source in series with the ele-
                                                      ment where the current is to be determined. The zero-valued
                                                      voltage source does not disturb the circuit because it is equiva-
                                                      lent to a short circuit. These zero-valued voltage sources are
                                                      necessary because the only current that PSpice is designed to
                                                      output is the current through sources.




                                                      2.2 DEPENDENT DC SOURCES

                                                      In discussing the data statements for dependent sources, we di-
                                                      vide them into voltage-controlled sources and current-controlled
                                                      sources. The description of a dependent source requires four
 kfl冶＄0n
 1111口11J11     Ideal dependent voltage and current   fields. The first field contains the name of the source, with the
sources: Section 2.1, pp. 27-28
                                                      first letter of the name identifying the type of dependent source.
                                                      The second field contains the node numbers identifying the
                                                      branch in which the source is located. The third field contains
                                                      the node numbers of the controlling branch if the source is
                                                      voltage controlled. If the source is current controlled the third
                                                      field contains the name of the zero-valued voltage source used to
                                                      compute the controlling current. The fourth field contains the
                                                      gain of the dependent source, which is the ratio of the output


                                                      tT址s computer-like typeface is used here and in all other examples when the
                                                      text can be typed verbatim in a PSpice source file.
                                          2. 2 DEPENDENT DC SOURCES                                                                                  9


quantity (voltage or current) to the controlling quantity (voltage
or current).
  For a voltage-controlled voltage source, the format is:
        且txx            Ni N2             NCi NC2               VALUE                 十
        니尸／             나H/                1小m1                 니-        ---




        Name            Node              Controlling           Voltage
                     connections            nodes                gain
                                                                                                                    15 n
   For instance, consider the circuit shown in Fig. 2, where the
dependent voltage source is named ES2. The data statement for
this voltage-controlled voltage source is:
           ES2                4 3                      1 2                        3
        Name               Node                   Controlling                   Voltage
                        connections                 nodes                        gain     V스
  Note that the order of the nodes is relevant to the proper de-
                                                                                          +




scription of the source. Node 4 is positive with respect to node
3- hence the order 4, 3. The reference polarity for the con-                              FIGURE 2 Circuit used to illustrate the data state-
trolling voltage v is positive at node 1; therefore the order of                          ment 幻ray이tage-contr에ed v이tage source.
the controlling nodes is 1, 2.
   The format of the data statement for a voltage-controlled cur-
rent source is:
       Gxxx            Ni N2              NC1 NC2                VALUE
      나YH/             니寸尸／               나卜H1/                  니V1/


      Name             Node              Controlling            Transcon-
                    connections            nodes                ductance
  The data statement for the voltage-controlled current source
in the circuit shown in Fig. 3 and called GS04 is:                                                                  5n
                                                                                                                    八八

                                                                                                                +   V스

      GS04              2 3                   1    3                  0. 2
      나＼   H/          니尸／                   나H/                     나H



      Name             Node              Controlling            Transcon-                                                           0.2vA
                                                                                                      8n            2
                    connections            nodes                ductance                              vvv            r
                                                                                                                                  \\//                   3
                                                                                                                                               e
  Here again the order of the nodes is essential to the proper de-
                                                                                                                     1
                                                                                                                              n                 /
                                                                                                                                                <
                                                                                               ov                    >>
                                                                                                                          n
                                                                                                                          /                 10 n :
                                                                                                                     L
scription of the voltage-controlled current source. The reference                                                                                    1
direction for the current source is from node 2 to node 3; there-                                      6！二．
                                                                                                                                                     1
fore the order of the node connections is 2, 3. The controlling
voltage, 工J스, is positive at node 1; thus the order of the con-                           FIGURE 3 Circuit used to illustrate the data state-
trolling nodes is 1, 3.                                                                   ment for a voltage-controlled current source.
   A current-controlled source requires insertion of a zero-valued
voltage source into the circuit to measure the controlling cur-


十Thenormal uppercase typeface is used here and in all other examples when the
source file elements are identified by descriptive placeholders. These placehold-
ers cannot be typed verbatim in a PSpice source file. They must be replaced by
values that PSpice expects.
10                                                                          DATA STATEMENTS FOR DC ANALYSIS


                                                                            rent. After you name this zero-valued voltage source, you enter
                                                                            it in the appropriate field in the data statement for the current-
                                                                            controlled source.
                                                                               The format of the data statement for a current-controlled
                                                                            voltage source is:

                                                                                       H兀工工               Ni N2                     \／工工工          VALUE
                                                                                                          나＼       m1i
                                                                                                                                    니中尸            나m尸1



                                                                                   Name of          Node                         Name of the      Trans-
                                                                              current-controlled connections                      zero-valued   resistance
                                                                                voltage source                                  voltage source
                       4O!                                                                                                     used to measure
                                                                                                                                the controlling
                                              50!
:20c! 中 ／스
                                                                <
                                                                                                                                    current
                                                                < <




                                                                      >>>      The polarity of the current-controlled voltage source is rele-
                                              Bi\                           vant to the behavior of the device; hence the order of the nodes
                                                                            is important. As before, Ni is positive with respect to N2. Note
                                                                            also that the controlling current is directed into the positive ter-
                                     <>
FIGURE 4 Circuit used to illustrate the data state-                         minal of the zero-valued voltage source.
ment 幻r a Cu口帥卜contr에ed v이tage source.                                         Consider the circuit shown in Fig. 4, which contains a current-
                                                                            controlled voltage source. Then consider the same circuit re-
             VDELTA
                                                                            士awn in Fig. 5, with the nodes numbered and a zero-valued
                                          in                                voltage source labeled Vdelta inserted in series with the branch
             \q』
                   ／                                                        containing iA. For the current-controlled voltage source named
                                                                            HS01, the pertinent data statement is:
                             ;4n                      247.5 V


                        31
                                              1!                                 HS01              4 0                         Vdelta              8
:,20O!
         a                                V   V   V                              나尸／              니1H/                     <
                                                                                                                           /                   나V尸／



                                                                                 Name              Node                    Controlling         Trans-
                             '10!!
                                                                                                connections                 current          resistance
                                          +                                   The source file also contains the data statement describing the
                                          HS0 1                             zero-valued voltage source:
디GURE 5 The 이rcu仕 shown in F呼 4, with the
nodes numbered and the zero-valued voltage                                             Vdelta                  2 5                   DC                0
                                                                                       \m1卜H/              나／        =m/                           니尸／


source inserted to measure the Current ia.                                              Name                Node                   Type of         Value
                                                                                                         connections               source

                                                                               The format for the current-controlled current source is:

                                                                                        F兀x工               Ni N2
                                                                                                           \=HH/
                                                                                                                                      V兀x工             VALUE
                                                                                       나尸／
                                                                                                                                      1m尸／             나＼   H/



                                                                                   Name of                  Node                  Name of the            Current
                                                                              current-controlled         connections               zero-valued            gain
                                                                                current source                                   voltage source
                                                                                                                                used to measure
                                                                                                                                 the controlling
                                                                                                                                     current
                                                                   2. 3 RESISTORS                                                          11


  Assume that the current-controlled current source in the cir-
cuit shown in Fig. 6 is labeled Fl and that the zero-valued
voltage source used to measure the controlling current is called
Valpha. Then the data statements describing the dependent
source and the zero-valued independent source used to measure
the current are:
                        Fl
                          Vaipha
                                                  0 1
                                                  0 5
                                                          Vaipha
                                                          DC
                                                                   0. 1
                                                                    0
                                                                                                                                VALPHA
                                                                                                                                         C
                                                                                                   Fl


                                                                                    FIGURE 6 Circuit containing a current-controlled
                                                                                    current source used to illustrate the data state
2.3 RESIsTORS                                                                       ments for this type of source.

Data statements used for specifying resistors include three fields.
The first is the element name, which must consist of a unique
string of characters, the first of which is "R" (or "r") to identify
the element as a resistor. The second contains the node numbers
that identify the branch in which the resistor is located. The third
contains the value of the resistance, in ohms.                                           Nilsson        Resistors and Ohm's law: Section
  The format for identifying a 100-fl resistor named RX7 con-                       2.2, pp. 29-32
nected to nodes 7 and 12 is:
           RX7                                    7 12             100
          Name                                     Node            Value
                                                connections
We can now illustrate a PSpice source file for a resistive circuit
by constructing one for the circuit shown in Fig. 5:

  Example of a Resistive Circuit                               in PSpice




                 3 22 34 2 l 4
  듬：           0    5




                                 i 3 45 5 0 0
                    1
  Rc        2 3     4
  Rd        3 4     10
  Re        4 5     20
  Vdelta    2 5     DC     0
  Vi        1 0     DC     247.5
  HSOI      4 0     Vdelta     8
  .END


  We stated in Section 1.2 that you may perform a simple dc
analysis without providing control statements or output state-
ments in the source file. That is, only data statements that de-
scribe the circuit are needed. To illustrate this type of analysis
we use PSpice to find the node voltages and source currents in
the circuit shown in Fig. 6.
12                                                             DATA STATEMENTS FOR DC ANALYSIS


                                                                  The input source file is:

                                                                  Example of Sim口le DC Analy드I드
                                                                  Fl        0 1     Vaipha   0. 1
                                                                  Valpha    0 5     DC       0
                                                                  Vi        21      DC       20
                                                                           40345
                                                                  Ri            10
                                                                  R2           22
                                                                  R3            2
                                                                  R4       i4233
                                                                               3. 6
                                                                  R5           68
                                                                  .END


                                                                 The pertinent printed output data are:


                     NODE     VOLTAGE                NODE       VOLTAGE             NODE    VOLTAGE           NODE        VOLTAGE


                 (       1)     -14. 1230        (        2)        5. 8770     (      3)     3. 2967     C          4)    -1. 1732

                 (       5)        0. 0000




                       VOLTAGE SOURCE CURRENTS
                       NAME         CURRENT

                       Val口ha              -4. 84日E-02
                       Vi                  -1. 2弓0E＋야：)

                       TOTAL POWER DISSIPATION                      2. 5日E+01       WATTS


                                                               Voltages are given in volts, and currents are given in amperes.
                                                               Note that the PSpice output format uses "E" for the exponential.
                                                               This is equivalent to "e" used in this manual.
                                                                  The total power dissipation value is automatically printed
                                                               whenever you invoke simple dc analysis. In PSpice this power
NnSS0n
 '111a)1J11     Definition of power for a basic circuit        represents the net power generated by the independent voltage
element: Section 1.6, pp. 14-15
                                                               sources in the circuit. If a dependent source or an independent
                                                               current source is generating power, its value is not included. For
                                                               example, in the circuit shown in Fig. 6 the power developed by
                                                               the 20-V source is 25.80 W, and the total power dissipated in the
                                                               five resistors is 25.87 W. The difference of 0.07 W is developed
                                                               by the current-controlled current source. Example 1 presents a
                                                               more dramatic illustration of this situation.
                                                                        2. 3 RESISTORS                                                               13



EXAM P L E                             1

                                                                                                                                        th
a) Use PSpice to find the voltages Va and Vb for the circuit shown
   in Fig. 7.
                                >><
                                                                                                                                    m   때     n
                                                                                                                                              Z

                                <<
b) Use the PSpice solutions to calculate (1) the total power dis-
   sipated in the circuit, (2) the power supplied by the inde-
                                l
   pendent current source, and (3) the power supplied by the
   current-controlled voltage source.                                                           FIGURE 7 Circuit used to check power
                                                                                                뎨ssipation.
S       0 L     U I         I    0     N

                                                                                                                                        1!)
a) The circuit shown in Fig. 7 is redrawn in Fig. 8. Note the in-
   sertion of a zero-value dc voltage source in series with the                                                                         R3

   20-fl resistor. The names of the circuit components are                                                                          VDELTA
                                                                                                                Al    U
   shown to facilitate reading the PSpice source file:                                          024A    (dc)
                                                                                                                                          20.385ia
                                                                                                                              R2
    Circuit   U弓ed t口 Check Power Di目sipat i口n
    Ii          01      DC        24
    Vdeita      1 3     DC        0



                     0002
    Hi      2 0     Vdelta   20. 3846                                                           FIGURE 8 The circuit shown in Fig. 7 redrawn for
    Ri      1 0    5                                                                            PSpice analysis.
    R2      3 0    20
    R3      1 2     1
    .END


    The pertinent PSpice output is:

        NODE         VOLTA日E                     NODE         VOLTAGE            N（玉堤        V口LTA日E           N｛가茫       VOLTAGE


    (          1:)    104. 0000              (          2:>    106. 0000     (          3)    104. 0000




           VOLTAGE SOURC:E c:URRENTS
           NAME          CU！카긋ENT

           Vd日ita                          5 . 冬)OE+OO

           TOTAL POWER DISSIPATION                               O. OOE+00        WATTS

    Hence

                                      Va = V(1) = 104.00 V;
                                      Vb = V(2) = 106.00 V.
14                                                                       DATA STATEMENTS FOR DC ANALYSIS


b) 1.
                      ,
                               1042
                                                     2163.20 W;
                P.
                          =                      =
                                   그
                P5O
                               -        --




               尸20O =
                              쭝＝
                                                     540加W;
                              (1nc - 104'i2
               P1O =          '_    l
                                   __
                                        '   =_       "   '
                                                             4.
                                                                  00W.

              2PmS = 2163.20 + 540.8 + 4 = 2708 W.
     2. P24A(supplied) = 104(24) = 2496 W.
     3. Pn(supp1ied) = 106(2) = 212 W.
  Note that the sum of power dissipated equals the sum of power
supplied. Note also that the total power dissipated given by
PSpice is 0 W, because there are no independent voltage sources
in the circuit!
                                                                        15




CHAPTER 3


CONTROL STATEMENTS
FOR DC ANALYSIS
When other than the simple dc analysis described in Section 1.2
is desired, four dc control statements are available: . OP, . DC,
.TF, and . SENS. (Note that control commands always begin
with a period.)




3.1 THE .OP CONTROL STATEMENT

The . OP (operating point) control statement instructs PSpice to
compute the bias point (the dc operating point) for the circuit. In
fact, PSpice always calculates the operating point because this in-
formation is needed before you proceed with other types of anal-
ysis. Thus the actual effect of the . OP control statement is on
the values printed in the output file. These values fall into three
categories:

  ' voltages at each node;
  ' currents in each voltage source and total power dissipated;
    and
  ' operating points for each device.

  The default output for simple dc analysis (described in Section
1.2) includes all values in the first two categories listed. Thus the
.OP command causes operating point values to be printed for
each device.
  The values that define the operating point depend on the type
of device. For example, the operating point values for dependent
sources are the dc voltage across the device and the dc current
16   CONTROL STATEMENTS FOR DC ANALYSIS


     through the device. If we add the . OP statement to the source
     file in Example 1, we can generate the following output in addi-
     tion to the output produced by the source file used in Example 1:

       共共共卄 CURRENT-CONTR（가. LED VOLTA日E SOURCES


       NA川E              Hi
       V-SOURCE          1. 060E+02
       I- SOURCE        -2. 000E+OO

        From the circuit shown in Fig. 8 note that the voltage drop
     across the dependent source Hi is just the voltage at node 2,
     namely, Vsource = V(2) = 106 volts. The current through Hi
     is equal to the current flowing through R3 from node 1 to node 2
     and can be computed from the node voltages as follows:
                                  V
                            Is啣 = 而
                                  V(1) - V(2)
                                       1
                                  104 - 106
                                      1
                               = 卞2A.




     3.2 THE .DC CONTROL STATEMENT

     The . DC (direct current) control statement allows you to incre-
     ment an independent input source (either voltage or current)
     over a specified range of values. You also specify the size of the
     increment. The general format for the . DC control statement
     contains five fields:
          . DC      SRCNAM        START       STOP         INCR
         니m戶1/      나小尸1/         나Vmm1/      나尸／          뇨寸＼ 小／



       Command       Name of   Starting Stopping Incrementing
                   independent  value    value       value
                     source
     For example, the control statement
                      . DC    VS01     -5   10      1. 0
     causes a dc voltage source named VS01 to start at -5 V and stop at
     10 V, with interim steps of 1.0 V. PSpice analyzes the circuit for
                               3. 3 THE .TF CONTROL STATEMENT           17


each of these discrete values of VS01, so you might have to wait
quite a long time before the analysis is completed.
    The . DC control statement also allows you to sweep a second
independent source over a specified range of values. For each
specified value of the second source, you sweep the first source
through its designated range. Hence, you can use PSpice to gen-
erate a family of characteristics; each member of the family cor-
responds to a specific value of the second source. Designers
often use this feature of PSpice to plot the output characteristics
of semiconductor devices.
    When a second source enters the analysis, the format for the
 . DC control statement contains nine fields. The first contains
 .DC to identify the type of analysis. The next four describe the
 source name, starting value, ending value, and increment for the
first source, just as these fields appear in the . DC statement for a
 single source. The last four describe the source name, starting
value, ending value, and increment for the second source. The
following statement represents symbolically the nine fields.
. DC    SRC1          START1   STOP1    INCRi      SRC2      START2
+      STOP2      끄놔CR2



3.3 THE .TF CONTROL STATEMENT

The . TF (transfer function) control statement enables PSpice to
compute three characteristics of the circuit being analyzed. First,
it computes the ratio of the output variable to the input variable.
This ratio is referred to as the transfer function gain of the cir-
cuit. Second, it computes the resistance with respect to the input
source. Third, it computes the output resistance with respect to
the terminals of the output element. The general format of the
 . TF control statement contains three fields:
               . TF             OUTVAR             INSRC
               나VH1             나H/               니H\   H/



          Command                Output            Input
                                 variable          source


The output file contains the same information obtained from a
simple dc analysis and
    1. the ratio OUTVAR/INSRC;
    2. the input resistance with respect to INSRC; and
    3. the output resistance with respect to OUTVAR.
18                                                                                                      CONTROL STATEMENTS FOR DC ANALYSIS


rilusson
Ni怜＄  O11
                Determining Thevenin equivalents:                                                          You may use the . TF control statement to find the Th6venin
Section 4.1O, pp. 124-126
                                                                                                        equivalent with respect to a designated pair of terminals. Exam-
                                                                                                        pIes 2 and 3 illustrate this application.



EXAM PL E                                                                 2

Use PSpice to find the Th6venin equivalent with respect to ter-                                                                                                                            20 k.1

minals a, b for the circuit shown in Fig. 9.
                                                                                                                               4 kU                      1.65 kll
                                                                                                                                                              八 八


                                                                                                                                                                    /b
                                                                                                                                                                                  1
                                                                                                                           119.59     21 k1l듣                       0.6 kfl
                                                                                                                             mV
S        0 L        U                      T                 I    0 N                                                                                                                                            1b


The circuit shown in Fig. 9 redrawn for PSpice analysis is shown                                                            FIGURE 9 The circuit for Example 2.
in Fig. 10. The zero-value voltage source Vaib is used to mea-
sure the controlling current i b. We labeled the components to fa-
cilitate reading the PSpice source file. Compare Fig. 10 with
                                                                                                                                                                                                    R5, 20 k1l
Fig. 9 and note that the Th6venin voltage Vab is node voltage
V(5, 0) or V(5). If we specify V(5, 0) as the output variable in                                                                    R1. 4k11
                                                                                                                                                              VA田

the . TF control statement, the output resistance from PSpice is
                                                                                                                                                                         +            R3
the Th6venin resistance.                                                                                                                                                     /b                        F]        尸，n
                                                                                                                                쌔們         21 k{i        R2                           0.6k11   R4                ri0
   The PSpice source file for the circuit in Fig. 10 is:                                                                                                                                                    0.75 kll


                                                                                                                                                     0


                                                                                                                            FIGURE 10 The circuit shown in Fig. 9 prepared




                                        aO 2 O 3 4 O 5 4 O
    Finding a Thevenin Equivalent                                                                with PSpic日
    Vi     1 O        DC      119. 59e-3                                                                                    for PSpice analysis.




                        l2 2 34 4 5 5
    RI     1 2        4e3
    R2     2 O        21e3
    Vaib   2 3        DC      O
    R3     3 4        1. 65e3
    R4     4 O        6OO
    R5     4 5        2Oe3
    Ft     三3 4       Vaib      3'크
    R6     5 O        75O
    .TF      V (5, O)      Vi
    1END




    The pertinent data from the PSpice output is:


         N（끄）E                    V口LTn日E                                         N口DE        VOLTA日E          NODE     V（긔.TA日E                    N口DE             ＼기긔mTn日E


    (            1 :)                                            . 1196       (          2)       .O日日2    (      :3)        1 C)日82           (:             4)                      m O日고2

    (:         5 :)                                          -. 1OOO
                                      3. 3 THE .TF CONTROL STATEMENT                                                                19


  共共퓻汗         C針1ALL- SIONPL            f: HARACTEPISTIC:             S




         ＼八．瓦 0) / VI == m日1359E-01

         INPUT RESISTANCE AT Vi =                                 1 .523E+04

         0UTPUT RESISTANCE AT V (5,0) =                                7. 446E+02
                                                                                                       744.6fl
Hence the Thevenin equivalent is as shown in Fig. 11.
  You may also calculate the Thvenin voltage from the transfer
function ratio V(5)/V 1:                                                             0.10V




                     V   (5）     과？       (Vi)
                                                                                     FIGURE 11 The Thevenin equivalent of the circuit
                                                                                     shown in Fig. 10.
                                 = (- 0.8359)(0.11959)
                                 = -0. 100.




EX A M P L E                      3

Use PSpice to find the Thevenin equivalent with respect to ter-
minals a, b for the circuit shown in Fig. 12.

                                                             2V         3／小
                  3n                             1.111   4              __     6fl




                                                                                     디GURE 12 The 이rcu仕 幻rExample 3.


$ 0 L      U   T I             0 N

From the circuit shown in Fig. 12 note that i中 is the current in an
independent voltage source. Therefore we do not have to use a
zero-value voltage source to measure the controlling current i中.
Also note that there is only one connection to node b. PSpice re-
quires at least two connections to every node, so we must mod-
ify the circuit accordingly. We may do so in one of two ways.
First, we may connect a resistor that is large compared to the
other resistors in the circuit-say, 106 fl for this circuit-to node
b and any other node in the circuit without affecting the behavior
of the circuit. Second, we may connect a capacitor between node
b and any other node. The capacitor behaves like an open circuit
during dc analysis and therefore does not influence the dc
Thevenin equivalent.
20                                                                             CONTROL STATEMENTS FOR DC ANALYSIS


   The circuit shown in Fig. 12 is redrawn in Fig. 13 in prepara-
tion for writing the PSpice source file. Note that we connected a
resistor of 106(1 between nodes 0 and 3. Also note that we chose
node b as the reference node. We did so because PSpice auto-
matically prints all the node -to-reference voltages, and therefore
the Th6venin voltage becomes part of the printout if node b is
the reference.
   With three independent sources, we may choose which one to
use in the . TF control statement. As we are interested only in
the Th6venin voltage and resistance with respect to terminals
a, b, the choice is immaterial. In other words, the transfer func-
tion ratio and the input resistance at the source are not relevant
to the Th6venin equivalent at a, b. In the PSpice source file that
follows we selected the 20-V source as the input source.


                                                                2V       3／小




                                                                                                  FIGURE 13 The circuit shown in Fig. 12 redrawn
                                                                                                  for PSpice analysis.


A PSpice source file for finding the Th6venin equivalent is:


     Finding the Thevenin Equivalent                                    when a Dependent Source is Present




                      2334353573
     Ri     1 2        3
     R2     1 3        7
     Vi     2 3        DC:     20
     R3     0 4        1. 1
     R4     0 3        1e6
     V2     4 5        DC      2
     R5     5 3        (:）口 7
     Fl     6 5        V2      3
     R6     6 7        6
     V3     7 3        DC:     40
     .TF     v (i, o:)        Vi
     1END



     The relevant output from the analysis is:


         N口DE         V（긔. TA日E                    N口DE         V口LTAGE            卜山DE        V（긔mTn日E           N口DE      VOLTA日E


     (          1:)            12 ,0000       (:          2:)        is. 0000     c       3)     -2. 0000    (:          4) 2. 200E-06

     (          5)                 -2. 0000   (           6)         38. 0000     (       7)     38. 0000
                         3. 4 THE .SENS CONTROL STATEMENT                                                     21


               SMALL-S I GNAL CHARACTER I ST I Cs
         V (1,0) /V1 =       7. 000E-01
         INPUT RESISTANCE AT Vi =            i. 000E+01               14V


         0UTPUT RESISTANCE AT V (1, O) =            6. 000E+00
Hence the Thevenin equivalent is a 14-V source in series with a       FIGURE 14 The Thevenin equivalent for
6-fl resistor, as shown in Fig. 14.                                   Example 3.




3.4 THE .SENS CONTROL STATEMENT

The pur田se of the . SENS (sensitivity) control statement is to
obtain the dc small-signal sensitivities of each specified output
variable with respect to every circuit parameter. Hence for cir-
cuits containing a large number of elements tremendous amounts
of output data can be generated, particularly when the sensitivity
of more than one output variable is of interest. Example 4 illus-
trates how to use the . SENS control statement to predict the be-
havior of an unloaded voltage-divider circuit.


EXAM PL E                4

Use PSpice to study the sensitivity of the output voltage vO in the
voltage-divider circuit shown in Fig. 15. We numbered the
nodes in anticipation of writing a PSpice source ifie.                125V




S 0 L U T I          0 N
                                                                      FIGURE 15 The circuit for Example 4.
Because we have three elements in the circuit, PSpice calculates
the sensitivity of vO with respect to the independent voltage
source, the 25-fl resistor, and the 100-fl resistor. The PSpice
source file is:

  Example c汁 Sen드itivity Analysi드
  Vi    1 C)      DC  125
  Ri    1 2       25
  R2    2 0       100
  .SENS    V (2, O)
  1END
 22                                                  CONTROL STATEMENTS FOR DC ANALYSIS


  PSpice prints out the data associated with simple dc analysis
and the sensitivity data. The data relevant to sensitivity are:

      DC SENSITIVITIES OF OUTPUT V (2, O)

                 ELEMENT               ELEMENT              ELEMENT         NORMALIZED
                  NAME                  VALUE            SENSITIVITY       SENSITIVITY
                                                         (VOLTS/UNIT)   (VOLTS/PERCENT)

                   Ri                 2. 昏：)OE+0 1        叫日1000E-0 1      -＝고1ooc:)E-0 1
                   F仁？                1. 000E+02           2. OC乂匹卜心1       2. C山OE-01
                   Vi                 1. 2iOE+02           8. 000E-Oi       1 . 000E+OO

  From the simple dc analysis of the circuit, vO = V(2) = 100 V
when Ri, R2, and Vi are at their nominal values. From the sen-
sitivity data we deduce that
      1. if Ri increases by 1 i, V(2) will decrease by 0.8 V- that
         is, V(2) = vO = 99.2 V;
      2. if Ri increases by 1%, vO will decrease by 0.2 V to 99.8 V;
      3. if R2 increases by 1 fi, V(2) will increase by 0.2 V- that
         is, V(2) = vO = 100.2 V;
      4. if R2 increases by 1%, vO will increase by 0.2 V to
         100.2 V;
      5. if Vi increases by 1 V, V(2) will increase by 0.8 V- that
         is, V(2) = vO = 100.8 V; and
      6. if Vi increases by 1%, vO will increase by 1 V to 101 V.
   Because we have a linear circuit, the principle of superposition
applies, and therefore we may superimpose simultaneous effects.
For example, let's assume that Ri increases by 1 fi, R2 de-
creases by 1%, and Vi increases by 0.5 V. The effect on vO, or
V(2), will be vO = 100 - 0.8 - 0.2 + 0.4 = 99.4 V.
                                                                                       23



CHAPTER 4


0UTPUT STATEMENTS FOR
DC ANALYSIS
in Example 1 you could not specify which voltages and currents
you want to examine in the output file. The . PRINT command
gives you control over what appears in the output file.
   The print statement has three fields. The first contains the
command . PRINT. The second contains the type of analysis
performed to generate the output-in this case, DC. The third
contains a list of output variables to be printed. There is no limit
to the number of output variables you can specify and no limit to
the number of print statements in the source file.
                                                                                  十
       '-
            .PRINT
               -------
                          DC
                         -.尸
                                    OV1 <OV2 OV3. . .>
     Command Type of                             Output
             analysis                           variables
   In order to use the print statement, you must understand the
format for specifying voltage and current variables. Thus
V(N1, N2) specifies the voltage difference between nodes Ni
and N2. As before, the order of the nodes specifies the reference
polarity. Omitting N2 causes the second node to default to zero
or to the reference node.
   Similarly, I (Vxxx) specifies the current in an independent
voltage source named Vxxx. As before, positive current is
through the source, from the positive node to the negative node.
   Example 5 illustrates the use of the print statement in a source
file containing a . DC control statement. Note that you must state
explicitly the output variables to be printed by including a print
statement (the . PRINT command) in the source file.


tTriangle brackets are used in examples of PSpice statements to identify op-
tional fields. Ellipses are used in examples of PSpice statements to indicate addi-
tional identical fields. Neither triangle brackets nor ellipses should appear in ac-
tual PSpice statements.
24                                                            0UTPUT STATEMENTS FOR DC ANALYSIS


EXAM PL E                         5                                                                      諦U            日H니nm   /(7




For the circuit shown in Fig. 16 use PSpice to find the values of                               5U                       8U

iO and 'vO when vg varies from 0 to 100 V in 10-V steps.                                    +   V.



                                                                                                                                     5A@




                                                                             디GURE 16 The circu仕 幻r Examp旭 5.


                                                                                                32U          d         /／小＼.....
S     0 L      U I       I    0 N                                                                                      1+  냅 츠쁘止1U1
                                                                                                54                     \\/

The circuit shown in Fig. 16 is redrawn in Fig. 17 with the                                     5U                       8U

nodes numbered and the elements named to facilitate reading the                                 Hi                       53

PSpice source file. Note the insertion of a zero-valued indepen-                                        52       40U                  (入
                                                                                                                                     5A
                                                                                                                                     S미＜/
dent voltage source in series with the 3241 resistor to measure             IIIvso
the current iO. A PSpice source file that models this circuit is:

                                                                                     디GURE 17 The circu仕 shown in 디gure 16
                                                                                     prepared for PSpice analysis.

               332O34
     Circuit                            U
                                        H
              Used to Illu드trat臼 the .DC Control                      Statement
     ＼峙（:1           DC                 5
            U
            느
     I 弓1二1          DC                  U=

             l   4i2 l
     Vamp            DC
     尸1              5
     R2             二
                    n40
              =n
     R3              8
     P'4             32
     .DC    \／드c.    (:)     ic：川：) 1(:}
     =PRINT      DC:     I (Vamp)    V (1, 2)
     1巨ND



The relevant output from the program is:


     V弓口                     I (Vamp)         V ( 1, 2)

      O. OOOE+OO             -1 1 4OOE+OO     -1. 6OOE+C)1
      1. OOOE+O1             -1. 375E+OO      小1 . 5OOE+O 1
      2. OOOE+O1             -1. 35OE+OO      -1. 4OC)E+O1
      3. OOOE+O1             -1. 325E+OO      -1. 3OOE+O1
      4. OC山E+O 1            -1. 3OOE+OO      -1. 2OOE+O1
      5. OOOE+O1             -1. 275E+OC)     -1. 1OOE+O1
      6 口 OOOE+O1            -1. 25OE+OC)     -1. C心OE+O1
      7. OOOE+O1             -1. 225E+OO      -9.. OOOE+OO
      8. OOOE+O1             叫1 = 코：山E+OO     -8. OOOE+OO
      ’乳 OOOE+O1             -1. 175E+OO      -7. OOOE+OO
      1. OOOE+O2             -1. 1昏：)E+OC)    -6. OOOE+OO
                                               OUTPUT STATEMENTS FOR DC ANALYSIS                      25


  Now we alter the source file of Example 5 to sweep through
values of the current and voltage sources. Example 6 presents
the results.


EXA M P L E                                          6

The current source in the circuit shown in Fig. 16 varies from 0
to 5 A in 1-A steps. For each value of the current tabulate vO and
tg as Vg varies from 0 to 100 V in steps of 20 V.


S        0   L       U         T         I    0     N

In order to print out Iso, we insert a zero-value voltage source in
series with Iso. Refer to Fig. 17 and visualize this source placed
between nodes 0 and 5, where node 5 is a new node inserted be-
tween Viso and Iso. The PSpice source file is:
    C     U
          C          t   l
                         1닙              h
          r                                  both Voltage        and Current         S口urces Varied
                                    +
                 1
     1
                     l50l22l   0352033
                                    U
                 l
     l
    Vso                                       DC        0
    I弓O                                       DC        0
    Vi드O                                      DC        0
    Ri                                        5
    R2                                        40
    R3                                        8
    R4                                        32
    1DC    Vso                                0       100        20      Iso          0    5    1
    .PRINT    DC                                 \/( 1, 2)       I (Vi드1그）
    .END


The output from the analysis is:

     Vs.:'                                   V (: 1, 2 :)       I (Vi 드口:)

         C) .. 000E+00                         0. 000E+00        0. 000E+00
         2. 000E1-0 1                          2. 000E+00       -1 . 日40E-11
         4. 000E+ 01                           4. 000E+00       -3. 680E叫11
         6. 0(:)0E+01                          6. 000E+00       -5. 日20E6- 1 1
         8. 000E-'-Ol                         日1000E+00         -7.. 360E-11
         1 . 000E+0고                           1 . 000E+01      H'크 . 고00E呻11
         0.. C>OOE+00                        -3. 200E+00         1.汭>OE+00
         2. 0 0E+01                           -1 . 200E+00       1 . 000E+O0
         4. 000E+0 1                           8. 000E呻01        1 . 000E+00
         6. C)OOE+(:>1                         2. BOOE+(:)(D     1 . 000E+00
         日. 0C山E+0 1                           4. 800E+00        1 , (：乂)OE +C乂）
         1 . 000E+02                           6. 800E+00        1 . 000E+C)C)
         n .C)0c)E+C>C                       -6. 400E+OC)        2. 000E+O0
         2. 000E+0 1                         -4. 400E+00         2. 000E 00
         4. 000E+01                          尸고 . 400E+00        2. oooE+oo
         6. ( "DOE+0 1                       H止1. . 000E叫C) 1    고 . C乂）OE+00
         8. c)C心E+01                           1 . 600E+00       고 = 0CMDE 4. 0(_)
26                                                     0UTPUT STATEM ENTS FOR DC ANALYSIS



     1 . 000E+02        3. 600E+O0       2. 000E+Oc)
     0. 000E+OO       -9口 600E+Q0       3. 000E+00
     2. 000E+01       -7. 600E+O0       3. 000E+O0
     4. 000E+01      -5. 600E+O0        3. 000E+00
     6. 0汭）E+0 1     -3. 600E+아：}       3. 000E+00
     8. OC)OE+01     -1 . 600E+O0       3. 000E-'O0
     1 . 000E-'-02     4. OC)c:)E-0 1   3. 000E+Oc)
     0. 000E+C心      -1 . 280E+01       4.. OOC)E+00
     2. 000E+01      山m1. 080E+01       4. OOc)E+OC,
     4. 000E+01      -8. 800E+O0        4. 000E+00
     6. 000E+0 1     -6. 800E+C)C)      4. 000E+O0
     0. 000E+01      -4. 800E+00        4. 000E+Q0
     1. 000E+02      -2. 8OOE+OO        4. 000E+O0
     0. 000E+OO      -1. LOOE+ 01       5. C)OOE+00
     2. 批）0E+01      -1. 400E+01        5. c:)OOE+00
     4. 000E+C)1     -1 . 200E+C 1      s. 0C)OE+oc)
     6. 000E+01      -1 . 000E+0 1      5. OOOE+OO
     8. 000E+C)1     -8. 000E+00        5口 000E+00
     1 . (：心0E+C口    -6. m:H:)E+(：心     5. (：川）OE+00




              J口B 口口NC:LUDED

              T口TAL J口B TI卜IL                      ;？口 1亡4




                                                      Recall from Section 1.2 that in simple dc analysis the only out-
                                                   put voltages printed are the node-to-reference voltages. You may
                                                    use the . DC control statement and a print statement to obtain the
                                                    voltage between any two nodes. You do so by sweeping only one
                                                    source and then setting the sweep range to zero by making
                                                   STARF1 = STOP1 and setting NCR to any positive value.
                                                      To illustrate we return to the circuit shown in Fig. 6. We al-
                                                   ready have a simple dc analysis of this circuit-see Example 1 in
                                                   Section 2.3, with its accompanying printout. Recall that we ob-
                                                   tamned this printout without a . PRINT statement and that in this
                                                   mode we have no control over what is printed. Let's assume that
                                                   in the circuit shown in Fig. 6 the voltages V(3, 4), V(2, 4) and
                                                   V(1, 4) are of interest. To obtain these voltages we modify that
                                                   original PSpice source file in the following ways.
                                                       1. Change the independent voltage source entry to read
                                                                            Vi  2 1        DC        0
                                                       2. Add . DC control statement reading
                                                                        .DC        Vi   20      20       1
                                                             to the source file.
                             OUTPUT STATEMENTS FOR DC ANALYSIS          27


  3. Add . PRINT statement requesting the desired voltages to
     the source file.

       The modified source file is now:

  타；am口le 口f Sin耳Die D亡： Anal y드1弓 Hm Revised
  Fl         0 1    Vaipha      0. 1

                                 6
  Valpha     0 5    DC          0
  Vi         2 1    DC          0

                               2  18 0


            l 4233
  RI     1 4
         4 0

                             l22362
  R2



                          5 lU
                             1
  R3     2 3
                45l
  罷
  .DC    Vi    20
                  V
                      20                    1
                      m
  .PRINT    DC    V (3, 4)                   V (: 2, 4)   V (: 1, 4)
  1END


The output voltages from the analysis are:

  Vi                      V (3, 4)         V (2, 4)       V ( 1, 4:1

    2. 00C)E+01             4. 47C)E+C)0    7. 050E+00    -1. 295E+01


  You should verify that these results are consistent with those
given by the original source file. Note also that use of the . DC
control statement results in printing only the requested node
voltages, along with the voltage of the independent voltage
source-VI in this case.
                                                                      29



CHAPTER 5


0PERATIONAL AMPLIFIERS

rspice offers t뇨ee options for describing an operational am-
plifier (op amp) within a source file. The first is to model the op
amp with resistors and dependent sources. The second is similar
to the first, but now the model is a PSpice subcircuit and is as-
signed a unique name. The op amp subcircuit may be used like
any other PSpice circuit element, such as a resistor, and included
in multiple locations within the circuit being described. The
third is to take advantage of op amp models already supplied
with PSpice. These models are available in a device library and
may be accessed with the . LIB command. The library models
are considerably more sophisticated than the simple dependent-
source-based models and are designed to mimic the characteris-
tics of actual op amps.
   In general, if you have only one op amp in your circuit, mod-
eling it with resistors and a dependent source is best. If the cir-
cuit contains two or more op amps, you should create an op amp
subcircuit that you can use to represent each op amp in the cir-
cuit. You should use the library op amp models only when accu-
rate modeling of certain op amp characteristics is important to
the circuit analysis. Because the library models are complex, cir-
cuits containing them tend to occupy more space, and analysis of
such circuits takes longer.




5.1 MODELING OP AMPS WITH RESISTORS AND
    DEPENDENT SOURCES

In Section 6.7 of the textbook the author introduced an equiva-
lent circuit for the operational amplifier. That equivalent circuit
30                                                                                0PERATI0NAL AMPLIFIERS


                                                                                  is re士awn in Fig. 18, where we also numbered the nodes to 缸
                                                                                  cilitate discussion of the PSpice model.
                                                                                     The PSpice description of the equivalent circuit shown in Fig.
                                                                                  18 is:
                                                                                               RI          12             VALUEOFRI
                                                                                               묘兀兀工        3521           VALUEOFA
                                                                                               RO          3 4            VALUE OF RO
FIGURE 18 An equivalent circuit for an operational                                  Example 7 illustrates how to use PSpice to analyze a circuit
amplifier.                                                                        containing an operational amplifier.



EXA M P L E                                   7

                                                                                                                                  lOk)1
The parameters for the operational amplifier in the circuit shown
in Fig. 19 are R = 200 k(1, A = 10k, and RO = 5 kfl.
a) Use PSpice to find v1 and vO when Vg = 1 V(dc).
b) Compare the PSpice solution with the analytic solution for v,
   and vO.


 S 0 L U T I                             0 N                                                            디GURE 19 The circu仕 化r Examp旭 6.
a) We redrew the circuit shown in Fig. 19 in Fig. 20 in prepara-
   tion for writing the PSpice source file to find v1 and vO:

     타；am口le 6 -m Th日 O口 슥m口

                                 2 U4   4
                  D
                       DC:                                           j.
                       1C)C)()

                  N            U
                               H
                                      3 3U
                                          n
                       2OC）日：3

                               l l   2n
                                      n   4
                       iC)日：3

      g 5 lf l 口l E
                       2 O                                                -1Oe3
                                  1口
                       5日3                                                                              FIGURE 20 The circuit shown in Fig. 19 redrawn
      U只R RERR =
                       4可3
                                                                                                        for PSpice analysis.


     The pertinent output from the PSpice program is
                                          V (2) = 0.0027 V = v1;
                                          V (4) = -9.969 V = i石．
b) We obtain the analytic solution for vi and vO by solving the
   following simultaneous node-voltage equations:
     Vi-       1+     __   _      +Vi_
                                              1。
                                                  vo
                                                           0;   vo
                                                                      。vi + vO
                                                                          -      104 v' +    뜨4     0
         1            2。
                       。                                   0;        1         +5
                                                       -
                                                       _
                           5. 2 MODELING OP AMPS WITH SUBCIRCUITS        31


   We leave to you verification that the solutions for vi and v。are
                    v, = 2.742 mY       and    v。= -9.970 V.




   If we assume that the operational amplifier in the circuit
shown in Fig. 19 is ideal, we can alter the PSpice op amp de-
scription by making R and A very large and R。= 0. To illus-
trate we rewrite the source file in Example 7, with R = 200
Mf1, A = 108 and R。= 0. By making R。= 0, we eliminate
node 3 from the circuit. The PSpice source file becomes:



   X 口 5i f l l
             m    l
                  P e
             a
                        7 revisited    -- The Ideal   Op Amp
                          10        DC     1
                          1 2       1C川：心



   EUR RR ER
                          2 0       200e6
                          2 4       10e3
                          4 0       2 C)     -jOe日
                          4 0       4e3
   1END


The values of v, and v。from this simulation are
                             v1 = V(2) = 0.0000 V;
                             v。= V(4) = -10.0000 V.
  These results are consistent with the analysis of the circuit
shown in Fig. 19, if we assume that the operational amplifier is
ideal-that is, vi = 0 V and v。= -10 V.




5.2 MODELING OP AMPS WITH SUBCIRCUITS

In PSpice, a description of the topological connections of a cir-
cuit may include subcircuits. In other words, you may take a
portion of an overall circuit, describe it separately, and then in-
sert this description into the source file that describes the over-
all, or global, circuit. You define the subcircuit by naming the
group of element statements that describe it. There is no limit on
subcircuit size, and a subcircuit may contain other subcircuits.
    You define a subcircuit in a PSpice source file by first inserting
 a . SUBCKT control statement, which has the general form:
                  . SUBCKT       SUBNAM       Ni N2 N3 . . .
where SUBNAM is the subcircuit name and Ni N2 N3 . . .
32                                               0PERATIONAL AMPLIFIERS


                                                 are the external nodes of the subcircuit. The external nodes con-
                                                 nect the subcircuit to the 如bal circuit. The only restriction on
                                                 selecting the external node numbers is that you cannot use zero.
                                                 Any node numbers used in the description of a subcircuit that do
                                                 not appear in the . SUBCKT control statement are strictly local,
                                                 with the exception of 0, which is always global. You terminate
                                                 the subcircuit description by inserting an . ENDS control state-
                                                 ment. The general form of the . ENDS control statement is:
                                                                   . ENDS              <SUBNAM>
                                                 where SUBNAM is optional. If included, it indicates which sub-
                                                 circuit is being terminated. If it is omitted, all subcircuits being
                                                 described are terminated.
                                                    The data statement to include a subcircuit has the general
                                                 如rm:
                                                                 xyyyNl N2 N3 . . . SUBNAM
                                                 where x yyy indicates a subcircuit is being used, Ni N2
                                                 N3 . . . are the circuit nodes to which the subcircuit external
                                                 nodes are connected, and SUBNAM is the name of the subcir-
                                                 cuit being used.
                                                   To illustrate how to use a subcircuit in a PSpice source file, we
                                                 return to the op amp circuit discussed in Example 7, but here we
                                 5k0             use a subcircuit to describe the equivalent circuit. Figure 21
                                                 shows the subcircuit and the node number assignments.
                                                   The PSpice definition of the subcircuit is:

                                                   . SUBCKT              OPAMP     1    2   4   5

                                                                  l54
                                                   Ri       2                200e3
FIGURE 21 An operational amplifier subcircuit.     El       3                2   1      10e3
                                                   Ro       3                5e3
                                                   .ENDS                 0PAMP

                                                   When we use this subcircuit in the description of the circuit
                                                 shown in Fig. 20, the PSpice source file becomes:

                                                   q 弓f i
                                                                  0240
                                                             1   0     DC      1

                                                   V RRR
                                                             1   2     1000
                                                             2   4     10e3
                                                             4   0     4e3
                                                   .SUBCKT         OPAMP     1 2 4              5

                                                                  i54
                                                   Ri      2     1     200e3
                                                   El      3     5     2 1       10e3
                                                   Ro      3     4     5e3
                                                   .ENDS           OPAMP
                                                   Xl      2     0 4 0       0PF뇌너P
                                                   .ENU

                                                   Note the correspondence between the node numbers in the
                                                 .SUBCKT control statement and the Xl element statement. That
                         5. 2 MODELING OP AMPS WITH SUBCIRCUITS                                            33


is, node 1 of the subcircuit connects to node 2 of the main cir-
cuit, node 2 of the subcircuit connects to node 0 of the main cir-
cuit, and so on.
   A more realistic use of subcircuits occurs when we repeat a
subcircuit in the overall, or global, circuit. For example, con-
sider the circuit shown in Fig. 22, where we assume that the two
operational amplifiers are identical. We construct the PSpice
source file to find vOl and v。 2 when Vg = 0.5 V(dc) and the op
amp parameters are R, = 100 k(l, RO = 200c1, and A = 10g.
   In the following PSpice source file note the repeated use of the
OP川町P subcircuit and the use of the . DC control statement so
that only the node voltages of interest are printed out. For con-
venience we used the same node designations in the OPAMP sub-
circuit as in Fig. 21.


  PSpice Source File with a Repeated Subcircuit



                 02340   60
  Vq     1 0             DC           0
  Rs1    1    2          4e3
  Rf1    2 3             80e3
  Ri     3    4          3日：크



                      U1
  R2     4    0          20e3
  R드2    5    0          6e3
  Rf2    5    6          18e3
  Ri     6    0          1003
  1SUFCKT       OPAMP              1    2   4   5


           233        l54
  Ri     2    1          100e3
  El     3    5    2   1      1e4
  R0     3    4          200
  . ENDS        口PA川P
  xl     고    0    3 (:) （가카낚朴＞
  X2     5    4   6 (:) 마갸功IP
  .DC      Vg       0. 5           0. 5       1
  .PRINT       DC:       V ('.3 :)       V (6)
  1END



  The outputs from the PSpice analysis are:
                              vO1 = V(3) = -9.9780 V;
                              V。
                               2 = V(6) = -31.9154 V.


                                                        18 kf)




                                                                      FIGURE 22 A two-stage amp circuit.
34                                                                                                                                       0PERATIONAL AMPLI FIERS


                                                                                                                                       We test whether these results are reasonable by assuming that
                                                                                                                                     the op amps are ideal and then calculating the resulting values of
                                                                                                                                     vO1 and V。 2. We leave to you confirmation that these calculations
                                                                                                                                     yield v이 = -10 V and v。     2 = -32 V. We conclude from these
                                                                                                                                     results that we have made no errors in describing the circuit and
                                                                                                                                     hence are confident that the PSpice solution is correct.




                                                                                                                                     5.3 USING OP AMP LIBRARY MODELS

                                                                                                                                         One of the most powerful features of PSpice is the library of
                                                                                                                                         models for various electronic devices. The full version of PSpice
                                                                                                                                         has models for more than 5000 devices! The student version of
                                                                                                                                         PSpice has models for about 30 of the most commonly used
                                                                                                                                         devices. Among these models are two for op amps: the LM324
Nilsson          Desc먀川on of the 尸A741 op amp:                                                                                           and the 尸A741. Figure 23 presents a listing of the subcircuit
Section 6.1, pp. 190-191                                                                                                                 model for the MA741. As you can see, this model is very corn-
                                                                                                                                         plex, and some of its components are well beyond the scope of
                                                                                                                                         this manual or the textbook. Note that the initial comments de-
                                                                                                                                         scribe the external nodes for the subcircuit.
                                                                                                                                           In order to incorporate the 尸A741 subcircuit into your circuit
                                                                                                                                         you must tell PSpice which library contains the model you want
                                                                                                                                         to use. As illustrated in Example 8, you use the . LIB command
                                                                                                                                         in this case, with the format
                                                                                                                                                                              .LIB   fname.lib
                                                                                                                                         where fname is the name of the library file.

斗叫   mH        mH   Hm   mm   Hm   m   m=   nm   ·m   mH   Hm   mU   mH   呻   呻   叫   呻   叫   ·m   叫   m   叫   m   m   m   4m   mH   尸   呻   m   H   m   m·   ·   mn   ，··n




共 connect ion弓＝        n口n小invert inq input
*                      1 invert inq input
共                          1 口L喀it iv日 p c'w er 드Lippi y
·片                           1 n日gat iv臼 口C·니日r eupply
*                            1 1 output
共                            1
                             1
                                !
                                1
                                     1
                                     1

1 드나bc kt 나A741              3 4 5
斗

      l고 Ce
         11 1고 I크 , 6EA 巨--1고
          6  7 30. C乂）E- 1고

      C Cd d
          5 53 dx
         54  5 dx
   dip   90 91 dx
   din   92 90 dx
   d口     4  3 dx
   日gnd '크'크 (:) 口O ly （二？:) (3, (:):) (4, (:):) (:) . 드-I . !5

FIGURE 23 The p.A741 Op Amp Subcircuit Model
from the PSpice library file.
                                                        5. 3 USING OP AMPS LI BRARY MODELS                                   35




            9   640고l   l       95
                                             p口1y (5) vb vc vE크 vip              yin   0 10. 61E6 --410E6 10E6 10E6 -1C)E6
                                             11 12 188..5E-6
                                             10 99 5. 961E....9
                                             d.: 15. 16E--6




            9        늬m l二lll9 늬
                          二       m
                                             vliffl 1K
   m毗



                            U
                            1 U
                              H
                                             13 qx
            114
                                             14 qx




             nn
                                  늬
                                  山
   r2                                        100. 0E3
   rc 1                                      5. 305E3
   rc2                                       5. 305E3
   rel      13                               1 . 836E3




            7600    고633         873    47
   r e2     14                               1 . 836E3
   r ee     10                               13. 19E6
   r 口I                                      50




                                      m 5
   r口2                                       100




                 l                  늬m口
   rp
                               言             18. 16E3

                                             C 亡 C=
                                                  n亡   0ll
   vb
   v:            53

                                             dddd
   ye             4
   vi im          8
   vip      ’크 l  0 dc 40
   vi n       C) 日2 d亡 中：)
. model     dx D (Is==800. 0E- 18 F드＝=1)
. m口del     qx NPN ('. Is= 800. OE- 18 Bf= 크3. 75)
=ends



EXA M P L E                                                  8

Repeat the analysis of the circuit shown in Fig. 22, but this time
use the 幷A741 model from the PSpice model library.


S 0     L         U I                        I    0          N

The model's source file listing shows that the 尸A74l subcircuit
model requires explicit connections to the positive and negative
voltage supplies. These supplies are called VCC1 and VEE1 for
the left-hand op amp, and VCC2 and VEE2 for the right-hand op
amp.
                  L
                            P                7弓
  Using                                                          Am口 서odel 드
                       1
                       l
                            0
  VG                                                               DC:    0
  PSi                                                              4E3

                                234006       2508
  PF1                                                              日0E3

                            y
  Ri                                                               5E3


                              i i 2 3 4 5 5U
                                           n
  P2                                                               20E3

                            r=n            6047
  RS2                                                              6E3
  RF2                                                              1日E3
                            a
                                                U
                                                1
  RL                                                               10E3
                                                                 8l
                            r
  xl                                                               3    L(A741
  x고                                                                  6C亡
                                                                        나A74 1
                            b                                          DD
  vc01                                                                    1C)
  VEE 1                                                                   10
36                                                0PERATIONAL AMPLIFIERS


     VCC:2      9 C>        DC:        4(>
     VEE2       0 lu        DI::       40
     .LID   EVfL. LIB
     .DC:   V日     u. 5       () .5       1
     .PRINT    Di:      v (3)         V (6)
     .END


     The output from this source file is
                      v。
                       i = V(3) = -9.577 v;
                      V。
                       2 = V(6) = -30.64 V;
Note that these answers are slightly different from those obtained
when the simplified subcircuit model was used in Section 5.2.
                                                                                                                        37



CHAPTER 6


INDUCTORS AND CAPACITORS

Liata statements for inductors and capacitors are similar to those
used for resistors. As a minimum, three fields are required. The
first consists of a unique element name. If the element is an in-
ductor, the name must begin with the character "L" (either up-
percase or lowercase); if the element is a capacitor, the name
must begin with the character "C" (either uppercase or lower-
case). As with the description of a resistor, the second field con-
tain只 the node numbers that describe the branch in which the in-
ductor or capacitor is located. The third field contains the value         Nilsson   Inductors: Section 7.1, pp. 228-234
of the inductance (in henries) or the capacitance (in farads).
    A 10-mH inductor nimed LPGA8 connected between nodes 3
and 9 is specified as:
                       LPGA8           3 9        lOe-3
                   나＼    尸／       1尸              나，   小-      d




                       Name       Node     Value
                               connections
  The format for a 0.58-pF capacitor denoted Cl and connected
between nodes 5 and 0 is specified as:


                  Cl             5 0              0. 58e-6                 Nllsson    Capacitors: Section 7.2,
                나VH/            나戶m/
                                             늬1         戶HH/
                                                                      pp. 235-239
                Name             Node              Value
                              connections
You do not have to give the reference node 0 explicitly. That is,
if you give only one node number, the second node defaults to 0.
   For cases where inductors carry initial current, the current
                                                                                     8.75 mH
reference direction is from the first-named node to the second-       as111\            YY\1H1+          4
                                                                                      1니卜 5A
named node. For instance, consider the inductor shown in Fig.
24, which is carrying an initial current of 5 A oriented from         FIGURE 24 An inductor carrying initial current.
38                                                   INDUCTORS AND CAPACITORS


                                                     node 8 to node 4. Let's assume that the inductor is named L5.
                                                     The element data statement in the source file then is:
                                                                 L5         8 4           8. 75e-3                  IC = 5
                                                                            나＼   戶＝ /
                                                               니尸／                       니＝         eV=   m1/      나小H/


                                                                Name         Node                     V.카ue         Initial
                                                                          connections                              condition
                                                       Reversing the order of the nodes in the description of L5 re-
                                                     quires that the initial current be given as a negative value. In
                                                     other words, we may also describe the inductor in Fig. 24 as:
                                                                     L5      4 8        8. 75e-3                IC = -5.
                                                       For cases where capacitors carry initial voltage, the p아arity
                                                     of that voltage is positive at the first-named node. For instance,
                                                     consider the capacitor shown in Fig. 25, which is carrying an
5 .
                ](
               0.25 nF
                                1   l2
                                                     initial voltage of 12.8 V, positive at node 12. Assume that the
                                                     capacitor is named Cap36. The element data statement in the
FIGURE 25 A capacitor carrying an initial voltage.   source file then is:
                                                          Cap36            12 5               0. 25e-9              IC = 12. 8
                                                          나＼   HH/
                                                                            뇨HY尸／
                                                                                              나1/                   뇨＋      口＼尸-     /




                                                           Name          Node                       Value                 Initial
                                                                      connections                                        condition
                                                       As in the preceding case, reversing the order of the nodes re-
                                                     quires entering the initial condition as a negative value. Hence
                                                     we may also describe the capacitor in Fig. 25 as
                                                               Cap36        5 12        0. 25e-9                IC = -12. 8.
CHAPTER 7


TIME-DEPENDENT CIRCUIT
RESPONSE
We now describe some of the features of PSpice that you can
use when examining the behavior of a circuit as a function of
time. In PSpice, this behavior is called the transient response of
the circuit.




7.1 EXPONENTIAL PULSE SOURCES

In order to facilitate transient analysis, PSpice provides indepen-
dent voltage and current sources that are time dependent. In this
section we describe the exponential pulse. Although we base this
description on an independent voltage source, we may also use
this format to describe an independent current source.
   The exponential voltage pulse is described by the following
equations:
t늉 = vi,                                        0 뜨 t 드 T[兀
v8 = Vi + (V2 - V1)(1 - e_ _mnIT1),          TD1 드； t 드 TD2;
Vg = Vi + (V2 - V1)(1 - eU(t_Th1)/'1)
     + (Vi - V2)(1 - e t I')2)/T2)           TD2 5 t 드 TSTOP;
where
    Vi = initial value in volts;
    V2 = pulsed value in volts;
  TD1 = rise delay time in seconds;
     丁l = rise-time constant in seconds;
  TD2 = fall delay time in seconds; and
     T2 = fall-time constant in seconds.
40                                              TIME- DEPENDENT CIRCUIT RESPONSE


                                                The default values are as follows: TD1 = 0, TI =
                                                TSTEP,TD2 = TD1 + TSTEP, and T2 = TSTEP. Figure 26
                                                shows a graph of the exponential voltage pulse.
 V2                                               The syntax for an exponential voltage source, called Vexpso,
                       //
                                                positive at node Ni and connected to nodes Ni and N2, is
                                                    Vexpso Ni N2 EXP(Vi V2 TD1 TI                  TD2 T2).
 vi
                      J
     0     TD1       TD2    TSTOP          z.



FIGURE 26 The exponential voltage pulse.        7.2 TRANSIENT ANALYSIS

                                                You use transient analysis to examine the response of a circuit as
                                                a function of time. The control statement for transient analysis
                                                has six fields, the last three of which are optional. The format
                                                for the transient analysis statement is:
                                                . TRM4    TSTEP     TSTOP      < TSTART        < TMAX >>
                                                +    <UIc>
                                                The terms inside the angle brackets <> are optional, as we dis-
                                                cuss shortly. TSTEP is the printing or plotting increment.
                                                TSTOP is the final time. TSTART is the starting time; if omit-
                                                ted, it is assumed to be zero. TMAX is the maximum step size
                                                that PSpice uses for computational purposes. If TMAX is omit-
                                                ted, the value used defaults to either TSTEP or (TSTOP -
                                                TSTARF)/50, whichever is smaller. TMAX is useful when you
                                                want to guarantee a computing interval smaller than the printing
                                                or plotting interval (i.e., TSTEP).
                                                  Transient analysis always begins at time zero. If TSTART is
                                                not zero, PSpice analyzes the circuit between zero and TSTART
                                                but does not write data to the output file. In the interval between
                                                TSTART and TSTOP, PSpice analyzes the circuit and writes the
                                                data to the output file.
                                                  The abbreviation UiC stands for Use Initial Conditions. It is
                                                an optional keyword that tells PSpice not to determine a quies-
                                                cent operating point before beginning the transient analysis. If
                                                the keyword mc appears, PSpice uses the values specified in
                                                the element statements, that is, the IC = values. This option is
                                                of particular interest here, because our circuits do not contain
                                                nonlinear devices for which the quiescent operating point must
                                                be found.
                                       7. 3 TIME- RESPONSE OUTPUT                41


7.3 TIME-RESPONSE OUTPUT

You may use any of three different ways to examine the output of
a transient analysis. First, you may use the print statement to ob-
tamn a list of any desired voltage and current values for each time
step specified in the transient analysis statement. Second, you
may use the plot statement to generate a line printer plot of
voltages and currents versus time. Finally, you may use the
PROBE graphics postprocessor to generate high-quality graphs of
 voltage and current.


PRINTING
The format for the print statement is similar to that used for
printing the results of dc analysis:
        .PRI寸r        TRA寸        OV1 <0V2           0V3 . . .>

Again, there are three fields. The first is the . PRINT command.
The second specifies the type of analysis that was performed to
yield the output variables-in this case, 旺A寸 for transient anal-
ysis. The third consists of a list of output variables, which can ei-
ther be voltages at nodes or currents through voltage sources.
(See Chapter 4 to review the format used for voltages and cur-
rents.)


LINE PRINTER PLOTTING
You may use the plot statement to generate line printer plots on
any printer. The format is:
 - PLOT       THAN        OV1 <(PL01, PHIl)> <OV2
 +     <(PL02, PHI2)> . . . >
     The following notes describe the details of the plot statement.t
 1. The - PLOT command statement defines the contents of one
 plot with one to eight variables-that is, OV1, 0V2, . . . ,
 0V8.
 2. The syntax for the output variables is identical with that of
 the - PRINT command.
 3. The low and high plot limits, i.e., PLO and PHI, are optional
 and may be specified after any of the output variables. All ou印ut


 tA. Viadimirescu, K. Zhang, A. R. Newton, D. 0. Pederson, and A. Sangio-
 vanni-Vincentelli, SPICE Version 2G User's Guide, University of California at
 Berkeley, unpublished.
42   TIME- DEPENDENT CIRCUIT RESPONSE


     variables to the left of a pair of plot limits (PLO, PHI) will be
     plotted using the same lower and upper plot bounds.
     4. II plot limits are not specified, PSpice will automatically de-
     termine minimum and maximum values of all output variables
     being plotted and scale the plot to fit. More than one scale will
     be used if the output variable values differ by orders of magni-
     tude. This means that mixing such output variables on the same
     plot still yields a readable plot.
     5. The overlap of two or more traces on any plot is indicated by
     the letter X.
     6. When more than one output variable appears on the same
     plot, the first variable specified will be printed as well as plotted.
     If a printout of all variables is desired, a companion . PRINT
     command is required.
     7. There is no limit on the number of . PLOT commands
     specified for each type of analysis.

     PROBE PLOTS
     PROBE is a software package that allows you to examine the re-
     sults of PSpice circuit simulation using hi합-resolution 얗aphics,
     both at the terminal and as hard copy. PROBE is simple to use,
     and it can be a very powerful tool in visualizing circuit analysis
     results. Before running PROBE you must be certain that a file
     named PSPICE.DEV exists on your PSpice directory. This file
     describes the devices available on your system. You must input
     the type of graphics display and printer you have in order for
     PROBE to generate the appropriate graphics. You may easily cre-
     ate or modify the PSPICE.DEV file from the PSpice Control
     Shell. (See Appendix A for more information.) If you are using
     PSpice and PROBE at the operating system level, you can create
     or modify the PSPICE.DEV file in any editor.
        The PROBE software reads a data file that contains the results
     from PSpice analysis in a form especially suited to PROBE. You
     create this data file by using the command . PROBE in your
     PSpice source file. After completing a PSpice analysis, you may
     look at your results using PROBE, which you access from the
     Control Shell (details are presented in Appendix A) or directly
     from the operating system level by typing PROBE. PROBE
     searches for this special data file (usually called PROBE.DAT)
     and, upon finding it, displays a blank coordinate system on the
     screen with a set of menu selections at the bottom.
        Select the Add trace menu item to display any of the voltages
     or currents in your circuit. The F4 function key gives you a list
                                       7. 4 NATU RAL RESPONSE                                                           43


of available voltages and currents, in case you've forgotten the
node numbers and device names used. You may select one or
more for your display. The remaining menu items permit you to
erase traces, reconfigure the x and y axes, add or delete other
plots to the display, get a hard copy of the display, zoom in on
your plot, move a cursor over your plot to get numerical values
at any point, and label your plot. We illustrate many of these fea-
tures throughout the rest of this manual. You should take some
time to play with PROBE, as that is perhaps the best way to learn
about all of its capabilities.




7.4 NATURAL RESPONSE

To find the natural response of a circuit you first find the initial
inductor currents and capacitor voltages. When you know these
values you can describe the circuit for transient analysis. In con-
structing the source file for a transient solution you must decide
on the form of the output data, that is, whether to use a . PRINT
command, a . PLOT command, a . PROBE command, or some
combination of the three. Regardless of the form of the output
                                                                             NnSSOn
                                                                             NIISSOfl Computing the natural response of
data, you must choose appropriate values for TSTEP and
                                                                       RL circuits (Section 8.1, pp. 254-262), RC circuits
TSTOP, the time increment and ending time for the PSpice anal-
                                                                       (Section 8.2, pp. 263-267), and RLC circuits (Secs.
 ysis. For simple circuits, you can make decisions concerning          9.1-9.2, pp. 322-339)
 TSTEP and TSTOP by means of a preliminary circuit analysis.
 Time constants and frequencies of oscillation are important
 characteristics that influence these decisions. For more compli-
 cated circuits, a trial-and-error approach may be necessary be-
 fore you can satisfactorily choose a TSTEP and TSTOP.
   Example 9 illustr缸es how to use PSpice to find the natural re-
 sponse of a series RLC circuit. We incorporated a preliminary
 analytic solution as part of the example to permit checking the
 validity of the PSpice solution.



 EX A M P L E             9

 a) Analyze the natural response of the circuit shown in Fig. 27
    with respect to the type of damping, the peak value of v, and
    the frequency of oscillation.
 b) Write a PSpice source file to generate a plot of the voltage v,
    versus t for the circuit shown in Fig. 27.                         FIGURE 27 The circuit for Example 9.
44                                                                 TIME- DEPENDENT CIRCUIT RESPONSE


c) Analyze the plot obtained in (b) and check its values against
   the predicted values obtained in (a).
d) Modify your source file to produce a PROBE data file. Then
   use PROBE to generate a plot of the voltage v. versus t and
   use the PROBE cursor to identify the peak value of the
   voltage.



S 0 L U T I                       0 N

a) For the series circuit shown in Fig. 27, a = R/2L = 1어0,
   a2 = 106, and w = 1/LC = 50 x 106. Hence the response
   is underdamped, and the roots of the characteristic equa-
   tion are sl = -1000 + j7000 md/s and 52 = -1000
    - j7000 rad/s. Therefore the form of the solution for v. is

                       v, = (B1 cos 7000t + B2 sin 7000t)e4'여X노.

     From the initial conditions,

                                               dv
           q                  m 10                              45,000 V/
                                                   (0
                          =             and
                                        20d                 =
                                                 dt
                              -
                          =
                 (0)
                 (0)
                                                        )                   s.
            vr
     Solving for B1 and B2 yields

      U', = (- 10 cos 7000t + 5 sin 7000t)e크000t V,                         t 之 0.

   Based on the solution for v, the peak value of v is 7.70 V,
   and it occurs at t = 362.29 尸S. The damped frequency is
   7000 rad/s, and thus the damped period is 897.60 尸s.
b) From the preliminary analysis of the circuit we select TSTOP
   to be 2000 尸s, so we can analyze the first two cycles of the
   response. Selecting TSTEP to be 20 ps gives 100 points be-
   tween 0 and 2000 杉s and should result in a reasonable graph.
   If the resulting plot is not to our liking, we can always rerun
   the analysis with different values of TSTEP and TSTOP. The
   PSpice source file is:

     Natural            Re하岫n드臼 口f an PLC 亡i rC 1.1 i t
     C:1     1          0        2E小6       IC: 缶 --1 (:)
     只1      1          2       20
     Li      2          (:)      1 아三召      IC == --91:)日--3
     . IRAN                 2）日-6      코：k：山e냐;          UIC:
     .PLOT                  TRAN      V (1)
     . PROBE
     .END
                                       7. 4 NATURAL RESPONSE                                                                                   45


Figure 28 shows the results of this PSpice analysis.
          TIME         V ( 1)
       ( 斗)                -1 . 0000E+01   -5. 0000E+00               0. 0乂乂1E+00           5. 0000E+O0                        1 . 0000E+0 1

         0. 000E+00 巾1 口 000E+01 斗
         2. 000E-05 -9. 015EI-00 .     *
         4. 000E-05 -7. 日日7E+00 1          共
         6. 000E-05 -6. 664E+00 .              *
         B. 000E-05 -5. 364E+00 .                  共n
         1. 000E-04 -4. 029E+OO .                   .   *
         1..ZOOE-04 -2. 652E+00 .                                 *             .
         1. 400E-04 -1. 289E+00 .                                          *    .
         1. 600E-04 5. 494E-02 1                                                *
         1. 800E-04 1. 341E+00 .                                                .   *
         2. 000E-04    21554E+00 1                                                          *            .
         2. 200E-04 3. 672E+00 .                    1                                               *    .
         2. 400E-04    41671E+00 .                                                                      퓻1
         2. 600E-04 5. 550E+00 .                                                                         . *
         2. 800E-04 6. 276E+00 .                                                                         .     *
         3. 000E-04 6. 867E+OO .                                                                         .             *
         3. 200E-04 7. 286E+00 .                                                                                           *
         3. 400E-04    7. 567E4-OO .                                                                                           *
         3. 600E-04 7. 670E+OO n                                                                                               *
         3. 日OOE-04 7. 642E+00 1                                                                                               *
         4. 000E-04 7. 446E+00 .                                                                                           *
         4. 200E-04    7. 135E+00 .                                                                                        *
         4. 400E-04    6. 677E+00 1                                                                      .         *
         4. 600E-04 6. 128E+00 .                                                                         -     *
         4口BOOE-04 5. 463E+00 .                                                                          . *
         5. 000E-04    4 1735E+OO .                                                                     퓻．
         5. 200E-04    3. 927E+00 .                                                                 *    .
         5. 400E-04    3. 089E+OO .                                                             *        .
         5. 600E-04    2. 211E+00 .                                             .       *
         5 . 日00E小04   1. 334E+00 .                                             .   共
         6. 000E-04    4. 5日0E叫01 口                                             . 뷰
         6. 200E-04 -3 1887E-01 1                                              共．
         6. 400E尸04 -1. 198E+00 .                                          *
         6. 600E-04 -1. 952E+OO .                                      *
         6. 800E-04 -2. 638E+00 .                                 *
         7. 000E-04 -3. 251E+00 -                             *
         7. 200E-04 -3 .770E+00 .                       *
         7 .400E-04 -4. 205E4-00 .                  . *
         7. 600E-04 -4. 533E+00 .                   . 共
         7. BOOE-04 -4. 771E+00 n                   .*
         日1000E-04 小4. 895E+00 1                    퓻
         日口 小)OE-04 -4. 934E+00 1                   퓻
         B. 4（心E-04 -4. 日61E+C乂｝ 口                  斗
         8. 600E-04 -4. 712E+00 1                   . 斗
         8. 日OOE叫04 -4. 463E+00 1                   . 共
                   '4 -4. 151E+Ot) .
         1크 . 000E니：                                . 斗
         9口200E-04 -3. 758E+00 -                    .   *
         '3. 400E-04 -3. 319E+00 .                  .     *

         (continued)                                                                FIGURE 28 The PSpice-generated plot for
                                                                                    Exan耳）le 9.
46                              TIME- DEPENDENT CIRCUIT RESPONSE


  9. 600E-04 -2. 822E+00        共，
  9. 8（뇨）E叫04 叫고 . 300E+（乂1
  1. 000E-03 -1. 744E+00          퓻
  1. 02QE-03 -1. 1日4E+00
  1. 040E-03 -6. 162E-01
  1. OGOE-03 -6. 253E-02
  1. C)80E-03    4. 734E-01
  1. 100E-03      工788E-01
  1. 120E-C)3    1 . 445E+00             '共
  1. 140E-C臼 1.日68E+00                        共
  1. 160E-03     2. 234E+00
  l . 1日0E-03    2. 54日E-s-00
  1. 200E-03 2. 795E+00
  1 . 220E-03    2. 크86E+00
  1. 240E-C口 3. 103E+C山
  1. 260E-03 3. 164E+00
  1..280E-03 3. 153E+00
  1. 300E-03     3. 091E+00
  1. 320E-03     2. 크62E+00
  1 . 340E-03    2. 7 恥：)E+00
  1. 360E-03     2. 561E+00
 1 . 380E-03     2. 301E+00
 1. 400E-03      1 口 99日E+C)0
 1 . 420E-03     1 . 675E+00
 1. 440E-03      1. 326E+00
 1 . 460E-03     9. 69日E-0 1
 1. 480E-03 6. 047E-01
 1 . 500E-C口 2. 44 '크E-0 1
 1. 520E-03 -1. 078E-01
 1 . 540E-03 -4. 438E中0 1
 1. 560E-03 -7. 583E-01
 1 . 580E-03 -1 . 047E+00
 1. 600E中03 -1. 302E+00
 1 . 620E-03 -1. 526E+00
 1. 640E-03 -1. 707E+00
 1. 660E-03 -1. 853E+00
 1. 680E叫03 叫1. 953E+00
 1. 700E-03 -2. 016E+00
 1. 720E-03 -2. 032E+00
 1. 740E-03 -2. 014E+00
 1. 760E-03 -1. 952E+00
 1. 780E-03 -1. 861E+00
 1. 800E-03 -1. 731E+00
 1 . 820E'-03 -1 . 57 크E-'-O0
 1. 840E-03 -1. 396E+00
 1. 860E-03 -1. 198E+00
 1. 8日0E-03 놔9.日08E小01
 1. 900E-03 -7. 564E-01
 1 . 920E叫03 小5. 229E-01
 1. '크40E크＝.K3 小2 n '弘)7E-0 1
 1. 960E-03 -6. 014E-02
 1 . 9日（：
        匠m0：크   l . 638E叫0 1
 2. 000E-03 ：크n 7日9E-日01



                                                  디GURE 28 (con加iued)
                                        7. 4 NATURAL RESPONSE                                                                                                                       47


c) From the output data, v (max) = 7.670 V, which occurs at
   t = 360 its. The damped period is 1260 - 360, or 900 杉s.
   All these measured values agree with our preliminary analy-
   sis. Note that the PSpice-generated line printer plot uses "E"
   in the exponential form for all numeric values.
d) Figure 29 presents the output from the PROBE graphics post-          b0y 丁
                                                                            !Vol tage
   processor, along with the cursor output value for the peak
   voltage level. To create this plot, modify the source file by
   adding the . PROBE statement. Run PSpice to analyze the cir-
   cuit again, and then run PROBE, either from the PSpice Con-
   trol Shell or from the operating system. When the blank
   graph appears, select Add trace from the main menu and in-
   put V(1) as the variable. The plot will appear on the screen.
   Select the Label menu item and the Text submenu item to la-
   bel the y axis as shown in the figure. Then select Cursor
   from the main menu and use the arrow keys to position the           -109 ------      1 1 r1 1 日1 小1 1 m中 m 4 ! 1 = = = 1 = = ＝十＝= =+4   1 1 11   1 mm 丁 m mm = = = m = = = = = 山 = m m


   cursor at the maximum value of V(1). Watch the cursor values            03
                                                                           ［희v (1)
                                                                                        0 5n,s                      1 0.,s                           1.5ms                      20ms

   box in the lower right corner of the display. This box contains                                             Ti ire                 Cl =
                                                                                                                                      C2 =
                                                                                                                                                    371. 930u,
                                                                                                                                                    400. 000n,
                                                                                                                                                                            7 7319
                                                                                                                                                                            -9 982
   the x and y axis values of the first cursor, Cl; the x and y axis                                                                  dif=          371 530u,               17. 714


   values of the second cursor, C2 (which is positioned by mov-            FIGURE 29 The PROBE-generated 히아 化r
   ing the arrow keys while pressing the shift key); and the dif-          Example 9.
   ference between the x axis values of the two cursors and the y
   axis values of the two cursors. PSpice and PROBE use the
   same characters for scale factor symbols (see Table 1) in x and
   y axis values and cursor box values, as you see in Fig. 29. Fi-
   nally, you can make a hard copy of the display by selecting
   Hard copy from the Cursor menu.




   PSpice also provides an alternative method for specifying mni-
tial conditions. This alternative method is most useful in circuits
containing capacitors and semiconductor devices. If the circuit
contains inductors carrying initial currents, you must snecifv the
initiai currents in tne element statements. Instead of including
the initial capacitor voltages as part of the element statements,
you insert them by means of an . IC control statement in the
source file.
   The format for the . IC control statement is:


  . IC     V(nodnum) = value          V(nodnum) = value . . .
   Note that the node voltages are specified with respect to the
reference node. Sometimes this method of entering initial capac-
48   TIME- DEPENDENT CIRCUIT RESPONSE


     itor voltages is more convenient than entering them on the mndi-
     vidual element statements. In either case we continue to use the
     UIC keyword on the . TRAN control statement, because we do
     not need a preliminary bias analysis.
        To illustrate use of the . IC control statement we rewrite the
     source file for Example 9 as:

       Natural Re히：h그n드e 口f an 只LO: i:1:ir, :uit
       * U5e c1f an .10 Statement
       Ci      1 (:)          고em6
       F극1     1      고       小：)
       Li      2 0            lO므--3
       1I i::    v c: 1 :) == -10
       1TRAN          20e-6        2000日-6  UIC:
       . PL（그丁        TRn卜'1      v (: 1 :)
       nPROBE
       nEND

     We leave to you confirmation that this source file generates the
     same solution as the source file given in Example 9.
                                                                                                                           49




CHAPTER 8
，各多好鈿匕晦辯瑟툐巾皿訥竝듀我耐叱坼蜘島心苞阿淀娜몬哮諍多




SWITCHES

In this section we present two of several ways to model switches
                                                                            NnSS0n
in PSpice. The first involves a specially constructed voltage               1끼115=51J11 Sequential switching incorporates
source, and the second involves control by a circuit voltage or       t니／o or more switches in a single circuit: Section 8.5,
                                                                      pp. 282-286
current.




8.1 PIECEWISE LINEAR SOURCE

The piecewise linear (PWL) time-dependent source allows you
to define a single-valued function at a series of discrete times.
PSpice determines the value of the source at intermediate values
of time by using linear interpolation on the input values. The 丘lct
that the function must be single valued implies that the values of
time used in the description of f (t) must continually increase.
One of the many uses for this type of source is as a model for a
switch.
   The syntax for a piecewise linear voltage source named
Vgpwl, positive at Ni and connected at nodes Ni and N2, is:

    Vgpwl       Ni      N2       PWL (Ti   Vi   T2   V2   . . .)

Each pair of values Tj, Vj (where j = 1, 2, . . . ) specifies that
the value of the source is Vj volts at Tj seconds. Note that you
specify the times in increasing order so that Ti < T2 < T3 <

  Example 10 illustrates the use of the piecewise linear source
for modeling a transient analysis problem. This example also
demonstates the . OP control statement discussed previously.
50                                                 S 싸 IT（거 ES


EXAMPL                      E    10

The circuit shown in Fig. 30 has been in operation for a long                               7.5k)1             2k)2

time. At t = 0 the 80-V source drops instantaneously to 20 V.
Write a PSpice source file, using a PWL source, to model this            )
                                                                         18
                                                                                   『
                                                                                   80 V              』*(1i
                                                                                                     30 kfI!                」 55
                                                                                                                                    I
circuit. The results of the analysis should be a plot of vO (t) ver-
                                                                                                                      7／
sus t.
                                                                       FIGURE 30 The 이rcu仕 幻rExam히e 10.
 S 0 L          U T I           0 N

To simulate the drop in voltage from 80 to 20 V we insert a
piecewise linear voltage source of opposite polarity in series
with the 80-V dc source. We then step the piecewise source from
0 to 60 V over a short time interval. At the same time we make
the duration of the 60-V step long enou합 that the circuit reaches
                                                                       vp (V)
its new steady-state condition. We must now decide how rapidly
the source must rise to 60 V and how long it should remain at                 60
60 V. We leave to you verification that the time constant for the
circuit shown in Fig. 30 is 40 ms. We select a rise time for
the piecewise linear voltage source of 40 ms/ 1000, or 40 尸s.
The duration of the 60-V source should be long compared with                              40 LL s                          400 ms

40 ms, so we arbitrarily select 10 time constants, or 400 ms.
The piecewise linear voltage source has the waveform shown in          FIGURE 31 A piecewise linear voltage source.
Fig. 31.
   Figure 32 contains the circuit shown in Fig. 30 re血awn in
preparation for writing the PSpice source file. In describing the
output for the analysis of this circuit as a plot of vO(t), which in
this circuit is the voltage at node 4, V(4), we take advantage of
the . OP control statement. Including the . OP control statement
causes PSpice to calculate the initial conditions just prior to the
application of the piecewise linear source. In other words, in this
type of transient analysis problem we use PSpice to calculate m i-
tial conditions automatically. Thus no IC = value entries are re-      FIGURE 32 The circuit shown in Fig. 30 modified
quired on the element statements, and we also omit the UIC             for PSpice analysis.
keyword on the . THA寸 control statement.
   The PSpice source file for plotting V(4) is:
서odel ing       n
                n   a S낯it:h s ith a Pie.:ewj드e Linear S口니｝r 1: e
         寸工 l
vi        i         (:) DC      日O




                    23O4D
Vipwl 1＋
       口            2   PWL o     O 4Oe-6    6O 4OO臼·-3 6O1)
Ri        2         3   7. 5日3

         334
R2        3         O   3Oe3
R3        3         4   2e3
C: i      4         r)  5e- 6
.OF'
口 TRnN              2e如3         2OOe-：크
. F' 只口BE
.END
                                                                                      51
       8. 2 VOLTAGE- AND CURRENT- CONTROLLED SWITCH ES


We leave to you verification that the output of the PSpice analy-
sis yields the following results.
                        t, ms               (t), V
                                           v。
                        0                  64
                        40                 33.67
                        80                 22.50
                                          (t) approaches 16 V
  Furthermore, the PSpice analysis shows v。
as t approaches m.




8.2 VOLTAGE- AND CURRENT- CONTROLLED SWITCHES

PSpice provides two special circuit components that you may use
to represent actual switches more accurately. One such compo-
nent is the voltage-controlled switch, wherein the switch action
depends on a voltage level elsewhere in the circuit. The other
component is the current-controlled switch, wherein the 읽Vitch
action depends on the amount of current flowing through some
other element in the circuit.
  The formats for specifying the voltage-controlled and current-
controlled switches are as follows:
       S兀工兀                   N1N2                   Cl C2             MNAME
                              니＝
                                   =H尸1J                          니＝
                                                                         1m\   H/


     Name of               Node                  Nodes 的r                Model
voltage-controlled      connections              controlling             name
      switch                                       voltage
      w工兀t              N1N2                     VNAME                 入4NA入4E
                       나尸日＝           /         뇨HHn/   1V             卞11/




     Name of            Node                     Name of                      Model
current-controlled   connections               zero-valued                    name
      switch                                  voltage source
                                             used to measure
                                            controlling current

Each format has four fields. The first field is the name of the
switch: If it is voltage-controlled, the name must start with "S"
(or "s"); if it is current-controlled, the name must start with "W"
(or "w"). The second field identifies the branch of the circuit that
contains the switch by naming both nodes. The third field
identifies the control for the switch: For a voltage-controlled
switch, the two nodes across which the controlling voltage is
defined go in this field; for a current-controlled switch, the name
of the zero-valued voltage source used to define the controlling
52   SwIT（거 ES


     current goes in this field. The fourth field contains the name of
     the model used to define the switch.
        In addition to identifying the switch in a data statement, you
     must use the . MODEL statement to define the switch model. The
     .MODEL statement, which can be used for a variety of different
     devices in PSpice, permits you to define parameters that are par-
     ticular to a given device. The form of the . MODEL statement is:
             .MODEL       MNAME           DNAME(PVALUES)
     where
       MNAME is the name of the model, used in the fourth field of
       the data statement defining the switch;
       DNAME is the name of the device being modeled, in this case
       VSWITCH for a voltage-controlled switch or I SWITCH for a
       current-controlled switch; and
       PVALUES are the values of the parameters used to define the
       device.
     Both voltage- and current-controlled switches have four device
     parameters. Each has a default value, so you need to set these
     parameter values in the . MODEL statement only if you desire a
     value other than the default value. The parameters are:
     Parameter Name        Definition                     Default value
     RON                    ON resistance, in ohms        1.0
     ROFF                   OFF resistance, in o끄［lls     1+6
     VON                   control voltage level for
                           ON, in volts                   1.0
     VOFF                   control voltage level for
                            OFF, in volts                 0.0
     ION                    control current level for
                            ON, in amps                   le-3
     10FF                  control current level of
                           OFF, in amps                  0.0
     Parameters RON, ROFF, VON, and VOFF are used for the
     VSWITCH model, and parameters RON, ROFF, ION and 10FF
     are used for the I SWITCH model.
       For instance, the following statements identify a voltage-con-
     trolled switch named Sab, located between nodes 3 and 4 and
     controlled by a voltage drop between nodes 1 and 5. The model
     of the switch overrides the default values for the parameters RON
     and VON.
     Sab       3 4         1 5        SMOD
     . MODEL       SMOD      VSWITCH (RON = 5, VON = . 2)
     We illustrate the use of these switches in Example 12 in Chap-
     ter 9.
                                                                                                                        53




CHAPTER 9


STEP RESPONSE


The easiest way to find the step response of a circuit is to insert a
dc source at the p아nt where the step change takes place. To ii-                N沁80n
                                                                               싸uI8SOfl Comput!ng the step response of RL
lustrate the insertion of a dc source we return to the circuit used     and RC circuits (Section 8.3, pp. 267-275) and RLC
in Example 9 (Fig. 27) and define the problem in Example 11.            circuits (Secs. 9.3 and 9.4, pp. 339-352)




EXAMPL            E      11

a) The switch in the circuit shown in Fig. 33 is closed at t = 0.
   At the instant the switch is closed, the initial current in the
   10-mi-I inductor is 90 mA and the voltage across the capacitor
   is 10 V. Figure 33 also shows the references for these initial
   conditions. Make a preliminary analysis of the step response
   and calculate the maximum value of v, and the time at which
                                                                        FIGURE 33 The circuit for Example 11.
   it occurs.
b) Write a PSpice source file to plot v versus t from 0 to 3000
   p.s in steps of 20 p. s. Use PROBE to generate the plot.
c) Compare the PSpice solution with the preliminary analysis.



 $ 0 L U T I          0 N

a) From the solution of Example 9 we already know that the re-
   sponse is underdamped. Furthermore, we know that sl =
   -1000 + j7000 rad/s, that s2 = -1000 - j7000 rad/s, and
   that the damped period is 897.60 尸s. The step-response solu-
54                                                 STEP RESPONSE


     tion for v, takes the form:
           ye = Vf + （引 cos 7000t + B{ sin 7000加-1여刃r.
     The initial values of v, and dv5/dt are the same as in Example
     9, and the final value is 21 V. Hence B{ = -31 V and
     B; = 2 V, so
      v. = 21 - (31 cos 7000t - 2 sin 7000t)e l0刃t,        t 之 0.
     The maximum value of v5 is 41.22 Vat 419.32 尸 s.
b) The PSpice source file is:
     Step Response      with an Ideal Switch
     Cl    0 1          2e-6     IC = 10
     Ri     1 2         20
              33   20
     Li     3 2         l0e小：3    IC == 9oe小：3
     Vi    3 0          DC     21
     .TR帥4 20e-6          3000e-6      UIC
     1PROBE
     1END

     Figure 34 shows the plot generated by PROBE. We selected
     the Cursor menu item to enable the cursor to move. The ar-
     row keys on your keyboard move the cursor labeled Cl; hold
     down the shift key while pressing the arrow keys to move the
     cursor labeled C2. The cursors allow you to read the values
     of v5(max) and Td directly from the PROBE plot.                    cv
c) The ou印ut of the PSpice analysis yields
                   v5(max) = 41.36 V,   at 436.8 尸 s;                 -200 +
                                                                          Os          2 5mm   1 0m, s      1 5nms    2 0mm       25mm     30,,

                        Td = 1336.8 - 436.8 = 900 尸s;                      r司．v (ll
                                                                                                        Tree        Cl = 435842, J      41 302
                                                                                                                    C2 =    13358,,,    29545
                        vi = 21 V.                                                                                  d, t= -900 000u,    11 815



     These results agree with the preliminary analysis.                   FIGURE 34 Plot of t-C versus t for Example 11.




                                                   Let's now consider a more realistic model of the step response: a
                                                   modification of Fig. 33, wherein we added a 引Vitch controlled
                                                   by the voltage step to the ioop. Example 12 considers the effect
                                                   of the nonzero switch resistance on the step responsm Uf the RLC
                                                   circuit.


EXA M P L E               12

Use PSpice to model the circuit shown in Fig. 35. Assume that
the voltage source is the same as that used in Example 11 and
                                                                    STEP RESPONSE                                                       55


use the same values in the . THAN statement. Assume further
that the resistance of the switch in the ON position is 10 f. Then
use PROBE to generate a plot of v. versus t. Compare the results
here with those in Example 11.


S    0 1 U I          I     0   N                                                        FIGURE 35 The circuit for Example 12.

The PSpice source file that models the circuit in Fig. 35 is:

    Step Re드p口nse with a Reali드tic S낯itch
    Vi      1 0     PWL (0  0  ie- 6   21    1000e卞6                              21:>
    Si      1 2     1 0      SMOD
    Li      2 3     iOe-3    IC = 90e-3
    Ri      3 4     20
    Ci      4 0     2e-6     IC = -10
    . 서口DEL    마I口D      VSWITCH ( RON == io: >
    .TRAN     20e-6      3000e-6      UIC
    . PROBE
    =END

Figure 36 shows the PROBE plot of v. versus t. Note that the
values of v.(max) and Td are different in the two cases because of
the resistance introduced here by the model of the switch.
        400 -



        30V



        20V



        109



         00



        105



        209+           1                                         r            4
           Os        05mm       1 0mm      15mm    2 0em       25mm      3 Sins
           回 v (4)
                                        Time      Cl = 430. 842uJ
                                                  C2 =   1 3319m,
                                                                      37. 154
                                                                      25. 197
                                                                                         디GURE 36 F기아 of vC versus r 幻r the circu仕 of
                                                  01f= -094 737u,     11. 957            Example 12.
                                                                         57



CHAPTER 10


VARYING COMPONENT VALUES

In PSpice you use the . STEP statement within a source file to
vary the value of a circuit element over a specified range. This
feature of computer-aided circuit analysis is very powerful, for it
allows you to see the effects of changing a circuit parameter on
the behavior of the circuit.
   You may use the . STEP statement in one of two ways. The
first allows sweeping the value over a range:

. STEP     STYPE      MNAME         SVALUE        EVALUE        CVALUE

where

   STYPE is the sweep type-use LIN to sweep the value lin-
   early from the starting to the ending value, use OCT to sweep
   the value logarithmically by octaves, and use DEC to sweep
   the value logarithm ically by decades;

  MNAME is the name of the component model defined in a
  .MODEL statement;

   SVALUE is the starting value for the sweep;

  EVALUE is the ending value for the sweep, which may be
  greater than or less than the starting value (that is, the sweep
  can go in either direction); and

  CVALUE identifies the way the sweep value changes-if the
  sweep type is LIN, CVALUE is the increment used to corn-
  pute the next value in the sweep, and if the sweep type is OCT
  or DEC, CVALUE is the number of values to generate starting
  at SVALUE and ending with EVALUE.
58   VARYING COMPONENT VALUES


       The other format for the . STEP statement defines a list of dis-
     Crete values to use:

           . STEP       MNAME        LIST        Vi   V2    V3   ...

     where MNAME again is the name of a Component model defined
     in a . MODEL statement, and Vi V2 V3 . . . are the values
     that PSpice will use for the Component.
       In order to vary the value of a resistor, capacitor, or inductor,
     you need to use a . MODEL statement to define a model for the
     component that you want to vary. We introduced the . MODEL
     statement in Chapter 8 with regard to voltage-controlled and
     current-controlled switches. The format is:

              . MODEL       入'IN시vIE       DNA入4E(PVALUES)

     where MNAME is the name of the model to be used in the
     . STEP statement, DNAME is a standard device name available
     in PSpice, and PVALUES are the values of the parameters that
     characterize the device you are modeling. The device names for
     resistors, inductors, and capacitors are R且S, IND, and CAP, re-
     spectively. The parameters of interest that characterize resistors,
     inductors, and capacitors are the resistance multiplier R, the in-
     ductance multiplier L, and the capacitance multiplier C. You use
     the multipliers to compute the actual sweep value, which is the
     value specified in the . STEP statement multiplied by the multi-
     plier. The default value for the multiplier is 1 for resistors, induc-
     tors, and capacitors.
        For instance the PSpice statements

         Ra         3   4      Rmod          I
         .MODEL         Rmod        RES (R=1)
         . STEP         RES         Rmod (R)       100     200     10

     cause PSpice to analyze the circuit 11 times, once for each of the
     following values of Ra: 100 {1, 110 {l, . . . , 200 ft Note that
     computing the value for Ra involves multiplying the line value
     (the value at the end of the statement line that describes Ra) by
     the value of R in the . MODEL statement and then multiplying
     that by each succeeding value described in the . STEP state-
     ment.
        Example 13 demonstrates how easily PSpice can analyze the
     same circuit several times with a different value of a given com-
     ponent used in each analysis. We used PROBE to illustrate graph-
     ically the varying behavior of the circuit as the component value
     changes.
                                          VARYING COMPONENT     VALUES                                                     59


EXAMPL             E               13

Use the . STEP statement to vary the value of the resistor in Fig.
37 from 20 f to 100 fl in 20-fl steps. Then use PROBE to dis-
play the value of v versus t for each of the resistor values.



                                                                         FIGURE 37 The circuit for Example 13.
 S 0 L U I         I       0 N

We modified the source file from Example 9 to include a varying
resistor value by using the . MODEL and . STEP statements:

  Eff日Ct; 口f Varying F: 口n PLC Natural 侘e名p口n드臼
  C:1      1  0      2e- 6
  L고       고  o      10e-3        II:: = 0m '恥：)e叫：크
  P1       1  고      F川OD         1
  . IC:      V (1) = --iC)
  . 卜捉）DEL      RNOD      RESI]꾸．== 1 :)
  .STEP      LIN   RES    RM0D 可）             20, 100, 20
  . TFnN      20e·-6       2C)C)C)e- 6        UIC
  . Fj카그BE
  1ENE)


  Figure 38 shows the PROBE plot of the capacitor voltage ver-
sus time. Note that the analysis using the smallest value of resis-
tance, denoted그 on the graph, has the smallest damping ratio.
Increasing the value of resistance increases the damping ratio.
The largest value of resistance is denoted V on the graph. We
leave to you confirmation of these results analytically.

            100V。
                l tage




                                                     1
                                                                         FIGURE 38 Plot of capacitor voltage versus time
              Os                   05mb
                                    (1)
                                                    15mm      2. Om      as the resistance is varied in the series RLC
                                                                         circuit of Fig. 37.
                       1   !   0   v
                                                                                                                       61




CHAPTER 11


SINUSOIDAL STEADY-STATE ANALYSIS

We now discuss the features of PSpice that 們rmit you to exam-
mlle how a circuit behaves in response to a sinusoidal input at a
fixed frequency. This behavior is the ac steady-state response of
the circuit.




11. ] 引NUS이DAL SOURCES

The following equations describe the damped sinusoidal voltage
source:
          Vg = Vo,   0 드 t 드 TD;
         vg = VO + VAe1e('尸Th) sin [2irFREQ(t - TD],                      Nilsson Characteristics of sinusoidal sources:
                    TD 드 t 5 TSTOP;                                 Section 10.1, pp. 372-377

where
     VO = offset voltage in volts;
       VA = amplitude in volts;
  FREQ = frequency in hertz;
       TD = delay in secon小; and                                    V9


        0 = damping factor in seconds '.
The default values of TD and 0 are zero, whereas FREQ defaults      Va
to i/ TSTOP. Figure 39 shows a graph of the damped sinusoidal
voltage.
  The syntax for a damped sinusoidal voltage source named VG,        0           TD                            TSTOP    r
positive at node Ni and connected to nodes Ni and N2, is:
  VG      Ni   N2     SIN(VO      VA   FREQ     TD    THETA)        FIGURE 39 A damped 이nusoid졔 \／이怡ge.
62                                             SINUSOIDAL STEADY- STATE ANALYSIS


                                                  When constructing any of the time-dependent sources, you
                                               should check a plot of its waveform before using it in a specific
                                               problem. You can check the waveform by first applying it to a
                                               pure resistive circuit. The output waveform in a resistive circuit
                                               is a scaled replica of the input waveform. You may always choose
                                               a convenient scaling factor for the test circuit. For example, as-
                                               sume that you want to check the data statement for the damped
                                               sinusoidal voltage

                                                           Vg = 12.5 + 25e_O·l(t_l) sin [0.4ir (t - 1)] V.

                                               If you apply this voltage to the voltage-divider circuit shown in
                             2                 Fig. 40, the output voltage is 0.8Vg.
                                                  The following PSpice source file is used to generate a plot of
             毋．
                                          +


                      BOIl            VO
                                               vO in PROBE. From that plot and tabulated values of vO you can
                                               check the correctness of the vg data statement.
                             1        i
                             0                                            d

                                                                   드0
                                                                          e
                                                 亡：i r C u i t                    t口 Che.:k:: a Damp日d Sinu드c1i d
     『 A voltage divider used to check c9.
                                                             d
                                                             土 l
                                                 V口                                SIN ( 12. 三3 可5 (:）月 .2 1 0. 1 :)

                                                                      h
                                                                      口 H
                                                                        n U
                                                                   U      日
                                                 됴：1                               20
                                                             凸
                                                             止
                                                 F모                                臼：)
                                                                              i
                                                 . I！라뇩N                  1
                                                                                      10       UI':;
                                                 . F'R口BE
                                                 .END




                                               11.2 SINuSOIDAL STEADY-STATE RESPONSE

                                               The general format for the control statement that implements a
                                               sinusoidal steady-state analysis has five fields:

                                                        . AC              ATYPE           NP      FSTART       FSTOP

                                                  The first, . AC, identifies the type of analysis. The second,
                                               ATYPE, identifies the method used to vary the frequencies. For
                                               sinusoidal steady-state analysis you should use the keyword
                                               U1N. The third field, NP, contains the number of frequency
姓隔轟凡枷如 Steady-sta也 circuit response to 引flu-   points. The fourth, FSTART, is the starting frequency, and the
soidnI inputs: Secs. 10.2-1 0.9, pp. 377-406   fifth, FSTOP, is the final frequency. For sinusoidal steady-state
                                               analysis at a single frequency, set NP to 1 and make FSTOP
                                               equal to FSTART, where FSTART is the frequency of the sinu-
                                               soidal sources. In steady-state sinusoidal analysis all sources in a
                                               circuit operate at the same frequency.
                 11. 2 SINUSOIDAL STEADY- STATE RESPONSE                                                 63

  In addition to the . AC control statement, a . PRINT state-
ment is required in order for you to get a printout of the desired
voltages and currents. The output voltages and currents are
phasor quantities, so you must specify whether you want polar or
rectangular values. For voltages, follow the letter V with M (for
magnitude), P (for phase), R (for real part), or I (for imaginary
part). Thus the statement

         .PRI町         AC      VM (1, 3)      VP (1, 3)

prints the magnitude and phase angle of the voltage between
nodes 1 and 3, the reference polarity for V (1, 3) being positive
at node 1. The statement

         .PRINT        AC     VR (l, 3)      VI (1, 3)

prints the real and imaginary components of V (1, 3) .
   You may also generate current outputs in either polar or
rectangular form. The statement

        .PRINT       AC      IM (VS01)        IP (VS01)

prints the magnitude and phase angle of the current in voltage
source VS01. The current reference is through the source from
the positive to the negative terminal. To obtain this same current
in rectangular form, you use the statement

       .PRI町         AC      IR (VS01)        II (VS01)

  Example 14 illustrates how to use PSpice to find the sin멥e-
frequency steady-state sinusoidal response.




EXAMPL          E       14

The sinusoidal sources in the circuit shown in Fig. 41 are de-
scribed by the equations                                                    1 11



    Vg = 20 cos (105t + 900) V       and      i8 = 6 cos 105t A.
a) Use PSpice to find the magnitude and phase of vO and iO.
b) Check the PSpice results obtained in (a) against an analytic
   5아ut幻n 的r VO and J.


                                                                     FIGURE 41 The 이rcu仕 幻r Examp厄 14.
64                                                                                                    SINUSOIDAL STEADY- STATE ANALYSIS


 S 0 I. U T I 0 N

a) We redrew the circuit shown in Fig. 41 in Fig. 42 in prepara-
   tion for writing the PSpice source file. The source file is:

      AC Steady State Analysis
     共 口f the C:irc나it in Figure 42
                =
                n
                l
     Vi     1 C)     AC:     20         恥
                    止
                    凸 知
                      口
            n
     Ii     O   '    AC:     6       C)
                i
     Ri     1 2      1
             二
             巾
     p고     2 3 3 4  45
                                          3
                        U
                        m
     P3
                    H
                    n
     Li     3 C)    30e- -6
     ':.i
                  2 3 4 5
            4 5     2. 5e-6
     VI0    5 0     DC:      C)
     . AC    LIN    1     15'크 15. 4'크       ! 5 '크 15. 4'크
     .PRINT   Ac: Vm (2)    Vp (: 2)   Im (: vIo:}      Ip (VID)
     1END


Note that we must specify the frequency in a PSpice source file
in hertz.


b) We obtain the solution for the phasor voltage V, by solving a
   sin멥e node-voltage equation:
                            V.   V.        :
                                       . V..-i20                                                            / . ,,"
                     4
                                                 "
                     4++ J3 + 3     j4
                                     4 +      l1
                                                                                          "



                                -
                                                                                                  =
                                                                                                           6L0
                             "                              '   .            '   "
                                 /3
     The solution for V, is                                                                                              FIGURE 42 The circuit shown in Fig. 41 prepared
                                                                                                                         for PSpice analysis.
                                          V, = 16.31L71.510 V.
     Hence
                            ,                      1乙
                                                    "                                ..   .   .            .
                            乙                                       =        26L124.64"
                                           3            j4
                                                         4
                                                                        3.
                                      =        H    "   .
                                               -
                                                                                                      A.
     The pertinent output from the PSpice analysis is
             VM(2) = 16.31                                      and                  VP(2) = 71.51'.
     Therefore VO = 16.31L71.510 V. Because
           IM(VIO) = 3.261                                          and              JP(VI) = 124.6,
     1 = 3.261L124.60 A.



                                                                                                      Example 15 illustrates sinusoidal steady-state circuit analysis
                                                                                                      when the circuit contains dependent sources.
                           11 . 2 SINUSOI DAL STEADY- STATE RESPONSE                                                        65



EXAM P L E                          15
                                                                                                            0.5 p.F
The sinusoidal voltage source in the circuit shown in Fig. 43 is                                  200 )

described by the relationship
                         Vg = 8.94 cos (25000t - 116.57') V.

   Use PSpice to find Va and Vb in both polar and rectangular
form.
                                                                                        디GURE 43 The circuit 化rExam히e 15.

S     0 L          U I     I    0   N

We use the following PSpice source file to obtain both the polar
and rectangular expressions for Va and Vb.

    AC: Steady State Analysis of the Circuit                             in Figure       43


    ql i l 2 l
             1 0       AC      8. 94      -116. 57
             2   C)    3   0      0. 20
                               -20


    VEFRR C
             3   0     Vg
             1   2     200
             3   0     40
             2   3     0. 5e-6
    .AC       U 1N     1      3978.日7        3978 . 日7
    .PRINT          AC    Vm (2)      Vp (2)     Vr (2)                       Vi (2)
    . F캬2INT        AC    Vm (3)      Vp (3)     Vr (3)                       Vi (3)
    .END


In this source file the independent voltage source Vi measures
the controlling current i小. Also, the current gain is -20, be-
cause the reference direction for i巾 is out of the positive terminal
Of Vg. Finally, the frequency of the source is converted from ra-
dians per second to hertz.
   The pertinent output from the PSpice analysis is:

    FREQ                       VM (2)            VP (2)             VR (2)             VI (2)



                口
       3. 979E+(：               1 , E;'크'크E+01   -4 . '크고BE十03       1 . 5日'3E+01      -1 . 376E-03



    FREQ                       VM (3:i           VP (, 3)           VR (3:)            V1 (3 .)



       :3 . '크79E+03            7. ‘크 '크LE+O I   小亡1 . '크28E -C乂3    7. '크‘크LE+01      -6 . 日78E-03



    Then
                 Va = 15.99L - 0.004928' = 15.99 -              j0.001376 V
66                                               SINUSOIDAL STEADY- STATE ANALYSIS


     and
           Vb = 79.96L - 0.004928' = 79.96 - j0.006878 V.
   We leave to you verification that these results are consistent
with an analytic solution for the circuit.
                                                                                                                          67



 CHAPTER 12


COMPUTING AC POWER WITH PROBE

 I he interactive graphics capabilities provided by PROBE offer               Nilsson Defining and computing sinusoidal
the opportunity to study the relationships among the various ac         steady-state power quantities: Chapter 11, pp.
power quantities. In this chapter we investigate the relationships      429-456
among current, voltage, instantaneous real power, average
power, instantaneous reactive power, and reactive power for the
circuit shown in Fig. 44. Although we introduce several new
features of PROBE, you do not need any new PSpice constructs
in order to investigate ac power.
    To begin, construct a PSpice source file for the parallel RC cir-
cuit in Fig. 44, being sure to include the . PROBE statement:
                                                                        FIGURE 44 A circuit used to investigate AC power
                                                                        relationships.
  r: jr, -uit
                        니
                        nH
                      U드ed to Dem口n日t rate 슥nal ye is 口f AC. Pow（크r

                      n U
                l



                      =
  \Jq                         SIN ('0      1130  15크15. 49 0 0)
                1
                1 1
                  l
  Ri                          4(: . .s
  1:1                         . 105e-6
  .IRAN                . 2em毛          100f?..f三
  . F'R（그S咀
  .END



Have PSpice complete the analysis of this circuit and then in-
yoke PROBE.
   When the blank graph appears with the main menu below it,
select the menu item Plot control. From the Plot Control menu
select Add plot three times, which should give four blank plots
on the screen. You can plot many different variables in these
four plots and compare them. To switch among the four plots,
you must choose Select plot from the Plot Control menu.
  First, select the top plot on the screen-the symbol >>SEL
should appear next to that plot. Exit the Plot Control menu, re-
turn to the Main menu, and select Add trace. Then choose the
variable V (1) to plot the voltage supplied by the source to the
68                                                                                            COMPUTING AC POWER WITH PROBE


                                                                                           parallel RC impedance. The plot should look like the first one
2005 丁                                                                 -
                                                                               -...      i (top. )showninFig.
                                                                                                                45.
                                                          //
                                                                                            .Next, select tne seconu plot on.tne screen anu plot me currenL
                                                                                                                               .    .          .   . .           .




                                                                                      \\
                                                                                         ; through the source. Note tiie pnase reiationsnip Detween tiie
     L/
200V;Vol tmge
20。V+                                                  -/ 기                ,
     口 v (l)
                                                                                           source voltage and current: The current leads the voltage be-

 100 Cu"rent                 11
                                                                           1               cause the load is capacitive. Compute the power factor angle of
                                                                                           the load as follows:
      口 1 (vO)
1 0K 丁
                                                                                                                 ZL = R II 1/ jwC
                                                                            ＼二二켜
      Pomer0inttS)                                                                                                      R
-1 0K+
     口 -V (1）퓻i (vg) 9                0. 翕180m5. 50共cos(-3已87/ 57 3)
                                                                                                                      加RC + 1 '
                                                            N,1\
      。er
  400p。          (watt
          r\             /                                                                                      LZL = 0 - arctan (wRC)
                                                                                                                    = -arctan (l05 . 40.5 . 0.185 x 10기
                                  f            뎌             =
  어UU 十

     Os                   20u3       4Cus          SOus                    80mm       looms
      口        8 (l) ii (ml) 口 05共18아5 55共sir,(-30 87/573)
                                       Time
                                                                                                                    二＝ -36.870.
FIGURE 45 Some ac power characteristics from                                                     Now, select the third plot and graph the instantaneous power
the circuit shown in Fig. 44: top plot, source                                                supplied by the source. Recall that the expression for mstanta-
V이tage; second 히아， source current; third 히ot,
instantaneous and average power supplied by                                                   neous power is v (t) . i (t). PROBE allows you to supply algebraic
the source; bottom plot, instantaneous and re-                                                expressions when it prompts for the variable to plot, so you sim-
active power absorbed by the capacitor.                                                       ply type -v (1) * j (Vg) . Recall that V (1) is the voltage
                                                                                              across the source (which you plotted in the top plot) and i (Vg)
                                                                                              is the current through the source. Note that the minus sign ( - )
                                                                                              inverts the sign of the instantaneous power to conform to the
                                                                                              PSpice sign convention. In this plot you have confirmed that the
                                                                                               frequency of the instantaneous power is double the frequency of
                                                                                              the voltage and current.
                                                                                                  Now display the average power supplied by the source on top
                                                                                               of the plot of the instantaneous power. The formula for average
                                                                                               power is

                                                                                                                            P =     !
                                                                                                                                    乙
                                                                                                                                        VmIm
                                                                                                                                                    s
                                                                                                                                                   c。    (LZL)
                                                                                                                                                                     .




                                                                                              Select the top two plots, one at a time, and use the cursor to find
                                                                                              the maximum values Vm = 180 and Im = 5.56. Select the third
                                                                                              plot again and add the trace described by the expression:
                                                                                                                    . 5*180* 5. 56*cos (- 36. 87/ 57. 3)

                                                                                              Divide the impedance angle (LZL = 36.87') by 57.3 to convert
                                                                                              the angle from degrees to radians, as required by PROBE. In the
                                                                                              t血d plot shown in Fig. 45, the equation for average power pro-
                                                                                              duced a strai합Lt line that runs through the center of the plot of
                                                                                              instantaneous power, as you might have expected.
                                                                                                 Use the fourth plot to examine the reactive power in the cir-
                                                                                              cuit. On the fourth plot generate a plot of the instantaneous
                                                                                              power absorbed by the capacitor. Note that this is instantaneous
                          COMPUTING AC POWER WITH PROBE               69


reactive power, whose average value is zero. On top of this plot,
place the plot of the reactive power supplied by the source,
which is described by the expression:
           . 5*180*5. 56*sin(-36. 87/57.3)

You have completed the plot shown in Fig. 45. Now try to de-
scribe the relationship between the instantaneous and average re-
active power absorbed by the capacitor.
  This exploration of the ac power characteristics of the circuit
shown in Fig. 44 using the power of PROBE necessarily has
been brief. You should take the time to investigate further; try to
construct plots of complex power, for example.
CHAPTER 13


MUTUAL INDUCTANCE

A PSpice source file requires three element statements to de-
scribe a pair of coils that are magnetically coupled. Each coil in
such a pair requires a statement that contains the name, the                       Nn$$0n
                                                                                   NIISSOfl Analyzing circuits containing magnet-
polarity-sensitive node connections, and the self-inductance of             ically coupled coils: Secs. 13.2 and 13.3, pp.
the coil. The first-named node of each individual coil description          506-514
is the dotted terminal. The third statement identifies the coupled
coils by name and states the value of the coefficient of coupling
k. The name used to identify the coupled coils must start with
the letter K, and the value of k must be greater than 0 and less
than 1.                                                                                                          10

   We illustrate the PSpice description of two magnetically cou-
                                                                                                     0.8
pled coils with those shown in Fig. 46. If this pair of coupled
coils is named KCCPAJR and the individual coils are Li and L2,
the three PSpice statements are:

  Li           7   日     5
  L2           9   IC)   20                                                 FIGURE 46 A pair of magnetically coupled coils.
  KCCPAIP           Li    L2       c'. e


   Recall from our overview of data statements in Chapter 1 that
every node in a circuit must have a dc path to the reference
node. However, when a circuit contains magnetically coupled
coils, one part of the circuit may be isolated from another part
insofar as dc signals are concerned. If this happens, you must es-
tablish a dc path between the isolated portion of the circuit and
the reference node. You may do so by either coalescing two iso-
iated nodes into one node using a single conductor or by joining      (a)
                                                                                                           )b)
the two isolated nodes with a resistor. Figure 47 summarizes the
two techniques.                                                             FIGURE 47 Providing a dc path between magneti-
                                                                            ca卯 cou히ed c에5: (a) co히escing is이ated
   Example 16 illustrates the PSpice analysis of a circuit contain-
                                                                            nodes with a single conductor; (b) joining iso-
ing magnetically coupled coils.                                             lated nodes with a resistor.
72                                                              MUTUAL INDUCTANCE



EX. AM P L E                              16


a) Use PSpice to find the rms amplitude and the phase angles of                               211                  JP   /2



   i1 and i2 in the circuit shown in Fig. 48 when Vg = 141.42 cos
   lOt V.
b) Check the PSpice solution by using it to show that the aver-
   age power generated equals the average power dissipated.
                                                                              디GURE 48 The circu仕 幻rExam이e 16.
     S   0   L   U I            I     0   N

a)
         Before redrawing the circuit for analysis by PSpice, we note
         that Vg = 100LO" V rms, f = 5/ j了 斗 1.59155 Hz, and the
         coefficient of cou戶ling k = 6/ V而 = 0.75. Figure 49 shows
         the PSpice circuit. The PSpice source file that yields the rms
         amplitude and the phase angle of i1 and i2 is :
         타；ample 口f 卜lutual Inductance                                                        V너                   V口




                  ll24        0236
         Vi      1 0       AC       100      0
         Ri      1   2     2                                                  FIGURE 49 The circuit shown in Fig. 48 redrawn
         Li      2   3     4                                                  for PSpice analysis.
         L2      4 6       16
                     L   1上
         Ku i     Li      L2      (1. 75



                  4635        5306
         R2      4   5     200
         R3      6   3     10e6
         Vii     3   0     DC       0
         V12     5   6     DC       0
         . AC     LIN      1      1. 5'크 155     1口 5'크155
         ..PRINT       AC     Im (VI1)       Ip (VI1)      Im(V12)             Ip (V12)
         .END

b) From the PSpice solution,
                         /l = 2.958L - 67.43O A(rms)                and
                         12 = 0.6929L - 16.09O A(rms).
         Using the PSpice solution, we find that the total average
         power generated is
                 Pg = (100)(2.958) cos 67.43O = 113.532 W.
         The average power dissipated in R1 is
                                     P1 = (2.958)2(2) = 17.500 W.
         The average power dissipated in R2 is
                               P2 = (0.6929)2(200) = 96.022 W.
         As Pg = P1 + P2, the PSpice solution is consistent with the
         conservation-of-energy principle.




                                                                               .    口,   ,d                                    i   n    1
                                                                                                                                       니，   r   ',   11
                                                                                                                                   73




CHAPTER 14


IDEAL TRANSFORMERS

 T ou can use a pair of magnetically coupled coils to model the                     NnSSOn
ideal transformers in a PSpice source file by making L1 and L2                      끼IlSSOfl Analyzing circuits containing ideal
                                                                              transformers: Section 13.6, pp. 524-529
large enough that oLi and wL2 are much greater than the other
impedances in the circuit. In addition to setting large values for
L1 and L2, setting the coefficient of coupling equal to 1 would be
                                                                                         2 11
convenient. PSpice does not permit you to do so, but you may
choose a value that is arbitrarily close to 1, say, 0.9999. You
bring the turns ratio of the ideal transformer into the model by
using the relationship L1/L2 = (N1/N2)2.
   Consider the circuit shown in Fig. 50, where Vg = 50 C05
 b0OOt V. From the circuit diagram, N1/N2 = 1/5 and therefore                 FIGURE 50 A circuit containing an ideal trans-
L2 = 25L1. In picking values for L1 and L2, we want n L2> >                   幻rmer.
200 { . As co = 1000 rad/s, if we make L2 = 200 H, wL2 will
be three orders of magnitude greater than R2. Therefore we pick
L2 = 200 H, and thus L1 = 8 H.
   We redrew the circuit in Fig. 50 in Fig. 51 to prepare for writ-
ing the PSpice source file to find the magnitudes and phase an-
햅es of m and V2. Note the insertion of a single conductor at the
bottom of the circuit diagram. It establishes a dc path between
 all nodes and the reference node. Thus we reduced the five nodes             FIGURE 51 The circuit shown in Fig. 50 redrawn
in the circuit shown in Fig. 50 to four nodes in the circuit shown            for PSpice analysis.
in Fig. 51.
    The PSpice source file that generates the magnitudes and
phase angles of v1 and v2 is:
    E
          f0고        n
     m
                         Ideal ir크n好 f口r m1므｝尸 i:: i rC u i t
     a
     X

          口
              Hmn
                             Ac:     50       0
              U
   \／口
   佇. 1            i         2
   Li     el l 2 3 L 3       B
          l
   L고                        200
          口
   Ki                     L고     1 드｝’크 '3日‘9
   P2                       200                                 (continued)
74                   IDEAL TRANSFORMERS


                     口AC        LIN        1      159. 1549          159. 1549
                     . F：下：1卜IT     AC         Vm그：)     Vp (. .)       Vm (:：王）         V口 (:：王）
                     .END


                     The pertinent output from the PSpice analysis is:

     F忙E（그             1／꺼 (2:)            VP t그：)         ＼小1(3:)            VP ( :3)


      1 . 듸'크고E+02       4. o(:)(:}E+c)1    2. 406E44-01     2. 0乂）E+02       - '3. 052E801


                     Hence

                                           V1 = 40L0.24060 V    and
                                           1今 = 200乙 - 0.90520 V.
                        We leave to you verification that the analytic solution for Vi
                     and V2 yields
                                  V1 = 40L00         and     V2 = 200L0" V.
                                                                                                                         75




CHAPTER 15


FREQUENCY RESPONSE

We turn our attention to the constructs in PSpice that permit
you to examine how a circuit behaves as a function of the fre-
quency of its input. This behavior is the frequency response of             Ni188O1l
                                                                            1끼1188( " Computing the frequency response
the circuit.                                                         of series and parallel resonant circuits: Chapter 14.
                                                                     pp. 553-588




15.1 SELECTING FREQUENCY VARIATION AND NUMBER

You use the . AC control statement, introduced in Section 11.2
for sinusoidal steady-state analysis, to obtain the frequency re-
sponse of a circuit. You have a choice of three frequency varia-
tions: linear, decade, or octave. When you select the type of fre-
quency variation, you must also select the number of frequencies
(points) if the variation is linear or the number of frequencies
(points) per decade (octave) if the frequency variation is decade
(octave). Recall that a decade is a 10-to-i change in frequency
and that an octave is a 2-to-i change in frequency.
   Recall also that the general format of the . AC control state-
ment that implements a frequency response analysis has five
fields. The first contains . AC to identify the type of analysis,
and the remaining fields for each of the frequency variation types
are:

          .AC      LIN      NP     FSTART       FSTOP
          .AC     DEC       ND     FSTART       FSTOP
          .AC      OCT      NO     FSTART       FSTOP
76   FREQUENCY RESP0NSE


     where
       LIN = linear variation;
        NP = number of points;
       DEC = decade variation;
        ND = number of points per decade;
       OCT = octave variation; and
        NO = number of points per octave.

     In each case FSTARF and FSTOP are the starting and stopping
     frequencies in hertz.
       If you select a linear variation, the frequency increment 4f is

                        스／= FSTOP卜 FSTA1丁
                                        1JT, -


     For example, if FSTOP = 1801 Hz, FSTART = 1 Hz and the
     number of points is 181. Then


                        스／ =     I쁩1:
                                                 =   10 Hz
       If you select a decade variation, the frequencies within a given
     decade are

                            五 = FSD · l0可侖
     where FSD is the frequency at the start of the decade, ND is the
     number of points per decade, and k is an integer in the range
     from 1 to ND. For example, if ND = 20, FSTART = 50, and
     FSTOP = 5000, the frequencies in the decade between 50 and
     500 would be
                               fk = (50)lok/20,

     where k = 1, 2, 3, . . . , 20. Hence

                       fi = (50)101/20 = 56.10 Hz;
                       f2 = (50)102/20 = 62.95 Hz;


     If you select an octave variation, the frequencies within a given
     octave are

                             fk = FSO . 2k/NO

     where FSO is the frequency at the start of the octave, NO is
     the number of points per octave, and k is an integer in the
                        15. 2 FREQUENCY RESPONSE OUTPUT                            17



range from 1 to NO. For example, if FSTART = 400 Hz,
FSTOP = 3200 Hz, and NO = 10, the frequencies in the octave
from 400 to 800 Hz would be
                        fk = (400)2k/10

Hence

                 Ii = (400)20"' = 428.71Hz;
                 12 = (400)20"2 = 459.48 Hz;




15.2 FREQUENCY RESPONSE OUTPUT

You may use the . PRINT, . PLOT, and . PROBE statements for
PSpice output when the voltage and current variables are func-
tions of frequency. The formats for . PRINT and . PLOT are
similar to those used when outputting the results of dc analysis
(see Chapter 4) and transient analysis (see Section 7.2):

    . PRI町1        AC       OV1     <OV2 OV3          . . .>

.PLOT         AC        OVI      <(PLO1, PHIl) >       <OV2 <(PLL2, PHI2) >.   >

Note that the second field in each statement now contains AC to
identify the type of analysis that produced the data to be printed
or plotted.
  In ac analysis you may specify the voltage and current van-
ables in rectangular, polar, or decibel values. To obtain these
values, you replace the V and I in the usual format used to
specify voltage and current outputs with the following:

              VR or IR = real part;
               VI or II = imaginary part;
             VM or TM = magnitude;
              VP or IP = phase angle; and
            VDB or 1DB = 20 log,0 (magnitude).

 For example, VR(N1, N2) yields the real component of the
 voltage between nodes Ni and N2, and IR(Vxxx) generates the
 real component of the current in the voltage source Vxxx.
   Example 17 illustrates how to analyze the frequency response
 of a parallel RLC circuit with PSpice.
78                                                                               FREQUENCY RESPONSE


E X A M P L E                            17

a) The current source in the circuit shown in Fig. 52 is
                                                                                                                          中1L/>>\11
   50 cos wt mA. Use PROBE to plot vO versusf from 1000 to
   2000 Hz in increments of 10 Hz on a linear frequency scale.
                                                                                                                              k
                                                                                                                                                                                  I   ..
                                                                                                                                                                                  I
                                                                                                                                                   40 mH               0.25 cF        VO

                                                                                                                              8
b) From the PROBE plot, estimate the resonant frequency, the
   bandwidth, and the quality factor of the circuit.                                                                                                                                  .
                                                                                                                                                           (1
c) Compare the results obtained in (b) with an analytic solution
                                                                                                          디GURE 52 The 이rcuit 幻rExample ]7.
   for兀，4f, and 口．

 S 0 L U T I                            0 N

a) The PSpice source file for obtaining a plot of vO versus f is:
     Parallel      尸．LC ::ircuit   Used to
     퓻    IliListrat； 日 Fr equ日ncy P日sp口n드00
     Iq        0   1      AC:     50e- 3   C'
     P1        1   0       0
                          8e3
     Li        1   0        1n=
                              n
                          40e- 3
     Cl        1   0      1 25e나6
     1AC:       LIN         101      1000     코：H:)(:)
     . PROBE
     .END
b) Figure 53 shows the PROBE plot of vO versus!. We need to
   select the X Axis menu item and choose a linear range such
   as shown in Fig. 53. Using the Cursor menu item, we note
   that the peak amplitude of 400.0 V occurs at a frequency of
   1590.2 Hz in Fig. 53 (a). Thus we estimate the resonant fre-
   quency at 1590 Hz.
             400V                                          h                              4000 十
                    i Volta0K
                                                                                                Voltage
                    1

                 1
             3（力vi                                                                        300




                                                                                          2000




                                                                                          1000




              o4                                                                            0v +                                      1 느   기 =1
              1 0Kh             1 2Kh     1 4Kh           1 FKS       i. 8Kh      2 0Kh     1 0KS
                                                                                                                      r

                                                                                                           1 2Kh     i4K0              i5Kh                     i8Kh      20Kv
                回cli)
                                              ,
                                                                                              回nol)
                                              Frequency     Cl =   1 5902K,    400仄）0                                Frequency               Ci =     1 5521K,         282. 418
                                                            C2 =   1 0000K,     20 739                                                       C2 =     15321K,          282418
                                                            d17=   590 194,
       (a)
                                                                               379295     (b)                                                d, f=    -80 017.           0.000


                                                                                                          FIGURE 53 PROBE plot of vO versus f for
                                                                                                          Example 17, using the cursor in (a) to identify
                                                                                                          the resonant frequency and in (b) to identify
                                                                                                          the bandwidth.



                                                                                                                                                                                           t
                          ]5. 2 FREQUENCY RESPONSE OUTPUT           79


      To estimate the bandwidth we use both cursors to find the
   frequencies where vO = 399.7/V三 = 282.63 V. From the
   PROBE plot in Fig. 53 (b), the closest values are 282.42 V at
   1552 Hz and 282.42 V at 1632 Hz. Thus we estimate the
   bandwidth to be 1632 - 1552, or 80 Hz.
      We calculate the quality factor from the relationship Q =
   兀／可 = 1590/80 = 19.88..
c) A direct analysis of the circuit yields

                   1。= 1591.55 Hz;
                   Ii = 1551.76 Hz;
                   12= 1631.34Hz;
                   스f =12 = 11 = 79.58 Hz;
                    Q = 五／샵 = 20.

We summarize the comparison with the PSpice analysis as fol-
lo＼入／5:

         Quantity            Analysis         PSpice




          兀五玉可0
                             1591.55          1590.20
                             1551.76          1552.10
                             1631.34          1632.10
                               79.58            80.00
                               20.00            19.88

If necessary, we can obtain a more accurate analysis around the
resonant frequency from PSpice by rerunning the program with
different values of NP, FSTART and FSTOP.




  In Example 18 we use the . STEP command to vary the value
of the capacitor in the circuit shown in Fig. 52. We use PROBE
to look at the effect of this variation on the frequency response
characteristics of the circuit.



EXAM PL E               18

Modify the PSpice source file for Example 17 to step the capaci-
tor values from 0.15 尸F through 0.35 pF in increments of 0.5
p F. Then use PROBE to display the frequency response charac-
teristics for all values of capacitance. Comment on the effect of
the changing capacitance.
80                                                             FREQUENCY RESPONSE



S      0   L   U    T       I   0   N

The modified PSpice source file is:

     Ef f臼'2 t S 口f Varyina C: 口I-)
     * Parallel         RLC: Circuit        Frequency Re드5口on s（므
                   l
     Iq            1        A::     60e- 3            C)

                     nU
                      니U
     只1            C)       日呵3
     Li             H
                   (:)  H   中：h身，＜크
     f:i           C)       C:MOD         1
     . 川口DEL           CM（기）      CnF' (. C:== l ;)
     . STEP     C:AP     C：川OD 口：:1   0. 15e『唱           , 35e小6 . (:）드；E?.'0f5
     ,Al::      LIN         101       50)           :250c)
     . PR口SE
     .END
                                                                                  4008-,-
                                                                                            VoI t. ge
Figure 54 shows the PROBE plot. The smallest value of capaci-
tance produced the plot farthest to the right, denoted그 As the
capacitance increases, the plots move to the left. Hence the reso-                300V

nant frequency decreases as the capacitance increases. But we
expect this result because the equation for resonant frequency for
an R工？ circuit is                                                                 2008


                                        n
                                        Wr
                                             [1
                                                                                  b0oy

  Also, as the capacitance increases, the resonant peak becomes
sharper. That is, as the capacitance increases, the quality be-
comes higher. This result, too, comes as no surprise, because                       08+
                                                                                    0 4Kb               08Kb            1 2Kh        1.6Kb   2.0Kb
                                                                                                                                                       r
                                                                                                                                                     2 4Kh
                                                                                                                                                                 寸
                                                                                                                                                             2.6Kb
the equation for Q in a parallel RLC circuit is                                                    스    V   口   8 (1)
                                                                                                                                다equency


                                                                                  FIGURE 54 The relationship between changing Ca-
                                                                                  pacitance and circuit frequency response.




                                                               15.3 BODE PLOTS WITH PROBE

                                                               In Section 15.2 we described the method for generating a fre-
                                                               quency response plot with PSpice and PROBE. The . PRINT
                                                               statement for frequency response data can provide you with out-
                                                               put voltages and currents in several different forms: real and
                                                               imaginary parts, magnitude and phase angles, and dB magnitude
Ni怡S0n
I1l'bSUfl         Generating Bode plots from a cir-            and phase angles. PROBE also allows you to plot frequency re-
cult's transfer function: Secs. 17.6 and 17.7, pp.             sponse data by using these same forms. In Section 15.2 we plot-
705-722
                                                               ted linear voltage magnitude versus linear frequency. We now
                                                           15. 3 BODE PLOTS WITH PROBE                                           81


turn to another form: dB voltage magnitude versus log frequency
and phase angle versus log frequency. This is the form used to
generate Bode plots. Example 19 compares the exact dB voltage
magnitude versus log frequency and phase angle versus log fre-
quency plots to the Bode straight-line approximations using
PROBE.




EXAMPL                       E           19

Construct a PSpice source 丘1e to generate the frequency response
of the circuit shown in Fig. 55 for three different values of resis-
tance: 5 Cl, 50 Cl, and 500 Cl. Then use PROBE to plot the out-
put voltage magnitude in dB and output voltage phase angle ver-
sus log frequency. Finally, use the Label menu to overlay a
straight line Bode approximation plot and comment.

 S   0   L   U I                 I   0        N

In order to analyze the circuit three times with three different                         FIGURE 5' The cftcuit for Example 19.
values of resistance, we use a model for the resistor and step
through the values. The values required are listed in the . STEP
command. We need to perform some preliminary analysis of the
circuit to generate the values used in the . AC command: the
 starting and ending frequencies. We choose them so that the fre-
 quency band of interest, that is, the frequency band that contains
 the natural frequency of the circuit, is centered between the two
 end-point frequencies.
   Because this is a series RLC circuit, we know that the center
 frequency and the bandwidth are given by


                             幼＝          ，辰
                                                             and    月
                                                                         L
                                                                         R·
 For the circuit shown in Fig. 55, the center frequency is
                                                  1
                                                                   = 6324.56 rad/sec
         m" = V (25 x l03)(l x 10-6)
             二也 1000 H乙
 and the bandwidth ranges from
                                                       5
                                     w                     i。. = 200 rad/sec
                                                  25
                                                             -
                                                       <
                   l3narr。
                   夙m.
                                     *   =



                                         斗 32Hz
 82                                                                 FREQUENCY RESPONSE


 to



                                    255씌。. = 20000 rad/sec
                                                    -
                乃*
                          14. =
                                  斗 3.2 kHz.


Thus we choose 10 Hz as the starting frequency and 100,000 Hz
as the ending frequency, which places the center frequency in
the middle and provides adequate room for the wideband cir-
cuit's response. The PSpice source file is:

      RLC c:ircuit    Used to Illustrate      Bode Plots
                     02
      Ci      1   0      le- 6
      Ri      1 2        RM口D      I
      Li      2 3        25e-3
      Vi      3   0      AC     1
      .MODEL        RMOD      RES (R=1:'
      .STEP       RES      RMOD.R)       LIST    5, 50, 500
      .AC       DEC     300      1(1     i00000
      . PR口BE
      .END



   After completing the analysis we enter PROBE and use the
menu system to create two plots on the screen. In the upper plot,
we add the trace of VDB(1), which is the magnitude of the
voltage across the capacitor in dB. Note that the frequency axis
is already logarithmic, because the . AC command specified
frequencies in decades. In the lower plot, we add the trace
of VP(1), which is the phase angle of the voltage across the
capacitor.
  Now use the Label menu selection and the Line option to
overlay the straight-line Bode magnitude and phase-an함e plots.
The transfer function for this circuit takes the form



                      月
                            （s)
                                    :   , :   *(*
                                                        才，
                                                             1/LC

 and so has two poles and no zeros. The frequency of the two
poles is the center frequency, w, which we have already calcu-                        NnSSOn Constructing straightline
                                                                                      NIISSOfl                           Bode plot
lated as 1000 Hz. The straight-line phase angle plot consists of                 approximations: Secs. 17.6 and 17.7, pp. 706-709,
t뇨ee lines: for cv < u1, the straight line has a value of 0" for all             711-713, 715-716, and 718-719
frequencies; for cv > u2, the straight line has a value of -180"
for all frequencies; and for u, < cv < u2, the straight line has a
slope of - 132/c degrees/decade. Note that ui = 4.814'oO,
ii2= 4.8 lcv,, and ( is the damping coefficient. For the straight-
                                15. 3 BODE PLOTS WITH PROBE                                                           83


line approximation constructed in Fig. 56, we use ( = 0.7, SO
i/l= 333 Hz and u2 = 3002 Hz. The two straight lines intersect
at the natural frequency, wO. Use the Line cursor to plot these
two lines. The straight-line phase angle plot consists of three
lines: for w < 0.1wO, the straight line has a value of 0O for all 40                             1-
                                                                                                                         十

frequencies; for w > l0w7, the straight line has a value of
 - 180O for all frequencies; and for 0.1wO < w < lOwO, the
straight line has a slope of - 90O/decade. Use the Line cursor to
plot these three lines.                                            -40
                                                                                               straightl Inc
                                                                                               approxi mat ion
   Figure 56 presents the PROBE plot and the overlaid Bode 00 +                      +
plot. Note that, as expected, the accuracy of the Bode approxi-
                                                                                                 -I-
                                                                       口 1 0 cdh (1)
                                                                                                                         十
                                                                    04＋吐＝느＝=＝之＝
mation is very good outside the band of frequencies, where the
magnitude and phase an햅e are changing. Within this band,
which spans one decade on either side of wO, the accuracy of the -100d+
                                                                                        straighti 1 ne
Bode approximation depends on the damping ratio of the under-                          approximation

lying second-order circuit. When the damping ratio is small
(( < 0.7), the approximation is not particularly good. Simi- 200엶h
                                                                                                                        너1
                                                                                                 1-
                                                                                                       1 PIth
                                                                                                            苡h       100Kh
                                                                            0vp (l)
larly, when the damping ratio is large (( ' 0.7) the approxima-                                 F r equen cv

tion is also not particularly good. Only when the damping ratio        FIGURE 56 Actual frequency response and
is close to 0.7 does the approximation more nearly represent the        straight-line approximation of the frequency re-
actual frequency response.                                              sponse for the circuit shown in Figure 55.
                                                                                                                                              85




CHAPTER 16


PULSED SOURCES

The syntax for a periodic pulse voltage source named Vpp1, con-
nected to nodes 1 and 0, and positive at node 1 is
Vppl     1    0      PULSE(V1 V2        TD   TR    TF    PW    PER)

  The pulse parameters are:
   vi = initial value (volts);
   V2 = pulsed value (volts);                                       V


   TD = delay time (seconds);
   TR     rise time (seconds);
    TF = fall time (seconds);
   PW = pulse width (seconds);
                                                                                                1
                                                                                                1
  PER = period (seconds).



                                                                                                                1m布＋ 땐作
                                                                                            TF니
   The de丘ult values for the time parameters are TD = 0,                                       TO
                                                                                                                                                   r

TR = TSTEP, TF = TSTEP, PW = TSTOP, and PER =
                                                                                                +
                                                                                               TR
TSTOP. TSTEP and TSTOP are specified in the . TRA寸 control                                      +
                                                                                               Pw
statement. Figure 57 shows a graph of the periodic pulse. We
discuss an illustrative application of a periodic pulse source in
Example 20.                                                             FIGURE 57 A periodic pulse voltage source.


E X A M P L E          20




                                                                                                    中L22닉／1 1
 The circuit shown in Fig. 58 is excited by an impulsive current
                                                                                                                          中
 source, where i: = 78 (t) A. Use PSpice to plot vO(t) versus t.
                                                                                                                              l
                                                                                  5fl
                                                                                                                                  小
                                                                                                                                      1
                                                                                                                                          1
                                                                                                                                               .


                                                                        FIGURE 58 The circuit for Example 20.
86                                                      PULSED SOURCES


S 0 L U I         I   0 N

To use PSpice to obtain a plot of vO(t) we have to construct a cur-
rent pulse that satisfactorily models the given impulsive current
source. We begin by making a preliminary analysis of the circuit
and studying the nature of the transient behavior. In particular,
we need to get a feel for how rapidly the transient response de-
cays. This understanding enables us to build a current pulse
whose duration is brief compared to the life of the transient
voltage. The roots of the characteristic equation contain the in-
formation we seek.
  For the circuit shown in Fig. 58, the characteristic equation is


                      5'＋命+ -L느0.
For the given values of R, L, and C, the roots are
              S1,2 = -a 士 jWd = -1 土 j7 radls.
Hence the impulsive response takes the form
            vO(t) = Bie_ " cos O. at + B2e_cnr sin edt,
and therefore the duration of the pulse should be short compared
to a, or 1 s. Furthermore, in order for the transient to die out
before the next pulse arrives, the period of the pulse train should
be on .the order of 5 a or 5 s.
   We select a pulse duration of a/ 1000, or 1 ms. So long as the
duration of the pulse is brief with respect to 1 s, the exact shape
of the pulse is not critical. For convenience we construct the
trapezoidal pulse shown in Fig. 59. We arbitrarily choose the
break points to occur at TO/5 and 4TO/5.
   Having decided on the general shape of the current pulse, we
must now determine the height of the pulse, 12. We know from
the material on the impulse function that the impulsive current
75 (t) instantaneously charges the 0.1 F capacitor to 70 V.
(When the impulse has passed, the response is identical to the
natural response of the circuit, that is, the response associated
with an initial capacitor voltage of 70 V.) Therefore the current
pulse must charge the capacitor to 70 V during its duration of           FIGURE 59 The current pulse for Example 20.
TO seconds. Thus

                        「=    { j   『   "i   dt = 70.

   The integral of the current is simply the area under the cur-
rent versus time curve, which we can easily calculate in this case
                                              PULSED SOURCES               87


without integrating:


                        '）牛느70.
                       「：
   As T。= 1 ms and C = 0.1 F, we have
                          12 = 8750 A.
   If we label the top node in the circuit shown in Fig. 58 as 1,
                                                (t) versus t is:
the PSpice source file that produces a plot of v。

   타；aaipi日 口f a Pui드E크d S.그U｝戶C臼
   Iq   0  1 PUL.SE (0        8750    C)  0. 2M   0. 2M       0. 6M   5)
   Ri   1  0   5
   Li   1  0   C) n 2     IC = 0
   Ci   1  0   0. 1       11 : 口 0
   1TRAN     iOe- 3   1400e-3      C)    le- ·3    UIC
   .PL口T     TRAN     V (l)
   ,END

Note in the . TRAN control statement in this source file that the
plotting increment is 10 ms, that the computation increment
is 1 ms, and that TSTOP is approximately 1.5Td, where
Td = 2ir/7 S.
  The output of the PSpice analysis gives the following results.
The voltage at 1 ms is 69.24 V; the first minimum value of v。oc-
curs at 411 ms and is -47.13 V; and the damped period is
1301 - 411 = 890 ms. We leave to you verification of these re-
suits.




                                                          1
                                                                                                                       89




CHAPTER 17


FOURIER SERIES

both PSpice and PROBE can help you to understand the fre-
quency spectrum characteristics of periodic waveforms. In
PSpice the . FOUR command computes and prints the magnitude
and phase angle of the Fourier series decomposition of the peni-
odic signal at dc, the fundamental frequency, and the second                Nn$SOn Calculating the Fourier series repre-
                                                                            거IISSOfl
through the ninth harmonic frequencies. Transient analysis must       sentation of a periodic waveform: Secs. 18.1-18.4,
precede Fourier series analysis, because the Fourier series           pp. 738-752 and Section 18.8, pp. 764-767
coefficients are computed for the last complete cycle for the tran-
sient analysis waveform. Therefore, the duration of the transient
analysis must be a least one cycle of the waveform. If you want
PSpice to compute the Fourier series coefficients of the steady-
state waveform, then the transient analysis should be performed
for a number of cycles sufficient to insure the decay of the natu-
ral response.
   The format for the . FOUR command is:
 . FOUR      FFUND         OUTVAR1       <OUTVAR2         . . .>
The first field contains the . FOUR command. The second field
contains the fundamental frequency of the periodic signal in
Hertz; recall that the fundamental frequency in Hertz is the in-
verse of the period of the signal in seconds. The third field con-
tains the variables for which the Fourier coefficients are corn-
puted. As usual, these variables must be voltages defined
between two nodes or a current defined through a voltage
source. Including a . PRINT or a . PLOT command is not neces-
sary, as the Fourier coefficients automatically print in the output
file as PSpice analysis proceeds.
                                                                             NnSSOn
                                                                             싸IISSOfl Defining the Fourier transform and
   If a PSpice source file contains a . TRAN statement, you may
                                                                      its properties: Secs. 19.1-19.6. pp. 789-805
use PROBE to calculate and display the Fourier transform
coefficients whether or not the source contains a . FOUR com-
mand. In fact, PROBE calculates the Fourier transform
90                                                  FOURIER SERIES


                                                    coefficients independent of any PSpice calculation of Fourier se-
                                                    ries coefficients. The frequency resolution displayed by PROBE
                                                    is inversely proportional to the extent in time of the transient
                                                    analysis. Therefore, if you want a more accurate Fourier trans-
                                                    form plot, you should specify a longer time for the transient
                                                    analysis. You reach the Fourier transform mode in PROBE by
                                                    choosing the Fourier entry from the X axis submenu.
                                                       Example 21 illustrates both the PSpice computation of the
                                                    Fourier series coefficients and the PROBE computation of the
                                                    Fourier transform coefficients.




EXAM P L E                21

Suppose that the pulsed waveform shown in Fig. 60 is input to           vU)
                                                                              +V
                                                                               1。
the RC circuit shown in Fig. 61. Use a Fourier series analysis of
the input waveform to predict the frequency content of the out-
put waveform for two values of C: 1 尸F and 10 尸F. Then use
the Fourier transform mode in PROBE to confirm the PSpice
                                                                                    10     20          30   40     50
analysis and to display the frequency spectra 앉aphically.



                                                                              10

 S 0 L U T I           0 N
                                                                        FIGURE 60 The pulsed voltage waveform input to
We begin by computing the Fourier series components for the             the 이rcu作 shown in F呼 61 .
pulsed voltage signal shown in Fig. 60. Note that this waveform
has two properties of symmetry: odd symmetry and half-wave
symmetry. These symmetry properties tell us several things
about the Fot玎妃r coe丘icients:
     ·The dc component is 0.
     ·The Fourier series has only sine terms; the an coefficients are
                                                                                                1kfl
       0 for all values of n.
     ·Only the odd sine terms are nonzero; the b. coefficients are
      0 for even n.
     1Because of the form of the an's and the be's, the Fourier co-
      efficients expressed in magnitude and phase angle form are        디GURE 61 An 尸（; 이rcu仕 with pulsed v이tage
                                                                        input.
             An = bn      and      On = -90,        for odd n;
      both the magnitude and phase angles are zero for the even
      harmonics.
                                                                                             F0URIER SERIES                     91


Because of waveform symmetry, we can simplify the formula for
the coefficients:

                      4
              b"= j J f (t) sin kojOt dt = 80/2何k,                                                         k odd.
                                fT12.              -                -          -   -




    Thus we can represent the input to the circuit in Fig. 61 as an
infinite series of the form

              ,   =   40         ／+
                               ‘比』            40                        ,,   / + 40
         D        =        sin w,t +
                           ,.
                                               -       SIfl
                                                       S.     3m
                                                              3w,            t +             sin
                                                                                             S.
                                                                                                    5w   ,,t   +.   .   .


                      7T                      3/7T                                     37了
         Vg
   The circuit shown in Fig. 61 is linear and exhibits the prop-
erty of superposition. To compute the response of this circuit to
the pulsed waveform, we consider the response to each term in
the Fourier series independently and sum those responses.
   From a phasor analysis of the circuit, we know that


                                                                        m加         C
                                                                                   R    9                                   +
                                           VOk = l                            O




which we represent in magnitude and phase angle form as

                                                            40
                                                            - L0.
                                                            kir
                      1乙k=
                                        \/(kwORC)2 + 12Larctan kwORC '

   The following table compares the magnitude and phase angle
of the input pulsed waveform with the magnitude and phase an-
gle of the voltage across the capacitor for the circuit with C =
1 杉F and the circuit C = 10 尸F, for the first three odd har-
monic frequencies. For the circuit with the smaller capacitor, the
magnitudes do not change much between the input and the out-
put. For the circuit with the larger capacitor, the magnitudes are
much smaller at the output than they are at the input at all har-
monic frequencies. We use PROBE to investigate this difference
further.

Harmonic              Vg                     v。,c = 1 肛I그                                         I뇨 C = 10 4itF
First                 12.7L00                12.1L - 17.4O                                        3.9乙 - 72.30
Third                 4.2L00                 3.1乙 - 43.3O                                         0.5乙 - 83.90
Fifth                 2.5L00                 1.4L - 57.5O                                         0.2乙 - 86.4O
92                                                               F0URIER SERIES


  The PSpice source file that describes the circuit shown in Fig.
61 with the smaller capacitor value and the input shown in Fig.
60 is:




     F乙그urier Serie드 Anal ysi드 口f RC Circuit     with F기Jl 弓e Input -小 Small C


                  ii2   020
     V口                PULSE (- 10    10 0 le- 6   le- 6   .01  .02)
     RI                1e3
     Cl                 le- 6
     . TRAN    l0e- 6      .06
     .FOUR     50     v (1)     v (2)
     .1카？
        ．口BE
     口END




Note that in the . TRAN statement above, TSTOP = 0.06 sec-
onds. The choice of a value for TSTOP is based on an analysis of
the time constant for this RC circuit, which for C = 1 jtF is
1 ms and for C = 10 /{ F is 10 ms. Thus, TSTOP is large enough
to allow a 6 time constant decay of the natural response for the
larger value of C, insuring that the Fourier series coefficients will
be computed for the steady-state waveform.
   The Fourier coefficients for the first nine harmonics for both
the input waveform and the output capacitor voltage are:




     FOURIER COMPONENTS OF TRANSIENT RESPONSE V (1)



      DC C:口서PONENT ==                    -4 . 001드)91E-C口

      HAf카I口NIC                FREOUENCY             F口URIER      N（가구．MALIZED     PHASE               N（가라IALIZED
         N（그                      (Hz .)           C:（긔네尸ONENT     C（가IPONENT      (: DE日：)           PHASE (DE日：)




         l   345678
                              5. oC山E+0 1          1. 273E+01      1. 000E+00     -3. 600E-02           0. 000E+00
                              1 . OC)OE-f02        8. 004E小03      6 . 2日6E-04    -戶'크 . (:) 11됴＋01   -9. 008E+01
                              1 . 500E+02          4. 244E+00      3. 333E-C)1    小1. 080E-01         --7. 200E-02




          二凸
                              2. 000E+02           e. 004E-03      6. 286E-04     -9. 023E+01         -9. 01 크E+01




                   늬
                   m
                              2. 500E+02           2. 546E+00      2. OC)OE-01    -'1. BOOE-01        --1. 440E-01
                              3. 000E+0크           8. 004E-03      6. 286E小04     -9. 034E+01         -9. 030E+01
                              3. SOOE+02           1. 819E+00      1 . 429E-01    -2. 520E-01         -2. 160E-01
                              4 . c:)C)C)E -+-c고   8. 004E-03      6. 287E叫04     -9. 045E+01         -9 . 041E+01
                              4. 500E+02           1. 415E+00      1. 111E-Ol     -3. 241E--01        -2. 881E-01
                                                              F0URIER SERIES                                                             93



 F（가JRIE三P CO서PONENTS （가＝ TRANSIENT RESP마寸SE V (2)




       DC C:口MPON巨NT =                     9. 914491E--·04

                                                    FOURIER          NORMALIZED               PHASE             NORMALIZED
       HARMONIC               FREQUENCY
                                 (HZ ")            亡0川PONENT          COM디그NENT               (: DE日：}         PHASE (DE日：)
          N（그




                 l2345日7日9
                                                   1 . 217E+0 1       1 . C>OC)E+C)O         -1 . 755E+0 1      0.. C00E+C>0
                             5. 000E+C) 1
                             1. 000E+02            1 - 685E-03        1 - 384E-04             5. 694E+01        7. 44'3E+01
                             1 . SOOE+02           3. 083E+00         2. 533E-0 1            -4. 425E+0 1      -2. 670E+0 1
                             2. 000E+02            1 . 223E小03        1 - 004E-04             3. 663E+01        5. 4 18E+01
                             2. 500E+02            1. 348E+00         1. 107E-01             -5. 83日E+01       -4 . 083E+Ot
                             3. 000E+0고            9. 147E-04         7 . 513E-05              2. 5 承：)E+01     4. 345E+01
                             ：크. 5（心E+C고           7. 45日E-01         6. 1고LE叫C）고            -6 . 656E+01      中4 . 寸:) 1E+0 1
                             4. 000E4-02           7. 1 크5E-04        5. 910E-05               1 . 847E+0 1     3. 602E+01
                             4. 500E+02            4. 駐｝1E小01         3. 763E-02             --7. 310E+01      -5. 555E+01


  Note that this PSpice analysis confirms our previous hand cal-
culations for the first three odd harmonics. Note further that the
even harmonics are essentially zero-valued; the nonzero values
that are printed arise because of the imprecision inherent in digi-
tal computer calculations.
  Now examine the graph of the time response for both the input
pulsed waveform and the output capacitor voltage produced by
PROBE shown in Fig. 62. Because of the small capacitor value,
the output voltage basically is able to follow the input voltage.
Finding that the Fourier coefficients of the input and output
voltages are so similar is not surprising. Figure 63, produced
                                                                                       i5V-
 100
                                                                                          1Volt.g.




  50
                                                                                       105




  TV



                                                                                        50

  5V




                                                                                        0 '나心＝J                                          5000
-'CV                                                                                                    lOCH   200H        3000   400H
                   lOss      20r5      30mm     40.5   50.5   60.5                         OH
       05                                                                                   口 cli) 1 v)2)
        口 cli)   0 V)2)                                                                                        Frequency
                                    Time


디GURE 62 PROBE time response 히아 化r the 尸C                                                     디GURE 63 P日OBE Fourier trans幻rm of the
circuit with small C.                                                                         waveforms shown in Figure 62.
94                                                                FOURIER SERIES


from Fig. 62 in PROBE by selecting the Fourier option from the
X axis submenu, graphically confirms this similarity.
    The PSpice source file for the circuit shown in Fig. 61 with
the large capacitor value and the pulsed input shown in Fig. 60
is:

     Four ier                 Analysis 口 f RC: Circuit       with Pul드e Input mm Lar口e C:

                        ii2    020
     Vg                                PULSE (- 10    10     0   le- 6 le- 6 .01 1C)2)
     只1                                 1e3
     Cl                                 l0e- 6
     1TRAN                     l0e- 6     .06
     1FOUR                     50     v (1)     v (2)
     aPROBE
     .END

The resulting Fourier series coefficients for the first nine har-
monics of the capacitor voltage, confirming the hand calcula-
tions presented, are:

  F口U尸．IER C（가IF'口NENTS （가r TRANSIENT RESF’口NSE V (: 1 :)


     DC COMPONENT 口                       -4 口 0019弓1E中03

     HAR셰）NIC                        FRE꾜UENCY     FOURIER        N마2川ALIZED        PHASE              N（가카朴뇩LIZED
        NO                              (: HZ)    COMPONENT        COMPONENT        ('. DE日:)         PHASE (DE日)




         l23 4   日789
                                 5. 0c：山E+01     1. 273E+ 01       1 . 000E-'-00   -3. 601E-02          0. 000E+00
                                 1 . 000E+0근     8. 004E-03        6. 286E-04      ··-9. 011E +01     --9. 0c:)GEl-01
                                 1. SOOE+02      4. 244E+C'0       3. 333E如01      -1. 0日0E-01        -7. 202E-02
                                2. 000E+02       8. 004E-03        6. 286E-04




              口口
                                                                                   -9. 023E+01        卞9. 019E+01
                                2. SOOE+02       2. 546E+C山        ;h (：川乂）E-01    -1. 801E-01        --1. 440E-01
                                ：크 . 000E +()고   8. 004E叫03        6. 286E- 04     -9. 034E+01        -9. 030Ef0l
                                3. 500E+02       1.日19E+00         1. 429E--01     小．고 1 521E-01      叫2. 161［三中（) i
                                4. 000E+02       日1 004E놔03        6. 287E-04      -9. 045E+(:>1      叫'크 .（뇨UE+01
                                4. 日）OE+02       1. 415E+00        1. 111E-Ol      --3. 241E-01       m2 1日81E-01


 FOUR I巨F. C:O꺼PONENTS （긔r TRANSIENT 尸．ESP（긔나SE V
                                                  ( 2:}

     DC: COMPONENT =                      -4. 14334 1E니：}2

     HAF:꺼ONIC                       FREQUENCY     FOURIER        N（가교MALIZED       PH슥SE              N（가교．MALIZED
         N（그                            (HZ)      C（가뱌가그NENT       COM尸ONENT        (: DE日:)          PHASE (DEG)




         l고34S67好
                                5. 000E-'-0 1     3. 日63E+OC>      1 . 000E+00     .··7 n 2.93E+ 01       0. 000E+00
                                主 . 000巨＋(）고       1 口 :304E-02    3. 374E-03      -1. 기：){3［三＋02     日m'크 . '7日'크E+01
                                1 . ZOOE+02        4 口 460E-0 1    1. 154E-01      -8. 556E+01        ·-.1. 263E+01
                                2. 000E+02        6. 573E-03       1 口 701E呻（X3    -1 . 752E+02



                 늬
                 m
                                                                                                      叫 1 . 02고巨＋02
                                2. 500E+02         1. 606E-01      4 口 156E叫02     냐3.日57E+01         -1. 564E+01
                                3 . 000E+0고       '4 .：크86E叫03     1. 135E-03      -1. 765E-4-02      --1 . 036E+02
                                3 口 E恥：)OE+02     8. 243E-02       고口 134E-02      --E了. 991E+01      -1 口 698E+01
                                4. 0c:)OEfc:)2    ：크1 고8 '크E-（口    8. 51고E小04      ·．·1 . 770E+02     -1. 04 1E+02
                                4. SOOE-'-02      5. 077E- 02      1. 314E--02     小‘3 口 101E+01      ．·0,1. E308E+01
                                                            F0URIER SERIES                                                              95


PROBE plots of the time response for the input and output
voltages, as shown in Fig. 64, illustrate that the large capacitor
value prevents the output voltage from following the input
voltage. Because the voltage waveforms are so different in the
time domain, you should expect very different Fourier co-
efficients. You saw this difference in both the hand calculations
and the PSpice analysis. The PROBE generated plot of the
Fourier transformed voltages shown in Fig. 65 further confirms
the different spectral content in the two waveforms.

                                                                             160                                                          ]

                                                                                   Vol t50e



                                                                             120




                                                                             8V




                                                                             40




-000                                                                         0v
       0s         LO. s   20ms      30mm   40ms   50ms   60mm                     0H              1004   2004            300H   4004   5004
        口 0 (1) 0 v (2)                                                            口 v (1) 0   v (2)
                                 Time                                                                    F r equetl CV


FIGURE 64 P日（JBE time response 히아 幻r the 尸C                                        FIGURE 65 PROBE Fourier transform of the
circuit with large C.                                                              waveforms shown in Figure 64.
                                                                       97




CHAPTER 18
H                ,




SUMMARY

PSpice is one of numerous software packages designed to simu-
late an electric circuit or network. One of the helpful features of
these simulation programs is that they allow the user to define
the circuit in terms of a topological, as opposed to a mathemati-
cal, description. Although the primary purpose of PSpice is to
 facilitate the analysis of circuits containing nonlinear electronic
components, we have introduced it to you as a tool for analyzing
linear, lumped-parameter circuits. There are several reasons for
 this early introduction. First, it acquaints you with a powerful
 computational tool. Second, you can test the computer-generated
 values by direct computation, thus gaining confidence in your
 ability to formulate correct source files. Third, the computer
 makes it possible for you to attack circuit problems that are corn-
 putationally very complex and lengthy if attempted without the
 aid of a computer. These complex problems often add signifi-
 cantly to your understanding of circuit behavior. Finally, simula-
 tion software is part of modern engineering practice. The intro-
  duction of such software at an elementary level is a first step in
 preparing you for what lies ahead.
                                                                        99




APPEND以 A


GUIDE TO PSPICE CONTROL SHELL
AND PROBE MENUS
I he software packages PSpice and PROBE are stand-alone exe-
cutable programs. Usually, you can execute PSpice from the op-
erating system prompt by typing pspice. PSpice will then ask
you to input the name of the source file you want to simulate.
The file name usually has the extension . d1R. When PSpice has
completed the simulation, it writes the results to a file having the
same file name as the source file and the extension . OUT. This
output file contains a listing of the source code and output from
the analysis, including data requested in the . PRINT commands
and plots generated by the . PLOT commands. You may examine
this output file on your terminal or by printing it on a line printer
or other hard-copy device.
   If you have included a . PROBE command in your source file,
PSpice will also create a file called PROBE.DAT. You may run
PROBE to examine your results graphically by typing probe at
the operating system prompt. PROBE then automatically reads
the file named PROBE.DAT produced by PSpice analysis.
   MicroSim has bundled PSpice and PROBE together, along
with an editor, an on-line help 町stem, an on-line manual, a cal-
culator, and several other helpful tools within the PSpice Control
Shell. The Control Shell is menu-based, and may make PSpice
and PROBE a bit simpler for you to use. In this appendix we
present a brief introduction to the menus that you encounter in
the Control Shell and to the menus that you use with PROBE.
100   APPENDIX A


      THE PSPIcE CONTROL SHELL MENUS

      Normally you enter the PSpice Control Shelit by typing ps at
      the operating system prompt, which brings up the start-up screen
      for the Control Shell. At the bottom of the start-up screen two
      lines are displayed. The first contains the file that you are cur-
      rently working with; if there is no current file, the space for the
      file name will be empty. The second contains the definitions for
      the function keys, which include Fl, F2, F3, F4, F5, F6, and
      ESC. To access these functions, simply press the desired func-
      tion key on your keyboard. The following functions are avail-
      able.
      Fl- Help Pressing the Fl function key opens a window on the
      screen containing context- sensitive help. That is, if you are using
      the calculator and you press F1, a help screen will appear and
      describe the use of the calculator. Similarly, if you are display-
      ing the submenu for the Files option in the Main menu, the help
      screen describes the submenu selections. You remove the help
      screen by pressing the ESC key.
      F2- Move Pressing the F2 function key allows you to specify a
      new position for an overlaid window, such as the help screen.
      Moving an overlaid window sometimes is necessary for you to
      view the text on the main window.
      F3- Manual Pressing the F3 function key activates the on-line
      manual. This manual describes the syntax for specifying all the
      components of a PSpice source file. It includes several examples
      of correct syntax for each PSpice statement. To use this manual
      outside the editor or the browser, select manual topics from sev-
      eral successive windows. If you are in the editor or the browser,
      the manual becomes context sensitive. That is, a choice within
      each window is 노ghlighted to correspond to the type of state-
      ment on the current editor or browser line. This aid makes cor日
      recting errors in your source file easy, without your having to
      refer to any PSpice manuals or texts.
      F4- Choices Pressing the F4 function key displays the Choices
      window, which contains a set of responses appropriate to the
      current context. For example, when the prompt appears for the
      input of the current PSpice source file, pressing F4 causes all
      files on the current directory with the extension . CIR to be dis-
      played in the Choices window. You may select from among them

      ' The following references the PSpice Control Shell, version 4.5 and the Design
      Center 3, version 5.1, both from MicroSim.
     GUIDE TO PSPICE CONTROL SHELL AND PROBE MENUS                   101


by using the keyboard arrows and pressing enter or by using the
mouse.
F5- Calculator Pressing the F5 function key displays the cal-
culator window and an on-line simulation of a hand-held calcula-
tor. Pressing the F1 key from the calculator window will tell you
how to use the calculator.
F6- Errors The F6 function key invokes the Errors window,
w노ch displays any errors encountered when PSpice reads in the
current file. Such errors are usually the result of incorrect syn-
tax. You can identify them by displaying the file in the editor
and correct them with the help of the on-line manual.
ESC-Cancel Pressing this key causes the current window to
be closed and the previous window to be restored.
   The Main menu items appear at the top of the start-up screen.
They support creation of a PSpice source file and permit you to
execute both PSpice and PROBE. The selections include Files,
Circuit, StmEd, Analysis, Display, Probe, and Quit. Al-
though these Main menu selections are always displayed in the
start-up screen, only those items that are highlighted or bold-
faced may be selected. To select a menu item, you may type the
first letter of the item you want, or you may move the cursor to
the menu item you want by using the arrow keys on the key-
board, and hit the Enter key. If you have installed a mouse, you
may use the mouse to move to the entry you want, then hit ei-
ther the left or right mouse key.


FILES
Selecting Files opens a pull-down menu with selections that per-
mit you to create and edit a PSpice source file, browse through a
PSpice output file, and specify the peripherals available on your
computer. The Files menu contains the following items.
Edit This option runs the editor built into the PSpice Control
Shell on the current file. You may use the arrow keys on the
keyboard to position the cursor within the editor window. You
may also use several keyboard control sequences to position
within the window. Pressing the Fl key while you are in the ed-
itor will help you to learn the simple editing commands. Exit the
editor with the ESC key.
Browse Output This option opens a window containing the out-
put file for the current file. The output file has the same file
name as the current file, but has the extension . OUT. The output
file contains the results from a PSpice simulation. You may use
102   APPENDIX A


      the arrow keys and the editing control sequences to move within
      this output file. The output file is read-only; you are not permit-
      ted to make any changes in this file.
      Current File This option opens a window which prompts you to
      input the file name for the current PSpice source file. Press F4 to
      get a list of all files with the extension . CIR on the current di-
      rectory.
      Save File This option allows you to save the contents of the
      current file to a file name that you input. This procedure is useful
      if you have made changes to the current file and want to save
      both the changed and the original files.
      X-External Editor This option executes an external editor on
      the current file. It allows you to use an editor of your choice,
      rather than the one included with the PSpice Control Shell.
      R-External Browser This option executes an external editor on
      the current output file. You may read the file but not change it in
      any way. Again, this procedure permits you to use a browser of
      your choice, rather than the one included with the PSpice Con-
      tr아 Shell.
      Display/Pmn Setup This option opens a window that permits
      you to specify the display type, the printer port and the printer
      type for your system. For each entry, pressing the F4 key per-
      mits you to choose from a list of valid options for your system.


      CIRCUIT
      The Main menu Circuit selection permits you to make changes
      to your source file without returning to the editor. You make
      changes by specifying the type of PSpice statement that you
      want to modify (Device, Model). Then a window opens to dis-
      play all the lines in the current file that correspond to the Se-
      lected statement type. You may choose the specific statement to
      change by hi맙li帥ting it with the arrow keys. Any changes that
      you make to particular PSpice statements are automatically in-
      corporated in the current file. Remember to use the ESC key to
      exit from each window level.


      STMED
      The StmEd (Stimulus Editor) allows you to specify the form of
      the independent voltage and current sources in the current file.
      Only minimal support of the Stimulus Editor is provided with
      the Student Version of PSpice, so we do not discuss this feature
      further. If the Stimulus Editor is available on your system, refer
     GUIDE TO PSPICE CONTROL SHELL AND PROBE MENUS                   103


to MicroSim's PSpice documentation for a full description of
this feature.

ANALY引＄
The Analysis pull-down menu allows you to specify the type of
analysis PSpice will perform on your source file. You already are
familiar with how to specify analysis within the source file; for
example, to perform dc analysis, you need a . DC statement in
your source file, whereas to perform transient response analysis
you need a . TRAiI statement. The Analysis menu item permits
you to specify or change the analysis type without having to en-
ter the editor. Selecting an analysis type automatically adds the
appropriate PSpice statement to the current file. The submenu
contains the following selections.
Run PSpice This selection runs PSpice on the current source
file.
AC & Noise This selection permits you to specify ac analysis
and its parameters. A window allows you to enter the values for
the . AC statement, which are then written into the current file.
DC Sweep This selection permits you to specify dc analysis and
its parameters. You enter parameter values into a window at the
prompts. The result is addition of a . DC statement to the current
file.
Transient This selection permits you to specify transient analy-
sis or Fourier series analysis and their parameters. Enter parame-
ter values into a window and use them in formulating the . TRAN
statement or the . FOUR statement, which is added to the current
file.
Parametric This selection permits you to specify the format for
a . STEP command, which is added to the current file.
Temperature This selection adds a . TEMP statement to the
current file and is beyond the scope of this manual.
Monte Carlo This selection governs Monte Carlo simulation of
the current source file and is beyond the scope of this manual.
Options This selection allows you to change or add options and
option values to the . OPTIONS statement in the current file. See
Appendix B for a definition of this statement.

DISPLAY
The Display option allows you to specify output variables to be
included in a . PRINT statement. That statement is then added to
the current file.
104   APPENDIX A


      PROBE
      The Probe option allows you to run PROBE, to add a . PROBE
      statement to the current file, and to control the contents of the
      PROBE.DAT file that PROBE uses. The submenu contains the
      following items.
      Run Probe This selection executes PROBE, the graphics post-
      processor software used to display the results of PSpice simula-
      tion.
      Auto-run This selection allows you to set a flag that causes
      PROBE to execute automatically after PSpice analysis. The de-
      fault value for the flag is YES.
      None/Some/All This selection allows you to specify the circuit
      variables to be included in the PROBE.DAT file used by PROBE.
      The default is ALL.
      Command File This selection allows you to specify the name of
      a PROBE command file and is beyond the scope of this manual.
      L雎 to File This selection causes PROBE to create a log file.
      The default is to disable creation of this log file.
      Format This selection allows you to specify whether the inter-
      mediate file maintained by PROBE is in binary or ASCII format.




      QUIT
      The Quit menu selection allows you to exit the PSpice Control
      Shell or to execute a single operating system command and re-
      turn to the shell. Your choice is made from a pull-down menu.




      USING THE CONTROL SHELL MENUS
      Although the description of the Control Shell menu system
      might seem a bit imposing, you should play with it in order to
      become familiar with its capabilities. The on-line Help windows
      and on-line PSpice manual can assist you greatly in creating a
      PSpice source file and executing PSpice and PROBE. In just a
      short time you will be able to master the Control Shell and will
      perhaps wonder how you could have ever used PSpice without its
      support. To get you started, we present a sample session.
         1. Type ps from the operating system to enter the PSpice
            Control Shell.
   GUIDE TO PSPICE CONTROL SHELL AND PROBE MEN US                   105


 2. Select Files from the start-up screen menu.

 3. Select Current File from the Files submenu and type in a
    file name for your source file at the window prompt. Be
    sure to include the extension . CIR with your file name.
    Hit the enter (return) key to make this file the current file
    and to return you to the start-up screen.

 4. Select Files from the start-up screen menu again.

 5. Select Edit from the Files submenu. If you have specified
    an existing file name for the current file, the file will ap-
    pear on the screen. If you are creating a new source file,
    the screen will be empty.

 6. Type in your PSpice source file if this is a new file name,
    or modify the current file if the file name 심ready exists.
    Remember to include the . PROBE statement if you want
    to run PROBE to display your results. When you have
    finished, hit ESC to return to the start-up screen.

 7. Select 幻lalysis from the start-up menu.

 8. Select Run PSpice from the Analysis submenu. PSpice
    then executes and displays screens that indicate its pro-
    gress in simulating the circuit you specified in the source
    file. When PSpice has finished, it returns you to the start-
    up screen.
 9. Select Files from the start-up menu.

10. Select Browse Output from the Files submenu and read
     through the output file produced by PSpice. If you want to
    print the output file, hit ESC twice to exit the browser and
    the Files submenu. Then select Quit from the start-up
    menu and DOS Command from the Quit submenu and
    input type filename. OUT at the window prompt, where
    file砒ime is the name of the current file. When printing
    begins you return to the Control Shell by hitting the enter
    (return) key.
11. Select Probe from the start-up menu.
12. Select Run Probe from the Probe submenu and use the
    Probe menu items to create your plots. The Probe menu
    item Exit will return you to the PSpice Control Shell.
13. To exit from the PSpice Control Shell, select Quit from
    the start-up menu and Exit to DOS from the Quit sub-
    menu. You will then see the operating system prompt.
106   APPEN D 1X A


      THE PROBE MENU SYSTEM

      PROBE is a graphics postprocessor software package that reads a
      special file written by PSpice (if you have included the . PROBE
      statement in your PSpice source file) and displays PSpice-com-
      puted voltages and currents in a graphic format. You can execute
      PROBE from the PSpice Control Shell or from the operating sys-
      tern prompt. PROBE is menu-driven; when you invoke PROBE,
      a blank plot appears on the screen, with the Main menu options
      at the bottom. You select an option from the Main menu by typ-
      ing the first letter of the option name, using the keypad arrows
      to highlight the desired option, and pressing the enter key,-or
      by using a mouse if one has been installed. Each option from the
      Main menu produces a submenu from which you may further
      specify your choice. In the following sections we describe the
      Main menu and submenu options that are useful in displaying
      simulation results for electric circuits constructed from the tools
      described in the Nilsson text. Menu options that control the dis-
      play of digital data, Monte Carlo analysis, and the like are be-
      yond the scope of this manual. MicroSim's PSpice Reference
      Manual contains detailed descriptions of PROBE's capabilities.



      THE START-UP MENU
      The Start-Up menu allows you to select the type of analysis that
      generated the data you want PROBE to plot. If only one type of
      analysis was specified in the PSpice source file, you will not see
      the start-up menu. If you have specified two or more types of
      analysis in the source file, you must choose which one to look at.
      The following start-up menu options are available.
      Exit program This option terminates PROBE and returns you
      to the Control Shell or to the operating system, depending on
      where you invoked PROBE.
      Dc sweep This option allows you to plot the results from an
      analysis specified with the . DC command. It invokes the Analog
      P1야 menu.
      Ac sweep This option allows you to plot the results from an
      analysis specified with the . AC command. It also invokes the
      Analog Plot menu.
      Transient analysis This option allows you to plot the results
      from an analysis specified with the . TRAN command. It also in-
      yokes the Analog Plot menu.
     GUIDE TO PSPICE CONTROL SHELL AND PROBE MENUS                      107


THE ANALOG PLOT MENU
The Analog Plot menu is the main menu in PROBE and is dis-
played at the bottom of the plot screen when it first appears.
Each menu item invokes a submenu from which you can select
further. The menu and submenus contain the following items.

Exit This selection exits the Analog Plot menu and returns you
to the Start-Up menu.

Add trace This selection adds one or more'traces to the current
plot, if more than one plot is displayed, the trace is added to the
plot currently selected (identified by the symbol SEL>> next to
the plot). The traces can be any output variables resulting from
PSpice simulation or an arithmetic expression involving the out-
put variables. Pressing the F4 key will display a list of valid vani-
ables from which to select. Refer to PROBE documentation for
examples of the use of arithmetic expressions.

Remove trace This selection removes one or more traces from
the selected plot. A displayed submenu allows you to select All
or specific individual traces for removal.

X axis This selection invokes the x-axis submenu. The submenu
options are similar to those in the y-axis submenu. We describe
the axis submenu items after the Y axis entry.

Y axis This selection invokes the y-axis submenu. Both the x-
axis and y-axis submenus contain the following selections.
  · Exit This selection returns you to the Analog Plot menu.
  · Log This selection specifies a logarithmic axis. For ac anal-
    ysis, the x axis is already logarithmic.
  · Linear This selection specifies a linear axis. Except for the
    x axis in ac analysis, all axes start out linear.
  1 Auto range This selection asks PROBE to choose a conve-
    nient range of values to be displayed on the axis. All axes
    start out autoranging and this submenu item does not appear
    at the start.
  ·Set range This selection allows you to enter a minimum
    and maximum value for the range of values displayed on the
    axis.
  ' Restrict data This selection appears on the x-axis submenu
    only. It is used to restrict the range of x-axis data used in the
    computation of the Fourier transform coefficients.
108   APPENDIX A


        ·Unrestrict data This selection appears only if the Restrict
          data item has been previously selected from the x-axis sub-
          menu. It is used to undo the effect of the Restrict data in-
          put.
        1X variable This selection sets the variable for the x axis; it
         appears in the submenu of the X axis menu item only. The
         x-axis variable default depends on the analysis type: voltage
         or current for a dc 引Veep, frequency for ac analysis, and
         time for transient analysis. You use this submenu item to
         override the default variable for the x axis. A prompt will
         ask you to enter the variable to be displayed on the x axis.
         This option allows you to plot any variable versus any other
         variable for a given analysis.
        1Fourier This selection invokes the Fourier transform mode
         of PROBE. All traces currently displayed are transformed. If
         the x-axis variable is time, a forward Fourier transform con-
         verts the x-axis variable to frequency; if the x-axis variable
         is frequency, an inverse Fourier transform converts the x-
         axis variable to time.
        ·Quit fourier This selection reverses the transformation per-
          formed by the Fourier selection and returns the x-axis vani-
         able to its original state.

      Plot control This selection invokes the plot control submenu.
      This submenu contains many items, including the following,
      which are most often used.
        ·Exit This selection returns you to the Analog Plot menu.
        ·Add plot This selection adds a plot to the top of the screen
          and selects the new plot. A maximum of 20 plots may be
          displayed. Each plot has the same x axis but can have a dif-
          ferent y axis.
        ·Remove plot This selection removes the selected plot from
          the 小splay.
        ·Select plot This selection allows you to change the selected
          plot using the arrow keys.

      Display Control This selection invokes the display control sub-
      menu and provides a method for modifying display attributes,
      which is beyond the scope of this manual.

      Macros This selection invokes the macro control submenu,
      which is beyond the scope of this manual.
     GUIDE TO PSPICE CONTROL SHELL AND PROBE MENUS                   109


Hard Copy This selection generates a hard copy of the current
display on the plotting device, w址ch usually is a printer with
graphics capabilities.

Cursor This selection gives you control over two screen cursors
that you can use to read values from the selected plot. You acti-
vate the first cursor by using the left and right arrow keys. You
activate the second cursor by holding down the SHIFT key while
using the left and right arrow keys. A display window in the
lower right corner contains the current values at the location of
the two cursors. A cursor submenu provides specific cursor
placement commands, such as Peak, Trough, Mmll and Max,
which are beyond the scope of this manual.

 Zoom This selection allows you to identify a section of the plot
 and zoom in or out. The effect is the same as changing the vani-
 able range on the x and y axes. The zoom submenu includes the
 following items.
   ' Specify region After you have selected this submenu item,
     press the spacebar to identify one corner of the zoom region.
     Then use the arrow keys or the mouse to move the cursor to
     the opposite corner and press the spacebar a second time.
     This creates the zoom box and causes the display to be re-
     drawn within that box.
   ' X zoom in This item causes the x axis to be zoomed in by a
     factor of 2 on the currently selected plot.
   ' Y zoom in This item causes the y axis to be zoomed in by a
     factor of 2 on the currently selected plot.
   ' Zoom out This item causes the display to be zoomed out by
     a factor of 2 in both the x and y directions.
   ' Pan This item pans various portions of the screen by 10%
     in the direction specified by the arrow key being pressed.
   ' Auto range This item undoes all previous effects of zoom-
     ing and panning.

 Label This selection enables you to label your plot with both
 symbols and text by selecting various Label submenu items. The
 items you will use most often are:
   e Exit This item exits from the Label submenu back to the
     Analog Plot menu.
    ' Text This item allows you to enter text at a prompt and use
      the arrow keys to place that text anywhere on the plot.
110   APPENDIX A


        ' Line This item allows you to create a single strai합1t line
          anywhere on the plot by specifying the endpoints of the line
          with the arrow keys.
        ' Delete one This item allows you to delete any single ele-
          ment previously entered on the plot from the Label sub-
          menu. You use the arrow keys to position the cursor over
          the item to be deleted.
        ' delete All This item allows you to delete all elements en-
          tered on the plot from the Label submenu.
        'Move This item allows you to identify any previously en-
          tered plot element and move it to a new location. The arrow
          keys identify the item and also identify its new location.


      USING THE PROBE MENUS
      As was the case with the PSpice Control Shell menu system, the
      PROBE menus may seem complicated and confusing at first. But
      the only menu option you actually need at first is Add Trace.
      You should play with the PROBE menus and discover how the
      menu items affect the displayed trace. In a short time you will be
      using PROBE in sophisticated ways to provide added insight into
      the functions of the circuit you are studying.
                                                                         111




APPEND以 B


SPECIFYING PSPICE SIMULATION
PARAMETERS
You can use two PSpice statements to control parameters for
PSpice simulation and the output file that PSpice produces. The
first of these statements is . WIDTH, which controls the number
of characters printed in a row of the output file and has the state-
ment syntax:
                   .WIDTH         OUT = value
where value is the number of columns in a row and must be 80
(the default) or 132.
   The second statement is somewhat more complicated. The
.OPTIONS statement allows you to change some of the default
values for parameters used in circuit simulations. The format for
this statement is:
. OPTIONS       OPT!      <OPT2      ...>    <OPTn = value        ...>
Options come in two varieties: those that do not have values as-
sociated with them and those that do have values. Options with-
out values usually are called flags. The following flags are re!e-
vant to the use of PSpice described in this manual.
  ACCT Includes accounting information at the end of the out-
  put file.
  EXPAND Creates a list of devices from expansion of subcir-
  cults.
  LIBRARY Includes all lines used in the source file from
  PSpice libraries.
  LIST Creates a summary of circuit elements.
  NOBIAS Bias values for node voltages are not printed in the
  output file.
112   APPENDIX B


        NODE Includes a node table to summarize circuit connec-
        tions.
        NOECHO Source file listing is not included in the output file.
        NOMOD Model parameters are not listed in the output file.
        NOPAGE Form feeds and headers are not included in the out-
        put file.
        OPTS Includes a list of all flags and option values in the out-
        put file.
        WIDTH Sets the width of the output file to 132 columns.
         The following options with values 町e described with their de-
      fault values and units. This partial list identifies the options that
      are relevant to the PSpice description included in this manual.
      See the MicroSim PSpice documentation for a complete list of
      all options.
        ABSTOL = (1 pA) Sets the error tolerance on circuit cur-
        rents.
        CPTIME = (1E6 sec) Sets the CPU time allotted for the sim-
        ulation.
        GMIN = (1E-12 ohme1) Sets the minimum conductance in a
        circuit branch.
        ITLi = (40) Sets the iteration limit for dc and bias-point
        computation when the source file provides no starting point.
        ITL2 = (20) Sets the iteration limit for dc and bias-point
        computation when the source file provides a starting point.
        ITL4 = (10) Sets the iteration limit for the computation of
        any point in a transient analysis.
        ITL5 = (5000) Sets the total number of iterations allowed
        for all points in a transient analysis. Setting ITL5 = 0 re-
        moves the limit on iterations.
        LIMPTS = (叫 Sets the maximum number of points to be
        printed in the output or on a plot.
        NUMDGT = (4) Sets the number of digits used for printing
        numbers in the output file.
        Ply'｛厄L = (1E-3) Sets the abs아Ut이恤如仙n value for a ma-
        trix entry to be accepted as a pivot.
        PIVTOL = (1E-13) Sets the relative ratio between the largest
        column entry and an acceptable pivot value.
        RELTOL = (.001) Sets the relative error tolerance for volt-
        ages and currents.
        TNOM = (270 C) Sets the nominal temperature.
        VNTOL = (1 尸V) Sets the error tolerance on circuit voltages.
                                                                     113




APPEND以 (


DIFFERENCES BETWEEN SPICE
AND PSPICE
I he differences between SPICE (that is, the software package
SPICE2G.6 from the University of California at Berkeley) and
PSpice fall into two categories. The first category contains the
differences that you will encounter in attempting to use PSpice
to simulate a circuit described by a source file originally pre-
pared for SPICE. The second category contains the differences
you will encounter in going in the other direction-that is, in at-
tempting to use SPICE to simulate a circuit described by a
source file originally prepared for PSpice. In the discussion that
follows, we identify only those differences relevant to using
SPICE and PSpice for simulating circuits from material in the
Nilsson text. Other differences exist with regard to both analog
and digital electronic circuits, but we do not cover them here.
Refer to the MicroSim PSpice documentation appendices for the
complete list of differences.
   With the following exceptions, any source file developed for
SPICE can be successfully read and simulated by PSpice.

   1. PSpice does not support the following option fields in
      the . OPTION statement: LIMTIM, LVLCOD, M巴THOD,
      MAXORD, LVLTIM, and ITL3.

   2. PSpice does not support the IN= option for the . WIDTH
      statement.

  3. Voltage coefficients for capacitors and current coefficients
     for inductors must be incorporated into the . MODEL state-
     ment rather than into the statement defining the device.


  In general, SPICE can read and simulate a source file devel-
oped for PSpice. However, some features available in PSpice are
114   APPENDIX (


      not supported by SPICE. Any source file that uses any of the
      following features would have to be modified before SPICE sim-
      ulation.
        1. SPICE does not support voltage and current controlled
           switches.
        2. SPICE does not support models for resistors, inductors,
           and capacitors, such as those used in conjunction with the
           . STEP command.
        3. SPICE does not allow logarithmic sweeps of dc voltages or
           currents.
        4. SPICE does not support sweeps of parameters in a . MODEL
           statement.
        5. SPICE does not support the . LIB statement.
        6. All characters in a SPICE source file must be uppercase.
                                                                      115




H
 APPENDIX D


QUICK REFERENCE TO PSPICE

DATA STATEMENTS

In the syntax for data statements, xxx represents any alphanu-
meric string used to identify uniquely a circuit component, n+
represents the positive circuit node and n- represents the nega-
tive voltage node. Positive voltage drop is from n+ to n- , and
positive current flows from n+ to n- . Any elements in the syn-
tax specification that are optional are enclosed by brackets ([ ]).



IN DEPENDENT DC VOLTAGE AND CURRENT SOURCES


SYNTAX (VOLTAGE)        Vxxx      n+    n-     DC     value

SYNTAX (CURRENT) lxxx             n+   n-     DC      value

    where
    value is the dc voltage in volts for the voltage source and the
    dc current in amperes for the current source.


DESCRIPTION Provides a constant source of voltage or current to
吐比 circuit.


EXAMPLES    Vin     1     2       DC   3. 5

            Isource           3    0   DC     0. 25
116    APPENDIX D


      INDEPENDENT AC VOLTAGE AND CURRENT SOURCES

      SYNTAX (VOLTAGE)       Vxxx    n+    n-      AC   mag   [phase]

      SYNTAX (CURRENT)   lxxx       n+     fl-    AC    mag   [phase]
         where
        mag is the magnitude of the ac waveform in volts for the
        voltage source and in amperes for the current source;
        phase is the phase angle of the ac waveform in degrees and
        has a default value of 0.

      DESCRIPTION Supplies a sinusoidal voltage or current at a fixed
      frequency to the circuit.

      EXAMPLES   Vab     3     2    AC    10     90

                 112     4     6    AC    0. 5




      INDEPENDENT TRANSIENT VOLTAGE AND CURRENT SOURCES

      SYNTAX (VOLTAGE)   Vxxx       n+    n-     trans_type

      SYNTAX (VOLTAGE)   lxxx       n+    n-     trans_type
        where trans_type is one of the following transient waveform
        types.
        · Exponential EXP (start peak [delayll [risel [delay2] [fall])
          ＼人／
            ith
         start The initial value of voltage in volts or current in am-
         peres;
         peak The maximum value of voltage in volts or current in
         amperes;
         delay 1 The delay in seconds prior to a change in voltage or
         current from the initial value, which is 0 seconds by default;
         rise The time constant in seconds of the exponential decay
         from start to peak, which has a default value of tstep seconds
         (see . TRA寸);
         de1ay2 The delay in seconds prior to introducing a second
         exponential decay, from the maximum value toward the m1li-
         tial value, which has a default value of delay 1 + tstep sec-
         onds (see . TRAN);
                              QUICK REFERENCE TO PSPICE             117


 fall The time constant in seconds of the exponential decay
 from peak to final, which has a default value of tstep seconds
 (see . TRAN).
1Pulsed PULSE(min     max     [delay]           [rise]    [fall]
              [width]   [period])
 with
 mm1l The minimum value of the waveform in volts for the
 voltage source and in amperes for the current source;
 max The maximum value of the waveform in volts for the
 voltage source and in amperes for the current source;
 delay The time in seconds prior to the onset of the pulse
 train, which has a default of 0 seconds;
 rise The time in seconds for the waveform to transition from
 mm1l to max, which has a default value of tstep seconds (see
 . TRAN);
 fall The time in seconds for the waveform to transition from
 max to mmll, which has a default value of tstep seconds (see
  . ThAN);
  width The time in seconds that the waveform ren' 'ins at the
 max value, which has a default value of tstop seconds (see
  . TRAN);
 period The time in seconds that separates the pulses in the
  pulse train, which has a default of tstop seconds (see
  .TRAN).
1Piecewise linear PWL(tl vall t2 va12 . . .)
   with
  t1 vall A paired time (in seconds) and value (in volts for a
  voltage source and amperes for a current source) that
  specifies a corner of the waveform; all pairs of times and
  values are linearly connected to form the whole waveform.
 ·Damped sinusoid SIN (off    peak            [freq]     [delay]
                       [damp] [phase])
   with
  off The initial value of the voltage in volts or the current in
  amperes;
  peak The maximum amplitude of the voltage in volts or the
  current in amperes;
  freq The sinusoidal frequency in hertz, which has a de包ult
  value of 1/tstop hertz (see . TRAN);
  delay The time in seconds that the waveform stays at the mlli-
  tial value before the sinusoidal oscillation begins, which has
  a default value of 0 seconds;
118    APPENDIX D


          damp The sinusoidal damping factor in seconds이 used to
          specify the decaying exponential envelope for the sinusoid,
          which has a default value of 0 seconds 1;
          phase The initial phase angle of the sinusoidal waveform in
          degrees, which has a default value of 0 degrees.

      DESCRIPTION Supplies a time-varying voltage or current to the
      circuit whose waveform can be characterized as exponential,
      pulsed, piecewise linear, or damped sinusoidal.

      EXAMPLES   Vs 3 1 EXP (2 6 .5 .1 .5 .2)

                 Tin 4 0 PULSE (-.3 .3 0 .01 .01 1 2)

                 15 2 3 PWL (0 .2 1 .6 1. 5 .6 3 -.5)

                 Vg 0 3 SIM (0 2 100 0 0 90)



      DEPENDENT VOLTAGE CONTROLLED VOLTAGE SOURCE

      SYNTAX    Exxx   n+ n- cn+ cn- gain
        where
        cn+ is the positive node for the controlling voltage;
        en- is the negative node for the controlling voltage;
        gain is the ratio of the source voltage (between n+ and n- )
        to the controlling voltage (between cn+ and en- ).

      DESCRIPTION Provides a voltage source whose value depends on
      a voltage measured elsewhere in the circuit.

      EXAMPLE Eop      1    2    4    0     .5



      DEPENDENT CURRENT CONTROLLED CURRENT SOURCE

      SYNTAX Fxxx      n+   n-       Vyyy   gain
        where
       Vyyy is the name of the voltage source through which the
       controlling current flows;
       gain is the ratio of the source current (flowing from n+ to
       n- ) to the controlling current (flowing t뇨ough Vyyy).
                                           QUICK REFERENCE TO PSPICE   119


DESCRIPTION Provides a current source whose value depends on
the magnitude of a current flowing through a voltage source
elsewhere in the circuit.


EXAMPLE   Fdep       3       2   Veontrol             10



VOLTAGE CONTROLLED CURRENT SOURCE

SYNTAX    Gxxx   n+      n-          cn+     cn-      gain
  where
  cn+ is the positive node for the controlling voltage;
  cn- is the negative node for the controlling voltage;
  gain is the ratio of the source current (flowing from n+ to
  n- ) to the controlling voltage (defined between cn+ and
  cn기, in ohms니.


DESCRIPTION Provides a current source whose value depends on
the magnitude of a voltage measured elsewhere in the circuit.


EXAMPLE   Gon    3       6       4     1     0. 35



CURRENT CONTROLLED VOLTAGE SOURCE

SYNTAX    Hxxx   n+      n-           Vyyy     gain
  where

  Vyyy is the name of the voltage source through which the
  controlling current flows;
  gain is the ratio of the source voltage (defined between n+
  and n-) to the controlling current (flowing through Vyyy), in
  야ims.


DESCRIPTION Provides a voltage source whose value depends on
the magnitude of current flowing through another voltage source
elsewhere in the circuit.



EXAMPLE   Hout       7       2       Vdunimy     -2. 5e-3
120    APPENDIX D


      VOLTAGE CONTROLLED SWITCH

      SYNTAX     Sxxx   n+    n-        cn+     cn-   mname
         where
         cn+ is the positive node of the controlling voltage;
        cn- is the negative node of the controlling voltage;
        mname is the name of a VSWITCH model defined in a
        . MODEL statement (see . MODEL).

      DESCRIPTI0N Simulates a switch that is opened or closed, de-
      pending on the magnitude of a voltage measured elsewhere in
      the circuit.

      EXAMPLES    S32    13       12     4     0   smod
                  .MODEL      smod           VSWITCH (RON = 0. 1)


      CURRENT CONTROLLED SWITCH

      SYNTAX     Wxxx   n+     n-        Vyyy      mname
        where
        Vyyy is the name of the voltage source t뇨ough which the
        controlling current flows;
        mname is the name of an ISWITCH model defined in a
        .MODEL statement (see . MODEL).

      DESCRIPTI0N Simulates a switch that is open or closed, depend-
      ing on the magnitude of the current flowing through a voltage
      source located elsewhere in the circuit.

      EXAMPLE    Woff    4    8        Vab     imod
        . MODEL imod ISWITCH (ROFF = le+3, ION = le- 6)


      RESISTOR

      SYNTAX Rxxx       n+    n-       [mname]     value
        where
        mname is the name of a RES model defined in a . MODEL
        statement (see . MODEL)-note that mname is optional;
        value is the resistance, in ohms.
                                      QUICK REFERENCE T0 PSPICE         121


DESCRIPTION Models a resistor, a circuit element whose voltage
and current are linearly dependent.


EXAMPLE Rfor       3       4   16e+3



INDUCTOR

SYNTAX Lxxx      n+    n- [mname] value [IC = icval]
  where
  mname is the name of an IND model defined in a . MODEL
  statement (see . MODEL)-note that mname is optional;
  value is the inductance, in henries;
  icval is the initial value of the current in the inductor, in am-
  peres-note that specifying the initial condition is optional.


DESCRIPTION Models an inductor, a circuit element whose
voltage is linearly dependent on the derivative of its current.


EXAMPLE L44       1    9       3e-3    IC = le-2



CAPACITOR

SYNTAX Cxxx       n+       n- [rnnarne]     value [IC = icvalj

   where
   mname is the name of a CAP model defined in a . MODEL
   statement (see . MODEL)-note that mname is optional;
   value is the capacitance, in farads;
   icval is the initial value of the voltage across the capacitor, in
   volts-note that specifying the initial condition is optional.


 DESCRIPTION Models a capacitor, a circuit element whose cur-
 rent is linearly dependent on the derivative of its voltage.


 EXAMPLES   Ctwo       4       0   cmod   2e-6

            .MODEL         cmod       CAF(C = 1)
122   APPENDIX D


      MUTUAL INDUCTANCE

      SYNTAX    Kxxx   Lyyy    Lzzz     value
        where

        Lyyy is the name of the inductor on the primary side of the
        coil;
        Lzzz is the name of the inductor on the secondary side of the
        coil;
        value is the mutual coupling coefficient, k, which has a value
        such that 0 三三 k < 1.

      DESCRIPTION Models the magnetic coupling between any two
      inductor coils in a circuit.

      EXAMPLE   Kab    La     Lb   0. 5


      SUBCIRCUIT DEFINITION

      SYNTAX    . SUBCKT    name      {nodesl       . EN冶
        where
        name is the name of the subcircuit, as referenced by an X
        statement (see subcircuit call);
        nodes is the optional list of nodes used to identify the connec-
        tions to the subcircuit;
        . ENDS signifies the end of the subcircuit definition.

      DESCRIPTION Used to provide "subroutine"-type definitions of
      portions of a circuit. When the subcircuit is referenced in an X
      statement, the definition between the . SUBCKT statement and
      the . ENDS statement replaces the X statement in the source file.

      EXAMPLE    .SUBCKT       opamp      1     2    3   4   5

                 .ENDS


      SUBCIRCUIT CALL

      SYNTAX    Xxxx   nodes    name
        where
        nodes is the optional list of circuit nodes used to connect the
        subcircuit into the rest of the circuit; there must be as many
                                   QUICK REFERENCE T0 PSPICE          123

  nodes in this list as there are in the subcircuit definition (see
  Subcircuit Definition);
  name is the name of the subcircuit as defined in a . SUBCKT
  statement.

DESCRIPTION Replaces the X statement with the definition of a
subcircuit, which permits a subcircuit to be defined once and
used many times within a given source file.

EXAMPLE Xamp       4   2     8    5   1   opamp

LIBRARY FILE

SYNTAX    . LIB   [f"iame1
  where
  fname is the name of the library file containing . MODEL or
  .SUBCKT statements referenced in the source file, which by
  default is the nominal or evaluation library file.

DESCRIPTION   Used to reference models or subcircuits.

EXAMPLE .LIB       mylib. lib

DEVICE MODELS

SYNTAX . MODEL       mname       mtype [(par = value)]
  where
  mname is a unique model name, which is also used in the
  device statement that incorporates this model;
  mtype is one of the model types available;
 par = value is an optionally specified list of parameters and
 their assigned values, specific to the model type:
 1VSWITCH, which models a voltage-controlled switch and
  has the following parameters:
   RON, the resistance of the closed switch, whose default value
   islf;
   ROFF, the resistance of the open switch, whose default value
   is 1e6 fl;
   VON, the control voltage level necessary to close the switch,
   whose default value is 1 V;
   VOFF, the control voltage level necessary to open the
   switch, whose default value is 0 V;
124   APPENDIX D


        1ISWITCH, which models a current controlled s刃itch and has
          the following parameters:
          RON, the resistance of the closed switch, whose default value
          is1f;
          ROFF, the resistance of the open switch, whose default value
          is 1e6 11;
          ION, the control current necessary to close the switch,
          whose default value is le-3 A;
          1OFF, the control current necessary to open the switch,
          whose default value is 0 A;
        1RES, which models a resistor and has the parameter
             R, the resistance multiplier, whose default value is 1;
        1IND, which models an inductor and has the parameter
             L, the inductance multiplier, whose default value is 1;
        1CAP, which models a capacitor and has the parameter
             C, the capacitance multiplier, whose default value is 1.

      DESCRIPTION Defines standard devices that can be used in a cir-
      cuit and sets parameter values that characterize the specific
      device being modeled.

      EXAMPLES    .MODEL        imodel   IND (L = 2)

                  , MODEL    resist      R且S




      CONTROL STATEMENTS

      DC ANALYSIS

      SYNTAX     . DC [type]     vname   start   end   incre
                 [nest-sweep]
        where
        type is the sweep type and must be U1N for a linear sweep
        from the start value to the end value, OCT for a logarithmic
        sweep from start value to end value in octaves, DEC for a loga-
        rithmic sweep from start value to end value in decades, or
        LIST if a list of values is to be used; the default sweep type is
        LIN;
        vname is the name of the circuit element whose value is
        swept, usually an independent voltage or current source;
        start is the beginning value of vname;
                                   QUICK REFERENCE T0 PSPICE           125


   end is the final value of vname; note that when the sweep type
   is LIST, the start, end, and mnere values are replaced by a list
   of values that vname will take on;
   mnere is the step size for the LIN sweep type and is the number
   of points per octave or decade for the OCT and DEC sweep
   types;
   nest-sweep is an optional additional sweep of a second circuit
   variable, which follows the same syntax as the sweep for the
   first variable.

DESCRIPTION Provides a method for varying one or two dc
source values and analyzing the circuit for each sweep value.

EXAMPLES     . DC Vab 1 10 . 5

             . DC Ii   DEC .1 10 30 Vi DEC 10 100 30

TRANSFER FuNCTION

SYNTAX     . TF   output   input
   where
  output is the output circuit variable, which is a voltage or a
  current;
  input is the source circuit variable, which is a voltage or a cur-
  rent.

DESCRIPTION Computes the gain, input resistance and output re-
sistance between input and output.

EXAMPLE    .T그 V (6, 2) Vsource

SENSITIVITY

SYNTAX . SENS       vname

  Where vname is the circuit variable name (or list of circuit
  variable names) for which sensitivity analysis will be per-
  白rmed.

 DESCRIPTION Computes and prints to the output file a dc sensi-
tivity analysis of vname to the values of other circuit elements,
including resistors, independent voltage and current sources, and
voltage and current controlled switches.

EXAMPLE . SENS V (2) I (yin)
126   APPENDIX D


      TRANSIENT ANALYSIS

      SYNTAX    . TRAN    tstep   tstop [npval] istep    [UIC]
        where
        tstep is the time interval separating values that are printed or
        plotted;
        tstop is the ending time for the transient analysis;
        npval is the time between 0 and the first value printed or plot-
        ted, which by default is 0;
        istep is the internal time step used for computing values,
        which by default is tstop/50;
        UIC will bypass the calculation of the bias point, which usu-
        ally precedes the transient analysis, and use the initial condi-
        tions specified by IC = in inductor and capacitor data state-
        ments instead.

      DESCRIPTION Performs a transient analysis of the circuit de-
      scribed in the source file to calculate the values of circuit vani-
      ables as a function of time.

      EXAMPLE    . TRAN . 01 10 0 . 001 UIC

      INITIAL CONDITION

      SYNTAX . IC        Vnode = value
        where
        Vnode = value is one or a list of pairs consisting of a voltage
        node Vnode, represented in standard form, and the initial
        value in volts at that node.

      DESCRIPTION Sets the initial conditions for transient analysis by
      specifying one or more node voltage values.

      EXAMPLE .IC V(1) = 10 V(3,4) = -2

      AC ANALYSIS

      SYNTAX    . AC [type] num        start end
        where
        type is the type of sweep, which must be one of the following
        keywords:
           LIN for a linear sweep in frequency, which is the default;
                                  QUICK REFERENCE T0 PSPICE            127


    OCT for a logarithmic sweep in frequency by octaves;
    DEC for a logarithmic sweep in frequency by decades;
  num is the total number of points in the sweep for a linear
  sweep and the number of p아nts per octave or decade for a log-
  arit노llic sweep;
  start is the starting frequency, in hertz;
  end is the final frequency, in hertz.


D E SCRIPT ION Computes the frequency response of the circuit de-
scribed in the source file as the frequency is swept either linearly
or logarithmically from an initial value to a final value.


EXAMPLE   .AC      U1N   300     10    1000



STEPPED VALUES

SYNTAX    . STEP    [type]   name     start    end   mllere
  where
  type is one of the following keywords describing the type of
  parameter variation:


    LIN for a linear variation, which is the default;
     OCT for a logarithmic variation by octaves;
    DEC for a logarithmic variation by decades;
  name is the name of the circuit element whose value is to be
  varied;

  start is the starting value for the circuit element, in units ap-
  propriate to the type of circuit element;

  end is the final value for the circuit element, in units appropri-
  ate to the type of circuit element;

  incre is the step size for a linear variation and the number of
  values per octave or decade for the logarithmic variation. Note
  that when a discrete list of parameter values is desired, type is
  not used and the name is followed by the keyword LI ST and
  a list of parameter values.


DESCRIPTION Used to step a circuit element's value t뇨ough a
range either linearly or logarithmically or through a discrete list,
analyzing the circuit for each value.
128    APPENDIX D


      EXAMPLES     . STEP    DEC    RES     RMOD (H)       10    10e4   3

                   .STEP      V2   LIST     1     4   12    19


      FOURIER SERIES ANALYSIS

      SYNTAX     . FOUR     freq   vname
        ＼人／
          here
        freq is the fundamental frequency of the circuit;
        vname is the variable name or the list of variable names for
        which Fourier Series coefficients will be computed.

      DESCRIPTION Uses the results of a transient analysis to compute
      the Fourier coefficients for the first nine harmonics. Note the
      .FOUR statement requires a . THA寸 statement to perform the
      transient analysis.

      EXAMPLE     . FOUR    10e3    V (3)       V (6, 2)




      OUTPUT STATEMENTS

      OPERATING POINT

      SYNTAX     . OP

      DESCRIPTION Outputs information describing the bias point
      computations for the circuit being simulated.

      EXAMPLE    . OP


      PRINT RESULTS

      SYNTAX     . PRINT    type   vname
        where
        type identifies the type of analysis performed to generate the
        data being printed and must be one of the keywords DC, AC,
        or TRAN;
                                 QUICK REFERENCE TO PSPICE            l29


  vname is the variable name or the list of variable names for
  which values are to be printed.

DESCRIPTION Prints the results of circuit analysis in table form
to an output file for each program variable specified.

EXAMPLE    .PRI寸T      AC   V (3, 2)     I (Vsource)


Pioi RESULTS

SYNTAX     . PLOT    type   vname      11Ow]   thigh]

  where
  type identifies the type of analysis used to produce the values
  being plotted and must be one of the keywords DC, AC, or
  TRAN;
  vname is the variable name or the list of variable names for
  which values are to be plotted;
  low and high optionally sets the range of values of the mde-
  pendent variable to be plotted, which defaults to the entire
  range of values.

DESCRIPTION Generates line-printer plots of circuit variables
computed during dc, ac, or transient analysis.

 EXAMPLE    .PLOT TRANS I (Vin) V (4)




 PROBE
 SYNTAX    . PROBE    [vname]
   Where vname is the optionally specified variable or list of
 variables whose values from dc, ac, and transient analysis will be
 stored in the file that PROBE uses to generate plots, If no vani-
 able name is included, values of all circuit variables will be
 stored in the PROBE file.

 DESCRIPTION Generates a file of data from dc, ac, and transient
 analysis used by PROBE to generate high-quality plots.

 EXAMPLE    .PROBE V (2) V (3) V (4) I (Rin) I (Rout)
130   APPENDIX D


      MISCELLANEOUS STATEMENTS
      TITLE LINE

      DESCRIPTION Each source file must have a title line as its first
      line.

      EXAMPLE A Circuit to Simulate RLC
              *Frequency Response

      END STATEMENT

      SYNTAX .END

      DESCRIPTION Each source file must have an . END statement as
      its final line.

      EXAMPLE . END

      PRINTING CONTROL

      SYNTAX .WIDTH        OUT = value
        where

        value is used to specify the number of columns used in print-
        ing the output file, which must be either 80 (the default) or
        132.

      DESCRIPTION Used to change the number of columns in the out-
      put file from the default.

      EXAMPLE   . WIDTH    OUT = 132

      SIMULATION OPTIONS

      SYNTAX . OPTIONS       oname    [oname = value]
        where
        oname is the name or the list of names of option flags to be
        set;
        oname = value is the name and assigned value or the list of
        names and their values for options requiring values.

      DESCRIPTION Used to override the default specifications of many
      parameters used to control circuit simulation.

      EXAMPLE   . OPTION     NOPAGE      NONODE    RELTOL = . 1
                                                                                                                       131




PROBI.EMS

1. Use PSpice to find the voltages V(2,0), V(3,0),                            VDELTA
   and V(4,O) in the circuit shown in Fig. P.1.




                                                                                                      HS01

                                                        디GURE P.1



2. a) Use the output from PSpice simulation of the                  d) Verify that the power dissipated equals the
      circuit in Problem 1 to calculate the power                      power supplied.
      dissipated in each resistor in Fig. P. 1.
                                                                    e) What is the total power dissipated value out-
   b) Find the total power supplied by the indepen-                    put from the PSpice analysis?
      dent voltage source.
                                                                    f) How does the value in (e) compare to the pre-
   c) Find the total p叭Ver supplied by the current                     vious power computations?
      controlled voltage source.




3. Return to Fig. P.1 and replace the current con-                  compare the output with that obtained in Prob-
   trolled voltage source with an independent                       lem 1. In particular, compare the total power
   voltage source of 132 V, positive at the reference               dissipated values from each simulation.
   node. Use PSpice to simulate this circuit and
132                                                     PROBLEMS



 4. Use PSpice to find the voltages v口, Vb, and v, in                                                     /?]= 0.2O

    the circuit shown in Fig. P.4. Use the . DC con-
    trot statement so that these voltages can be                                                                                5 ／了, = 9.4O
                                                                                           120V
    specified directly in a . PRINT statement.                                                                          r   a




                                                                                                                                               V, 3凡＝11.211
                                                                                                                           <
                                                                                           120V                                      = 19.4O
                                                                                                                        Vb <

                                                                                                          /?3= 0.211


                                                           FIGURE P.4



 5. Use PSpice to find the Thevenin equivalent with                                                            3.514,

    respect to the terminals of the variable resistor
    RO in the circuit shown in Fig. P.5.
                                                                                                  4011

                                                                                                  1니卜    ／巾


                                                                                160V                              :80O




                                                           FIGURE P.5



  6. a) Label the terminals of the 10-fl resistor in the                                                                    ] ]/b
                                                                                                                                          1니卜    /e

        circuit shown in Fig. P.6 as a and b. Let a be
        the terminal at the top of the resistor. Now
        remove the 10-fl resistor and use PSpice to
        find the Th6venin equivalent of the remaining
        circuit with respect to terminals a, b.
      b) Use the Thevenin equivalent obtained in (a)                    2.7 A                                                                              135V

         to find the current in the 10-fl resistor.

                                                           디GURE P.6



  7. Use PSpice to find the Thdvenin equivalent with                                                    40／中

     respect to terminals a, b for the circuit shown in                            a

     Fig. P.7. Hint: Introduce a very small current                                                                                                            小
                                                                                                                                                       跏
     source in parallel with the 60-fl resistor to simu-                               .            +               2011                              60lTl1

     late no independent source in the original circuit.

                                                           디GURE P.7
                                                           PROBLEMS                                            133



                                                                                         30 n
 8. Assume that the resistors in the ciruit shown in
    Fig. P.8 can vary by 士2% and that the voltage
    of the ideal voltage source can vary by 士5%.                        40 V
    Use PSpice to predict the minimum and maxi-
    mum values of v。  .
                                                          FIGURE P.8


9. The op amp in the noninverting amplifier circuit                                             80 ki

   shown in Fig. P.9 has an input resistance of
   40 kfl, an output resistance of 1 kfl, and an
   open-loop gain of 10.
    a) Use PSpice to find the value of v, and i g if
       v8 = I V(dc).                                                                                           10 ka

    b) Compare the PSpice solution with the ana-
       lytic solution for v。and i4.

                                                          FIGURE P.9


10. The two op amps in the circuit shown in Fig.                               175 kfl

    P.10 are identical. Their parameter values are
    R1= 500kfLR。= 100f, andA= 104.
    a) Use PSpice to find v,i and v。
                                   2 when V4 =
       0.6 V(dc).
    b) Calculate v。 1 and l石3 if the amps are assumed                                                           5 k{I
       ideal. Are these values of v7i and v。 2 consis-
       tent with the output from the PSpice simula-
       tion in (a)?
    c) Now use the model of the 杉 A741C opera-
       tional amplifier found in the evaluation library
       to represent the op amps in Fig. P.10 and re-
       run the PSpice simulation. How do these re-
       sults compare with those obtained in (a) and
       (b)?
                                                          FIGURE P.10


11. An exponential voltage pulse is described by
           V4 =i2. 5V,     0 5t 51s;
                                     '
           V4 = 12.5 + 12.5(1 - e0 ' ')) V,
                is 드 t 드 11 s;
           V4 = 12.5 + 12.5(1 小
                - 12.5(1 - eO"l25(t山）) V,
                ii 5 드 t 5 31 5.                                                                        (continued)
134                                                     PROBLEMS


      These voltages are applied to the circuit shown                                                 20O

      in Fig. P.11.
      a) Use PSpice and PROBE to obtain a plot of
         仇（t) 如rO 드 t 5 31 s at increments of 200
         ms.
      b) Use the output from PSpice analysis to check     FIGURE P.11
         the validity of the analytic solution.




12. An exponential voltage source is described by
                                                                        a) Apply this pulse to the circuit shown in Fig.
      Vg = 10V,     0 드 t 드 1 s;                                           P.11 and use PSpice and PROBE to obtain a
      Vg = 10 + 30(1 - e_0.12升l)) y,                                       plot of vO(t) for 0 5 t 5 20s in increments of
           is 드 t 드 3 s;                                                   0.1 5.
      Vg = 10 + 30(1 - e0 '25(' ') - 30(1 - e ' 3)                      b) Use the data from the PSpice simulation to
                                                   )                       verify the validity of the analytic solution.
           V,    3s 5t 5 20s.




13. The exponential pulse from Problem 12 is ap-                                                               5O
    plied to the circuit shown in Fig. P.13.
    a) Use PSpice and PROBE to obtain plots iO and                                                                          1H
        vO for 0 5 t 5 10 s.
      b) Do the plots obtained in (a) make sense in
         terms of known circuit behavior? Explain.
                                                         디GURE P.13


14. Use PSpice and PROBE to plot i versus t for the
    circuit shown in Fig. P.14 when 4 = 50mA,
    VO= -10V, L= 10mH, R= 200f1, and
    C = 1 肛F. Use an analytic solution for i (r) to
    check the results displayed in the PROBE plot.
                                                         FIGURE P.14



15. a) In the circuit shown in Fig. P.15, V, = 0 and
       1J = -12.25 mA. The circuit element values
       areR = 20kfI, L = 8H, andC = 0.125 尸F.
       Use PSpice and PROBE to plot v (t) versus t
       for the time interval 0 5 t 5 11 ms.
    b) Use PROBE to identify the maximum value of
       v (t), the time at which the maximum value
       occurs, and the value of the damped period.
                                                         디GURE P.15
                                                                  PROBLEMS                                                          135



16. a) Use PSpice and PROBE to plot v (t) versus t                          b) Discuss the significance of removing the re-
       for the circuit shown in Fig. P.15 when the                             sistor from the circuit.
       20 kfl resistor is removed from the circuit.



17. a) For the circuit shown in Fig. P.15, find the                         c) Use PROBE to check the maximum value of
       value of R that will result in a critically                             v (t) and the time at which it occurs.
       damped voltage response.
    b) Use PSpice and PROBE to plot v (t) versus t
       凡rO 드 t 드 7 ms.




                                                             1
18. The switch in the circuit shown in Fig. P.18 has                                      40／스

    been closed for a long time. At t = 0 it is                                            V
    opened. Use PSpice and PROBE to plot 屯(t) ver-
    sus t for t > 0. In the transient analysis, let tstop
                                                                            H
                                                             >>                  >20fl
    equal five time constants and select tstep to give
    100 points between 0 and tstop.

                                                              FIGURE P.18



19. The 360-V. 3.6-fl source in the circuit shown in                                             3.6fl
                                                                                                 人 八 /\
    Fig. P.19 is inadvertently short-circuited at its

                                                                                                                   > \ ] 누>>노
                                                                                                                            11
    terminals a, b. At the time the fault occurs, the                                                           4 !)               6I

    circuit is in a steady-state operating condition.
                                                                                     )
                                                                                                                 /
                                                                                                                 <
     a) Use PSpice and PROBE to obtain a plot of the                                                          20 mH              15 mH
        short-circuit current for t 之 0. Make a pre-
                                                                              36나
        liminary analysis of the circuit to facilitate the                                                b
        choice of tstop and tstep.
    b) From the PSpice simulation and the PROBE
       plot, estimate at what time the short-circuit
       current equals 76 A.
                                                              디GURE P.19



20. The initial voltage on the capacitor in the circuit                                                          200 kIi

    shown in Fig. P.20 is 100 V. Use PSpice simula-
    tion and PROBE to obtain a plot of vc and v中 for
    r >0.

                                                                                  100 V                                            50 k62




                                                              FIGURE P.20
136                                                        PROBLEMS



21. a) The 0.1 p.F capacitor in the circuit shown in                                                   t= o
       Fig. P.21 is charged to 100 V. At t = 0 the
       capacitor is discharged through a series corn-
       bination of a 100-mH inductor and a 560-fl
       resistor. Use PSpice and PROBE to plot i (t)
       and Vc(t).
      b) Use PROBE to confirm the analytic solutions
         for this circuit. In particular, check the peak
         values, time of occurrence, and damped pe-
         niod.
                                                             FIGURE P.21



22. a) No energy is stored in the 100-mH inductor
       or the 0.4-SF capacitor when the switch in
       the circuit shown in Fig. P.22 is closed. Use                       48 V
       PSpice and PROBE to plot Vc(t) versus t.
      b) Use PROBE to confirm the analytic solution
         的r Vc(t).
                                                             FIGURE P.22



23. The switch in the circuit shown in Fig. P.23 has                                       (   =   o

    been closed for a long time before opening at
    r = 0.
      a) Calculate the damped period of the voltage
         vO(t).
      b) Use PSpice and PROBE to obtain a plot of
         vO(t) over the interval 0 5 t 5 1.5T.
      c) Use PROBE to determine the maximum mag-
         nitude of vO(t) and the time at which it oc-
         curs.
                                                             디GURE P.23




24. No energy is stored in the circuit shown in Fig.
                                                                                  d갸
    P.24 at the instant the dc current source jumps                                            H
                                                                                               2
                                                                                                              65ft
    from 0 to 8 A.                                                                     戶 卜 >
                                                                                                                     h.
      a) Use PSpice and PROBE to plot L(t) versus t                                    1                                  130 '
         的rt 之 0.
                                                                                                                     T
      b) Use PROBE to determine the peak value of
         瓦(t) and the instant at which it occurs.
                                                             FIGURE P.24
                                                            PROBLEMS                                                                            137



25. a) No energy is stored in the circuit shown in                                                         4n

       Fig. P.25 at the time the sources are ener-
       gized. Use PSpice and PROBE to plot v2 ver-
       sus t.
    b) Use PROBE to find v2(0), v2(叫, and
       dv2(0)/dt.                                                         3u(f) A                                                            15u(t) V




                                                          디GURE P.25



26. a) The initial energy in the circuit shown in Fig.                                                          0.25v小

       P.26 is zero. Use PSpice and PROBE to plot
       i (t).
    b) Use PROBE to determine i (0), i (a)), and the
       damped period.
                                                                                                                                               140fl




                                                          FIGURE P.26



27. a) No energy is stored in the circuit shown in                                                              20／小

       Fig. P.27 when the current source jumps to
       100 A. Use PSpice and PROBE to plot i (t).
    b) Use PROBE to determine i (0) and i (叫.


                                                                                    5n




                                                          FIGURE P.27



28. a) Use PSpice to simulate the source file listed in                                  7.5 k{)                         2 k{2

       Example 10 for the circuit shown in Fig.
       P.28.
                                                                        soy                        30 kC                         v,(f)
                                                                                                                                 .,      1      5. F
    b) Derive the analytic expression for vO(t) in the
       circuit of Example 10.
    c) Compare the output from the PSpice simula-
       tion to results predicted by the analytic solu-
       tion. For example, compare the results at
       t = 0, 40, and80msandatQc.
                                                          FIGURE P.28
138                                                      PROBLEMS



29. The following parameters pertain to the circuit                        a) Use PSpice and PROBE to generate a plot of
     shown in Fig. P.29: R = 1 kfl, R1 = 400 kfl,                             VB(t) and Vc(t) versus t. Use the analytic so-
    R2 = 100 kfl, R3 = 20 kf), R4 = 5 k(E                                     lution to guide the choice of tstep and tstop.
    l?5 = 50 kfI, R6 = 0.5 ku, R7 = 44J0fl,                                b) Use PROBE to find the maximum value of
    R8 = 50 kfl, C1 = 5 尸F, and C2 = 5 p.F. As-                               Vc(t) and the time at which it occurs.
     sume thatf (t) is a dc voltage that switches from
    0 to 4.04 V at t = 0. At the time the source is                        c) Compare the results of (b) to the analytic so-
    switched on, no energy is stored in the capacitors                        lution 如r vc(m口工） and t (ma工）.
    C1 and C2. The operational amplifiers are as-
    sumed to be ideal.




                                                                       3




                                                                5




                                                                b




                                                          디GURE P.29



30. a) Set the initial voltages on the capacitors Ci                       c) Use PROBE to check on whether vc(O),
       and C2 in the circuit of Problem 29 so that                            dvc(0)/dt, and VC( ) are satisfied.
       vc(0) = -5 V and dvc(0)/dt = io v/s.                                d) Use the ou印ut from PSpice and PROBE to es-
      b) Use PSpice and PROBE to obtain a plot of Vc                          timate Td and check it against the calculated
         and VB with the initial conditions from (a).                         value.
                                                            PROBLEMS                     139



31. Replace two of the ideal op amps in Problem 29
    with the 尸A741C op-amp model from the nomi-
    nal library. Use PSpice and PROBE to plot Vc(t)
    versus t and compare your results to those in
    Problems 29 and 30.


                                                                         500k11
32. The op amps in the circuit shown in Fig. P.32
    are ideal. At the instant the voltage source jumps
    from 0 to 250 mY no energy is stored in the ca-
    pacitors.
     a) Use PSpice and PROBE to plot vl and v。
                                             2 for
        0 三； t 드 0.5 s.
    b) Compare the results to the analytic solution
       for v。
            1 and v。2 at t = 0, 0.10, 0.20, 0.30,                                         5 ktl
       0.40, and 0.50 s.

                                                           디GIJRE P.32



33. Use PSpice together with PROBE to plot the
    transient response of vc in the circuit shown in
    Fig. P.33 from 300 to 1800 尸s in steps of 25 ps.
    Use a 5-,as increment for calculating the tran-
    sient response.

                                                           디GURE P.33



34. Use the . STEP statement in a PSpice source file
    to increase the size of the capacitor in the circuit
    shown in Fig. P.23 from 0.25 杉F to 12.5 pF in
    steps of 0.5 杉F. Use PROBE to find the maxi-
    mum amplitude of v。   (t) and the time at which it
    occurs as the capacitor value changes.



35. a) For the damped sinusoidal voltage
        Vg = 12.5 + 25e_Ol(t_ Dsin [0.47r (t - 1)] V
       calculate the maximum value of Vg, time at
       which the maximum occurs, damped period,
       delay time, and offset voltage.
    b) Use this sinusoid as the input to the circuit
       shown in Fig. P.35 and use PSpice to simu-
       late this circuit.
                                                           FIGURE P.35            (continued)
140                                                       PROBLEMS


  c) From the output of PSpice simulation, tabu-                         d) Compare the calculated values from (a) to the
     late the maximum value of vg, time at which                            output from PSpice simulation in (c).
     the maximum occurs, damped period, delay
     time, and offset voltage.




36. Assume that the damped sinusoidal source de-                                                           10 11

    scription in Problem 35 is applied to the circuit
    shown in Fig. P.36. At the time vg is energized,
    the initial charge on the capacitor is zero.
      a) Use PSpice and PROBE to plot vO(t) versus r.
      b) Does the plot obtained in (a) make sense in
         terms of known circuit behavior?
                                                           디GURE P.36



37. The sinusoidal voltage source in the circuit                                                      73011
                                                                                                       八人                  !                          WV
    shown in Fig. P.37 is generating a voltage of                                                                                                +         +
    6 cos 104irt V.
      a) Use PSpice to find the amplitude and phase
                                                                                                              5.
                                                                                                                                                 V0        V1

         angle of v0, v1, v2, and i o.                                                      ),
                                                                                                                                                                     18mH
      b) Test the results obtained in (a) by showing
                                                                                                         0.01 '    F                "
         that they are consistent with the conservation
                                                                                                                       T
         of energy principle-namely, that the average
         power delivered equals the average power ab-
         sorbed.
                                                           디GURE P.37




38. The phasor-domain circuit shown in Fig. P.38 is                                         0.0511     尼0511

    based on a frequency of 60 Hz.
      a) Use PSpice to find the amplitude and phase
                                                                                                                               V.
         angle of V1, V2, and V3.
                                                                                                                                        穹7211
                                                                                            0.06 11    尼0611
      b) Repeat (a) with the impedance of the neutral                                                                                                           V3
                                                                                                                                                                     <
                                                                                                                                                                     <   811
                                                                                                                                                                     <
         conductor first increased by a fiuctor of 100
         (that is, Z = 6 + j6 f) and then increased                                                                            V,
         by a factor of 1000 (that is, Z = 60 +
                                                                                                                                        穹72011
                                                                                            0.0511     厄0511
         j60fl).
      c) Describe the adverse effect on the operation
         of the circuit when the impedance of the neu-
         tral conductor is increased.
                                                           FIGURE P.38
                                                          PROBLEMS                                                             141



39. The phasor-domam circuit shown in Fig. P.39 is                                                         01829 U

    based on a frequency of 5000 rad/s. Use PSpice
    to find the magnitude and phase angle of I and
    IiifVg= 40+ j30V.                                                                                                  八6463 U




                                                                                                                       /1 fl




                                                        FIGURE P.39




40. An electrical load operates at 240 V(rms) with a                  c) Simulate the circuit using the source file from
    frequency of 60 Hz. The load absorbs an average                      (b). Then use PROBE to generate plots of the
    power of 8 kW at a lagging power factor of 0.8.                      instantaneous power, average power, reactive
    a) Calculate the reactive power of the load and                      power, and complex power.
       the complex power of the load.                                 d) How do the PROBE results compare to the
    b) Calculate the impedance of the load and use                       analysis   in   (a)   ?
       this impedance to construct a PSpice source
       file.




41. a) For the circuit shown in Fig. P.41, use
       PSpice to find the value of capacitance that
       results in transfer of the maximum average
                                                                              10／르
       power to the load. Assume that the load resis-                        V (rm引
       tance is 4000 fi and that the source frequency                                                                          /XC

       is 60 Hz.
    b) For the capacitor value determined in (a), use
       PROBE to compute the average power tram-
       ferred to the load. Does this agree with the
       analytic result?
                                                        FIGURE P.41




42. For the circuit shown in Fig. P.41, assume that                   determine the value of load resistance and load
    the load resistance can vary from 0 to 4000 fl                    capacitance that transfers the most average power
    and that the load capacitive reactance can vary                   to the load. Assume that the source operates at a
    from 0 to -2000 fI. Use PSpice and PROBE to                       frequency of 60 Hz.
142                                                       PROBLEMS



43. The sinusoidal voltage source in the circuit
    shown in Fig. P.43 is described by the equation
                                                                                                                       1
    Vg '= 202 cos 75000t V. Use PSpice to find the
    amplitude and phase angle of iO.                                                                                  16 mH
                                                                                                                                  3900
                                                                                                                                           1



                                                           FIGURE P.43



44. Use PSpice to find the amplitude and phase angle                                                1    4H
    of i in the circuit shown in Fig. P.44 when
    Vg = 100 cos 2 V.


                                                                                                                                         20fl




                                                           FIGURE P.44


45. a) Use PSpice to find the rms magnitude and the                      loft   7.5 mH   15fl
                                                                                                75 mH
       phase angle of i1 and i2 in the circuit shown in
       Fig. P.45. The sinusoidal voltage source is
                                                                                                1
                                                                                                    '   \         S    ＋니卜 /2


                                                                                                              3H           4kfl
       operating at a frequency of 1600 md/s and has
       an rms value of 150 V.
    b) Test the PSpice simulation results by using
       them to determine whether average power
       generated equals average power dissipated.
                                                           디GURE P.45



46. The coefficient of coupling k in the circuit shown                          300 ft

    in Fig. P.46 is varied from 0.3 to 1.0 in steps of                                                        S
    0.1.
                                                                                                                  mR              >900 !1
                                                                                                                                  >
      a) Use PSpice to construct a table that shows
                                                                                                        ;16
         how the magnitude of i1 varies with k when
         V9 = 100 CO5 75000t V.
      b) Analytically solve for the value of k that
         yields the maximum magnitude of ii. Call this
         value kmax.
      c) Use PROBE to predict the value of kmaX from
         the simulation and compare that with the
         value from the analysis.
                                                          디GURE P.46
                                                           PROBLEMS                                          143



47. a) Use PSpice to find the magnitude and phase                                    24 n

       angle of vO in the circuit shown in Fig. P.47
       i f l)g = 500 cos 1000wt V.
    b) Compare the results of PSpice simulation to
                                                                                                            iooc
       the analytic solution for vO.




                                                         FIGURE P.47




48. a) Use PSpice to find the magnitude and phase                      4fl   O.8mH

       angle of vO in the circuit shown in Fig. P.48                                                .
       if v9 = 456 cos 5000t V, N1 = 1000 turns,
       and N2 = 500 turns.                                                                  Ideal

    b) Compare the PSpice simulation results to the                                                     T   "" " "
       analytic solution for vO.
                                                         디GURE P.48



49. a) Use PSpice and PROBE to plot the amplitude
       of vO versus frequency for the circuit shown in
       Fig. P.49.
    b) Use PROBE to estimate the resonant fre-
       quency, bandwidth, and quality factor of the
       circuit.
    c) Compare the results obtained in (b) to calcu-
       lated values of fO, 夙 and Q.
                                                         디GURE P.49



50. a) The current source in the parallel resonant
       circuit shown in Fig. P.50 is ig =
       4 cos wt mA. Calculate the unity power factor
       resonant frequency (fO), the frequency at
       which vD is maximum (f, ), the value of vO at
       f, and the value of vO atf, .
    b) Use PROBE to plot the amplitude of vO
       versus f.
    c) Compare the results of PSpice simulation to
       the results from (a).
                                                         FIGURE P.50
144                                                       PROBLEMS



51. The sinusoidal voltage source (vi) in the circuit
    shown in Fig. P.51 has a peak amplitude of
    10 V. Use PSpice and PROBE to identify (a) the
    unity power factor resonant frequency; (b) the
    magnitude of vO at unity power 拓ctor resonance;
    (c) the maximum magnitude of vO; and (d) the
    frequency at which the maximum magnitude oc-
    curs.

                                                           디GURE P.51




52. The circuit parameters shown in Fig. P.51 are                       e) Calculate the magnitude of v, in decibels at
    changed to the following values: R1 = 2 ktL                             the frequency found in (d).
    L = 20 m}1, R2 = 200 kfTl, C = 250/21 pF,
                                                                        f) Use PSpice and PROBE to construct a plot of
    and R3 = 8 kfl. At the same time the peak
                                                                            vO in decibels versus log f. Start the plot at
    amplitude of Vg is changed to 100 mY.
                                                                           fm/1000 and stop the plot at l0f,,,. Overlay a
    a) Derive the transfer function VO/ V.                                  straight-line Bode magnitude plot on a hard
      b) Calculate the unity power factor resonant fre-                     copy of the PROBE plot and compare.
         quency兀                                                        g) Use the PROBE cursor to identify the values
      c) Calculate the magnitude of vO in decibels at                      calculated in (b)-(d). How do the simulation
         the frequency found in (b).                                       results compare to the analytic results?
      d) Calculate the frequency (fm) at which the
         magnitude of vO is maximum.




53. In the circuit shown in Fig. P.53 the sinusoidal                                   10 kfl
    voltage source is generating the voltage Vg =
    100 cos 64500t V. The variable capacitor is
    varied from 5.72 nF to 9.72 nF in steps of 1 nF.
    Use the . STEP statement in PSpice to simulate
    this circuit and PROBE to plot the steady-state
    magnitude of vO versus C for the stepped values
    of C.
                                                           디GURE P.53




54. For the circuit shown in Fig. P.53, use PSpice to                   to graph the results in Bode plot form: That is,
    simulate the frequency response characteristics of                  plot the magnitude of vO in decibels versus log f.
    the circuit. Continue to use the . STEP state-                      Overlay a straight-line Bode magnitude plot using
    ment to vary the capacitance but now let the fre-                   the PROBE label menu and com妃nt on its accu-
    quency vary from 100 Hz to 106 Hz. Use PROBE                        racy.
                                                          PROBLEMS                                   145




55. a) For the circuit shown in Fig. P.55, derive the
       transfer function V。/Ig.
    b) Use PSpice and PROBE to produce a Bode-
       type frequency plot, including both the mag-
       nitude of vO in decibels and the phase angle of
       vO in de얍ees versus logf. Be sure to choose a
       range of decades for the PSpice simulation
       that includes the frequencies where the mag-
       nitude and phase angle change.
    c)
       Overlay the straight-line Bode approximations
       on both the magnitude and the phase angle
       plots produced by PROBE. How close are the
       Bode plots to the actual plots? For what range
       of frequencies are the two plots most differ-
       ent?
                                                         디GURE P.55


                                                                                            R1
56. The circuit shown in Fig. P.56 has a voltage
    source of constant magnitude and phase angle
    but variable fre꾸lency. Use PSpice and PROBE                           VS= Vm COS cof

    to create a family of Bode-type frequency re-
    sponse plots of the magnitude of vO in decibels
    and the phase angle of vO in degrees versus log!
    as R is varied over the range 0 fI to 106 ft
    Choose about six values for R within that range.
    Then overlay the Bode straight-line magnitude
    and phase angle plots on those produced by
    PROBE. For what value of 凡 does the Bode plot
    vary the least from the actual plot? For what
    value of R does the Bode plot vary the most
    from the actual plot?
                                                         FIGURE P.56




                                                                       4
57. a) Derive the analytic solution for the circuit
       shown in Fig. P.57, where i g = 7 b(t).

                                                                                                 I
                                                                            50!
    b) From the analytic solution, find the minimum
       value of vO(t), the time at which the minimum
       occurs, and the damped period.
    c)
       Use PSpice to simulate this same circuit.
    d) Use PROBE to plot vO(t) versus t and deter-
       mine from the plot the values from (b). How
       do the simulated values compare to the ana-
       lytic values?
                                                         FIGURE P.57
146                                                        PROBLEMS



58. The voltage source V5 in the circuit shown in                                                  v9 CV)
    Fig. P.58(a) is generating the signal shown in
    Fig. P.58(b).                                                               500 ku)                  400

      a) Derive the expressions for v。  (t) for the time
         intervals t <0, 0 드 t 5 0.5 s,
         0.5 s 5 t 드 1.0 s, and t 之 1.0 s.                                                                 0   0.5   1.0      r（引

      b) Use PSpice and PROBE to obtain a plot of
                                                                                                        -400
         v。 (t) versus t. Simulate the voltage source
         with a pulse.
      c) Compare the results from the simulation with
         those predicted by the analytic expressions.
                                                            디GURI P.58




59. The current source i in the circuit shown in Fig.                                             勺 (mA)
    P.59(a) has the waveform shown in Fig. P.59(b).
      a) Use PSpice and PROBE to plot i。
                                       (t) versus t
         for 0 드 t 드 1000 杉S.
      b) Derive the analytic expressions for i。
                                              (t) for                                     2.5 H
                                                                                                          0    350   750    f (Hs)
         t 之 0.
      c) Use the results from PSpice simulation to                                                      -24
         check the results predicted by the analysis in
         (b)   .
                                                                          (a)                     (b)


                                                            디GURE P.59




60. The circuit shown in Fig. P.60 has been in oper-                                                                 8 kn
    ation a long time. At t = 0, the voltage drops
    instantaneously to 12.5 V and the current source
    reverses direction.
                                                                                                                             5 FL F
      a) Use PSpice and PROBE to obtain a plot of
         仇（t) versus t for 0 5 t 드 500 n哈．
      b) From the PROBE plot, note the time at which
         vO(t) is zero.
      c) Check the result in (b) with the analytic solu-
         tion for v。
                   (t) = 0.
                                                             디GURE P.60
                                                                  PROBLEMS                                                          147



61. There is no charge on the capacitor when the           v9 (mV) .

    voltage pulse shown in Fig. P.61(a) is applied to              50
    the ideal integrating amplifier circuit shown in
    Fig. P.60.
    a) Use PSpice and PROBE to obtain a plot of
                                                                    0
       vO(t) versus t over the time interval 0 to 3 s.                  1         2   f(s)

    b) Using the PROBE cursor, read off the values
       of vO at 0, 0.5, 1.0, 1.5, 2.0, 2.5, and 3 s.              -50
    c) Compare the simulation results to the analytic
       solution for vO.
                                                            (a)
                                                                                             (b)

                                                          디GURE P.61



62. Repeat Problem 61 with the feedback capacitor
    paralleled by a 5-Mfl resistor. What is the effect
    of the parallel resistor?



63. Assume that the ideal operational amplifier in the                  b) Compare the output to the ideal operational
    circuit shown in Fig. P.61(b) is replaced by an                        amplifier circuit simulation, considering espe-
    op amp that has an output resistance of 75 (1, an                      cially the solution at 0, 0.5, 1.0, 1.5, 2.0,
    input resistance of 2 Mu, and an open-loop gain                        2.5, and 3 5.
    of i05.
    a) Use PSpice and PROBE to plot the output
       voltage in the interval 0 5 t 5 3 s.



64. The signal voltage in the circuit shown in Fig.                     b) Compare the results of the PSpice simulation
    P.64(a) is the periodic square wave shown in                           of v,1 to the analytic solution for vO1.
    Fig. P.64(b).
    a) Assume that vO1(0) = 4 V and use PSpice and
       PROBE to obtain a plot for the interval
       0 5 t 5 1.6 s.                                                                                                        etc.




                            500 kti

                                                                                                         2.4       3.2              r佃）




                 (a)
                                                                            (b)

                                                         FIGURE P.64
148                                                          PROBLEMS



65. The input signal in the circuit shown in Fig.                                                                  4 1L F

    P.65 is the periodic square wave shown in Fig.                                              IF-
                                                                                                 2 F
                                                                                               - 4V +
                                                                                                                   1(
    P.64(b).
                                                                                 500 k1l   느    5V
      a) Assume that v。1(0) = 4 V and v。
                                       2(0) = 0 V.                                                                 5V
         Use PSpice and PROBE to obtain a plot of v。
         and t拓2 的r0 드 t 드 1.8 s.
                                                   1
                                                                                                                   1
                                                                                                                      5V         10k12
      b) Compare the PSpice simulation for v。
                                            2 to the
         analytic solution for v。
                                2.

                                                              FIGURE P.65


66. a) Compute the expressions for the Fourier Se-                             waveform and the output voltage. How do the
       ries coefficients of the periodic waveform                              analytic results compare to the PSpice out-
       shown in Fig. P.64(b).                                                  puts?
      b) Compute the expressions for the Fourier Se-                        d) Use PROBE to plot vg and v。  1 versus t. Then
         ries coefficients of v。
                               1 in the circuit shown in                       use PROBE to compute and display the
         Fig. P.64(a). Assume that its input is the                            Fourier transforms of these waveforms. How
         waveform shown in Fig. P.64(b).                                       do they compare? What is the effect of the
      c) Use the PSpice . FOUR statement to compute                            op-amp circuit on the frequency content of
         the Fourier Series coefficients of the first nine                     the voltage at the output?
         harmonic components for b야h the input



67. a) Compute the expressions for the Fourier Se-                             v,
                                                                                ,l, and V。2. How do the analytic results corn-
       ries coefficients of v, 1 and v。
                                      2 in the circuit                         pare to the PSpice outputs?
       shown in Fig. P.65. Assume that its input is                         c) Use PROBE to plot vg, v, ,1, and v。
                                                                                                                 2 versus t.
       the waveform shown in Fig. P.64(b).                                     Then use PROBE to compute and display the
      b) Use the PSpice . FOUR statement to compute                            Fourier transforms of these waveforms. How
         the Fourier Series coefficients of the first기ne                       do they compare? What is the effect of the
         harmonic components for the input waveform,                           op-amp circuit on the frequency content of
                                                                               i拓land i石2?
                                                     149




ANSWERS TO SELECTED PROBLEMS


 1. 198V; 66V·,-l32V



 4. 111.20 V; 117 V; 228.3 V



 7. V, == 0 \／·, 凡 = 2M1



14. The PROBE plot agrees with the solution
    i = (500t + 0.05)e '（比A, t 之 0.



19. a) The PROBE plot agrees with the solution
       i = 100 - 36em째mm24e닉00'A.
    b) 3.47 ms



23. a) 22.44 杉s
    b) The PROBE plot agrees with the analytic so-
       lution (_500/7)e_ t sin Wdt, where
       a = 40000 rad/s, Wd = 280 krad/s.
    c) 67 V at 3.4 /1s



24. a) iL = 8 - 8e나 cos 8t - e ' sin 8t A
    b) From the plot, iL(ma兀) = 13.39A at 400 ms.
150   ANSWERS TO SELECTED PROBLEMS



      27. a) The PROBE plot agrees with the analytic so-
             lution (- 100 + 84et + 36e2i)u(t) A.

          b) i (O) = 20 A; i（叫 = 크OOA



      29. a) The PROBE plots agree with the analytic so-
             lution for VB and Vc: vc = (5 - 5e_t cos lOt
             - 0.5e나 sin lOt) V and
             Va = -25.25et sin lOt V.
          b) 8.655 V; 320 ms
          c) 8.652 V; 314.16 ms; compare to (b)



      32. a) The PROBE plots agree with the analytic so-
             lutions: v01 = (- 1.25 + l. 25e2o') V, t 之 0
             and i拓2 = (5 卞 10e_ tOt + 5e_20t) \/, t 之 0.
          b) t               v01 (V)                         v。
                                                              2 (V)
                        PROBE        幻lal.              PROBE      Anal.
             0           0（勺               0              0（勺             0
             0.1        -1.081          -1.081            1.996         1.998
             0.2        -1.227          -1.227            3.738         3.738
             0.3        -1.247          -1.247            4.515         4.515
             0.4        -1.25           -1.2496           4.819         4.819
             0.5        -1.25           -1.2499           4.933         4.933

      (*) Actually, the cursor reading from PROBE for this value is not
      exactly zero, due to its representation in the computer, but has a value
      whose units are microvolts (DV), which is essentially zero.



      35. a) 34.63 V; 2.19 s; S s; 1 5; 12.5 V
          c) 34.59 V; 2.20 5; 5 5; 1 5; 12.5 V
          d) Compare the values in (a) and (c).



      37. a) vO = 3.675L6.886' V; v = 1.690L57.66" V;
             V2 = 1.946L - 51.140 V;
             iO = 2.917L - 19.780 mA

          b) Pdel = 2 P     = 9.6637 mW



      39. I0 = 18.68L - 9.9" A; I1 = 3.688L139.4" A
                             ANSWERS TO SELECTED PROBLEMS   151



4
    a) i1 = 2.361L - 64.290 A;
       i2 = 74.15乙 小 21.41O mA
    b) Pde1 = 154.64 W; Pdj: = 153.65 W; checks to
       1 W in 155 W




48. a) 508.4L - 41.99OV;
    b) 508.41L - 41.99O V




51. a) 159.155 kHz;
    b) 7.50 V;
    c) 7.94V;
    d) 225.25 kHz




53. C (nF)       Iv。
                   I (V)
     5.72         27.03
     6.72         28.34
     7.72         28.83
     8.72         28.34
     9.72         27.01




58. a) VO = 0, t <0
       v。= 400 - 400e_4t V. 0 5 t 5 0.50 s
       vO = -400 + 745.87e4(i10·5) V, 0.5 드 t 드 1 s
       VO = -2.99.06e4(i l) V, 1 드 t 드 m S
    b) The PROBE plot agrees with the analytic ex-
       pressions in (a).
    c) Quantity       Anal. (V)   PROBE (V)
        vO(0.2)         220.27        219.7
        vO(0.5)         345.87        345.0
        v。(0.7)        -64.86       -64.41
        vO(1.0)       -299.06      -298.60
        v。(1.2)       -134.38      -134.30
152   ANSWERS TO SELECTED PROBLEMS



      61. a) The PROBE plot agrees with the analytic so-
             lution.
          b), c) t (s)         PROBE           Anal.
                                 vO (V)        v, (V)
                     0        4.2 )< 10田         0
                     0.5     -2.497             -2.5
                     1.0     -4.994             -5.0
                     1.5     -2.497             -2.5


                                                  0 0 0
                     2.0      7.975 x 10小
                     2.5      7.975 x 10 5
                     3.0      7.975 x iO-



      65. a) The PROBE plots agree with the analytic so-
             lutions:
               vO1= (- lOt+ 4) V, 0 5t 5 0.8s
               VO1 = (lOt - 12) V, 0.8 드 t 드 1.6 s
               i九,1 = (- lOt + 20) V, 1.6 드 t 드 2.4 s
               i石2 = (5尸 + 4t) V, 0 드 t 드 0.8 s
               V。2 = (- 5t2 + 12t - 6.4) V, 0.8 5 t 드 1.6 s
               V。2 = (5t2 - 20t + 19.2) V, 1.6 5 t 드 2.4 s
          b)    t            PROBE            Anal.
                              V。2 (V)         V。
                                               2 (V)
               0           -2.5 x 10田          0
               0.2         -0.60              -0.60
               0.4         -0.80              -0.80
               0.6         -0.60              -0.60
               0.8          2.857 x 10田        0
               1.0          0.60                0.60
               1.2          0.80                0.80
               1.4          0.60                0.60
               1.6         -1.722 X 10巧         0
                                                                                                                   153




 INDEX
 .AC, 62, 63, 65, 126                    Data statements, capacitors, 37,     Fourier transform, 89, 90
 AC power, 67                                     121                         Frequency response (. AC), 75,
 AC steady-state analysis (. AC),           current-controlled current               126
        61, 63, 65, 126                          source夕 10夕 118                bandwidth, 81
   printing, 63, 67                         current-controlled switch, 51,      center frequency, 81
 Ammeter, 8, 18, 24                              120, 123
                                            current-controlled voltage          . IC夕 45夕 126
Bode plots, 80                                   source, 9, 119                Ideal transformers, 73, 74
  straightline, 82                          dependent DC sources, 8            Impulse response, 85
                                           device models, 52, 123             IND model, 58, 124
 CAP model, 58, 124                        exponential pulse sources, 39,     Inductors, 37, 121
 Capacitors, 37, 121                             116                               initial conditions, 37
    initial conditions, 38                 general, 4, 115                    Initial conditions, capacitors, 38
Circuit topology, 4                        ideal transformers, 73                  general (. IC), 45, 126
Circuit variables, 23, 26, 63              independent DC sources, 7, 115          inductors, 37
Comment line, 2                           inductors, 37, 121                      UIC, 40
Cont이 statements, AC steady-              mutual inductance, 71, 122          ISWITCH model, 51, 120
          state an띠ysis (. AC), 61,       piecewise linear sources, 49,
          126                                    117                          .LIB, 34, 123
   DC analysis (. DC), 16, 24, 124        pulsed sources, 85, 117
   Fourier series (. F0UR), 89, 128       resistors, 11, 120                 .MODEL, 52, 58, 123
   frequency response (. AC), 75,         sinusoidal sources, 61, 117        Mutual inductance, 71, 72, 122
         116                              subcircuits, 32, 122
   general, 4, 15, 124                    switches, 49                       Natural response, 43
   initial conditions (. IC), 45, 126     voltage-controlled current         Node connections, 19, 71
   operating point (. 0P), 15, 50,              source, 9, 119
         128                              voltage-controlled switch, 51,     .0P, 15, 50, 128
   sensitivity (. SENS), 21, 125                120, 123
   transfer function (. T그), 17, 18,                                         Op amps, equivalent circuit, 30
                                          voltage-controlled voltage           general, 29
         125                                    source, 9, 118                 ideal, 31
  transient analysis (. TRA寸), 39,      .DC, 16, 24, 124                       library model, 34, 35
         40, 126                        DCanalysis (. DC), 11, 16, 24,         subcircuits, 32, 33
  varying element values                        124                          Operating point (. 0P), 15, 50,
         (. STEP), 57, 127              DC sweep (tow variables), 17, 24            128
Current-controlled current source,      Dependent DC sources, 8              .OPTIONS, 111, 130
         10, 118                        Device models (. MODEL), 52, 123     Output file format, 5
Current-controlled switch, 51, 120,
                                                                             Output statements, general, 5, 23,
         123                            .END, 2, 3, 130                             128
Current-controlled voltage source,      End statement (. END), 2, 3, 130       . PLOT, 5, 43, 129
         9, 119                         . ENDS, 32, 122                        . PRINT, 5, 23, 24, 128
Current sources, AC, 64, 65, 116        EXP, 39, 116                           . PROBE, 6, 42, 44, 129
  current-controlled, 10, 118           Exponential sources (EXP), 39,
  DC (dependent), 8                           116                            Piecewise linear sources, 49, 50,
  DC (independent), 7, 115
                                                                                     117
  exponential pulse, 39, 116            Fields, name, 2                      . PLOT, AC, 77
  piecewise linear, 49, 117               number, 2                             DC, 5, 43, 129
  pulsed, 85, 117                       .FOUR, 89, 90, 128                      TRAN, 41, 44
  sinusoidal, 61, 117                   Fourier series (. FOU昑, 89, 90,      Plot statement (. PL0T), 5, 125
  voltage-controlled, 9, 119                   128                           Polarity, 4
154                                             INDEX


Power dissipation, 12, 13           Pulsed sources (PULSE), 85, 86,      .T已 17, 18, 125
.PRI町, AC, 63, 77                         117                            Thdvenin equivalent, 18, 19
  DC, 5, 23, 24, 128                PWL, 49, 50, 117                     Title line, 2, 3, 130
  TRAN夕 41                                                               .TRAN, 40, 126
Print statement (. PRINT), 5, 128                                        Transfer function (. TF), 17, 18,
.PROBE, 6, 42, 44, 129              RES model, 58, 124                           125
PROBE graphics post-processor,      Resistors, 11, 120                   Transient response (. TRAN), 39,
        AC power, 67                                                             40, 126
  algebra, 68                                                              printing, 41
  analog plot menu, 107             Scale factors, 3                       plotting, 41, 44
  Bode plots, 80                    .SENS, 21, 125
  Fourier transform, 89, 90         Sensitivity (. SENS), 21, 125        UIC, 40
  frequency response, 78            Sensitivity ot却此 22
  general (. PROBE), 6, 42, 44,     Simulation parameters, ill           V町ying element values (. STEP),
        129                         SIN, 61, 117                                57, 127
  menu system, 106                  Sinusoidal sources (SIN), 61, 117    Voltage-controlled current source,
  st町tup menu, 106                  Source file creation, 3                     9, 119
  straightline Bode plots, 82       SPICE versus PSpice, 113             Voltage-controlled switch, 51, 55,
  using menus, 110                  Statements, continuation, 1                 120, 123
PSpice Control Shell, 3, 99            fields, 1                         Voltage-controlled voltage source,
  Analysis menu, 103                .STEP, 57, 59, 79, 127                      9, 118
  Circuit menu, 102                 Step response, 53                    Voltage sources, AC, 64, 65, 116
  Display menu, 103                 Subcircuit description (. SUBCKT),     current-controlled, 9, 119
  Files menu, 101                           31, 122                       DC (dependent), 8
  function keys, 100                Subcircuit end (. ENDS), 32, 122      DC (independent), 7, 115
  Probe menu, 104                   .SUBCKT, 21, 122                      exponential pulse, 39, 116
  Quit menu, 104                    Switches, current-controlled, 51,     piecewise linear, 49, 117
  Stmed menu, 102                           120, 123                      pulsed, 55, 117
  using menus, 104                    general, 49                          sinusoidal, 61, 117
PSpice in general, 1                  ideal, 54                            voltage-controlled, 9, 118
PSpice model library, 34, 123         realistic, 54                      VSWITCH model, 51, 55, 120
PSpice quick reference, 115           voltage-controlled, 51, 55, 120,
PULSE, 85, 86, 117                          123                          .WIDTH, 111, 130
