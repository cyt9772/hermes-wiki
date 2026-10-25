---
source_url: /run/media/yutae/Data/Coding_Information_Theory.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 3e50497ee3f4df013386405b99b2ea78cd8dcf3c0e573a20491fc47a0e3c8a57
---

# Coding and Information Theory (2nd ed) (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출. 일부 토큰은 원서 원형과 미묘히 다름 (인식 오류 아님, text-layer 원본). 원문 PDF(`/work/wiki/raw/books/Coding_Information_Theory.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Coding and Information Theory (2nd ed)
- authors: Richard W. Hamming
- pages: 280 (pdfinfo)
- source file: `Coding_Information_Theory.pdf` (sha256: `3e50497ee3f4df01…`, 324 MB)
- extract: `pdftotext -layout` @ 2026-10-25, 676,733 chars

## Original text (all 280 pages)

Richard W. Hamming
      econd Edit



Codii and
In아m計a
Coding
and
初／ormat加nT)노eory
Second Ed玭이1




Co成兀g
and
Information Theory



RICHARD W. HAMMING

Na，
  口／／七7stgr口（luate Sc出rool




PRENTICE－月Al工 / Englewood C／刃노 NJ 07632
Library of Congress Cataloging-In.加t小C으tion I加ta
Hamming, R. W. (Richard Wesley) 1915
   Coding and information theory.

    Bibliography: p.
    Includes index
    1. Coding theory. 2. Information theory.
I. T川e.
OA268.H35       1986   519.4    85- 17034
ISBN 0-13-139072-4




Editorial/production supervision and
  interior design: Nicholas C. Romanelli
Cover design: Frederick Charles Ltd.
Manufacturing buyer: Rheit Conklin



@1986, 1980 by Prentice-Hall
A Division of Simon & Schuster, Inc.
Englewood Cliffs, New Jersey 07632




All rights reserved. No part of this book may be
reproduced, in any form or by any means,
without permission in writing from the publisher.


Printed in the United States of America


10 9    8   7 6    5   4




ISBN         0-13-139072- 4                         01




Prentice-Hall International (UK) Limited, London
Prentice-Hall of Australia Pty. Limited, Sydney
Prentice-Hall Canada Inc., Toronto
Prentice-Hall Hispanoamericana, S.A., Mexico
Prentice-Hall of India Private Limited, New Delhi
Prentice-Hall of Japan, Inc., Tokyo
Prentice-Hall of Southeast Asia Pie. Ltd., Singapore
Editora Prentice-Hall do Brasil, Ltda., Rio de Janeiro
Whitehall Books Limited, Wellington, New Zealand
                                                 Co,玎e砒S




Preface


 1   Introduction 1

     1.1    A Very Abstract Summary 1
     1.2    History 2
     1.3    Model of the Signaling System 4
     1.4    Information Source 5
     1.5    Encoding a Source Alphabet 7
     1.6    Some Particular Codes 9
     1.7    The ASCII Code 10
     1.8    Some Other Codes 12
     1.9    Radix r Codes 15
     1.10   Escape Characters 15
     1.11   Outline of the Course 17



 2 Error-Detecting Codes        20

     2.1    Why Error-Detecting Codes? 20
     2.2    Simple Parity Checks 21
     2.3    Error-Detecting Codes 22
     2.4    Independent Errors: White Noise 23
     2.5    Retransmission of Message 25

                                                       V
vi    Contents

     2.6    Simple Burst Error-Detecting Codes 26
     2.7    Alphabet Plus Number Codes: Weighted Codes 27
     2.8    Review of Modular Arithmetic 30
     2.9    ISBN Book Numbers 32



 3 Error-Correcting Codes 34

     3.1    Need for Error Correction 34
     3.2    Rectangular Codes 35
     3.3    Triangular, Cubic, and n-Dimensional Codes 37
     3.4    Hamming Error-Correcting Codes 39
     3.5    Equivalent Codes 42
     3.6    Geometric Approach 44
     3.7    Single-Error-Correction Plus
            Double-Error-Detection Codes 47
     3.8    Hamming Codes Using Words 49
     3.9    Applications of the Ideas 49
     3.10   Summary 50



 4   Va亢able-Lengt力 Codes: Ha乃沇口n Codes            51

     4.1    Introduction 51
     4.2    Unique Decoding 52
     4.3    Instantaneous Codes 53
     4.4    Construction of Instantaneous Codes 55
     4.5    The Kraft Inequality 57
     4.6    Shortened Block Codes 60
     4.7    The McMillan Inequality 62
     4.8    Huffman Codes 63
     4.9    Special Cases of Hu卄man Coding 68
     4.10   Extensions of a Code 72
     4.11   Huffman Codes Radix r 73
     4.12   Noise in Huffman Coding Probabilities 74
     4.13   Use of Huffman Codes 77
     4.14   Hamming-Huffman Coding 78



5 Miscellaneous Codes         79

     5.1    Introduction 79
     5.2    What Is a Markov Process? 80
                                                         Contents   vii

    5.3    Ergodic Markov Processes 84
    5.4    Efficient Coding of an Ergodic Markov Process 86
    5.5    Extensions of a Markov Process 87
    5.6    Predictive Run Encoding 88
    5.7    The Predictive Encoder 89
    5.8    The Decoder 90
    5.9    Run Lengths 91
    5.10   Summary of Predictive Encoding 94
    5.11   What Is Hashing? 94
    5.12   Handling Collisions 95
    5.13   Removals from the Table 96
    5.14   Summary of Hashing 96
    5.15   Purpose of the Gray Code 97
    5.16   Details of a Gray Code 98
    5.17   Decoding the Gray Code 99
    5.18   Anti-Gray Code 99
    5.19   Delta Modulation 100
    5.20   Other Codes 101



6 Entropy and Shannon's First Theorem 103

    6.1    Introduction 103
    6.2    Information 104
    6.3    Entropy 107
    6.4    Mathematical Properties of
           the Entropy Function 114
    6.5    Entr아갸 and Coding 끄9
    6.6    Shannon-Fano Coding 121
    6.7    How Bad Is Shannon-Fano Coding? 122
    6.8    Extensions of a Code 124
    6.9    Examples of Extensions 126
    6.10   Entropy of a Markov Process 129
    6.11   Example of a Markov Process 131
    6.12   The Adjoint System 133
    6.13   The Robustness of Entropy 136
    6.14   Summary 137



7   T九eC뇨innel and Mutu可In加rmation 138

    7.1    Introduction 138
    7.2    The Information Channel 139
viii    （勿nt日I打


       7.3    Channel Relationships 140
       7.4    Example of the Binary
              Symmetric Channel 142
       7.5    System Entropies 145
       7.6    Mutual Information 148

 8 C九annel Capaci砂 153

       8.1    Definition of Channel Capacity 153
       8.2    The Uniform Channel 154
       8.3    Uniform Input 156
       8.4    Error-Correcting Codes 158
       8.5    Capacity of a Binary
              Symmetric Channel 159
       8.6    Conditional Mutual Information 161

 9 Some Mathematical Preliminaries 164

       9.1    Introduction 164
       9.2    The Stirling Approximation to n! 165
       9.3    A Binomial Bound 170
       9.4    The Gamma Function f (n) 173
       9.5    n-Dimensional Euclidean Space 176
       9.6     A Paradox 179
       9.7    Chebyshev's Inequality and the Variance 181
       9.8    The Law of Large Numbers 183
       9.9    Other Metrics 189


10 S九口nnon농 Main T九eore刃i 191

       10.1   Introduction 191
       10.2   Decision Rules 192
       10.3   The Binary Symmetric Channel 195
       10.4   Random Encoding 196
       10.5   Average Random Code 201
       10.6   The General Case 204
       10.7   The Fano Bound 205
       10.8   The Converse of Shannon's Theorem 207

11 Al뇽ebr口加 (oding T九eory            209

       11.1 Introduction 209
       11.2 Error-Detecting Parity Codes Revisited 210
                                                   （勿ntents   ix


11.3 Hamming Codes Revisited 211
11.4 Double-Error-Detecting Codes Revisited 213
11.5 Polynomials versus Vectors 214
11.6 Prime Polynomials 215
11.7 Primitive Roots 219
11.8 A Special Case 220
11.9 Shift Registers for Encoding 224
11.10 Decoding Single-Error-Correcting Codes 227
11.11 A Double-Error-Correcting Code 228
11.12 Decoding Multiple-Error Codes 234
11.13 Summary 234



Appem伽A: 及i7岫V油九 and I九e Sample T九eorem 237

A.1   Introduction 237
A.2   The Fourier Integral 238
A.3   The Sampling Theorem 240
A.4   Bandwidth versus Rapid Change 242
A.5   AM Signaling 242
A.6   FM Signaling 244
A.7   Pulse Signaling 245
A.8   Bandwidth Generally 246
A.9   Continuous Signals 247



Appendix B: Some Tables for Entropy Calculations 250


References 253


Index 255
             Preface to the Second Edition




The second edition is mainly an expansion of the material in the first
edition. The changes were made to (1) increase the clarity of the pres-
entation, (2) extend some of the basic ideas, and (3) indicate further
practical details. I have resisted the urgings (both from others and
myself) to include more difficult codes, such as Reed-Muller, Viterbi,
Fire, and cyclic. They seem to be more suitable for a second course,
and in any case require a firmer mathematical background than I have
assumed, if they are to be "understood." I still believe that it is better,
in this subject, to master the fundamentals than it is to rush through,
with little real understanding, a large body of material. There are now
many excellent texts devoted to algebraic coding theory.
     Bostrom Management Corporation is thanked again for excellent
cooperation.
                                                         R. W. HAMMING




x
                                                   C아玎en打   ix

11.3 Hamming Codes Revisited 211
11.4 Double-Error-Detecting Codes Revisited 213
11.5 Polynomials versus Vectors 214
11.6 Prime Polynomials 215
11.7 Primitive Roots 219
11.8 A Special Case 220
11.9 Shift Registers for Encoding 224
11.10 Decoding Single-Error-Correcting Codes 227
11.11 A Double-Error-Correcting Code 228
11.12 Decoding Multiple-Error Codes 234
11.13 Summary 234



Appem伽 A: B口n小vidt九 and I九e Sample T九eorem          237

A.1   Introduction 237
A.2   The Fourier Integral 238
A.3   The Sampling Theorem 240
A.4   Bandwidth versus Rapid Change 242
A.5   AM Signaling 242
A.6   FM Signaling 244
A.7   Pulse Signaling 245
A.8   Bandwidth Generally 246
A.9   Continuous Signals 247



Appendix B: S이ne Tables for Entroj砂 C口九U끄ztions 250


References 253


Index 255
             Preface to the Second Edition




The second edition is mainly an expansion of the material in the first
edition. The changes were made to (1) increase the clarity of the pres-
entation, (2) extend some of the basic ideas, and (3) indicate further
practical details. I have resisted the urgings (both from others and
myself) to include more difficult codes, such as Reed-Muller, Viterbi,
Fire, and cyclic. They seem to be more suitable for a second course,
and in any case require a firmer mathematical background than I have
assumed, if they are to be "understood." I still believe that it is better,
in this subject, to master the fundamentals than it is to rush through,
with little real understanding, a large body of material. There are now
many excellent texts devoted to algebraic coding theory.
     Bostrom Management Corporation is thanked again for excellent
cooperation.
                                                         R. W. HAMMING




x
                 Preface to the First Edition




This book combines the fields of coding and information theory in a
natural way. They are both theories about the representation of abstract
symbols. The two fields are now each so vast that only the elements
can be presented in a short book.
     Information theory is usually thought of as "sending information
from here to there" (transmission of information), but this is exactly
the same as "sending information from now to then" (storage of infor-
mation). Both situations occur constantly when handling information.
Clearly, the encoding of information for efficient storage as well as
reliable recovery in the presence of "noise" is essential in computer
science.
     Since the representation, transmission, and transformation of in-
formation are fundamental to many other fields as well as to computer
science, it is time to make the theories easily available. Whenever and
wherever problems of generation, storage, or processing of information
arise, there is a need to know both how to compress the textual material
as well as how to protect it against possible mutilation. Of the many
known encoding methods, we can indicate only a few of the more im-
portant ones, but hopefully the many examples in the text will alert the
student to other possibilities.
     The text covers the fundamentals of the two fields and gives ex-
amples of the use of the ideas in practice. The amount of background
mathematics and electrical engineering is kept to a minimum. The book

                                                                      xi
xii   Preface to the First Edition

uses, at most, simple calculus plus a little probability theory, and any-
thing beyond that is developed as needed. Techniques that have re-
cently arisen in computer science are used to simplify the presentation
and the proofs of many results. These techniques are explained where
they are used, so no special knowledge of computer science is required.
Many other proofs have been greatly simplified, and when necessary
new material has been developed to meet current technological needs.
An effort has been made to arrange the material, especially the proof
of Shannon's main result, so that it is evident why the theorems are
true, not just that they have been proved mathematically.
     Chapter 11, on algebraic codes, develops the needed mathematics
of finite fields. Because of its mathematical difficulty, this chapter is
placed last and out of logical order. It can follow Chapter 3, if desired.
There is a deliberate repetition in the text; important ideas are usually
presented at least twice to ensure that the reader understands them.
     The text leaves out large areas of knowledge in the belief that it is
better to master a little than to half know a lot. Thus more material
may easily be added (at the discretion of the teacher) when it seems
appropriate for the class.
     I have followed custom in referring to Hamming codes and Ham-
ming distance; to do otherwise would mislead the student and be false
modesty.

Acknowledgments

It is difficult for the author to recall all his indebtedness to others, since
he has known about the material from many years of working at the
Bell Laboratories. Teaching a course at the Naval Postgraduate School,
based on N. Abramson's elegant, small book, Information Theory and
Coding (Ref. [A]), rearoused this author's interests in the two fields.
Short courses on the topic at other places further developed many of
the simplifications, elaborations, and examples, and the help of many
students is gratefully acknowledged. The help of Albert Wong is es-
pecially appreciated.
      In the actual production of the book, thanks are due to Bostrom
Management Corporation, especially to Doug Thompson. However,
as always, all faults are to be assigned to the author.
                                                           R. W. HAMMING
    Chapter 1



                                                       Introduction




    1.1 A Very Abstr口Ct Su,刃兀ary

     Although the text uses the colorful words "information," "transmis-
     sion," and "coding," a close examination will reveal that all that is
     actually assumed is an information source of symbols s1, s2, . . . ,Sq.
     At first nothing is said about the symbols themselves, nor of their pos-
    sible meanings. All that is assumed is that they can be uniquely rec-
    ognized.
          We cannot define what we mean by a symbol. We communicate
    with each other in symbols, written or spoken (or even gestures), and
    we may or may not think in terms of symbols, but since we must use
    symbols to define what we mean by a symbol, we see the circularity of
    the process. Thus the meaning of a symbol must remain at the intuitive
    level.
         Next we introduce (Sections 4.8 and 6.2) the probabilities Pi'P2' . . . ,
    Pq of these symbols occurring. How these p, are determined is not part
    of the abstract theory. One way to get estimates of them is to examine
    past usage of the symbol system and hope that the future is not signif-
    icantly different from the past. For any discrete probability distribution
    there is the value of thelentropy function:




1   The function H of the probability distribution p, measures the amount



                                                                                1
2    Ch. I / Intro加Cti(가I


of uncertainty, surprise, or information that the distribution contains.
This function plays a leading role in the theory and provides a lower
bound on the average code length. Later we examine more complex
probability structures involving the symbols s.
     The problem of representing the source alphabet symbols si in terms
of another system of symbols (usually the binary system consisting of
the two symbols 0 and 1) is the main topic of the book. The two main
problems of representation are the following.

    1. Channel encoding: How to represent the source symbols so that
       their representations are far apart in some suitable sense. As
       a result, in spite of small changes (noise) in their representations,
       the altered symbols can, at the receiving end, be discovered to
       be wrong and even possibly corrected. This is sometimes called
       "feed forward" error control.
    2. Source encoding: How to represent the source symbols in a mm1l-
       imal form for purposes of efficiency. The average code length


                              L = 2 pili

       is minimized where 1, is the length of the representation of the ith
       symbol s,. The entropy function provides a lower bound on L.

     Thus, in principle, the theory is simply an abstract mathematical
theory of the representation of some undefined source symbols in terms
of a fixed alphabet (usually the binary system) with the representation
having various properties. In this abstract theory there is no transmis-
sion through the channel, no storage of information, and no "noise is
added to the signal." These are merely colorful words used to motivate
the theory. We shall continue to use them, but the reader should not
be deceived; ultimately this is merely a theory of the representation of
symbols. Clearly, this is a fundamental theory for much of human
symbol manipulation.


1.2 History

The beginnings of both coding and information theory go far back in
time. Many of the fundamental ideas were understood long before
1948, when information theory was first established on a firm basis. In
1948 Claude E. Shannon published two papers on "A Mathematical
Theory of Communication" in the Bell System Technical Journal (re-
                                                 Sec. 1.2. I History    3

printed in Ref. [S]). The papers almost immediately popularized the
field of information theory, and soon additional papers on information
theory appeared in the journals, and courses were taught on the subject
in electrical engineering and other departments of many universities.
     As in most fields that suddenly open up, many of the early appli-
cations were ill advised; but how else are the limitations of a new field
to be discovered? As a result of the overexpectations of what infor-
mation theory could do, disenchantment gradually set in, and a con-
sequent decrease in the number of courses taught. Now, perhaps, a
more just evaluation can be made, somewhere between the wild enthu-
siasm of the first days and the sad disappointment that slowly
followed.
     Information theory sets bounds on what can be done, but does little
to aid in the design of a particular system. The idea that it is therefore
useless to know information theory is false, as the following analogy
shows. Consider the theory of evolution as taught in biology. Few
students will ever apply it directly in their lives, yet it is a valuable
constellation of ideas. In spite of this lack of direct application, when
the ideas behind

    1. Small changes in the species (variations)
    2. Survival of the fittest (selection)

are mastered, the ideas can profitably be used in many other situations,
often far removed from biology. For example, when looking at a social
institution, such as a computer science department, a university, a mil-
itary organization, a banking system, a government, or even a family
relationship, one asks: "How did the present situation arise?" and
"What forces selected this particular realization for survival?"
      A little more appreciation of the power of the theory suggests the
questions: "Given the present forces on the social institution, what are
its possible variations (its ability to respond to the forces)?" and "How
will it evolve (what will survive)?" Thus the ideas in the theory of
evolution can be used in many situations far removed from biology.
      When asking "How will it evolve?" it is often worth the effort to
consider three similar questions:

     What can evolve?
     What should evolve?
     What will evolve?

With the answers in mind, you are in a position to consider how to bring
the third answer more into line with the second-how to improve things,
4     Ch. 1 I introduction

 rather than merely settling for the inevitable that will occur if you do
 nothing active to alter the world.
      Similarly, information theory has ideas that are widely applicable
 to situations remote from its original inspiration. The applicability of
 the ideas is often not exact-they are often merely suggestive-but the
ideas are still very useful.
      At about the time that information theory was created, and in about
the same place, coding theory was also created. The basic paper, how-
ever, was delayed by patent requirements until April 1950, when it
appeared in the Bell System Technical Journal (reprinted in Refs.[Bi],
[Bla], and [T]). In the case of coding theory, the mathematical back-
ground was at first less elaborate than that for information theory, and
for a long time it received less attention from the theorists. With the
passing of time, however, various mathematical tools, such as group
theory, the theory of finite fields (Galois theory), projective geometry,
and even linear programming have been applied to coding theory. Thus
coding theory has now become an active part of mathematical research
(Refs. [Bi],[B3],[B4],[C],[Gui,[Li],[L2],[MS],[Mc],[P],[W]).
      Most bodies of knowledge give errors a secondary role, and rec-
ognize their existence only in the later stages of design. Both coding
and information theory, however, give a central role to errors (noise)
and are therefore of special interest, since in real life noise is everywhere.
     Logically speaking, coding theory leads to information theory, and
information theory provides bounds on what can be done by suitable
encoding of the information. Thus the two theories are intimately re-
lated, although in the past they have been developed to a great extent
quite separately. One of the main purposes of this book is to show
their mutual relationships. For further details on the history of coding
theory, see Refs. [B2] and [TI. By treating coding theory first, the
meaning of the main results of information theory, and the proofs, are
much clearer to the student.

1.3 Model of the Signaling System

The conventional signaling system is modeled by:

    1. An information source
    2. An encoding of this source
    3. A channel over, or through, which the information is sent
    4. A noise (error) source that is added to the signal in the channel
    5. A decoding and hopefully a recovery of the original information
       from the contaminated received signal
    6. A sink for the information
                                                   Sec. 1.4 / Information Source   S

      This model, shown in Figure 1.3-1, is the one that we will use for
 our signaling system. It has many features of signaling systems now in
 use.



                                 (Noise)
                                                          (4)




                   Encode   H+
                                 m
                                           Channel   H＝    杉    Decode

      (1)            (2)                     (3)                 (5)         (6)
                   Figure 1.3-1 Standard signaling system

     The boxes ENCODE and DECODE should both be thought of as
 being divided into two parts. In the ENCODE box, we first encode
 the 少, ircg, taking advantage of any structure in the symbol stream.
 The more structure there is, the more, typically, we can compress the
 encoding. These encoded symbols are then further encoded to com-
pensate for any known properties of the c?za杉序可. Typically, this second
stage of encoding expands the representation of the message. Thus the
ENCODE box first （如明 요urGe李nco曲艮．巍IIQ雎立上墨磁q心心g1呂肛
                                                                        M'
ing. The DECODE box must, of course, reverse these encodings in
the proper order to recover the original symbols.
     This separation into two stages is very convenient in practice. The
various types of sources are separately encoded into the standard in-
terface between the source and the channel, and then are encoded for
the particular channel that is to be used. Thus there is great flexibility
in the entire system.


1.4 Information Source

We begin, therefore, w油 the f . 黛낀：坦型Fe．· The p0꿔er of both
coding and information theory is to a great extent due to the fact that
we do not define what information is- we assume a source of infor-
mation, a sequence of symbols in a source alphabets1, S2, 1 1 1 , sq, having
q symbols. When we get to Chapter 6 we will find that information
theory uses the entropy function H as a me工5ure of information, and by
implication this defines what is meant by "the amount of information."
But this is an abstract definition that agrees only partly with the corn-
monly accepted ideas concerning information. It is probably this ap-
6    Ch. 1 / introduction

pearance of treating what we mean by "information" that made infor-
mation theory so popular in the early days; people did not notice the
differences and thought that the theory supplied the proper meaning in
all cases. The implied definition does give the proper measure to be
used for information in many situations (such as the storage and trans-
mission of data), and people hoped that their situation was one of these
(they were often wrong!). Information theory does not handle the
meaning of the information; it treats only the amount of information,
and even the amount depends on how you view the source.
      The source of information may be many things; for example, a
book, a printed formal notice, and a company financial report are all
information sources in the conventional alphabetic form. The dance,
music, and other human activities have given rise to various forms(sym-
bols) for representing their information, and therefore can also be in-
formation sources. Mathematical equations are still another informa-
tion source. The various codes to which we turn next are merely particular
ways of representing the information symbols of a source.
      Information also exists in continuous forms; indeed, nature usually
supplies information to us in that form. But modern practice is to
sample the continuous signal at equally spaced intervals of time, and
then to digitize (quantize; Ref. [J]) the amount observed. The infor-
mation is then sent as a stream of digits. Much of the reason for this
use of digital samples of the analog signal is that they can be stored,
manipulated, and transmitted more reliably than can the analog signal.
When the inevitable noise of the transmission system begins to degrade
the signal, the digital pulses can be sensed (detected), reshaped, and
amplified to standard form before relaying them down the system to
their final destination. At the destination the digital pulses may, if
necessary, be converted back to analog form. Analog signals cannot
be so reshaped, and hence the farther the signal is sent and the more
it is processed, the more degradation it suffers from small errors.
      A second reason that modern systems use digital methods is that
large-scale integrated circuits are now very cheap and provide a powerful
 method for flexibly and reliably processing and transforming digital
signals.
      Although information theory has a part devoted to analog (contin-
 uous) signals, we shall concentrate on digital signals both for simplicity
of the theory and because, as noted above, analog signals are of de-
creasing importance in our technical society. Almost all of our large,
 powerful computers are now digital, having displaced the earlier analog
 machines almost completely in information-processing situations. There
 are almost no large, general-purpose hybrid systems left (1985). Most
 of our information transmission systems, including the common tele-
 phone and hi-fi music systems, are also rapidly going to digital form.
                                 Sec. 1.5 I Encoding a Source Alphabet      7

1.5 Encoding a Source Alphabet

It is conventional to represent information (digital signals or more simply
symbols) as being in one of two possible states: a switch up or down,
on or off, a hole punched or not, a relay closed or open, a transistor
conducting or not conducting, a magnetic domain magnetized N-S or
S-N, and so on. Currently, devices with two states, called binary de-
vices, are much more reliable than are multistate devices. As a result,
binary systems dominate all others. Even decimal information-pro-
cessing systems, such as hand calculators, are usually made from binary
parts.
      It is customary to use the symbols "0" and "1" as the names of the
two states, but any two distinct symbols (marks), such as a circle and a
cross, will do. It is often useful to think of the 0 and 1 as only a pair
of arbitrary symbols, not as numbers.
      First we consider merely the problem of representing the various
symbols of the source alphabet. Given two binary (two-state) devices
(digits), we can represent four distinct states (things, symbols):

                                       00
                                       01
                                       10
                                       11

For three binary digits we get 23 = 8 distinct states:

                                000            100
                                001            101
                                010            110
                                011            111

For a system having k binary digits-usually abbreviated as bits- the
total number of distinct states is, by elementary combinatorial theory,

                                       2
                                           "


In general, if we have k different independent devices, the first having
n1 states, the second n2 states, . . . , the kth having n,,, states, then the
total number of states is clearly the product

                                7ilri2 · . · /ik

For example, if n1 = 4, n2 = 2, and n3 = 5, we can represent 4 x 2
x 5 = 40 distinct items (states). This provides an upper hound on the
number of possible representations.
 8    Cli. 1 / Introduction

        This is the maximum number of source symbols we can represent
 if all we consider is the number of distinct states.. In Chapter 4 we
 discuss how, using variable-length codes, to take advantage of the prob-
 abilities of the source symbols occurring. For the present we merely
 consider the number of distinct states-and this is the same as assuming
 that all the source symbols are equally likely to occur.
        We have emphasized two-state devices with two symbols; other
 multistate devices exist, such as a "dead-center switch," with three states.
 Some signaling systems also use more than two states, but the theory
 is most easily presented in terms of two states. We shall therefore
 generally use a binary system in the text and only occasionally mention
 systems with r states.
       Human beings often attribute meanings to the sequences of 0's and
 l 's, for example in the ASCII code (Table 1.7-1). The computer (or
 signaling system), however, merely regards them as sequences of 0's
 and l 's. In particular, a digital computer is a processor of streams of
 the two symbols-it is the user (or possibly the input or output equip-
ment) that assigns meanings; the computer merely combines 0's and l 's
according to how it is built and how it is programmed. The logic circuits
of a' computer are indi加ent to the meanings we assign to the symboLs;
so is a signaling system.
       This is the reason that information theory ignores the meaning of
the message, and by so doing it enables us to understand what the
equipment does to messages. The theory provides an intellectual tool
for understanding the processing of information without paying attention
to meaning.
       Typically, the channel encoding of the message increases the re-
dundancy (to be defined accurately later), as shown in Chapters 2 and
3. The source encoding (mentioned at the end of Section 1.3) usually
decreases the redundancy, as shown in Chapters 4 and 5.
       We need to think of the source as a random, or stochastic, source
of information, and ask how we may encode, transmit, and recover the
original information. Specific messages are, of course, actually sent,
but the designer of the system has no way of knowing which of the
ensemble of possible messages will be chosen to be sent. The designer
must view the particular message to be sent as a random sample from
the population of all possible messages, and must design the system to
handle any one of the possible messages. Thus the theory is essentially
statistical, although we will use only elementary statistics in this book.


Exercises

1.5-1 Compute the number of license plates                 of the form
      number number number letter letter letter            Ans. (26)3(10)3
                                     Sec. 1.6 / Some Particular Codes   9

1.5-2 How many instructions can there be in a computer with eight
      binary digits for each instruction?         Ans. 28 = 256

吐伊Discuss the 蜘迪畔y system, which uses alternate two- and f加e-
   state devices:；前詐斗甘立띠
                                           六U. ．吠缸？少쓰‘
1.6 So刃w Pai仇cular Co加S

The binary code is awkward for human beings to use. Apparently,
people prefer to make a single discrimination among many things.
Evidence for this is the size of the usual alphabets, running from about
16 to 36 different letters (in both upper- and lowercase) as well as the
decimal system, with 10 distinct symbols. Thus for human use it is often
convenient to group the binary digits, called bits, into groups of three
at a time, and call them the octal code (base 8). This code is given in
Table 1.6-1.

                         TAB!月 1.6-1 0ct口I Code
                          Binary           Octal
                                             0
                           000


                                             l
                                             1 八
                                               乙 八
                                                 4
                                                 V 4
                           001
                           010
                           011
                           100
                                             <
                                             U 6
                           101
                           110
                                             n
                                             /
                           111


     In the octal representation numbers are often enclosed in paren-
theses with a following subscript 8. For example, the decimal number
25 is written in octal as

                                   (31)8

Thus in America, Christmas is Halloween:

                          'Dec 25= Oct31
                            (25)l0 = (31)8

    As an example, in Table 1.7-1 of the ASCII code in the next section
we have written the octal digits in the left-hand column rather than the
10    C/i. 1 I Introduction

binary digits. The translation from octal to binary is so immediate that
there is little trouble in going either way.
     Occasionally, the binary digits are grouped in fours to make the
hexadecimal code (Table 1.6-2). Since computers usually work in bytes,
which are usually 8 bits each (there are now 9-bit bytes in some corn-
puters), the hexadecimal code fits into the machine architecture better
than does the octal code, but the octal seems to fit better into human
psychology. Thus neither code has a clear victory over the other in
practice.

                        TABLE 1.6그 Hexadecimal Code
                         Binary         Hexadecimal




                                              0l23 456 789 ABCDEF


戶沚ercises         ,
            )＼뇨   兀．U

44L Since 28 = 35, compare base 2 and base 3 computers.

1.6-2 Make a multiplication table for octal numbers.

1.6-3 From Table 1.6-2, what is the binary representation of D6?
                                                       Ans. 11010110


1.7 The ASCII Code

Given an information source, we first consider an encoding of it. The
standard ASCII code (Table 1.7-1), which represents alphabetic, flu-
meric, and assorted other symbols, is an example of a code. Basically,
                                          Sec. 1. 7 / The ASCII Code     11

                     TABLE 1.7-1 Seven-Bit ASCIi Code
   Octal   Char-      Octal   Char-     Octal    Char-     Octal   Char-
   Code    acter      Code    acter     Code     acter     Code    acter

    000     NUL        040    SP          100     @         140  '
    001     SOH        041    !           101     A         141  a
    002     STX        042                102     B         142  b
    003    ETX         043    #           103     C         143  c
    004    EOT         044    $           104     D         144  d
    005    ENQ         045    %           105     E         145  e
    006     ACK        046    &           106    F          146  f
   007     BEL         047                107     G         147  g
   010     BS         050     (          110     H         150  h
   011     HT         051     )          111     I         151   i
   012     LF         052                112      J        152   j
   013     ＼牙         053     +          113     K         153  k
   014     FF         054     -          114     L         154  1
   015     CR         055     -          115     M         155  m
   016     SO         056                116     N         156  n
   017     SI         057      /         117     O         157  0
   020     DLE        060     0          120     P         160  p
   021     DC1        061     1          121     Q         161  q
   022     DC2        062     2          122     R         162  r
   023     DC3        063     3          123     S         163  S
   024     DC4        064     4          124     T         164  t
   025     NAK        065     5          125     U         165  U
   026     SYN        066     6          126     V         166  V
   027     ETB        067     7          127     W         167  w
   030     CAN        070     8          130     X         170  x
   031     EM         071     9          131     Y         171  y
   032     SUB        072     :          132     Z         172  z
   033     ESC        073     ,          133     1         173  {
   034     FS         074     <          134     \         174     I
   035     GS         075     =          135     1         175  }
   036     RS         076     >          136               176
   037     Us         077     ?          137     -         177 DEL

this code uses 7 binary digits (bits). Since (as noted already) computers
work in bytes, which are usually blocks of 8 bits. a sinQle ASCII symbol
orten uses o tiltS. m ne eigntn rnt can De set in many ways. It is usually
set so tnat me totai number or i "s in tne eignt positions is an even
number (or else an odd number- see Chapter 2). Sometimes it is
always set as a 1 so that it can be used as a timing source. Finally, it
may be left arbitrary and no use made of it. To convert to the modified
ASCII code used by the LT33 8-bit teletype code, use 7-bit ASCII code
+ (200)8.
12     Ch. 1 / Introduction

       The purpose of the even number of l 's in the eight positions is that
 then any single error, a 0 changed into a 1 or a 1 changed into a 0, will
 be detected, since after the change there will be, in total, an odd number
 of l 's in the whole eight positions. Thus we have an르rror-detecting
 code that gives some orotection against errors. Perhavs more imoortant.
 1ne,cooe enaDies me maintenance tq oe aone mucn,more easily anu
;eliably since the presenceof errors is determined by the machine itself,
rand to some extent the source of the errors can actually be located by
 the code.
       We shall frequently use the check of an even (or odd) number of
 l 's. It is called a pasj . heck, since what is checked is only the parity
 (the evenness or oddness) of the number of l 's in the message. Many
 computers have a very useful instruction that computes the parity of the
 contents of the accumulator.
       We are now in a better position to understand the ASCII code
 (Table 1.7-1). The ASCII has a source alphabet of

                                 27 = 128

possible characters (symbols). These characters are represented (en-
coded) inside a computer in the binary code. An even-parity check can
be used to set the eighth position of the 8-bit bytes of the ASCII code.
The three printed symbols of Table 1.7-1 are in the octal code. As an
example

                              127 = 1 010 111

 (where we have dropped the first 2 bits of the first octal symbol). For
 an even-parity check this would be 127 = 11 010 111

E노ercises

1.7-1 Write the letters P and p in binary.

1.7-2 To what does 01 11110      010 correspond?

 1.7-3 Using base 4 code, write out the lowercase ASCII alphabet.
                                           乙二    i1
 1.7-4 Write out the uppercase ASCII alphabet in base 16.

                     "Y "V
1.8 Some Other Codes

 Another familiar code is the Morse code, which was once widely used.
 Part of the code is given in Table 1.8-1. The dash is supposed to be
 three times the length of the dot. Although the Morse code may appear
                                                                 Sec. 1.8 I Some Other Codes   13

                             TABLE 1.8.1                         Morse Code




                              ABC了EFGHrJKLMNOPQRSTUVWXYZ
                    似




 to be encoded in a binary code, it is, in fact, a t工nary (radix 3, r = 3)
 code, having the symbols dot, dash, and space. The space between
 dots and dashes in a single letter is 1 unit of time, between letters it is
.3 time uni ts, and be工뾰e료n皿ords it is 6 time tin汭
      We now make a brief digression to introduce a notation. We will
 continually need the binomial coefficients

                                                                    ii!
                            C(n k ' =
                        \,,. V ' " ' " "                        k! (n- k)!

 They count the number of ways a set of k items can be selected from
 a set of n items. We have adopted the old-fashioned notation C(n, k)
 because it is easily produced on a typewriter, it is easily set in print,
 and it can be gracefully handled by most computers. The currently
 p아川ar notation

                                                           (n
 14    Ch. 1 I Introduction

  is difficult for most equipment to handle and is awkward when it appears
  in running text.
       J he Morse code is clearly a variable-length code that taks advap-
  tge of the high frequency of occurrence of some letters, such as "E,"
  by making them short, and the very infrequent letters, such as "J,"
.relatively longer. However, the problems that arise when trying to
  recognize the words of a variable-length code are great enough in this
  case to cause almost complete replacement of the Morse code by the
  van Duuren code, which,uses three out of seen positions filled with l 's
  an1the other f四깬岫呵s. There are C(7,『3) = 35 加誌茄le 的0rds in
  this code, and as with the 8-bit ASCII code, the van Duuren code permits
  the detection of many types of errors since the receiver knows exactly
  the number of l 's that should be in the received message unit of 卜even
 time slots.                                                                                              9) q/A뉘 1:）小WY뇨W 耐e\
        Another w沁ely used s血叩Ic code is th6口이玎＜f-5 code. As the
 name implies, two out of five positions are filled with l 's. In this code
 there are, very conveniently, exactly C(5, 2) = 10 possible symbols.
 One of the many ways of associating the code symbols with the numerical
  values of the decimal digits i sth力T247'thde, which is a weighted code
 where we ft h weights 0, 1, 2, 4, and 7 to the successive columns of
 the code. The corresponding decimal digit is the sum of the weights
 where the l 's occur, 빤h쁘쓰인트르뜨르만喚lth한쁘프廻bin쁘0旦土7
 坦畔en쯔으 The code is given in T的Ic比그 Again, any single error
 in i 而essage can be recognized because it will have an odd number of
  l 's in it.


 Exercises

 1.8-1 Table 1.8-2 is one assignment of number values to the 10 possible
       symbols of the 2-out-of-5 code; how many possible 2-out-of-5
       codes can there be?                                     Ans. l0t

                                                                 TABLE 1.8그   The 2-Oz吐＜J／万 Code

        0 1 2                                        4           7            Decimal                        Corresponds to:




                                                                                                                       20 l2




                                                     000lll000
                                                                 000000
                                                                                                                00l0
        l 1l 0




                                        l 0 0 l0 0
                  ］
                  上 0




                                                                                            U 6 m
                                                                                                / 8 O
                                                                                                    / 0                              二 4 4 4 m
                                                                                                                                             / m
                                                                                                                                               / m
                                                                                                                                                 / m
                                                                                                                                                   /
                                                                                  4
                                                                                  l n
                                                                                    乙 n1V 4
                                                                                          1 <                                    1 口 n
                                                                                                                                 i 3
        4




                  l 0 1
       工
       ］




                                  0 41l 1


                      l0 0 l0 0
                                                                                                                    l4

        00 l000                                                                                                             1d
                                                                 ］上

                                                                 dl
                             l
                             m
                                                                 4
                                                                 11

                                   0                 ll          mi
                                       Sec. 1.10 / Escape Characters      15

 1.8-2 Write 125 in the 2-out-of-5 code.
                                              Ans. 11000   10100       01010

 1.8-3 Of all possible 7-bit odd-parity symbols, how many are not used
       in the van Duuren code?                                 Ans. 29


1.9 Radix rCodes

 As noted earlier, most systems of representing information in computers
 (and other machines) use two states, although the Morse code is an
 example of a signaling system with three symbols in the underlying
 alphabet. The reason for the dominance oftwo-symbol signaling sys-
 tems is that two-state devices tend to be more reliable than multistate
 devices. On the other hand, human beings clearly work better with
multistate systems-witness the letters of the alphabet, together with
the various punctuation symbols and the decimal digits. Thus it is
necessary at times to consider codes with r symbols in their alphabets.
For the Morse code, r = 3.
      The English language alphabet uses 26 letters, both upper- and
lowercase, plus miscellaneous punctuation marks. Occasionally, you
see a system in which there are exactly the 26 letters, the 10 decimal
digits, and a space, a total of 37 symbols. We examine this important
code in Section 2.7.
      In more abstract notation we assume a source alphabet S consisting
of q symbols sl, S2, · · . , Sq. These are, in turn, represented in some
other symbols, say the binary code. We may, therefore, either think
of the ASCII code as having r = q = 27 = 128 symbols s1, S2, . . . ,
S128, or we may think of each symbol as being a block of 8 binary digits
with 1 extra bit appended to the 7 necessary bits.                    /


1.10 Escape（沇口r吼比rs

 When sending information it is usually necessary to control, from the
 source end, the remote equipment that is being used. For example, we
 have to tell the equipment what to do with the information that is being
 sent. Therefore, it is necessary to have a number of reserved symbols
 to which the remote equipment responds. "End Of Message" is such
 a symbol; another might be "Carriage Return"; another a "Shift Type
Font" from lower- to uppercase or back again; and still another might
be "Repeat Last Message." In the ASCII code the entire first column
of the table is devoted to special characters.
     How can this control be done if we do not wish to restrict the
information that can be sent through the system? If, for example, we
16    Ch. 1 / Introduction

were using binary digits as numbers in our message, how do we avoid
those combinations of bits that are control symbols for the remote equip-
ment? If by chance our stream of binary numbers happened to contain
such a reserved symbol, then the equipment would respond to the re-
served symbol when we did not want it to do so. Evidently, some kind
of restriction on what can be sent is necessary, but the question is: How
can this be done with the least pain to the user of the system?
      One way this could be done is to add an extra binary digit to each
block of digits, using, say, a 0 if it is message and a 1 if it is a control
instruction. As can be seen, this will waste a good deal of channel
capacity if the control words are rarely used. Furthermore, it does not
solve the problem of relaying control words through one piece of equip-
ment to another piece of equipment.
     In one form of FORTRAN, the aspostrophe (') is used to delimit
a string of characters. For example, the string of symbols ABC is written

                                  'ABC'

In the FORTRAN processing, the apostrophes are stripped off and the
string ABC emerges.
     If the string happens to contain an apostrophe, such as the string
FINNEGAN'S WAKE, you need to write

                        'FINNEGAN 'S WAKE'

The processing strips off the first of the pair but lets through the one
加imediat的／ f아lowing.
      To see how to write the underlying program of the FORTRAN
compiler, we use a (slightly extended) state diagram, which is widely
used in finite automata theory. Each state consists of READ NEXT
SYMBOL followed by WHAT TO DO. We have three states to con-
sider: (1) the normal state of processing FORTRAN text, (2) the usual
inside-the-string state, and (3) the inside-the-string state that looks for
an immediately succeeding apostrophe. The state diagram is shown in
Figure 1.10-1. If the system has more than one reserved symbol, slight
variations on this diagram will handle them.
      In the field of logic this problem is known as the metalanguage
problem: How does one talk about the language itself, especially when
one has to use essentially the same language to do the talking? In
practice we use voice accents (quote marks) to indicate that we are
 talking about the language itself, and we leave them out when we are
 merely talking. There are other formal devices for solving this common
 problem that arises in computer science and in other fields of information
                                   Sec. 1.11 / Outline of the Course   17

                                                                     Do
                                                                   normal
                                                                    thing




   Normal
    State                親                    Special
                                               State

                 Figure 1.10-1 Reserved symbol automata


handling and processing, and these may also be adapted to this common,
vexatious problem.
     In controlling a digital computer the failure to distinguish between
the various levels of metalanguages is a source of constant confusion.
A FORTRAN program and the instruction to COMPILE it are in dif-
ferent languages. A program requires two end marks, one for the
metalanguage level of COMPILE to indicate the end of the source
program and to stop the compilation process, and one for the FOR-
TRAN program to be used at RUN TIME to end the actual compu-
tation.


月工erc加e

1.10-1 Describe in detail how you would encode 'Help!' to get through
       the FORTRAN-type system described in the text.
                                                     Ans. "Help!"


1.11 Outline of the Course

We have introduced the main topics as well as a number of codes with
varying properties, and now have a basis for discussing the material the
course is to cover.
     In Chapters 2, 3, and 11 we look at ways of channel-encoding
information (messages, sources of symbols) so that any errors made in
going through a channel, up to a given level, may be detected and/or
corrected at the terminal end without recourse to the source. For a
18    Ch. 1 / Introduction

detected but uncorrectable error, we might call for a repeat of the
message, hoping to get it correct the next time. In general, the error-
detecting and error-correcting capability will be accomplished by adding
some digits to the message, thus making the message slightly longer.
The main problem is to achieve the required protection against the
inevitable errors (noise) in the channel without paying too high a price
in adding extra digits. This is encoding for the channel.
     In Chapters 4 and 5 we focus on source encoding. The compression
of messages is important for efficiency. In transmission through space
the shorter message will use the signaling equipment for a shorter time;
for storage problems less storage will be needed for the compressed
code. This is source encoding. In Chapters 4 and 5 we look at this
side of the problem and examine ways to reduce the amount of infor-
mation being sent. We do this by examining the structure of the mes-
sages being sent. When there is a great deal of structure in the infor-
mation being sent, a good deal of message compression can be achieved,
and hence greater efficiency results. Since there are so many properties
that messages can have which allow message compression, we can look
at only a few of the most common ones. We restrict our attention to
general methods and must neglect the many special, trick methods,
which are often fairly easy to invent.
     In Chapter 6 we introduce the central concept of the entropy of a
source of information and show how it is connected with the concept
of the maximum amount of information that can be sent through a given
channel. Thus we get a bit closer to the concept of exactly what in-
formation is. The first of Shannon's encoding theorems is for a noiseless
channel, and is fairly easy to prove. The second theorem, presented
in Chapter 10, discusses sending information through a noisy channel
and is much more difficult to prove. Fortunately, the simple binary
symmetric channel is the realistic case, and for this case the proof is easy
to understand. The proof in the more general case is more difficult,
and is only sketched.
     Shannon's two theorems set bounds on what encoding can accom-
plish. Unfortunately, the second of his theorems is somewhat noncon-
structive and does not tell us how in practice to achieve the bounds
indicated. The result is not useless since it indicates where we can
expect to achieve large improvements in a signaling system and where
we can expect at best only small improvements.
     The definition of a channel in information theory is often not a
practical one and we need other ways of assessing this central concept
of channel capacity for transmitting information. Therefore, Appendix
A looks briefly at how, in practice, we measure the channel capacity of
a signaling system, especially for continuous signals.
                                     Sec. 1.11 / Outline of the Course     19
       We remind the reader that while we often use the
                                                                 language of
 "signaling from here to there," all of it is applicable to
                                                            "signaling from
  now to then" through some storage medium. In this
                                                             case it is often
 the first of Shannon's theorems (the noise-free one)
                                                          that is important.
       Traditionally, the development of both coding and inform
                                                                   ation the-
 ory is done in as elegant and general a way as possi
                                                         ble-usually highly
 abstract, with many fancy mathematical symbols, and devoid
                                                                  of practical
 aspects. This approach is not necessary, and we regula
                                                           rlyFause to show
 how what we are talking about is reflected in comm
                                                           on sense and in
 actual practice, and how it suggests going about the
                                                           design of future
 systems. We also try to make the proofs of the results
                                                               as intuitively
 obvious as possible rather than merely mathematical
                                                        ly elegant. Along
 the way we introduce many small, practical details that
                                                              are important
 when designing a whole system.
      But let us be clear about the approach we are
                                                          adopting. When
there are so many different highly evolved and highly
                                                         involved signaling
systems now in use, and so many new ones over the immed
                                                              iate horizon,
it is impractical to take them up one at a time. It
                                                       is necessary to take
an overview approach and concentrate on the fundamenta
                                                               ls that seem
most likely to be relevant for understanding both
                                                      past and future sig-
naling systems. Indeed, this is the only reasonable
                                                          approach to any
rapidly changing field of knowledge. The approach throug
                                                                   h special
cases simply leaves the student surprised by tomorrow's
                                                            system. Thus,
of necessity, the treatment is, at times, abstract and avoids
                                                                many of the
messy details of current systems.
Chapter 2



                            Error-Detecting Codes
                                  깁
                               師小1m出명              Co丸
                                  日Yb.介0，航戍万回 훤 푸이               잭건좋이

                                   분此苞촁누 如진 사乷焉 ，以已 ！卄玄
                                   白1y也咤＼各이 1卜늉3卜叫中 芟t,.



2.1 Why Error-Detecting Codes?                                                 ,/r'

We first examine channel encoding. The problem is to design codes
that will compensate for the inevitable noise that is in all realistic chan-
nels. More and more often we require very reliable trans小如n throu합
the channel, whether it be through space when signaling from here to
there (transmission), or through time when signaling from now to then
(storage). Experience shows that it is not easy to build equipment that
is highly reliable. By "highly reliable" consider how much computing
a modern computer does in 1 hour. At one operation per microsecond
it does 3.6 billion (109) operations in 1hour (and each operation involves
many individual components). By comparison there are less than 3.16
billion seconds in 100 years (more than your probable lifetime). Sim-
ilarly, reliable transmission systems require very high reliability of their
 individual components. Reliability in the transmission of words of hu-
 man languages is one thing; for transmission of computer programs it
 is something else-hence the importance of detecting errors. Fur-
  thermore, as already noted, error detection is a great aid in high-quality
 maintenance. Without error detection, a large digital system soon be-
 comes unmaintainable.
     If repetition is possible, then it is frequently sufficient merely to
 detect the presence of an error. When an error is detected we simply
 repeat the message, the operation, or whatever was being done, and
 with reasonable luck it will be right the second (or even possibly the
 third) time (see Section 2.5).



 20
                                     Sec. 2.2 I Simple Parity Checks    21

      It is obviously not possible to detect an error if every possible
symbol, or set of symbols, that can be received is a legitimate message.
It is possible to catch errors only if there are some restrictions on what
is a proper message. The problem is to keep these restrictions on the
possible messages down to ones that are simple. In practice, "simple"
has in the past tended to mean "easily computable," but it could in the
future mean "easily looked up." In this chapter we investigate the
problem of designing codes such that at the receiving end, any single,
isolated error can be detected. In Chapter 3 we consider correcting at
the receiving end the errors that occur in the message.



2.2 Si刃zple Pa,立yC九ecks

 The simplest way of encoding a binary message to make it error detecting
 is to count the number of l 's in the message, and then append a final
 binary digit chosen so that the entire message has an even number of
 l 's in it. The entire message is therefore of even parity. Thus to
 (n - 1) message positions we append an nth parity-check position. At
 the receiving end the count of the number of l 's is made, and an odd
 number of l 's in the entire n positions indicates that at least one error
 has occurred.
       Evidently, in this code a double error cannot be detected. Nor
 can any even number of errors be detected. But any odd number of
 errors can be detected. If (1) the probability of an error in any one
 binary position is assumed to be a definite number p, and (2) errors in
 different positions are assumed to be independent, then for n much less
 than lip, the probable number of single errors is approximately np.
 The probability of a double error is approximately n(n 中 l)p2/2, which
 is approximately one-half the square of single error. From this it follows
 that the optimal length of message to be checked depends on both the
 reliability desired (the chance of a double error going undetected) and
 the probability of a single error in any one position,p. For more details,
 see Section 2.4.
       Counting the number of l 's and selecting an even numberis equiv-
르.1인｝t to working in a 刃1odu1o 2 口rithmetic. '斗呱d心必吃2" means that
 every number is divided by 2 (the modulus) and only the remainder i s
=ke匹. In this arithmetic (which counts 0, 1, 0, 1, . . .) we count modulo
 2 the number of l 's in the (n - 1) message positions and then put this
  sum into the nth position. Thus there are an even number of l 's in the
 n positions sent. 工h妊 ye끄叩旦r幻쏘加ck초genera끄yme괴끄-t뇨끄：                 出竝y.
 In practice, it is occasionally convenient to adopt an odd-parity check
  so that the message of all 0's is not a legitimate message. The changes
22    Ch. 2 I Error-Detecting Codes

necessary in the theory are sufficiently easy to make that we will continue
to use even-parity checks throughout the theory.
     To actually find the parity of a string of 0's and l's we can use a
two-state finite automaton (Figure 2.2-1). We start in the state 0, and
each 1 in the message causes a change in the state. The final state at
the end of the message gives the parity count.




                     Figure 2.2-1 Parity count circuit

     Many computers have an instruction that directly counts the number
of l's in the accumulator register. The right-hand digit of this sum is
the required count modulo 2. If this or an equivalent instruction is not
available, then logically adding (exclusive OR, XOR; see Section 2.8)
one half of the message to the other half preserves the parity count in
the sum. Repeated use of this observation halves at each step the length
of the message and will produce the required sum modulo 2 of all the
l's in the accumulator. Thus about "the first integer greater than or
equal to log2n" logical additions will be needed.


2.3 Error-Detecting Codes

It is common practice to break up a long message in the binary alphabet
into runs (blocks) of(n - 1) digits each, and to append one binary digit
to each run, making the block that is sent n digits long. The final block
may need to be padded out with 0's. This produces the redundancy of

                           n                1
                                  =   1+
                          n- i             n- i

where the redundancy is defined as the number of binary digits actually
used divided by the minimum necessary. The excess redundancy is
1I(n - 1).
     Clearly, for low redundancy we want to use long messages. But
for high reliability short messages are better. Thus the choice of the
                         Sec. 2.4 / independent Errors: White Noise     23

length n for the blocks of message to send for a given probability of
error p is an engineering compromise between two opposing forces.
    The 2-out-of-5 code mentioned in Section 1.8 is an example of an
error-detecting code with n = 5 that uses an even-parity check. The
van Duuren 3-out-of-7 code is another such code, but uses odd parity.
Neither uses all the symbols it could. A variant is the word count
occasionally used in sending telegrams.
    Many other examples of this simple kind of encoding for error
detection occur in practice. For example, when making a memory
transfer to tape, drum, or disk, the logical sum of all the words being
transferred can be appended as a check word. See Ref. [WJ for hard-
ware realizations.



2.4 Independent Errors: White Noise

We have already mentioned (Section 2.2) the model usually assumed
for errors in a message: (1) an equal probability p of an error in each
position, and (2) an independence of errors in different positions. This
is called "white noise" in (a poor) analogy with white light, which is
supposed to contain uniformly all the frequencies that are detected by
the human eye. The theory for this case is very easy to understand.
But in practice there are often reasons for errors to be more common
in some positions in the message than in others, and it is often true that
errors tend to occur in bursts and not be independent (a common power
supply, for example, tends to produce a correlation among errors; so
does a nearby lightning strike; see Section 2.6).
     It is only fair to note that due to the rapid pace of technological
change, it is not possible at the design stage to have much of an idea
 about the noise patterns of errors that will actually occur, so that white
noise is often a reasonable assumption.
     The probability of an error in any one position is p; hence the
probability of no error is 1 - p. From the assumed independence of
 the errors, that is, for white noise, the probability of no error in the n
positions is

                                 (1 - p)"

     The probability of a single error in the n positions is

                              np(1 - p）月中l
24       C/i. 2 / Error-Detecting Codes

The probability of k errors is given by the kth term in the binomial
expansion

1 = [(1 - p) + p1" = (1 - p)" + np(1 - p)" 寸1
                                                                               可
                                                                               " In' 小 1.
                                                                                                                                            .l                         ."fl        '2                              pfl"
                                                                                                                                                                                        +                     +
                                                                                                                                                             p)
                                                                                                                    '
                                                                                                                                                                               _
                                                                          +                      2
                                                                                                                                       '
                                                                                                                                           (.
                                                                                                                                                     -                                      ·   .         .

                                                                                       "
                                                                                                                              P
                                                                               "             '




For example, the probability of exactly two errors is

                                                                                                                                           2
                                         n
                                                  (n
                                                           -
                                                                                                                              fl
                                                                               P
                                                                                                                                   _
                                                                                   2
                                                                                                               p)
                                                                                       (1
                                                                                                 中

                                                           二
                                                                     1)
     We can get a formula for the probability of an even number of
errors (0, 2, 4, . . .) by adding the following two binomial expansions
and d如idin只 by 2:


            = [(1 - p) + 낀’1三 ．각 C(n, k)p"(l - p)"二 』叩界라．
                                                 尸m1                      1    17                          싸




               [(1 - p) - p1" = 2                                                      G 1)"C(n, k)p' (l - p)fl _ (
                                                                          k= O


(The [     ] in the next equation means "greatest integer in.")

             l1「
               +        .   -寸    2P n       )
                                                       =       [n/
                                                                          2]
                                   p)                                                                                                                                               2m
                   (l
                   (1
                                                       =
                                                                                                                        p2m
                                                                                                                                                                  p)
                                                                                                                                                                          4.
                                                                                       (n,
                                                                               C
                                                                                                                                                (l
                        乙
                                                                                                                                                         -
                                                                                                                                                                                                    (2.
                                                                                                                                                                                                              4-
                                                                                                                                                                                                                   1)
                                                               m= O
                                                                                                     2m)
The probability of an odd number of errors (which will always be de-
tected) is 1 minus this number.
     The probability of no errors is the first term (m = 0) of the series
(2.4-1). Therefore, to get the probability of an undetected error, we
drop the first term of (2.4-1), to get

                                 [n/2]

                                 2               C(n, 2m)p2m(1 - p)" H2m                                                                                                                            (2.4-2)
                                 m= 1


Usually, only the first few terms are of any importance in evaluating
this formula.

Exercises

2.4-1 If p = 0.001 and n = 100, what is the probability of no error?
                                                      Ans. exp (- 붊)
                                      Sec. 2.5 / Retransmission of Message    25

2.4-2 If p = 0.001 and n = 100. what is the orobabilitv of an undetected
            error?                    .            1        '!.,L .h. A
                     h1n느，A1小1   ＼丁'\71나卜   e\m／놔r니U=j   t/V也'乞八（노 ' e"나t '
                     八＼녀bn4引      9U "      ( ' "  1 二
2.4-3 If p = 0.01 and you want the probability of an undetected error
      to be 0.005, what is the maximum length n that you can use?
                                     Ans. n = 10 but almost n = 11

2.4-4 For small p and arbitrary n, do Exercise 2.4-1. Ans. exp (- np)
       //
  \,
2.5 Retrans刃ziss加n 可Message

When an error is detected, it is often possible to ask for a retransmission,
a recomputation, or repeat of the process being done. For example,
in the Bell Relay Computers the code used for representing the decimal
digits was a 2-out-of-S code, and whenever an error was detected, a
second, and even a third trial was made. On the Model 6 Relay Com-
puter, if after the third trial the message was still not acceptable, then
the whole problem was dropped and the next one taken up, in the hope
that the defective part would not be used in the new problem.
      When reading magnetic tapes it is the custom to use at least an
error-detecting code, and to call for repeated readings of the tape if the
parity checks are violated. How many repetitions to use depends on
your model for the error. If you think that the error is due to a slight
loss of magnetization, then with luck a subsequent trial will read the
tape correctly; but if you think it is due to a more permanent failure,
then repetitions will probably occur until another, independent error
occurs, so that then the parity check is met. You will therefore get a
message with two errors in it, rather than the right message! 11'hus the
strategy of "detect an error, and if one is9岬立 call for one or more
repetitions" is sound only if the type of르rror you expect is transient.
      Parity checks have long been used in computers, in both hardware
and software (Ref. [W]). For example, in the early days of unreliable
drum storage, every WRITE on the drum was followed by the logical
sum of all the registers that were used for the message being stored on
the drum. This check sum was then stored in a final register of the
block on the drum. The drum was next read back and checked to see
if the message was written properly. Only then was the information
being stored released from the machine's storage registers. When later
 the drum was read, the parity check (the logical sum of all the registers
being stored) was again computed to see if the sum was identically zero.
If not, retrials were made to read it again. This method depends on
 the fact that x + x = 0 for logical addition.
26     Ch. 2 / Error-Detecting Codes

2.6 Simple Burst Error-Detecting Codes

Noise (errors) often occur in bursts rather than in isolated positions in
 the received message. Lightning strikes, power-supply fluctuations, and
loose flakes on a magnetic surface are all typical causes of a burst of
n아se.
      Suppose that from measurements in the field we agree on the max-
imum length L of any burst we are to detect. For ease of discussion
(since the changes necessary to handle other cases are easy to invent)
assume that the burst length L is the accumulator word length of the
computer. We have only to select the appropriate error-detecting code
(or error-correcting code of Chapter 3) and instead of computing parity
checks over the bit positions, we compute parity word checks over the
corresponding word positions. In effect, we work in words, not bits,
and have L independent (interleaved) codes, one over each bit position
in the word (see Section 3.8). If a burst covers the end of one word
and the beginning of another, still no two errors will be in the same
code since we assumed that any burst length k was (0 5 k 5 L).
      Thus we can send messages through noise that is "bursty" provided
that we recognize the noise pattern and design for it. For reliable
hardware, see Ref. [W].

     Example. If the message is

                               Fall 1980

this can be encoded in ASCII in a burst code as follows (no parity check
is used here):


                    F a
                     = 106 = 01        000   110
                     = 141 = 01        100   001]
                   1= 154= 01          101   100
                   1= 154= 01          101   100
                  sp = 040 = 00        100   000
                   1 = 061 = 00        110   00띠
                   9 = 071 = 00        111   o0a\
                   8 = 070 = 00        111   000
                   0= 060= 00          110   000
                 Check sum = 00        000   111 = BEL

The encoded message is therefore

                            Fall 1980BEL

where BEL is the single ASCII symbol 00 000
            Sec. 2. 7 / Alphabet Plus Number Codes: Weighted Codes    27

Exercise

2.6-1 Given the message

                              101   01010
                              011   00110
                              000   11110
                              110   00110
                              111   10101

      add the appropriate check to form a burst error-detecting code
      of word length 1 byte.                        Ans. 111 00001



2.7 Alj坑abet Plus Nu刃zber Codes: .也뇨色加尸d rM口g

The codes we have discussed so far have generally assumed a simple
form of white noise. This is very suitable1量？r many types oL프laGhines,
although in serial transmission the loss of a symbol (or the insertion of
an extra one) is a common error in some systems, and is not caught by
such codes, hence causes a loss of synchronization.
     When dealing with human beings, another type of noise is more
appropriate. People have a tendency to interchange adjacent digits, of
numbers; for example, 67 becomes 16. A second common error is to
double the wrong one of a triple of digits, two adjacent ones of which
are the same; for example, 667 becomes 677, merely a change of one
digit. These are the two most common human errors in arithmetic.
In a combined alphabet/number system, the confusion of 'oh," and
"zero" is very common.
     A rather frequent situation is to have an alphabet, plus space, plus
the 10 decimal digits as the complete set of symbols to be used. This
amounts to 26 + 1 + 10 = 37 symbols in the sending alphabet.
Fortunately, 374욘꾸dme꾜mme1aD4JVe4;an1J＄旦世1町Q끄0쁘ing廻럇h쁘
趣프r쁘프匙C地ig We weig／玎 the syn伯아s with weights 1, 2, 3, · · ·
beginning with the check digit of the message. We reduce the sum
modulo 37 (divide by 37 and take the remainder) so that a check symbol
can be selected that will make the sum 0 modulo 37. Note that a "blank"
at the end, as a check symbol, is not the same as nothing.
     It is easy to compute that an interchange of adjacent digits will be
detected, and that doubling the wrong digit (which is the changing of a
single symbol) will also be detected. If the interchanged digits are the
kth and (k + 1)st, their original sum,
28    C/i. 2 / Error-Detecting Codes

becomes

                           (k + 1)sk + ksk+ i

and the change

        ks1, + (k ,+ l)sk+1 - (k + l)Sk - ksk+ j = Sk+1 - Sk
        ,；了，     亡    1     1 1        ,, ，七7/
cannot be dividel by 37 with a remainder 0 unless 5k = Sk + 1. A similar
argument applies to the interchange of any two digits, adjacent or not
(assuming a message length less than 37). Many other interchanges can
also be caught. The change of "oh" to "zero" is the change of a single
symbol. Such a code is very useful when human beings are involved
in the process. Notice that the length of the message being encoded is
not fixed, and can exceed 37 symbols if necessary (although special
precautions are then required). This type of encoding can be used on
credit cards, the names of some kinds of items in inventory, and so on.
The probability that a random encoding will get through the input check
is 多. Thus by using this simple parity check, forgery attempts will be
caught about 97% of the time.
     When the check symbol is the "space," this can sometimes be
awkward. If it is awkward, then frequently the whole label, say an
inventory name, can be dropped and a new label chosen in its place (a
loss of about 多 of the possible inventory names results).
     To 塑끄쁘뜨t얀世쁘C匙迷쁘쁘三雙好皿얏했甦立낸쁘f엣뽀ute
th르 runni프g sum아브흐竺으f끄끄프빤心s, and깔뺀쁘쁘迪，                  , 코g, " :  .l
                  number entered into the final sum n times, the next
nu而碗ni=a石硫S. 珏而next n - ）石而酉，言hd否o on, do而小o the last
number, which will get into the final total only once. Thus you have
血끄르믹唾姮끄貞앞4口i3쁘i of the numbers that correspond t야k Sym.-
bols of the alohabet being used.
     it tnis "summing tne sum" seems mysterious. consicer tne message
w x y z.'

       Message                      Sum                Sum of sum

          w                            w                    w
          工                        w +工                  2w + x
          y                       w+ x+ y             3w+ 2x+ y
          z                  w+ x+ y+ z             4w+ 3x+ 2y+ z


where we see the weighted sum emerging. This is sometimes known
as "progressive digiting."
              Sec. 2.7 / Alphabet Plus Number Codes: Weighted Codes                29

      Example. 110 = 0, 1 = 1, 2 = 2, . . . ,9 = 9, A = 10, B = 11,
. . . , Z = 35, bi = 36, then encode

                                                           A6 / 7

We proceed as follows:

                                                          Sum       Sum of Sum




                      A6M 7 工
                                                                        0    8
                                                           10



                                 色拍7 工
                                                             =




                                                                         6브n乙 m/
                                                           16=

                                                                        =l
                                                           52=



                                                           59=
                                                                       137
                                                         59 + ｛工／
                                                             =
                                                                     196 + 工




Since 11 + x must be divisible by 37, it follows that

                                         x = 37 - 11 = 26 = 0

The encoded message is therefore

                                                          A6 7O

To르迦드必 堡心뜨匈筵世빤女匹흐르쁘밈迦y起텍四쁘d끄ie邈的찐e
proceed as follows:
                                                         印


           A6 M 7 Q
                                                     4
                                10 )<
                                 6 x 4 = 24
                                                 4
                                36 x 3 = 108 3
                                 7 x 2 = 14
                                         2
                                26 x 1 = 26
                                  Sum = 222 := 37 )< 6 = 0 m이如幻 37

     The method of encoding used in this section is an example of en-
coding for human beings rather than for the conventional white noise.
We see how dependent the encoding method chosen is on the assumed
noise. It is necessary to emphasize this point because the theory so
often tacitly assumes the presence of white noise that the reader is apt
to forget this basic assumption when involved with an elegant, complex
code.
30    Ch. 2 / Error-Detecting Codes

Exercises

2.7-1 If0 = 0, 1 = 1. . . . .9 = 9, A = 10, B = 11. . . . .Z = 35,
      bi = 36, encode

                           B23F             mod 37

                                                                Ans. B23F9

2.7-2 In the same code as that of Example 2.7工 is

                                       K9K9
                                                      갸   r 1            乙
      a correct message?                                  J




                                                                         戶




2.8 Revie叩of Modular Ant九met加 （目：
                                《；k                  目？eK꺼한       宦녕 )
Because we are often going to use parity checks, we need to get a firm
grasp on the arithmetic of the corresponding manipulations. We have
seen that mod 2 addition ("mod" is an abbreviation for "modulo") is
the arithmetic that the simple binary parity checks use and is the same
as logical addition (exclusive OR; XOR). The rules for this form of
addition are

                               /0     + 0   =   0
                           /         0+ 1= 1
                           \ 1+ 0= 1
                                    \ 1+ 1= 0

There are no numbers other than 0 and 1 in the system. If we choose
to work in normal arithmetic, then we merely divide the result by 2 and
take the remainder. When we later come to the algebra of linear equa-
tions and polynomials, where the coefficients are from the mod 2 number
system, we will have the same table for addition. For multiplication
we have the rules

                                     0x0=       0
                                     oxl=       0
                                     1 乂 0 = 0
                                     lxl=       1

Th쁘쁘쁘啣心뜨唾姪丘뇨廷쯔p만姮艮
                              Sec. 2.8 / Review of Modular Arithmetic     31

      Occasionally, we will work modulo some other number than 2.
 For example, in the preceding section we used numbers modulo 37.
 (｝엣쁘旦ydb르쁘르으口i凹凹 以坦쁘흐쁘르끄 (such르므21프므曳y쁘뜨h血k드
 t蜘U江也a＄드2斗코II迫型르끄뜨d끄9t召Q上l翅t쁘쁘坐J브e. You have
 only to read the preceding paragraph and make simple changes to under-
 stand the corresponding arithmetic and algebra. For addition and sub-
 traction mod p, we divide every number by p and take the positive
 remainder.
      For multiplication mod m (not a prime) we must be more careful.
 Suppose that we have the numbers a and b congruent to a' and b' modulo
 the modulus m. This means that

                              a 三a'     modm
                              b =b '     modm
 or

                              a = a' + k1m

                             b = b' + k2m

 for some integers k1 and k2. For the product ab we have

                口b = a'b' + 口' k2m + b 'k1m + 自k批2

                口b = a小r     mod m

      Now consider the particular case

                    a= 15,        b= 12,         m= 10

We have

                        口' = 5,        b' == 2
and

                       口b 三 可b' 三三 0         modl0

跏毗：a nor b is四n轟激崙啓吻加加如峽血
we have the important vrovertv that if a vroduct is zero. then at least one
契莎갠竺三쁘으뇨 nence tne importance or a prime moauius. INOW ＼자e
see why 37 was so convenient a number in Section 2.7.
     Modular arithmetic should be clearly understood, especially the
need for a prime modulus, because in Chapter 11 we will face the
problem of constructing a corresponding modular algebra. In the next
section, we therefore give yet another example of this type of encoding.
32    Ch. 2 / Error-Detecting Codes

                                                        "「川
2.9 ISBN Bo仄 N刃兀bers                               睾딥！計빠
The International Standard Book Number (ISBN) now appears on most
textbooks. It is (usually) a 10-digit code that publishers assign to their
迦으坦 A typic 石oo而ill［下而ye



although the hyphens may appear in different positions. (The hyphens
are of no importance.) The 0 is for United States and some other
English-speaking countries. The 13 is for Prentice-Hall, the publisher.
The next six digits, 21-2571, are the book number assigned by the pub-
usher, and the final digit is the weighted checksum, as in Section 2.6.
Modulo 10 will n얌皿or뇨선쯔끄（쯔브으껜m塑으프쁘쁘二 갼쁘쁘잊
use the check sum     쁘끄l) and are fo.rced to allow,an X if the required
bhe乙ka恒正玉1可           5 nelore, mis coulo oe avoiueu Dy giving up i-i 01
the possible book names.
     Searching around, I found the ISBN

                                            0-1315-2447-X

To check that this number is a proper ISBN, we proceed as follows:




                   0l3l寸 2447
                                 4
                                 l 月
                                   냐 <
                                     U 0     l <
                                             d U




                            n世
                                       l
                                            10
                                            20

                           八／느 /
                               b 0 m/ m
                                      /
                                            32
                                            48
                            才
                            l 4l   느八
                                    乙 八
                                      4
                                      V     68
                                 ／
                                 八
             X                              95
                                           132 = (11) x (12) = 0 mod 11

It checks!
     Here again we see a simple error-detecting code designed for human
use rather than for computer use. Evidently, such codes have wide
applicability.
                                 Sec. 2.9 / ISBN Book Numbers   33

Exercises

2.9-1 Check the ISBN 0-13165332-6.

2.9-2 Check the ISBN 0-1391-4101-4.

2.9-3 Consider the ISBN 07-028761-4. Does it make sense?

2.9.4 Check the ISBNs in your current textbooks.
（沇叩ter 3



                          丑rror-Correcti兀g Codes




3.1 Need forE片t才 Correc作이7

For channel encoding, simple error detection with repetition is often
not enough. The immediate question is: If a computer can find out
that there is an error, why can it not find out where it is? The answer
is that by proper encoding this can, indeed, be done. For example, we
can write out, or do, each thing three times, and then take a vote. But
as we shall see, much more efficient methods are available. As an
example of the use of an error-correcting code, when information is sent
from space probes to Earth, the signaling time is so long that by the
time an error can be discovered, the source may long since have been
erased. The codes currently used are very sophisticated and can correct
many simultaneous errors in a block.
     Error correction is also very useful in the typical storage (memory)
system. Many organizations, for example, store much of their infor-
mation on magnetic tapes. Over the years the quality of the recording
gradually deteriorates, and the time comes when some of it cannot be
read reliably. When this happens, the original source of the information
is often no longer available and therefore the information stored on the
tape is forever lost. If some error-correction ability is incorporated into
the encoding of the information, the corresponding types of errors can
be corrected.
      Error correction has long been used and can be incorporated into
 the hardware. For example, the old NORC computer had a simple
 type of error correction for isolated errors that occurred on its cathode-



34
                                          Sec. 3.2 / Rectangular Codes     35

    ray-tube storage device. Often, it is only the storage device that uses
    the error correction. The STRETCH computer that IBM built "to
    stretch the state of the art" had single-error correction and double-error
    detection (Section 3.7) throughout much of the computer. On the
    STRETCH acceptance test it has been claimed that an error in a circuit
    developed in the first few minutes and that the error-correcting circuits
    fixed up the errors for the rest of the hour. Currently, most high-
    density magnetic recording uses some form of error correction, as does
   hi-fi digital recording of music. As the components get smaller, solid-
    state memories generally go to error-correcting codes. See Ref. [W]
    for hardware checking.
   .    , T匙旦犁三咀르逃曲珏雙旦剋lit工越9上足in. th쓰咬쁘쯔르프샐쁘쏘쯔
 ，屯솬쁘쁘9· We mentioned earlier that error-detection programs tor drum
 'sThrage were in the software. Error correction could also be used there.
   In many other places, correcting codes are built into the software. The
   software approach has the advantage that the error correction can more
   easily be put on the important parts of the information and omitted
   from the less important parts. Furthermore, only as experience reveals
   the weaknesses of the computer system is it known where error pro-
   tection is most needed as well as how much is needed. Only after
   simulation of error protection in software has proved that it handles the
   problem should it be added to the system in the form of hardware.
   However, error correction in software will clearly use a lot of computer
   血ne.


 \ 3.2 Redi口兀g뇨lar (而司
  The first, and simplest,..m江多Qr1르1江rng工刃de a心-the＝口字｛k啣小

  拌駑쁜
    ，援群曙｛퍅曜甲誓，芦，黑，썲크措鷺崙弩，裂
  isotatea singie errors. However, it is aiso oovious tnat mis encoaing
  system is very, inefficient. Three computers in parallel with the asso-
  ciated "compare and interrupt if necessary circuits" is expensive.
  Therefore, we look for better methods of encoding information so that




 蕪算發姦發藿
, or not the final corner bit is used has little importance; for even-parity
  checking, the parity sum of its row and its column are the same. Thus
36     Ch. 3 I Error-Correcting Codes

                                rn - i
                                  八




                                                          O O O 1 1 1 O X
                                                                            X X X
                        /
                                              1
                        O O O            I.
                                                  1

                                                  1
                                   .     .

                                                      .

                                                      S




                                   I      I   I




                            O = message position
                            x = check 四sit油n

                       Figure 3-2.1 Rectangular codes
                                                                                    多｛   )
the original code of (m - 1)(n - 1) bits of the rectafigle becomes an
array of mn bits. 가fJ쁘艸型yi카地竺匹르 1 十 1 (                           小 ) , IL
（艮：   끄土끄(p竺二1)佃二끄· For a                 멉yen  size mn,  the redundancy
쁘11 be smaller the more the rectangle approaches a s小1缸e. 』1인四쁘1e
（쁘竺으f亘d르兀 싸e hay르고L二D汕迦皿1唾orma如n and 2厦 -1上巨ts
of checking alone the sides.
尸Ai議而g痂fcode, for example, was the code that the NORC
computer used for its cathode-ray storage tubes. Rectangular codes
often are used on tapes (Refs. [B2], [W}). The longitulj ip?rity
checks are on the individual lines, and an extra line is put at " t1ie '杞 of
the block to form the vertical parity check. Unfortunately, the machine
designer rarely lets the user get at the parity-check information so that
by using suitable software programs the isolated error could be
corrected.



Exercises

 3.2.1 Discuss various possible rectangular codes for 24 message bits.

3.2-2 Discuss the use of the corner check bit. Prove that for even-
      parity checks it checks both row and column. Discuss the use of
      odd뽀延抑쁘뜨如 in this case.

 3.2-3 Compare an n2 code with an (n - 1)(n + 1) code.
               Sec. 3.3 / Triangu／口r, Cubic, 口nd 肛1갸mension口／ Codes                  37

 3.3 Triangu끄1乙 Cub屯 and n-I万刃zensional Codes



韓難薰韓囍囍茗轅越照衾
 O맺｝ro쁘쁘쁘四own col帥n（助땐吸 3.3기· Thus for a given size we



                                    0。 。j X        "
                                    o ohx
                                    o x
                                     x

                              Figure 3-3.1 Triangular codes

lower the redundancy we use. The triangular array of bits of infor-
mation has n(n - 1)12 bits with n bits added for the checks. Thus the
redundancy i亨1- + 2／伽 - 1).
    A triangular code of side n has
                                                               쨔쓰） .. 斗枇mA큭e
                   n(n - ] \                                       2.                \J



,When
 ,,,,we
     ,,c。
        ,m,,",'
           pare
              a"2 ,
                triangu
                    messa
                      c。dlareandn
                              with
                               geacheck
                                   square
                                     bitsc。d窄：
                                             e rf。,\,agiven
                                                      :,：牛t
                 ,1-
number of parity check-bits we find that the triangular code has more
message bits. We have included the cubic code in Table 3.3-1.

                  TABL丑 3.3-1 Con叩口rison 可T介肥e Cod뇨S
               Square                     Triangular                    Cubic
       Message     Check             Message Check              Message   Check
 n     (n- i)2     2n- 1            n(n - 1)/2 n              n3 - 3n + 2 3n - 2

  2        1              3               1         2              4             4
  3        4              5               3         3             20             7
  4        9             7                6         4             54            10
  5       16             9               10         5            112            13
  6       25            ii               15         6            200            16
  7       36            13               21         7            324            19
  8       49            15               28         8            490            22
  9       64            17               36         9            704            25
 10       81            19               45        10            972            28
        38     Ch. 3 I Error-Correcting Codes

            Once we have found a better code than the simple rectangular ones,
        we are led to ask the question: What is the best that we can do with
        respect to keeping down the redundancy? For a cube we can check
        each plane in three dimensions (Figure 3.3-2) by a single bit on the

)C 欌껀却 貞 꽝루．

  한 섟幽 아YDT外 난촁무

 = 선毛 咤러七 서！ 꺼e1
  털면디        伊毗 I,＼土"＼이如

  ,/引칵 핫嶝．


              Figure 3-3.2 Cubic code, showing only One plane and its check
              position


        corresponding edge. The three intersecting edges of check bits use
        3n - 2 positions out of the n3 total positions sent. The excess redun-
        dancy is roughly 3/n2 extra bits,
            If the use of three dimensions is better than two dimensions, then
        would not going to still higher dimensions be better? Of course we
        쁘끄뜨프쁘마으越쁘g약he bits 쁘t旦뜨띤如en針onal 아 higher sp쯔드
        we only imagine them so arranged to calculate the p p p y ecks.
        A在d츰而6面r5疝雨瓦而gover t1百ihiee-dimensional pl5ies in
        four-dimensional space will lead to (approximately) an excess redun-
        dancy of 4/n3. We soon come to the conclusion that the highest possible
        dimensional space might be the best, and we want a total of 2" bits of
        which (n + 1) are checks (one check in each direction plus the common
        corner bit). There would be, therefore, (n + 1) parity checks. .If坐y
        were suitably arran으ei in some order, then they would give a number
        called the syndro／兀e, which wE而而何繭l函誌示在；                  兀而面료；
        of a parity check, or a 0 when it is satisfied. These (n + 1) bits form
        an (n + 1)-bit number, and this number (the syndrome) can specify any
        of 2n +l things-more than the 2" locations of the corresponding single
        error plus the fact that no error occurred. Notice that the check bits,
        as in the simple error-detecting codes, are equally protected with the
        message bits. All the bits sent enter equally-none is treated specially.
             However, we see that there are almost twice as many states in the
        syndrome as are needed to indicate when the entire message is correct
        plus the position of the error if one occurs. Thus there is almost a
                            Sec. 3.4 I Hamming Error-Correcting Codes       39
   factor of 2 in the loss of efficiency. Nevertheles
                                                      s, this suggests a new
   approach to the problem of designing an error-corfec
                                                            ting code, which
   we take up in the next section.


  Exercises

  3.3-1 Make a triangular code of 10 message
                                                    positions.

  3.3-2 Discuss in detail the four-dimensional 2 x
                                                        2 x 2 x 2 code.

  3.3-3 Compare the three codes of Table 3.3-1
                                               that use approximately
        10 check bits.




 3.4 Hamming Error-Correcting Codes

 In this section we adopt an algebraic approach to
                                                   the problem that was
 started in the preceding section-finding the best
                                                    encoding scheme for
 single-error correction for white noise. Suppose that
                                                        we have m inde-
 pendent parity checks. By "independent" we mean,
                                                       of course, that no
 sum of any combination of the checks is any other
                                                      check-remember
 that they are to be added in our modulo 2 numbe
                                                    r system! Thus the
 three parity checks over positions

                    Check 1:      1,   2,   5, 7
                          2:                5, 7,    8, 9
                          3:      1夕   2,            8夕 9

 are dependent checks since the sum of any two rows
                                                          is the third. The
 third parity check provides no new information over
                                                            that of the first
 two, and is simply wasted effort.
      The syndrome which results from writing a 0 for each
                                                                   of the m
 parity checks that is correct and a 1 for each failure can be viewe
                                                                        d as
느an rn-bit number and can represent at most 2m
                                                      things. We need to
 represent the state of all the message positions being
                                                           correct, plus the
 location of any single error in the n bits of the message.
                                                              Thus we must
have the inequality

                                2m 之 n + 1                           (3.4-1)
    Can such a code be found? We will show how to
                                                     build ones that
exactly meet the equality condition. They repres
                                                 ent a particular so-
 40     Ch. 3 I Error-Correcting Codes

 lution to the problem of designing a suitable code and are known as
 丹a中州袖zg code孚    ．
      江뇨보m批디1山denying上len꾜f止嗅}翅끄끄끄竝gj9血主브빤쓰드흐쁘
 과ome소뇨끄-g竝ethe코elu皿-I：山S也Qn- 뇨沮lion)꾜I皿世르rr얀』                  －브世뽀四브
in the_synlrome meaning no error4. What positions should the parity
 checks use? Let us look at the binary representations of the position
 numbers (Table 3.4-1). Evidently, if the syndrome is to indicate the
 position of an error when it occurs, every position that has a 1 in the
 last position of its binary representation must be in the first parity check
 (see the extreme right-hand column of the table). Think carefully why
 this must be true. Similarly, the second parity check must be tripped
 by those positions that have a 1 in the second-lowest position in its
 binary representation; and so on.


                            TABLE 3.4-1 Check Positions
                      Position                       Binary Representation




                          ll 八
                             乙 n4V 4 =\V 6 m
                                           / 8 O
                                               / 0




                           1 1 1




       Thus we see that the first parity check covers positions 1, 3, 5, 7,
  9, 11, 13, 15, . . . ; the second, 2, 3, 6, 7, 10, 11, 14, 15, . . . ; the third,
  4, 5, 6, 7, 12, 13, 14, 15, . . . ; the next, 8, 9, 10, 11, 12, 13, 14, 15, 24,
  25, . . . ; and so on.
       To illustrate what we have just said (see Table 3.4-2), let us design
  a simple error-correcting code for four binary digits. We must have
  2" 之 n + 1 and we easily see that 23 之 (4 + 3) + 1 = 8. Therefore,
  we will need to have m = 3 parity checks, and this gives 7 = n = total
. of 毗ssage 이小 par泗小eck p匹쁘쁘느 The po師毗 to use to set the
  parity checks will for convenience be picked as 1, 2, and 4. Thus the
  information message positions are 3, 5, 6, and 7.
                             Sec. 3.4 / Hamming Error-Correcting Codes                        41

         TABLE 3.4-2 Encoding a 4-Bit Message and Locating Error

         Encode
             1 2 3 4 5 6 7                                           Position
              -- 1 - 0 1 1                                           Message
              0 1 1 0 0 1 1                                          Encode
                  x                                                  Error
              0 1 0 0 0 1 1                                          Receive

          Locate error                                           V
                                                                 <
                                             7 l7l7l =




                                   l d
                                     1 0 0
                             4
                             l 0 n
                                 乙 4         n4V 0 n4口 0 <
                                                         U 0 4
                                                             l
            Check 1
                                                                     Fails -'   1

                                               0 6l6 l
            Check 2
                                                                     Fails -*   1
            Check 3
                                                      l
                                                      ]
                                                                     Correct -p 0
          Syndrome                                                   3 -p position of error
          Correct (add 1 into the error position)
                     1                   Correct error
               0   1l
                         l
                         0 0 1 1         Corrected message


     To encode the information message, I write the message in the
positions 3, 5, 6, 7 and compute the parity checks in positions, 1, 2, 4.
Let this message be, say, __1_011; the spaces are where the parity checks
are to go. The first parity check, which goes in position 1, is computed
over positions 1, 3, 5, 7, and looking at the message I see that position
1gets a 0. I now have 0_i_Oil. The second parity check, over positions
2, 3, 6, 7, sets position 2 as a 1. I then have Oil_Oil as the partially
encoded message. The third parity check is over positions 4, 5, 6, 7,
and looking at what I have, I see that position 4 must get a 0. Thus
the final encoded message is 0110011.
     To see how the code corrects an isolated error, suppose that when
the message 0110011 is sent, the channel removes the 1 in the third
position from the left. The corrupted message is then 0100011. For
the receiving end, you apply the parity checks in order. The first, over
positions 1, 3, 5, 7, evidently fails, so the lowest-order digit of the
syndrome is a 1. The second parity check, over 2, 3, 6, 7, fails, so the
second digit of the syndrome is 1. The third parity check, over 4, 5,
6, 7, succeeds, so the highest-order digit is a 0. Looking at the syndrome
as a binary number, you have the decimal number 3. Thus you change.
(logically add 1) ;he symbol in position 3 from the received 0 to a l .
The resulting sequence of 0's and l 's is now correct, and when you strip
 42    C九 3 / Error-Correcting Codes

  off the checking bits 1, 2, and 4, you have the ori只inal information
. mess口ge 10끄 in 까)缸加'is 3, 5, 6, 口nd 7.
       Note that the check positions are equally corrected with the message
  positions. The code is uniform in its protection; once encoded there is
 ,no d끄erence between themegge and the check digits. The cute part
  of the Hamming code is the numerical ease of both the encoding and
  the code correction based on the syndrome at the received end. Also,
  note that the syndrome indicates the position of the error regardless of
  the message being sent; logically adding a 1 to the bit in the position
  given by the syndrome corrects the received message, where, of course,
  the syndrome "all 0's" means that the entire message has no errors.
       The redundancy in the example of four message bits with three
  check bits seems high. But if we took 10 check bits, we have, from
  equation (3.4-1), 210 5 10 + message positions + 1, or 1024 - 11
  = 1013 之 message positions. This shows that the excess redundancy
 rises like log2 of the number of message positions.


月工ercises

3.4-1 Discuss the Hamming code using four checks.

3.4-2 Discuss the Hamming code for two checks. Ans. Triplicate code

3.4-3 Show that 1111111 is a correct message.

3.4-4 Correct 1001111 and decode.          . . ,
                                          O\ t I
                          \/'vv    V
3.4-5 Locate the error in 011100010111110, where we have used four
      checks as in Exercise 3.4-1. What is the correct message?

方.4而. What is the probability that a random sequence of 2" - 1 0's and

  '" l 's will be a code word? , ,.,M止 (,i "                    Ans. 1/2"
3.5万q岫alent Codes

The example above is one way of encoding a message. There are many
other equivalent codes. It should be obvious that any interchange of
the positions of the .code will leave us with a code that is only trivially
different. Similarly, if we were to complement (change 0's to l 's and
l 's to 0's) all the digits appearing in a certain position, then again we
would have a trivially different code.
                                           Sec. 3.5 I Equivalent Codes   43

      We can, if we wish, use this observation about the interchange of
 positions to move all the check bits to the end of the message (see Figure
 3.5-1). For the arrangement we have the permutation

                  H                           <
                                              1V
                  +
                         H                 /0

                         H                 m
                                           11

                         H                /
                                          m

                         H                 / n乙

                        H                  n
                                           AU

                        H                  4
                                           1




                                                       0@ @
                                                   判
                                                            3   5   7
                                                   批
                                                          3 6       7
                                                   招
                                                          5 6       7

                      Figure 3-5.1 Hamming code positions
 Of course, the syndrome that emerges must also be changed by the same
 table. This permutation makes the "masking" of the message to get
 the parity checks, and to make the correction, less simple in appearance,
 but it is exactly the same amount of work by the computer, since for
 each check bit we still mask the received message to get the check bit
 by the "parity sum." Where we p垣ce the check bit is also changed.
 Although the meaning of the syndrome has its position changed, the
 syndrome is still essentially the same and refers to a unique place. The
position to logically add the correcting bit is therefore changed, but that
can be found either by a fo好llula or by a table lookup, which enters the
 table with the syndrome, and the entry in the table is the word with a
1 in the position to be corrected. Of course, for a long code a message
might be two or more words long. The table size is proportional to n.
The original Hamming code used computing power rather than table
lookup, and, in general, for very long codes this is necessary.
      One advantage of putting the check bits at the trailing end rather
世췐브唾世뽀ed throughout the message is.th Ls江tingDn the eiwnded'
me g          g e the same result as on the original messages
      As an alternativi to decoding a message, you could, in these days
of cheap, large memories, simply use the message as the address and
look up the encoded message. Similarly, the encoding process could
be a table lookup using addresses as long as the message of the encoded
44     Cli. 3 / Error-Correcting Codes

block. Such methods, being rapid, tend to emphasize short blocks with
higher redundancy than the more elaborate process of encoding (as given
above), which works on arbitrarily long messages (although, of course,
the longer the message, the more parity checks must be computed-in
parallel if you have the available equipment).


Exercise

3.5-1 In the n = 15 code, discuss in detail the encoding and decoding
      if the four parity checks are moved to positions 12, 13, 14,
      and 15.


3.6 Geometr初 Appr야iC九

  We have just given an algebraic approach to error-correcting codes.
  A diffe뢰lt. equivalent approach to the topic is from n-dimensional
. g ometry. In this model we consider the string of n 0's and l 's as a
  point in n-dimensional space. Each digit gives the value of the corre-
  sponding coordinate in the n-dimensional space (where we are assuming
  that the encoded message is exactly n bits long). Thus we have a cube
  in n-dimensional space; each vdrex is a string of n 0's and l 's. The
  space consists only of the 2" vertides; there is nothing else in the space
  of all possible messages except the 2" vertices. This is sometimes called
  a "vector space."
        Each vertex is a possible received message, but only selected ver-
  tices are to be original messages. A single error in a message moves
  the message point along one edge of the imagined cube to an imme-
  diately adjacent point. If we require that every possible originating
  message be at least a distance of two sides away from any other message
  point, then it is clear that any single error will move a message only one
  side away and leave the received message as an illegitimate message.
  If the minimum distance between message points is three sides of the
  텔b드北브l叩yin日e error will leave the recei代旦끄뜨흐5旦g르고으프r to the
  priginal message than to any other message and thus we can have single
   ew）工工：Orrection,
        Effectively, we have introduced a distdnce functipn. which is the -,
  minimum number of sides of the cube we have to traverse to get from
   one point to another. This is the same as the number of bits in the ,
   representations of the two points that differ. Thus the distance can be
   looked on as being the number of l 's in the logical difference, or sum,
   of the two points. It is a legitimate distance function since it satisfies
   the following three conditions:
                                         Sec. 3.6 / Geometric Approach      45

     1. 工he뇨dista꾜ce;froina꾸oiU玉拓8eit4昏0年
     2. . The distance from point x to point y is the same as the distaiice
          ft묘w. y to 工 agd is a positive nu好血弘．
     3. The triangle ineaualitv holds-the sum of two sides (distance
          rrom a to c pius mle aistance rrom c 10 0)_is at ieast as great as
       ,the length of the third side (the distance from a to b).

This distance function is usually called the Hamming distance. It is the
 listance function for binary white noise.
      Using this distance function, we can define various things in the
space. . In particular, the sur口ce of a sphere about a point is the set of
points a given distance away. The surface of sphere of radius 1 about
the point (0, 0, 0, . . . , 0) is the set of all vertices in the space which
are one unit away, that is, all vertices that have only one 1 in their
coordinate representation (see Figure 3.6-1). There are C(n, 1) such
points.


                             (1, 1, 0)




                                                       (0, 1, 1)


                  (0, 00)                (0, 0, 1)
     Figure 3-6.1 Three-dimensional spheres about (0, 0, 0) and (1, 1, 1)



      We can express the minimum distance between vertices of a set of
 message points in terms of the error correctability possible. Themn-
 imnm distance must be at least 1 for uniqueness of the code (Table
 3.6-1). A minimum distance of 2 gives single-error detectability . A
 minirnuii,i奴弘及툐占在,3gives 針ngle七rr야 correctability; any 釘n의e error
 leaves the point closer to where it was than to any other possible mes-
.' ag   Of course, this minimum-distance code could be used instead for
 double-error detection. A minimum distance of 4 will give both single-
 c 아르oiretion plus double-error detection. A minimum distance of
 5 would allow double-error correction. Conversely, if the required de-
46      Ch. 3 / Error-Correcting Codes

                     Ti 月4上 t 今1 Mean虹可Mi, 山num就S呻

                Minimum
                Distance   Meaning

                           Uniqueness
                    n乙
            /              Single-error detection
                    n
                    4U
            r
                           Single-error correction 白戶如岫I吐xrar
                            념ee蜘叫91
            i
            1
                    4      Single-error correction plus double-error
            1
            1
                             detection (or triple-error detection)
                    5毗
            1
                           Double-error correction
                \
            \
                \
                                                    ,   ..ur’的                     ，「'W   '




gree of detection or correction is to be achieved, the corresponding
minimum distance between message points must be observed.
     In the case of single-error correction with the minimum distance of
3, we can surround each message point by a unit sphere and not have
the spheres overlap. The volume of a sphere of radius 1 is the center
plus the n points with just one coordinate changed, a volume of 1 + n.
The total volume of the n-dimensional space is clearly 2P?, the number
of possible points. Since the spheres do not overlap, the maximum
number of mPssage positions k must satisfy

              Total \／아山iie
                             ；之miximnm number of snheres
           Volume of a sphere
                                                                       스   ,   .




or


                                                  介
                                                               下뇨，
Since

                              r n =m『D
                              2m+ ' 之 2' (n + 1)
or
                                 2' ' 之 (n + l)

This is the same inequality as we derived from the algebraic approach,
equation (3.4-1).
  Sec. 3.7 / Single-Error-Correction Pl比f Double-Error-Detection Codes    47

      We can now see the restrictions for higher error correction. Thus
 for double-error correction we must have a minimum distance of 5, and
 we can put nonoverlapping spheres of radius 2 about each message
 position. The volume of a sphere of radius 2 is the center position plus
 the n positions a distance 1 away, plus those with two coordinates out
 of the n changed, which is the binomial coefficient C(n, 2) = n(n - 1)!
 2. Dividing the total volume of the space, 2", by the volume of these
 spheres gives an upper bound on the number k of possible code message
 positions in the space



                      11+n二뇨크                                        (3.6-2)


 It does not mean that this number can be achieved, only that this is an
 upper bound. Similar inequalities can be written for larger spheres.
      When the spheres about the message points completely exhaust the
 space of 2' points, leaving no points outside some sphere, the code is
 called a perfect code. Such codes have a high degree of symmetry (in
 the geometric model each point is equivalent to any other point) and a
 particularly simple theory. In only a comparatively few cases do perfect
 codes exist. They require that the inequalities be equalities.


 Exercises

 3.6-1 Extend the bounds of (3.6-1) and (3.6-2) to higher error-correcting
       codes.

 3.6-2 Make a table for the bound for double-error correction of equation
       (3.6-2) (n = 3, 4, 5, . . . , 11).


 3.7 Single-Error-Correction Plus
     Double万rror-Detect勿n Coi加S

 It is seldom wise to use only single-error correction, because a double
 error would then fool the system in its attempts to correct, and the
 system would use the syndrome to correct the wrong place; thus there
 would be three errors in the decoded message. Instead, a single-error-
 correction plus a double-detection code makes a reasonably balanced
 system for many (but not all) situations. The condition for the double
,detection is that the minimum distance must be increased by 1; it must
 be 4.
          48     Ch. 3 / Error-Correcting Codes

        To make a double-error-detecting code from a single-error-
  correcting code, we add one more parity check (and one more position):
  this check is over the whole message. Thus any single error will still
  produce the right syndrome and the added parity check will give a 1.
  A double error will now cause a nonzero syndrome, but leave this added
, parity check satisfied. Fhis situation can then be recognized as a double
  error; namely, some syndrome appears, but the extra parity check is
  still correct (Table 3.7-1). It is easy to see that two points which were




            (./。
               \。
               S。
                Sy
                On
                me'"二”ndr
                    ginthin卜alomg 뇨e ，.
                  Something
                                       0 l0
                                       ld
                                        0          ,D빤쁘쁘뜨


          at the minimum distance of 3 from each other in the original code had
          a different number of l 's in them, modulo 2. Thus their corresponding
          extra parity che르k立브쁘世上르소竺코進트인世y, increasing the distancc
          between them to 4.
               The argument we have just given applies to both the algebraic and
          geometric approaches, and shows how the two tend to complement each
          other. We have not yet given any constructive method for finding the
          higher error-correcting codes; we have only given bounds on them.
          Chapter 11 is devoted to the elements of their construction. The full
          theory for error-correcting codes has been developed over the years and
          is very complex, so we will only indicate the general approach.
               Notice that the theory assumes that the correcting equipment is
          working properly; it is only the errors in the received (computed) mes-
          sage that are being handled.



          月．rercise


                      that
          \/    to any ouuthe argument to
                           minimum oistance extra error           can applied
                                             to get m1le next-nlgner (evenJ mmll-
(三1Show
                                            get
                                                         detection
                                                                      be
                imum distance.
                                  Sec. 3.9 I Applications of the Ideas    49

3.8 Hamming Codes Using Words

 On many computers it is difficult to get at the individual bits of infor-
mation, but the computer words are readily available. We can therefore
 think of the parity checks as being whole words; we logically add, not
bits, but words. The logical sum over all the selected words plus the
check should give a word with all 0's, and any failure marks the failure
 of the parity check. If we have, for example, a single-error-correcting
code, then we get the location of the wrong word and can reconstruct
it easily by, if nothing else, looking at the bits of the parity checks. It
 should be clear that we could simply add the parity-check failure word
to the word in the location of the erroneous word to get the correct
word. In this fashion we can correct the errors in any one word, whether
it is one, two, . . . , or all the bits of the word that are wrong.
      A mixed system results when you use the parity check on the ASCII
code bits. The ASCII parity check locates the word with the error and
the single-error-detecting parity word over all the words gives the po-
sition in the word that is wrong. Again, you simply add the parity check
to the word that is wrong to do the correction. This amounts to a
rectangular code. It will correct any odd number of errors in a single
word.


3.9 Applica在ons of the Ideas

In Section 1.2 we claimed that not only were the ideas in the text directly
useful but they also had wider general application-we used evolution
as an example.
     The central idea of error detection and correction is that the mean-
ingful messages must be kept far apart (in the space of probable errors)
if we are to handle errors successfully. If two of the possible messages
are not far enough apart, one message can be carried by an error (or
errors) into the other, or carried at least so close that at the receiving
end we will make a mistake in identifying the source.
     In assigning names to variables and labels in a FORTRAN, COBOL,
ALGOL, Pascal, Ada, and other high-level language, the names should
be kept far apart; otherwise, an intellectual "slip of the pen" or a typical
error in keying in the name can transfer one name to another meaningful
name. If the names are made to differ in at least two positions, single
typos will be caught by the assembler. Thus the use of short mnemonic
names should be tempered by the prudent need to protect oneself against
small slips.
50    Ch. 3 I Error-Correcting Codes

     If you estimate the time to locate an error in miswriting a name
against the time to add one or more characters to all the names while
writing the original program, you will see that using longer-than-mini-
mum names is probably a very wise idea-but it is unlikely that this
computation will convince many people to do so! Minimal-length names
are the source of much needless confusion and waste of time, yours and
the machine's.
     The distance function in the Hamming codes is based completely
on white noise. Sections 2.7 and 2.9 are included to emphasize that
the proper distance function to use depends in some cases on the psy-
chological distance between the names as well as more uniformly random
keystroke errors.


3.10 Su刃1刃wry

We have given the fundamental nature of error detection and error
correction for white noise, namely the minimum distance between mes-
sage points that must be observed. We have given methods for con-
structing codes for:

Single-error detecting                                 mmn. dist.    = 2
Single-error correction                                mmn. dist.    = 3
Single-error correction + double-error detection       mm1l. dist.   = 4

     Their design is easy, and they are practical to construct in software
or in hardware chips. They can compensate for weak spots in a system,
or can be used throughout an entire system, to get reliable performance
out of unreliable parts. One need not put up with poor equipment
performance, but the price is both in storage (or time of transmission)
and equipment (or time) to encode and possible correct. You do not
get something for nothing! The codes also make valuable contributions
to maintenance since they pinpoint the error, and the repairmen will
not try fixing the wrong things (meaning "fix" what is working right and
ignore what is causing the error!). A more widespread use of the idea
of distance between messages was sketched in Section 3.9.
     The use of such codes, and more highly developed codes, is rapidly
spreading as we get faster and smaller integrated-circuit components.
Increasingly, in VLSI (very large system integration) chips the code is
part of the hardware.
（沇a까er4




                           Variable-Length Codes.
                                          月虹加an Codes




4.1 Introduction

 We now turn to the topic of source encoding. The codes we have looked
 at so far have all used a fixed length, and they are called block codes
 from the fact that the messages are of fixed block lengths in the stream
of symbols being sent. The Morse code mentioned in Chapter 1- is an
example of a variable-length code, and we now examine variable-length
codes in more detail. The advantage of a code in which the message
symbols are of variable length is that sometimes the code is more efficient
in the sense that to represent the same information we can use fewer
  igits on the average. To푠666 plish ti뉵, we need to know something
  bout the statistics of the messages being sent. If every symbol is as
likely as every other one, then the block codes are about as efficient as
any code can be (see Section 4.6). But if some symbols are more
probable than others, then we can take advantage of this to make the
most frequent symbols correspond to the shorter encodings, and the less
frequent symbols correspond to the longer encodings. This is exactly
what the Morse code does. The letter E in the English language occurs
most frequently, and corresponds to the encoded symbol "dot."
      However, variable-length codes bring with them a fundamental
problem: At the receiving end, how do you recognize each symbol of
the code? In a binary system, for example, how do you recognize the
end of one code word and the beginning of the next? If the probabilities
of the frequencies of occurrence of the individual symbols are sufficiently




                                                                        51
52   Ch. 4 / Variable-Length Codes.' Huffman Codes

different, then variable-length encoding can be significantly more effi-
cient than block encoding.
     In this chapter we take advantage only of the frequencies of oc-
currence of the individual symbols being sent, and neglect any larger
structure the messages may have. An example of a slightly larger scale
structure is the fact that in English the letter 0 is usually followed by
the letter U; in Chapter 5 we take advantage of such correlations in the
message being sent.

Exercise

4.1-1 List advantages and disadvantages of variable-length codes.


4.2 Unique Decoding

We need to make clear when we are talking about the symbols to be
sent and when we are talking about the symbols used by the signaling
system. We will refer to the source symbols when we refer to the
symbols (such as the letters of the En믿ish alphabet) that are to be sent,
and to the code's alphabet when we refer to the symbols used in sending
(such as 0 and 1 in the binary system). In general, we will assume that
the source alphabet being sent has q symbols, sl, s2 . . · , s, , and that
the code's alphabet has r symbols (r for the radix of the system).
     The 如st property th카 we need is胛蜘eiJec갸I砬可匈-the rece毗d
message must have a single, unique possible interpretation. Consider
a code in which the source alphabet S has four symbols, and they are
to be encoded in binary as follows:

                                 Si = 0

                                 S2 = 01

                                 S3 = 11

                                 S4 = 00

The particular received message 0011 could be one of these two:



                            0011出4,
                                  1, S3 :, 51,
Thus the code is not uniquely decodable. Although this property of
unique decodability is not always absolutely essential, it is usually highly
desirable.
                                               Sec. 4.3 / Instantaneous Codes        53

       To get our thoughts clear, we make a formal definition:

     Definition. The nth extension of a code is simply all possible con-
catenations of n symbols of the original source code.
   0다．
     賈．m.／乙斗＼
      This is also called the nth direct product of the code. There are q'
symbols in the nth extension. The definition is necessary because the
mes g I send look to you, the receiver as concatenations of the
encoded symbols of the source alphabet, .and y need to decide which
sequence of source symbols I sent. 促or뇨nique decodabilityt no two
encoded concatenations can be the same, even for different extensions. )
Clearly, only if every distinct sequence of source symbols has a corre-'
spondiiig encoded sequence that is unique can we have a uniquely de-
codable signaling system. This is a necessary and sufficient condition,
but it is hardly usable in this form.


Exercises       ,   I        I tv-ti.:긔‘ L\    \\
                f   노＼'t勺 1 ' "                hn\
4.2-1 Is the code 0, 01, 001, 0010, 사11)uniquely decodable?

4. 2 Is the code
  2-                    0,   01, oii,   通     uniquely decodable?


                                                     0多姓.1
4.3 Instantaneous Codes
                                                     r1,, L,可 I.    .    L石    한
C。nsider計出，；曾，낢ife：許뗘」
                                                                         1k1              \
                                                    毖I'k   d七加d／名이
                                                                                Me
                                                                                          /
                                        Sl= 0

                                        S2 = 10

                                         53 = 110

                                         54 = 111

Now consider how you as the receiver would decode messages sent in
this code. You would set up what is equivalent to a finite automaton,
or if you prefer, a decision tree. Starting in the initial state (Figure
4.3-1), the first binary digit received will cause a branch, either to a
terminal state s1 if the digit is 0, or else to a second decision point if it
is a 1. For the next binary digit this second branch would go to the
terminal state S2 if a 0 is received, and to a third decision point if it is
a 1. The third would go to the terminal state s3 if the third digit is a
0, and to the terminal symbol s4 if it is a 1. Each terminal state would,
  54      Ch.    4 / Vari功le工ength Code오‘ Hu丹man C아加S


                                                                      o(Si
                                                                             =
                                                                戶2 =10
                                                                  3          :   ],
                                                                                      ],
                                                                                           0,
       Initial state
                                                                 ]S,
                                                                I14 -




   小忘，砂
                       缸孤기） ,,{.( 小小b '
                \        //
                   까pure 小3.1 Decodii坦 tree
         ；加，,。1( 上叩f'
  of course, emit its symbol and then return control to the initial state.
  Note that each bit of the received stream is examined only once, and
  that the terminal states of this tree are the four source symbols s1, s2,
  s3, and s4.
       In this example the decoding is instantaneous since when a complete
   y bol is received, you, the receiver, immediately know this, and do
  not have to look further before deciding what message symbol you
,received. No encoded symbol of this code is a prefix of any other
  symb아· 끄Li珏쁘亘四낫jYp르夕f co奴套，                쁘쁘t主涎哄世ac깬꺄끄且回／e
  since the binary digit 0 indicates the end of a symbol, plus the fact that
 珏垂皎玉芟枷匹꾜更和西匹西奭n人八入NM．小
      From this you see tile basic equivalence ot tile existence ot the
 decoding tree and the instantaneous decodability; each implies the other.
 Notice again that using the decoding tree means that each received
 symbol is looked at only once in the decoding process.
      The following code is uniquely decodable but is not instantaneous
 because you do not know when one symbol is over without looking
 further:

                                  自     0

                                  S2 = 01
                                                                             /
                                  53 = 011

                                  54 = 111

 (It is the previous code with the bits reversed.) We can see the trouble-
 some code words are prefixes of other words; that is, they are the same
                       Sec. 4.4 / Construction of Instantaneous Codes   55

as the beginning part of some other symbol. Now consider the string

                              0111 . . . 1111
                                        S4 S4

It can only he decoded by first going to the end and then identifying
runs of three l 's as each being an s4 until the first symbol is reached.
Only then can it be identified as s1, s2, or s3. Thus you cannot decide
whether you have the word that corresponds to the prefix, or if you
must wait until more is sent to complete the word. The simplest way
to decode messages in this particular code is always to start at the back
end of the received message! This puts a severe burden on the storage
and also causes a time delay.
     In view of the existence of the decoding tree, it is clearly both
necessary and sufficient that an instantaneous code have no code word s,
which is 르 끄坦肛 可앤毗er code word, 욱． If we had to deal with a
noninstantaneous code, then the attempted decoding tree would have
a structure which instead of returning to the start would, when it realized
(finally) that it had received a complete word some time ago, emit the
proper code word and then go to an appropriate place in the tree, not
necessarily the start. As in the example above, the tree could require
potentially infinite storage.


4.4 C。       n 。f Instantane。
     nstructi。
                                      g, 帥4tt;'的 (4)
                                des L니枷
                            us C。

,, *,,쏀，헒，믄／
           ,；寸m i嗜, c.dJ，능；
                         ce『{i二 ,,出｛:”，너쩟는,,,, 伊，,/，二，
                                                    ,
are preferable to ones that are not, and since it will turn out (Section
4.7) that they cost us nothing extra, it is worth concentrating on them.
Let us, therefore, explore the problem of constructing them.
     Given that we are to construct a code with five symbols s/ in the
source code S, and that the code alphabet is binary, we can assign

                               Si = 0

                               S2 = 10

                               S3 = 110

                               S4 = 1110

                               55 = 1111

to get an instantaneous (comma) code (Figure 4.4-1).
56   Ch. 4 / Variable-Length Codes: Huffman Codes




                       Figure 4-.4.1;\Decoding tree

      In this construction the use of the 0 for the first symbol reduced
 the number of possibilities available later. Instead of this, let us use
 two digits for the first two symbols, s1 = 00 and s2 = 01. We can now
 use 53 = 10. With two symbols yet to go, we cannot use s4 = 11;
 instead, we must try s4 = 110, which leaves us with s5 = 111. We get
 the code

                                S1 = 00

                                S2= 01

                                S3 = 10

                                 S4 = 110

                                 S5 = 111

 This code is clearly instantaneous since no .Symbo1 is a prefix of any
 other symbol, and the decoding tree is easily constructed (Figure
 4.4-2).
      Which of these two codes is better (more efficient)? This depends
 on the frequency of occurrence of the symbols Si- By "better" we mean-p
 of course, that the sent mes阻ges on the average will be shorter, mor우
 efficient. We will investigate this more closely in Section 4.8. 므ui:
 dently, "e妊1(妃恥 ' must dep帥加nt加proba瓦切可the various sym加｛$
 being used in the messages being sent.
                                        Sec. 4.5 / The Kraft Inequality                   57




                                                                               = 110




                                                                               = 111

                           Figure 4.4,2 Decoding tree

 Exercises

 4.4-1 Devise a similar example using six words.

厄南盲뇨d orobabilities th毗侄而戊豌區苡he 毗er 可the two codes in
\,，누   /tflis section. .          - -              Ans. V3 十 J4 十 D5 V5. .Pi
                                                        ＝니卞1＝   七느Hmm小＝   H1




 4.5 T九e Kraft Inequality 力 tr的m1서           뉵 t化e 으1 날하 寸늬烏                      수식겁으乏

 The Kraft inequality, 蜘꿔崙說굶諡, gives conditions on the
                                 上上1j when the lengths of ,the code
 existence of instantaneous codes；
 words permit forming an instantaneois code, but it does not discuss the
,Fodej selL

    Theorem. A necessary and sufficient condition for the existence 0f
 a n工 ptaneous9qcje ) or q SymbolS si (z = 1, · · · , q ) .,, encou드u
 型앞雲of lengths ll 드 /? 드 /I 드 · · · 드 뇨J艮


                                                                                       (4.5-1)
 58     Cli. 4 / Variable-Length Codes: Huffman Codes

 wh心탸心必1的ad奴 (flux的er of symb아s') of the a如habet of the encoded
 symb이S.
     This inequality is asserting that we cannot have too many short
 encoded symbols. Most of the 1, must be reasonably large.
     It is easy to prove the Kraft inequality from the decoding tree,
 whose existence follows from the instantaneous decodability. We pro-
 ceed by induction. For simplicity consider first the binary case (see
 Figure 4.5-1). For a tree whose maximum length is 1, we have either




 (a)   True for tree of length 1                                    (c)   Tree of length n

 (b)   Assume true for length n - 1                                           Y2K' + 1/2K " = K


                        Figure 4-5.1 Proof of Kraft inequality

one or two branches of length 1. Thus we have either (for one symbol)

                                                   {드1
or (for two symbols)
                                                   n
                                                                      1
                                                                난
                                                            1
We next assume that the Kraft inequality is true for all trees of length
less than n. Now given a tree of maximum length n, the first node leads
to a pair of subtrees of length at most n - 1, for which we have the
inequalities K' 드 1 and K" 5 1, where K' and K" are the values of their
respective sums. Each length I, in a subtree is increased by 1 when the
subtree is joined to the main tree, so an extra factor of 吉 appears. We
have, therefore,
                                               K       1
                                                       H2
                                                                    지     드
                                                                          1
                                           !
                                       1
                                   2
                                          Sec. 4.5 I The Kraft Inequality     59
         For radix r instead of binary, we have at most r branch
                                                                       es at each
   node中at most r subtrees each with an extra factor of h/r
                                                                    when joined
    to the main tree. Again the theorem is true.
         When can an inequality occur? A moment's inspection
                                                                      shows that
   if every terminal node of the tree is a code word,
                                                          then K = 1. Jt主
   only when some terminal nodes are not used that
                                                       lhe inequality occurs
   But if any terminal node is not used for a binary code
                                                                  alphabet, the
   preceding decision is wasted and that corresponding digit
                                                                      can be re-
   moved from every symbol that passes through this node
                                                                in its decoding.
   Thus if the inequality holds, the code is inefficient, and how
                                                                       to correct
   for this is immediately evident for binary trees. Thus
                                                            K = 1 for binary
 工rees with all the terminals used. It is only for radix
                                                               r> 2 that it is
  reasonable to have unused terminals and hence a K less
                                                                 than 1. Since
  the theorem gives a condition on the lengths only, the
                                                                 main use is in
  questions of the existence of a code with a given set
                                                           of lengths.
        Note again that the theorem refers to the existence of such
                                                                         a code,
  and does not refer to a particular code. A partic
                                                        ular code may obey
  the Kraft inequality and still not be instantaneous, but
                                                               there will exist
 codes that have the 1. and are instantaneous.
        In the next two examples we will assume that only the
                                                                     code word
 lengths are given since this is what matters in the theorem, not
                                                                      the actual
 code words. If the lengths when encoded in binary
                                                           symbols are 1, 3,
 3, 3, the Kraft sum will be 占 + 궁 = 글, and an instantaneou
                                                                    s code with
 those lengths is possible. One of the words of length
                                                            3 could be short-
 ened to 2 bits. But if the lengths were 1, 2, 2, 3,
                                                        the sum would be 吉
 + 2(i) + 吉 = 읗, and such an instantaneous code could
                                                               not exist.
        Let us apply the theorem to yet another example.
                                                                  Suppose that
 we pick the radix r = 3 and want words of lengths 1,
                                                              2, 2, 2, 2, 2, 3,
 3, 3, 3. The Kraft inequality gives on the left side
                                                        } + 5(i) + 4(h) =
 碧， so we cannot hope to find an instantaneous code
                                                             with these con-
 straints. If we drop the last code word of length 3,
                                                          the sum would be
 exactly 1 and we can find such a code. To find an instan
                                                                 taneous code
 with these lengths, we proceed systematically: S1 = 0,
                                                          s2 = 10, 53 = 11,
54 = 12, s5 = 20, S6 = 21, 57 = 220, Sg = 221, 59 =
                                                           222. In this con-
struction we have followed the decoding tree (Figur
                                                         e 4.5-2), and have
systematically increased the ternary (base 3) number
                                                          equivalents of the
codes so that the argument is easily followed. The reade
                                                              r should realize
that the three symbols 0, 1, and 2 are arbitrary and
                                                          are not numbers.
Thus any interchanges of the three symbols at any
                                                         stage would leave
the code essentially the same; it merely interchanges
                                                            the order of the
branches at a node. Indeed, one could interchange
                                                           the order at one
node without doing so at another and still have an
                                                        equivalent code.
60   Ch. 4 / Variable-Length Codes: Huffman Codes




                      Figure 4-5.2 Decoding tree

万工ercises

4.5-1 Does the infinite-length comma code il = 1, 12 = 2. . . . ...= k,
      . . . satisfy the Kraft inequality? (Use r = 2.)

4.5그 Generalize Exercise 4.5-1 to radix r.

在：司Carry out th트叩mputation ofgfor. comm色드으d巳
4.6 S加rtened Block Codes       , 7卜상 町，卜p卜         티i亭忙 캄기

Returning for the moment to the earli.蒿謚瓢, 如如애actly
2m code words in a binary system (尸n in a radix r system), we could use
m digits to represent each symbol. But suppose that we do not have
an exact power of the radix but still want the maximum length to be as
short as possible. To see what can happen, consider the case of five
symbols. Of the eight binary symbols

                                 000
                                 001
                                 010
                                 011
                                 100
                                 101
                                 110
                                 111
                                 Sec. 4.6 / Short日妃dB幻ck Codes       61
we can drop any three. But if we drop 001, 011, and 101, we can
shorten three branches of the decoding tree and still have instantaneous
decodability. We will have

                               Sl= 00

                               S2 = 01

                               53 = 10

                               54 = 110

                               55 = 111

(See Figure 4.6-1.) Instead of this choice, we can drop 目1, 010, and
011 and shorten only one branch of the tree to the code.




예） k7卜 rb악 깝우

 礁궁삐  전횅赴 叫가
  4장 甕 卜11Y늄니며
                      Figure 4-6.1 Decoding tree
  ' J이2.   찾뒀 ．                                            S5


                              Si = 0
                              S2= 100

                              S3 = 101
                              S4 = 110

                              S5 = 111
62   Ch. 4 / V口ri功厄Length Code오" 月LI丹力1an Codes


(See Figure 4.6-2.) In both cases there now are no unused terminals
and therefore K = 1. We will call these shortened block codes; they
are essentially block codes with small modifications.

                                                             ///

                                                     . 尸＼


                                                     :       L
                                               /／노       '




                                 Figure 4.6그


Exercises

4.6-1 Discuss the case of two symbols in a ternary base.

4.6-2 Discuss the case of five symbols in the ternary base.


4.7 The McMillan Inequality

The Kraft inequality applies to instantaneous codes, which are a special
case of uniquely decodable codes. McMillan showed that the same
inequality applies to uniquely decodable codes. The underlying idea
of the proof of the necessity is that very high powers of a number greater
than 1 grow rapidly. If we can tightly bound this growth, then we know
that the number is not greater than 1. The proof of the sufficiency
follows from the fact that we can do it for instantaneous codes which
are special cases of uniquely decodable codes.
     The necessity part of the proof begins by taking the nth power of
 the Kraft expression

                             [
                             q
                             2山
                                         ]111111d
                             r
                                                         仰
                                     l
                                     小
                             1
                             1
                                     1
                                                              Sec. 4.8 / Huffman Codes   63

When we expand the left-hand term we find that we have a sum of many
terms to various powers: the exponents running from n, the lowest
possible power, to ni, the highest, where I is the length of the longest
          Thus we        the exp,
                                                   \
symbol.
                    have
                                                                    "
                                      ,ression
                                                                "
                                                                         9_
                                                        lNk
                                                                              1O\
                                                 =
                                                        n rk
                                                     k _di T
                                  K
where Nk is the number of code symbols (of radix r) of length k. Since
the code is uniquely decodable, Nk cannot be greater than rk, which is
the number of distinct sequences of length k in our code alphabet of
radix r. Therefore, we have the bound



                    K'唯,슷 小 小 1<可
(The + 1 comes from the fact that both end terms in the sum are counted.)
This is the inequality we need, since for any x > 1 a sufficiently large
n makes the numberx " > ni. 恥l忍咀n be chQsen as
                                                       large as we please,
and it follows therefore that the number K (the Kraft sum) must be
 c 1.
     From this we see that there is very little to gain from avoiding
instantaneously decodable codes and using the more general uniquely
decodable codes·, both have to satisfvthc same Kraft ineciualitv on the
iengtns or me encooea symDols.




4.8 Huffman Codes

Now for the first time we will make use of the probabilities of the various
symbols being sent. As in the Morse code, we want the most frequent
symbols to have the shortest encodings. If the probability of the ith
symbol is p, and its length is i, then the average length of the code is


                                                     身尸‘Ii              越c以寸也b旨）
                                                     ' "'               小浸 꽉乞R욕 츈晷？芎
     With no loss in generality the p, may be taken in decreasing order.
If the lengths I』
                ：are not in the opposite order, that is, we do not have
both

                           J 1 브 P2 ＞尸노 之 1· ,.1> F)q
64    Ch. 4 / Variable-Length Codes: Huffinan Codes

and

                         h1 5l2 5l3 5. 1 1 5lq

then the code is not efficient in the sense that we could have a shorter
average length by reassigning the code representations of the symbols
s1, S2, S3, . . · , 5q. To prove this assertion, suppose that for m < n we
have both conditions (for some m and n)

                      pm > pn       and     lm> ln
In computing the average length, we have, among others, the two terms

                           Old: pm!m + pnln

By interchanging the encoded symbols for Sm and sn we get the corre-
sponding terms

                          New:    j7r7i/n + p,lm

Subtracting the Old from the New we have the change due to this
reassignment:

New - Old: p (1n - Im) + p,(lm 小 ln) = (pm 小 p,)(l. - im) < 0

From the foregoing assumptions this is a negative number; we will de-
crease the average code length if we interchange the encoded symbols
for Sm and s, . We therefore assume that the two running inequalities
both h아d.
     We begin our examination of Huffman coding with encoding into
the binary alphabet. In Section 4.11 we look at the base r alphabet.
We will use "source symbol" for the input s1 and "code alphabet" for
the alphabet into which we are encoding.
     The first thing to prove is that the two least frequent source symbols
of an efficient code have the same encoded lengths. Suppose that the
maximum coded symbol has length 1. If there is only one of such length,
then since the code is instantaneous, any shorter coded symbol of length
1 - 1 (or shorter) is not a prefix of the maximum-length coded symbol.
Therefore, the last part of the longest symbol could be dropped with
no loss of information in decoding. Thus the two longest symbols must
have the same length, and because of the running inequalities, they must
be the two least probable.
     The proof of the encoding properties, as well as the method of
encoding, is a reduction at each stage to a shorter code. We simply
                                                                           Sec. 4.8 / H毗枷口n Codes                    65

combine the two least probable symbols of the source alphabet into a
single symbol whose probability is equal to the sum of the two corre-
sponding probabilities. Thus we have to encode a source alphabet of
one less symbol. Repeating this step by step, we get down to the
problem of encoding just two symbols of a source alphabet, which is
easy-merely use 0 and 1. Now in going backward one of these two
symbols is to be split into two symbols, and this can be done by ap-
pending a second digit 0 for one of them and 1 for the other. In the
next stage of going back, one of these three symbols is to be split into
two symbols in the same way. And so it goes. For one special case
given below, Figure 4.8-1 shows the reduction process, and Figure




            Si              pi

            Si             0.4 ,1                        0.4                       0.4 \   /0.       6
                                                       =＝二1，
                                  N끼
                                           노건之：




                                                                               ><:
                                                                      니．   .




            S2            0.2'- ..＼늬                                                       7乙 =9·4
                                           ＼智＼
                                }
            S3            0.2\，人                           0.
            54             0'                              。2   2.
            S5             0.11)

                         0riginal                     디rSt                      Second           Third
                                                      reduction                 reduct油n         reduction

                            Figure 4-8.1 Reduction process




 그 平日
            니                              1                               r1              1                 I

  弓
                                       P

                                                 1                   0.4                                         0

                                                 01                  0.2                                         l

                                                 000                 0.2

                                             。1。
                                             。                       。.2

                                                 。11
                                                 。
                                  “기
                 1凹11+
                                                       寸



                                Figure 4-8.2 Splitting process
66     Ch. 4 / Variable-Length Codes: Huffman Codes

4.8-2 shows the corresponding splitting (expansion) process. The gen-
eral case should be obvious from this.
    'How do we know that this process generates an efficient code?
Suppose that there were a shorter code with code length L' with

                                  L' <L

Let us compare the two decoding trees. In an efficient binary code, all
the terminals are occupied and there are no "dead branches." (A dead
branch would enable us to shorten the code by deleting the correspond-
ing binary digit in all the terminals that pass through this useless decision
point.)
     If there are only two symbols of maximum length in a tree, they
must have their last decision node in common, and they must be the
two least probable symbols. Before we reduce a tree, the two symbols
contribute

                              iq(Pq + Pq-i)

and after the reduction they contribute

                          (iq - 1)(pq + Pq-i)

so that the code length is reduced by

                                Pq + Pq-i

If there are more than two symbols of the maximum length, we can use
the following proposition: Symbols having the same length may be in-
terchanged without changing the average code length. Using this, we
can bring the two least probable symbols so that they share their final
decision node. Thus after the reduction, we have shortened the code
by the amount

                               Pq + Pq-i

Therefore, in either code we shorten the code and decrease the average
code length by the same amount.
     We apply this to both the decoding trees we are comparing. Since
both are decreased by the same amount, the amount of inequality be-
tween their lengths is preserved. Repeated application of this will re-
duce both trees to two symbols. In the Huffman code the length is 1;
for the other it must be less than 1, which is impossible. Therefore,
for binary codes the Huffman code is the shortest possible code.
                                                                     Sec. 4.8 I Huffman Codes                          67

       The encoding process is not unique in several respects.
                                                                 First, the
 assignment of the 0 or 1 symbols to the two source
                                                         symbols at each
 splitting stage is arbitrary, but this produces only trivial differe
                                                                      nces.
 Second, when two probabilities are equal, it appears
                                                        to be a matter of
 indifference which we put above the other in the table,
                                                            although the
 resulting codes can have different lengths of words. Howe
                                                              ver, in both
 cases the average length of the encoding of messages in these
                                                                codes will
 be the same.
      As an example of two different Huffman encodings
                                                             of the same
 source, let

                                                   Pi = 0.4

                                                   P2 = 0.2

                                                   P3 = 0.2

                                                   P4 = 0.1

                                               P5= 0.1

If at each stage we put the merged states as low
                                                    as possible, then in
Figure 4.8-1 we get lengths (1, 2, 3, 4, 4) and the averag
                                                           e length is

       L = 0.4(1) + 0.2(2) + 0.2(3) + 0.1(4) + 0.1(4)
                                                                                                           = 2.2
On the other hand, if we push the merged
                                                states up as high as pos-
sible (Figure 4.8-3) , we will get lengths (2, 2, 2, 3,
                                                        3) and the average
length is

       L = 0.4(2) + 0.2(2) + 0.2(2) + 0.1(3) + 0.1(3)
                                                                                                           = 2.2


              Si                    P1

             Si    伉） 켜나 0.4 00                        0.4 00                0.4                      1       0.6 0



                                         ;7乙.·21
             S 2 10 켜中 0.2 10
                                                       0.2                                   ;:><r.
                                                                                                              .4
                                                                                                                   1



                                                              少
             $3 ] 1   ..- 0.2                                                                         01
                                                              !7Z.
                                                                                  ·4i
                                                                         \
            54 010 寸                1 010           \ -0.2J 11
                                                                             0.
                                                                                        2)
                           -   0.
                               에
                                                          '
                                         /
            $5                               011
                   011 十


                       Figure 4-8.3 Alternative coding
68    Ch. 4 I Variable-Length Codes: Huffman Codes

Both codes have the same efficiency (average length) but not the same
set of lengths of the symbols.
     Which one of these two codes should we choose? A very reason-
able choice is the one whose average length would vary least over the
ensemble of messages. We therefore compute the variances in the two
cases:

           Var(I) = 0.4(1 - 2.2)2 + 0.2(2 - 2.2)2 + 0.2(3 - 2.2)2,
                      + 0.1(4- 2.2)2 + 0.1(4- 2.2)2= 1.36
      Var(I1) = 0.4(2- 2.2)2 + 0.2(2- 2.2)2 + 0.2(2 - 2.2)2
                      + 0.1(3 - 2.2)2+ 0.1(3 - 2.2)2 = 0.16

Thus the second code has significantly less variability in use on finite-
length messages, and is therefore probably the preferable code. .J1Js.
true that always moving a combined state as high as possible w且Lgive
a minimum variance code, although we do not prove it here. By moving
a merged symbol higher than it should be, we can greatly reduce the
variance for a small increase in the average length.

Exercises
                                                                  P
4.8-1 Give the Huffman code for Pi           l弓1
                                                   P
                                                   J
                                                   八1   l
                                                        中3
                                                          9   n
                                                              a   d
                                                                  4
                                                                  4J
                                                                           l小        =
                                                                                         !




                                                              仍
4.8-2 Give the Huffman code for Pi = 吉，P2 = 去，                         P4 = 궁， and
                                                                   }
                                                                   m
                                                                                             =
                                                                   h
      P5 = 솖．

4.8-3 Give the Huffman code for Pi                 仍          尻        m        工比       帥       1 1
                                                                                                       =
                                                                                                       =




      P5 =      16.



4.8-4 Give the Huffman code for Pi = 끎，P2 = 붊，P3 = 솖， and p4
      솖．
4.8占 (3iVe
4.8-5 Give the Huffman
               H1lff1llan COde
                          code for     PrObabihheS1,
                               fOr the probabilities s, 1,, 1,, 1,, 1
                                                                    is, and 냥i.

4.8-6 Show two distinct decoding trees for the case L } , 吉, and 吉.


4.9 Special Cases of Huffman Coding

There are a number of interesting cases of Huffman coding to look at.
First, if all the symbols are equally likely and if there are exactly q = 2''
source symbols, then the (binary) Huffman code will be a block code
                              Sec. 4.9 I Special Cases of Huffman Coding                                         69




          1

          .                    .
          1                                                      .
                              .

                                                                 e



                             티ther
                                   or
                                          q=
                                              2m, =     p,
                                                                     듦
                                         Pg-i + Pq> P 1 -'- s卜ortened block code
                                                                             ＋岫岫
                                        Figure 小9.1

 with all symbols having the same length m (see Figure 4.9-1). If there
 are not exactly 2'n source symbols we will get a shortened block code
(Section 4.6).
     The second case is more interesting. Suppose that the two least
probable symbols have their probabilities such that their sum is greater
than the most probable symbol; that is, P9-a +P? > p1. In the Huffman
process (see Figure 4.9-1) the corresponding symbol word will go to the
top. It then follows that the next two least probable symbols will corn-
bine and will go to the top, and so on. If the number of original symbols
q is an exact power of 2, then the repeated combining process into the
final code of two symbols will have each symbol go through the same
number of splitting steps, and each symbol will acquire the same number
of binary digits in the expansion process. Thus again we will have a
block code. If q is not an exact power of 2, then, of course, there are
small modifications to the foregoing process, and we get a shortened
block code (Section 4.6).
     It 始 on虹when the브obabilities of the source sy岫olsoft匙 毗ssag르，
are very different that we get a significant economy from the Huffman
encoding process. This is what we would expect if we but thought a
bit- only when there are large differences in the probabilities of oc-
currence does the variable length of the code symbols pay off.
     For example, if the pr的abilities ／가 have grea나師和晦：         \
                                           '       'i                                           ！尸 ,\ ,   낚1V
                                   ,    :> ;       \         n           /         V\ 7          ), V 人 !  (A cLi\
                                               .) k=i+ 1             '             1 1J    \\    七)     / "'
for all I, then a comma code will emerge. In 回6fis- e的ation (4.9-1)
says些，아 쁘吏 prob的世til프t le旦st르旦great as two-thirds of the sum
of all th드p型babil吐ies that 的llow. '                        ,
 Koh Wee Jin observed that (4.9-1) can be improved to p1 之 2                          Pk
70   Ch. 4 / V口rn功／e工ength Codes: Hu力67i口n Codes

                  Pq- 4

                  Pq- 3


                  Pq_2

                  Pq- i


                    Pq


                  Pq_ 4

                  Pq-3

                  Pq- 2

                  Pq너

                    Pq

                   Figure 4-9.2 The two possible cases

    To prove this, we begin at the bottom of Figure 4.9-2. The sum
Pg + Pq- i can be greater or less than Pq- 2' but it cannot be greater
than Pg- 3rn Thus at the next stage we get the sum

                          Pq + Pg- i + Pq- 2

and Pg-2 has been combined only once. .epeating this at each stage,
we see that we can get a comma code. The cole


                                 dl e八
                                     J
                                     口
                           n

                                   l
                          Pk = i;            (k< q)
                                   고
                                   l
                                         l
                          Pg =   q
                                 八
                                 乙




is such a code and permits a comma code rea1izati9n.
     If at any stage of reduction one of these conditions applies, then
you know that beyond that point the corresponding splitting process will
apply. This can save time in some cases.
      As a practical observation it is often convenient to add one symbol
 for your 에n use, an escape character (end of message) (see Section
                                                  Sec. 4.9 / Special Cases of Huffman Coding                  71

 1.10). In the Huffman decoding tree, each other terminal returns the
 control to start of the tree, but this escape state allows you to escape
 the decoding process and resume other tasks. Obviously, you assign a
 very low probability to this escape character so that it has little effect
 on the re$tbf theZode.
       The蜘占H卒               , where the 展8item (k = 1, 2, . . . , q) has
 a frequency6璇發小ery common in1anguage problems. Of course,
 the distributioi ig cut off someplace or else there would be an infinite
 number of items (and the infinite series 1/k does not converge). Let
 us compare the performance of a standard block code where each symbol
 has the same length with what Huffman encoding can do. Table
 4.9-1 gives the results, where the first column gives the number of items,
 the second the length of each symbol in bits, and the third the Huffman
 encoding average length. The last two columns give the gain and the
 percent gain in using Huffman codes even in this rather unfavorable
 case where there is not a great deal of variation in the probabilities.
      If you examine the Huffman encoding method, it soon becomes
 clear that you can work with any numbers that are proportional to the
 probabilities. Thus you may use the frequencies rather than the prob-                                                         7m
 abilities, or you can multiply through by some suitable constant to con-
,vert the probabilities to integers to make the work easier. Your escape                                                            \
 character should be given a frequency of 1 to minimize its effe

                                                   十，, \17
                                                 ,,，尸／
                TAB!月 4.9-1 ( z加／I가缸r沾끄ti移石nco如din 口 i/n町枷Zn C叫＜少,
                                                                                            酉／ d,1
                                                                                       //   1' )          5
                 Block Code                           Huffman
   n               Length                         "     m               7   d늚 「，d穹點


       248珀끄M




                      l n二 m4V 4 드나 6 m/ 8 Q
                                                        1.0                 0                       0




                                           / 0
                                                       "1.8                 0.2                    10
                                                      k乙6&                  0.32                   11
                                                        3.43                0.57                   14 /
                                                        4.17                0.83   \               17
                                                        4.89                1.11                   18.5
   128                                                  5.60                1.50                   20
   256                                                  6.26                1.74                   22
   512                                                  6.90                2.10                   23
                     l
  1024"                                                 7.54                2.5                    25


Exercises

4.9-1 (Difficult) Discuss what happensin. 浿sesthat lie between the two
                                                                                                              咬｛
                                                                                                                   戶
                                                                                                                   ,>    1（노
                                                                                                                        " ",




                                                             그 1at孕J了
      main results.
                                                       됴


                                                            ！
                                                            느
                                                      qq
                                                       객n
72    Ch. 4 / Variable-Length Codes: Huffman Codes

4.9-2 Verify first three lines of Table 4.9-1.

4.9-3 Discuss using frequency = j如r an escpe character.



4.10 E工tens加ns 可a Code

In Section 4.2 we defined an extension of a code. We are now in a
position to see why they are useful. Suppose for the purposes of a
concrete example that we have two symbols s1 and s2 with probabilities
Pi = 궁 andp2 = }.

                                                        Encoding
                        S         P      2
                                         m3
                                                        S1 -p  =
                                                                    0
                        S   n
                            乙
                                  Pn
                                   乙     }              s2-         1
                                                                    =




The average code length is 1.
     The second extension takes two symbols at a time (the first exten-
sion of a code is itself):




                                                                                         춤目
                                                        Encoding


                                                                                  也T多g
                    s1s1;       Pi.i =                                  1     4
                                                                              m
                                                                              六


                    SlS2;       Pp.2                                          누


     幽！冽狼赴너歸｛
       )
             缸J.P".
                    s2s1;


                  1 = 彭八
                                P2,1
                                         ]
                                              //         (}1
                                                        52s2            001

Here Pi.i is four times as proIab1e as P2,2. The average length for
Huffman encoding is圈= 0.94444 . . . for comparison. The next ex-
tension takes three        ols at a time gives 졺 = 0.93827. . . . Taking
four s, at a time leads to the average code length 0.93827. . . .
     Thus we see that extensions increase the variability and hence allow
Huffman coding to achieve some compression. We will show in Section
6.9 that a lower bound'0 on what can be achieved for this example is
0.91830. . . .
                   自 名 h 뇨寸．                       1씨
                                                               rr

Exercise

 4.10-1 Compute the average code length of the extensions given in this
        section.
                                                 Sec. 4.11 / Huffman Codes Radix r                          73

4.11 Hi｛寸沇an Codes Radi工 r

     When we go to a radix r code the modifications to the Huffman
encoding scheme are easy to make. In the binary code we always found
at each stage the number of items (two) to combine into the merged
state. When we are in radix r> 2 this is not necessarily true, and we
need to think first.
     At each stage when we combine r symbols into a single symbol
(with the probability that is the sum of the probabilities of the individual
symbols) we replace r symbols with a single symbol. Thus each merging
of r states reduces the number of states by r - 1. But at the last state
we will want to have a full complement of r states to assign the encoding
symbols 0, 1, 2 . . . , r - 1. Thus we want to have

                                    k(r 尸 1) + r

states when we begin, where k is some integer. However, this is the
same as
                                   k(r - 1) + 1

(the integer k has been increased by 1 in this new notation). Often we
will not have that number, so we will add enough states each with
probability p = 0 until we do have the needed number.
     Figure 4.11-1 gives one concrete example for base 4 (from Huff-


              Si
                             pi


              Si   1        0.22             1       0.22    1        0.40 0                         1.00
                                                                    I
              S2   2        0.20             2       0.20    2     /0.22 1
              S3   3        0.18             3       0.18    3    //    0.
                                                                             20 2
              $4   00       0.15             00     0.15)                    侶 3
                                                            I '
                                                             띠／
                                                                       0．
              $5   01       0.10             01      0．伯 1 d1

             56    02       0.08             02
                                                            V
                                                     0.08 (02
                                                          1
             S7    030      0.05
                                   lo39o.o7J 떠
             S8 （日1         0.02 1031
                                        y/
                                   .1
                         Figure 4-11.1 Huffman radix 4
                                                                                                     1

                                                                                    J !
                                                                                                h(



                                                                                        \\1JJ   1    2
                                                                                                     /
                                                                                    尸
74    CIt. 4 / V口Ti口ble工ength Codes: H14丹man C아加S

man's original paper), where we have added two symbols s9 and s10,
both with probability zero. After two reduction stages we reach four
symbols, which we encode as 0, 1, 2, r 中 1 = 3. The backward path
of splitting goes as for radix 2 with the obvious changes.
     For the proof of the efficiency of the encoding we first, if necessary,
again add enough symbols of probability zero to the alphabet of symbols
s, so that at each stage r symbols can be combined. The trees will
therefore have all their terminals filled, and we will be able to argue,
as in the case of the binary trees, that no other encoding can be more
efficient.

Exercises

4.11-1 Use the data of Figure 4.11-1 and encode in radix 3.

4.11그 Given Pi = 吉， P2 = 吉， P3 = 궁，P4 = 솖，P5 = 古，P6 = 去， and
      p7 = 솖, encode Huffman for r = 2, 3, and 4. Find average
      code lengths. Compare for r = 2 and 4.
                                             Ans. r2 = 31/12 - 3

4.11-3 In Exercise 4.11-2, after multiplying each probability by 240 to
       get equivalent frequencies and an escape character of frequency
       1, find code for r = 2 and also draw the decoding tree.

4.11-4 Do Exercise 4.11-3 for radix 4. Compare with your answer in
       Exercise 4.11-3.


4.12 Noise in Hi｛乃加an Coding 까obab끄泣es

Suppose that the estimates of the probabilities p are not accurate. How
much does the average code length suffer? In short, will small errors
in the estimates greatly degrade (or improve) the system?
     To answer this question, let the p, be the original Huffman code
design probabilities and
                                                                   (4.12-1)

be the probabilities for the source that is actually used. Clearly,

                               1 근，     ; F',
                               = Z1 e1 =＝乙了V                       (4.12-2)
                               모J生뇨．四幷. 呼：』

since both p, and p,' are probability distributions that sum to 1.
                                       Sec. 4.12 / Noise in Huffman Coding Probabilities                                                                                      75

     As one measure of the size of the errors e, we use the variance


                                                                                 l 寸口
                                                                                    1
                                                                                             q心烏                       m毗尸    :,p之                                      (4.12-3)

Multiply (4.12-1) by 1, and divide to get the new average symbol length:

                                                                                                                              2
                                                                                                                       l Hq
                                                                         L
                                                                             1
                                                                                 P       r

                                                                                         L
                                                                                                 누
                                                                                                     卜
                                                                                                                                   J
                                                                                                                                   아 n
                                                                                         /
                                                                                             ／
                                                                     1
                                                  L +               !q 2                                 lie,
                                                                                                                         11




The last term is the change in the average code length.
     With the two conditions (4.12-2) and (4.12-3) on the e, we resort
to the method of Lagrange multipliers to find the extreme cases. The
Lagrange expression is



              2=)2 l.e．夕26
                      , ,－먀2<                                                                                                                                   1
                                                                                                                                                                J/
                                                                                                                                                                    1
                                                                                                                                                          0
                                                                                                                                                          八J乙
                                                                                                                                                                \
with Lagrange multipliers X and gi. The partial derivatives with respect
to e, are to be equated to zero; that is,


        型 叱   l mq
                                /
                            /
                                                 入
                                                                                                                       0            (i = 1, 2, . . . , q)               (4.12-4)   =H
                        1
                                                                                                                                                                                    1




肌now sumth毗四uatm恐汽 如me「
                    1
                \
                                                                    l H口l         口
                                                                                  ； i
                                                                                                                              入        0
                                                                                                                                                                        (4.12-5)

which determines A. Next we multiply equations (4.12-4) bye, and sum
to get
                                                 n乙i                                                                   n乙i
                                                                                 e                                     l mq
                                                 l mq                                                           八 ／q
                                                                                                                                    e = 0                               (4.12-6)
                                                                1
                                                                                                                        H
                                                            L
                                                        1
which determines FL. Finally, we multiply equations (4.12-4) by 1, and
sum to get

                                                                                                                                     eq
                                    l mq
                                                        l eq
                                           口白／
                                                                                                                                                      口
                                                         入                                                                         d甘
                                                                                                                                   l
                                                 n
                                                 乙1i                                                                          싸乙                  e
                                                                                         2
                                                                                                                                              2
                                                                                                         ii
                                                                                     i
                                                                                                                                          i
                                                                                                                                                                           6j 軒（{ 3         브
                                                                                                                                                                           ==/          -
 76     Ch. 4 / Variable-Length Codes: Huffman Codes

 Using the A from (4.12司 and the FL from (4.12-6), we have

                            [
                                                                                ［詩
          1
          l                 lm
                            r1
                                                                                         0
              2                                               n乙i
                                                                                     e
            1q               尸q
              1
                  =


                                        I   J            Lq
                                                -


                                                                    ei7]
                                                         14
                                 2i12
                                                                           2/
 Using (4.12-3), this takes the form



              （詩＜4)2=1詩乃－｛抑）'］『'        = Fvariance of (L1 Ivariance of (e1
                                                                                         (4.12-7)

迅4뇨쁘그吼그밈쏘匡玉血；. }'餉示교r誨；除님，.
      These are the extreme (Chebyshev) values possible for a fixed if2.
 The equation shows that the more variable the I., the more harm (or
 good) the errors in the estimates of the p, could cause in the average
 of the syn小이 length.
      That errors e1 can make no change in the average length can be
 seen from the following example. For q 之 3 let, for some e,

                                            e1 = (12 中 /3)e

                                            e2 = (13 - 乙）e                                   (4.12-8)
                                            e3 = (ll - 12)e

                                            e1= O              (i> 3)

 Clearly,

                                                1
                                                小 Lei = U
                                                    1-
                                                q

 To find the corresponding o2 we have, from equation (4.12-3),

                      [(12 - l3)2 + (13 - li)2 + (1l - 12)2]e2 = (J2

 Now consider the average code-length change,

      11e1 + 12e2 + l3e3 + 0 = (1112 - 1113 + 1213 - 1211 + 1311 - 1312)e

                                            =
                                                0

  Hence these changes e, [equations (4.12-8)J do not change the average
  code length.
                                    Sec. 4.13 I Use of Huffman Codes       77

       From equation (4.12-7) we conclude that Huffman coding is fairly
  robust; small changes in the probabilities do not seriously degrade the
  system. But we have not answered the question of how much a redesign
  using the new probabilities could have imoroved matters.
          Y 蝴咤 H매地" 叫" P唯                      才'/ 2拉미       앙玄 玄毫윽 ' J남
 4.13 UseofH꺄序加zn Codes

   The design of a Huffman code is highly recursive, and therefore is easy
   to program on a computer. The finite automata scheme (tree) of de-
   coding mentioned in Section 4.2 provides a method for decoding Huff-
   man codes using a single r-way branch per received code symbol of radix
   r. The method is simple and rapid and each received symbol is examined
   only once.
        The encoding of a Huffman code is for reasonably sized source
   alphabets, a simple table lookup. If we have a lot of information to
   put into long-term backup storage in a computer, for example, and if
   the source code has symbols whose probabilities vary greatly, then it
   may well be worth encoding the information into an appropriate Huff-
   man code to save long-term storage. As we have seen, it depends on
   the variability of the probabilities p1.
        For a particular hand-held language translator, a dictionary of about
   12,000 bytes (8 bits) was compressed into an 8192-byte ROM storage
  device using compression methods resembling Huffman codes. The
  encoding of the operations in the Intel 432 used Huffman-like codes to
  compress the programs that are run.
        Programs have been written to automatically scan a text, design a
  code, compress the text, and store the text along with the decoding
  algorithm. The program counts the frequencies of the source symbols
  and adds one special symbol called "end of text" of frequency 1 (see
  Section 4.9). This special symbol is used to end the decoding. Such
  programs have been known to reduce the storage of data to less than
  half the original amount.
        We may also ask what happens to the decoding process when an
  error arises. It is evident that in a comma code the first appearance of
  a comma will resynchronize the decoding process. But in many codes
  it is not obvious how long you will go before you are resynchronized.
  A satisfactory theory is slowly emerging, but for this text about the best
- that can be done is to use Monte Carlo methods on the given code.
  Encode a number of typical messages, insert a change, deletion, or
  addition to the coded stream of digits, and then apply the decoding tree
  to see how long it is until the text is coming out correct again. In a
  78    Ch. 4 / Variable-Length Codes: Huffman Codes

  block code the insertion or deletion of a single bit will indefinitely alter
  the decoding process; a block code can never recover from a single such
  error.


  Exercises

  4.13-1 Discuss writing a computer program to find a Huffman code
         from the p1.

  4.13-2 Discuss the use of a decoding tree for Hamming codes rather
         than the computing methods of Chapter 3.

r4. 了．了F。
        r the c。
               mma c。
                    de s1 = 0. s, = 10. s, = 11. sh。w that』an
         e.rror 딴one mt can ne propag呼（} aroitrarii恥．프"                  ti-ltnt " 느Q프
         sioer s1(f3y,s2. j                         ,.rr   \C)
                                  i,   ,. '   ＼口）                '




  4.14 Hamming-Huffman Coding
                                                     1
                                       尸




  How can we combine the source compression of Huffman encoding with
  the noise protection of Hamming encoding? As far as is now known,
  you encode in a Huffman code and take the output stream, break it up
  into blocks, and encode it into a suitable noise-protecting Hamming
  code. For decoding you reverse the process: decode Hamming, then
  Huffman.
        A reasonable question is to ask if a single encoding process can do
  a better job. It is left to the reader to try. We note that in the decoding,
  tree nodes near a terminal must not be used by other branches of the
  tree.
  小e紬M帥心 0婉              몇 叭叭師n,
                                                    鈿（( , H艸＞3 (0（뇨 叫
今如뇨， 缺）
      『 2：呻                        篆것毛 '뼈                             " 확 芽i
                                                                     “引

   恤汕十 「品卜 싻찌 如서                                           小伽，' G地'七；" ' 』’
   弩（ 破斗，
                                                       뇨，
                                                            ,




                                                                뇨人C-心＼
 Chapter 5



                                  Miscellaneous Codes




5.1 In勿oduci加n

  There are many different codes for the many different situations that
  arise in practice. We can study only a few of the more important ones
  and hope that you will be able to create your own when the need arises.
       We shall first look at Markov processes', which enable us to handle
  some of the larger probability structures that arise typically in languages,
  larger than the simple frequency of occurrence that is used by the Huff-
 man code.
       We will then examine predictive coding, which is very general and
, t es advantage of any structure you know about that can help yoq
 predict the next symbol accurately. The better your ability to predict
  the next symbol, the shorter the final message you have to use. Nothing
 is said about how you predict, only that you have written a program
  that incorporates all the structure that you are going to use. This is a
  very general method of code compression. Thus, as we said we would,
  we have gone to very general methods and have skipped the many special
 codes for special cases. However, it is hoped that the reader, when
 faced with a special case and having seen the codes we have given, will
 be able to invent an appropriate method of suitably encoding messages
 for compression.
       We then discuss the remarkable idea of random encoding, both for
 its practical value and for its theoretical use in proving the main result
 of information theory. 工he particular method we examine is callecF




                                                                           79
 80    Ch. 5 / Miscellaneous Codes

  "hash coding         is widely used in computer software, but has appli-
 cations to other situations.
       Finally, we will look at Gray codes, used to go工eliably from analog-
j o-digital representations and back. Since this occurs so often in practice
  (because nature provides us basically with analog signals), it is a part
  of the education of computer science students and others who have to
  deal with "real" signals. We also show a simple variant useful in testing
 memories of computers. For more material, see Ref. [J].



5.2   4境口I Is a Ma毗ov Process?

 Up to this point we have used only the probabilities of occurrence of
 the source alphabet s1, S2, · . . , Sq. Familiarity with natural languages
 shows that there is often much more structure in a language. Thus, as
 we noted before, in English the letter 0 is almost always followed by
 the letter U; the probability of seeing the letter U depends very much
 on the letter that came before it. In probability theory the notation

                                                   p(U I 0)

 means "the_probability of seeing U given that ( I ) you have just seen
 the letter 0." In general, in the notation of ajth-order Markov process,

                           p   (s1      I   sf1,     Si2, .   .   .   ,   sf1)
 is the conditional probability of seeing s, given that you have just seen
 all the letters s, , 뇨， · · . , s功 in that order. Note that the sequence of
 syn小아s is

                                     Si1' Si2, . . . , Si1, Si


      This is clearly a situation that arises in practice-the previous part
 of the message can often greatly influence the probabilities for the next
 symbol that you will see from the source.
     ,In computer language a zero memory source uses each source sym-
 bol independently of what has preceded it. A f-memory source uses
 the previous j symbols, and this idea corresponds exactly to a jth-order
 Markov process.
       We consider the system as being in some state. For a one-memory
 source there are q states, one for each symbol s, of the source alphabet.
 The standard weather prediction that "tomorrow will be like today" is
 an example of a one-memory predictor. For a two-memory source there
                                              Sec. 5.2 / What is a Markov Process?                               81
                  /


 are q2 states, one state for each pair of source symbols. The linear
 trend predictor

                                           yn+1 = 2y,, - yn_ i

is a two-memory source; the next value y-, + 1 is estimated from the two
previous symb아sy, and y, 寸 In general, 的ra 川犯mory 5에rce there
are q' states in the Markov process.
      As an example of a simple one-memory source, suppose that we
have an alphabet of three symbols, a, b, and c. Let the probability that
an a is followed by any of the three letters be each} . Let the probability
that the letter b is followed by another b be 글, and either of the other
two letters, a or c, be L Finally, let the probability that the letter c is
followed by a c be 글, and either of the other two, a, or b, be L We
have




               加 如 加
                                               小                                      (
                            n b
                                      l
                                      m3             q   J
                                                             l
                                                             H3   P   C   n   H 1
                                                                                    = (\J
                                                                                            l
                                                                                            U3

                                              b
                                              =      )                              ) )
                                                     /
                                                                          b
                                                                                    /
                                      l
                                      14
                                              b b            l
                                                             U2   P   C       =
                                                                              =             l
                                                                                            14   =
                                                                                                             )
                                               P P
                                                                                                         /
                                      l
                                      14
                                                   c) = 吉         p(c I c) = 글
                                                                                                     (
                       c)
                                  =
                                                                                                 \
     It is conventional to use a tr口7奴如月 g相鉀 to illustrate such a Mar-
kov process. There are, of course, three states in this case (Figure
5.2-1), labeled a, b, and c and indicated by the circles. Each directed
line is a transition from one state to another state, whose probability is
indicated by the number alongside the line. For example, p(a I b) is
the directed line from b to a and has the probability of transition of L
In this example each state has three lines "out" and three lines "in."




                                  Figure 5-2.1 Transition graph

    We may assign a concrete interpretation to this diagram. Let a
mean "fair weather," b means "rain," and c mean "snow." Given that
today is fair, it is equally likely that tomorrow it will be any of the three
82    Ch. 5 / Miscellaneous Codes

states, fair, rain, or snow. But if today is either rain or snow it is a
50-50 chance that it will be the same tomorrow, and only 1 in 4 that it
will be either one of the other two.
     We may write the graph in a matrix form as follows, where the
label of the current state is given by the letter on the left of the matrix
and the next state after the transition is given above the matrix. The
matrix entry is the transition probability. We have

                                                                     n                    b            C
                                                                          수
                                                                              A
                                                                                                           )
                                                                              1
                                                                     l}                   l
                                                                                          3            l
                                                                                                       3

                                                   口 b
                                                            /
                                                            1
                                                                     l
                                                                     4                    l
                                                                                          2            l
                                                                                                       4
                                                            1
                                      H                     1
                                                                                                                           (5.2-1)
                                                   C            \    l
                                                                     4                    l
                                                                                          4            工
                                                                                                       2
                                                            1
                                                            \
In a transition matrix the sum of the elements in any row must total
exactly 1, since the current state must go somewhere.
     Now suppose that instead of having a definite state today, we have
a probability distribution for today's state (pa, Pb' p.), where, of course,
Pa + Pb + p = 1. Itcan bethatonep1 = 1 andtheothertwo are0,
which means that we have a definite state today. If we multiply this
row vector on the right by the transition matrix (5.2-1), we get the
probability of tomorrow's weather:



                                                                           \\
                                                                                  l
                                                                                                            뇨
                                                                                  m
                                                                                                                                     )
                                                                                  }
                                           P       P                                                                                 (\
                                                                Pr
                                                                      ///1\
                                                                                                            ＼1
                                               n       b
                                                                                  吉                         J
                                                                                                                                     !


                                                                                  1
                                                                                  m4
                                                                                                            /
                                                                     1
                                                                     m2   P       b           吉／), , 4Pa + }Pb + 吉／7, ]
                                           l       i
       = [}Pa + {Pb +                      机       琨
     To find the probabilities 2 days ahead, we multiply on the right
again by the transition matrix (5.2-1). Because of the associativity of
matrix (and vector) multiplication, this is the same as first multiplying
the matrix by itself to get the square of the matrix, and then multiplying
the original distribution on the right by this. We get, for the square of
the transition matrix,
                                                                                                       0
                                                                                                       m6
                                                                                                                 꼬拍
                                                                                                                      3
                                                                                                                      n6
                            l
                            13   l
                                 43   1
                                      l3               l
                                                       13       l
                                                                13       l
                                                                         13




              / / r 1 1 \
                                                                                                       l三
                                                                                                        J             1쩍
                                                                                                                       J
                                                                                      \
                                               /                                               /
                                           \
                                               i
                                                                                                       3
                                                                                                       m8             6
                                                                                                                      中8
                                                                                                                 브明
                                                                                      1
                                                       t
                                                       14       l
                                                                弓q       t
                                                                         U4
                                           1
                            l
                            U4   l
                                 m2   l
                                      14                                                               l
                                                                                                       七4             l
                                                                                                                      山4
                                               i
                                                                                               1
                                           J                                          1
                                               1
                       \
                       \    1
                            l4   l
                                 44   l
                                      12   /
                                           /
                                               \   \   l
                                                       m4       1
                                                                14       1
                                                                         l2       /   /
                                                                                               \
                                                                                                   \
                                                                                                       m
                                                                                                       3
                                                                                                       1
                                                                                                       叫
                                                                                                        8
                                                                                                        4        m菰
                                                                                                                      m
                                                                                                                      9
                                                                                                                      1
                                                                                                                      m
                                                                                                                       8
                                                                                                                       4
                                                                                        Sec. 5.2 I What is a Markov Process?                 83

  Writing this matrix in the form


                                                                .                       /40      52                    52\
                                                   由1
                                                                                        \
                                                                                            39   ：二:87                                   (5.2-2)



 we see immediately that the entries in the square of the transition matrix
 are less variable than were those of the original, (5.2-1). If we square
 this matrix (5.2-2), we get the matrix for predicting 4 days ahead. For
 this particular original transition matrix it is not hard to prove that the
 successive powers converge to a limiting matrix.
      Do the successive transition matrices preserve the property that the
 sum of any row is exactly 1? To prove that they do, we have from the
 two general matrices P and P' the entries for the next one, P":


                                                                까‘，/ = 2 Pi,kP白

 where by hypotheses the row sums for both matrices are

                     2/7，·，k= 1                                                              and                       2p;c,j = 1

 We compute, therefore, the row sum of the product matrix

                                    /
                                            口乙k
         2 PL                                     Pi,kPcJ) = 쥬 Pi,icPi,j = 쭈 Pi,k = 1
                                r
                                                                                                                                                   1 H
                            1
                        \
                                        \




 as required.
      If we start with a matrix with a given distribution, what is the limiting
 distribution for powers of this matrix? For the limiting product of the
 matrix, what is the probability distribution of the states a, b, and c?
 Clearly, we must have a distribution that does not change its probabilities
 when going to the next day; that is, we must have, for our particular
_matrix. (5.2-1).

                                                                                /
                                                                                                                   \
                      P
                                                  P                                                                      P           D
                                                                                                               \
                                                                                                                                 P   P
                                                                            1
                      馬                     加
                                                            J
                                                                                                           1
                                                                                                                             m   加
                                                                        1
                                                        U
                                                                                                       1
                                                                    \
                                                                                    \              /
                                                                                                   /
84    Ch. 5 / Miscellaneous Codes

This is equivalent to the three equations

                                           i
                                           D
                                            l
                                            14



             += +
                          l
                          百V   P
                               口                 D
                                                 1       l
                                                         寸4   P
                                                              C
                                                                  P
                                                                  口


             小 1
                          l
                          43   P
                               口
                                            l
                                            百二   P   b   l
                                                         14   P
                                                              C
                                                                  끄
                                                                  b



                          吉／7. + 吉／7b + {PC = PC

or
                                                                  0
                                       P P +
                          n
                          二1
                           3   P                         l
                                                         14   P
                                         b   b   b

                                               P
                               口                              C
                                   1




                          l
                          U3   P                         l
                                                         m4   P   0
                               口       l4
                                        4  l
                                           尸2  l
                                               14             C
                                                 1




                          l
                          m3   P
                               a
                                       += +=
                                       +
                                                =        l
                                                         U2   끄
                                                              C
                                                                  0


Only two of these three equations are independent, so we solve the top
two with the side condition (the one nonhomogeneous equation)

                           Pa + Pb + Pc = 1

After some algebra ＼자e get 如r the eq恥茁brm恥季岫的河

                      ／乙 = 큐，                        Pb = PC = 슈      (5.2-3)

Thus, regardless of what state distribution we start with, for this tran-
sition matrix (5.2-1) we get the same equilibrium state distribution
(亮 유, 유). Note carefully that we will be in some definite state-
these numbers are probabilities only!


万工ercises

5.2-1 Compute the fourth and eighth powers of the transition matrix
      (5.2-1) and compare the variabilities of all four matrices.

5.2-2 Starting with the square of the transition matrix (5.2-2), compute
      the equilibrium state distribution.


5.3 Ergodic Markov Processes

,The Markov process above is called ergodic-from any state we can
 get to any other state, and in time the system settles down to a limiting
1distribution independent of the initial state. This does not mean that
 for the matrix above the weather in time becomes a mixture of fair
                                 Sec. 5.3 / Ergodic Markov Processes       85

rain, and snow, but only that in the long run our expectation settles
down to a probability mixture of the states. The long-term probabilities
are independent of today's weather.
      There are many other types of Markov processes. For example,
Figure 5.3-1 shows a nonergodic graph. We see that once we leave
state a, we will never get back there. Depending on which path we
first take, we may go to the single ending state d, or else end up going
around three states g, h, and i. We do not expect that this kind of
graph will be a good model of an information source, so we will set this
type aside.




                       Figure 5-3.1 Nonergodic graph

     Even if we do end up in a set of states for which we can get from
any one to any other, it does not mean that the probabilities settle down
to a single number. Consider, for example, a checkerboard with the
transitions being up or down, or left or right, but not diagonally. If we
start on a red square, we will find that after an even number of transitions
we are on a red square, but for an odd number of transitions we are on
a black square. Thus there is an alternation of probabilities for each
color of the current square. The theory of all possible Markov processes
is therefore messy in principle, but the Markov processes we care about
for information systems are ergodic and do not have these peculiarities.
In the long run the message symbols settle down to fixed probabilities,
although as noted above, not to a mixture of actual symbols but to a
probability distribution. It is easy,for example,to understand the words
"terminal state" and the words "a set of terminal states." And it is
easy to see that if the terminal set is not all the states of the system, the
system is not ergodic in the sense that we can get from any one to any
other. Furthermore, we must avoid any alternation of states. For any
information source that we may have to encode, we expect to have an
ergodic source, although it is not completely impossible that other sys-
tems could occur. The complications, if they do arise, are not difficult
86    Ch. 5 / Miscel／口neous C야加S

to work out.     We shall assume in the future that all our systems are
ergodic.


Exercise

5.3-1 Given the symbols 0 and 1, draw the one-, two-, and three-memory
      Markov diagrams.


5.4 Efficient Coding of an Ergodic Markov Process

It should be immediately evident that we can use the Markov structure
of the source to improve the encoding of the source. For each state in
the Markov system we can use the appropriate Huffman code obtained
from the corresponding transition probabilities for leaving that state.
Depending on how variable the probabilities are for each state, the
encoding will gain a lot or not. However, as we increase the order of
the Markov process, we tend to gain less and less while the number of
states approaches infinity rapidly.
     Let us do this Huffman encoding for the weather matrix of Section
5.2. For state a (today) we get (tomorrow) the binary encoding




                            P P P
                                        l
                                        13
               口 = 1          n
                                                                        =


                                        l
                                        m3
               b= 00          b                 L, = 亨 = 1.6667 . . .   1 H




                                        l
                                        13
               C = 01         r
                                                                        =




For state b,




                                    P P P
                                             l4
                  a = 10              口

                                             l
                                             百七
                  b= 0                b              Lb = 클 = 1.5
                                             l4
                  C = 11              C



For state c,




                                    P P P
                                             l4 l4
                   a = 10              口

                   b = 11              6             Z』, = 글 = 1.5
                                             l2
                   c= 0                r




At equilibrium we get [using the equilibrium probabilities (5.2-3)] the
average code length

               (ai ＝츄LO + 슈Lb + 유i』
                                  . = ｛子 = 1.5454 . . .
                          Sec. 5.5 / E工妃nsi（가is of a M口rkov Process    87


     On the other hand, let us code the average frequencies of the letters
a, b, and c. The probabilities are clearly the equilibrium probabilities
(5.2-3)                                     枷｛ 卜m，小 C-小，  H
                                                           寸    '




                   Pa = 슈        Pb = 슈      PC = 슈

The code is



                                        mml
                               =    q
                               b
                               ==
                               1

                               1
                                    C


We get, therefore,

                     L = 큐（2) + 유（2) + 슈（1) = 쀼

      Thus the average code length LM for the individual state encoding
is less than the encoding L of the average frequencies

                           LM = 뀨 ＜二 쀼 = L
                                                            I
As we expect, the Markov-state system shortens the average code length.
The gain would be much greater had the probabilities been less uniform.



Exercise

5.4-1 If the fair weather a has probabilities p(a I a) = 긍, p(b 1 a)
       = p(c 卜a) = 吉， and the others are the same in this section, show
      that ／小／ = 菅 < 首 = L.




5.5E工比n缸이is of a Markov Process

We have already (Section 4.2) defined an extension of a source. For
example, the octal code is the third extension of the binary code. In a
sense, an extension is simply a concatenation of the source symbols into
longer symbols. We need to examine the extension of a Markov proc-
ess.


    Definition. If S is an mth-order Markov information source with
alphabet s, s2. . . . .sq, and if its transition probabilities from one of
 88      Ch. 5 / Miscellaneous Codes

 the qm states to the next is given by

                                                   p    (s1
                                                                1 s1, SJ2.   ,                 .   .   .
                                                                                                           .       s/,,,)                                (5.5-1)

then the nth extension of this source is labeled S" = T with q" symbols
t1, t2, . . . , t4. Each t is a sequence of n symbols from the alphabet
of S. The system S" is a kth-order Markov process where k is the first
integer greater than or equal to (rn/n). Since each t, corresponds to
some sequence of n of the 易, the conditional probabilities of T,

                                                   p(t, I til' i J2' . . . , t,k)                                                                        (5.5-2)

can be obtained from the original transitional probabilities of S by pre-
dicting one s, at a time while looking back at rn earlier symbols. Re-
writing (5.5-2), we have for (kn 之 m) and repeated applications of
(5.5-1),

p(s11, SZ2, . 1 . , Si, 1 Sj1, Sj2, . . . ,

                      = p(s,, 1 si,, SJ21 . . . , si, ,) p(s,2 1 J2, SJ3 . . . , s1, ,, s.,)

                       .   .   .   p
                                             (s1
                                                        ,     1 si   ,   .   ,,,,        Si, - m . ,,          .        .        .        ,   s1
                                                                                                                                               ,_
                                                                                                                                                    ,)
This product assumes n > m; if not, the last term would be

                                   p   (s1
                                                    ,         1 s/ S/
                                                                ,,               ,   .    :,   .   .   .   ,       s,
                                                                                                                            ,_       1)
     The formalism is more complicated than the idea! We will need
the results of this section later.



5.6 Predictive Run Encoding

We have just shown how to use the transition probability structure of
the messages to reduce the length of the encoded messages; the simple
frequencies of the separate input symbols can be used to design a Huff-
man code, and the Markov process can handle the larger correlations.
Besides these, there are many other possible structures of the input
messages that could be used to shorten the encoded message, but they
are far too numerous to investigate in detail in this text. Instead, we
examine the general case; we assurne that you have either a program,
                                    Sec. 5. 7 / The Predictive Encoder   89

or some hard-wired equipment, that can recognize the patterns to be
used to predict the next symbol. For simplicity we assume a binary
source. Using this program, we will then encode the input stream of
binary messages into a corresponding binary stream which has relatively
long runs of 0's separated by comparatively few l 's. The better your
ability to predict the next symbol, the longer will be the runs of 0's.
The stream of 0's and l 's is followed by a second stage of encoding,
where the code compression occurs. We will send a stream of numbers,
each number giving the length of the corresponding run of 0's, and the
receiver will be able to reconstruct the original message using equipment
almost exactly like the encoder.



5.7 T九e Pred加作ye 月ncoder

 Whatever the pattern of the input message that you can recognize and
use to predict the next symbol, we assume that you have written a
program to do this. You are merely required to predict the next symbol
in the input stream. Your predictor can be a fixed one, or it can be
 "adaptive" in the sense that it can gather statistics about how well it
does, and from them make modifications to itself. It can be linear or
nonlinear-nothing is being said about how you do the predicting.
     It is necessary to emphasize the generality of the program you are
supposed to supply for your particular application. The method we are
going to discuss makes the single assumption that the program predicts
the next input symbol correctly most of the time. The better the pre-
dictions are, the more the input message is finally compressed.
     As shown in Figure 5.7工 there is a source S of input symbols Si.
In part (a) there is a predicting program in the rectangular box labeled
P which predicts from the stream of symbols si (for i < n) the predicted
symbol p, . Assuming that both input and output are using the binary
system of 0's and l 's, we logically add the two current symbols, input
s, and predicted p, , to get the error e,i of the nth prediction. The output
symbol en is a 0 whenever the prediction p, is the same as the input
symbol s, , and a 1 when the prediction is wrong. The predictor P also
gets the error messages en and is therefore in a position to correct itself
and to know exactly the past message stream up to the next prediction.
     As noted, if the predictor is fairly good, there will be a stream of
0's with an occasional 1 here and there. A random predictor would
have half 0's and half l 's. Even a poor predictor would have many
more 0's than l 's.
  90        Ch. 5 I Miscellaneous Codes




                                P




       Sn
 Source                                                         Stream of
                                                                U's and 1's

                                            (a)
en                                                                      en
                Encode                            Channel   Decode




                                            (b)




                                      (c)
                         Fi昏1re 5-7.1 Predictive encoding


 5.8 The Decoder

.,At the receiving end (Figure 5.7-ib) there is a decoder, which is essen-
  tially the same as the predictor. Assuming that the box labeled P is
  identically the same as the box in the encoder, then if the two start out
                                                       Sec. 5.9 I Run Lengths   91

 in the same state, it follows that each will make the same predictions.
  When a 1 comes to the decoder in Figure 5.7-ic, it logically adds this
 error to its prediction and thus the correct output emerges. Again, the
 error message e,: is supplied to the predictor. The slight difference
 between the form of the information at the two ends requires only slight
 modification to the equipment; thus the two ends of the signaling system
 are essentially the same.
       We need to model the situation in mathematical symbols so that
 we can evaluate how good it is. Let p be the probability of the predictor
P being right for each symbol. (Note the reversal of the role of p; it
 is now the probability of being right.) We assume that the probability
 is a constant since otherwise there is a known structure that you should
have incorporated into the predictor. For the same reason we assume
 that each prediction error is independent of the others. Your formula
may, of course, be recursive; it is the errors we are assuming are in-
dependent. Let 1 - p = q be the probability of guessing wrong.
Naturally, we assume that p 之 { , since otherwise we would simply re-
verse the symbols p and q by complementing the predicted 0's and l 's
and have a suitable p.
      These probabilities are not to be confused with the errors in the
equipment; they are associated with the predictor P. Because of the
foregoing assumptions about the predictor, the output stream of 0's and
l 's has a fixed probability of error and adjacent positions are mndc-
pendent. The prediction errors are "white noise" (Section 2.4). A
large p means a good encoder; a p near 글 means that you are doing
hardly better than guessing.



5.9 Run Lengths

The probability p(n) of a run of exactly n 0's is (since each run of 0's
ends with a 1)

                   p(n) = pflq             (n = 0, 1, . . .)

Summed over all lengths n, we have

                                                   q
                                                             口
                                                             三 q
                                       P
                2p'q = q
                                       n
                                   2
                                               l   小
                                                        P          1
                               M
as it should be.
      Suppose that for the moment we decide to send a k-digit binary
number to represent a run length. For a reason we will soon see we
can do this only for run lengths 0 to 2" 中 2. At the receiving end the
92      Ch. 5 I Miscellaneous Codes

receiver copies down the indicated number of 0's and follows this by a
1. If the sent number is 0, we simply copy down a 1. For the binary
number (2" - 1) the receiver copies down (2k - 1) Os and does not
copy down a 1. If the next number sent is 0, then of course a 1 is
copied, and for any other number that number of 0's is copied followed
by the 1. Thus we can send any length of a run of 0's we need by
sending a sufficient number of k-digit binary numbers, k > 1.
     We shall not attempt to use a Huffman coding system. In the
original case we have a potentially infinite input alphabet, since in prin-
ciple any run length could occur; after "blocking it" into runs at most
k digits, we could, if we wished, use Huffman encoding.
     Returning to the proposed method, what is the expected number
of digits sent? To find out, we need to sum the probabilities of occur-
rence times the number sent in each case. Thus we construct the table

                      Length of Run              Number of Digits Sent

                0 드 n 드 (2' 小 1) -i                        k
            (2k - 1) 5 n 드 2(2k - 1) - 1                  2k
           2(2k - 1) 5 n 드 3(2" - 1) - 1                  3k
                               etc.


     The expected length is [setting 2" - 1 = m and p(n) as the prob-
ability of a run of exactly n 0's]

                [p(O) + p(l) + . . . + p(m - 1)]k

             + [p(m) + p(m + 1) + . . . + p(2m - 1)]2k
             + [p(2m) + p(2m + 1) + . . . + p(3m - 1)]3k
             +.   .   .




Since

                                       可미 = pflq

we get

                            q[1+ p+ . . .     +pm_ l]k

                          + qpm[i + p + . . .      + pm- '12k

                          + qp2m[1 + p + . . .     + pm-l]3k
                          +.   .   .
                                                                                                     Sec. 5.9 / The Predictive Encoder              93

Summing the terms in brackets, we arrange the expression in the form.

                                                                       p
                                                                                                     + 2pm + 3p2m
                                                      11
                                                q
                                                              -,
                                                                           ml
                                                                                               [1
                                                      L
                                                                   q                       j                                 ·   .




This sum is, in turn,



                                               q[" , "' ][(, -',小 1느
We need a short table (Table 5.9-1) of the function (k > 1)

                                                                                                          k
                                                                                               1 - J7(2" l)




                                                                                                                    人H   入m//
                                                                                /\/\/＼小니
so that for a given p 之 吉 we can pick the best k (Table 5.9-2).

                                                                                                      可
                                                                                                      砒
                                                                                                      兀
                                                           TABLE 5.9-1



                                                                                                              p
k                      0.5                     0.6                 0.7                              0.8           0.9     0.95        0.98       0.99




 八
 乙 八4U 4 <
         V 6 m
                       2.29                    2.55




             / 8 9 0
                                                                   3.04                             4.10          7.38   14.0        50.0    67.3
                                                                   3.27                             3.80          5.75    9.94       34.0    44.2
                                                                                                    4.15          5.04    7.45       22.7    28.6
                                                                                                                  5.20    6.28       15.3    18.7
                                                                                                                          6.25       10.7    12.8
                                                                                                                          7.01        8.33    9.71
                                                                                                                                      7.58    8.67
l                                                                                                                                     8.05    9.05



                                               TABLE 5.9그 Table 可司／'C加nCy 可Encoding

                                                                       Expected
                                                                       Number                                 Expected Length        Compression
 p                     Optimum k                                       of Digits                                  of Runs              Ratio




                              n乙 nJ 4
                                    1 6 m/ 8
0.7                                                                             3.04                                  3.33               0.91
0.8                                                                             3.80                                  5.00               0.76
0.9                                                                             5.04                                 10.00               0.50
0.95                                                                            6.25                                 20.00               0.31
0.98                                                                            7.58                                 50.00               0.16
0.99                                                                            8.67                                100.00               0.087
 94    Ch. 5 / 凡fiscel／口neous Co（加S

      The number of encoded bits in the string of 0's and 1's for a run
 of length is n + 1; hence the expected length of the encoded runs is


            各（4『
             (n+1)
                1)/"
            p1= 。 p《q=＝ q
                       《＄小(n+
                           『1「1p)") =q
                                    ＝《（,(1-1 p)2 q
                                                 n= 。



      Suppose that we compute the variance. We get
                                         l
                                         J
                    X
                    2山
                                                 2
                                                     脚
                         1
                                             \
                                                     +
                                         Hq
                                 n
                                     1
                         r
                                                                                 1)'「
                                                                              『+ i)
                                             J
                                                 +




                                                         =




                                                              ［
                         1
                                                                                                   -
                                                                     (n
                                                                     (4
                                                         如2   q>                                       1
                                                                                               "
                                                                                        2pfl
                         \   \               /
                                             /
                                                         ＝    『    ' ,    二   "   ]++
     From these tables we see that the efficiency of the run encoding
 depends on the choice of k, and for optimal design this in turn depends
 on p. Evidently, it is easy to select an appropriate k when p is given.


 Exercise

 5.9-1 Discuss the use of Huffman encoding of the run of zeros.



 5.10 Summary of Predictive Encoding

'Because of the generality of this scheme of message compression it is
 necessary to emphasize both that it does not do everything, and that its
 efficiency depends completely on the predictor that is supplied. The
 better the predictor, the longer the runs of 0's and hence the compression
 at the second stage of encoding. The generality of the predictor is
 unlimited in theory, although in practice it must be simple enough so
 that it can keep up with the stream of the input alphabet. All it has to
 do is predict the next symbol in the input stream. How it does its job
 is not a part of the theory. If the encoding is to run in real time, then
 there are buffer-size problems, but on a computer problem this is not
 a vital p아nt.


 5.11 What Is Hashing?

  건뺀쁘완s a method of redu如gJ坐뜨如ndan아 可 an e毗岫le of 刃i
  ,messages that have been selected from a much large ensemble of M
;i1 ible messages. It is, however, a reduction in a particular sense
   only.
                                      Sec. 5.12 I Handling Collisions    95

      To make matters specific, consider the ensemble of names of peo-
 pie, the names of variables in a FORTRAN program, or any other rich
 source of names. In any particular application, payroll, FORTRAN
 compilation, or other processing of the names, we expect to have only
 a very small sample from the ensemble of possible names. Suppose,
 to be definite, that we expect to have 500 names. We will assign 10
 bits (210 = 1024, which is more than twice 500). For each name we
 will take the first 10 bits, do a logical addition of the next 10 bits, the
 next 10, and continue to the end of the name (padding out the last 10
 with 0's if necessary). This process generates a unique "hash" sum from
 a given name, but of course two different names could generate the
 same hash sum.
      Given this original name, we place in a hash table at the computed
 10-bit hash number location (perhaps with a constant added) a pointer
 to the original name. As a result we have a table of pointers back to
 the original names, but the table allows the direct location of an item
by simply going, via the hash table, to the calculated location rather
than by a search through the table of names to find the required name.
      What is the probability of two different names leading to the same
hash sum? If the hashed names were random, and that is what we are
trying to do by the logical addition of each 10 bits, there are approxi-
mately글 times 5002 possible collisions. Like the famous birthday prob-
lem where 23 different people gives a probability of more than half of
at least one duplicate birth date, the probability of at least one collision
is very high. Yet the probability of any one name having a collision
with any other name is less than 吉, since we have more than twice as
many name locations in the table as there are names. Thus the typical
name when hashed (encoded) into the 10 bits has less than half a chance
of having a collision with any other name; still some collision in the full
500 names is highly probable. We must, therefore, allow for them.



5.12 Handling Collisions

How shall we handle collisions? A simple method is to go to the cal-
culated (hashed) place and if this is empty, we make the entry; but if
it has an occupant, we look down the table and insert the new entry in
the first empty location that follows. This means that when we look
for an entry at a later time we have to look not only at the computed
place, but if the pointer there does not point back to the correct name,
we must continue looking at the consecutive nonempty places and check-
ing if their pointers give the name until we come to either a match or
else a blank. In the latter case we know that there is no entry corre-
96     C/i. 5 / Miscellaneous Codes

sponding to the given name. If we want to make a new entry, as we
would in a FORTRAN compilation, we enter it in the empty location.
In this way we can construct a table of hashed names.
     Of course, if we knew all the names in advance, we could find a
particular encoding that would avoid collisions. But if we either have
to handle a growing table of names, or else do not want to spend the
time to find a special encoding, this approach, through what can be
called "random encoding," is useful.


5.13 Re刃wvals fro刃i i力e Table

In some problems it may occasionally be necessary to remove a name
from the file of names. This would not happen in a FORTRAN corn-
pilation, but it does happen in some applications. How can we do this?
Evidently, we compute the address of the name's pointer and if it is
there (or in some following location), we remove it. If there is an
occupied cell following the removed one, we must look to see if when
it was entered it had been moved down, and if so we must move it back
up. Indeed, we must examine all the successive entries until we come
to a blank, to see how each should be placed. This is simplest done by
constructing a pseu面file of names from the f에O帥垠 a미配帥tp이nters,
and simply reentering them. In this fashion we can keep a file of
computed names up to date.


5.14 Summary of Hashing

We see that given a collection of names that may individually be rep-
resented by very long (or possibly only occasionally very long) strings
of characters, we have compressed them into a length that is slightly
longer than minimum. The use of more than minimal redundancy de-
creases the frequency of collisions and the attendant waste of computer
time, and it is an engineering decision as to how many more than the
minimal number of bits to use. In our example we used one extra bit
and had half the cells of our table empty. The use of two extra bits
would greatly decrease the number of collisions, but would double the
space of the table in storage.
     We see that the random encoding is based on the number of entries
expected but not on their detailed structure, and this allows the use of
a greatly compressed table which can be used in a direct lookup fashion
rather than a searching fashion. We have substituted computing power
(the hashing algorithm) for searching, since we go directly to the corn-
                              Sec. 5.15 / Purpose of the Gray Code     97

puted address, and with at most some local fiddling around we find the
entry, if the entry exists.
     This random encoding is based on the idea that the hashing algo-
nthm we used gives random encodings. Certainly, two names that differ
by a single letter will still be separated. It will only be by chance that
two fairly different names will collide. The hashing algorithm we used
is a very simple one, and there is an extensive theory for how to design
a hashing algorithm for various kinds of data (Ref.[K]). The one we
used is clearly fairly effective, but probably could be'improved upon.
We will not go into this point further. We are exploiting the fact that
random encoding produces a degree of uniformity from an unknown
but structured source-it tends to spread out bunchings.
     The main results we want to emphasize are two. First, this is a
useful method of encoding data for some purposes; it reduces the re-
dundancy without actually having the redundant structure of the messages
(names). Second, this is an example of random encoding, a concept we will
need in Chapter 10.


5.15 Purpose of the Gray Code

Another important code is the Gray code. It is designed to meet a
common need which is best described in terms of a particular application,
although it has wider uses. Suppose that we have a rotating analog
wheel (see Figure 5.15-1) and have a number of brushes rubbing on the




                  Figure 5-15.1 Eight-sector binary wheel
98    Ch. 5 / Miscellaneous Codes

wheel (or lights shining), each on its own track. In order to record how
far the wheel has rotated, the tracks are divided into sectors. For the
typical binary system the number of sectors would be a powerof 2, thus
giving rise to a binary number of n digits. There are, of course, n
tracks, one for each digit (the figure has three tracks).
     If we use direct binary coding of the sectors, then when the wheel
moved from, say the binary number 011 to the next binary number 100,
each of the three brushes would find that its value changed. Suppose
that we tried to read at the moment of changing sectors. We could
expect any number to emerge from this attempt to read.
     The Gray code is a method of encoding for which successive num-
bers change by only one position all around the wheel. Thus the attempt
to read when the brushes are between two sectors can give only one of
these two numbers, and no large error will occur.


5.16 Details of a Gray Code

We have just effectively defined a Gray code, but the definition does
not give a unique code. In practice we use one simple version, usually
known as the Gray code.
     The definition of the Gray code is made inductively. For a one-
digit code we have the two states, labeled as 0 and 1 (see Figure 5.16-
1). Notice that in going around the circle we also have the transition
from the 1 to the 0 that occurs in going from the bottom of the column
to the top. Imagine these as a column. Below these two we write the
symbols in reverse order, and attach to the first two a leading digit 0
and to the last two a leading digit 1. Examination shows that as we
pass from the original set to the new set, we change only the leading
digit from a 0 to a 1, the other digits being a copy. All the rest of the
new symbols also change by one place only because they are the same


             d
                           （年
                     01




                          Figure 5-16.1 Gray codes
                                        Sec. 5.18 / Anti-Gray Code     99

as the original except in reverse order. The transition from the last to
the first is a change in only the first (attached) digit. In the figure we
show the process of going from one to two digits, from two to three
digits, and part of going from three to four digits.


Exercise

5.16-1 Show that for a four-binary-digit code, there can be different
       codes with the basic property of changing only one digit in going
       to the next sector.



5.17 Decoding the Gray Code

The numbers that come from the coding wheel of an analog device are
typically in the Gray code, and we usually need them in the binary code
if we are to process them in a computer. Reading from left to right we
take all the 0's as being correct and also take the first 1. But the next
position should be complemented. If this position is a zero, we continue
complementing, but if it is a 1, we complement it and stop comple-
menting until we pass another 1. Thus the number of earlier l's we
met controls whether we complement the next digit or not. We corn-
plement on an odd number of earlier l's and do not complement on an
even number of l's. This simple rule, together with the general sim-
plicity, makes the particular code the favorite solution to this problem
of having only one digit change between successive numbers. The state
diagram is easy to prepare.


Exercises

5.17-1 Make a state diagram for decoding the Gray code.

5.17-2 Describe the rule for going from binary to Gray (for simulation
       modelrng).



5.18 Anti-Gray Code

One day when I was reading a journal, I noticed a paper which observed
that when testing a memory device it might be a good idea to arrange
the memory addresses such that the switching tree has as many changes
as possible. Shortly after this point I set the paper down and began to
1伽1     Cli. 5 / Miscellaneous Codes

 think about just what the problem was (since I noticed that the paper
 was rather heavy going).
      It is evident that in going from one address to the next, the l 's
 complement would have the most changes. Next, it is evident that two
 successive complements would get back to the same address, so the best
 that could be done is that one stage of complementing be followed by
complementing all but one position. This, in turn, means that taking
every other address would form a Gray code. On the average of the
k possible bits you have k - 글 bits changing in the switching tree.
This is a good example of the rich variety of useful codes that are
possible, and that once you are reasonably familiar with a wide variety
of codes, it is easy to develop others to meet your specific needs.
      To fill in the details, if you have a k bits for the address of the
memory you are testing, you first construct a Gray code on k - 1 bits
and append a leading 0. Then you interpolate the complement of each
address immediately after the address. No new address can be ah old
one because all the old ones begin with a 0 and all the-complement
addresses begin with a 1. No two complement addresses can be the
same because then two of the original addresses were the same. Thus
you will have 2" distinct addresses in the final code.
     For example, if you want a code for a 4-bit address, you begin with
the 3-bit Gray code with leading 0's. You then get

                     Original
                                       \            lev
                                uray   1           L ouc


                                0000       0000      (     0110
                                0001       1111      1     1001
                                0011       0001      I     0111
                                0010         110     J     1000
                                0110       0011      1     0101
                                0111       a.100     j     1010
                                0101       0010      I     0100
                                0000       1101     1      1011


     An alternate idea is simply to reverse the order of the address bits
so that adjacent numbers are placed far from each other. This can be
useful if you have different storage banks in a very high speed computer.



5.19 Delta Moduli玎U刃1

Another method of encoding is to send the difference between the
current signal and the previous signal. For slowly changing signals this
                                                       Sec. 5.20 / Other Codes          101

means that typically, you can send fewer digits. When changes occur
that are more rapid than the method can keep up with, the transmitted
signal falls behind, but with suitable terminal equipment this loss will
be made up in time (Figure 5.19-1).

                                                                       Back on
                                                                        signal


                                   Signal


                                                                  卜，       .   step
                                                            Max. step
             /'




                                                     Max. step

                                         }Max.
                                                     step




        I         1   I              I           I      I     I        I              기me
      n= 1        2   3   4   5     6            7      8     9        10

                                  Figure 5-19.1

     Thus you send

                              스yn = yn - y小l

and use fewer digits in 스y than in y月. The method is widely used with
suitable modification to combat noise.


5.20 Other Codes

A topic of some interest is that of resynchronizing a decoding system if
a single symbol is either lost or is added to the stream of digits coming
into the receiver. In a Huffman code we could be in some trouble, but
usually, the receiver will resychronize fairly soon. But how long it will
take on the average is not a simple question, although it has been
investigated in some studies. Evidently, in any particular case a Monte
Carlo simulation of a code with errors can be run, and from the simu-
lation suitable conclusions can be made. Within a computer these syn-
chronization errors are not likely to occur-only a changed digit is likely.
102    Ch. 5 I Miscellaneous Codes

     One way of avoiding resynchronization problems is to use a parallel
channel. Another way, when using serial transmission, is to embed the
message in a longer block with synchronization pulses at both ends.
This, of course, wastes capacity, but it does catch spurious pulses.
     With the current low cost of accurate crystal clocks it is common
practice to use clock pulses either from a single clock, or by keeping
several clocks in synchronization, so that both the sender and the re-
ceiver have the same timing pulses.
    The topic is not of enough general interest to do more than point
out the problem and the obvious solutions. Many other methods of
code compression can be found in Ref. {DG].
 （沇a刃ter 6




                            Entropy and Shannon's
                                                First T九e아e刃1




 6.1 Introduction

  Up to this point we have been concerned with coding
                                                             theory; now we
  begin information theory. Coding theory answers the
                                                             questions of (1)
  how to design codes for white n아se{mainly), and
                                                       (2） 上to쁘起工0皿恥르S旦
J he message when the probabilities (structure) of the messag
                                                               es are known.
       We now need a general method for measuring the
                                                             structure of the
  source. To do this we introduce the concept of
                                                   entropy. While entropy
  was used long ago in many physical situations, 크nd the
                                                               concept in in-
  formation the y ars a strong resemblance to the
                                                         classical definition.
  we shall study entropy on its own merits in this particular
                                                                field, and not
 get involved in the various suggestive analogies.
                                                         For us, entropy is
 simply a function of a probability distribution pi. For
                                                            some analogies,
 see Refs. [Ga], [Gu], and [ME].
      Information theory combines noise protection and
                                                             efficient use of
 the channel into a single theory. However, the simple
                                                           model of channel
noise (white noise) is sometimes unrealistic, and
                                                       we will occasionally
 treat more general patterns of errors. 工h竣起
                                                 奭立to血e．立fl (江與nt르凹，二
cPU正c/ qi？坦l照P ' y, which is taken up in Chapter 8.
     ,1'he result we are headed for is Shannon's main theore
                                                                m in Chapter
10, which gives a relationship between the chann
                                                      el capacity C (to be
defined in Chapter 8) and the maximum rate of
                                                   signaling possible. We
will prove the remarkable theorem that we can come
                                                            arbitrarily close
to the maximum rate of signaling and also achiev
                                                       e an arbitrarily low
rate of error. In a sense this achieves both
                                              Huffman-tvpe compression ,



                                                                         103
  104        C/i. 6 I Entropy and Shannon's First Theorem

  and Hamming-type noise protection in the same code. Unfortunately,
  the proof is not constructive, so that while information theory sets the
  bounds on what can be done, it does not tell us how to achieve them.
  Yet, as we said in Section 1.2, the theory is very useful.
      In this chapter we prove a very special case of the main theorem,
  namely the noiseless coding theorem, where we ignore the problem of
  noise. When this theorem and its proof are understood, the proof of
  the main theorem will appear a bit clearer-once a lot of preliminary
  mathematical results are covered in Chapter 9.



  6.2 Information

    Suppose that we have the source alphabet of q symbols sl, S2, · · . , s,,
    each with its probability P(Si) = Pi' P(52) = P2' . . . ' P(5q) = Pq·
    When we receive one of these symbols, how much information do we
    get? For example, if p1 = 1 (and, of course, all the other p, = 0), then
    there is no "surprise," no information, since you know what the message
    must be. On the other hand, if the probabilities are all very different?
 P then when a symbol with a low probability arriv 二 you feel more sur-
  . D " d,了et more information, than when a symbol with a higher prob-
 中abi1ity arrives, Thus information is somewhat inversely related to the
    probability of occurrence,
         We wish to construct this function 1(p), which measures the alpount
    of information-surprise, uncertainty-in the occurrence of an event
    of probability p. We assume three things about 1(p).


        ft    0 real nonnegative measure)
味：本J 三. 八P1P2) = 八．Pi) + 1. p2).tOr inciepenoent events (aouiuve).
   -          1   (p)   之   .   (a,                   .        .       .   .   .   ..   .   .   .




        '了. I ( ) is a continuous iunction 01 p.

        The second of these conditions is known as the Cauchy functional
   equation for the function 1(p), meaning that it serves to define 1(p).
   If p1 and p2 are both the same number p. not necessarily the same event,
   then

                                      （쓰LJ伽） + 1(p) = 21(p
                                      1

   Now if Pi = p and P2 = ／尸, then we have小

                                      1(P3). = I (P) + 1(p2) = 31(p)
                                                    Sec. 6.2 I Information       105

and in general we have

                                   I(pfl) = ni（끼 沁『
We recognize that the standard law of exponents for positive integers
applies to the function 1(p). Following this clue we adapt for our needs
the usual exponent extension to fractional values. We set

                               pfl = y,        p = ylln

and hence


                                   I(y)『 n1(y11'）工r，景）
                                                     ，劣，ci.E뎌宬）
or, after some further manipulation,                       0             t




                                               m
                                                               =   ml   （肝   )
                                   J(ym/n) =
                                               n   幻）          二 恥m
Thus for the rational numbers the function of I (p) obeys the same
formula as the log function. Assumption 3 of continuity allows us to
extend this to all numbers (0 5 p 드 1), rational or irrational. Thus we
have


                                   프可二츠坐르r
for some constant k and some base of the log system. From the first
assumption it is natural to pick the constant k as 小 1, and we have,
finally,


                         1   (p)    =
                                        나.   gp =   log二
for some base of the log system.
     Let us examine and illustrate this additive property 2 that we as-
sumed, since it plays so central a role in deriving the measure of sur-
prise. Consider the simultaneous and independent toss of a coin and
roll of a die. We feel that each outcome (coin and die) has no influence
on the outcome of the other. The coin has two equally likely outcomes
and the die has 6. The product space of the two independent trials has
12 equally likely outcomes. If ci is the outcome of the coin and d1 is
106     Ch. 6 / Entropy and Shannon's First Theorem

 the outcome of the die, then the derived formula of 1(p) is

                               l (c1d1) = 1(c) + 1(d1)

                               log 솔 = log { + log 吉

which is, of course, true.
     The words "uncertainty," "surprise," and "information" are re-
lated. Before the event (experiment, reception of a message symbol,
etc.) there is the amount of uncertainty; when the -event happens there
is the amount of surprise; and after the event there is the gain in the
amount of information. All these amounts are the same.
     This is an engineering definition based on probabilities and is not
a definition based on the meaning of the symbols to the human receiver.
The confusion at this point has been very great for outsiders who glance
at information theory; they fail to grasp that this is a highly technical
definition that captures only part of the richness of the usual idea of
information.
     What base of the log system shall we use? It is simply a matter of
convention since any set of logs is proportional to any other set. This
follows directly from the fundamental relationship for logs:

                                =   log,        ,   x
                           x                            =           b)   log,   , x
                                                , a
                    logO
                                                            (logO
                                           g,
                                    l。
     It is convenient to use the base 2 logs; the resulting unit of infor-
 mation is called a bit (binary digit). If we use base e, as we must
 whenever we get into the calculus, then the unit of information iscalle立
.a nat. Finally, sometimes the ase lO is used and the unit is called a
 Hartley. after R. V. L. Hartley, who first proposed the use of the
 logarithmic measure of information.
      We are using the word "bit" in two different ways, both as a digit
 in the number base 2 and as a unit of information. They are not the
 same, and we shall be careful to say "bit of information" when we mean
 that definition and there could be confusion.
      It is easy to convert logs from one base to another using


           log1。2 = 0.30103 . . .                           log2 10 = 3.32193 . . .

           log1。e = 0.43429 . . .                           loge 10 = 2.30259 . . .

            loge 2 = 0.69315 . . .                          log2 e       = 1.44270 . . .
                                                                        Sec. 6.3 / Entropy   107

      We have just found one solution to the Cauchy functional
                                                               equation,
 namely I (p) = log2 (lip). Is this solution unique, to within the base
 of the log system? Suppose that there were another solution
                                                                  to the
 derived functional equation

                                            J(pfl) = nl(p)

 Call it g(p). Hence we have the equation

                                      g(pfl) = ng(p)

Now take the difference of the two solutions and allow for
                                                           the constant
of proportionality C, which depends on the base



               g
                   (pfl)
                           -   C log2二 =             n   [g
                                                              (p)
                                                                    -   C log2   1]
Next, pick C as (p0 羊 0, 1)


                                      c =           g(p。 )
                                                   幻g2(l在7n)

This choice makes the right-hand side of the equat
                                                   ion above equal to
zero at Po. Now for any number z there is an n such
                                                     that (assuming Po
neither 0 nor 1)

                                               z = p8

Hence the left-hand side of the equation becomes


                                  g
                                      (z)
                                               =    C log2,

and the solution is essentially unique. The continuity assum
                                                             ption covers
the two values of p that were omitted, namely 0 and
                                                        1.


6.3 Entr까砂

If we get I (s) units of information when we receive the symbo
                                                                  l s,, how
much do we get on the average? The answer is that
                                                           since pi is thQ
probability of getting the information i (s1), then on the averag
                                                                  e we get
 108     Ch. 6 / Entropy and Shannon's First Theorem

 for each syn小이 욱，

                                                                                                1
                                p. (5') = n1.
                                「／   1
                                         (s1)              =
                                                               p,
                                                                    log2          82
                                                                                           p-
                                                                                                i



 From this it follows that on the average, over the whole alphabet of
 symbols s1, we will get


                                                    q
                                                    2日                            1
                                                     p, log2瓦

 Following custom, we label this important quantity (for radix r)



                                                                                           ()
                       r


                                                                                                         (6.3-1)
                           瓦（S)                 ＝    客p,                   log,        .



                                                                                                    -I



 and call it the entropy of                         g aling system S having symbols si and'1
中probabil      p , Of course,


                           ‘』m（分三 I-12(S) log,2

       This.is血르 entropy function for a distribution when all that is con-
 aidered are the probabilities p, of the symbols si. In Section 6.10 we will
  consider the entropy of a Markov process.
       Corresponding to each distribution P = (P1'P2. . . . .,nq) of symbols
  s, there is a single number called the entropy and labeled H (S). This
  is analogous to the usual idea of an average of a distribution小the
  average is a single number which, in some sense, summarizes the dis-
  tribution. ,工e entrpp       ( )      e weighted average of the logs of the
  reciprocals of the probabilities of the distribution. The entropy is a
  single measure of a distribution; it is the average information of the
  alphabet S.
       As an alternative approach to the entropy function, consider that
  in a long message of N symbols (from the alphabet S) you expect Np1
  of the first symbol; Np2 of the second, and so on. The probability P
  of a message of length N with these numbers of symbols is exactly

                           P = j7(I'
                               p1戶   d ' )j7(I
                                            2Pd'戶' ) . . . p目仰q)

                              = 1
                                F畔)
                                  1 r2
                                    n(P2) · · · j7q(pq)]N
                                                       J
                                              Sec. 6.3 / Entropy    109

Hence the information is



                    미計畦p, log(--)
and the information per symbol of the alphabet S is



                   口口；面’「，
which is again the entropy (as it should be).
     It is important to realize that a remark like "Consider the entropy
of the source" can have no meaning unless a model of the source is
included. Using random numbers as an example, you have formulas
for generating pseudorandom numbers. Suppose that we had a table
of such numbers. If you do not recognize that they are pseudorandom
numbers, then you would probably compute the entropy based on the
frequencies of occurrence of the individual numbers. Since pseudoran-
dom-number generators do a good job of simulating random numbers,
you would also find that each new number came as a complete surprise.
But if you knew the structure of the formula used to generate the table,
you would, after a few numbers, be able to predict perfectly the next
number-there would be no surprise. Your estimate of the entropy
of a source of symbols therefore depends on the model you adopt of
the structure of the symbols.
     The entropy function (6.3-1) involves only the distribution of the
probabilities-it is a function of a probability distribution Pi and does
not involve the s,. For example, if the probabilities are 0.4, 0.3, 0.2,
and 0.1, then from the table of Appendix B, column 3, we have


                           p        plog-

                           0.4      0.52877
                           0.3      0.52109
                           0.2      0.46439
                           0.1      0.33219

                           Sum      1.84644

The entropy of this distribution is therefore 1.84644 (approximately).
Although we should write the entropy function H (S) as a function of
110     Ch. 6 / Entropy and Shannon's First Theorem

                  p log 二．
                        r




            1.0
            0.9
            0.8
            0.7
            0.6

            0.5
            0.4
            0.3

            0.2
            0.1
            0.0
                    0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1.0

                                      이四2舌
                                      Figure 6-3.1

P, we will continue to refer to the alphabet S and write H (S), although
occasionally we will write H (P), when there are only two events, with
probabilities p and (1 - p).
    The function of p 1Og2(llp) is graphed in Figure 6.3-1. From



                                      叫小e = log2（計 log2「
      d (    .      i\       d (
      而 \p iog2 司 = 而 \p
We see both the infinite slope at p = 0 and that the maximum occurs
at p = lie, where the derivative is zero.
     We also need the property (since it is equated to zero, we can
ignore the factor loge 2)

                               urn （工 log. 工） = 0
                              t1140




To prove this, we write it as
                                                                   Sec. 6.3 / Entropy   111

 and apply l 'H6pital's rule by differentiating both numerator and de-
 nominator separately:


                    ，쁘, (-'；二：) = ,쁘, (-x) = .
     As another example of the entropy of a distribution, consid
                                                                  er the
 source alphabet S = {s1, s2, s3, s4}, where Pi = 글，
                                                     P2 = 吉, p3 = 吉, and
 p4 = 吉． With r = 2 we have the entropy

            珏（5) = { log2 2 + { log2 4 + 吉 log2 8 + 吉 log2 8
                   = () 1 + ({)2 + () 3 + G)3
                   = 1弓 bits of information

      As one application of the idea of entropy, consider the toss
                                                                   of a
 coin when both sides are considered to be equall
                                                  y likely.

                            i (功 = log2 ()             1 = log2 2 = 1
                    H2(S) = (1)i (s) + ({)I(s2) = 1

      The distribution consisting of just two events is very comm
                                                                      on. If
p is the probability of the first symbol (event), then the entrop
                                                                  y function
is



             此（P)   ＝
                              미咀
                                           （計山嶇 ! )
and is tabulated in the last column of the table in Appen
                                                                       （,
                                                                            ,

                                                          dix B. The
graph of this function is given in Figure 6.3그 Note that at p
                                                              = 0 and
p = 1 it has a vertical tangent, since


           加.g2（如（나嶇（,! ,)]
           = [m（計 小小 ! ,) 미log2 e
            如g2   （計嶇 ! )                         （,
                                                       ,
     An application similar to the coin is the roll of a well-balance
                                                                      d die
(singular of dice). We have



                        i
                            (s,
                                   )   =   log2
                                                  （計       '   如g2 6
112   Ch. 6 I Entropy and Shannon's First Theorem

           H(p)

         1.0
         0.9
          0.8
         0.7
         0.6
         0.5
         0.4

          0.3
          0.2
          0.1
          0.0
                   0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1.0
                Figure 6-3.2 Entropy function for two probabilities

and the entropy is

                  H (S) = 6[U(s3] = log2 6

                         = 2.5849 . . . bits of information

As we see from this examnie. whenever all the orobabilities are eaual,
tne average over tne atonabet is tne same as me inlormation ror any
 \/＼尸尸尸4入나小1H寸N／             尸1   J戶＼ 小니＝   dH尸＼ /＼十      ＼小＼／八       十小H尸11J

one event.
Hn而ai example of the computation of the entropy of a distribution
is the entropy of Zipf's law (Section 4.9), where the frequency of the
kth item is proportional to 1/k. Thus for N items, we have the prob-
abilities

                              m瓦     (k= 1, 2, . . . ,N)
                      Pk =

 where
                                            N
                                                l
                                                4
                                                1
                                                k
                                    N
                                   C
                                   U        2
                                            m
                                                                                 Sec. 6.3 I Entropy   113

The entropy for the N items is

                                           N
              112(N) = 小 2 Pk log2 Pk
                 누
                1 H




                      n評，[log2(斗log2 SN]
                               半1/
                                               =


                                                          (log2   1.
                                                                   82    1   -    log2   SN)   ]
                      긍，（汁느小芎｛)
                                            + log2
                          }N
                      =
                      =                              SN
where


                                           TN겯，빻
                                            八八八八스스
Using the recursive definitions

                                          Sl = 1

                                          T1 = 0

                                     SN
                                               SN     l                 l刃                                  1 H




                                                                        N
                                                                        &N
                                 TN = TNmi                              b


then




is easily computed.
     We have Table 6.3-1 (corresponding to Table 4.9-1).
     The entropy function of a distribution summarizes one aspect of a
distribution much as the average in statistics summarizes a distribution.
The entropy has properties of both the arithmetic mean (the average)
114     Ch. 6 I Entropy and Shannon's First Theorem

                            TABLE 6.3-1 Entr까砂 of Z切／노 L口w
              N                        Entropy                            Huffman Lff(N)




               2 48 垢 끄 M
                                           0.918                               1.00
                                           1.792                               1.80
                                           2.618                               2.68
                                           3.403                               3.43
                                           4.149                               4.17
                                           4.864                               4.89
             128                           5.553                               5.60
             256                           6.222                               6.26
             512                           6.873                               6.90
            1024                           7.511                               7.54


and the geometric mean. We have


                                  H(S)
                                  'v.v'v...
                                            = 2 p1 l。
                                                    g2 (I
                              (


                                           =
                                                       2嶇口
                                                                 n
                                                                 匕    "

                                                                 q
                                                                 n
                                                                 m                         H1




which is a weighted geometric mean.


Exercises

6.3-1 How many bits of information do we get from one draw of a card
      from a deck of 52 cards?

6.3-2 Forp1 = LP2 =               l
                                  14   凸       6             P
                                                             4   吉，PS = 솔， and p6 = 靑，compute
                                                   1
                                               +
                                   1

      the entropy.                                                  Ans. 孕 + 卄 log 3 = 2.34177


6.4 Mat九ematic可 Prope凡ies oft九e Entropy Funct加n

The entropy function measures the average amount of uncertainty, sur-
prise, or information that we get from the outcome of some situation,
say the reception of a message or the outcome of some experiment. It
is therefore an important function of the probabilities of the individual
events that can occur. Thus in designing an experiment we usually wish
            Sec. 6.4 / Mathematical Properties of the Entropy
                                                                Function       115




    1.0-
    0.8 기
   0.6
                                                      V = 幻ge X
   0.4 시
   0.2 -

                                 I   I   I   I   I                             x
                             1.0 1.2 1.4 1.6 1.8 2.0                       卜

  -0.2-
  -0.4

  -0.6
  七.8
  -1.0

  -1.2
 -1.4
 -1.6
 -1.8


                    Figure 6-4.1 Bound on log, x function


 to maximize the amount of information we expec
                                                     t to get; we wish to
 maximize the entropy function. To do this we need
                                                       to at least partially
 control the probabilities of the individual outcomes of
                                                          the experiment;
 we need to "design the experiment" suitably.
                                                   The maximum entropy
is increasingly used as a criterion in many situations.
                                                            Therefore, the
entropy function is worth some study for its own sake,
                                                           independent of
the particular applications we will make of it.
     The entropy function has a number of mathematical properties
                                                                        that
are very useful, and we examine them before getting deepe
                                                                  r into the
theory. A first property of the loge x function can be seen
                                                               from Figure
6.午1.
     Fitting the tangent line at the point (1, 0), we find that the slope
116    Ch. 6 / Entropy and Shannon's First Theorem

is

                                            d(log x)
                                                                1
                                               dx
                                                            =
                                                     x= 1



so that the tangent line is

                                           y-   o = 1（工 -1)

or
                                                y = 工 中1

Thus we   have
                  for
                        all x   greater
                                                 than zero the useful inequality                                                                     ,




                                          l四eX 드 x - 1                                                                                                   (6.4-1)

or
                                          log2 x 드 （工 - 1) log2 e

The equality holds only at the point x = 1.
    The second result we need is the fundamental relationship between
two probability distributions. Let the first probability distribution be
xi with of course 2 xi = 1, and the second probability distribution be
yi with correspondingly 2 yi = 1. Consider, now, the expression in-
volving both distributions


                                                                                                     칸 치
                             l。g,
                        冬J咀（斗1 ，在
                                                                                 /
                                                                                                         \
                                                                            O
                                                                    X       l
                                                                                     /
                                                                                                             r
                                                                             e           1
                                                                            Ob
                                                                                                                 1
                                                                                                     \
                                                                    1
                                                                                             1
                                                                                                                     J
                                                                        i
                                                                                                 \
                                                                                                                         /
 Using the previous relation (6.4-1) , we get



                 ,,,', 2 x log午l。gS.2 x七 1)
                                                已, ;, 拜 (yi - 均
                                                                                                                                                 0
                                                                                                                             \
                                                                                                     工
                                                                                                                                 \
                                                                                                                                     1
                                                                                                                                         r
                                                                                                         /                                   /
                                                                                                                                  r
                                                                                                                                      '
                                                                                                                                          "   ,




                  Sec. 6.4 / Mathematical Properties of the Entropy Function                                                                                                    117

Converting back to logs base 2, we have the fundamental Gibb. me:.
．쁘竺望，

                                                                                       I. 八今小小겨

                                                            각如（沙 0 ,'                                                                                   (6.4-2)



Not깹：
    ：豁哭：빴烈黑擺烈器誌如帥on
that lead to the maximum entropy (the minimum clearly occurs when
one p, = 1 and all the others = 0). We have


                                                                                         꿔ith           2j가 = 1                               刀 9

          We begin by considering the quantity
                                                                                           . 드．'ii교) 3느蜂북鈿却）
                                                                                                    '                                                 rr

                                                                                                늡뇨｝比
                                                                                                4
                                                                                                                                 t, .' ,, 月，Li.
                                                                                                                                    e1P小'7 y' 八亡j 力
                        珏（旬如2q = 枷幽小 嶇位「‘
                                                                              2 ／가 log2                                                                                     =   %
                                                                                                         八
                                        ,,'雋評
U,mgm. Gibb, m.qmlky (6.4.2) Wkhy' : l/q
                                                            H2(S) - log2q 5 0 ，茨 74，多彪列／」이 71't " "！허 붊覓 수갸
Therefore,                                                                                    能 客의 추套이
                                                                                              겊，作磁서 걷拉걍니
                                                                                           (6.4司
                                                                                                    ，吉七．
For equality in (6.4-3) we must have all the pi = 1/q.
    For an alternative derivation of this important result, we use the
                                                                                                                                                                                      J
Lagrange multipliers, and consider the function

                                                                                                                                  n
                                                                                                                         /
                                                                                                          入                                           l
                                                                                                                                                                        \
   f(p1
   ／似22，                                                                                                                         q
                                                                                                                                 口
                                                                                                                     1
                                                                                                                                  i
                                                                                                                                                                    1
                                                                          1
                  P2,
                           ·   ·.   ·.   ,,   m
                                                                              2       p loge                     1
                                                                                                                             \                              /
                                                                                                                                                                1
                                                        =
                                                                                                                                                            /
                                                                                                             \
                                              Pq)
                                                                     ge
                                                            l。
                                    [
    af=
    ap1
                          1
                        loge 2 L           （計小卜.
                                         loge                                                       (I = 1, 2, . .                                ,
                                                                                                                                                       q)
          .   .


          卜八卜X; \n人r2e
                                                    .   .


                                                    'd) (_c/ 二 =2
                                                                 .                昱      ,    1
                                                                                       R‘加4 小H仁；
                                                                                  '       ｛乙 尸
118    C力． 6 / Ent꺄）y 口nd Shannon's First Theore刃i

      Since everything in this equation is a constant, it follows that each
p1 is the same constant. Jf all the p/ are equal. each has the value ll q,
wher , as usual, the distribution has q members. Thus the maximum
entr아싸 is

                             Ha(S) = lo監了

For any other distribution than the equally likely distribution, the en-
 tropy is less than log2 q.                                  1/
      Based on this result, we now ask: What book has the maximum
information? Of course, the answer depends on the size of the book,
 the size of the type font, the variety of the type font, and so on.
Supposing these to be fixed; then the answer is obviously, the book with
uniformly random letters! Each letter will come as a complete surprise!
      This shows how far the formal engineering definition of information
is from the usual human meaning of information. Yes, the definition
of information that Shannon made is proper for computing machines,
for the telephone system, and for communication systems, but flies in
the face of the normal human meaning of information. It was the failure
to notice that the definition is appropriate for machines and for machine-
like situations, but is not appropriate for what we normally mean by
"information," that led to so many misapplications of information theory
in the early days. Now that we understand the limitations of the def-
inition we are better able to apply information theory usefully. The
very limitation of the definition to machines is what makes the definition
so useful in such situations-the definition eliminates much that is vague,
uncertain, and confusing. By limiting the theory to a sharp definition,
we can get sharp, useful results in many situations. Perhaps it would
have been better had Shannon called it communication theory, but the
title information theory is often appropriate.
      A simple, familiar application of this principle-that the uniform
distribution contains the most information-is given by the standard
grading system of A, B, C, D, and F. Setting aside F as having special
properties, namely that the student must take the course again, if we
want to communicate the maximum amount of information with the
grading system, then we should use all the other grades equally often.
 Of course, we may want especially to distinguish the very best, and give
comparatively few A's. This is, however, giving a different meaning
 to information than we have defined. The common habit in graduate
 schools of giving only A's and B's is a plain waste of signaling capacity.
 The extreme of one probability being 1 and all the others therefore
 being 0 is the case of a constant signal. There is no information trans-
 mitted. "The constant complainer is soon ignored."
                                                                 Sec. 6.5 / Entropy and Coding                                    119

       In dealing with a new situation it is often useful to look at the
. extremes that can arise. For entropy of a distribution H2(S) we get the
  least value, for one extreme, Pi = 1, and all other p, = 0- no surprise:

                        H2(l, 0, 0, . . . ,0) =0

As we proved, the maximum occurs when all the probabilities are equal,
namely
                                                l
                                                d
                                                l eq
                                                                                         l Hq
                                            /
                                                                                                          \
                                        1
                                                                                                                  m
                                                  小q
                                                                                                      1
                       H2                                  1 1
                                    1
                                                                                                                          口
                                                                                                  1
                                1
                                                                                                                      1
                            \
                                                                                           /  /
6.5 Entropy and Coding

We now prove a fundamental relationship between the average code
length L and the entropy H (S). Given any instantaneous code it has
some definite code word lengths 1. represented in some radix r. From
the Kraft inequality (4.5-1), we have

                                                K          q
                                                           2m
                                                                             /
                                                                                     l
                                                                                                              1
                                                                         r
                                                                                                                              (6.5-1)   =
                                                                                                                                        <
                                                                     1
                                                                                                                                    H
                                                                                 7
                                                                 \
We now define the numbers Q. (pseudo probabilities):

                                                      Q                                  亡K
                                                                                                                              (6.5-2)

where, of course,


                                                    2Qi= 1
                                                    1= 1


The Q, may be regarded as a probability distribution. Therefore, we
can use the fundamental Gibbs inequality (6.4-2),



                         昏log2（욧）如
Upon expanding the log term into a sum of logs, we notice that one
120     Ch. 6 / Entropy and Shannon's First Theorem

term leads to the entropy function,


                            q
                            2m
               m
               =
                   （
                   나
                                 n   O曲
                                         骨       뜨   온   .   / 1\
                                                 乙 p, log2 I ;; J
                                                 1= 1       \VV


Using (6.5-2) in the right-hand side, we obtain



                          5 2p.(1og2 K 小 log2 r ")

                          드log2 K + 2 p.!1 log2 r
                                          i= I




By the Kraft inequality K 드 1, so that log2 K 드 0. Dropping this term
can only strengthen the inequality. We have, therefore,


                       H2(S) s 2 (pili) log2 r = L log2 r

 or

                                     Hr(S) 5 L                      (6.5-3)


        L is岫比棚山的毗念h,



             斟叫非斗’4pill
毗re
                                                                    (6.5-4)


     This is the fundamental result that we need; the entropy supplies
a lower bound on the average code length L for any instantaneous
decodable system. By the McMillan inequality of Section 4.7, it also
applies to any uniquely decodable system.
     For efficient binary codes K = 1 and we have log2 K = 0. There-
fore, the inequality occurs (in the binary case) only when

                                 I가 羊 0i = 2나'

  Table 6.3-1 shows how Huffman coding approaches the entropy for the
  Zipf distribution.
                                         Sec. 6.6 / Shannon-Fano Coding        121

 6.6 Shannon-Fano Coding

 In Section 6.5 we assumed that the code word lengths I, were given.
 Suppose, as is more likely, that the probabilitiesp, are given. Huffman
 coding gives the lengths, but that method makes each length depend on
 the whole set of probabilities.
      Shannon-Fano coding is less efficient than is.Huffman coding, but
 has the advantage that you can go directly from the probability p, tQ
 the code word length l，· Given the source symbols s1, S2, · · . , sq and
 their corresponding probabilitiesj7l, P2, . . . , Pq, then for each p there
 is an integer i1: such that



                     比（計小g, (去                            + 1              (6.6-1)


 since the two extreme values just span a unit length. Removing the
 logs, we get



                           （計r' < (立）
 Take the reciprocal of each term. We obtain




Since 2 pi = 1, when we sum this inequality, we get

                                    브   온 /1\       1
                                1       乙 1 = 1 二＞ !                       (6.6-2)
                                        江1 \r7      r

which gives the K往仁才立如田丑且． Therefore, there is an instantaneous
uecouaoie coae naving inese bnannon-rano iengtns.
     To get the entropy of the distribution of p., we multiply the equation
(6.6-1) by p, and sum:


             H,(S) = 乶 p, l。g, } d 모pj1 <H,.(S) + 1
                       1= 1 '       !    Pa   '=1

.In terms of the average length L o            e        (6 5-4), we have

                      t面；;；二；i；二＼                                          (6.6-3)
  122     Ch. 6 / Entropy and Shannon's First Theorem

   Thus for Shannon-Fano coding we again have the entropy as a lower
   bound on the average length of the code. It is also part of the upper
   bound. It is not as easy to directly find an upper bound for Huffman
   coding (Chapter 4), but since Huffman coding is optimal, it is at least
   as good as Shannon-Fano.
        How do we find the actual code symbols? We simply assign them
   in order. For example, from the probabilities

                 Pi = P2 = 去'       P3 = P4 = P5 = P6 = 8

   we get the Shannon-Fano lengths,

                    11 =12 =2,       13- 14- 15- 16- 3          小入---

   We then assign

                                         53 = 100

                                         S4 = 101

                                         S5 = 110

                                         S6 = 111

     We are assured by the Kraft inequality, which we showed that Shannon-
     Fano coding obeys, that there are always enough symbols to assign for
     an instantaneous code. Our orderly assignment leads readily to the
     decoding tree and the prefix condition is met.
          This shows that we can do fairly well even with Shannon-Fano
     coding, but it is interesting to see how the left-hand inequality arises.
 /First,뇨丈쁘얀나三뜨빳빳ty p, w란르 르xactly웃잇므alto th잇e드'1?뜨ocal of a
/ P9꾄탓．얀ther旦쁘x r, then쓰드브엣坐쁘느쁘삔型f아t迹쯔旦培nm銀t
I ot code word lengths-the average word length would be exactly the
\entr py To get the c喆首布O崙誌＝而的邵啣n角可而rnbers in'
  ". increasing sequence and of the required lengths.


   6.7 How Bad Is Shannon -Fano Coding?

   Since Huffman coding is optimal, and we have temporarily descended
   to the less-than-optimal (at times) Shannon-Fano coding, it is reason-
   able to ask "How bad is Shannon-Fano coding?" Consider the fol-
   lowing examples.
                    Sec. 6. 7 / How Bad Is Shannon-Fano Coding?                  123

    For a source alphabet s1, s2 with probabilities
                                   l
               Pi = 1 -        갼
                               巾
                                                                       (k 之 2)


we get



                        log2
                                       （二，
                                             )   帥g2 2 = 1

Thus 11 = 1. But for 12, we have



    （斗呻小12          嶇
謐璘多囍凞；黛黛黛蒸韓之
the average word length. Clearly, Huffman has

                                             L11 = 1

For Shannon-Fano, we have



           LSF= 1(1 如 佃 =n1 + 7k2"- 1
We have the table

                                                  .       k-       i
                                                  l   十
                    k                                      2
                                                               "




                    2                        i + { ＝二 1.25
                    3                        1 + } = 1.25
                    4                        1 + ii = 1.1875
                    5                        1 + 吉 = 1.125
                    6                        1 + 食 = 1.078125

                                              etc.
 124    Ch. 6 / Entropy and Shannon's First Theorem

    As another example of the possible loss of efficiency, 匙Ppose that
 욘나－
   卜        ymb이s have 世르3am요1江ba珷d口그奴二 Shannon寸Fano
 would have
                              log2 q 5 1 < log2 q + 1
                           /\／八／   八／   뇨d小니／ ＼니／   Hm八느／           뇨＝戶口＋



 If q is not a power of 2, then Huffman would shorten some of the
 symbols, but Shannon-Fano would not.

         ：農熬黑；器恕otLl
n記瓮黑准悠"默烈：
\ in practice does Huffman dominate Shannon-Fano coding.

 6.8 Extensions of a Code

 We introduced the idea of entropy in a simple situation, 9越慰U쁘g
 e望르빤트뉜哄必3쁘브壑쁘剋얀얏焚蛙也으久c쁘뜨翅g. Weneedto
 devel6百 the idea of enti6py for both the extensions (Section 4.2) and
 Markov processes (Sections 5.2 to 5.5) we studied earlier. This we now
 do in Sections 6.8 and 6.10.
      The loss in Shannon-Fano coding compared to Huffman, when
 measured by the entropy function, occurs when the reciprocals of the
 probabilities are not exact powers of the radix r. If we encoded not
 one symbol at a time, but made up a code for blocks of n symbols of
 the source code at a time, then we could hope. to get a better approx-
 imation to the lower bound Hr( j.
      But more important, a立쁘엣必쁘르쁘虹（Section 4.10小쁘므쁘
 abilities of the extension are more variable than the original ir6babil-
 娠立前we expecTil陌t汪師｝傘fl臧統雨而4區而뉴ew誌而而d
 that both Huffman and Shannon-Fano encoding are efficient. We first
 review the concept of the extension of a code.

       Definition. The nth extension of a source alphabet sl, s2, . . · , Sq
  symbols of the form s11s,2 . . . s,,,           having the probabilities
  Qi = j7hj7i2 . . . pt,,. Each block of the n original symbols now becomes
  a single symbol t,with    probability      Q1.     We this alphabet
                                                            label     S" =  T.
      We saw this definition in Sections 4.2 and 5.5, so it is not a new
  idea. The entropy of this new system is easily calculated as follows:


                   耳（S8):Hr(T) 三客Q.log姑）
                      嗟Q띠,ilPi2.1 .,',)
                                                                                          Sec. 6.8 / E打en跏ns 0／口 ( 'ode   125

         Expand the log term as a sum of logs. We get


                                                                    們2m
                                    m1




                                                                            Qi加七，)
                                                              n             q'i
                                                = k2= l1=2 1 pi1p2 . . . p,, log.

For a typical single term that occurs in the summation over k, we have


i= 1
立p11p,
               2   .   .   .   p,
                                         logy
                                                   (I)
                                                              P1k
                                                                             二多，· · · ‘立，p11pi2 ·尻！og亡，)
For each summation not involving i k, the sum is 1 (since the sum of the
probabilities must be 1). That leaves only the summation overik. But



                                                  昏如（計瓦（S)
Hence the sum of all the terms, since they all have the same form, is

                                                         Hr(T) = Hr(Su1) = nH;(S)                                     (6.8-1)

     The ei玎r아낌 可th帥th 毗跏sion of an a枷口bet is n times t加 entrof砂
of the original alphabet. But note also that the extension has qfl symbols.
     We can now apply the result (6.6-3) to the extension T. We have
(where L is the average code length of the nth extension)

                                                   Hr(S") s L, <H;(S') + 1

Apply (6.8-1) and divide by n,

                                                         月．
                                                                      (S)
                                                                                  5   드<        月，
                                                                                                     (S)
                                                                                                           +   !      (6.8긔
                                                                                      n                        Ti


Since the extension has n symbols s, in each ti, it follows that a better
measure is L = LAIn. Thus for a sufficiently large nth extension of the
code, we can bring the average code word length L as close as we please
to the entronv H.(S). This is Shannon. s noiseless coding theorem: The
nm ex1enszon oj a coae sansjzes (o.o-z).
                                                                                          戶1尸
   느中
126   Ch. 6 I Entropy and Shannon's First Theorem

6.9 月工ani甲／es 可月工te加ions

                                                         4三3   P
Suppose that the source alphabet is s1, s2 with Pi = 륭, i7) = 吉. The
          =
                                                               八J二




entr아汐 Is

          H2(S) = 궁 log2 클 + } log2 3

                 = log2 3 - 4 = 1.5849 . . . -0.6666.

                 = 0.9182958. . .

Huffman coding gives

                            s1= 0,     52= 1

so that the average length of the code is 1. Shannon-Fano would give

                            11= 1,     12 =2

and the average length is

                       G)l    ()2-- 4-
                       (4)1 + G)     - 1+
                                                     l
                                                     甘
                                                     ］
In Section 4.10 we gave the average Huffman code lengths for several
extensions. For Shannon-Fano we get, for the second extension,

                        log2 뭉 드 /l,    11   =   2

                        log2 을 드 /2'    12 = 3

                        log2 을 드 /3,    13 = 3

                        log2 旱 드 /4,    14 = 4

The average code length is


               뇨＝（計 七小）『（枷
                       8+ 12+ 4         24
                                           = 2.666 . . .
                              9         9

    It happens that for this case we can compute the extensions for
Shannon卞Fano coding. In th틔弓也足努9映on 奴re will be
                                                                                                 Sec. 6.9 / E끄가까교es of E工把nsi이is                                      127

          ＼乙 Number of Terms                                                                                                Probability
                         .
                                  /
                    I-
                             .,




                                                                                                                                          갇y쓰鉀1
                                                          C(n, 0)

                                                          C(n, 1)




                                                                                                                                         1 1쓰 y 1 1 1l系
                                                              C(n, i)




                                                          C
                                                               (n,
                                                                           n)
To find the corresponding I, we have


                                                               (
                                                               I3n
      log2-
      「82      1=
                                  =
                                      log2
                                      1.
                                             82
                                                                       -             \
                                                                                    .)   =    nlog23
                                                                                                           -           (n
                                                                                                                                                                   (6.9-1)
          Pi
                                                                                                                              -            i)
                         ' = n(log2 3 - 1) + i 드 Ii                                                                (i = 1,2, . . .                        ,
                                                                                                                                                              n)
Let


                                             肛＝쯔必心題三끈些쏘，-1)                                                                                                        (6.9긔


                                                                                                       Ii,附「｛
                                                                                                            '邕
Then the average code word len


                                                                                             矛二iA, + i)                            ：工沮
                                                                                n
                                                      l
                                                                                                                   l
                                      = - A, 2 C(n, i)28 ' +                                                                 2C(n, i)i2" '
                                                  予
                                                                                                               予
                                                                                                                            i= o


For the first sum, we have

                                              (2 + 1)' = 2 C(n, i)2' 1 = 3"
                                                                                             i= O


For the second sum, we have

                                                              (2 + 工）" = 2 C(n, i）工'2" 1
                                                                     /＼니／八뇨／
                                                                           ＼니／ \／늬／                      ＼八나十늬／              늬／
128                     C九 6 / En什opy 口nd Sh口nnon's First The片日n

Differentiate with respect to x:

                                        n(2 + x)小1 = 2 C(n, i)ix2e12' 1
                                         H斗／   누H戶＝   =/m나小니／                  N나／   ＼니＼       ==\
                                   r\



Set 工 = 1:

                                               n3n_ l = 2 C(n, i)i2'                                 '

Assembling the parts, we have
                                                                        A
                                          LF                           l予
                                                                               n
                                                                               nJ
                                                                                     (
                                                                                     )
                                                                                     +
                                                                                     =
                                                                                           l
                                                                                               n3n_ l
                                           S                               n
                                                                                           予
where from (6.9-2),

                                 An 之 n(10g23 - 1) = n(O.5849625 . . .)

We compute a short table of A,1 and include in the last column of the
table the results for Huffman coding.

                        n(10g23 - 1)                  A.                                 LSF(n)/n          LH(n)In




      4
      1
      工 n
        乙 n
          4
          口 4
            1 <
              V 6 n
                  / 8

                                                               V d
                                                                 1 =
                                                                   \
                                                                   V <
                                                                     V 6
                         0.5849 . . .                                                1.33333 . . .       1.00000




                                                       4
                                                       l n
                                                         乙 n
                                                           乙 n
                                                             4
                                                             V n
                                                               4
                         1.1699 . . .                                                1.33333 . . .       0.94444. . .
                         1.7549 . . .                                                1.00000. . .        0.93827 . . .
                         2.3398 . . .                                                1.08333 . . .       0.93827 . . .
                         2.9248 . . .                                                0.93333 . . .       0.92263 . . .
                         3.5098 . . .                                                1.00000. . .
                         4.0947 . . .                                                1.04762 . . .
                         4.6797 . . .                                                0.95833 . . .
      O
      / 0
                         5.2696 . . .                                                1.00000. . .
      l                                                6
                         5.8496 . . .                                                0.93333 . . .

From (6.5-3) the lower bound is H (S) = 0.91829. . . . Shannon-
Fano coding apiroaches the entro. irre:ularl , but accordin: to the
earlier result               面es appro油 뜨如센少       ．
     Summarizing our discussion up to this poi; i:

       ‘絮器措祭嗇) fo匙쁘翅斐쁘쯔쁘沙9d奴묘口且
                                                  此(S) 5 L log2 r
                                                          Sec. 6.10 / Entropy of a Markov Process                                                  129

     2.．駟映프延女끄S쁘쁘쯔
                                    H2(S) 드 LSF log2 r < 札（S) + 工；
                                    ＼入戶小／ \/／人／                                人느

     3. In Section 4.10, since Huffman coding is optimal,




    4. In equation (6.8-2) the nth extension satisfies

                                                           L lo            r                                      + lo              r
                                                     5
                                                                                                   (S)
                                                                               !
                                                                  g2
                                                                                                                         g2
                                          (S)
                               H2
                                                                                         H2
Assembling all this we get for the nth extension,

                                                           r               sF                                 r                         + log2 r
                       5                                                                                           < H2
                           L
                                    (n)
                                                lo
                                                               드
                                                                       L
                                                                                   (n)
                                                                                              lo
                                                                                                                              (S)
                               8
                                                     g2
                                                                                                         g2
                                                n                                        n
                 (S)
       J-
            I2
                                                                                                                                            n


where 1...(n is the average code length for the nth extension for Huff-
mnn rind L...-(nl is tor Nhannon-卜ano. mne table Dears tfllS out ex-
perimentally. '[his running inequality shows clearly wny in section o. I
we are justified in saying that the theoretical loss in going to Shannon-
Fano coding instead of the optimal Huffman coding was not serious for
large n. For small n the practical loss may be significant.



Exerc加es

6.9-1 Do example for p = {.

6.9-2 Do for general value of p.



6.10 Entropy of a Markov Process

In Section 5.2 we introduced the idea of a Markov process to enable us
to represent certain types of structure in the input stream of data. In
particular, it handles correlations between successive symbols. We now
examine the entropy of a Markov process.
     Given that we have already seen the previous m symbols,

                                                           Si1, S12 ' · · · ' Sim
                                                                                                                                     缶                                                                                     /
                                                                                                                                                             90h 느 1/
                                                                                                                                                                                                        q
                                                                                                                                                         1二 넌 七
/
/\\                                                                                                                                             入1/
                                                                                                                                                                                                                .·'· ci',-)今；雨3
                                                                                                                                                                                         比

                                                           h（이4,'＼才                                                                                                                     戶
                                                                                                                                                                                        뇨／
                                                                                                                                                                                    b
                                                                                                                                                                                            ＝
                                                                                                                                 /
                                                                                                                                 /
                                                                                                                                                                                1
                                                                                                                                                                            1
                                                                                                                                                                        1
       130      Ch. 6 / Entropy and Shannon's First Theorem

       what is the probability that the next symbol will be s? In mathematical
       symbols this conditional probability is written as

                                                                        p(s1 I sf1, s,2, . . . , 뇨）

      Note again that the sequence of the symbols is

                                                                             Sil, Si2, . · . , Si_, Si


            For the zeroth-order Markov process the probabilities depend only
      on the symbol s, and is written in the earlier notation as p尸 For the
      first-order Markov source we have the digraph frequencies of pairs of
      syn化아s of the alphabet.
            Using our "surprise" definition for the amount of information we
      get when we receive a symbol 5, we define the information as


                 1(c. I                                                                    ) =                                   (                                                      1
                                                                                                                                                         1 sf1, Si,
                                    c.
                                                                                                                                     \p
                                                 c.
                                                                             v.
                                                                                                       ina
                 -   "   I   "Il,
                                             '        2'   "   '    "   ' "In!                         '         "bZ                          (si
                                                                                                                                                                                                .   .   .   ,   s,
                                                                                                                                                                                                                     _)



      given that we have already seen (are in the state)

                                                                                    Si1j s'12, . . . , 옥，,1


          The conditional entropy over the alphabet S of symbols s, is naturally
      given by the expression

      It (S I S,,, Si.,, . . . , s1_)

                         크＝ 二／
                            'cc' 尸＼
                                 nil, ) p                                          r                                            V ' mrlO                                                                        1
                                   口i                              i 口ii' 口12 '               '    "         '             ) "Em! 1 "b2                           1 _.i, . I 1끼                             .1
                                         S                                                                                                                         ／八햐 I J ii!                              햐2) ·



      This is the conditional entropy of the source alphabet S given that we
      have the sequence of symbols

                                                                                          Si1' S12 . . . , 욱，n


           We next consider the larger system and allow for the probability
      of the states of the Markov process occurring. Let


                                                                         p
                                                                                  (s11,
                                                                                                  si2,                 .    .    .   ,   s.
                                                                                                                                                    _)
                                                      Sec. 6.11 / Example of a Markov Process                                                                    131

be the probability of being in the state

                                                              Si1, Si,, · · · 9 욱，기


Then it is natural to define the entropy of the Markov system as the
probabilities of being in a state times the conditional entropies of the
states, that is, by the expression

   毛「月（S) =2P（욱,, 욱,, . . . , 옥，
                               ）月（옥：
                                   1옥：
                                     ，옥,, . . . , 욱．고
                                    )rr1
                                                      !
                               : ？뇨, 入夕,,．小1．쇼廂：m而二
Using our earlier definition                                  of the conditional e'ntropy, we get                                                                     V 1 1 ' I"" 吻

H(S) = 2 2 p(si1, s2, . . . , 욱, ,) p(s1 I si1, s,2, . . . , s,,,)

                                                                                        m81
                                                                                        x    log
                                                                                                       I,   (,
                                                                                                                 ,        s.,,       sf2,
                                                                                                                                            .   .   .   ,   s,
                                                                                                                                                                 ,)


But since


\＼끈숏欠
we have the entropy of the Markov process as



          =
          =
              5
              ，쭈，
                    1   p
                        「
                            （50,
                            (s11,
                                             5」
                                             52
                                                  ，
                                                      ·   ·   ．   ,   5':
                                                                      Sjm, 57)
                                                                           s)
                                                                                 1.
                                                                                 log2
                                                                                        82
                                                                                                   [
                                                                                                   , m,              :,   ,1     ,




6.11 Example of a Markov Process

As an example consider the Markov process (in a binary alphabet) shown
in Figure 6.11-1. In symbols the second-order Markov process is de-
fined by

                                           p(O I 0, 0) = 0.8 = p(l I 1, 1)
                                           p(l I 0, 0) = 0.2 = p(O I 1, 1)
                                           p(0 1 0, 1) = 0.5 = p(l I 1, 0)
                                           p(l I 0, 1) = 0.5 = p(0 1 1, 0)
132             Ch. 6 / Entropy and Shannon's First Theorem

                                                  0.8



                                      0.2
                                                                      必小o) +.·！（小o)
                                                            0.5


                                                                                                                  /
                                                                                               . 1        /
                                                                                                                               ;\
                                                                                          似브프響
                                      0.5                   0.2         o.
                                                                                 DIYo,
                                                                                                     o)       :   o.   tJ.   (1.    o)
                                                                        P[.·이 +2 U砂“ ..t
           D      t
                  卜 口                 1工6
                                                                                                                  1
                                O                                  =             咐
           \
                          k
                                                                  \//
                                                                  1
           /
                                                   0.8
 0.
                                                                  드




                                                                                                  b
           1
                          1
                                                                                          I-  "
                                    Figure 6-11.1 Markov process                         亡必 ,H X=i三 .
                                                                                         1:r                  尸


               What is the probability of being in the particular states 0,0; 0,1;

1,         and 1,1?           Using the읔bvious symmetry, we see that1
                          j．工          ＼工                  （少                6
      0;
                        p(O, 0) = p(l, 1)       and      p(O, 1) = p(l, 0)

Theref毗, 茴謐덖孰 th卿娜毗
                                p(0, 0) = 0.5p(O, 1) + 0.8p(O, 0)
                                 p(0, 1) = O.2p(O, 0) + O.5p(O, 1)

These equations both come to the same form:

                                    O.2p(O, 0) - O.5p(O, 1) = 0                                  (6.11-1)

Since we must be some place, we also have

                          p(O, 0) + p(O, 1) + p(l, 0) + p(l, 1) = 1

or

                                               2p(O, 0) + 2p(O, 1) = 1                           (6.11-2)
                                                                                                   Sec. 6.12 I The Adjoint System                                              133

The solution of (6.11-1) and (6.11-2) is



                                                p(O, 1) 티희于 p(l, 0)
                                                                                                                    i)
                                                p       (O,                        O)         =   牙p      (1,
和藪互西西區翅뜨                     robabilities of the er2odic                                                                                         5.
 ' - In the general case, these equilibrium probabilities can be corn-
puted in principle, but in practice they are often hard to find. Contin-

                                                                                                                q
uing with the example, we now have the table for the equilibrium state.

                                                                                                                                             小                                 功
      $II'       Si2'                 p   (s1       1     s,
                                                               ,                        s,   2)




                                                                                                                                                          孕寺i므在去缶缶4n
                                                    더
                                                    0


      0 0 0 0
                  0 0
                            0
                                                                                                                自
                                                                           U n
                                                                             二 8
                                                               8기겨／e <
                                                                     U ＜
                                                                       口 <
                                                                         V <
                            l
                            1




                                                          0000000
                                                                                                                츄
                dl
                l 4
                            0
                                                                                                                츄
                            l
                            d
                                                                                                                츄
  1l4l
     dld
                  0 0

  l                         0 l 0 l
                                                                                                                長
                                                                                                                츄
                l
                =l4
                                                                                                                츄
                                                                                                                5
                                                                                                                仁
From the table we can now compute


        ,5':,5')
     (s11,s, s) 1.82[
                 log21[,p(,(s1In1s,1,                                                                      m
湘烈 슥「（57,
                                                                                                                                            勻m
                 = 2[4log2(／죵）]『 2［枷 （d三）
                                        ]
                                                                                                                                                      /                    1
                                                                                                                                                               l
                                                                                                                                             O
                                                                                                                                                      1
                                                                                                                                                                       1   \
                                                                                                                                    4
                                                                                                                                                      1
                                                                                                                                                                       1
                                                                                                                                                      1
                                                                                                                                    1
                                                                                                                                                                       J
                                                                                                                                                      1
                                                                                                                                                               而
                                                                                                                                                                       /
                                                                                                                                                      \
                                                                                                                          rH7
                                                                                                                         八\
                        뜨，
                         (1。g210 - 3) + l,(l。
                                            g210                                                         l
                                                                                                                         乙
                                                                                                                                O
                                                                                                                                二
                                                                                                                                n
                                                                                                                                O
                                                                                                                                b
                                                                                                                                        n
                                                                                                                                        乙

                        /                                                      I


                 = 0.801377 . . . bits per binary digit


6.12 T加 A可oint Sys妃刃i

To find the entropy of the Markov source, we need to find the stationary
probabilities of being in each state of the Markov process. But as noted
before, they are often very hard to find. Therefore, we need some
134      Ch. 6 / Entropy and Shannon's First Theorem

method of bounding the entropy. This method, which we now develop,
is based on the concept of an 口a加油 莎釘帥．
      How can we find a bound on the entropy of a Markov process?
We will use a first-order Markov process for simplicity; nothing except
the notation differs for the nth-order system.
      Since we have found that the fundamental Gibbs inequality for
two distributions is our basic tool, we write it down for the distributions
we know, namely p(s1), p(s1), and p(s1, s.). The symbols p(s1, si) is the
probability of the pair of symbols, and is also p(s1, s1). We have, already,

                                      2p(s1, s,) = p(s1) = Pi
and

                                      2p(s1, s,) = p(s1) = p/

Thus we start with, using (6.4-2),



                     믐
                         S2   p
                              「
                                      (s1,
                                      （5,
                                                    ,   5')
                                                        s,         log2
                                                                   1.             82   [   P   p
                                                                                               (si)   (s1,         P         (si)
                                                                                                                             s,     )1
                                                                                                                                     ]
The equality occurs only when for all i and j we have the equalities
p(s1, s.) = p(s加(s1). We now use the conditional probability expression

                                      p(s1, 옥） = p(s, I 易）p（功

to get

                                                                                           , p                          1
                                                             s/)
                                                                                                                                    ]
                                                                                                             (s,
                                                                                                                       ),,
                                                                                                                   I s1)
                                                                          log21
                                             (s1,
                                  p
or expanding the log term and transposing, we get


         믐p(s1,s1)log2[, (,"匕，)］다무「(s1,s加.g2［六］
Therefore, again using the conditional probability,


          ）旱「p(s1
       p(s1)
      쭈2(5,      I s))1.82[
              （5n5)   log2 ,P(S,
                             (, I,1匕，)
                                   si)]1수「p(s1)
                                           （57)log2 Lp(s1)i
                                                                                                                               드 /I(S)
                                        Sec. 6.11 / E工（2mple 0／口 凡I口rkov Process                                                                                                     135

where H (S) is the entropy of the original symbols, which we will call
the adjoint system. We can therefore write


                           \    2p
                                                  (s1)
                                                                     H
                                                                                (S
                                                                                                                s, 드 )              H
                                                                                                                                                    (S)
and the entropy of the Markov process is bounded by the entropy of
the adjoint system, which is the zero memory source with probabilities
of the source alphabet p(s,) = p. The equality holds only if p(sj, s,)
= PIP尸 TI仙꿔인쁘쁘旦쁘쁘프얏雙쁘땐빤哄墅甦프빳쁘끄쁘뜨
奴르匙그7끄石
       The entropy of an extension of a Markov process is easily found
from our earlier entropy calculations of a Markov source and of an
extension. Again we consider, for the sake of simple notation, only a
first-order Markov chain. We have



                       H(S)
                       4(54) =슥晏「p(t1,
                                  （b ()t,) 1.82I
                                           log2Lp, (ti
                                                   (i
                               =        勘
                                                             (t1,
                                                                                     ()
                                                                                                       log2
                                                                                                                          [ ]       , （뒤                  '乙）
But it is a first-order process; hence

                         p(t3., t,) = p(s1, s,,, . . . , si,, s1)

We now apply the original conditional probabilities repeatedly to get

             p(뒤 t) = p(s11 1 s1)p(s1, I sn) . . . p(s1, 1 si,_ J
                                                                                                                     r                  1                            ]
              月 （Sn)
                           =   믐p
                                                (t1,
                                                                           t,
                                                                                )         log2
                                                                                                                                                                         「   ·   ·




                                                                                                                           [,
                                                                                                                     [P
                                                                                                                          （욱
                                                                                                                                        '나，
                                                                                                                                                                )]
                                                                                                 t1)
                                                                                                                                              (,
                                                                                                                                                                     1
                                    +                    p
                                                                                                                                                                     I
                                                                    (t1,
                                            s
                                                                                                              log2
                                                                                                                                              (s,
                                                                                                                               Lp
Each term may be reduced by summing over all the symbols not in the
log term:


        晏「p(t1,
           （7,m)t) 1.8:
                   log2 ,p(s11
                          G1匕，s,,)2) = 2
                                      목2(5,
                                         p(s1, s1)
                                              57)1.82
                                                   log2 1,Lp(st
                                                            (,1
                                                                                 = H (S)
136        Ch. 6 / Entropy and Shannon's First Theorem

Therefore,

                                                  /\/\／人V小入m1戶
                                                                 H (S기 = nH(S)

as we expect.


6.13 T加 Robi玎mness 可En勿아砂

We have just seen the central role entropy plays in coding theory, and
it is natural to ask how robust (sensitive) it is with respect to small
changes in the distribution P = (m, P2' . . . , pg). There are two cases
of importance; first, the maximum entropy distribution p, = 1/q; and,
second, the general distribution. The changes in the distribution can
be written in the form

                               P; = Pi + 스P,                                            with 2 스j7, = 0

or else in the relative change form,

                              p: = p,(l + 巳）                                            刊ith 2 p局 = 0

We can use the Taylor expansion about the original distribution:

                                                                                        (x                    2                     ('
f(x)       f(a) +                   (x
                                                                                                         a)
                                                                     +
                                                                                                                              (a)
                                                                                               -!                                        -!
                                                                                  (a)
                                                                                                                  +
                                                                                               2!                                         3!
       =                                 -                                                                                "
                          '                                                  ['
                              (a)            a)
                                                                                                                                                            '       +
                                                                                                                      f
                    f
                                                                                                                                               a)
or else the Cauchy form with the mean value 0:


       肛） /(.=      ）『／             如）(:                         -
                                                                     .）『f,
                                                                                        ,(0)        ('        ; ) " '               佃
                                                                                                                                         ＜0 ＜기


      We can also get upper and lower bounds in the various cases, and
so on. Thus many different formulas can be derived that measure the
robustness of the entropy function. We will derive only one example,
that using the additive error.
      We begin with the robustness of the maximum entropy distribu-
lion, where Pi = 1/q for all i. Using the n variable representation of
the Taylor series, and for the moment regarding all the 스p1 as inde-
pendent variables, we have
                                                                                   M                 q
                                                                                                     口
             H(S') = H(S) + 2                                                     쁘明                l
                                                                                                    12                而
                                                                                                                  a2H '
                                                                                                                          （却I,           +          .   .       .
                                                                       Sec. 6.14 / Summary   137

We have for the individual terms in the expansion


                     札（S') =
                            +
                                            ' 2（計 」2') log七『 却1)
                     瓦（S')                   v, . fi . \ .
                                            H乙
                      a스/가                      loge \4 十 스Pi) - I
               a2H.(S')                           1
                a（스j7i)2                      1!q + 스／'I

Therefore, evaluating these derivatives at 스p, = 0, we have


   札（S') =
               瓦（S)         -        （如加）                      2 스p' 근乙 2 q（却II +
           =    He    (S)   -   믈2            （却 『 ,I'     ·   ·   ·




We recognize the sum as being effectively the variance of the changes
from the uniform distribution. As you would expect, at an extreme the
value of the entropy changes very little for small changes in the distri-
bution.


6.14 Summary

We have introduced the concept of entropy and have applied it to various
sources of information to obtain bounds on what can be done by suitable
encoding of the source. Entropy, which measures uncertainty, surprise,
and information, is clearly the natural mathematical tool to use in such
situations. In practice, entropy has uses far beyond this limited area
of application, but we cannot go into them here.
      Shannon's noiseless coding theorem shows that by using a suitably
large extension of the source, the average length of the encoded message
can be brought as close to the entropy of the source as desired.
We demonstrated this both for a simple source and for the more com-
plicated Markov source. However, we have not done it for all possible
types of sources. The noiseless theorem is a forerunner of Shannon's
main result that even in the presence of noise (errors), we can find a
suitable encoding system. We prove this in Chapter 10.
Chapter 7



                                                T九C（沇annel
                        and Mutual Information




7.1 Introduction

Let us review where we are. We are concerned with sending infor-
mation either from here to there (transmission), or from now to then
(storage). As shown in Figure 7.1-1, we start with a source of infor-
mation (symbols) on the left and encode it in some fashion, such as was
discussed in Chapters 2 through 5. It is then sent through a channel.
In actual practice the channel is noisy, in the sense that the output is
not always the same as the input. Next, the message is decoded, and
finally the decoded message is sent on to its destination.
     It is time to look more closely at the channel. We will use the
concept of entropy developed in Chapter 6. How much information
actually gets through the channel? How shall we measure the mutual
information of the two ends of the system? How shall we define the
capacity of the channel? These are the questions we examine in this
and the next chapter.



                                     N이se


      Source                                                  Sink
                               그1
                    Encode H        Channel H   Decode

                      Figure 7.1-1 Signaling model



138
                                  Sec. 7.2 / The Information Channel       139

      Furthermore, we must learn to look at the system
                                                        from the receiving
 end, where the decisions are to be made, instead of
                                                      looking at the front
 end and following what happens to the signal as
                                                     it goes through the
 system.


 7.2 T九e／可ornu毗onC九anne!

  An information channel is a statistical model of the
                                                          medium through
  which the signal passes (or in which it is stored). In practic
                                                                 e, there are
 physical limitations on the fidelity with which the transmission
                                                                      can oc-
 cur. We need to formalize this idea in order to
                                                       compute how much
 information goes through a given channel.

            a1
                                                                    b1 \
       /
           a2
                                                                    b2

           a3
                                                                    b3
           1
                                                                    .
 A <       S                       P(bj I 키）
                                                                    S    >B
           S
                                                                    S
           1
                                                                    S

           S
                                                                    .

           aO



                           Figure 7.2-1 Channel

     Figure 7.2-1 illustrates what we mean by a channel. A
                                                                channel is
 described by a set of conditional probabilities P(b1 1 a.),
                                                             which are the
probabilities that an input a1 from an alphabet of q
                                                       letters will appear
as some b/ from an alphabet of s letters. We use
                                                      a capital P for the
channel probabilities. The sizes of q and s of the alphab
                                                             ets need not
be the same. For example, in an error-correcting
                                                      code, the alphabet
of possible received symbols is much larger than is the alphab
                                                                 et of sent
symbols; thus s 之 q. On the other hand, a chann
                                                     el may always emit
the same symbol when either of two different input
                                                        symbols are sent,
so that s 드 q.
    In this model the channel is completely described
                                                         by the matrix of
140     C九 7 / The Ch口nnel and Mi甘U口／Information

conditional probabilities

                                P1,1 = P(b1 1 a.)

Note the customary reversal of the subscripts. A row contains all the
probabilities that a particular input symbol a1 becomes the output symbol
b1. This matrix appears in Figure 7.2-1.
    This approach evades all questions of signal form, detection equip-
ment, band width, and so on, and concentrates on the information.
낮 끄쁘브므쁘브프쁘塑엣프쁘以쁘些으f멘m旽？叩erties:

      1. The ith row corresponds to the ith input symbol ai.
      ？·延日亘c匹如뜨進延畦亘砥瑟丕遍珏轉와b
                                                               墳，
      i. m !le su딴j型쁘브쁘엣뜨 in a ro＼자 is always 1, tnat
                       S              S

                       2P.1 = 2 P(b1 I a.) = 1
                      /= l           尸＝ l



         This merely means that 虹웃旦c也砂1코h丑르匙르즈뜨竺坦쁘쯔
         something will come out, and the ( . I .') give the distribution
         or tnese proDaoilitles.
      4. If丑引主 thea뜨쁘b世y of the input symb이 口iof occurri!1g,
         then

                            q   S

                           2 j2P(b1 I a.)p(a3 = 1
                        1= 1    =1



      This means that when something is put into the system, then cer-
 tainly something comes out.
                       P.
      The probabilities .1 characterize the channel completely. We are,
 of course, supposing that the channel is stationary, meaning that the
 probabilities do not change with time, and for the moment we are
 supposing that the errors that do occur are independent of each other.



 7.3C뇨znnel Relat油is九加S

 In the transmission system the input symbols are selected with proba-
 bilities p(a1), and consequently the received symbols b. will have some
 corresponding probabilities of occurring p(b1). (This notation is clear,
 although it does not satisfy the strict canons of mathematics.) The two
  sets of probabilities p(a,) and p(b1.) are related by the following channel
                                                                      Sec. 7.3 / Channel Relationships                     141

 equ口tion工’

                 p(a1)P1.1 + p(a2)P2,1 + . . . + p(a, )Pq,l = p(b1)

                 p(a1)P1,2 + p(a2)P2.2 + . . . + p(aq)Pq,2 = p(b2)

                                                                                                                        (7.3-1)


                 p(a1)P1,5 + p(a2)P2,, + . . . + P(aq)Pq,: = p(b5)

 or in a more compressed notation,
         了
          i, > p(a1)P(b1 1 a.) = p(b1)                                                               1, 2, . . . ,s)
          !／之＼
                      /\/

    If the channel had no noise, then for each i, one P.., = 1 and all
others = 0. Thus one p(a1) = p(b1). For all noise each output for a
given a has the same probability, namely p(a1)/s; hence p(b1) = 1/s.
    For a uniform input p(a1) = 1/q; hence



                                   p
                                       (b1)
                                                        =       吉무P
                                                                                  (b1
                                                                                               a1)


     We write the probability of a pair of symbols ai and b. occurring as
P(a1, b1). This has the same meaning as P(b1, a1). We can write this
probability in two ways: either as

                            P(a1, b1) = p(a1)P(b1 1 a1)

or as

                            P(a1, b1) = p(b1)P(a, I b,)

Equating these two forms of the same thing, we get [p(b1) 羊 0]

                             ."                         .             P(h' 1 a)n(a"
                            P(a,
                                              I                                                                        (7.3-2)
                                                  b1)
                                                            =         -   '   p
                                                                                        (b1)
This is known as Bayes' theorem on conditional probabilities. It is
clearly symmetric in the two sets of symbols. The P(b1 1 a1) are known
as the forward conditionalprobabilities, since they start at the front with
142    Ch. 7 / The Channel and Mutual Information
                                                                      \
the a given and express the probabilities of occurrence of the b1. The
P(a, I b.) are correspondingly known as the backward conditional prob-
abilities; given the output, what symbol probably caused it?
      In the Bayes' formula (7.3-2) we may use the channel relationships
(7.3-1) for the p(b1) and put them in the denominator to get the equiv-
alent expression,

                                      1 I a加
              午 m,J   b) =
                (a, Ib1) = ,P(b
                           q                  (a,)               (7.3-3)
                                   2 P(b1 I a,)p(a,)

Summing this over all the a, clearly gives


                           2P(a, 1 b.) = 1

 which nl旦an邑工Jaj given output b,, some ai was certainly put jn.to th.立
 cHanneL.
/=\\，月／

7.4E工a刃iple 可 the Binary Sy刃imeti切 C九口nnel

A binary channel is probably the single most useful model of a channel.
It has two input symbols, 0 and 1, and two output symbols, 0 and 1.
Figure 7.4-1 illustrates this channel. The binary channel is said to be
symmetric if

                                .1 '          Pl,O = PO,l




                                       P0.0
      a=                                                      b= 0




      a=                                                       b= 1

                  Figure 7.4-1 Binary symmetric channel
              Sec. 7.4 / Example of the Binary Symmetric Channel      143

     If P1.0 羊 P0,1, then the engineer would probably adjust things so
that they were equal, so that the chance of a 0 becoming a 1 would be
equal to the chance of a 1 becoming a 0.
     Let the probabilities of the input symbols be (lowercase letters)


                         p（口 = 0) = p
                         p(a = 1) = 1 - p

Next, let the binary symmetric channel probabilities be (upper case
letters)


                          P0,0 = P1.1 = P

                          P0,1 = P1,0 = Q

The l｝匙多잊J珽뜨迹生프畔d아今



                           上브
The channel relationships (7.3-1) become

                    pP + (1 - p)Q = p(b = 0)                       (7.4-1)
                   pQ + (1 - p)P = p(b = 1)

Note that these equations can be simply checked by computing their
sum:

   p(b = 0) + p(b = 1) = p(P + Q) + (1 - p)(P + Q)

                          = (p + 1 - p)(P + Q) = (1)(1) = 1

      Given that we know what symbol we received, what are the prob-
abilities for the various symbols that might have been sent?
      We first compute the two denominators for equation (7.3-3):


                2P (b1 1 a，·)p(a1) = Pp + Q(1 - p)


                2P (b2 1 a.)p(a1) = Qp + P(1 - p)
144    C九 7 / The C力anne! and兀伽tu口／I/ bri加加n

We then have

                                                  No            All
                                                 N이se          N아Sc


 P(a = 0 I b = 0)             ／勿
                                                   1                p
                         ／勿 + Q(1 - p)
                     e      Q(1 小 p)
 P（口 = l lb = 0)                                   0           i-       p
                         Pp + Q(1 - p)

 P（口 = 0jb = 1)               Qp                   0                p
                         Qp + P(1 - p)
                           P(1 - p)
 P（口 = l lb = 1)                                   1           i-       p
                         Qp + P(1 - p)


which involve the choice of the probabilities of the source.
    For no noise P = 1, Q = 0, while for all noise P = { = Q. In
the special case of equally likely input symbols (p = 士）, we have the
very simple equations

             P(a= Olb= 0) =P=            P(a= l lb= 1)
             P(a= l lb= 0) =Q= P(a= ojb= 1)

     As an example of a peculiar channel, suppose that P = 옳 and Q
 = 솖 for the binary symmetric channel probabilities. But suppose also
that the probability of the input a = 0 is sent 끎 = p and a = 1 is sent
솖= (1 - p). We then have

                           P（口 = olb = 0) = ｝굘
                           P(a = 1 I b = 0) = 赤
                           尸（口 = olb = 1) = 끓
                           P（口 = l lb = 1) = 옳

     Thus if you receive a b = 0, then almost certainly an a = 0 was
sent. But if a b = 1 is received, it is still a 끓 > 륭 probability that a =
0 was sent. Therefore, regardless of what symbol is received, you must
assume that an a = 0 was sent!
     This situation arises whenever both

                P(a= 0Ib= 0) >P(a= l lb= 0)
                P(a= olb=          1) >P(a= l lb= 1)
                                          Sec. 7.5 / Sys妃m Entr갸兀es                   145

From the earlier equations for the binary symmetric channel these con-
ditions are

                             Pp> Q(1 - p)
                             Qp > P(1 - p)

or both

                                   p> Q
                                   p> P

In words, this says that the bias in the choice of input symbols is greater

'""" '"' "'"' """' """""'：崙"客斟未際"寐mis暖朴如4)
                                                 하4,m, 0 1
7.5 Syste刃i Entropies 下，了1                    ,34} r       ."나 '            1쿄｝
In Chapter 6 we developed the concept of the entropy of an information
source (which we now label A). The entropy measures the average
amount of information per symbol of the source, or equivalently, the
uncertainty associated with the source. 丑(A) = 0 when the source is
匹rtain and H     戶samaximurn when all the_a. are e.ual 'ke1 . We
have the definition of the entropy as
                                                                   흔PCtj1ai) f'(& )
                                                                       1e
                                                                   1


                    耳（」
                      ）已客「(a1)log侃）
                   r八／＼小／\／뇨／ V\   7／   니十나            午
                                                                                  (7.5-1)


As noted, the entropy function has the following properties:
                                                                                      ('机b)
                                                                                  P
   ！·Z. 耳 （.A) 브0. .           . .      . ..            . . : 민和）P(qi)
        t1rV1) 5 1ogq, wnere q is me numoer ot input symDols.
    3. H,(A) = log月 when all the source symbols are equally likely.

     The rest of this chapter is simply the systematic use of the entropy
function applied to various distributions of the model of the signaling
system.
     Clearly, corresponding to (7.5-1), the entropy of the received sym-
bols should be defined by


                    耳（B)＝』客
                          「(b1)logy［南］                                            (7.5-2)
146   Ch.   7 / The Channe/ 口nd 凡lutu口／Infor刃2口tion


This quantity measures the uncertainty of the output symbols and has
the same properties as the entropy of the source, since all the properties
were derived from the form of the entropy function.
     Similar expressions for the conditional entropy may be derived as
f이lo씨s. W르 na빳ally have f아the cond蜘nal e跏갸깹 g                           ic-
史凹二                          H나H
                 Hr(A I 하）                                                                                                                            (7.5-3)
                                               立／              (.    기b加.                            g,
                                                                                                     8r        I,
                                                                                                               LP        (a
                                                                                                                         (,         i   .   ,)]
    If we average (7.5-3) over all the b1, using of course the appropriate
probabilities p(b1) as weights, we get
                                       S


        .//：인쁘二名脚叩 b )

                             上如蜘小小，niI'b)i
                                        b1)] (7.5-4)
                             소加小『뇨'b1)]
     Doing exactly the same thing except that we view it from the sending
end, corresponding to (7.5-3), we get the conditional entropy having
sent a,:
                                                                                                               r                    1
                 Hr(B a') 已몸P(b기 "') logr Lp(b, 1 a)
                                                                                                                                                      (7.5司


Similar to (7.5-4), averaging this time over the input alphabet we get
the corresponding conditional entropy,
                                                      』s                                                            F
                         I
                                  三q
            Hr                                                                                                                                        (7.5-6)
            4,    (B
                  (3m)
                             A)   =
                                           i
                                                    i j    1
                                                               P
                                                               2
                                                                    (a,
                                                                    (:
                                                                            ,,,   b1)
                                                                                  6,    )1.
                                                                                              logr        8r
                                                                                                                    LP
                                                                                                                              (b1
                                                                                                                                        I as)     ]
    We now connect two ends of the channel together. In order to
measure the uncertainty of the joint event for both source and receiver,
we define the joint entropy in a similar way:



            느싸吐空쓰브，南］                                                                                                                                 (7.5-7)


n First we examine the joint.en9opy for the special case when A and
ii are statistically inaepenaent ror 411.1 ana j (rneaning.tnat wnat comes
out uoes not aepeno on wnat goe투 in, au noise).                                                                                         m1le inoepenoence

                                                                    二,＼卜）
                                                                        十K八8\1n
                                                                    Sec. 7.5 I System Entropies                     147

 condition is expressed by the equation

                                  P（口i, 하） = p(a1)p(b1)

 The joint entropy therefore becomes



      瓦似쓰益少小出計따匍｝                        +


 Since

                  q
                  2니  P   n
                                   =1                    and                  2p (b,) = 1
                                                                              j= 1


we get (for independent input and output)

                       Hr(A, B) = Hr(A) + Hr(B)                                                                 (7.5-8)

    Normally, the output of a channel depends at least partly on the
input (otherwise, why are we using it?). In this case can write

                        P（口i, 하） = p(a1)P(b1 1 a.)
                        八／        니／ ＼小H小／                          ＼日八y八1

and the j아nt entr아汐 is


             Hr(A, B) =
                                  詐P(a1,b1띠六］
                                  i= 1j ==1




But
                              +
                                                 :   P
                                                         (a1,
                                                                    bj)
                                                                              1ogr
                                                                                         [,
                                                                                               (.
                                                                                                    』

                                                                                                    11a1)
                                                                                                            ]
                                  2P(a1, b,) = p(a1)

Therefore,

                          온           . . ,                     I         i          ]
         月.(A, B)
             q ＼力＼/    = 自p（口' 'Og' L而5]
                                     q       S
                                                                                                      1
                          + 2 2 P(a1, b1) logr
                                                                                              P(b1 I 吼）.

                      ＝共多2六多민스）
                                                                         b5'" 趾텨「'" ' 山准了
                                             股冕口寸 i伊1b;)＝띠       r ．'    "
                                                         （少 f: (a더 너）
148    Ch. 7 / The Channel and Mutual Information           "         /


The joint entropy is the sum of the source entropy and the conditional
entropy given A.
     The conditional entropy Hr(B I A) represents the information loss
in the channel in going from input to output. It is how much must be
added to the source entropy to get the joint entropy. Hr(B I A) is
called the equivocation. It is also called the noise entropy of the channel.
     Since A and B play symmetric roles, we clearly have the corre-
sponding expression to (7.5-9),

                    Hr(A, B) 三i/,（引 + 耳（A I B.)                                    (7.5-10)

      In summary, in this section we have defined various entropies: H (B)
by  (7.5-2),  H (A, B) by (7.5-7), H (A 1 B) by (7.5-4), H (B I A) by (7.5-
6),  H (A  I b.) by (7.5-3), and H (B I a.) by (7.5-5). Each is derived by
using the    appropriate probability distribution.



7.6 Mutual Information

Consider again the transmission system of Figure 7.2-1. The input sym-
bols are the a, and the output are the b., and the channel is defined by
the conditional probabilities P:,1.
     Prior to reception the probability of the input symbol a, was p(a).
This is the a prioriprobability of a. After reception of b力 the probability
that the input symbol was a, becomes P(a1 I b1), the conditional prob-
ability that ai was sent given that you received b1. This is an a posteriori
probability of ai. The change in the probability measures how much
the receiver learned from the reception of the b1. In the ideal channel
with no noise, the a posteriori probability is 1, since you are certain
 from the received b1 exactly what was sent. In practical systems there
 are finite nonzero probabilities that errors will occur and you, the re-
 ceiver, cannot be absolutely sure what was sent.
      The difference between the information uncertainty before (the a
 priori probabilities) and after reception of a b/ (the a posteriori prob-
 abilities) measures the gain in information due to the reception of the
 b,. This information is called the陀tual info而atio? and is naturally



                    g,. - 址쁘뇨'으d
               쯔쓰lo-..--.--                     (a,
                                                                                     (7.6-1)
                         小8,1              FP
                                                                ,   b)
                          =

                                       .
                                                          (a)
                                                      p
                                                                    J
                                log,
                              e戶卞누／\/\/q\
                                                                                           Sec. 7.6 I Mutual information                                                          149

lithe two probabilities p(a,) and P(a, I b1) are the same, then we have
gained no information and the mutual information is zero. No infor-
mation has been transmitted. It is only when we have learned something
new about the probabilities of the ai from the received b1 that the mutual
information can be positive.
     Multiply numerator and denominator of the log term of (7.6-1) by
p(b小 Since

              P(a, I b)p(b1) = P(a1, b.) = P(b1 I a.)p(a1)

we have

             n
             nm
              HJ
               J   地
                       b1) =                  1og
                                                            '
                                                                    I P(a,, b,) 1
                                                                    Lp
                                                                                (a加
                                                                                                     (bi
                                                                                                         i             )
                                                                                                                                      =    I
                                                                                                                                                   (b1;
                                                                                                                                                          a,   )
                                                                                                                                                                   {
                                                                                                                                                                   J
                                                                                                                                                                       (7.
                                                                                                                                                                             6-
                                                                                                                                                                                  2)
    The mutual information i (a,; b.) has the following properties:

    1· 旦엣｝쓰心쁘恥얀딪프 ！드뜨쯔뽀亡the 血飾tion gives

                                   n                                                  O
                                                                                               [P(a1 I b)'                                                             &=
                                                                                                                                                                       /
                                                                                               L
                                                        b
                                                    J
                                                                                                                           (a)
                                                                                                                                               -




                                                                                               [
                                                                                                                   p
                                                                                                                                  I
                                                                                                                                           )]
                                                                                                                                               ]
                                                                                                [P
                                   ,;.')
                                      a1) ==
                                                                                                             (b1
                        I
                        7
                            (b1;
                                                                                                                                      a,
                            (.
                                                                         logr
                                                                                      8r
                                                                         1.
                                                                                                               p
                                                                                                                           (b1)
       and／奴仰녔크包a,).
    2. We alSo have                    !

                                              /(an 하） 드 /(at)                                                                                                          (7.6-3)
                                       , I＼小八八／\/\／入／
       This follows from the definition

                                          . .                                                  I i i
                                   1
                                       (a1)
                                                                =

                                                                         log,              .   Lp
                                                                                                      (ai)
                                                                                                                                  i
       and

                   I (a,; b) = log,.P(a, 1 b.) + 1(a,)

      The maximum for the .robability                                                                                                                     and the maximum
for its log is ere ore 0:

                                              i (a,; b1) 5 1(a,)
150     Ch. 7 / The Channel and Mutual Information

      毛Ii喚哭빳쯔긴엿뜨뜨主깐，that is, 吐
                                       P（口i s 하） = p(a)
                                      +\/\/\/\/\／六卜



        or what is the same thing, if

                                    P(a, b1) = p(a1)p(b1)
                                r\ V\ ／나／ 入느m//           누


        then




      Because of the inevitable noise the behavior of a channel can be
understood only on the average. We therefore begin by averaging the
mutual information over the alphabets using the appropriate probabil-
ities of the symbols occurring:

                  I (A; b/) = 2 P(a1 I b1)I (a1; b.)
                                                                                                                   (7.6-4)
                                                                                                              )1
                                                      I
                                                                                                               j
                                                                        fP
                                                                                                ,1
                                                                                                      b
                                                                                (a1
                                                                                                     )
                                                                                                          1
                                =

                                                                        L
                                           P
                                                          b1)
                                                (a
                                                                 logy
                                                                                          (a,
                                                                                    p
Similarly,



                  l
                      (a7;
                             B) =     쭈i   P
                                               (b1
                                                      I ) a,
                                                                logr
                                                                        L
                                                                        [P
                                                                             (b1{
                                                                                    p
                                                                                        (b1)
                                                                                                     a,
                                                                                                               j
                                                                                                              )]
                                                                                                                   (7.6-5)


Finally, we get

               I (A; B) = 2 p(ai)I (a1; B)
                                    i= 1




                              = 旱구「(as,b1.)log,.［二
                                               ，(：出］                                                               (7.6-6)

                              = I (B; A)

by symmetry. The first 뗀9j2女포L쁘므｛프：
                                  塾 are called the con르1-
韶韶們蜘，黑響／瓷始器升鴛紫甲，畿臂
                 ，
ainnaoei iii given tnat a,· was sent.
     mne tniru, I (A; L5), wnicn is symmetric in tne two aipnaDets, pro-
vides a measure of the information gain of the whole system and does
                                        Sec. 7.6 / Mutual Information        151

not depend on the individual input and output symbols but only on their
probabilities; it is called the system mutual information. The system
mutual information has the properties:

     l. d企五）    르꼬4'皿ll血皿d型끄로lit'世L匹뽀르血뇨요立；血皿소
     2. I (A; B) = 呵쁘旦으世y프즈쁘 d B ,are independent.
     3. I (A; B) = I (B;AJ (from symmetry).

     We can relate these various entr아疵計O each 야her by the f에아ving
algebraic manipulations. For example, from the Gibbs inequality
(6.4-2), we have



  戈好 已客，立「（./,b1) log［出’
                      ，::] 如
             = 2 2 P（口／, b1) 伽gP佃I, 하）
               i= 1 j= 1


               中 log p（口：:) - log p(b1)] 之 0

             = -2 2 P(a1, b1) log
                                         I         i       1
                   I     J              ［尸（a, b1) j


               냐「(a1)log［六］수「(b1)log [p(b1)1j 之 0              1-
                                                                    4-
             = H (A) + H (B) - H (A, B) 之 0
             H八／       小小小m八八小7口＼            小7\       /


Using the results (7.5-9) and 7.5-10), namely

                       H (A, B) = H (A) + H (B I A)

                                  = H (B) + H (A 1 B)

we get the two results

                   I (A; B) = H (A) - H (A I B) 之 0
                               = //（引        H (BIA) 之 0                 (7.6-7)

Therefore,

                             0 5 H (A I B) 드 H (A)

                                                                         (7.6-8)
152    Ch.   7 / T加 Ch口nne/ 口nd 九tutu口／Infor刃i口tion


and

                           H (A, B) 드 H (A) +H (B                                              (7.6-9)

Equation (7.6-9) shows that the joint entropy is maximum when the two
alphabets are independent.
    As examples of rela브으sii s, the average mutual information is

             ..
             J                 I石可
                                 『 叫- H(A, 네
             kV(A; B) = 1 H (A) - H(A J B)                                                 I
              \         (H(B) -H (BJA)                                            ,        1
                  \/＼八小Hm口m／   니八d1m卞小月尸1나＼              ／小1戶八＝ 八V




The equivocation is

                       쯔A나힌二쯔스느：쯔쯔흐)
                       빈킨스느쯔쓰二三（쓰흐）
The 如m t entr아갸 is

                                fH
                                           (A)
                                                    + H   (B)
                                                                ,   -   I
                                                                            (A;
                                                                                      B)
               H (A, B) = 1 //(A) + H (BpA)
                "- .-'--' (,H (B) + H (A I B)
                                     r小＼         ／戶＼m/
                                                         \/\/＼口戶＼
 Chapter 8



                                                                 C九anne! Ca刃aci勺




8.1 Definition of Channel Capacity

Given the conditional probabilities P(b1 I a.) = P11 which define a chan-
nel, what is the maximum amount of information that we can send
through the channel? This is the main question addressed in this chap-
ter.
     The mutual information connects the two ends of the channel to-
gether. It is defined by equation (7.6-7),

                         I (A; B) = H (A) - H (A 1 B)

where the entropy H (A) is the uncertainty of the source before the
reception of B, and H (A I B) is the average uncertainty after the re-
ception of the b. of B느 Thus I (A; B) is the change in the information.
An alternative expression for I (A; B) is equation (7.6-6),



              I
              7
                  （」
                  (A;
                        ；5)
                         B) =   裝2
                                     A,
                                          B   P
                                                  (.
                                                  (a,
                                                        ,
                                                            6)
                                                            b)
                                                                  log.
                                                                  1.
                                                                         8
                                                                             「
                                                                                 f
                                                                                 Lp
                                                                                      P
                                                                                          (a)
                                                                                                (a,
                                                                                                      p
                                                                                                          (b)
                                                                                                                b)
                                                                                                                     1
                                                                                                                     ]
where we have dropped subscripts and adopted an obvious summation
convention.
     This formula involves the input symbol frequencies p(a). We saw
in the example of a binary symmetric channel (Section 7.4) how a poor
match of the p(a) to the channel can ruin a channel. Indeed, we know
that if the probability of one symbol is p(a) = 1, then all the others



                                                                                                                         153
154     Ch. 8 / Channel Capacity

must be zero and the constant signal contains no information. How
can we best choose the p(a) to get the most through the channel, and
what is that amount?
    We postpone the problem of choosing the p(a) by using a standard
mathematical trick; we simply define the channel capacity as the max-
imum over all possible assignments of the p(a):

                           C = max I (A; B)                        (8.1-1)
                                   p （口）



This makes the channel capacity depend only on the P,., and temporarily
evades the difficulty of finding the suitable p(a). The probabilities p(b)
are determined from both the p(a) and the P1,1 via the channel equations
(7.3-1). By this definition there is no question of ever having a higher
mutual information than the channel capacity C, since by definition C
is the maximum.
     You want me to measure the capacity in bits per second (or some
such units). But remember that storage is the same as transmission.
Hence we measure capacity in bits of information per bits sent.



8.2 The Uniform Channel            , 『

From equation (7.6-7) we have the mutual information

                    I (A; B) = H (B) - Hr(B 1 A)

From equation (7.5-6) this is


      , I(A; B) = Hr(B) - 쭈쭈 P(a, b) logr [P(/,hl a)]
                 = H(B) - 耳 p(a) 芎 P(b I a) log. [p(bhl a)]
     In a highly symmetric code, such as a parity error-detecting code,
a perfect error-correcting code, and many others, each symbol is equiv-
alent, in a sense, to any other symbol in the code-the differences in
the probabilities for errors in the various symbols are inessential. For
example, we can convert any symbol into the 0, 0, . . . , 0 symbol (in
the binary system) by the trivial process of complementing each position
that has a 1 in it. If the channel has white noise, and this is what most
of the codes were designed to handle, then the entries in any row of
                                                                   Sec. 8.2 / The Uniform Channel                 155

the channel matrix, for the cases above, are merely a permutation (rear-
rangement) of those in the first row. Each symbol has the same set of
transition probabilities as any other symbol.
      Under the condition that each row is a permutation of the first row,
it follows that the sums


               2P(b 1 a) log.                                                                      H (B 1 a)   (8.2-1)
           H
                B
                                       .／戶mH／        戶니나
                 ＝卞斗／   八／   戶＼
               尸＝




are independent of a. No matter which symbol a you pick, this average
will be the same. We can, therefore, sum over all the symbols of the
alphabet B and get for each a

            I (A; B) = H ,(B) - W2 p(a) = Hr(B) - W                                                            (8.2-2)


Thus we see the use for the following definition (a special case of corn-
mon occurrence).


 米D匹쁘批：
      스쯔剪吻                                           伽nnel has a n姐tr汰
                                                                     ，

                                                             P1.2
                                                             P2.2



                                                             Pq.
                                                                   2


such that each row is a permutation of the first row.

      Suppose that we think of our channel as an extension of the binary
symmetric channel. Each alphabet symbol is a block of n bits and each
bit is subject to the same independent probability of success P (and
 failure Q). This definition makes the error-detecting and perfect error-
correcting codes have symmetric channels.
      As a trivial example, consider the noiseless channel where each
input symbol a goes into exactly one output symbol b; that is, for each
given a, one P(b I a) = 1 and all other P(b I a) = 0 for that a. Each
term, therefore, is


                             P
                                  (b
                                                a)
                                                      logr
                                                                       [P
                                                                            (bhI
                                                                                   a
                                                                                       )
                                                                                           ]   =   0
156    Ch. 8 / Ch口nnel C口／）口city

Hence W = 0 and

                        I/(A; B) := Hr(B) = Hr(A)

as we expect.



8.3 Unjform Input

Given a uniform channel, clearly the sensible way to use it is to use
uniform p(a) for the input alphabet symbols. We have the formula
(8.2-2)

                                                                                       (8.3-1)

     Suppose that we apply this formula to an n-bit single-error-detecting
binary code. [We know from (6.8-1) what the answer will be, but for
exercise we will compute all the details.] The number of input symbols
is q = 2n -1, since (due to the parity check) only half of the possible
sequences of n binary digits are possible inputs. Because of the errors
that are possible, any binary sequence could come out. We have the
following situation (where P = probability of no error per bit sent):

        Number
          of
         Cases                 Type                                      Probability

            1            No error
           n             One error
        n(n - 1)
                         Two errors
            2                                                  ／今
        C(n, k)         k errors
                                                                    난이
But



                   w＝
                          믐P
                                  (b
                                       I   a)
                                                log2
                                                       [,
                                                            （이
                                                             ' ,    )]
                                                                                                                Sec. 8.3 / Uniform Input                                                 157

Grouping together all the cases having the same probability, we have



                =       屈
                    八시니八H시小／
                                         C    (n,                  k)             pn                 kQk
                                                                                       ＼小n나八八／\/＼戶니， 小／
                                                                                                                log2
                                                                                                                                [PP                        kQk]               (8.   3-    2)
Expand the product in the log term into two log terms:


                                                                                                     )                                        ()
                                                                                                                       /＼八小．八＝八／\/V




                        (n          -        k)
                                                            log2
                                                                                       (}                      + k log2                                                       (8.3-3)


From the first term we get for the sum (8.3-2) (to take care of the
n - k factor and then the n factor),
                                                                                                               1k
                                                                                                               k =

             （掘，
                                                                              M                                             小


                                                                                                                                              P
                                                                                                                n n
                                                                                                                                                  n


                                        , (,
                                                                                                                                          \
                                                                                                 1
                                                                   n!1
                                                                                                                                                      kQk
                                                                                                                            1


                                                                                                 k
         唾
                                                                                                                                          )
                                                        -
                      ，巴끄 k)!                                                                                                                                                 Q
                                                                                                                                                                              k

                ＝如（}）瓦；
                                                                                                                                                                   什



                    =        n기叩                    ,              仁，
                                                                        \i_
                                                                              )
                                                                              /             (P             ,    Q)      n             l       :       nP          1四,   (1)
From the second term of (8.3-3) we get for the sum (8.3-2), correspond-
ingly,


                                                                   小g2                                     (句
Together they give




where we have used the natural notation



                112們=「嶇（小 蜘（古)                                                                                                                                                (8.3-4)


The mutual information (8.3-1) now becomes

                                   1(A; B) = 1-12(B) - nH2(P)                                                                                                                 (8.3-5)
158    Ch. 8 / Channel Capacity

The entropy of the nth extension is again n times the entropy of one
symbol.




8.4 Error-Correcting Codes


In Section 1.3 we observed that sometimes the encoding process was
broken un into two stages. one to suitably match the source of infor-
mation. 小e second to m訊h the cli而兪f由e而雨if교三3奸二O而而百
而슈區on可늉侖示능f而而盂繭百面ti陌玉伽iti。                        n 。f the channel and call
it part of the channel. Indeed, sometimes it is arranged so that as far
as the user is concerned, it appears as if it were the channel. Let us
examine what this channel looks like.
     For a perfect error-correcting code of n bits and probability P of
being correct for each single bit in the white noise channel, then for the
channel errors P,.1 the user sees the following table. Remember in this
channel a single error is correctly corrected, and a double error is wrongly
corrected into a triple error.


              Occurrence of:                  Actual Probability

              No errors                         P., + n아）" l
              One error                               0
              Two errors                              0
              Three or more errors              1 - [no error]


       Thus the channel errors have a peculiar structure in terms of the
 original causes of errors. However, we may still apply the methods of
 the preceding section to this uniform channel.
       When the error correction is either in hardware or is automatically
 included in the software, the user sees the above. It also indicates what
 was earlier observed: In practice, for a variable probability source, we
 are likely to use a Huffman code to match the source, and then apply
 some error-correcting code to blocks of this encoding. More and more
 often computers are being built with error detection and/or correction
 in the hardware. It is a matter of preference on your part whether you
 wish to regard this as a single process of encoding, or as two processes,
 or whether you wish to regard the second stage of encoding as belonging
  to the channel itself. How to handle the situation should be clear.
                Sec. 8.5 / Capacity of a Binary Symmetric Channel        159

Exercises

8.4-1 Apply this section to the 7-bit single-error-correcting code.

8.4-2 Extend this section to minimum distance of four codes.
                                         V

8.5 Capaci砂 可a 川nary多y刃1刃zelr元（沇anne!

If P is the probability of correct transmission, then the channel matrix
for a binary symmetric channel (Section 7.4)

                                           P
                   p
                       (a   =    O)   0              0 p   (b=   0)
                       p(a= 1) 1                    >1 p(b= 1)

is given as


                                      （二       QP
Let p = probability of choosing a = 0. Then 1 中 p = probability of
choosing a = 1 and the mutual information for this uniform channel is
equation (8.2-2). Using log2 and temporarily dropping the subscript 2
on the entropy function H, we have

                                1(A; B) = H (B) - W

where, from (8.2-1),


                       쓰 믐7(6 a) log [P/ 1 a)]
                            = P log（枷 叫古）
                            =，思超）
using (8.3-4). Therefore,


                       스｛蚣母就(B늪名喉，                                    (8.5-1)
160     Ch. 8 / Channel Capacity

      To find H (B) we note that [equation (7.4-1)]

                                    p(b = 0) = pP + (1 - p)Q
                                    p(b = 1) = pQ + (1 - p)P

It is easy to see that

                                          p(b = 0) +p(b = 1) = 1

For convenience we set

                              p(b= O) =pP+ (1- p)Q= x                                                           (8.5-2)
Hence

                                                    p(b = 1) = 1- 工

and using the notation of (8.3-4),


        I
            (A;   B) =         x    log
                                                    (   +   (1
                                                                 -   x)
                                                                          log
                                                                                (,    1
                                                                                          ,       -   H   (P)
                             = H (x) - 11(P)

    To get the channel capacity C, we ask: What choice of the symbol
probability p maximizes the mutual information I (A; B)? Since we are
working with the variable x, this is the same as asking what maximizes



                   H   (x)      =         x   log       （小日岫 ! )                     （,       ,

From section 6.4 the maximum occurs for x = 글, and

                         //（글） = 글 log 2 + 글 log 2 = log 2 = 1

The capacity of the channel is therefore


                               七r擥三兀4년느1二쓰P)                                                                    (8.5-3)


      We can find the value of p from (8.5-2) as follows:

                                    x = { = pP + (1 - p)Q
                                          { = pP 十 (1 - p)(l 中 P)

                                           = pP + 1 - p - P + pP
                               Sec. 8.6 / Conditional Mutual Information                   161

 Transposing and rearranging, we get

                                         = 1 -2                     P
                               (1 - 2P)p
                                                           乙

Since the channel probability P 羊 吉 (else no information is sent) it
follows, on dividing by (1 - 2P) 羊 0, that the symbol probability p(a,)
is


which is what we would expect from the symmetry.
    Thus we쁘뜨쓰[0쁘－女暳越咀j血뾔S廻廻雙
                                                으프쁘므브Ii쁘쓰
cap므쁘L      꿋
                  C = 1 - H2(P) = 1 - H2(Q)          (8.5미
                                                      ／八뇨／\J八H/                 m누 긔


which occurs when the two input symbols are chosen with equal fre-
quency.


8.6C이M玭on可 Mutua/ 初加r刃zat加n

How can we find the symbol probabilities p(a) to meet the channel
capacity in more general cases? This section gives one very useful result
that helps answer this question in many situations.
     Returning to the general channel, we can write


            In(A;
              'A·
                ,
              ' ,'' B)'' = 巴_d
                           2可  n(a)
                                'm' 2 P(b
                            4 r \ ' 늉 Pr
                                       '' I1' m
                                              a)' l.g
                                                  l。 J[P(b .a)
                                                           '        口 [' p(b)          j
                          = 2 p(a)I (a; B)

where we have written the conditional mutual information as


                F(n.
                - ' n ,' 尸 '
                     ,'   B)
                               =   2
                                   늉 ' '' '
                                       P
                                           (b
                                                I ' 'mg [' Pt!기.
                                                 a)
                                                      1。
                                                               [P
                                                                    (b
                                                                         ,ia)
                                                                                   1
                                                                                   ]
In general, l (a; B) depends on a, but we have the theorem: 'When the
input symbols are picked to meet the channel caiiacity C. then'



for every of a [assuming that p(a) 半 01.
     To prove this, we assume the contrary, that some symbol, say a1,
is operating above capacity. Then, since the average is C, there must
be some symbol, say a2, that is operating below C. Thus we assume
162     C/i. 8 / Ch口nnel C口I）口city


that

                                                                               I (a1; B) > C

                                                                               I (a2; B) < C

     For an infinitesimal change that increases p(a1) and decreases p(a2)
by the same amount (to keep the total probability equal to 1), the direct
rate of change in I (A; B) is the difference

                                                              al(A ; B)                                  ol(A ; B)
                                                                     加佃）                                  ap(a2)

But the change in the p(a) induces a change through the channel equa-
tions in the p(b). The rate of change in each p(b) is given by

                                                              P(b I a) - P(B I a2)

From the expression for the mutual information,



                  I(A;』；B)
                  7（    5) = 쭈A「p(a)
                                 （. B P(b I
                                  ）各7(61.)1.8fP
                                            a) log (b
                                                   p(b)I a)]j
we have, therefore, the instantaneous rate of change in I (A; B) as



       恥(bI a1)log[P（出'丁 믐「(bI a2)log["잃川
        +              p

        = I (a1; B) - I (a2; B)
                                (a)         { 믐 -                    P    (b     I   a)         [-              -   ]       [P   (b        a1)   -   P   (b   a2)   ]}


        -       믐
                B A
                  )p                  (a)       IP I) ]  p
                                                         (b    (b)       a)     j    [P    (b            I a1)          -        P    (b   I a2)]
        = I (a1; B) - 1(a2; B)

        -2        [P(b 1 口l) 寸 P(b 1 a2)]

            二   （, ,       四）               -       ,(   , ,         바                    (1         -     ,)
       口石二(a而크
                        Sec. 8.6 / Conditional Mutual Information   163

     Since we were operating at channel capacity and it is the maximum
that can occur, and since the change has an instantaneous rate that is
positive, we see that if our hypothesis were true, we could get above
the maximum by a suitably small change in p(a1) and p(a2). We con-
dlude, therefore, that the hypothesis that any letter operates above the
channel capacity must be wrong; el坦ryJyjzr1wL.yj.. h. source alphabet

妃쏵袈黑器總굶黑絮三鴛瓷黑器퓽無寯籌孺
the md加1(如카可미' s that meet channel capaci勺-we can find them one
at a time.
（沇叩ter 9



                                  Some Ma玩em航cal
                                              Pre功冗m72anes




9.1 Introduction

Some people believe that a theorem is proved when a logically correct
proof is given; but some people believe that a theorem is proved only
when the student sees why it is inevitably true. The author tends to
belong to this second school of thought. Therefore, we make a digres-
sion at this point to prove, rather than assume, a number of results that
are needed to understand the proof of Shannon's main result. The
subjects are presented in sufficient detail so that a general appreciation
of them is obtained, not just a mere acquaintance with the result. Thus
more than the minimum material is occasionally presented.
      The two main ideas are n-dimensional space, and the law of large
numbers. We have already seen how n-dimensional space is useful for
representing code symbols. Since we are going to use large extensions
of codes to get near the entropy, and hence the channel capacity, the
dimension of the space of the proof will be very high indeed.
      The law of large numbers is needed to handle the fact that when
we are near ideal signaling rates, the number of errors in a code word
is very high. The manner in which the probable number of errors is
distributed is central to the proof of Shannon's main result.
      We will also need to bound the tail of a binomial distribution to
show that it does not contribute very much. For this we need the famous
Stirling approximation to n! This approximation is often used but is
rarely presented in a simple manner.




164
                               Sec. 9.2 / The Stirling Approximation to n!        165

9.2 T九e Stirli兀gAj까7ro工I刃zation to n!

The Stirling approximation to n! is

                                 n! - nt1e "\ /                ;;i            (9.2-1)

It is widely used but is seldom completely presented. We need it, so
we shall derive it.
      The quantity n! is a product, and products are hard to approximate.
This suggests approximating the log of n!:


                                 logn! = 2 logk
                                                   k= I


(all logs in this section are loge). The summation in turn suggests the
integral (which we do by integration by parts)

                                                                          n


                    f"
                         log
                                 x   dx
                                          =   (x
                                                     log
                                                           x    -    x)
                                                                          l

                                          = n log n - n + 1                   (9.2-2)




                         Figure 9.2-1 Trapezoid rule
166    Ch. 9 I Some Mathematical Preliminaries

    If we use the trapezoid rule to approximate the integral (see Figure
9.2-1), we will under-approximate the area. Therefore (log 1 = 0),


            J"
                 log
                        x   dx
                                   !   {   log
                                                 1 + log 2 + log 3 +   .




                                       + log(n - 1) + { logn
                                   之 log n! 尸 글 log n

We have, using (9.2-2), and transposing one term,

                       nlogn - n + fl ogn + 1 之logn!

Taking antilogs (which due to the positive growth and monotonicity of
the log function preserves the inequality direction) we get, term by term,
the upper bound,

                                       rine1八／;ie 之 n!                     (9.2-3)

    To overapproximate the integral we use the midpoint integration
formula and note (Figure 9.2-2) that if the midpoint line segment is




                                                                                 x




                                 Figure 9.2그 Midp이nt 的rmula
                                    Sec. 9.2 / The Stirling Approximation to n!                                   167

tilted until it is tangent to the curve, then the area under the line segment
is not changed. For the first half-interval, 1 드 x 5 클, we use the tangent
line at x = 1 to get a bounding triangle of area 吉. For the last half-
interval we use the maximum, log n, and get a bounding area { log n.
We have, therefore,


   1:
         log
               x   dx돠
                             + log 2 + log 3 +              .   .   .       + log   (n
                                                                                         -   1)
                                                                                                  + {   log
                                                                                                                 n

                                          l
                                          18
                         드 log n!    + 글 小 글 log n

Again use (9.2-2) and rearrange, to get

                         n log n - n + 1-           츙 + 글 log n 드 log n!

Take antilogs, we get the lower bound,

                                        n"eH"\ /i e718 드 n!

        The coefficient C of the approximation

                                        n! = nne "Vi C

lies, from (9.2-3) and (9.2-4), between

                                           e718 5 C 드 e


or, in numbers,

                             2.39887 . . . 5 C 5 2.71828 . . .                                                (9.2句

Since the midpoint formula has approximately one-half the error of the
trapezoid rule, and the errors of the two formulas have opposite signs,
a better guess at C is the weighted average

                              2e718 + e
                                               =250534                  '    == r                             (9.2-7)
                                    3           小   !   n




It will turn out that the value for C (for infinite n) is

                                    ＼厄；
                                      ;= 2.50663 . . .
168         Ch.        9 / Some 1%了口them口tic口／ Preli,兀m/ianes


     If we want to get this coefficient C exactly (for infinite n), we use
a trick and consider the integral

                                          /,                =        1:                               12
                                                                                                           m8* !d노                                             旴0)
A trigonometric substitution gives (k 之 2)

                                           fn/2
                         /k   =
                                          J。 cos' ' 工（1 + 釘n" 兀） dx
                                          I0

                                                                                                       。2
                                                                                                       iT!

                                                                                                                         cos' 2x( H sin 工） sin 工 (／工


Integration by parts gives
                                                                                                                         1T12                                                 m   ／八
                                                                                                                                                           1
                       ：『         "                                                                                                                            1
                                                                                                                                                                 l                     cos
                                                                                                                                                                                             '
                                                                                                                                                                                                 1xcosxdx
                                                                                                                                          k
                                                                                                                                                                                  "
                                                                                                                         0
                                               '
      乙＝         /,.                  :            卜？                                 sin:
                                                                                                                                                       -
                                                                                                                                                                         J。
                                  /, 1
                       42
                                          k
             =
                                                                1)
             =
                                                                                                 Ik
                 'k-
                 7,
                                                        -




Solving for 'k ' we have the recurrence relation for the integral,

                                                            =
                                                                                                                         '                                     (k 之 2)                                      (9.2-8)
                                                                          (k
                                           7
                                                                                                           -
                                                                                                                               )7h2
It is easy to show that

                                                                                                                         1l = 1

                                                                                                                                          ii
                                                                                                                         Jo = ;
                                                                                                                                          乙


           We next note that since cos x 5 1 for all x in the interval,

                                                                               '2k-                            i         > '2k > '2k+ 1                              -
Divide through by I2k_ 1:

                                                                                             ,         ,                              \                              i
                                                                                             I
                                                                                                                                                '2k+
                                                                                                                         '2k
                                                                                                       -           ;11                -        ;1
                                                                                                                   1 2k 寸 i                    1 2k- 1
                          Sec. 9.2 / The Stirling Approximation to n!                                 169

Substitute from (9.2-8) for the integrals to get


             1> 2k[2k:_ ' 打·긔'卜2k
                               2k +,
We can make the numerator in the square bracket equal to (2k)! by
multiplying both numerator and denominator by the denominator. We
also use the fact that

                   2k(2k - 2)(2k 小 4) . . . 2 = 2kk!

to get

                             1                  (2k)!                     12                2k
                   1 > irk
                             L2       '   (k!    )2
                                                      "
                                                          (k!        )i            >   2k   + 1


     We now take the positive square root of each term:



                1＞마k!)(2k)!2221
                            '구 :k1+ 1                                                             >



Finally, we substitute the approximation (9.2-5)

                             n! = rinen\/5i C

into this for each factorial to get



          kkk好甘C小/1 :2k+1 ,
      1＞마：(
Practically everything cancels and we have

                                  匹
                                                                               ,       1
                                                                               2k+ 1
                                                                /1
                                  C
Therefore, for large k,
170      Ch. 9 / Some Mathematical Preliminaries

Thus we have the Stirling approximation. As Table 9.2-1 shows, the
ratio of Stirling's approximation to the true value is remarkably good
even for small values. The table shows that the approximation was
designed to be relatively exact for n = 以）, but the difference does not
approach zero.

                                          TABLE 9.2-1 Stirling Approximation
       n                                  Stirling                  True                    Stirling/True




        4l 八乙 2口 41 <J 6 n/ 8 0/ 0
                                                                                l n乙 /b 4
                                              0.92214                  1                      0.92214
                                              1.91900                  2                      0.95950
                                              5.83621                  6                      0.97270
                                                                           싸乙
                                             23.50618                 24                      0.97942
                                            118.01916                120                      0.98349
                                            710.07818                720                      0.98622
                                          4,980.3958               5,040                      0.98817
                                         39,902.395               40,320                      0.98964
                                        359,536.87               362,880                      0.99079
       l
                                      3,598,695.6              3,628,800                      0.99170


      If this seems strange, consider the two functions

                                                     f (n) = n + \/i
                                                     g（미 = n
The limit of the ratio

                                        f(n')     fl + 'Ji      .          1
                                       ＝寸긋 =                 == 1 + :==1H l
                                       g(7iJ          n              Vn

The difference

                                                /（미 -g（川 = V万 -3 CC

9.3 A Birn刃U自ii Bound

Another mathematical result we need is the number of vertices in the
unit cube of Section 3.6 that are in a sphere of radius n. This comes
from the Hamming bounds like (3.6-2). Thus we need a bound on a
sum of binomial coefficients

                                     1 + C(n, 1) + C(n, 2) + . . . + C(n, Xn)                           (9.3-1)

where 0 < X < { . (We suppose that Xn is an integer.)
                                                                      Sec. 9.3 / A Binomial Bound                                  171

      Since A < 吉, the terms are all monotonically growing in size, and
 the largest is therefore the last one,


                                C                                                                        :
                                            ,4)
                                                   =
                                                        (,
                                                        (An)!                                            !
                                【
                                    (n,
                                                                 ,),(n!
                                            An)
                                                   =
                                                                                               ,,
                                                                                                     )
                                    （4,
                                                                                                                              3-
                                                                                                                        (9.
                                                                              (n
                                                                                   -           An)
                                                                                                                                   2)
We apply the upper and lower Stirling's approximations (9.2-3) and
(9.2-4) to each factorial as appropriate to get


 r (1}  노 11\ 4：二
                                           n1eH"\／듀 e
    ' " " " / 卞 [（入n）入" em入" \／仄；;e7'8] [(n 놔 入7i)(' ＋入4)ed" 卞入"入／n 1 入n e718]


Regrouping terms, we get



         C(n,An）小，n,(nfl- Xn)뇨 -'伊小品．,.,
                                                  eVi
                           x
                               e(718)＼仄；;e7'8)'v'(1 - 시n

The first and third brackets are exactly 1 and the other two become


           C
               (n,
                     An)
                               5    [             1      ,   -




                                          AA(1 - 入）（上H入'i LeJ／叭（1- 入）nj
                                                                          ,   ]r
                                                                               "       -   -             1
                                                                                                             11/
                                                                                                                   2

                                                                                                                       (9.3-3)


The log to the base 2 of the denominator of the first bracket is

   log[ AX(1 - 入y시 = 入 log 入 + (1 卞 入） log (1 小 入） = -H（시

Hence the first bracket of (9.3-3) is

                                                       2" （시                                                           (9.3-4)

The second bracket is a constant times nm("2).
    We now write the original series (9.3-1) in the reverse direction

           C(n, 入n) +C(n, 入n- 1) +. . .+C (n, 1) +1

and we bound the sum by a geometric progression. To get the "rate"
of the bounding geometric progression, note that in going from term to
term in the usual way, each binomial coefficient is found from the
172     Ch. 9 I Some Mathematical Preliminaries

preceding one by multiplying by (term by term)
                                      l
                     nm
                      l
                          n               n        八乙
                              H                H

                                                                7i H 入n + 1
             !
                              2       1
                                               3        1

                                                                    入n

If we start from our maximum term C(n, Xn) and go down, we have
the multipliers which are the reciprocals of the previous numbers and
are in the reverse order:

                          사i               3     2   1
                 n-       Xn+ 1 ' " " " 'n- 2 'n- l 'n

We need to bound these. An upper bound of these numbers is

                                                     入
                                                   1- 入

so an upper bound on the sum of the binomial coefficient terms is the
largest term times

                                  入        m

                                                            1        1 - 入
                 工
                                                                              (9.3-5)
                 2
                                                                              =


                 向
                                  1
                                                                入    1- 2入



      Assembling everything of (9.3-1), we have [use (9.3-4) and (9.3-5)]



          計(n,k)(28/ [e'2X小 X)]"'，‘소（可"
For all n sufficiently large the product of the last three terms is less than
1; hence for sufficiently large n,


                                      2C (n, k) 5 2nH(X)                      (9.3句


where H (X) is the entropy function of X. This is our needed inequality.
   Note that the sum of all the binomial coefficients of order n is


                                          2C (n, k) = 2"
                                       k= O
                                                               Sec. 9.4 / The Gamma Function 17(n)                                                173

as can be seen from the generating function


                                            (1 + x)' = 2 C(n, k)x'
                                                                                             k= O


when you set x = 1.


9.4 T九e Gami兀a Fundi加n F(n)

To extend the factorial function to nonintegral arguments we begin with
the study of a certain definite integral as a function of a parameter n.
Consider the integral


                                                17   (n)
                                                                    =           fe寸닉노
                                                                                                                                              (9.4-1)


The exponent n 中 1 is conventional. For n > 1 we can integrate by
parts to get

                                                                                              伽
                                                                                                              I
                                                                                                              D
                                                                        m

                                                                                                                                              +
             17
                                                                                                                                          1
                                                                                                                      e_
                  (n)
                         =          :   "       '    튼；
                                                                        0                                     J。               xxn_
or

                                            I,（미 = (n - 1)F(n 叫 1)

For n = 1 we have


                         17   (1)
                                            =              j   e_
                                                                            x
                                                                                        dx
                                                                                               =     -
                                                                                                         e나
                                                                                                                  戈




                                                                                                                  0
                                                                                                                           =
                                                                                                                                      1


and it follows that for integer n,

                        17(2) = 1
                        17(3) = 2!
                        17(4) = 3!




                        17(n) = (n - 1)!                                                           (n = 1, 2, . . .)
174    Ch. 9 / Some Mathematical Preliminaries

The gamma function provides the natural generalization for the factorial
function since the integral also exists for noninteger n.
    We consider next the gamma function for argument { . We have


                                                  I-   ,（吉）                       =                  뇨네2                                                  dx
The substitution x = t2 rationalizes the integrand and gives


                      F   ({)                 =
                                                                             e_
                                                                                          t2
                                                                                                                dt                    =        2
                                                                                                                                                         J。
                                                                                                                                                         I,         e
                                                                                                                                                                          t2
                                                                                                                                                                               dt
                                                           J。                                              t


Since the integrand is an even function, we can write this as


                                                                F   ( )                   寸：                         ,            e       !2        dt
This is often called the error integral.
    Consider, now, the product



                  F       （글）（굴）          F                         =                 f          ,         尸                  '       d노J ,                         e     Y2 dy



We transform (formally) to polar coordinates


                                              ({)]2
                                                                             =

                                                                                      i i:
                                                                                                                     g
                                     [r                                      =            J2i,                                        e
                                                                                                                                              『2r
                                                                                                                                                               dr   dO
                                                                                                                                          出
                                                                                                  n
                                                                                                 n乙

                                                                                                                                          0



Therefore,

                                                                                  F({) = \／규

    To justify the formal change to polar coordinate, suppose that we
consider finite limits


                           1
                               (L)                     =                J-            L
                                                                                                 e
                                                                                                               x2
                                                                                                                         dx
                                                                                                                                          J         ,          e
                                                                                                                                                                    , 2
                                                                                                                                                                          dy
                                   Sec. 9.4 / The G口mm口 Funct加nr（미                   175




              Figure 9.4-1 Rectangular-to-polar coordinates


We have from Figure 9.4-1,


                        .,     .   ..   .. , .        (2町 (L\巨       .,     .   ..
           f2竹 尸
                 e           r ar ati 5 1IL) 5                   e        r ar au
          I0
          J。 J。                                  J。 J。
                        '                                            '
                                                         J0
               I0                                J0
or

                    ir(1 叫 e '2) 드 /(L) 5 ir(1 小 e21-2)

As L -p   a , we get

                              町 드 /(L) = F2({) 5 丁r


Thus the transformation from rectangular to polar coordinates is jus-
tified and we believe that F({) = V.
176   Ch. 9 / Some Mathematical Preliminaries

9.5 小D加妃nsional Euc／
                   自lean 枷ace

n-Dimensional space merely means that we have n independent variables
x1, x2, . . . , x月. Euclidean space means that we use the Pythagorean
distance

                              工2 + 堵 + . . . + 工三 = r2                                                                                 (9.5-1)

and we can define a sphere of radius r by this expression.
     A little reflection on classical Euclidean geometry will suffice to
see why the volume of an n-dimensional sphere depends on the radius
r as r". Therefore, we have the formula for the volume

                                                   V (r) = Car"                                                                        (9.5-2)

where Cn is some constant depending on n. For example,

                                                                     4'rr
         C2 = IT             and                   ('3 =                                        (note that C1 = 2)
                                                                              3
                                                                     =e
     To find the values of Cri, we use the same trick as in Section 9.4
of multiplying the gamma integral by itself and then going to polar
coordinates (which worked so well). Let us consider the product of n
of the integrals. We have [using (9.5-1)]

        r  l41
                 n
                                           乂
                                                                                                        r2
                     =   IT nf2 =     J:       ,    i:   ,       ·        ·        ·   f_   ,   e
                                                                                                              血，   dx2.   .   .   dx
                                     = J e_r' 斗이「
This last step takes a moment's thinking about the shell of thickness Lr
and comparing this with our result in two dimensions,


                         J ' 呵,'）小 = 2寸e '"r dr
as we really did in Section 9.4 (although it was disguised somewhat by
the conventional method).
     We have, therefore, using (9.5-2),

                                      2                                                             l
                               :8/
                                           =       c         J   『
                                                                              e_       r2nrn_
                                                                                                         dr
                                           Sec. 9.5 / n-Dimensional Euclidean Space                                                                   177

Set r2 = t. Then dr = 吉t- "2 di', and


                  :nI2                 ：   프判                                 ，『   e              '    "   "     ',   :;'di          '

                                       -




                                                 2
                                                                   I
                                                                   J。
                                                                                   e4             《t
                                                                                                       (8/2           1)        dt
                                           n如（斗미；                                                                                        +   1)
Therefore,
                                                                                                       町n12
                                                           n
                                                      c'       4          =                       /                         \


                                                                                            （知）
                                                                                        '
                                                                                   1
It is easy to show that


                                                                                                  끄 n
                                                                   q
                                                                                                           cn口
                                                                                                                                                  H

                                                                                                                                                  1




and we can compute the table (of the volume of a unit sphere in n
dimensions)

                   n                                               C           "




                         1
                         l n V d
                           乙 2 1 <
                                 V 6
                                                            2                                                          2.00000. . .
                                                            qT                                                         3.14159. . .
                                                         4ir/3                                                         4.18879. . .
                                                          4T 2/2                                                       4.93480. . .
                                                       81T2/lS                                                         5.26379. . .
                                                         ir316                                                         5.16771 . . .
                         m
                         / 8
                                                      16ir3/105                                                        4.72477 . . .
                                                        'rr4/24                                                        4.05871 . . .


                  2k                                       町k/k!                                                       -+                0


    From the table we see that the volume of the unit sphere, or equiv-
alently the coefficient of r", comes to a maximum at n = 5 and falls off
rather rapidly toward zero as n approaches infinity.
    For n = 2k, the volume of an n-dimensional sphere of radius r is

                                                                       ）「2k
                                                (i;
                                                                                                  =        （   『k!              '
178    Ch. 9 / Some Mathematical Preliminaries

From this we see that once

                                                  k > '7rr2

then increasing k (or equivalently n) will decrease the volume. Indeed,
given any radius, no matter how large, the dimension of the space n
can be increased until the volume of the sphere is arbitrarily small.
[For odd-dimensional spaces, we have, from the original definition of
F(n), equation (9.4-1), that

                                                                 1rn/2 rn
                                    V,(r) = Cnrn =
                                                               F(n12 + 1)

will change smoothly with increasing n.]
     We now consider the fraction of the volume of an n-dimensional
sphere that is within a distance r of the surface (r is used here as any
small positive number). We have


                                                                                    Eer
                                                                                                  n




                                                                                     \ \ 1 r /r
                                                                            /
               shell                C,r ' - C (r 尸 E)" = 1
                                                                            1
                                                                            1
                                                                                l                     H
                                                                                                      1
                                                                            1
                                                                            1
            , , n1   . . n1i,   -          Cnrn
                                                                            \
which approaches 1 as n gets large. Thus for a high-dimensional space,
almost all the volume of a sphere is arbitrarily close to the surface.
Indeed, no matter how thin a shell you wish to use, and how close you
wish to get to 1 (say 99.44%), it is possible to find an n0 such that for
all greater n, the two conditions are met. There simply is not much
volume inside a high-dimensional sphere; almost all of it is "on the
surface."
      Let us now examine the angle between the vector from the origin
 (0, 0, . . . , 0) to the point (1, 1, . . . , 1) and any coordinate axis. The
projection on each axis is, obviously, exactly equal to 1 (its coordinate
 value on that axis). The length of the vector is \/n; hence the angle
 we want, 0, is given by


                                          cos.        =   ｛느
As n -     m, this approaches 0; hence 0 -)   ir12. Thus for sufficiently
large n, the diagonal line is "almost perpendicular" to each coordinate
axis!


Exercises

9.5-1 Show for any family of convex similar figures that "almost all of
      the volume is on the surface."
                                            Sec. 9.6 / AP口r口do工       179

9.5-2 Show that the volume of a 2k-dimensional sphere divided by the
      corresponding volume of an enclosing cube is ('T114)"(1/k!).


9.6 A Par口而工

The results of this section are not needed but are included to show how
unreliable your intuition is about spheres in n-dimensional Euclidean
space.




                                                       (0, 0)




                          Figure 9.6.1 A paradox

     Suppose, as shown in Figure 9.6-1, that we have a 4 x 4 square
centered about the origin (0, 0) and have four unit circles in each of the
four corners. Now consider the radius of the circle about the origin
that is tangent on the inside to the four circles. It has a radius

     r2= \/(1_ 0)2+ (1_ 0)2_ 1= V                  _ 1= 0.414. . .

     Next consider the same situation in three dimensions. We have a
4 x 4 x 4 cube with eight unit spheres in the corners. The inner sphere
has the radius

                      r3 = \/3 - 1 = 0.732 . . .

     Finally, consider the similar situation in n dimensions. We have a
4 x 4 x . . . x 4 cube with 2? unit spheres in the corners, each one
touching all its n neighboring spheres. The spheres are packed in prop-
erly. The distance from the origin to the center of a sphere is given by
the expression

          V(1_ o)2+ (1_ o)2+ . . .+(1_ 0)2= Vi
180    Ch. 9 / Some Mathematical Preliminaries

Again subtracting the radius of the corner unit sphere, we get the radius
of the inner sphere in n dimensions as

                                   r, = V;i - 1                               (9.6-1)

      When n = 10, this is

           r1。=VT6-        1= 3.16. . .-1=                    2.16. . .>2

and the inner sphere reaches outside the cube! Does this seem impos-
sible? The spheres are convex surfaces to be sure, the distance is surely
the correct Euclidean distance, and the radius of the corner sphere is
surely 1- so there is no escape from the conclusion. Contrary to any
normal intuition, the inner sphere for n 之 10 reaches outside the cube.
     To compound the paradox further, consider the volume of this inner
sphere relative to the whole cube as a function of n. We have, for the
special case of n an even number n = 2k, and using (9.6-1),

                        volume of sphere                       (V;i - l)n
            ratio =                        =                        .

                      volume of whole cube
                                                                ’
                                                        Cri
                                                                    'I. " .



                      C    (\ /7i 小 l) "
                       V2k       42k


                      "'吃咨/ )2k[(1 制丁"
                                                   \／巨k 기 \／三k


                 月詰' [(i 缶）"" ]                                               (9.6-2)


 Using Stirling's approximation (9.3-1) for k!,

                                  k! 느 k노寸 \/2;;i

 and the result from the calculus,


                            工m+ 工
                             如，
                                    (i그，
                                           )   '   寸1


 We get for (9.6-2),


                        ratio: 42*二e“2kk\뇨k「；，丁'
                                  : （쥐'寫                                       (9.6-3)
                  Sec. 9. 7 / Chebyshev's Inequality and the Variance                                          181

 But

                                            쯔
                                                = 1.06747. . .
                                        8
 Taking loge of both sides, we get, as k approaches infinity, loge (ratio)
 = (0.065288 . . .)k - ＼厄k- 글 loge k 卜 글 幻g, 2 -今 m. Therefore,
 we see that the factor



                                                    （뒤                       '


will go to infinity faster than the other two factors in the product
(9.6-3),


                            e ＼厦"                                                          1
                                                    and
                                                                                         \／巨규k

can decrease it.
     We conclude that the volume of the inner sphere becomes arbitrarily
larger than the volume of the cube which contains all the 22k = 2' unit
spheres in the corners.
     The case of the odd dimension n = 2k - 1 does not change matters;
it only makes the details more messy.


9.7C九e力ys九ev농 /nequa／吻 and I九e Varia砒e

If a random variable X is discrete, then the mean square is given by the
expectation

                                                             工


                           E｛肛｝ = 2                                              玗可助
                                                    7=
                                                                 -




and if the variable is continuous, it is given by



                           E{M}
                                                :   f        ,           尸p              (x)
                                                                                                     d노

For any E > 0, since the integrand is positive, we have


                       ,   尸，                                                        ,    ,               d노
                                                                     '
                  I:
                                  )d노
                            (/
                                                                                               尸小）
                                                         I
                                                                         ,       口
182     Ch. 9 / Some Mathematical Preliminaries

and this can be written as



            E{ -}>1,m,xp(x)dx! 821, ,, p(x)dx
It follows therefore that

                      E{X2} 之 E 2 Prob{ 1 X 1 之 E}

or


                       Prob{ 냥 1 三 .} 5 E｛冬" }                  (9二1)


This is the famous Chebyshev inequality (expressed either in continuous
or discrete notation).
     The variance, or dispersion, of a random variable X, labeled V{X},
is the mean square measured about the mean value

                               E{X} = 口

Thus the variance of a random variable X is

                   V{X} = E{(X - a)2}
                         = E{X가 -2口E｛치 + E{r尸｝
                         = E{X가 - 2a2 + 口2
                         = E{X2} - a2 = cr2

Clearly, since E{1} = 1, the variance has the property that for any
constant

                                V｛아 = 0

We also have

                             V{cX} = c2V{X}

      If X1 and X2 are independent random variables, and if we write

                      피X1} = a1        V｛치｝ = ci-子

                      E｛石｝ = a2        V｛차｝ = 畦
                                        Sec. 9.8 / The Law of Large Numbers          183

 then we find that

       E{（兀 小 떠）
               （石 中 a2)} = 万｛(X1 - a1)}E{X2 - 口2)} = 0

The variance of a sum of two independent random variables X1 and X2
is

   V｛兀 + 兀｝ = 万｛
               （兀 + x2- 口l 小 口2)2}

                           = E{（石 - ai)2} + 2E{(X1 - a仄兀 1 口2)}

                                  + E{(X2 - a2)2}

                           = V{X1} + V｛石｝ = O三 + 畦                                 (9工2)

     It follows by induction that the variance of a sum of any number
of independent random variables is the sum of their variances.


Exercises

9.7-1 Carry out the proof of the Chebyshev inequality for the discrete
      variable case.

9.7-2 The entropy is the expected value of log (lip1). Examine the
      corresponding formula for the variance.
                                           Ans. 2 p, 1og2(11p1) - 了2


9.8 The Law of Large Numbers

If we make a large number of Bernoulli trials (meaning that success or
failure is a random variable X with values 1 or 0, respectively, and each
trial is independent of all other trials), then we can ask for the number
of successes relative to the total number of trials, and hope that this
ratio will approach the probability of a single trial. This is simply hoping
that the frequency of successes in a long run of trials will approach the
probability of a success for a single trial. To get the formalism going,
we consider the random variables 兀, which is 1if the ith trial is successful
and 0 if it is not. What will the average be? We set up the expression
for the expectation of the average


            E{
                 ,
                     (X1
                             『兀
                                    『   ·   ·   ·   『兀）
                                                          }   :
                                                                  l
                                                                  d
                                                                  1n  2E{X1} = 口

where a is the expected value of a single trial.
184          Ch. 9 I Some Mathematical Preliminaries

         We next look at the variance of the average


                             心小小，[2(Xi a)]2}
                                                                           （兀－
                                  =

                                                                     2
                                                뇨｛                                       .)"}
by (9.7-2), since the cross products drop out. But these are identical
trials; hence




                                                                     no2            a2

                                                                         /22        n



      We now apply Chebyshev's inequality (9.7-1),


      Prob      {                          >E
                                                             \111\

                                                             1
                                                             J
                                                                     드
                                                                           E
                                                                          l구
                                                                                    l
                                                                                    구
                                                                                        2 （戈
                                                                                                     n
                                                                                                          /
                                                                                                         4乙
                                                                                                          J
                                                                                                          1
                                                                                                          \
                                                                                                              1
                                                                                                              )rj
                                                                                                                H
                                                                                                                    )
                                                                                                                    /
                                                                                                                        (9.8-1)


Reversing things, we can write this as


                      Prob    {       !,2 （兀 H .) < E. l. 之 1 - :=
                                                                /iEH
                                                                               )1

                                                                               J
                                                                                           d
                                                                                                m2
                                                                                                U




     T九eore刃i: Weak law of ／口rge numbers. If 兀，兀， . . . , 兀 are n
independent identically distributed random variables with mean a and
variance a2, then given any E > 0, and 8 > 0 however small, there is
an integer n0 such for all n > n0,


                    口 -r      드        {x1 + x2 + . . . + xn} 드 a + E                                                   (9.8-2)
                                  1    .             -   -




                                  n


with probability greater than 1 - &. The theorem states that the average
can be brought, probably, as close as you please to the expected value
a.
                              Sec. 9.8 I The Law of Large Numbers       185

      The proof follows whenever we pick n。such that [from (9.8-1)]

                                 으三 < 8
                                 1m   n2
                                 'to乙
 or
                                           르耐
                                 no>

       Since this theorem is widely misunderstood, we pause to comment
 on it. In the first place, since they are Bernoulli trials, that means that
 the trials are independent-the trials have no memory of what has hap-
 pened in the past. Therefore, the very concept that the law of large
 numbers means that in time any run of bad luck will later be "compen-
 sated for" by a run of good luck must be false. What happens is that
 any fluctuation from the average will be "swamped" (probably) in the
long run, not that there will be compensation.
      Furthermore, it does not mean that the sum comes close to the
expected value, which is, of course, np.,. For example, in 10 tosses of
a fair coin, you expect 5 heads, but a value as large as 8is not surprising.
In the million tosses we do not expect to be as close as 3 (as we were
in the 10 tosses with 8 heads) from the expected value, but it is per-
centagewise that we come closer and closer-probably! The misun-
derstanding comes when you do not watch where the n is- it is in the
denominator and when it is there, probably the differences between the
number of actual successes and the expected number of successes divided
by the n will decrease as n gets larger and larger. But if you talk about
the difference between the number of observed successes and the ex-
pected number of successes, it can grow indefinitely large with larger
and larger n. In this it resembles the earlier Stirling approximation
(Table 9.2-1).                                                        "
      Because of its central role in the proof of Shannon's theorem, let
us illustrate the theorem by an experiment. Let the probability of an
event (success) be

                                 p = 赤

In N Bernoulli trials, what is the probability of k successes? The k
successes can occur in any k of the N trials, namely

                                 C（川 k)

different ways; therefore, the probability for the k successes (and, of
           186    Ch. 9 / Some Mathematical Preliminaries

           course, N - k failures) is

                                     C(N, k）少（i- p尸寸                              (9.8-3)

           The expected number of successes is

                                                pN


13-

12 니

11-

10 미

 9띠

 8미
                                                N = 100

      7-
 6-
 5-
 4켜
                                                          N = 30


                                                                        N = 10
 3-
                     1
                                                                                            kN
                                            1                       1             1

                    0.05      0.10         0.15           0.20     0.25          0.30

                            Figure 9.8.1 Law-of-large-numbers example

               In Figure 9.8-i we have plotted horizontally k/N so that the distri-
           bution of (9.8-3) is centered at the same place, namely p, the expected
           value of a single trial.
                To compensate for the compression of the horizontal axis, we plot
           N times the function (9.8-3), namely

                                     NC(N, k)p' (l - p)N_ k                       (9.8-4)

           Thus the area under the curve is held constant. Figure 9.8-i gives the
           distribution for N = 10, 30, 100. We see the peaking up of the distri-
           bution near p = 솖 and the falling away of the probability at places far
                           Sec. 9.8 I The Law of Large Numbers    187

away from the neighborhood of p = 솖. In Figure 9.8-2 we have shrunk
the vertical axis and give the cases N = 100, 300, 1000. (Only a few
points are plotted and the curve for N = 1000 would, in fact, be very
smooth indeed if we plotted all the points.)




                                                           長i
              Figure 9.8-2 Law-of-large-numbers example
188    Ch.   9 / So,刃eM口the刀i口tic口／Prelimin口ries


      Thus we see how, as the number of trials N increases, the distri-
bution centers around the expected value p, and the variance decreases
like iiv刃. At N = 1000, for example, a deviation of k/N of as much
as 0.05 is very unlikely indeed. The probability of being at all far from
p can be made as small as you please by picking a sufficiently large N.
      We are going to use this theorem when we encode a message in a
very large extension. We can expect that the distribution of the dif-
ference between the number of actual errors in the transmission of the
block of symbols and the expected number of errors, when divided by
N, will get to be a very narrow spike indeed-provided that the N is
large enough. Always probably!
      We can use the law of large numbers in an interesting way to explain
more about the nature of n-dimensional space. Suppose that we con-
sider the vector from the origin to the point with coordinates 士 1 chosen
 at random for each of its coordinates. Now let us choose another such
random diagonal line. What is the angle between them? Each vector
is of length \/i. The cosine of the angle is therefore given by

                                    n


                                   2 （土1)（土1)
                         cos 0 = ' " '＼屈＼屈

But uniform random products ( 士 1)( 士 1) are 土 1 uniformly; hence



                            cos 0 =
                                         n


But "almost surely" for large n the sum divided by n (the average of
士l's) is near zero; hence, as in Section 9.5, the angle approaches 町/2,
a right angle.
     But there are 2t2 such random diagonal lines; hence in n-dimensional
space, for sufficiently large n, there are almost 2P2 almost perpendicular
lines! Now 2" is very much larger than n; for n = 10, we have 210 =
1024. Thus even at 10 dimensions n-dimensional space is very "vast"
indeed!



Exercise

9.8-1 Make similar plots for p = { , N = 5, 10, 20.
                                             Seer. 9.9 / Other Metrics   189

9.9 Other Metrics

The preceding material has been developed using the Pythagorean dis-
tance, L2:


                          d2 = 2 (x, - y,)2
                                 1=1


since that is the familiar distance measure. But coding theory often
uses the Hamming distance, L1:

                                n

                          d= 2         1 兀i H yi 1




                               Cfrc陀 in L1


                               Figure 9.9-1

With this distance function the circle (in two dimensions) looks like
Figure 9.9-1.
    The other main distance is the limit of the L distance as n -p m:

                        d, = 心2 I x, - y,4 H

In the limit we see that the tendency of the high power in the sum is to
select out the largest term and ignore the rest; hence we have the Che-
byshev, L, distance:

            d = tim 甲2 1 工, 小 yi n1 = max 1 工／ - yi 1
190   Ch. 9 / So力ie Mathem口tic口／Prelimin口ries




                             Circle in L,.,

                             Figure 9.9그


In this distance the circle becomes as shown in Figure 9.9-2.
     Many of the phenomena of this chapter apply independent of the
distance function used, but it is evident that the four-circle paradox
changes as the distance function changes.
     It is important to realize that the nature of n-dimensional space
depends on the distance function used, but that the "vastness" of the
n-dimensional space remains.
（沇apter 10



                     S九am加兀농 肋rain T九eo肥刃1




10.1 Introduction

In Chapter 6 we introduced the concept of entropy, and in Section 6.8
proved that there are encoding methods that come arbitrarily close to
the entropy of the input. In particular, we showed [equation (6.8-2)]
that by a suitably large extension of length n we can achieve the mlle-
qualities for the average code length L:

                       Hr   (S)   5   드 <Hr   (S)   +   !
                                      ri                ?2


Thus the encoding process can be done arbitrarily well, and the entropy
Hr(S) provides the limit on what can possibly be done.
     We next looked at the channel itself, and defined a channel capacity
C, equation (8.1-1). In the present chapter we prove the fundamental
result that even in the presence of noise, we can get arbitrarily close to
the channel capacity. More specifically, we can get arbitrarily close to
the rate, and keep the reliability of sending messages through the chan-
nel arbitrarily close to 1.
     We will prove the theorem for the binary symmetric channel, since
in this case the proof is easiest to understand, and it also provides the
most common model used in practice. We will merely indicate how
the underlying ideas can be extended to prove the theorem for more
general channels. The rigorous proof in the general case is complex in




                                                                      191
192     Ch. 10 / Shannon's Main Theorem

all its details and does not shed much more light on why the theorem
is true in general.


10.2 Decis良刃iRules

Suppose that you are at the receiving end of the channel and have
received the symbol b.. Which a. should you assume was sent? That,
or course, depends on me cnannei, tnat is, on me r (o1 1 a1) ana aiso on
the source probabilities p(a1) = p,.
     To get a feeling for what is involved, consider the particular channel
where we have the channel matrix P1,1 = P(b1 I a,):

                                        b1    b2    b3

                                              I
                         l   3       5        0.3   0.
                         口 口 n
                             -*(0. 2          0.3   0.51                    (10.2-1)
                                  10.
                                                         2\
                           4
                           n      \0.3        0.3   0.4/



Let d(b1) be the result of the decision rule you will use when b1 is
received. Even if you have a uniform input and all the p(a1) = } for
the source alphabet, the three sets of rules for this channel

                Rule 1                  Rule 2                  Rule 3
              d(b1) = a1         d(b1) = a1                   d(b1) = a1
              d(b2) = a1         d(b2) = a2                   d(b2) = a3   (10.2-2)
              d(b3) = a2         d(b3) = a2                   d(b3) = a2

are each defensible-arguments can be made in favor of each. Note
that we are here considering one symbol at a time, not runs of symbols.
     In the general case, there are s rules (one for each received symbol)
each of which may have any one of the q input symbols, so there are
in total

                                         qs
possible decision rules for picking an a, when a b1 is received.
     To settle the question of which set of decision rules to adopt, we
shall invoke the widely used ma工imum-likelihood rule of statistics. This
rule says that you should "take the symbol that is most probable, given
                                         Sec. 10.2 / Decision Rules    193

that you have observed what you have." In mathematical terms we
require (given equal frequency of the use of the input symbols, which
is the reasonable way to use a binary symmetric channel)

                                 d(b1) = a*

where a* is defined by the conditions

                   P(a* 1 b1) 之 P(a1 I b)        for all i        (10.2-3)

In words, given that you have received b1, no other a1 is more probable
than is a*. These are not the channel probabilities. To get to them
we use Bayes' theorem on each side of this inequality:

                    P(b1 I a* )p(a)* > P(b, I a加(a1)
                         p(b1)                p(b1)

Under the assumption of the uniform probability of the input symbols,
we have p(a*) = p(a小 and we get

                         P(b1 I a* ) 三 P(b3 I a,)                 (10.2-4)

for all i. Thus we now have the maximum-likelihood condition
(10.2-3) in the form used in defining the channel.
      We can use this rule even when the source alphabet is not equally
likely. This is not optimal in general, but- like giving away the opti-
mality of Huffman encoding and using Shannon-Fano encoding- what
we give away will not cost us too much in the long run. We will still
be able to obtain the desired result. This indicates a certain robustness
of the final theorem-it is not a delicately true theorem. We can deviate
fairly far from the best possible at various stages and still find that the
theorem can be proved.
     The maximum-likelihood rule is still not unique, as you can see
from the example (10.2-2). In the example for the channel (10.2-1),
clearly for the maximum-likelihood rule you must take

                                 d(b1) = a1

But given b2, you can pick any one of the following three:

                                 d(b2) = a1

                                 d(b2) = a2

                                 d(b2) = a3
194    Ch. 10 / Shannon's Main Theorem

as our rule. You will have finally, by the maximum-likelihood rule,

                                      d(b3) = a2

Thus there are three possible maximum-likelihood rules (10.2-2) for this
channel.
     What is the probability of error using this channel and this decision
rule? If we write the probability of an error as P(E I b1), then we have,
since P(a* I b) is the probability that the symbol a* we pick was the
source of the received b1,

                     P(E I b.) = 1 小 P[d(b1) 1 하］                          (10.2-5)

as the probability of making an error given that we have received b.
The average error j E is given by

                        PE = 2 P(E I b.)p(b3.)

This may be written as, using (10.2-5),

                  PE = >.p(b) - 2 P(a* Ib)p(b)

    Using Bayes' theorem (Section 7.3), we can reverse the conditional
probabilities to get to the channel probabilities [remember that all p(a)
= 1/q)]

                      PE = 1 - 2 P(b I 口' )p（미
                                                                           (10.2-6)

                          小諱P                              (b        I )
                                                                     a*


   Let us calculate this for the channel (using the underlined rule).
From



                                      0H 0 0        000
                                                      n
                                                      4V


                                           <U1 n乙
                              /
                           4
                           l 小八
                              J
                              1
                                                      八J
                              1
                                           n
                                           4U         八
                                                      4J
                              \
                                  \                             苔）
and using formula (10.2-6) we have

                    J노= 1 - 吉(0.5 + 0.3 + 0.5)

                        = 1 - }(1.3) = 0.5666 . . .
                         Sec. 10.3 / The Binary Symmetric Channel     195

10.3 T九e Binary Sy刃1刃wtr切 C九anne!

We now illustrate Shannon's main theorem by showing how the error
in the channel can be reduced by using an error-correcting code for the
binary symmetric channel. For a single binary digit we have the stand-
ard diagram

                                        P




                                       P
Note that P = the probability of correct transmission. We naturally
assume that Q < 吉, since if Q 之 글, we merely reverse the 0 and 1 at
B. For Q = 솔 we have all noise and the channel capacity is zero.
     For the nth extension of the channel (Section 8.2), we send n binary
digits. For example, for the third extension (octal code) we have for
single-error-correcting code (maximum-likelihood detection):

                Messages        Unused         Received




                                                   跏帥毗m蜘mmm
                   000                001
                                      010
                   111                011
                                      100
                                      101
                                      110




                   I나o error     P3

                     1 error     3P2Q (correctable)

                     2 errors    3PQ2

                     3 errors    Q3
                 ／노 - Q3 + 3PQ2 = 少(Q + 31乃

If P = 0.99 (99% reliable), we get

                            I노 = 3 )< 10니
196    Ch. 10 / Shannon's Main Theorem

      We see that the Hamming distance is in this case the maximum-
likelihood detector. In general, for "white noise" the minimum Ham-
ming distance provides the maximum-likelihood detection. In the case
of two message points of the same minimum distance from the received
symbol, we simply give up, or else toss a coin and guess (we will be
right half the time). In the case of more than two message points the
same distance away, we can still guess.
      For the nth extension of the binary symmetric channel, we see that
we have a uniform channel. How we use the channel in practice may
be another matter.


10.4 Ran勿刃zE兀coding

We are now ready to prove Shannon's main theorem, which states that
there exists a method of encoding messages that is arbitrarily close to
capacity and arbitrarily reliable in transmission (storage). We will prove
the theorem only for the binary symmetric channel, both because that
is the channel of main interest and because for this restricted case the
proof can be made intelligible to unsophisticated beginners.
     We will use block codes of n binary digits. These are simply the
nth extension (Section 6.8) of the binary code. There are 2' possible
strings of n binary digits, but if we are to have protection against the
noise of the channel we cannot use all of them. We must keep the
encoded messages far apart (in the Hamming distance) so that the noise
of the channel cannot cause errors (for almost all messages).
     First, how many messages do we need to be near capacity? If we
have M equally likely message [which is the way to use a uniform channel
(Section 8.2)], then the information per symbol a, is, since
                                        l
                               P
                                        而
                                                                        (10.4-1)
                    1   (a1)   =   in       !   =
                                                         1
                                                               = In M
                                                         1IM
                                                    in
                                            p

Now we know from Section 8.5 that the capacity of a binary symmetric
channel is

                        C = 1 - H (P) = 1 - H (Q)

for one binary digit, and hence for the nth extension we will have the
                                     Sec. 10.4 / Random Encoding       197

capacity
                          nC = n[1 - 11(Q)]

(by Section 8.3). To be near capacity we must have

                       I (a) = In M = n(C 中 l)

where cl is a small positive number. This may be written

                              - - -, .      2'C
                          M = 2r1(L - El) = =H    'iEl
                                                                   (10.4-2)
                                             '2
Looked at this way, we see that by increasing n the denominator can
be made arbitrarily large, so that we are taking a small fraction of all
possible messages of length n bits that can get through at capacity C-
provided that n is made large enough!
     Second, how do we design the code book so that all messages are
equally likely and are far apart? Frankly, at this point, we do not know
how to do this in general and we resort to random encoding. We know
from the end of Chapter 9 that in n-dimensional space, random points
are far apart, provided that n is large. Judged from the center of the
cube, two random vertices will almost certainly be almost a quadrant
apart. Thus, making random choices for the encodings is not as foolish
as at first it may seem.
     1To get the encoding of the first message in the code book, we toss
a well-balanced coin n times and record the corresponding sequence of
0's and l 's as the encoded message. We do the same for the second
message in the code book. And so on through the whole M messages
in the code book. There will be exactly nM tosses of the coin; hence
we will get one particular code book from the ensemble of 2"M possible
code books.
      An alternative and equivalent method of getting the code book is
to write all possible 21 binary sequences on slips of paper, put them in
a container, stir, select the first one as the encoding of the first entry
in the code book, return this slip, stir, draw the second slip as the second
encoded line of the code book, and so on, until all M messages in the
code book have been assigned. These are equivalent methods, and
both run the risk of having the same encoded sequence emerge for two
different messages. For large n, however, this is very, very unlikely,
as we will have to prove if we are to show that the error rate can be
made arbitrarily small.
198    Cli. 10 I Shannon's Main Theorem

     We picture these sequences as message points in an n-dimensional
Hamming space (Section 9.5). The probability of an error in any one
position of the block of letters is Q = 1 - P, and we expect nQ errors.
We consider a sphere about the chosen message point with a radius of
size nQ. Now consider slightly increasing this sphere by a relative amount
r2. The radius is now (see Figure 10.4-1)

                             r = (Q + r2)n                        (10.4-3)




                        Figure 10.4-1 Sending end


(r is the radius and is not the number of symbols or the radix, and r2 is
so small that Q + E2 < 글). The actual size of E 2 with respect to el will
be determined later.
      By the law of large numbers (Section 9.8) there is, for sufficiently
large n, an arbitrarily small probability that the received message will
fall outside this new sphere. (Since almost all the volume of an n-
dimensional sphere is near the surface, it is natural that we are mainly
concerned with a shell of thickness 2nE2 centered about the distance
nQ.) Thus if we use maximum-likelihood detection, and if we can prove
that almost surely no two spheres overlap, then we will have the result
that you, the receiver, can almost surely know what was sent.
      For the receiver we must invert the picture, and draw it centered
about the received message symbol b1 (see Figure 10.4-2). Drawing the
same-size spheres about the b1, we find the same probabilities for the
a1 being in the spheres as we had for the b/ to be in the spheres about
a1. We need to set up a formula for the error that you cannot decode
the message correctly.
      You will be in error if the proper a, is not in the sphere S(r) about
 the received b1, and you will also be in error if there is more than one
possible a1 in the sphere since then you will not know how to decode.
(We will decline to guess.) The following table gives the situation.
                                                Sec. 끄l4 / 凡rn而m Enc아／ing             199




                                                             ne2



                             ·a1
                            Figure 10.4그 Receiving end



                                    Correct          Other a,
      Cases                        a, in S(r)        in S(r)            Error



          4
          l n
            乙 n
              4
              U 4
                                     Yes               Yes          Error
                                     Yes               No           Correct
                                     No                Yes          Error
                                     No                No           Error

From this table we set up the probability /)E of an error. The
                                                               first term
covers cases 3 and 4 (too much noise) , while the second
                                                            term covers
case 1 (code points too close together). We have

                    ／노= P{a, 匹 S(r)}
                         + P{a, E S(r)}P{at least one other                     (10.4-4)
                                                code word is in S(r)}

where E means "is contained in" and 匹 means "is not contai
                                                                 ned in."
Since P{a1 E S(r)} 5 1 we can simplify (10.4-4) slightl
                                                        y by dropping this
factor:

                         ／노 드 P{a1 匹 S(r)}
                              + P{at least one other                        (10.4-5)
                                code word is in S(r)}

     We now look at the second term on the right. The words
                                                              "at least
one other     ...means "one or more code points in sphere in addition
           ..
to the given a,." Now given two events E1 and E2 it is clear that

             P(E1 and/or 夙） = 尸（瓦） + P(E2) - P（弓乙）
200     Ch. 10 / Shannon's Main Theorem

since a point in E1E2 has been counted in both E1 and E2 and must be
subtracted out. Since all probabilities are nonnegative,

                   只瓦 and/or 尻） 드 P（弓） +/)（瓦）

It is evident from this simple case that (summation over A - ai means
all of A except a.)

      P{at least one other code word is in S(r)} 5        2      P{a E S(r)}
                                                         A- 口i



where the summation is over the M 卞 1 code words not sent. We now
have, for (10.4-5),

                 가 드 P｛口i 匹 S(r)} + 2              P｛口 E S(r)}           (10.4-6)
                                           A 寸口i



In words, the first term is the probability that the sent word is not within
the sphere about the received word (equivalently, that the received word
is not within the sphere about the sent word). The second term is the
sum over all the terms not sent, any one of which might be in the sphere
of radius r, which is, relatively with respect to n, slightly larger than the
Hamming distance corresponding to the expected number of errors.
We hope that by using randomness the message points will be spread
out and that there will be only a very small chance that any other symbol
will be in the sphere. This, in turn, rests on the vastness of n-dimen-
sional space; it is very unlikely that any two random points will be near
to each other in a sufficiently high-dimensional space.
      The first term of (10.4-6), which depends only on the single symbol
ai, can be made less (by the law of large numbers) than any preassigned
positive number 3 = 6(r2, n) simply by making the block length n so
large that the extended sphere of radius r = n(Q + r2) covers the
 distances for all but the arbitrarily small number of possible cases. We
have, therefore, for (10.4-5),

                       I노 드 3+      2      P｛口 드 S(r)}                   (10.4-7)
                                   A -a1



One way of looking at this equation is that the first term contributes to
the error rate depending only on the particular code symbol sent; the
second term depends on all the other symbols in the code, and is related
to the rate of signaling, since it contains the M - 1possible code symbols
other than the correct one.
                               Sec. 10.5 / Average Random Code       201

10.5 Average Random Code

All that we have done so far seems reasonable, except possibly the
choice of a random code (although we hope that it has at least been
made plausible by the earlier use of hash coding-Sections 5.11 to 5.14
and much of Chapter 9). It is the sort of thing one would think of in
the normal course of research. But the next idea of Shannon's, that
we should average over all random codes (but what else is there to do?)
is not one of those things that comes to mind easily. Of course, once
the idea is suggested, it is something to try.
     We therefore now average over all codes. We use a wavy line for
the average over all the code books. The code words come from the
urn one at a time (or else are made up bit by bit by the random toss of
a coin) and we chose [equation (10.4-2)1 M = 2n(C 1) words. There
are M symbols of n bits, so there are in all (as we earlier observed)

                                  2nM

possible code books we could use. With the random selection all these
code books are equally likely; namely, each occurs with probability

                                   1
                                  2nM

The average, weighted by this probability, gives the probable error

                                 可
The b is a fixed constant for all the code books and does not depend
on the whole code. Hence when we average over all the codes, equation
(10.4-7) becomes (since all code points a 羊 a』 ： are equivalent on the
average)


                ／노 드 8 + (M - 1)P｛口 E三 S(r)}

                    5 8 + 凡IP{a E S(r)}       （口 羊 a1)           (10.5-1)

     To evaluate P{a E S(r} (a 羊 a1), we fix our attention on any
particular line of the code book, not that of a1. Since the code books
were made up randomly, the encoding of the line we are looking at will
vary uniformly over all the space of sequences of n binary digits. What
is the probability that this point will be in the sphere S(r)? This prob-
 202      Ch. 10 / Shannon's Main Theorem

ability must be the ratio of the volume of the sphere to the total volume.
The total volume is, of course, 2". Let N (r) be the number of points
inside the sphere S(r). Then


                     P{a슬S(r)} = 뿌             （口 羊 巳）           (10.5-2)


       But for our binary symmetric channel, this is

            N (r) = 1 + C(n, 1) + C(n, 2) + . . . + C(n, r)


                  = 2 C(n, k)

Recall that [from (10.4-3)]

                 r= （口 + 62)n        and       Q + E2 ＜二 吉

We can apply the binomial inequality of equation (9.4-6) using Q + s2
= 入） to get

                              N (r) S 2nH(X)

Hence equation (10.5-2) becomes

                  P｛口 E S(r)} 드 2 2[1m11（入）]     （口 羊 口i)        (10.5-3)

Assembling things, we have for equation (10.5-1),

                        ／노 드 6 + M？小- H(X)1                      (10.5-4)

       For a binary symmetric channel, equation (8.5-3), we have

                      C = 1 - H (P) = 1 - H (Q)

Therefore, the exponent in equation (10.5-4) may be written as

            1- H （시 = 1 - H (Q + e2)

                          1 - H (Q) + H (Q) - H (Q + E2)

                          C- 田（Q + C2) 寸 月（Q)1                  (10.5-5)

But the entropy function is convex downward and can be bounded at
                                                        Sec. 10.5 / Average Random Code                          203

 any point Q by fitting a tangent line at Q:



                          H
                                    (Q 『 82)            5月
                                                                          （Q)『 62岩 Q
 where (since 0 드 Qs 글）

           쁘m= log
                      （計吼노）                                                           1og
                                                                                               /1
Therefore, (10.5-5) becomes



             1   -    H
                              (X)
                                      !         C   -        c2     log
                                                                           (1
                                                                                    a Q)   =        C   -   83

where E3 is defined as


                                          小E2
                                                              log
                                                                          ( )
                                                                           '    /
Now (10.5-4) becomes

                                      J노 56 + M2Hn(C_ E3)

From (10.4-2),

                                                    M = 2n(C- et)

and

            PE 5 6 + 2n(C- EI) 2-n(C--E3) = 6 + 2-n(EI_ E3)

Thus as long as we pick e2 small enough so that


                     El- 83 = El - E2 log


then the average error

                                                             可
can be made arbitrarily small by choosing n sufficiently large.
204    Ch. 10 I Shannon's Main Theorem

    We have now shown that the average code meets our requirements;
hence there must be at least one code that does. Thus we have proved
Shannon's result:


     Theorem. There exist codes that are arbitrarily reliable and which
can signal at rates arbitrarily close to the channel capacity of the binary
symmetric channel.

      What do we learn from the proof? We learn that theoretically
suitable codes exist, but we also learn a number of other things. We
see from the use of the central limit theorem that the messages will have
to be so long that we are, on the average, correcting many errors in
each message. We also see that we must send very long messages to
get an efficient code. But long messages require a lot of information
to be gathered before anything can be sent, meaning that in many
circumstances nothing will be sent until enough has been gathered to
do the encoding of all of it. Further, we see that the code book, being
random and with large M, must be very large indeed! There can be
no short description, as there is for the Hamming codes, for instance,
telling how to encode and decode a message-it is random and "ran-
dom" means that no short description is possible.
      We see that it is a theoretical result, not a practical result. Yet
 this does not mean that it is worthless. We see the nature of the problem
 of efficient encoding-we must have long messages and we must correct
 many erroneous bits in each message if we are to make very efficient
 use of the channel. The theorem sets bounds but does not suggest much
 other than that very good codes must be very long, often rather im-
 practical ones.



 10.6 The General Case

 The proof of Shannon's main theorem in the general case goes along
 the lines of the special case of the binary symmetric channel. The
 differences in the proof arise from the question of finding an equivalent
 metric to the Hamming distance (which was appropriate only for a
 channel with white noise). We also have the problem of counting the
 number of possible messages that lie within a "sphere" with the new
 distance function. Finally, we cannot use the simple formula for the
 capacity of the channel but must go back to fundamentals.
      The metric we need is the probability of errors. If the "noise" is
 not white, the spheres become ovals with their longer directions in the
                                                                                                                  Sec. 10.7 / The Fano Bound                                                                               205

directions of the more probable errors, and the shorter in the directions
of the less probable errors.
     Once a suitable metric is found, we pick the "ovals of equal prob-
ability radius" about the received symbols, increase them as before, so
that by the law of large numbers when n is sufficiently large, almost
certainly the original symbol is inside. We choose the number of mes-
sages M so that we are close to capacity. We must also use a sufficiently
large n so there is arbitrarily low probability of an overlap of the ovals.
Other꿔ise, the proof is the same as for the binary symmetric channel.




10.7 The Fano Bound

To prove the converse of Shannon's theorem, that we cannot signal
arbitrarily reliably at a rate higher than the channel capacity C, we need
an important bound due to Fano. For convenience we use the notation

                                             戶E = 2 P（口' , b) = 1 - PE
                                                                   B


where, as before [equation (10.2-5)],

                                                        PE =                                   2                        P(a, b)
                                                                                       且A- 口中



         Consider the expression


    月（PE) + 八log (q -1)
                                                            =
                                                            ：           乙！
                                                                        'E              log   .8              ( ) '-         PE         i\          + 'E             log             (i-           )
                                                                                                                                                                                     )
                                                                                                                                             logt
                                                                                                                                                            "    -



                                                            =           ,                          , ,
                                                                                                                                                                P
                                                                             ,)                               P   (a,         b)
                                                                        B,        A-               a                                                                            i\
                                                                        『믐P(a*, b) log（去，
                                                                                        )                                                                                                                       (10工1)


The equivocation H (A 1 B) from equation (7.5-4) is of a similar form,



3  I :=
H（川5)
    (A     B)    ,
                 B,   ，크   A-   ,a ,   /(.
                                       P     (a,   ,   b)
                                                       6)   1.   log[   8I, (                            ,i             b)    ]
                                                                                                                               + B P
                                                                                                                                   穹2                 (.
                                                                                                                                                      (a*       ', ,       6)
                                                                                                                                                                           b)              1.
                                                                                                                                                                                           log[   8I,  p   (*    i   lb)     ]
206     Ch. 10 / Shannon's Main Theorem

Subtracting equation (10.7-1) from this, we get

H (A I B) - H (PE) - PElog (q - 1)


 = ,B,A
    ，具-a',,「（.,
            P(ab)log
                6)1.8[(, -，仁
                          i)p(, 1m)1
                                  )j                            +무
                                                                                   P
                                                                                        (a
                                                                                                 ',   b)
                                                                                                            log
                                                                                                                   [P
                                                                                                                        (c;
                                                                                                                                  b)
                                                                                                                                       ]
It is difficult to apply the Gibbs inequality here, so we go back to basics.
To apply the inequality

                                                    loge工 5 X 卞 1

we must convert this inequality to log2 by writing it as

                                                    lo只工
                                                    H=1 < 工 -   1
                                                    tog e


Apply this to each sum. The 1/log e will factor out of each term on the
right-hand side. Ignoring the log factor, we get for the right-hand side,



 ! ,，具-a',,P(a,b)1(L(q, -出1)P(a, 나）
                                                                                                                                  l
                                  b) j
                                     1l+무P(a
                                        B *,b)I,
                                              LP(a*'E b)
        =,트
          ， ,.?,, p(b)－八『戶후p(b)－瓦
                ／노
        =   q
                '    -   1
                             (q
                                  -   1)
                                           푸p
                                                B    (b)
                                                           + 1E>
                                                               B     ..   P
                                                                              (1
                                                                                   ')
                                                                                             -        (PE
                                                                                                                  + PE)
        =PE+ PE- (PE+ PE) =O

Hence we have the important Fano inequality

                         H (A I B) 드 H (PE) + J E log (q - 1)                                                                 (10.7-2)

    Note first that we have not used any decision rule, although the
results depend on it. Second, when do we have equality? Equality
occurs when

                                                loge x = 工 -1

namely when x = 1. This corresponds, since we used it in both sum-
                   Sec. 10.8 I The Converse of Shannon's Theorem      207

mations, to both


              P（이b) = , 尸E-1          for all b and 口 半 口永

and

                   P（口木 1 b) = 1- ／노         for all b

The second, however, is included in the first, since

                      2P(a 1 b) = 1        的r all b



10.8 T九e Converse of S九annon농 T九eore刃1

To prove the converse of Shannon's theorem, we use Fano's inequality
of equation (10.7-2). We want to prove that the probability of error
cannot be kept arbitrarily small if we exceed the channel capacity. That
is, we cannot make

                       M = 2n(C+ E)      (s > 0)

for M equally probable original messages. Suppose we try. Then for
the nth extension of the alphabet, we have that the change in the entropy

                        H (A ") - H (A " 1 B")

is less than or equal to nC (the channel capacity measured in blocks of
n symbols is defined as the upper bound). But p = 1/M, so


                    叩卜 2 加gM
                             = log M = n(C + e)

We have

                     H (A ") - H (A " 1 B") 5 nC

Rearranging, we have

                n(C + E) 卜 nC = ne 드 H (A " 1 伊）
208    Ch. 10 / Shannon's Main Theorem

Applying Fano's result (10.7-2), we obtain

            nE s H (A " I B") 드 H (PE) + PE log (q - 1)

Now H (PE) 드 1 (from Section 8.5), so using q - 1 <q = M, we have

                            nE s 1 + PE(nC + nr)

or

                                nr - 1
                                         드
                                             /JE
                               nC + ne

We can therefore write

                ,,
                fJ n   >
                            ns - 1 ? r- l ln        E
                                             HH

                =乙         nC+ nE     C+ r         C+ r

which is independent of n. As n -p m, PE is bounded away from 0.
Hence the error cannot be made to vanish if the rate exceeds the channel
capacity.
     As an illustration, suppose that we tried to send at a rate of twice
the channel capacity. If we sent every other bit through the channel,
we could get them through arbitrarily reliably. For the missing bits,
the receiver tosses a coin and is right half the time; thus almost three-
fourths of the message is correct and one-fourth erroneous.
（沇a까cr11



                       Algebra元 Codi兀gT九e이y




11.1 Introduction

Shannon's main theorem, which used very long block codes, shows that
we can signal at a rate arbitrarily close to the maximum rate and with
arbitrarily few errors. The proof is based on random encodings which
use very long blocks, and in any one of the long words there will probably
be many errors to be corrected at the receiver, which means that to be
efficient we must work at high error-correction rates. In Chapter 3 we
showed how to design single-error-correcting codes as well as double-
error-detecting codes. The theory of multiple-error-correcting codes is
very elaborate, so we merely sketch the main ideas involved in how to
design and implement some multiple-error-correcting codes.
      The idea of a random code is appealing until you think about the
terminal equipment. If the code words are long, then the encoding
book must be very large, since by definition "random" means that there
is no pattern and each encoding must be looked up because there can
be no formula for computing the encoded message from the source
information as there are for regular codes. The decoding book must
be even larger, since although only M selected sequences can be sent,
every one of the 27i possible sequences of n bits (in a binary channel)
must have an entry for decoding the received message. Otherwise, we
must do a very large amount of computing to find the proper message
 to associate with the received message. Thus, in practice, large random
codes are hopeless. (But remember the discussion of hash coding in
 Sections 5.11 to 5.14.)



                                                                      209
  210     Ch. 11 / Algebraic Coding Theory

        We have, therefore, to look for highly structured codes,
                                                                     and to do
   this we need the theory of the algebra of finite fields (Galoi
                                                                      s fields).
   As noted above, the topic of algebraic codes
                                                   is vast, and we can only
   touch the surface to indicate some of the ideas involv
                                                            ed in the higher-
   error-correcting codes. This is not a book for expert
                                                             s who are going
   to design coding systems ideally fitted to complex situati
                                                                ons; the book
  was organized for those who need some acquaintance
                                                            with what can be
  done, and hopefully if a situation arises that requires
                                                            more theory the
  reader will at least recognize the possibilities and go
                                                            to other sources
  for more details (e.g., Refs. [Bi], [B3], [B4], [C], [G], [Gu],
                                                                   [Li], [L2],
  [MS], [Mc], [P], [PW], [V], [W], [WJ]). Howe
                                                       ver, it is only fair to
  warn the reader that in practice we seldom know the noise
                                                                  well enough
  to justify using many of the more elaborate codes that have
                                                                     been de-
 veloped (and usually based on pure white noise). Occas
                                                               ionally, we do.
       We will emphasize binary block codes, both because they
                                                                     are most
 widely used, and because the base r codes are somew
                                                               hat messier in
 notation, although the ideas needed are usually not
                                                         significantly differ-
 ent. We also deliberately review the Hamming codes
                                                             of Chapter 3 so
 that you will remember them this time! You will see
                                                              them in a very
 different light.


11.2 Error-Detecting Parity Codes Revisited

The single-error-detecting parity codes of Section 2.2
                                                       used a single parity
check over all the positions. If we write a 1 for each
                                                          position that is
checked and a 0 otherwise, we get the matrix (in this
                                                          case the trivial
m )< in姐tn지

                          M= (1, 1, i, . . . ,i)

This matrix says that the parity check involves every
                                                      position.
     Consider an encoded symbol which is now labeled c;
                                                           it is a vector
of n binary digits, say,

                           c= (0, i, 0, . . . ,1)

Let the transpose of c, written cT, be the corres
                                                  ponding column vector.
We have (using mod 2 arithmetic, of course) the matrix
                                                            product

                                 McT = 0                             (11.2-1)
for every encoded word to be sent. It is important
                                                    to see why this is
so. When inspected, equation (11.2-i) is simply a
                                                   statement of what
                                                         Sec. 11.3 / Hamming Codes Revisited            211

the parity check is. The 1 digits in the matrix M select the positions of
c that enter into the parity check.
     Suppose next that a single error is made in sending the code symbol
c. The error changes one binary digit. Recalling that we do our arith-
metic modulo 2, the received word is

                                                                 c+ e

where e is the error vector with all 0's except a 1 in the position of the
error.
    Consider, finally, the expression (using mod 2 arithmetic)

        M(c + e)T = McT + MeT
                                                 = MeT 羊 0           (syndrome for a single error)

The syndrome of the erroneous message (the result of applying the parity
checks) in this case is a 1 whenever there is an odd number of errors
and a 0 whenever there is an even number of errors, including no errors.


끄．3 月ram,砒ng Codes Revisited

In Section 3.4 we examined a special case of single-error-correcting
codes. These Hamming codes used the parity checks

                                         d
                                         l
                                     ／
                                     八
                                                 1, 3, 5, 7, 9, 11, 13, 15, .
                                                 2, 3, 6, 7, 10, 11, 14, 15, .
                                         e 그
                                           1
                                           V 4
                                             1
                                                 4, 5, 6, 7, 12, 13, 14, 15, .
                                                 8, 9, 10, 11, 12, 13, 14, 15, .              .
                                                 etc.

In the further special case of n = 7, we write the matrix

                                                                          \
                                                  l0
                                         0   0       l
                                                     1

                                                             1 月
                                                             m
                                                             1 l 0
                                 /
        M                                 l1
                                           d        00
                             1
                                                  上
                                                  1
                                                  d
                         1
            l
            ]
                                                                     l.
                                                                              H毗
                                                                                   帥ycheck,
                                         00       0ll                I J f- seconu parity cHecK
                     1
                                                                     1/ e11iirst parity cnec1(
                 1
             \
                                     \




where we have put the parity checks in sequence from the bottom up.
Each position in any parity check has a 1 in the corresponding row of
the matr奴．
    Again let c be a code word. We again have for all code words,

                                                          McT = 0                                 (11.3-1)
212    Ch. 11 / Algebraic Coding Theory

since this is the definition of an encoded word. In technical jargon the
matrix M annihilates every properly encoded word c. A single error e
will change the original message I sent to the received message you get.
It will now be
                                  c+ e
and we will have again

                 M(c + e)T = MCT + MeT
                               = MeT = the syndrome                      (11.3-2)

Thus the syndrome of the error depends on the error and not on the
code word sent. The syndrome is the column where the error occurs.
Thus the columns of the parity-check matrix M are all the syndromes
that can appear for any single error.
     To generalize for any parity-check code, we can write a parity-
check matrix M which has l 's in the places of each row where the
corresponding parity check is applied and 0's where the parity check
does not apply. We 口Ssume that the rank of this parity-check matrix
M is equal to the number of rows in the matrix (using, of course, modulo
2 arithmetic). For example, the matrix (compare Section 3.4)

                                  l 0 4l
                                  1

                                           m1l 0 ]1   Jl ml 0      l 0
                                                                1l 4
                                                                     \
                                                                     \
                           M
                                                                     1
                                 //111\
                                                                     1
                                                                     1
                                                                                11

                                                                     J
                                                                     r
                                 \
                                                                     /
has only rank 2, since if the bottom two checks are satisfied, the upper
one is also satisfied. (The sum of all three rows is 0 0 0 0.) If the
rows are not linearly independent, then at least one syndrome digit is
determined from the others, and we are not going to get all the different
syndromes we want-we will waste signaling capacity.
     The encoding process in the general parity-check case assures us
that
                                McT = 0

for all legitimate code words. Thus once more, the error e gives rise
to the received message c + e and

                   M(c + e)T = MeT = syndrome

The syndrome again depends only on the error and is the corresponding
column of the matrix.
    If there is a single error, then you have the following decoding rule:
The syndrome is exactly the corresponding column of the parity check
                Sec. 11.4 / Double-Error-Detecting Codes Revisited   213

 matrix. Therefore, by comparing the syndrome with the columns of
 the matrix until you find a match, you can locate the position of the
 error.
      Thus you see that for any single-error-correcting code, given any
 syndrome you can find the corresponding column of the check matrix
M (the syndrome "all zeros" means no error).
      If we are to have multiple-error-correcting codes, then the syn-
 drome is exactly the sum (modulo 2) of the correcting codes' columns
 of the matrix corresponding to the error positions. This correspondence
must be unique if you are to find the proper columns of the matrix and
hence the corresponding multiple errors that induced the syndrome. If
a syndrome does occur, and it is not the sum of the permitted number
of columns, then there is nothing you can do to correct the errors that
have occurred. You can only detect the presence of some errors.
      To be specific, in a double-error-correcting code any possible syn-
drome that can arise from two errors must be the sum of a unique pair
of columns of the matrix-there cannot be two different pairs of columns
leading to the same syndrome, since if there were, you would have no
way of knowing which pair of errors gave rise to the observed syn-
drome. Nor can a sum of any two columns be some other single col-
umn. In symbols you have

              M(e1 + e2)T = Mer + Mef = syndrome

and the syndrome must be unique for every pair of errors e1 and e2, as
well as for every single error (and cannot be all 0's, since that means
no error).
    The same sort of argument applies to higher error-correcting codes.


月工erc加e

11.3-1 Discuss the problem of triple-error-correcting code design.



11.4 Double．
           月rror-l厄ect加g Codes Rev打社ed

For the double-error-detecting code of Section 3.7, we have the matrix
(for n = 8) where we have added the overall parity check as the top
row of the matrix,




                             1 0 l
                                   0
                                            月l   0    l
                                         l
                                         4     l
                                               1
                                           4l 0

                             工
                                                     4 l l
                                        l
                                        d        l
                                                 d


                                 d
                                        4l     0 0

                                                     工
                                                     1
                 M=
                                           l
                                           4
                                       dl 0
                                               4 l
                                               l m
                                                             三）
                        （三
214    Ch. 11 / Algebraic Coding Theory

Any syndrome with the first component equal to 1 must have the rest
of the components as the syndrome of a single error, with the syndrome
all 0's meaning that the additional parity check position is wrong (see
last column of the matrix M). If the first component of the syndrome
is 0, there is either zero or some other even number, 2, 4, 6, 8, . . . ,
of errors. In the first case the message is correct, and in the second
case you do not know what to do since the syndrome is not a column
of the matrix M. You can merely note the presence of an even number
of errors for this code.



11.5 肋｛yn｛刀ni口加 Versus Vectors

Originally (as we did in Chapters 2, 3, and 10) the code sequences of
0's and l 's were regarded as vectors. The significant step forward occurs
when this view is replaced by the view that they are polynomials-the
digits of the code word are to be regarded as the coefficients of the
powers of the variable (indeterminate) x. Thus the sequence

                           1,   0,   1, 1,   0

is now to be viewed as the polynomial

                         /\（功 = 工4 + 工2 + 工

In a sense we are using a generator function representation of the code
sequence of 0's and l 's.
     Another example is the sequence 0, 1, 1, 0, 1, which corresponds
to the polynomial

                         P2(x) = x3 + x2 + 1

     The set of all polynomials of a given degree with integer coefficients
permits addition and subtraction (which in our case of modulo 2 arith-
metic are the same thing!) of any two of them. For example, using the
two polynomials above, P1(x) + P2(x) = x4 + x3 + x + 1. Addition
is associative, (P1 + P2) + P3 = P1 + (P2 + P3). The zero element
(0, 0, 0, 0, 0) corresponds to the zero polynomial and is identically
zero. Since each nonzero polynomial is its own additive inverse, and
the sum of any two polynomials is another polynomial of the same degree
(at most), it follows that the set of all polynomials of degree n forms a
group. Remember that the coefficients of the polynomials can be only
0 or 1.
                                   Sec. 11.6 / Prime Polynomials     215

     In Section 2.8 we examined modular arithmetic. One of the pur-
poses of modular arithmetic is to be sure that all the numbers that can
arise will fall within the given range of numbers. This is accomplished
in modular arithmetic by dividing all numbers by the modulus m and
using only the m positive remainders 0, 1, . . . ,(m - 1), which are all
less than the modulus.
      When we face the class of polynomials we find that the product of
two polynomials has the degree that is the sum of the degrees of the
individual polynomials. To keep the product within the maximum de-
gree less than n (so that the polynomial will be identifiable with a code
sequence), we must similarly reduce the degree. Thus we need a poly-
nomial to use as a modulus. Just as with modular arithmetic where we
divide all numbers by the modulus and identify the remainder as the
number, so we will now divide all polynomials by the modulus poly-
nomial of degree n and use the remainder as the product. As a result,
the remainder will have n coefficients (the degree is n - 1), which we
can then identify as a code symbol.
      We saw in Section 2.8 why we want a prime number as our mod-
ulus. For a prime modulus, if the product of two numbers is zero, then
at least one of the two numbers is zero. If the modulus is not a prime,
it is possible that neither number is zero, although their product is.
Similarly, we want a prime polynomial as our modulus-a prime poly-
nomial being one that cannot be represented as the product (in the field
of coefficients) of two nontrivial polynomials.
      A polynomial of degree n might by chance have its coefficient of
the highest power 0 so that the polynomial was really of lower degree.
Since we have only 0 and 1 in the field of coefficients, we will use the
standard words monic polynomial to mean a polynomial whose coeffi-
cient of the highest power of x is i.
      But the reader may well ask: Why do we want to multiply poly-
nomials together? The answer is simply that we want to introduce as
much structure into our theory as we can. Then, and only then, will
the codes we finally get be highly structured, and as a result we can
hope that the encoding and decoding equipment will also be highly
structured (meaning easy to build in hardware or to program in soft-
ware). In practice, we simply do not want to face random, or even
lightly structured codes.


11.6 Prime Polynomials

A prime polynomial is a monic polynomial that cannot be factored into
a product of lower-order polynomials. But since our field of coefficients
uses arithmetic modulo 2, we cannot be sure of how old familiar results
216     C九 끄 / Algebr口ic Coding Theory

will now appear. Thus we will experimentally explore what can hap-
pen- we will avoid going into all the technical details of finite fields to
prove how factorization must occur.
     For polynomials of degree zero there is only the single, trivial poly-
nomial (if you care to call this degenerate case a polynomial), namely

                                  尸 == 1

It corresponds in normal arithmetic to the number 1.
     For monic polynomials of degree 1 there are only two polynomials,

                                    工
                                  工 + 1

both of which are prime polynomials (just as we disregard the use of 1
as a factor in factoring integers, we disregard the trivial polynomial 1
as a factor).
     For monic polynomials of degree 2 we have four possibilities (each
of the coefficients of x. and 1 may be 0 or 1):

                    工2            =   工 · 工


                    工2 + 1        = （工 + 1)（工 + 1)
                    工2 +   工      =   工   （工   + 1)
                     x2 + x + 1 = prime

The fact that

                            x2 + 1 = (x + 1)2

may come as a surprise at first, but multiplying out the right-hand side,
we get

                               x2 + 2x + 1

Since 2 = 0 (mod 2), we have

                          工2 + 2工 + 1 == 工2 + 1

      Is the polynomial

                               工2 +   工 +      1
                                                 Sec. 11.6 / Prime Polynomials                   217

a prime? Are you sure? We try dividing by the two lower-degree
polynomials. If x2 + x + 1 is composite, these are the only possible
factors. Clearly, x is not a factor. We then try

                                          0                 工
                     工 + i     i 工2 + 工 + 1
                                   工2        +              工

                                                            00
                                                                          4
                                                                          l 0 dl
                                                                                   = remainder

Yes, x2 + x + 1 is a prime polynomial.
    For further practice we examine the eight possible cubics

                                                        =       工 1工 ' 工




                        工                               = 工（尸 + 1)
                        工 +   1

                                                        = 尸（工 + 1)


                                                        =       工
                                                                    （工2
                                                                             +      工 + 1)

                 工3 +   工2 + 工 +             1 =


where we have given the four obvious factorizations, and left the others
blank.
    If a cubic can be factored, then one factor must be of first degree.
We have given those divisible by x, so we need only try to factor x + 1.
We have forx3 + 1,


                                             l 0            ll
                                   l上 0 ml
                                             4
                              ll
                  1 1




                                             0 ml l l
                                   l 1l

                                                            l
                                                        1
                                                        0 = remainder
218     C/i. 11 / Algebraic Coding Theory

Hence

                     （工 + 1)（尸 + x + 1) = 工3 + 1

You can check this by multiplying out the product.
   Next we try 工3 + 工 + 1:
                                           0

                                  d
                                  l 0 dl
                                            lm

                            ll
                                           ll
                     1 1


                                  ll

                                           ll 00   ll 0

                                                   li
                                                          = remainder

We see that x3 + x + 1 is prime. Similarly, x3 + x2 + 1 is prime,
since by observation

                     工3 + 工2 + 1 = 工 · x（工 + 1) + 1

      Last, we try

                           工3 +        工2 +         工 +           1


From the experience above we now see how to factor directly. Thus
we ＼入／
     rite

         尸（工 + 1) + （工 + 1) = （尸 + 1)(x + 1) = （工 + 1)3

and it is not a prime.
    We have, therefore,

                              工3 + 工 +                    1
                              x3 + x2 +                       1


as the only two prime monic polynomials of degree 3.
     We shall not go on finding the prime polynomials of higher and
higher degrees. Evidently, for each particular polynomial we need only
try lower-order prime polynomials up to half the degree of the given
polynomial, and we are beginning to see how to do some of the fac-
torizations in our head (see also Exercise 11.6-1). In any case, we are
                                         Sec. 11. 7 / Primitive Roots   219

not trying to show how to make the best codes but are content to show
F山＼vc아如g theory dev아아）s toward 뇨gher error-correcting codes which
have a good deal of structure in them, so that the terminal gear is
practical to build in software or hardware.
     The idea behind the proof that there are always prime polynomials
of every degree goes as follows. We know that there are 21 distinct
polynomials of degree n. Given how many prime polynomials there
are of each lower degree, we can compute how many distinct products
of degree n we can form. The difference between these two numbers
is the number of prime polynomials of degree n there must be. By
suitable bounds on each number we can obtain a bound on the next
number.


Exercises

11.6-1 Prove the theorem: If and only if the sum of the coefficients of
       a polynomial = 0 (mod 2), then x + 1 is a factor.

11.6-2 Carry out the factorization of polynomials of degree 4.

11.6-3 Carry out the factorization of polynomials of degree 5.


11.7 Primitive Roots

We need to make one more digression before returning to error-
correcting codes. In normal algebra, the nth roots of unity are the roots
of x' 卜 1 = 0. Their explicit form is given by

                 e2TtICI12
                             (k= O, 1, 2, . . . ,n-     1)

Note that (e2 1kIn1)Pt = cos 21Tk + i sin 2'Trk = 1 and hence they are all
roots of unity.
     Some of these roots, for example k = 1, are such that their suc-
cessive powers generate all the other roots. Indeed, if k is relatively
prime to n, this will happen. To prove this result, take the successive
powers, m = 1, 2, . . . , n - 1, n, of this root:

                                  e2竹ik/n



These mth powers are
                                 e2nu/cm/ri
220    Ch. 11 / Algebraic Coding Theory

If any two of these were equal, then we would have

                               e2丁了ikmi/n == e2町ikm2/n


or

                               e2町uJc(m1_ m2)h7 =                        1


This means that

                     k   (m1    卞    m2)     H       ,     八nm           ;n   . 八nn.
                                             -           fl jllfl,       111L175드1
                               n


Since k is relatively prime to n, this means that they have no factors in
common and n must divide m1 - m2. However, m1 - m2 is less than
n, so m1 = m2. Therefore, if k is relatively prime to n, the successive
powers of that root generate all the roots of unity and it is a primitive
root.
     The reason that primitive roots are important is that a primitive
root can serve as a generator of the whole set of numbers we need.
However, we must examine the problem in our modulus 2 arithmetic.


11.8 A Special Case

The perfect Hamming codes have n = 2力i - 1 digits. For the case n
= 7 = 23 - 1, we have the matrix (Section 11.3)


                                   凡kh                                                 n니V
                                         0       0               0   上
                                                                     1
                                                                     d
                                                            l
                                                            4 l1
                     M                工
                                      1
                                      d  l
                                         d l
                                           d                   0
                                                                 l
                                                                 4                           (11.8-1)
                                           0                1l 0 0



We know that any rearrangement of the columns of the matrix M will
not fundamentally change the code; it will only affect how and where
we find the column corresponding to the syndrome that emerges when
a single error occurs.
     To illustrate the new approach, suppose that we use the prime
polynomial

                                     工3 + 工 + 1

as our modulus. Let a be a root of this polynomial. Thus

                                    口3 + 口 + 1 = 0
                                                                                  Sec. 11.8 / A Special C口se   221

or


                                                                                a+ 1


This means that the powers of a which are 3 or higher can be reduced,
using this equation, to sums of lower powers. Thus every polynomial
in a can be reduced to a linear combination of 1, a, and a2. Now
consider a column 3-vector which has components 1, a, a2 from the
bottom up. The column vector gives the coefficients of the correspond-
ing power of a. Note that multiplication by a shifts each component
up one position, and that a3 = a + 1 is used whenever a3 occurs, so
that only 1, a, and a2 appear in the vector. For the various powers of
a we have the corresponding 3-vectors



                                      \
                           (o\
                  1= (0j
                                \1I
                          (0\
                  口 =     Ill
                           \0/
                          (i\
              口"      =   (01
                            \0/
             口" = 口 + 1 = (1)
                                                   fo\
                           1                             \l/
              口4      =   a2 + 口 =




                                                                                               )
                                                                (1
                                                                      \0   三）
              a5          a3 +            a2                               a2 + a
                      =
                                               =
                                                                                  + 1=    (!
                                                                                               1
                                          1)
              a6 = a3 + a2 + a = a2 + 1= 10
                                                                                          \1
                                  -                             /0\
              a
                  '   =   口" + 口 =                             (0J
                                                                     \l/
                                                                           1
222     Ch. 11 / Algebraic Coding Theory

as we should. Thus we have shown that a is a primitive root of the
prime polynomial, since its successive powers generate all seven possible
different nonzero 3-tuples.
     If we write the columns of this new matrix in the form (for con-
venience we are reversing the order of the columns),


                                                             n 0 41l 0
                            6
                                           口 0 ]1
                            口      口   <
                                       U           n4U   口                4l
                                                         l
                                                         d
                            0                      l
                                                   4
                                                                              /

                                   d
                                   l d
                                     l l
                                       1
                                                                               \
                               \
                                           4
                         l
                         m
                        / r 1 \l
                               1                         00  2           0 0 l
                                                                               1
                                           n dl 1l 0
                                                                             月
                                                                               1
                                                                               /
we find that this is merely the matrix M (11.8-1) rearranged. In this
new arrangement of the columns you compare the syndrome you corn-
pute at the receiving end with the successive powers of a (which you
can either store or generate as needed). When you get a match between
the syndrome and a column, you have that column as the corresponding
power of a that matches. (A slightly different, but equivalent, decoding
matrix would result if we used the prime polynomial x3 + x2 + 1.)
     How do I encode? Since we want the syndrome 0, 0, . . . 0 to
mean no error, I must require that the sent polynomial be exactly div-
isible by the modulus polynomial x3 + x + 1. Thus I put the message
in the positions corresponding to a6, a5, a4, a3, and temporarily put
zeros in the other three positions corresponding to a2, a, and 1. When
I divide this polynomial by the modulus polynomial, I will get a re-
mainder. If this remainder is put into the last three positions of the
polynomial I wrote (or if you wish is added to the polynomial), then
the result will be exactly divisible by the modulus polynomial. This,
then, is the encoding process-supply the last three positions by using
the remainder upon division by the modulus polynomial; thus the whole
polynomial is equal to zero modulo the prime polynomial.
      To decode at the receiving end, you simply divide the received
polynomial by the modulus polynomial. The syndrome (remainder)
 that results when it is written as a power of a gives the column where
 the error occurred. We now have a different way of viewing the earlier
 Hamming codes. This approach is suggestive of what to do next.

      Example of Encoding. Given the code above, I encode the message

                         1 0               0 1 -                 尸

as follows. The message corresponds to the polynomial

                                           a6 + 口3
                                                 Sec. 11.8 / A Special C口Se         223

I divide this polynomial by the modulus polynomial x3 + x + 1 to get
the remainder.

                                                     00            00
                                l     00 00 00
                                                             l
                                                             4


                          ll
                                                               0
          1 0    1 1
                                 1]lJ

                                                     0 0 0
                                  0     0
                                   ldl4   l
                                          ml1
                                                               0


                                                 l
                                                 4 l
                                                   =         ] l
                                                             1 4
                                  00 00
                                                                   00 0
                                                     0         0
                                                 l
                                                 d           l
                                                             1
                                                                      = remainder

Therefore, the encoded message is

                        (1 0           0   1 1 1 0)

and the message polynomial is divisible by the modulus polynomial x3
+ 工 + 1.
     Suppose that there is an error at the underlined place (which is the
a3 place) so that the received message is

                        (1 0           0   0 1 1 0)

You divide the received message by the same modulus polynomial as I
used to encode the message as follows:


                                           l0l
                                                 0           1 1



                               00 00
                                       0         l
                                                             1 0

                                   l
                                   1 l
                                     d     l
                                           J   l
                                               J
                                       0   0     0


                                   l
                                   d l
                                     d                  l
                                                        d l
                                                          1
                                           1
                                           l
                                           ] 上
                                           1 j
                                             0


                                           ll
                                                 0
                                                   4 l
                                                   l d
                                                 0   l
                                                   l
                                                   4
                                                 0 0 0
                                                                   尸H今 remainder

But this remainder is
224    Ch. 11 / Algebraic Coding Theory

This is the fourth position from the right (which is where the error
occurred). You add a 1 in this fourth position to get the corrected
message, and then drop the last three places to get the original message.


Exercises

11.8-1 Find the decoding matrix for the prime polynomial x3 + x2
       + 1.

11.8-2 Repeat the encoding and decoding of the example for the mes-
       sage 1 0 1 0 and an error in the a2 position.

11.8-3 Find the decoding matrix for x4 + x + 1.

11.8-4 Find the decoding matrix for x4 + x3 + 1.

11.8-5 Show that the syndrome for two errors is the sum of the separate
       syndromes.


11.9 訊恥 Regis比rsfor Enc야在ng

We have developed the theory of algebraic codes in terms of these codes
because they are easy to realize in either hardware or software. The
apparent complexity of much of the previous division process for the
modular reduction of polynomials can be handled simply by means of
shift registers with feedback paths. Suppose that we have the 7-bit poly-
nomial code of Section 11.8, and I want to encode the message 1 0 0 1.
The encoded message will be a polynomial of the form

            1 .工6 + 0. 工5 + 0.工4 + 1 . 工3 +   非工2 +    水工 +   非1


(where * indicates the coefficient to be determined) and is to be divisible
by the modulus polynomial x3 + x + 1 (the one we used in Section
11.8).
    I will first set the three unknown coefficients equal to zero and, as
before, divide by the modulus polynomial to get the remainder. When
I add the remainder a2 + a to the original message polynomial a6 + a3,
I will have the encoded message

             口6 + 口3 + 口2 + 口 =      （口3   + 口 + 1)   (a3 + 口）
and this, as shown, is exactly divisible by the modulus polynomial a3 +
a + 1.
                               Sec. 11.9 I Shift Registers for Encoding                225

   Encode



                                                                             0. 0. 0




             Feedback paths

                 Figure 11.9-1 Shift register with feedback

      How can I do the division process in practice? Imagine the shift
 register in Figure 11.9-1. The digits of the message are imagined to
 come from the right, the highest power first, with three trailing zeros
 automatically supplied. The arrows below the register positions show
 where the "feedback" occurs. The feedback paths are determined by
 the modulus polynomial. When there is a 1 in the highest position, it
 is then added to (subtracted from) the indicated positions. We can
 follow the details in Figure 11.9-2, where we have omitted the early


                                                                        寸H
               State                                                   0 0 0
               Feedback                                                0 0 0
               Result                                                  0 0 0
Shift                                                              =   出 口 =   =   =   =   =




Sh淑




Shift




                        Figure 11.9-2 Numerical details
      226          C九 끄 / 川gebr口ic Coding 了heory

      stages, since nothing of interest has happened during the first four shifts
      until the leading digit gets to the left-hand position. The diagram starts
      there at the top line. The next line shows the digit fed back and the
      third row (just above the double line) shows the result of the addition.
      (We show the adding of 1 in the left position to match the division
      process in detail; it is not fed back in practice.) The shift occurs at the
      double line, and we next see the shifted digits. The set of three lines
      between the double lines gives the details before the next shift. In total
      there are, in this case, four sets of three lines. The end result is the
      remainder. A comparison will show how the shift register does the
      same thing as the division process.
            Figure 11.9-3 shows a practical encoder. The digits of the message
      still come from the right, but now they also go out on the left through
      the dotted switch. When the remainder is computed, I have all the
      original message digits sent out and I then change the position of the
      switch so that I can now shift out the remainder to form the entire coded
      message (omitting the first digit, which is, of course, always zero). The
      encoding is that simple!


                                  /)4
      Out
p1H         ＜二
                  \\
                 Switch
                                             '
                                                                                   0. 0. 0
                              '
                          \             出,
                                                 Figure 11.9-3 Encoder


           Shift registers are not hard to build in practice, even with the ad-
      ditional ability to logically add (exclusive OR) in each position. The
      rest is similarly easy to build in hardware.
           In software it is also not difficult to program. I test for the 1 in
      the left position and jf I find it, I logically add the pattern of l 's required
      by the feedback paths (the modulus polynomial). Then I shift and
      repeat. The details are not difficult to supply.
           Thus the encoding for this code is fairly simple. We next turn to
      the decoding process.
                Sec. 11.10 / Decoding Single-Error-Correcting Codes
                                                                         227

 Exercises

 11.9-1 Write a program to encode a message following the
                                                          model in
        this section.

 11.9-2 Draw a schematic of a shift register x4 + x3 +
                                                                1.




 11.10 Decoding Single-Error-Correcting Codes

 At the receiving end you do the same as at the encod
                                                            ing end, except
 that you also have to store the message so that you can make
                                                                the needed
corrections when they occur.
      After the division process you have the remainder中the
                                                                 syndrome
of the error. The all-zero remainder means "the messa
                                                          ge is correct and
therefore send on the first 4 bits."
     If the remainder is not zero, it is some power
                                                      of a, say ak. How
can you find which power? A table lookup might
                                                     be appropriate for a
reasonably short code, but for a very complex one
                                                       this might require
too much storage [although the price of storage is curren
                                                          tly (1985) falling
very rapidly].
     Looking back at Section 11.8 you see that a7 = 1; hence
                                                                      a6 =
1/a. You can compute from the syndrome (remainder), which
                                                                    is a':

                                  ak_ i
                 (a6)
                        a"   =                modulo （口3 + 口 + 1)
              (a今口k- i = 口k口




until you recognize 0 0 1 = 1 as the remainder. You then
                                                             know k.
     For example, suppose that I had the message of Section 11.9,


                                 1 0      0 1 1 1 0

and an error occurred in the a2 term. Thus you receiv
                                                      e

                             1 0          0   1 0 1 0
228    C九 끄 / 川gebraic Coding Theory

The division process will go as follows (simplified):

                         0 1l
                 1 0            1 0 1 0
                                l
                                m
                 1 0

                                00   0 l   4l l
                         Jl
                        l
                        d

                                     l
                                     m      0      0
                                                       -p        remainder

Therefore, you start with this remainder, which is some unknown power
of a, say the kth.




Multiply by a6 = 1/a. This is equivalent to shifting each component
down one position. When a 1 is shifted out the bottom, you use 1/a
1 + a2. Thus you have

                                                            fo
                            口6口k =         ak_ i       =    (1
until a0 = 1 is recognized:


                       a6口k- i           口k- 2

                                                   =   （小
In this case k = 2- you need to add a 1 in the a2 position.
     If you shifted out backwards you could use the powers of a as a
test, and when the match occurred add 1 to the digit being shifted out.
     You could also start with the highest power of a and compute down
until you get a match. In this case you could shift out forwards.
     Notice that in software this needs to be done only if there is an
error-otherwise nothing need be done beyond getting the syndrome
and testing it for all 0's. In real-time coding systems, you must have
the capacity to do the computing whether or not it is used.


11.11 A I가冗able万rror-Con四ci加g Code

To partially illustrate a double-error-correcting code, we need to go to
a higher Hamming code with four parity checks and 15 total positions.
                                       Sec. 11.11 / A Double-Error-Correcting Code                                                      229

We examine the polynomial

                                                           x4 + x + 1

as a possible candidate for the modulus polynomial. Clearly, x is not
a factor of the polynomial. If the polynomial is to be divisible by x + 1,
the sum of the coefficients must be 0 (by Exercise 11.6-1, a small mod-
ification of the old factoring rule still applies here). We have, therefore,
only to try as the factor the single irreducible quadratic x2 + x + 1 to
find that we have a prime polynomial.
     Next, we need to test to see if it meets the primitive condition.
We compute the successive powers of a:




                                                                   1｛
                                                                                        三）
                                                                                   /0
                                                                              10
                                                                                        。
                                                               a
                                                                         =    I
                                                                                   \i
                                                                                   /0
                                                           a2           =    11\
                                                                                        。




We find that a15 = 1, as it should, and no earlier power equals 1. Thus
it is a primitive polynomial and we have the parity-check matrix:

                                                                                                                              0 0 0
                                       l



                                                                                                                  n 00
                                       l                                                                               4
                                                                                                                            口
                                                                                                            口 0
                                       口                                                                        <
                                                                                                                J                 m
                                                                                                                                  乙
         口14 口13 口12                                                                                                        m4U


                                                                                                                            l
                                                                                                                            1
                                                    口10 口9 口8 口7 口6
                                                                                                                                    l
                                                                                                                                    1
                                                                                                                                    4




                                llll                0lll
                                                           上
                                                           1            l0                                              4
                                                                                                                        ]   q 0 0   0

          dl 0 0

                   dl 1l 0 1l          1l dl 1l 0                                            d1上 ml 0 0
                                                                                                                                  l
                                                                                                                                  1
                                                                           l
                                                                           dl4

                                                                                                                      l1l
                                                                                                                        1
                                                           0
                                                                                                          l
                                                                                                          d 1
                                                                                                            ]
                                                                                                                            口 0   0 0
                                                           l
                                                           d            0 l0                                                    l
                                                                                                                                4
        4
        1
        l                                                  0                 l
                                                                             a                              0                   0 0 0


    If we want to correct more errors than this single-error-correcting
code does, then we must add more rows to the matrix. We will add
four more rows, but how?
 230      Ch. 11 / Algebraic Coding Theory

     At present, two different double errors can produce the same result
for the syndrome, that is,

                               a" + 口m = 口k ' + am'


For example, columns a and a2 give the same syndrome as columns a12
and a14. We need more rows. How about using the square of a as a
generator? Unfortunately, the two syndromes (let a1 be some power
of a and a2 be some other power of a)

                      a1 + a2 = s1 = first syndrome

and

                      口三 + a글 = S2 = second syndrome

are simply related by the equation

          S子 = (al + a2)2 = a三 + 2口l(i2 + 口｝ = a三 + 口글 = S2

       We next try using the cubes for the second syndrome,

                                  a? + ag = S2

We rearrange this:

               S2 = a코 + a글 = (a + a2)(a子 + 口l口2 + 畦）

                  = h（好 + a1口2 + 姑）

                  =
                      s1
                       (a1a2
                                + s1)

so that

                                  口l +    口2 =    Si



                                        塑 h
                                 2l
                      a1口2       S               (if   s1 羊 0)


     In all this computing when we want to do a multiplication (or
division) we represent the quantities as a power; hence we add (or
subtract) the exponents; when we want to do an addition we use the
column vector representations and add the corresponding components.
                        Sec. 11.11 / A Double-Error-Correcting Code                     231

 Thus we constantly go between the two forms of representation. The
 matrix itself gives the needed table for the conversions.
     Given the sum and product of two numbers, we almost automati-
cally think of the quadratic equation and its roots,



                       a2   -    (s1)
                                         a +       (5子
                                                              呻，
                                                                   )       :
                                                                               .

The two roots give the individual syndromes of the errors.
    If there is only one error, then the syndromes are

                                             a1 = S1

                                             口？ =        S2


and


                                             毛
                                             H 퍼
                                2l
                                 S
                                                         2l
                                                         n
                                                          S
                                                          乙
                                                                       0           +=



The quadratic equation becomes, therefore,

                      口2 + Si口 = 0                       or            口 = SI

                                                                       口 = 0

      For no errors, we have


                                        Si         S2= 0


and the quadratic equation is

                                 口2 = 0                  口 = 0

                                                         a=        0


    Thus for the lower rows of the matrix we use a3 rather than a as
the generator of the columns. The columns are therefore those cor-
responding to

                  1    a3       a6      a9     a'2        a15      a18         .
232     Ch. 11 / Algebraic Coding Theory




                                              \
(in reverse order). We get the complete matrix M, therefore,
                               少                  少
                                                                                                                                                                                            0
            /
            少 l00
                                                                                                      8
                                                                               0


                                                                                                                                                                                            n 000      000
                                                                               l




                                                          口 m11 dl l1 0
                                                                               口




                                                                                                      口 0 l0 l
                                                                                                                                                                   l
                                                                                                                                                                   d
                                                                                                                            l
                                                                                                                            4ld

                                                                                                                                        0    0 000
                          11上 ]1 0 dl        l dl dl 1l                          l 4
                                                                               0 1 l 1l   Jl 0 1l 0               1
                                                                                                                  l 0 =
                                                                                                                      l 1
                                                                                                                        l                              0 0 11工 1
                                                                                                                                                               l
                      /
                                                                                                                                                                                                    l
                                                                                                                                                                                                    d          l
                                                                                                                                                                                                               d

                                                                                                                                                                   000 l0   0
                 lm                                                                                                                                                                         l


                                                                                                                                          4l
                                                                                                                                           d      11
                                                                                                                                                                                            口 00     0     000
                                                                                                                                         l
                      /
                                                                                                                                                                                                       工
                                                                                                                                                                                                       1
                                                                                                                                                                                                       d
                                                                                                                            l
                                                                                                                            d
                                                                                                                                                                                                  l
                                                                                                                                                                                                  d

                                                                                                                                                                         lJ
                                                                              000

                          dl 0 dl 0          ml dl 0 0    dl 0 0 0                                    Jl 0 1上 0
                                                                                          m1l dl dl
                                                                                                                  l J1l 0 0                00   000    l 4
                                                                                                                                                       4 l 1
                                                                                                                                                           l l
                                                                                                                                                                                                                    r/
                                                                                 lm
                                                                                                      \
                                                                                                      \\          4
                                                                                                                                                                                            十 0 dl 0 0 41上 al 0 0   r
                                                                                          l
                                                                                          1                                                                                                                         /
                                                                                                                                                                                                                    /
as the parity-check matrix for double-error correction. The syndrome
s1 is from the upper rows and the syndrome s2 is from the lower rows.
The two syndromes, through the quadratic equation, give us the two
roots necessary to locate the two errors.
      How do we do the encoding? How to satisfy all the parity checks
at the same time is not clear, but depends on the use of the famous
Chinese remainder theorem-which it is not appropriate to go into in
this very elementary introduction to multiple-error correction. The
elementary nature of the book prevents us from going deeply into the
more difficult parts of coding theory.
      As a concrete example that is easy to follow (and contains the
general case as well as evades the encoding process) take the valid code
of all 0's. Next we assume that during transmission the 0's in positions
corresponding to a3 and a4 are changed to l 's. The syndrome of the
received message will be the sum of those two columns:
                  l
                  d



                           000
                                                                                                                                                                                /l\
                                                                               00                                                                                          101
                                                                               1
                                                                                                                                                       S1=
                                                                                                                                                            -
                                                                                                                                                                            i
                                                                                                                                                                                         lI = a '
                                                                                                                                                                                             m

                                                                                                                                                                                      \l/
                                                                                                                                                                            tl
                                                                                                                            dl 0 l1 0
                                                                               1                                                                                                       1
                      1                                                        1
                            0                                                                                                                                                 0
                                                                               1

                                                                                                                                                                            1 )
                                                                                                                                                                                /0\
                                                                                                                                                                            I l] 1




                                                                                                                                                                    (0\
                                                                                                                    l
                                                                                                                    4                                                                                     =   a
                                                                                                                                                       "             =        0
                                                              U/
                                                                                                                                                                                      \1/
We next calculate
                                                                                              『.                                             /1)
        1
        h
                                                                                                                                                                                       '              10
                                                                                                                     =
                                                                                                                                                                         0                             /i\
                                                                          /
   2l                                   n        2                                                                                                                                                                      a7
    S                                   月J
                                                                               如14
                                                                                a14
             h                                                                                        + a
                                                                                                                                        (0
                                                                                                                                             。         +                 iJ=
                                                                                                                                                                                                      tij=
                                                                                                                                                                                                               '
                                                                                =
                                                                                                                                                                                                      \1/
                                                                          7
                                                                                                                     =


                                                                                                                                             1                           。/
                        Sec. 끄. 끄 / A Double万rror- Correc跏g Code                               233

Hence the quadratic equation is

                             工2 + a7工 + a7 = 0

Tryx = 1, 1 + a7 + a7 = 1,




Try 工 = 口／;




       口2 + a8 + 口7


                         4)4）『（!):(!)
                                   U,
                                   。/
                                             1U J
                                             \1/
                                                            1l J
                                                            \1/
                                                                             11
                                                                             \。
                                                                                       또 n




                             )(
Try 工 = a2;



       口4 + a9 + 口7 =        (三）         +   (!         +                =   ()
                                                                                       王 n
                                   1 1       1 1 I          t ' I            1 '
                                   1/             \。/             \1/             \。


Try 工 = 口3.



       a6 + a10 + a7                                                                   =   n

                                   UI
                                   。l         I\il' I             \il
                                                                   I I       IU
                                                                              \。

Try 工 = a4:




       ."   『a4   『a7    =   （三）         小/                 I\
                                                            101    i\
                                                                   i/
                                                                   ii
                                                                             1/0
                                                                              \。           .
 234    Ch. 11 / Algebraic Coding Theory

 Try 工 = 口5.




        am+a12
            +a7=(!) +(川小.
and so on. Hence the two errors are in positions a3 and a4.
    You can pick any two errors or a single error (or even no error)
and carry out the computation in detail to see how the system works.
The powers of a are given in the top four rows of the matrix.


11.12 Decoding Multiple-Error Codes

For multiple-error-correcting codes there is a simple decoding rule.
You might think that you must effectively, as in Section 11.11, turn over
the syndrome problem to a computer. For a double-error-correcting
code, the computer must find the zeros of the quadratic. One very
simple way to find the roots is to evaluate the quadratic at each position
of the stored message as it is being shifted out. If the power of a satisfies
the quadratic, then it is a root and is one of the positions to be corrected.
     Evidently, you need do this only when there are errors. But in
real-time signaling you need to store several messages at the same time.
When such a system is in operation, you will be shifting out and cor-
recting one message, computing the corrections of a second message,
and working on the first stages of a third. Thus at a minimum there
will be two message time delays. This can be important in the feedback
paths of control circuits! It could cause instability problems.


11.13 Summary

In this chapter we have given the argument for why we want a highly
structured code: so that we can then encode and decode using systematic
methods. We have shown how the division process of dividing one of
our polynomials by another polynomial can be implemented easily.
      We showed how the syndrome is uniquely tied to the error and is
independent of the message. We next got down to the necessity of
using polynomials modulo a prime (nonfactorable) polynomial. We
then saw that the additional condition that the polynomial have a prim-
itive root is necessary so that all the elements can be written as powers
                                               Sec. 11.13 / Summary       235

 of it- sort of going to logarithms. Finally, we illustrated the
                                                                      methods
 by devising one particular double-error-correcting code.
       We did not attempt to provide all the theory of finite fields
                                                                     necessary
 to justify all that can be done, nor to create a general theory
                                                                   ; we merely
 showed how a code could be found. The general codes
                                                                are presented
 so that special cases can be recognized, or even develo
                                                            ped if necessary;
 more than this would make the book far too long and
                                                               would not add
 much to those devoted to algebraic coding theory that
                                                           are already avail-
 able (see the References).
      It is necessary to clearly state that almost all of coding
                                                                   theory was
 developed in the days when computing was relatively
                                                          cheap and storage
 was more expensive. In the year 1985, we are seeing
                                                            a great decrease
in the cost of storage, and hence there is a need to
                                                          reconsider all the
theory that we have developed in the past. Methods
                                                           of design, encod-
ing, and decoding which depend more on table lookup and
                                                                  other forms
of storage and less on computing need to be researched
                                                             and developed.
Again, you need to be warned that the theory is almos
                                                            t all designed to
meet white noise, and in practice often the noise is not
                                                               white and the
theoretical benefits of a code may therefore not be
                                                        realized in practice.
Appendi工 A



                                    Bandwidth and the
                                    Sampling Theorem




A.1 Introduction

This appendix appears to have only a slight connection with the earlier
material; certainly, the mathematical tools used are completely differ-
ent. One reason for including it is that in practice the channel matrix
(Section 7.2)

                                  （只， /)
is rarely available. But more important, to send digital information we
normally use analog channels that are almost exactly linear. The ca-
pacity of analog signal channels is typically measured by "bandwidth";
therefore, it seems necessary in a book on coding and information theory
to at least glance at the idea of bandwidth and related topics such as
power.
      The eigenfunctions (the proper functions) of a linear, time-invariant
system are the complex exponentials

                                   e2n可i


Eigenfunction means that the system does not change the form of the
function, only the amplitude. Time-invariant means that the behavior
of the system is not a function of time but only of the inputs. This is
characteristic of most current communication systems. Linear means



                                                                       237
238    Appendix A / Bandwidth and the Sampling Theorem

that the sum of two functions put into the channel gives the sum of the
individual outputs as the output. This is characteristic of most channels
provided that we avoid overloading them. The frequency f is measured
in rotations (when we do the calculus we use the angular frequency
m= 2rrf). The independent variable is t, usually time.
      A band-limited function is a function whose frequencies are all
limited to some band. A familiar example is a hi-fi system, which
typically will have a lower limit at best of a few cycles per second, say
15 or maybe even a hundred, and an upper limit of around 18,000 cycles
per second. . International convention uses the symbol Hz (hertz) for
"cycles per second." Radio and television stations are limited to certain
bands of frequencies so they do not interfere with each other's broad-
casts. Many other systems have a natural limit to their band of fre-
quencies, although in most all cases the band is not as sharply cut off
 as the theory indicates.




A.2 The Fourier integral

The Fourier integral is the natural mathematical tool for handling band-
limited functions. The Fourier integral represents a function g(t) as a
sum of complex exponentials (the eigenfunctions) in the form



                            g   (t)     =       f (f),   G        e2:         ' '   df
The function under the integral G(f) is called the transform of g(t). It
is related to the original function by the interesting formula



                        G         (f)       =   L.           g   （加－    2可남
which is the same as the original one except for the sign on the i; one
integral has a " +i " and the other has a "- i " term in the exponent.
     The Fourier integral is like a glass prism that breaks up a light beam
into its colors-frequencies. The function G(f) gives the amount (am-
plitude) of the frequencyf in the original time signal g(t). The integral
is simply the properly weighted sum of all possible frequencies; G(f) is
the weight at frequency f.
     There are positive and negative frequencies to correspond to the
pair of functions cos 2irft, sin 2可t, which have the exponential repre-
                                             Sec. A.2 / The Foi玎jeT Ii玎egr口／             239

sentation


                         m,
                         c。 2寸- e21T +-' e "2 ' '
                          s2rrft-
                                      乙
                                             e2TTift -               e 2mt'
                         sin 2可｝ =
                                                                2i
                                             G(f)
                                                 1




                                                 //1/
                                                                    2F


                                                                                 1
                                                                                     f
                     -
                         F                                                  F


                   Figure A.2-1 Band-limited function
    As an example of a band-limited function, suppose that G(f) is
zero outside the band (Figure A.2-1) ,

                                       -F 드 / 드 F

Thus we have


                         g
                             (t)
                                   =    1-
                                             F
                                                 G
                                                        (f)e2似可

Suppose further that inside the band the function G(f) is a constant
1/2F, chosen so that the area under the function G(f) is exactly 1. We
have, therefore,

                         ..            fF    1          -
                     g(t) = n-
                     g(D    J-F2F e'- 9' dj
                                       1 e2 刃 F
                                             "」


                                   2F 2'rrit                -
                                                                F
                                   e21了iFt -            r211iFi            1
                                                 2i                      2irFt
                                   sin 2ir Ft
                                        2'nFt
 240   Appendix A / Bandwidth and the Sampling Theorem

     This is the classic function (sin x)Ix shown in Figure A.2-2. It has
a main lobe about zero of width 2/F and side lobes of half that width
which decrease in size like lit. The larger F is (the wider the band),
the narrower is the center lobe and the side lobes as well. This suggests
that a function can peak up suddenly only if the function has a wide
bandwidth.


                         1.0




-2/F          -1/F      -0.5           1/F           2/F          3/F


                         Figure A.2-2 f (x) = 뽁즈

A.3T加 Sa,까刃i兀gT九eore刃i

The famous sampling theorem connects the rate of sampling with the
bandwidth that is necessary to reconstruct the function from the sam-
ples. Before stating the theorem, we need to remind readers of some
of their experiences. When viewing a movie or a TV program, what
you see is a sequence of still pictures flashed so frequently that they
appear to be moving; typically, about 15 to 20 times a second is enough
to fool the human eye. However, there are clues to the sampling. For
example, when the stagecoach in the "Western" starts moving, the
wheels appear first to speed up, then to slow down, stop, go backward,
stop, go forward, and so on, depending on the speed. The reason is
easy to see (Figure A.3-1). When the stage coach wheel has turned so
fast that one spoke advances to the position of the next spoke, they will
appear to be standing still. Indeed, when the spoke gets merely to half
the position of the next spoke during one time interval between samples,
the wheel will appear psychologically to stand still and to have twice
the number of spokes that it really has. At a rate slightly faster than
this, the spokes will appear to be going backward.
                                 Sec. A.3 / The Sampling Theorem       241




       SLOW ROTATION          MIDDLE ROTATION        FASTER ROTATION

    APPEARS AS A DIRECT    APPEARS AS IF STAND-    APPEARS AS A BACK-
    대玎AT山N                 什寸G ST比L 베TH DOUBLE     밖ARD ROTATION
                           THE NUMBER OF SPOKES

                                 Figure A.3-1


     This can be viewed as the consequence of a simple trigonometric
identity, cos [2ir(m + a)t + 卜 = cos[2ir(at) + 卜], where m = an
integer and 0 5 a < 1. Clearly, any multiples of 2ir can be removed
from trigonometric sine and cosine functions when the sampling interval
is 1 (which we can always have by scaling the time variable). If a >
L we can also reduce the effective frequency further by taking half-
integer multiples from the frequency, since that merely changes the signs
of the functions = cos[2町(1 - a) - 巾]. Thus high frequencies will
always appear, because of sampling, to be low frequencies. The highest
frequency that can be observed without change is that which has two
samples taken in each full cycle. Lower frequencies have no aliasing,
but higher ones are aliased into lower frequencies, aliased in the sense
that at the sample points the two frequencies have the same samples.
     Once this is grasped, we can state the sampling theorem. Given
the samples of g(n) (at all integer values of n) of a band-limited function
g(t), we form the doubly infinite sum


                   g(t) = ,立, g(k) (sin，
                                       (k-
                                       咎-t)'))
Inspection of the terms shows that at the sample points, say at t = k,
the kth term with coefficient g(k) peaks up to the correct value and all
other terms have the value zero. Thus the sum has the proper value
at this point. There is, of course, the remaining question: Is the re-
constructed function band-limited? We see from Section A.2 that it
is- after the shifting of a (sin x)/x term it is still band-limited.
     Since this is not a mathematics course, we will not try to prove that
the series converges (it obviously does at the sample points), let alone
that it converges to the right function. Both are true.
242     Appendix A / 及zndwi加i 口nd the S口7刃p／加g Theorem

 A.4 Ban內山i比 Versus Rapid C九ange

From the preceding section we see that the bandwidth of a signal is
 inversely proportional to the width of the main lobe of the function (sin
 2rrFt)I (2町Ft)-it takes a wide band of frequencies to get a narrow
 spike. We are not in a position (lacking a great deal of mathematical
 theory) to prove that no shape of the amplitude G(f) in the band can
give a narrower spike than the rectangular shape, so we are reduced to
making suggestive observations as to why this is so.
     It is not rapid change itself that is impossible for a narrow-band
 function; we have only to select any particular frequency, other than
zero frequency, and take a sufficiently large an amplitude to have as
large a change as we want in as short a time as we want. Rather, we
want a change from one extreme to another, from a maximum to a
minimum, or the reverse. This means that at the ends of the interval
we want a horizontal tangent. Thus we have, essentially, a cos 2irFt
(0 5 2ir Ft 5 町), and the transition takes place in time 112F. Again
we have the same reciprocal relationship between frequency and rate
of change of the signal.
     The sampling theorem, of course, is saying the same thing; we must
have the necessary bandwidth, and this requires at least two samples in
the highest frequency present in order to reconstruct the original signal
(assuming that the samples we have go from the time -m to + x).



A.5 AM Signaling

 Most people know at least a little about AM (amplitude modulation)
 radios. The frequency of broadcast that you tune the radio set to is
 called the "carrier frequency" and is a constant frequency carefully
 controlled by the sending station. All the radio station does is change
 the amplitude of the frequency they send, and of course in turn that of
 the signal you receive (see Figure A.5-1). This, however, amounts to
 a small change in frequency, because the product of two cosines is a
 pair of cosines each shifted in frequency from one of the original ones
 (see a few lines later).
      The radio receiver, by tuning, filters out all the frequencies that
are broadcast except those close to the carrier frequency. Then in one
way or another the received signal is "rectified"- meaning that the
negative parts are either cut out or else are actually reversed in sign
and are made positive. When the result of this is "smoothed" a bit, it
is, approximately, the original modulation curve that the station imposed
on its carrier.
                         243
너
m1 < 亡＝ 智m
    노 띨 8O O
           C山尸 8O
             1
                    山d
                    q
                    H
2恥     Appendi工 A / Bandwidth 口nd the S口r刃pling Theorem

    How does this involve the bandwidth? Suppose that the musical
note to be broadcast is the pure sinusoid

                                cos 2irft

and that the carrier frequency wave is

                               cos 2irf0t

where f。is very much larger than f. The modulated signal that is sent
is the product of the two cosines:

     (cos 2可以cos 21T和） = 吉 cos 21T(f0 + f)t + 글 cos 2'rr（九 - f)t

Enough information is contained in either of the two terms to reconstruct
the original-provided that the carrier frequencyf。is known (you select
the carrier frequency you want when you select the station by your
tuning). Thus there are "single-sideband" signaling systems which
broadcast only one of the two terms and suppress the other.
     Inspection of this formula shows that to receive a band of frequen-
cies of the original signal, you need to receive the same bandwidth (but
shifted up by the carrier frequency). Thus it is bandwidth that is nec-
essary to transmit the information-and the wider the band available,
the more different signals you can transmit. Put simply, large bandwidth
gives high fidelity, and lack of bandwidth will suppress many frequencies
and give low fidelity.
     The same is true in telephone conversations, although there is no
carrier in the simplest cases. The telephone design allows the trans-
mission of frequencies up to around 3600 Hz and pretty well suppresses
those above 3600 Hz. This bandwidth gives medium fidelity. Higher-
quality phone conversations ("quality" in tone, not in content!) would
require wider bandwidth, and it is a fact of nature that bandwidth costs
money and effort to achieve. The bandwidth originally chosen for
telephones was an engineering compromise at that time between quality
and cost, and it is not easily upgraded when the installed physical plant
is so large.



A.6 FMS智nat加g

Signaling using AM, because of the fading and other properties it has,
is not as good as FM (frequency modulation), In AM the amplitude
of the transmitted signal is modulated; in FM the frequency is modu-
                                          Sec. A. 7 / Pulse Signaling     245

lated, meaning that the information is sent by directly varying the fre-
quency. By using automatic gain control at the receiving end, the
amplitude of the signal is kept approximately constant in spite of fading.
    If the receiver has a filter (tuner) that lets less and less of the signal
through when the frequency is farther and farther away from the carrier
frequency (typically, this is much higher than the AM carrrier fre-
quency), then the energy (or power, if you prefer to measure things as
energy per unit time) changes correspondingly. Thus loosely speaking,
FM works with the signal

                           A cos 2ir[f。+ f (t)]t

where f (t) is small with respect to the f) of the carrier. Again it is
bandwidth that is necessary to convey the information.
    By using a much wider band than that used in AM, FM has much
more ability to suppress noise and more faithfully reproduce the original
signal. For the same bandwidth both AM and FM are equally effective.


A.7 Pulse Signaling

Typically, digital signals are sent as one of two states. One of two
frequencies can be used, or one of two voltages (pulses) to signal. In
the case of pulses, the corresponding representation in the characteristic
modes (the eigenfunctions) of the linear, time-invariant signaling sys-
tem,
                                  e2ni/1

is given by a Fourier integral. But a linear system can give various gain
and phase shifts to each different frequency. Therefore, the original
pulse is apt to have quite a different shape at the detecting end. Further
distortion comes from the inevitable "noise" of all real systems.
      The wider the bandwidth, the more rapidly the system can change,
and the more rapidly pulses can be sent down the system. Not that the
pulses move faster, but they are spaced more densely in time. The
inevitable distortion of the signaling system must not be allowed to grow
too large before detection, reshaping, amplification, and retransmis-
sion. By spacing the repeaters sufficiently closely together, the deg-
radation of the original pulse is kept small and hence the reliability is
made high.
      Sometimes it is the change of state of the system that indicates a 1
and no change a 0, rather than pulses for l 's and no (or negative) pulses
的r0눔．
246    Appendi工 A I Bandwidth and the Sampling Theorem

      There are many elaborate systems for pulse signaling; especially
difficult are the problems of timing synchronization, and these lead to
involved systems. Error detection and correction are often incorpo-
rated into the pulse system.



A.8 Barn加id比 Genera幻

This appendix is intended to familiarize the reader with several aspects
of channel capacity as equivalent to bandwidth. Without the use of a
formidable amount of mathematics associated with the Fourier integral,
the results can only be sketched. The aim of the appendix is to indicate
that in some sense channel capacity as defined in information theory is
related to bandwidth, which is the way channel capacity is usually rated
in practice.
      From Shannon's theorem we would expect that very sophisticated
methods of encoding information could achieve great improvements in
noise suppression without going to wide bandwidths. It is the corn-
plexity of the encoding and decoding that has stopped such efforts on
a wide scale, such as for radio and TV. As we have seen, good encoding
methods involve very long messages, and this has both severe storage
problems and delays to contend with, let alone the processing of the
signal. Thus practical signaling systems rarely come near to the ideal
of Shannon's theorem. But the appearance of cheap microcomputers
and cheap digital storage devices may change matters in the near future.
       In TV it is necessary to achieve all the possible changes at each
spot on the screen from one picture frame to the next, and this requires
 very wide bandwidths. But psychological tests indicate that human
beings cannot process much more than 40 to 50 bits per second, if that
much. Even allowing for the fact that various people seeing the same
picture will process different parts of the picture, still the disparity be-
 tween what is done and what seems to be the minimum necessary is
 almost a millionfold. It is in this way that Shannon's theory is most
useful-it points to places where there are possibly large gains and steers
 the engineer away from places where there can be only small improve-
 ments at best.
       There is only so much bandwidth in the spectrum of available fre-
 quencies that will pass through the earth's atmosphere, and already much
 of it is assigned to various uses. In a sense bandwidth is a "natural
 resource" that is definitely limited, not in the sense that the use from
 moment to moment consumes it, but in the sense that various competing
 uses of it cannot be made at the same time. From information theory
 we have a guide to where the bandwidth is used efficiently and where
 it is being wasted.
                                                   Sec. A. 9 / Continuous Signals   247

      Because of the availability of cheap, reliable microcomputers, dig-
ital signaling methods that permit easy protection against noise (errors)
are of increasing importance, and we have, therefore, neglected analog
signaling systems in this brief discussion.




A.9 Continuous Signals

In actual practice, we usually send continuous (analog) signals (Section
 A.1), even when we have already encoded the message into binary
digits. Thus it is necessary to look briefly at the information contained
in an analog signal.
     Most signaling systems use band-limited signals (Section A.2). Na-
ture comes fairly close to this in many situations, although the absolutely
sharp cutoff of the model does not occur in practice. Given a band-
limited function of bandwidth W, the famous sampling theorem (Section
A.3) says that it takes 2WT samples to reconstruct the signal of duration
 T. We assume that this theorem is true.
     If we are sending the information in a continuous form of signals,
each of duration T, each signal is represented by exactly 2WT numbers
x. taken at equally spaced intervals. Thesse 2WT samples, numbers,
can be viewed as a point in a 2WT-dimensional space, where we are
now thinking of the space as continuous between the points.
     It is natural to associate the coresponding energy E with


                                                                                (A.9-1)


The distance (radius) from the origin to this signal (using Euclidean
distance) is



                             r
                             「
                                  =
                                  ＝
                                           (
                                           (2D1/
                                                           2



Hence we have

                                 r = (2WE)"2

Since the signal power S is the energy E per unit time, we have


                                      s=
                                                     EHT
248    Appendix A / Bandwidth and the Sampling Theorem

and the radius of the sphere of signals being sent is

                            r = (2WST)112                     (A.9긔

    The noise added by the channel is also measured by its power, this
time labeled N for "noise power." Thus each sent signal is disturbed
by the noise and at the receiving end lies in a sphere about the sent
signal of radius

                                 (2WNT)112                     (A.9-3)

The whole (original) sphere (A.9-2) must be enlarged for this added
noise and now has a radius of

                         r = [2WT(S + N)]112                   (A.9-4)

     As before (Section 3.6), we ask: How many spheres of radius of
the noise (A.9-3) can fit in the enlarged sphere (A.9-4) of received
messages? We divide the total space of received messages up into
spheres of radius = (2WNT)112 about the sent signals and get an upper
bound on the total number of possible messages M that will be distinct
at the received end. Using the formula for the volume of a 2WT-
dimensional sphere, we get the bound

              Ms 町叩' [2WT(S + N)］叩T F(WT + 1)
                      [' (W丁 + 1)  ,WT(2WT入／\H丁
                              WT
                    i'     S'\
                 5; Ii   + -=1
                    \      NJ

     The amount of information sent is the log of the number of equally
likely sent messages; hence

                                                   1    s\
                    1= loaM = WTloal 1+ -I
                       n。      - -- C7 \ - Ni

and the rate of information being sent per unit time is


                            W log   (i
                                         /



                                             +      )
                                                 r겨 \




This is the standard formula in the usual "signal-to-noise" form.
    We have found an upper bound for the capacity of a channel with
                                     Sec. A.9 / Continuous Signals    249

bandwidth W and corresponding powers in both the signal
                                                              and noise.
It is much more difficult to get a lower bound since we
                                                             will have to
repeat the essentials of Shannon's main theorem and show
                                                              that we can
indeed pack in that many spheres (less a small amount
                                                         that still leaves
us arbitrarily close to capacity). The mathematical details
                                                            in Chapter 9
and the proof of Shannon's theorem in Chapter 10 were
                                                          both arranged
so that this fact would seem to be probably true
                                                 without proof.
                                                                   忿轟茹




Appendix B



                                       Some Tables for
                            E兀tr아iy Calculat油is




                  Five-place Tables of the Functions:
          log2 (l/p), p log2 (lip), H2(p) for p 0.00(0.01)1.00


         p           log (u/p)       p log (lip)         H(p)


        0.00            -                 0                 0
        0.01         6.64386          0.06644           0.08079
        0.02         5.64386          0.11288           0.14144
        0.03         5.05889          0.15177           0.19439
        0.04         4.64386          0.18575           0.24229
        0.05         4.32193          0.21610           0.28640
        0.06         4.05889          0.24353           0.32744
        0.07         3.83650          0.26856           0.36592
        0.08         3.64386          0.29151           0.40218
        0.09         3.47393          0.31265           0.43647
        0.10         3.32193          0.33219           0.46900
        0.11         3.18442          0.35029           0.49992
        0.12         3.05889          0.36707           0.52936
        0.13         2.94342          0.38264           0.55744
        0.14         2.83650          0.39711           0.58424
        0.15         2.73697          0.41054           0.60984
        0.16         2.64386          0.42302           0.63431
        0.17         2.55639          0.43459           0.65770
        0.18          2.47393          0.44531           0.68008
         0.19         2.39593          0.45523           0.70147



 250
                                  Appendix B /   251

  p     log (lip)   p log (lip)      H(p)


 0.20    2.32193     0.46439        0.72193
 0.21    2.25154     0.47282        0.74148
 0.22    2.18442     0.48057        0.76017
 0.23    2.12029     0.48767        0.77801
 0.24    2.05889     0.49413        0.79504
 0.25    2.00000     0.50000        0.81128
 0.26    1.94342     0.50529        0.82675
 0.27    1.88897     0.51002        0.84146
 0.28    1.83650     0.51422        0.85545
 0.29    1.78588     0.51790        0.86872
 0.30    1.73697     0.52109        0.88129
 0.31    1.68966     0.52379        0.89317
 0.32    1.64386     0.52603        0.90438
 0.33    1.59946     0.52782        0.91493
 0.34    1.55639     0.52917        0.92482
 0.35    1.51457     0.53010        0.93407
 0.36    1.47393     0.53062        0.94268
 0.37    1.43440     0.53073        0.95067
0.38     1.39593    0.53045        0.95804
0.39    1.35845     0.52980        0.96480
0.40    1.32193     0.52877        0.97095
0.41     1.28630    0.52738        0.97650
0.42     1.25154    0.52565        0.98145
0.43    1.21754     0.52356        0.98582
0.44    1.18442     0.52115        0.98959
0.45    1.15200     0.51840        0.99277
0.46    1.12029     0.51534        0.99538
0.47    1.08927     0.51596        0.99740
0.48    1.05889     0.50827        0.99885
0.49    1.02915     0.50428        0.99971
0.50    1.00000     0.50000        1.00000
0.51    0.97143     0.49543        0.99971
0.52    0.94342     0.49058        0.99885
0.53    0.91594     0.48545        0.99740
0.54    0.88897     0.48004        0.99538
0.55    0.86250     0.47437        0.99277
0.56    0.83650     0.46844        0.98959
0.57    0.81097     0.46225        0.98582
0.58    0.78588     0.45581        0.98145
0.59    0.76121     0.44912        0.97650
0.60    0.73697     0.44218        0.97095
0.61    0.71312     0.43500        0.96480
0.62    0.68966     0.42759        0.95804
0.63    0.66658     0.41994        0.95067
0.64    0.64386     0.41207        0.94268
252   Appendix B / Some Tables for Entropy Calculations

           p          log (l/p)      p log (lip)      H(p)


          0.65        0.62149         0.40397        0.93407
          0.66        0.59946         0.39564        0.92482
          0.67        0.57777         0.38710        0.91493
          0.68        0.55639         0.37835        0.90438
          0.69        0.53533         0.36938        0.89317
          0.70        0.51457         0.36020        0.88129
          0.71        0.49411         0.35082        0.86872
          0.72        0.47393         0.34123        0.85545
          0.73        0.45403         0.33144        0.84146
          0.74        0.43440         0.32146        0.82675
          0.75        0.41504         0.31128        0.81128
          0.76        0.39593         0.30091        0.79504
          0.77        0.37707         0.29034        0.77801
          0.78        0.35845         0.27959        0.76017
          0.79        0.34008         0.26866        0.74148
          0.80        0.32193         0.25754        0.72193
          0.81        0.30401         0.24625        0.70147
          0.82        0.28630         0.23477        0.68008
          0.83        0.26882         0.22312        0.65770
          0.84        0.25154         0.21129        0.63431
          0.85        0.23447         0.19930        0.60984
          0.86        0.21759         0.18713        0.58424
          0.87        0.20091          0.17479        0.55744
           0.88        0.18442         0.16229        0.52936
           0.89        0.16812         0.14963        0.49992
           0.90        0.15200         0.13680        0.46900
           0.91        0.13606         0.12382        0.43647
           0.92        0.12029         0.11067        0.40218
           0.93        0.10470         0.09737        0.36592
           0.94        0.08927         0.08391        0.32744
           0.95        0.07400         0.07030        0.28640
           0.96        0.05889         0.05654        0.24229
           0.97        0.04394         0.04263        0.19439
           0.98        0.02915         0.02856        0.14144
           0.99        0.01450         0.01435        0.08079
           1.00        0.00000         0.00000        0.00000
                                                                   R可erences




                        ABRAMSON, N. Information Theory and Codin
                                                                  g. New York:
              [A]
                        入4cGraw-Hill夕 1963.
            [Bi]         BERLEKAMP, E. R. Algebraic Coding Theory.
                                                                   New York:
                         McGraw-Hill, 1968.
            [B2]        BERLEKAMP, E. R., ed. Key Papers in the Devel
                                                                      opment of Cod-
                        ing Theory. New York: IEEE Press, 1974.
        [B!
                    ]   BLAHUT, R. E. Theory and Practice of Error-
                                                                   Control Codes.
                        Read旽，入4A: Addison八Wesley, 1983.
       [Bla]            BLAKE, i., ed. Selected Papers on Algebraic Codin
                                                                          g Theory.
                        Stroudsburg, PA: Dowden, Hutchinson & Ross, 1973.
       [BM]             BLAKE, J. F., and MULLIN, R. C. An Introduction
                                                                        to Algebraic
                        口nd Combin口to亢口／ Coding 刀ze（刃． New York:
                                                                    Academic Press,
                        1976.
                        CLARK, G. C., and CAIN, J. B. Error-Correc
                                                                   ting Coding for Dig-
      [Cl
                        ital Communications. New York: Plenum, 1981.
[DG]                    DAVISSON, L. D., and GRAY, R. M. Data Compressio
                                                                         n. Strouds-
                        burg, PA: Dowden, Hutchinson & Ross, 1976.
                        GALLAGER, R. G. Information Theory and Reliable
                                                                        Communi-
[G]
                        cation. New York: John Wiley, 1968.
[Ga]                    GATLIN, L. L. information Theory and the Living
                                                                        System. New
                        York: Columbia University Press, 1972.



                                                                                   253
254          References

             GUIASU, s. Information Theory with Application工 New York:
             入'IcGraw-I궤1, 1977.
             JAYANT, N. S. Waveform Quantization and Coding. New York:
             IEEE Press, 1976.
             KNUTH, D. E. The Art of Computer Programming, Vol. 3: Sort-
             ing and Searching. Reading, MA: Addison-Wesley, 1973.
             LIDL, R., and NIEDERRETIER, H. Finite Fields. Reading, MA:
             Ad小的n-Wesley.
             LIN, S., and COSTELLO, D. J., JR. Error-Control Coding: Fun-
             damentals and Applications. Englewood Cliffs, N.J.: Prentice-
             Hall, 1983.
     MCELIECE, R. J. The Theory of Information and Coding. Read-
     ing, MA: Addison-Wesley, 1977.
[ME] MARTIN, N. F. o., and ENGLAND, j. w. Mathematical Theory of
     Entropy. Reading, MA: Addison-Wesley, 1981.
[MS]          MACWILLIAMS, J., and SLOANE, N. J. A. The Theory of Error-
                                                                       -
              Correcting Codes Amsterdam: North-Holland, 1977. (Amen-
              can edition: Elsevier, New York.)
[P]
     PLESS, v. Introduction to the Theory of Error-Correcting Codes.
     New York: John Wiley, 1982.
[PW] PETERSON, W. w., and WELDON, E. J., JR. Error Correcting Codes,
     2nd ed. Cambridge, MA: MIT Press, 1972.
  [S]
              SLEPIAN, D.,ed. Key札pers in枷Deve／   아功ient of／刃和rm口玎이'1
              Theory. New York: IEEE Press, 1974.
[T]           THOMPSON, T. M. From Error-Correcting Codes through Sphere
              Packing to Simple Groups. Washington, DC: Mathematical As-
              sociation of America, 1983.
      [VJ
              VITERBI, A. .j., and OMURA, J. K. Principles of Digital Commu-
              nication and Coding. New York: McGraw-Hill, 1979.
  凹］          WAKERLY, . . Error-Detecting Codes, Self-Checking Circuits and
              Applications. Amsterdam: North-Holland, 1978.
      [WJ]    WOZENCRAFT, J. M., and JACOBS, I. M. Principles of Commu-
              nicarion Engineering. New York: John Wiley, 1965.
                                                                   Index




      A                                     capacity of, 160-61
                                          Binomial coefficient bound, 170-73
Abramson, N., 253
                                          Binomial coefficients, 13
Abstract theory, 1
                                          Bit, 7
A미이nt system, 133
                                            of information, 106
Algebraic coding theory, 209
                                          Blake, I., 253
AM signaling, 242
                                          미ock code, 68
AND, 30
                                          Burst error-detecting codes, 26
Anti-Gray code, 99
                                          B叭e, 10
ASCII code, 8, 10, 11, 27
  table of, 13
Average code length, 2, 63                      C
Average error probability, 201            Cain, F.B., 253
Average random code, 201
                                          Carrier frequency, 224
                                          Cauchy functional equation, 104
      B                                   Channel, 138
                                            definition of, 139
Backward conditional probabilities, 142     encoding, 2
Bandwidth, 237                              properties of, 140
  example, 238                              uniform, 154-55
  generally, 246                          Channel capacity, 103, 201
  vs. change, 242                           of binary symmetric ch出lnel, 160-61
Bayes' formula (theorem), 141               definition of, 153
Berlekamp, E.R., 253                        encoding, 5
Bernoulli trials, 183                     Channel relationships, 140
Binary encoding, 7                        Chebyshev's inequality, 181-82
Binary symmetric channel, 18, 142, 159,   Clark, G., 253
       195                                Code compression, 18

                                                                           255
256       Index

Codes:                                       E
  anti-Gray, 99
  burst-detecting, 26                  Efficient codes, 51, 56, 64
  comma, 54, 59, 69                       Markov, 86
  delta m어ulation, 100                 Eigenfunctions, 237
  error-correcting, 34                 England, J., 254
  error-detecting, 20                  Entropy, 103, 107
  ext이好幻ns of, 72                         conditional, 130, 146
  Gray, 80, 97                            joint, 146
  hash, 94                                of Markov processes, 129
  hexadecimal, 10                         received symbols, 145
  Huffman, 51                            robustness, 136
  instantaneous, 53-55                    of source, 18
  miscellneous, 79                        source alphabet, 145
  Morse, 12-13                         Entropy function, 1, 107
  octal, 9                                fund게mental inequality, 115
  predictive, 79                         maximum of, 117
  rad奴 r, 15                             properties of, 114-19
  random, 79                             table of, 250
  resynchronization of, 101            Equilibrium probabilities, 133
  Shannon-Fano, 121-22, 126            Equivalent codes, 42
  2-out-of-5, 14, 23                   Equivocation, 148
  unique, 52                           Ergodic Markov processes, 85
  van Duuren (3-out-of-7), 23          Error correction, 34
  variable-length, 12, 51              Error-correcting codes, 35-36, 158
  weighted, 27                           perfect, 158
Coding:                                Error-detecting codes, 20, 22, 147, 210
  Huffman, 51                            probability, 24
  Shannon-Fano, 121                      why, 20
Combinations, 13                       Error integral, 174
Comma codes, 54, 69                    Errors of interchange of symbols, 28
Conditional mutual information, 150,   Escape characters, 15
       161                             Evolution, 3
Conditional probability, 80            Excess redundancy, 22
Continuous signals, 247                Extensions of a code, 53, 72, 124
Costello, D. J., 254                     Markov process, 87
                                         examples, 126
      D

Davidson, L.D., 253                          F
Decision rule, 192
Decision tree, 53                      Fano bound, 205
Decoding tree, 54, 56-57, 60, 62       Finite automation, 53, 77
Delta modulation, 100                  Finite fields, 210
Digital signaling, 6, 237              FM signaling, 244
Direct product, 53                     FORTRAN, 16, 49, 95
Double-error-correcting code, 228-34     compile, 17
Double-error-detecting code, 47        Forward conditional probabilities, 141
                                                                   Index   257

  Fourier integral, 238                 Interchange of symbols, 28
  Fund쾨mental error formula, 199        ISBN book numbers, 32

          C                                     J

 Gallager, R.G., 253                    Jacobs, I.M., 254
 G出아s fields, 4, 195                    Jay카U,卜LS., 254
 Gamma function, 173
 Gatlin, L.L., 253                            K
 Geometric approach, 44                 Knuth, D.E., 254
 Gibbs inequality, 117
                                        Kraft inequality, 57, 62, 121
 Gray codes, 80, 97
                                          theorem, 57
   decoding, 99
   details of, 98                             L
 Gray, R.M., 253
   code, 97                            Law of large numbers, 183
 Guiasu, S.. 254                         theorem, 184
                                       Lin, S., 254
                                       Logical add (XOR), 23, 31
          H

Hamming, distance, 45, 189                   人I
   meaning of, 46
                                       MacWilliams, J., 254
Hamming error-correcting codes, 39,
                                       Markov process, 80, 129, 131, 135
         210-11, 213, 220
                                         ergodic, 84
   exam미e, 41
                                      Martin, N., 254
   parity checks, 39, 210
                                      Maximum likelihood rule, 192, 196
     table of, 40
                                      McEliece, R.J., 254
Hamming-Huffman coding, 78
                                      McMillan inequality, 62
Hartley, 106
                                      Metalanguage, 16
Hash coding, 94
                                      Memory source, 80
   collisions, 95
                                      入4idpoint 的rm따a, 166
  remov키s, 96
                                      Minimum dist카lce, 45
Hexadecimal code, 10
                                      Minimum variance codes, 68, 75
History, 2
                                      Model of signaling system, 4
Huffman codes, 51, 63, 71, 114
                                      Modular arithmetic, 30
  examples of, 65, 67-68
                                      Modulation, 242
  noise in, 74
                                      Modulo 2 arithmetic, 21
  radix r, 73
                                      Monic polynomial, 215
  use of, 77
                                      Morse code, 12, 13, 51, 63
  variability of, 68
                                        table of, 13
                                      Mutual information, 148
      I                                 definition of, 148
Independent errors, 23                  properties of, 149-51
Information source, 1, 5
                                            N
   definition of, 104
Instantaneous codes, 53               nat (unit of information), 106
   construction of, 55                n-dimensional codes, 37, 45
258    Index

n-dimensional paradox, 179           Random type fonts, 118
肛面nensional space, 176               Rectangular codes, 35
  Euclidean, 176                     Redundancy, 22, 36
     distance, 176                   Reliable, 20
n-dimensional spheres, 177           Restrictions on codes, 21
   coefficients, 177                 Resynchronization, 101
  向rmula 匈r, 177                     Retransmission, 25
   table of, 177
Noise, 23
                                           S
   entropy, 148
   in Huffman codes, 74              Sampling theorem, 240
Noise power, 248                     Single-error-detecting plus double-error-
Noiseless coding theorem, 104, 125           correcting codes, 46, 228
NORC computer, 34                    Shannon, 2
                                     Shannon's theorems:
      O                                main, 191
                                          converse, 207
Octal code, 9                              general case of, 204
Omura, J.K., 254                       noiseless, 125
                                     Shift registers, 224
      P                              Shortened block codes, 60
                                     Side lobes, 240
Parity check, 21, 40
                                     Slepian, D., 254
  computing, 22
                                     Sloane, N.J.A., 254
  even, 21
                                     Source alphabet, 2, 6
  odd, 21
                                     Source encoding, 2, 5
Peterson, W.W., 254
                                     Stirling's approximation, 165-70
Pless, V., 254
                                        table of, 170
Polynomials, 214
                                     STRETCH computer, 35
  prime, 215
                                     Syi小이， l
  primitive root, 219
                                     Symmetric channel, 18
Predictive encoding, 79, 88
                                     Syndrome, 38, 39, 212
   encoder, 89
   decoder, 90
   run length, 91                           T
   summary, 94
Prime polynomials, 215                Thompson, T.M., 254
Primitive roots, 219                  Transition graph, 81
Probabilities of symbols, 1, 63         equilibrium, 83
 Pulse signaling, 245                   limiting matrix, 83
                                        matrix, 82
                                        probability, 82
       R
                                      Trapezoid rule, 165
 Radix r codes, 15, 72                Triangular codes, 37
 Random code, 196, 203                Two-out-of-five codes, 14, 23
   average of, 201                       table, 14
 Random encoding, 79, 196             Two state devices, 6
                                                            Index   259

      U                                  w
Uniform channel, 154-55            Wakerly, J. 254
  definition, 155                  Wallis integrals, 168
Uniform input, 156                 Weighted codes, 27
Unique decoding, 52, 62            Weldon, E.J., Jr., 254
                                   White noise, 23, 39
                                   Wozencraft, J.M., 254

      V                                  x
van Duuren code (3 out of 7), 23   XOR (instruction), 30
Variable length codes, 13, 51
Variance, 181
                                         z
  minimum, 75
  of sums, 184                     Zipf distribution, 71
Viterbi, A.J., 254                   entropy of, 112
                                      Coding and Information Theory

                                           Homework No. 7 (due test)
                  channe四1 cascade로 connect되어 있을 경우，



                                                        B                                                 C
                            Channel 1                                               Channel 2


in case ‘.

channel 1 의 input alphabet : A                  output alphabet: B

channel 2 의 input alphabet : B                  output alphabet: C
Show that
                                                 //（川 C) 2H（川 助
                                                 /(，寸,B) 2 /(，才, C)

          P(ck i b1,a1) = P(ck b1)              for alli, j小
(hint :
          尸（a 1 bf,ck) = 尸（a1 吃）                f。
                                                 r a11i, k)
                                                        j,
2. In BSC.


                                                                                                      9
                                  1 ／入 1




                                                                                                 1
                                                                                                 日e
                                                                                    T   二二   M
                                                                                             Q
                                                                                                              1




                                                                I   -   I




find channel capacity.

                 1/ 2    1/ 2口                                               2/ 3       1/ 3
      T=                                                     (b) T=
             H
                 1/ 3    2/ 31                                               1/ 3       2/ 3
(a)
                 9/ 10    1/ 10                                             rl/ 2 1/ 2
（이 T =                                                       (d) T= I
                 1/10     9/ 10                                             L"2 1/ 2

3. (Channel Capacity)

(a) Let C denote the capacity of a discrete memoryless channel with input alphabet X={xl,x2.....xN}

and output alphabet Y={yl,y2.....yM}. Show that C 드 min{logM, logN} . What interpretation can
you make of this fact?
                                                           a   '                   A   '




                                                                                       1
                                                           b   '




                                                                                       1




(b) Find the capacity of the channels A and B as shown in the below Figure. What is the

capacity of the cascade channel AB?(Hint: Look carefully at the channels, avoid lengthy math.)
                                                      Coding & Information Theory
                                                      Homework No. 6 (due test

1. Source 키phabet고｝ 각 syn小이이 다음과 같이 주어질 때， 각각에 대하여 binary Huffman code와 binaiy

Shannon下ano code를 구성하고 average length를 구하라．

               =   {s1,s2,s3,s4,s5,s6}
                                     끄         끄           끄                    P
                                                                                                        l W
                            刃
      IS
                           l 3      l 4       l 6         l 9                  l万
(a)
                           寸        H         H
                                                  =       小




           S   =               s2,s3,s4,s5}
                                                   P4          P
                                                                                l 9
                    {s1,
                 1        1
                                                  l 9         l 9
(b)
                                                                           =
           Pi 二二:," P2 ' :'P3 =
                                                  1           H                 小
                                                                           =
           "     3 "' 二 3 "
                                                                           ＼
                                                                           나
           S   =   {s1,        s2,s3,s4,s5,s6,s7}
(c)
                           1        1         1            1                         1           1           1
           0' == : .O, = -.P3 = : .".刀 = m.=.' 'i75 = :                                ,' 끄6 == =1,' i'兀' = 二H
           "               2 '"     4 '"      8' 斗        16 ' "                    32 ' "      64 " ' 64
2. Second order Markov process




(a) Find the conditional probability of each state.

(b) Find the probability of equilibrium state.


(c) Find 瓦（S k 'I，옥, )

(d) Find the Entropy given Markov process.

3. Show that the Shannon-Fano Theorem is satisfied by all arbitrary radix-r


                                                                  urn三쁘＝                 //   ,   (S)
                                                                  n-*a)        fl

4. The conditional mutual information of two partitions A and B assuming C is by definition

                                        I (A万 IC) 나n川 C) +H田IC卜月（A · 히 C)


       (a) Show that

                                                       I (A万 IC) = I (A万 · C) - ／似C)
       (b) From (a) it follows that I (A, B . C) > I (A, C) interpret this inequality in terms of

the subjective notion of mutual information.
