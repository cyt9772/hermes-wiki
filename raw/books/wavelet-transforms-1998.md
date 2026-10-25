---
source_url: /run/media/yutae/Data/Wavelet_Transforms.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 203930cd3f4218f17a452c49017df1b6f3fa0a0d50cef2972c7d9cc71548dc09
---
# Wavelet Transforms: Introduction to Theory and Applications (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출 (~701,090 chars). 일부 토큰은 인식 오류로 깨짐 (한/영 혼용 OCR 산출). 원문 PDF(`books/Wavelet_Transforms.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Wavelet Transforms: Introduction to Theory and Applications
- authors: Raghveer M. Rao, Ajit S. Bopardikar
- edition: 1st
- year: 1998 (first printing July 1998)
- publisher: Addison-Wesley Longman, Inc. (Reading / Harlow / Menlo Park)
- pages: 322 (pdfinfo)
- isbn: 0-201-63463-5
+ source file: `Wavelet_Transforms.pdf` (sha256: `203930cd3f4218f1…`)
+ extract: `pdftotext -layout` @ 2026-10-25, 701,090 chars

## Chapter structure (from TOC)
| # | topic | page |
|---|-------|------|
| 1 | Continuous Wavelet Transform — correlation/operator view, inverse CWT | 1 |
| 2 | DWT & Orthogonal Wavelet Decomposition — MRA, Haar, MRA examples | 25 |
| 3 | MRA, Orthonormal Wavelets & Filter Banks — Daubechies D4, PRQMF | 51 |
| 4 | Alternative Wavelet Representations — biorthogonal, nonseparable, wavelet packets | 95 |
| 5 | Wavelet Transform & Data Compression — DTWT image/audio, JPEG comparison | 133 |
| 6 | Other Applications — denoising, speckle, edge detection, image fusion, comm | 183 |
| 7 | Advanced Topics — CWT revisited, lifting, bandlimited biorthogonal, PRCC | 219 |
| A | Appendix: Fundamentals of Multirate Systems (noble identities) | ~285 |

## Original text (all 323 pages)

Wavelet Transforms
          Wavelet
         Tran針orms

Introduction to Theory
   and Applications



         R（그ghuveer F＼기． Rao
                             and

           Aj汁 S. B야兀r(批（아




                              A
                             VT
                     ADDISON-WESLEY
         An Imprint of Addison Wesley Lon凹llan, Inc.
Reading, Massachusetts . Harlow, England 1 Menlo P缸k, California
       Berkeley, California 1 Don Mills, Ontario 1 Sydney
           Bonn 1 Amsterdam 1 Tokyo 1 Mexico City
MATLAB and Simulink are registered trademarks of The MathWorks, Inc. For information,
please contact:
    The MathWorks, Inc.
    24 Prime Park Way
    Natick, MA 01760-1500
    Phone: (508) 647-7000
    Fax: (508) 647-7001
    E-mail: info@mathworks.com
    w八／w.mathworks.com
Many of the designations used by manufacturers and sellers to distinguish their products are
claimed as trademarks. Where those designations appear in this book, and Addison Wesley
Longman, Inc. was aware of a trademark claim, the designations have been printed in initial
capital letters or all capital letters.
The authors and publisher have taken care in preparation of this book, but make no expressed
or implied warranty of any kind and assume no responsibility for errors or omissions. No
liability is assumed for incidental or consequential damages in connection with or arising out
of the use of the information or programs contained herein.
The publisher offers discounts on this book when ordered in quantity for special sales. For
more information please contact:
    Computer and Engineering Publishing Group
    Addison Wesley Longman, Inc.
    One Jacob Way
    Reading, Massachusetts 01867

Library of Congress C吐aloging-in-Publication Data
Rao, Raghuveer M.
    Wavelet transforms: introduction to theory and applications /
  Raghuveer M. Rao, Ajit S. Bopardikar.
         p. cm.
    Includes bibliographical references and index.
    ISBN 0-201-63463-5
    1. Wavelets (Mathematics) 2. Signal processing-Mathematics.
 I. Bopardikar, Ajit S. II. Title.
  QA403.3.R36 1998
  515'.2433-dc2l                                         98그2332
                                                              CIP

Copyright 匣） 1998 by Addison Wesley Longman, Inc.
All rights reserved. No part of this publication may be reproduced, stored in a retrieval
system, or transmitted, in any form, or by any means, electronic, mechanical, photocopying,
recording, or otherwise, without the prior written permission of the publisher. Printed in the
United States of America. Published simultaneously in Canada.
Cover image by Raghuveer M. Rao. Pseudocolor plot of the phase of the continuous wavelet
transform of a complex-valued random signal. Wavelet used: Mexican hat.
Text printed on recycled paper.

ISBN 0-201-63463-5
1 2 3 4 5 6 7 8 9- MA--0201009998
First printing, July 1998
To Chitra and Chirag whose love and
support made this possible, to Nikhil
who has brought new joy, and to my
              parents
       -Raghuveer M. Rao



To my parents and to the people with
  whom I have shared my dreams
       -Ajit S. Bopardikar
                                   CONTENTS




    Preface   xi


    Acknowledgments        xiii



1   CONTINUOUS WAVELET TRANSFORM 1
    1.1   Introduction I
    1.2   Continuous-Time Wavelets 1
    1.3   Definition of the CWT 3
    1.4   The CWT as a Correlation 8
    1.D   Lonstant ( -ractor rutering interpretation and i ime-lrequency Kesolution ii
    1.6   The CWT as an Orerator       19
    1.7   Inverse C叭T 20
    1.8   Problems 22



2   INTRODUCTION TO THE DISCRETE WAVELET TRANSFORM AND
    ORTHOGONAL WAVELET DECOMPOSITION 25
    2.1   Introduction 25
    2.2   Approximations of Vectors in Nested Linear
          Vector Subspaces 29
          2.2.1    Example of Approximating Vectors in Nested Subspaces of a
                   Finite-Dimensional Linear Vector Space 29
          2.2.2    Example of Approximating Vectors in Nested Subspaces of an
                   Infinite-Dimensional Linear Vector Space 31
    2.3   Example of an MRA       32
          2.3.1    Bases for the Approximation Subspaces and
                   Haar Scaling Function 35
          2.3.2    Bases for the Detail Subspaces and Haar Wavelet 36
          2.3.3    Digital Filter Implementation of the Haar Wavelet Decomposition 41
    2.4   Problems 50

                                             VII
Viii   Co／卄en朽

       3   MRA, ORTHONORMAL WAVELETS, AND THEIR RELATIONSHIP TO
           FILTER BANKS 51
           3.1   Introduction 51
           3.2   Formal Definition of an MRA        52
           3.3   Construction of a General Orthonormal MRA           53
                 3.3.1   Scaling Function and Subspaces         53
                 3.3.2   Implications of the Dilation Equation and Orthogonality     55
           3.4   AWa＼肥let Basis 幻r the 入4RA          58
                 3.4.1   Two口scale Relation 幻r 少（t)        59
                 3.4.2   Basis for the Detail Subspaces 61
                 3.4.3   Direct Sum Decomposition 63
           3.5   Digital Filtering Interpretation     64
                 3.5.1   Decomposition Filters 64
                 3.5.2   Reconstructing the Signal 68
           3.6   Examples of Orthogonal Basis-Generating Wavelets 70
                 3.6.1   Daubechies D4 Scaling Function and Wavelet       71
                 3.6.2   Bandlimited Wavelets       71
           3.7   Interpreting Orthonormal MRAs for Discrete-Time Signals       78
                 3.7.1   Continuous-Time MRA Interpretation for the DTWT        78
                 3.7.2   Discrete-Time MRA      79
                 3.7.3   Basis Functions for the DTWF 82
           3.8   Miscellaneous Issues Related to PRQMF Filter Banks       84
           3.9   Generating Scaling Functions and Wavelets from Filter Coefficients 89
           3.10 Problems 92


       4   ALTERNATIVE WAVELET REPRESENTATIONS 95
           4.1   Introduction 95
           4.2   Biorthogonal Wavelet Bases     95
           4.3   Filtering Relationship for Biorthogonal Filters 102
           4.4   Examples of Biorthogonal Scaling Functions
                 and Wavelets 104
           4.5   Tw아I汁Ti이好ional＼사avelets 109
           4.6   Nonseparable Multidimensional Wavelets 115
           4.7   Wavelet Packets 121
           4.8   Problems 126


       5   WAVELET TRANSFORM AND DATA COMPRESSION 133
           5.1   Introduction 133
           5.2   Transform Coding 142
                                                                               C（긔卄ents   ix

    5.3   DTWT for Image Compression 147
          5.3.1   Image Compression Using DTWT and Run-Length Encoding 149
          5.3.2   Embedded Tree Image Coding 151
          5.3.3   Comparison with JPEG 166
    5.4   Audio Compression 170
          5.4.1   Audio Masking 175
          5.4.2   Standards Specifying Subband Implementation:
                  ISO/MPEG Coding for Audio 177
          5.4.3   Wavelet-Based Audio Coding 178
    5.5   Video Coding Using Multiresolution Techniques: A Brief Introduction 181


6   OTHER APPLICATIONS OF WAVELET TRANSFORMS 183
    6.1   Introduction 183
    6.2   Wavelet Denoising 183
    6.3   Speckle Removal 189
    6.4   Edge Detection and Object Isolation 192
    6.5   Image Fusion 200
    6.6   Object Detection by Wavelet Transforms of Projections 204
    6.7   Communication Applications 208
          6.7.1   Scaling Functions as Signaling Pulses 208
          6.7.2   Discrete Wavelet Multitone Modulation 214


7   ADVANCED TOPICS 219
    7.1   Introduction 219
    7.2   C叭丁s Revisited 219
          7.2.1   Parseval's Identity for the C人／T 219
          7.2.2   Inverse CWT Is a Many-to-One Operation 220
          7.2.3  Wavelet Inner Product as a Projection Operation 222
    7.3   Bridging the Gap Between C叭／Ts and D八Ts 223
          7.3.1 CWT with an Orthonorrnal Basis-Generating Wavelet 223
          7.3.2   A Trous Algorithm 224
    7.4   Regularity and Convergence 229
    7.5   Daubechies Construction of Orthonormal Scaling Functions 232
    7.6   Bandlimited Biorthogonal Decomposition 236
          7.6.1   Scaling Function Pair Construction 241
          7.6.2   Wavelet Pair Construction 243
    7.7   Design and Selection of Wavelets 244
          7.7.1   The Lifting Scheme 244
x   C이卄en朽

             7.7.2   Best Basis Selection 248
             7.7.3   Wavelet Matching 250
      7.8    Perfect Reconstruction Circular Convolution Filter Banks   252
             7.8.1   Downsampling 252
             7.8.2   Upsampling 255
             7.8.3   Procedure for Implementation 255
             7.8.4   Conditions for Perfect Reconstruction 257
             7.8.5   Procedure for Constructing PRCC Filter Banks 258
      7.9    Interpolators Matched to the Input Process 259
             7.9.1   Interpolation Sampling 260
             7.9.2   Frequency-Sampled Implementation of Bandlimited DWTs 262
      7.10 The Scaling Operation and Self-Similar Signals         264
             7.10.1 LTI Systems and Eigenfunctions 264
             7.10.2 Continuous-Time Linear Scale-Invariant System 265
             7.10.3 Scaling in Discrete Time 268
             7.10.4 Discrete-Time LSI Systems         271


    A FUNDAMENTALS OF MULTIRATE SYSTEMS 279
      A.1 The Downsampler        279
      A.2 The Upsampler        280
      A.3 Noble Identities     282


    B LINEAR ALGEBRA AND VECTOR SPACES 285
      B.1 Brief Review of Vector Spaces         285
             B.1.1   Vector Subspace   286
             B.1.2   Linear Independence and Bases          286
      B.2    Inner Product Spaces    287
      B.3    Hulbert Space and Riesz Bases 288


      Bibliography     291

      Index    301
                                 PREFACE




The wavelet transform has been perhaps the most exciting development in the last
decade to bring together researchers in several different fields such as signal pro-
cessing,image processing,communications,computer science, and mathematics-to
name a few. This book provides an introduction to wavelet transform theory and
applications for engineers. The subject has been taught previously as part of several
of our graduate courses in the Electrical Engineering Department at the Rochester
Institute of Technology and is now being taught as a complete course. Most of the
students who take the course are working engineers from local industries such as
Eastman Kodak Company, Xerox Corporation, Harris, RF Communications, and so
on. A challenge in teaching this audience has been to cast the material in a lan-
guage familiar to engineers with a basic undergraduate degree while maintaining
accuracy and rigor. Over the years we have been able to develop an approach using
geometric analogies and filtering concepts to meet this challenge successfully. Our
students and colleagues have been urging us to write a book that adopts such an
                                                                                     to
approach because they find the material in the mathematically oriented books
 be daunting and inaccessible. We have endeavored    to keep  the presentatio n in line
with their exhortations.
   Application of the wavelet transform has almost come to be regarded as being
synonymous with data compression. So it should come as no surprise that we
have an extensive chapter on this application. However, there are properties of the
wavelet transform that make it naturally suited for application in many other areas.
It has been our desire for some time to bring out this fact. The reader will find a
detailed chapter devoted to such applications.
   The book starts off with a discussion of the continuous wavelet transform. This
is in keeping with the teaching approach in our classes. Rather than starting with
one or two chapters devoted to notation and basic material such as Fourier analy-
sis, the reader is led directly into the subject using basic linear filtering principles.
The wavelet transform is introduced in the context of reconstructing a signal from
the outputs of filters with impulse responses that are generated by dilation of a
single function. Chapter 2 introduces the basics of discrete wavelet transforms
and multiresolution analysis. The latter concept is first developed in the famil-
iar setting of linear vector spaces and Fourier series. The role of wavelets is then

                                           xi
Xii   Preface


      introduced through the Haar wavelet and piecewise constant approximations of
      signals. Chapter 3 considers multiresolution analysis based on orthogonal wavelet
      basis functions in greater detail. Subband filter bank implementations for signals
      and images as well as efficient implementation are discussed. Chapter 4 looks at al-
      ternative wavelet representations such as biorthogonal bases, wavelet packets, and
      multiresolution analysis of images. Chapter 5 provides a detailed treatment of the
      use of wavelet transform techniques in signal and image compression. In Chapter 6,
      wavelet transform application to areas such as denoising, object isolation, and de-
      tection are explained. Lastly, Chapter 7 treats several advanced topics. A question
      that arises often is which wavelet to choose in an application. Chapter 7 addresses
      this issue. It also deals with some of the latest research on generating wavelets and
      decompositions that are tailored specifically to meet certain objectives. Through-
      out the text, the presentation is patterned after what is usually found in electrical
      engineering texts and generally stays away from the "theorem-proof" model. The
      readers do not have to be familiar with real analysis or functional analysis. The con-
      cept of integration as dealt with traditionally in undergraduate engineering courses
      should suffice for understanding the material, and because it serves perfectly well in
      most applications, the attendant sacrifice in mathematical rigor should be of minor
      importance from a practical viewpoint. Problem sets are provided at the ends of
      Chapters 1 through 4. We also provide a disk with MATLAB routines that illustrate
      the concepts developed in the text.
                   ACKNOWLEDGMENTS




It is our pleasant task to acknowledge the help of many in making this book possible.
The book has been influenced considerably by the suggestions and work of B.S.
Adiga, Joseph Chapa, Sohail Dianat, Ajay Divakaran, and Wei Zhao. Sohail Dianat
and Ajay Divakaran were also part of the fine review panel assembled by Addison
Wesley Longman, the other members of which were Prashant Gandhi, Perry Li, and
Mike Sablatash. Our many thanks to them.
    Our thanks to the Electrical Engineering Department and the Center for Imaging
Science at the Rochester Institute of Technology for their support. We are indebted
to the many graduate and undergraduate students for their comments. Many others
have played a role in the creation of the book by providing us with opportu血ies
to present our research work, critiquing portions of the manuscript, being research
collaborators, making suggestions, and so forth. The following is our attempt to
list their names: Akram Aldroubi, Mark Alford, Peter Anderson, Richard Buck-
ley, V. Chander, George Cleetus, Roy Czernikowski, David Ferris, Wesley Foor,
Roger Gaborski, Joe Garcia, Mark Getbehead, Sebastian Gracias, Ed Hoefer, Lyman
Hurd, Shubha Kada끄abe, Anand Kannan, Thomas Kenney, Yogish Lavanis, James
LeBlanc, Ed Leiby, Jim Leone, Jingquan Li, Richard Lyons, George Mathews, Steven
McLaughlin, James Michaels, Terry Montonye, Dinesh Nadarajah, S.V. Narasimhan,
Colonel Nielsen, Kannan Panchapakesan, Paul Patti, Athina Petropulu, Majid Rab-
bani, P. Ravindra, V.U. Reddy, Harvey Rhody, Vincent Samar, Andreas Savakis,
Carl Schauffele, John Schott, N. Sitaram, M.K. Sridharan, Venkatesh Subramaniam,
Ken Swartz, Harold Szu, Brian Teller, Raman Unnikrishnan, Madhu Vairy, Xinran
Wang, Ted Wilcox, Paul Willson, Valerie Zelenty, and Michael Zoltowski.
    Finally, we thank Addison Wesley Longman for all their efforts. In particular,
Simon Yates came up with the idea, Tara Herries bore the brunt of the review
chores, and Lynn Merriam and Maureen Hurley saw the book through the final
 stages. Our heartfelt thanks to them.
                                               -Raghuveer Rao and Ajit Bopardikar

It is my pleasure to acknowledge gratefully the mentoring of Chrysostomos Nikias
early in my career. It has been a privilege and an honor to have received his
guidance.
                                                                -Raghuveer Rao
                               CHAPTER ONE


Continuous Wavelet Transform                      料7i




Li     Introduction
The beginnings of the wavelet transform as a specialized field can be traced to the
work of Grossman and Monlet [1984]. Their motivation in studying wavelet trans-
forms was provided by the fact that certain sei珊c gna1s can be modeled suitably
by com帥旽 translations and 軸喪嚼 臨夏駟ip'已砥ill計ory hi耐on 可 鈿ite du-
ration called a wavelet. The earf5? resiil[s We related to what is now known as the
continuous wavelet transform (CWT) [Grossman and Morlet 1984]. However, "wavelet
transformlike" expressions can be found in earlier work done in several fields such
as 凡nction representation, quantum mechanics, and signal processing.1 The inter-
est triggered by the work of Grossman, Monlet, and colleagues was sustained and
                                                                             ions and
niir ek蜘en connections were discovered bet毗en wavelet representat
devel6pfr? hts in other fields [Meyer 1993b]. For a historical account of the wavelet
transform the reader is referred to Meyer [1993b] and Daubechies [1996]. In this
 chapter we provide an introduction to CWFs and their properties.


1.2 Continuous-Time Wavelets
Consider a real or complex-value continuous-time function 少 (t) with the following
properties [Daubechies 1988; Grossman and Morlet 1984]:

  1. The f끄lction integrates to zero:


                                            J
                                                too砂(t)dt
                                                  。。        =   0.
                                                                                                 (1.1)


lThe term wavelet can also be found in the seismic signal processing literature in a context other than
the wavelet transform (see Stone [1984]).

                                                       1
    2          Continuous Wave/el Transform




                   디gure ] .1 The cut기（二 B-spine 낚／（그＼,elet.



               2. It is square integrable or, equivalently, has
                                                                                              finite energy:

                                                                    /
                                                                    I. 야）

                                                                             I
                                                                                 '
                                                                                     (t)
                                                                                           I2dt <的.             (1.2)
                                                                   .' H 00



         The function 砂 (t) is a mother wavelet or wavelet
겅의 二＞                                                        if it satisfies these two properties
         as well as the admissibft吐＼/ condition defined later in
                                                                     this chapter. While the ad-
                i y conditioni拍            in             a simple            ' wavelet transform,
        miss
                                           eful
                                                     formulating
        prop tis 1 and 2 suffice to define the CWT, and they
                                                                                                      inverse
                                                                      capture essentially the rea-
        Sons for calling the function a wavelet. Property
                                                             2 implies that most of the energy
        in 少 (t) is confined to a finite duration. Property 1 is sugge
                                                                        stive of a function that is
        oscillatory or that has a wavy appearance.2 Thus, in contra
                                                                          st to a sinusoidal func-
        tion, it is a "small wave" or a wavelet. The two prope
                                                                    rties are easily satisfied and
        there is an infinity of functions that qualify as mother
                                                                     wavelets. Figure 1.1 shows
        the plot of a wavelet called the cubic B-spline wavelet.
                                                                 This particular wavelet is sup-
        ported compactly. In other words, the entire wavelet has a finite
                                                                               duration: 0 5 r 5 4
        sec. However, it is possible to have wavelets that
                                                             are not supported compactly. For

        2 A function does not necessarily have to
                                                    oscillate to satisfy this property.
                                                                           De丹n川onoftheCWT     3



                 j

               0.8

               0.6

               0.4

               0.2
       e(t)
                 0                         \J
                                                                   V
              -0.2

               0.4

              -0.6
                                                       1       1

              -0.8
                     15   -10       5                      0           5   10     15
                                                           r



    Figure 1.2 The Monet wovelet.



example, a Moniet wavelet, which is constructed by modulating a sinusoidal function
by a Gaussian function [Daubechies 1990; Vetterli and Kovacevic 1995], is a wavelet
of infinite duration. But most of the energy in this wavelet is confined to a finite
interval. 恥r instance, consider the real-va岫 必뗐雙J쁘뜨le르

                                                                                       (1.3)
                            『小e_ t' cos         （亡y）
                                                                       ·




Its plot is shown in Figure 1.2. More than 99% of the total energy of the function is
contained in the interval tI <2.5 sec.


1.3 Definition of the CWT
                                                     下쿄｝표示 ttt呻 )
Let f (t) be any square  integrable  function. The   CWT or continuous-time wavelet
transform of f (t) with respect to a wavelet 少 (t) is defined as (三 stands for is defined
as) [Grossman and Morlet 1984; Daubechies 1992]

                                    ／以그  I    . /i 1 b\
                          W@?, b) 三 / 八D=＝少' 1 4:1 卜／t                                 (1.4)
                            .1.
                                \ J  -00
                                        v iai   \ a j

                          ？能 由匕싸耐'叭）
4    Continuous Wave/at Transform

     where a and b are real and * denotes complex conjugation. Thus, the wavelet
     transform is a function of two variables. Observe that both f (t) and 少 (t) belong
     to L2(R), the set of square integrable functions, also called the set of energy
                                                                                     signals
     [Couch 1997]. Equation 1.4 can be written in a more compact form by
                                                                                   defining
     少a,b (t) as


                                         蜘（『）
                                            ：出『（升'"도"                                             (1.5)

     Then, combining Equations 1.4 and 1.5,                                           曳
                                        W(a,b) f 0 f(t)呪，b(t) dt. : ,,.j *.,9W/
                                        W(.,5)=/0                                             (1.6)

    Notice that

                                                              少1,o(t) == 砂（t).              (1.7)

      The normalizing factor of 1/..J a ensures that the energy stays the same for all a
    and b; that is,



                                    -
                                        00
                                        。。   仇
                                                 ，
                                                     b的工的12
                                                                                      dt
                                                                                            (1.
                                                                                                    8)
     for all a and b. For any given value of a, the function 砂a,b(t) is a shift of 砂a,0(t)
     by an amount b along the time axis. Thus, the variable b represents time shift or
    franslation. From

                                                         I   /t\
                                             砂口，o(t) = =＝砂 1 寸 1                            (1.9)
                                                       \/ I기 \a/
    it f毗ws t岫而,（小sat如e-scaled 如帥帥叱e-蜘出 小on可 砂（t). Since
    a aetermines tne amount or time scaling or auation, it is rererrea to as tne scaie or
    dilation variable. Figure 1.3 shows two dilations of the Morlet wavelet. If a > 1,
    世브르主크흐旦必9t翅g延丑잊긋地gJ奴地埃只毖邑쁘畦9a映K낫火人工且唯起多쿄
    contraction of 砂 (t). Negative values of a result in a time reversal in combination
    wun culanon. since tne L vv i is generatea using auates ana transiates or tne singie
    function 少(t), the wavelet for the transform is referred to as the mother wavelet.

    Example 1.1
         Let the mother wavelet be

                                                1             1       05t< 2     1/
                                        少（D= i Hl                     I/ 25t< 1            (1.10)
                                             ( 0                      otherwise
                                                                      De丹nition of the （아VT   5




                       a = 1/2




           0.5




          -0.5




           -   I   尸
                                                                                     (A)
                          -10      -5           0          5         10         15
                                                r




      \    0.8           a= 3

           0.6

           0.4

           0.2




          -0.2

          -0.4

          -0.6

          -0.8
                                                                                     (B)
                1
               -15         -10     -5           0           5         10        15
                                                    r



Figure 1.3 A Monet wavelet dilated by factors of a = 1/2 (A) and a = 3 (B).
6   Con月nu이.jsW（그velet Transform

         This wavelet, called the Haar wavelet [Daubechies 1988,
                                                                 19921, is piecewise continuous
         and is discussed in more detail in Chapter 2. Using this
                                                                  wavelet, we find the CWT of
         the piecewise continuous function



                                         f(t) =
                                                                !!
                                                                                                          O.
                                                                                                                   15t<
                                                                                                                                          .
                                                                1U
                                                                 tJ                                       Otller1Vise.
                                                                                                          otnerw  lS

         We find the CWT separately for positive and negative values
                                                                                                                                                              of a. For a > 0,



                            砂ab(t) = i el/Va
                                            1 1/Vi                                                       b 5 t <b +a/2
                                                                                                         b + 口／2 드 t < b + 口                                                      (1.12)
                                     1     0                                                             otherwise.

        Using the unit step function,



                                                           三
                                                                                !I                                 t> 0
                                                                                                                                                                                  (1.13)
                                                                                                                   /<0.
                                                 (t)
                                            u
                                                                                      [U
        Equation 1.12 can be written as


                               1 1                                                                   /                                    a\                     그
                    九，b(t) =7計" (t -끼＝" 寸卜키＋"（卜b " )]'                                                                                                                           (1.14)

        Because f (t) is zero outside the interval 0 드 t <1,
                                                                                                                                                   its CWT is given by



                                        W(a, b) = J。'                                      I
                                                                                                                   a,      b
                                                                                                                                (t)
                                                                                                                                          di.                                    (1.15)

        Substituting Equation 1.14 in Equation 1.15 we have



                                                                                                                                                                                 (1.16)
                                   W(a, b)             =
                                                                 士
                                                                                               ［71
                                                                                                               -
                                                                                                                               2/2 + /31

       ＼人／
         here



                                   '1
                                        三

                                                                                                     b) di

                                                  j
                                                A1
                                                            u              (t
                                                                                           -




                                        :
                                   '2
                                   72                  。
                                                       a! " u
                                                            0
                                                                                (7．
                                                                                (t_
                                                                                                         》
                                                                                                         b_
                                                                                                                                  a
                                                                                                                                      )
                                                                                                                                      "       di
                                                                                                                                                                                 (1.17)



                                   13            j     'U            (t.
                                                                                                     b
                                                                                                                          a)
                                                                                                                                      dt.
                                                                                                               De加1!加a of the （가4／了    7




          {
On evaluating the integrals we find


                                     m
                                     l
                                                                 b< 0
                     n                           l       b                                                                   (1.18)
   H
  1 H
                                                                 0< b< 1
                                                     0
                                                                 b> 1




                                                         {
                                                                                              2
                                I
                                                                          -    b<
                                                                                        -a/
                                11
                     /2   =                      卜
                                                         （b＋     口／
                                                                      2)          2드b드1
                                                                                -口／
                                                                                                  -   a/
                                                                                                           2                 (1.19)
                                (0                                             b> 1- a/2
                                                 m
                                                 l
                                                                              b < -a
                                    0
                                +
                                l月=      )
                                                          b           n
                                                                              -a <b < 1 - a                                  (1.20)
                                (
                                \
                     13
                                     1


                                             /
                                                                              b > I - a.



   Let us now obtain the CWT by computing W(a, b) as a function of b for different
values of a. Observe that associated with the expression for each of Ii, '2, and 13 in
Equations 1.18, 1.19, and 1.20 respectively, there is a pair of values of b at which the
expression changes. These are 0 and 1 for Ii, -a/2 and卜 a/2 for '2, and -a and 1 - a
for 13. In substituting these back into Equation 1.16, these six values have to be taken
into account because the expression for W(a, b) (for a given a) will change as b (which
goes from -以그 to 以）) crosses these values.
   For 0 <a < i, we have -a < -a/2 < 0 < I - a < 1 - a/2 < 1. Therefore,




                                                                 뇨去뇨多
                                                                               b < -a
                                                                               -a 5 b 5 -a/2
                                                                               -a/2 <b 드 0
                          W(a, b) =                                            0 < b < 1- 口                                   (1.21)
                                                                               1- a <b 5 1- a/2
                                                                               1- a/2 5 b 드 1
                                                             0                 b> 1.


        For I <a <2, we have -a < -a/2 < 1- a < 0 < 1- a/2 <1. Thus, over this range,


                                                                 0                    b < -a
                                                                    佃＋b)
                                                                 H二石叫                 -a 5 b 드 -a/2
                                                                  b
                                                              ；石                      -a/2 <b 드 1 놔 口
                                                                 n＋乃-1                                                        (1.22)
                              W (a, b) = t                          \/a
                                                                                      I 中a < b < 0
                                                                 a+b-1
                                                                                      0< b 드 1 - a/2
                                                                   \/;
                                                                 1-b
                                                                 二百                   I- 口／2 드 b< I
                                                                 0                    b> 1.
8    Continuous Wave/et Transform

              Finally, for a > 2, we have -a <1 - a <-a/ 2 < 1 - a/2 <0 < 1, which yields




                                                                          0분孕＝區
                                                                              而0
                                                                                       b ＜二 -a
                                                                                       크i < b << 1- 口
                                                                                       1 나i 5 b 5 m口／2
                                1끼a, b) ==                                             -a/2 <b <1 - a/2              (1.23)
                                                                                       1- 口／2 드 b< 0
                                                                                       0 ＜二 1
                                                                                       b> 1.

              For a <0 we find that

                                      1 r              /       口\
                      t少n h(t) = ---= I u(t - b) - 2u It - b - = I + u(t - b - a) ]I .                               (1.24)
                       '   "       i/ -aL 5           \        2!               'I                                        S

           Going through the integration as in the case of a > 0 we find that (see Problem 9 at
           the end of this chapter)

                                                       w（口，b) = 卞w（寸a, 1- b).                                        (1.25)

             Figure 1.4 shows a contour plot of I W(a. b기2. The svmmtrv given by Eauation
          i.zD is capturea ry tne plot. 4i ne quantity W (a, b) 느 is cailea tne caIo2ram Of I 잎. I lIe
          J     ons of peaks in a scalqgram provide information about the positions and duration
          of events in the original signal. For a two-dimensional function such as an image, this
          property corresponds to the ability of the CWT to provide information regarding the
          location and size of an object in the image. The CWT for this example approaches
                                                                                                zero
          as a 수 0 and also as a -3 士oo (see Problem 3).
             As this example shows, it is difficult to obtain a closed-form expression for the
          CWT even for simple functions and wavelets. Therefore, we typically use numerical
          aigoritnms to nna waveiet transtorms.                                                    -


    1.4 The CWTasaCorre伯t伯n
    We now provide an interpretation of the CWT that has a bearing on its application
    in areas such as pattern detection and classification. The set of square integrable
    functions forms a linear vector space under addition and scalar multiplication.3 Fur-
    thermore, this vector space comes with a well-defined inner product. Given two
    finite energy signals x(t) and y(t), their inner product, denoted by (x(t), y(t)), is
    얹yen by



                                    仁（!
                                    (x
                                         (
                                             t)
                                                  )，
                                                       ,   『
                                                           y
                                                               （!
                                                               (
                                                                    t)
                                                                         ))   =
                                                                              =
                                                                                  Jpoo
                                                                                   -
                                                                                         x
                                                                                             (t)
                                                                                                   y*
                                                                                                        (t)
                                                                                                              dt.   (1.26)

    3See Appendix B and [Hoffman and Kunze 19711 for a discussion on vector spaces and related topics.
                                                                                                  The CWr as a Correlation      9




          Figure 1.4 Contour plot of W2(a, b) for Example 1.1.




     The total energy in x (t) is given by

                      \
                                                        /
                                                        i. 00
                                                                 Ix   (t)       I" di                                  (1.27)
                                                       1/ e （刃



                          V

which is 仁（t)，工' (t)). The square roo如f the energy is called the，끄凹如f4）        쏘ld巫
denoted by IIx(t) II [Hoffman and Kunze 1971].4 From Equation 1.26 we see that the
CWT is essentially a collection of inner products of a signal f (t) and the translated
and dilated wavelet 砂a,b(t) for all a and b:


                                                  W(口, b) = (f (t), 砂a.b(t))                                           (1.28)




'   This is   known
                              as the . L2 norm.
                                 With the inner          . and norm asproduct           defined
                                                                                                        the space of   square
inte旨ravie mncuons, L （八) rorms wnat is xnown as a i-in口en 斗及C已
10    Continuous Wavelet Transform

      The CWT has a cross-correlational interpretation as well. The cross-correlation
      R (t) of the two functions x(t) and y(t) is defined as




                     斟牡
                           R,
                                 ,(r)
                                          =   f   x
                                                      (t)
                                                            y   '
                                                                    (t
                                                                         -   r)
                                                                                  =   (x
                                                                                           (t)
                                                                                                 ,   y
                                                                                                         (t
                                                                                                              -   r)
                                                                                                                       )
                                                                                                                           (1.29)

     Jvhere t is the lag or shift parameter. Using Equations 1.5 and 1.9, Equation 1.28 can
     be written as

                                W(a, b) = (f (t), 仇,O(t - b)) = Ri,仇，。(b).                                                 (1.30)

     In other words, the C叭／T is the cross-correlation at lag b between f (t) and the
     wavelet dilated to scale factor a. Using the Cauchy-Schwarz inequality (see Ap-
     pendix B),

                                        1W（口, b)12 5 IIf (t川211仇, b(t)!12.                                                 (1.31)

     This in turn implies that W(a, b) always exists because the function and the wavelet
     have finite norms. Equality holds in this relation if and only if

                                                      砂口, b (t) = af (t )                                                  (1.32)

     for some scalar a. Therefore, if there actually is a pair of values (a, b) for which
     Equation 1.32 is satisfied, then the scalogram I W(a, b)I2 achieves its maxi尹lum at
     this pair of values. Even if Equation 1.32 is not satisfied, the position of the global
     maximum in the real part of W2(a, b) (which is the same as the scalogram when
     the wavelet is real-valued) provides a measure of the fit between f (t) and the
     corresponding 砂a,b(t), as explained next.
        A measure of the separation between f (t) and 砂a,b (t) is provided by II f (t) -
     少a,b(t)112. We have (see Problem 12),

                   llf (t) - 仇,沁川2 = IIf (t川2 + II砂口, b(t)II2 -2 Re[ W（口, b)}                                              (1.33)

     where ReE I stands for "real part of." Note that 砂a,b(t) is closest to f (t) for that
     value of the pair (a, b) for which the left-hand side is minimized. Of the quantities
     on the right-hand side, only ReF W(a, b)} varies with a and b (the term II仇, b(t)下 is
     a constant by Equation 1.8). Furthermore, it has a negative sign associated with it.
     끄L1封迦끄쯔如끄珥v갚쁘延쯔쁘女르끄 because it corresponds 的 the minimum
     value of the le作hand side, yields the va뇨es 可a and b
                                                                 that 쁘브쁘쁘르竺므)塾竝e
         ' " e 1etw-en f (t) and 少a,b(t).
        Similarly, working with Ii f t) +砂a, b (t) 112, which provides a measure of closeness
     between f (t) and 寸砂(t), we see that th르꼬迦地쁘廻쁘些쯔르蛔亡仁b)뇹坦峽多Jn中
                           Constant Q-Factor Filtering Interpretation and Time-Frequency Resolution                       11


瓷業黑絮냥喆讒群쀼然黑喆醬喆읊齧齬읊然名
and translated (and possibly negated) version of the mother wavelet and the input
signal f (t). Local maxima usually disclose local features in the signal that correlate
well with the wavelet for values of dilation and shift corresponding to the location
of such maxima.


1.5 Constant Q-Factor Filtering Interpretation and
    Time-다equency Re＄이네ion
The C＼人／T offers, 如止an立挺옛餌4．匙lectivity; that is, it is able to localize events
both in time and in frequency. Its ability to localize events in time is easy to establish.
The segment of f (t) that influences the value of W(a, b) for any (a, b) is that stretch
of f (t) that coincides with the interval over which 砂a,b(t) has the bulk of its energy.
This windowing effect results in the time selectivity of the CWT.
   The frequency selectivity of the CWT is explained using its interpretation as a
collection of linear, time-invariant filters with impulse responses that are dilations
of the mo出er wavelet reflected about the time ax奴 璵프쁘쁘甦四쁘旦奐뜨典르t
虹으匹契竺奭包쯔으2뜨쁘四皿쏘rO 덛g끈als 凹n be ex匹雙쁘르旦브크즈앤YQI!典m,
and the CWT was seen in Equation 1.30 to be a cross-correlation in b parameterized
by the scale factor a. Denoting the convolution of two signals hO') and x(t) by


                                    h(t)
                                          .!0)
                                    60) * x       (t)
                                                        :
                                                                J
                                                                I00
                                                                -
                                                                      h(r)x        (t
                                                                                               -   r)   dr    (1.34)

＼人／e have


                                        므느으三（b) 싼쿄-b).                                                        (1.35)
Thus, for any given a, the wavelet transform W(a, b) is the output of a filter with
hnDnlSe
US1l/        'es'x"se 小
      tt上1J드 1L口1八J11C八尸 甲口'. n
                              0 ''- "'  and illl)1lt
                                    Y ' 1t工.' Unt111 Jf \ "     b1e
                                                         ,-,J.. 1 뇨 h"  "e
                                                                    工111 V   11 C
                                                                           뇨 a     111工工11시肛11 'f
                                                                                 onir'끄lr'l
                                                                                1八／                6kerS Daran}=
                                                                                               1/1 1工工11口1느7 t/11二1111'
eterizea Dy tne scate ractor a.
   For the purpose of illustrating the frequency selectivity of the CWT let us choose
the 入tie工ican ／끄it 凹a叱let

                                                 少（t) = (1 中 2t2)e나'                                          (1.36)

which is obtained by taking the second derivative of the negative Gaussian function
_e_t2 /2. A plot of the wavelet is shown in Figure 1.5. Let 山(w) denote the Fourier
transform of 少(t):

                                            11
                                                 (w)        =   /：砂     (t)   e-
                                                                                        iwt.
                                                                                                               伍37)
12    Con升flu아is Wave/et Transto口）9



                     ]

                                                               \

                   0.5




                                                 \/
                    0




                 -0.5
                    -10                -
                                           5               0                 5                 10
                                                           i


             Figure 1.5 The Mexican hat wavelet,




         From the plot of 凹(w) 2 shown in Figure 1.6, it is seen that the wavelet is essen-
      tially a bandpass function (see Problem 13 for a definition of bandpass functions)
      with the Fourier transform magnitude centered5 at approximately 2 rad/sec. Since
      time reversal does not change the Fourier transform magnitude of a real-valued
     wavelet, Figure 1.6 applies to the frequency domain characterization of 砂(- t) as
     well. The 3-dB bandwidth, defined as the difference between the two frequencies
     on either side of the peak at which the squared magnitude of the Fourier transform
     is exactly half its peak value, is approximately 2 rad/sec, covering the band from
     I rad/sec to 3 rad/sec. This gives a Q-factor (ratio of the center frequency to fixe
     3-쁘些쁘쁘쁘）" 竺앴鉀苡更巫奭苾區五而示而.的而
                              「is小而nt


     bCentering here is not to be taken literally. The center frequency here refers to the frequency
                                                                                                     at which
     the Fourier transform magnitude attains its peak value.
     6 The term Q-factor is commonly used in assessing the quality of band rejection or the sharpness of
     response in tuning filtering applications such as broadcast reception. The higher the value of Q, the
     sharper the tuning.
                    Constant Q-Fac幻rF肝ering Interpretc材幻n and Time-Frequency Re＄이（片幻n       13




       Figure 1.6 Squared magnitude of the Founer transform of the Mexican
                  h아 니八그V쉬et.


with respect to wavelet dilation because

                                下［少(t人D] = I'小I' (aw)                             (1.38)

where F[ I denotes Fourier transformation. The center frequency of F[砂 (t/a)I for
any a is at 1/Ia I times the center frequency of the mother wavelet, and its 3-dB
bandwidth is also 1/lal times the 3-dB bandwidth of the mother wavelet, thus
yielding the same value for the Q-factor as before. Thus the continuum of filters to
which we alluded previously is actually a set of constant-Q bandpass filters. It is
this bandpass nature that gives rise to the frequency selectivity of the CWT.
   By virtue of the relationship in Equation 1.38 it follows that for a large value of a,
the associated filter has a frequency response centered at a low frequency value and,
therefore, the corresponding W(a, b), seen as a function of b for this fixed a, captures
the frequency content of f (t) around this low frequency. On the other hand, the
smaller the value of a, the more the bandpass shifts to a higher frequency, implying
that the CWT at small scales contains information about f (t) at the higher end
of its frequency spectrum. The squared frequency response magnitudes for three
different values of a for the Mexican hat wavelet are shown in Figure 1.7. Observe
 that as a increases, the frequency response shifts to the lower end of the spectrum
 with a corresponding shrinking of the bandwidth to maintain the constant Q-factor.
14   Continuous Wavelet Transform




           Figure 1.7 Squared magnitude frequency responses of a Mexican hat
                      way이et as a function of a. Here 吼佃）= 下（少口，0(Hr)).


     Example 1.2
         The combined effect of time and frequency localization is brought out in this example.
         Let

                                                        f (t) = f (t) + f2(t)                   (1.39)

         where

                                                                          100)   0. < t <. 10
                                f1(t) =
                                                 1sin
                                                                   (rt/
                                             1u                                  ounerwise

         and

                                                                          200)   5 <t <15
                                力（t) =
                                          !sin
                                                            (兀t/
                                          L0                                     otherwise.

         Thus f (t) is the sum of two truncated sine waves or tones of two different frequencies
         with a partial overlap in time. A plot of f (t) is shown in Figure 1.8. The scalogram
         of this signal obtained through the Mexican hat wavelet is shown in Figure 1.9 as an
         intensity map in which the darkness is proportional to the value of 1 W(a, b)已 Peaks
         occur in the scalogram for lower values of scale in the range 0 5 b 드 5 than for the
         range 10 5 b 5 15. This is a reflection of the fact that f (r) = f1(t) for 0 < t 드 5 and
                     （力nS幻nt Q-Fac幻rF肝e巾X키nte四re幻加n and 刀me-Frequency尸esolut/on                       15




    F勾바eli I가아 of f (t) 幻r Ex（그m히e 1 ,2.


     f (t) = f2(t) for 10 5 t 5 15. The frequency of f2(t) (1/400 Hz) is half the frequency of
     fi (t) (1/200 Hz), and there is an inverse relationship between the scale and frequency
     as shown in this section. Also, for the time interval 5 < t 드 10, f (t) is an addition of
     both fi (t) and f2(t), and for b in this range the scalogram shows this superposition by
     having significant values at scales corresponding to both frequencies. This illustrates
     the time and frequency selectivity properties of the CWT. Notice the spread in the
     peaks in both the a and b directions. The spreading in the b direction is attributed
     to the fact that 出』,1,(t) is spread out in time; that is, it is not confined to an infinitesi-
     mally small interval for values of (a, b) in the neighborhood of the peaks. The spread-
     ing in the a direction is similarly attributed to the fact that 'lI (w) is spread out in
     frequency, as seen in Figure 1.7.                                                          1


  It is not always possible for the CWT to resolve events in frequency. The same
holds true for resolving events in time. Quantitative metrics for time and fre-
quency resolution are based on the duration and bandwidth respectively of the mother
wavelet [Akansu and Haddad 1992]. The first moment of a mother wavelet 砂(t) is
given by [Akansu and Haddad 1992; Papoulis 1977]


                                    to 裝 ／므자沙 (t기2 dt
                                                                                            (1.40)
                                          t    ／甘(4，기2,/, ,
]6   （力nt/n山us Wavelet ／口ns幻rm




           디gure ].9 Sc이ogrart) 幻rExam힌e 1.2.



     Here 渺（이2,／戈 陟（奸 dt acts like a 까的abi胤y dens卿 func如n and, there佃e, t0
     provides a measure of where 砂 (t) is centered along the time axis. It is similarly pos-
     sible to locate the center of 山(w), the Fourier transform of 少 (t), along the frequency
     axis by taking its first moment


                                      ／戈이山佃기노CL)
                                                                                      (1.41)
                                    蜘＝ ／戈凹（w)I2 dw '

     A measure of the duration of the wavelet or the spread in time is given by [Akansu
     and Haddad 1992; Papoulis 1977]


                                        ／戈 (t - 匈거的平 dt
                                                                                      (1.42)
                                            ／戈 m（畔 dt          '

     The quantity under the radical sign is the second moment of the wavelet about to.
     This measure is known as the root mean square (RMS) duration. The RMS bandwidth
                    Constant Q-Factor Filtering Interpretation and TimeFrequency Resolution   17

of the wavelet is given similarly by


                                  ／툐佃 -o劤沁回2 dw
                                                                                    (1.43)
                                \   亡二 凹（w)I2 dw "

Fast decays in time and in frequency are required for the wavelet and its Fourier
transform to have finite values for the numerator integrals in the previous equations.
For functions that do not decay fast enough, alternative measures such as length of
interval with substantial energy (say, 95% of total energy) can be used.
   Let 스t少 and AnJ砂 be the RMS duration and bandwidth respectively of a mother
wavelet 砂（t). TheF小IS duration 可 its dilation 仇, 0(t) is then 스印(a) 三 k기스t砂． From
Equation 1.38, the corresponding RMS bandwidth is 스w砂 (a) 三 A(D少 /1a I. We have

                           스t少（a）八0)砂（a) = 스t少／\nV = C砂                             (1.44)

where c* is a constant. Thus, the product of the duration and the bandwidth is
invariant to dilation. Equation 1.44 indicates that decreasing 스i砂 (a) results in an
increase in 스w1, (a) and vice versa. The smaller the value of 스印 (a), the better the
ability of the CWT to resolve events closely spaced in time. Similarly, the smaller the
value of 스w,(a), the better the ability of the CWT to resolve events closely spaced
in frequency. At very small values of a, the CWT possesses good time resolution
(ability to separate very close events in time) because the RMS duration of the corre-
sponding dilated wavelet is small. However, the frequency resolution at such scales
is poor because the RMS bandwidth of the dilated wavelet is large. The opposite is
true for large values of a. Because of the reciprocal relationship between scale and
frequency, it also follows that the CWT provides better frequency resolution at the
lower end of the frequency spectrum and poorer resolution at the higher end of the
frequency spectrum. This ability to provide variable time-frequency resolution is a
hallmark of the wavelet transform. It makes the wavelet transform a natural tool
in the analysis of signals in which rapidly varying high-frequency components are
superimposed on slowly varying low-frequency components such as certain seismic
signals and music compositions.
    We have examined the effect of dilation on time and frequency resolution. How-
ever, the CWT involves translation of the wavelet as well. The translation parameter
b affects only the location of the wavelet and not the duration or bandwidth, which
are affected solely by the dilation, as shown next. The first moment and hence the
center of 少a,0(t) is at0, as verified by using Equation 1.40. Observe that if to 尹 0,
the location of 仇,0(t) depends on the value of a. The first moment of 砂a,b(t) is
at0 + b. However, the second moment of 砂a,b(t) about at0 + b is the same as the
second moment of 仇,0(t) about ato, indicating that the parameter b merely affects
 the location of the wavelet and not the RMS duration. The RMS bandwidth is also
18   Continuous Wavelet Transform

     not affected by b because translating a function does not affect the magnitude of its
     Fourier transform.
        The variation of time and frequency resolution as a function of a is shown graphi-
     cally using time-frequency cells, as shown in Figure 1.10. The center of each rectangle,
     obtained from the first moments in time and frequency, indicates the position of
     the wavelet in time and frequency, whereas the rectangle itself bounds the spread
     of the wavelet in time and frequency as characterized by the corresponding second
     moments. Given an event localized at some (T, Q) in the time-frequency plane, for
     any other event to be resolvable it should be localized in the time-frequency plane
     outside the bounding rectangle of the time-frequency cell at (T, 52). An alternative
     view is that associated with a time-frequency cell centered at (T, 52). There is an
     ambiguity in localizing events in time and frequency to within its bounding rect-
     angle. It follows from Equation 1.44 that the area of each bounding rectangle is
     c小 Because a decrease in the uncertainty of time localization is accompanied by
     an increase in the uncertainty of frequency localization (in other words, when the




       Figure 1.10 Time-frequency cells for 砂a.b(t) shown for a fixed b and three different
                   values of a. The mother wavelef and its Fourier transform are centered at
                   t0 and wo respectively.
                                                                       The CW了 as an Opera幻r        19


time-frequency cell is narrow in time it is wider in frequency) and vice versa, it is
not possible to reduce simultaneously the uncertainty in both dimensions. For this
reason, Equation 1.44 is called the uncertainty principle governing time-frequency
resolution.
   The constant c砂 in Equation 1.44 is a function of the wavelet used. A wavelet
with a smaller value of c砂 provides better simultaneous localization in the time-
frequency plane than one with a larger value. This follows from Equation 1.44.
How small can one make the time-bandwidth product of a function? It turns out
that the smallest time-bandwidth product is associated with the Gaussian function7


                                     f (t) = V2Jra
                                              =1I ／案                                      (1.45)


and is equal to 1/2 [Papoulis 19771. Therefore, the uncertainty principle can be
restated as

                                    A知（a）八0)砂（a) 三 1/2.                                   (1.46)


1.6 The CWT as an Operator
 The CWT takes a member of the set of square integrable functions of one real
 variable in L2(R) and transforms it to a member of the set of functions of two real
.yariables. Thus it can be seen as a mapping operator from L2(R) to the latter set.
 Define

                                     w砂［f (t)] 三 W(a力）.                                   (1.47)

Then W少 [ I is to be read "CWT with respect to 砂 (t) of." The notation for the
operator uses 砂 as a subscript to remind us of the fact that the transform depends
not only on the function f (t) but also on the mother wavelet. We now enumerate
various properties of the CWT using the operator notation:

    Linearity-

                         W11, Laf(t) ＋月g(t)1 =a끼7V,[f (t)1＋月끼2砂［g(t)]                     (1.48)

    for scalars a and 月 and functions f (t), g(t) E L2(R).


7The Gaussian function is not a wavelet. Why? Although we have defined the time-bandwidth product
in the context of wavelets, the definition applies to other types of functions as well.
20   Con升加印S 너／
              （그velet 了ransform


         Translation-
        ／尸＼八／ 八小／   /\mm




                                    W砂［f (t - T)] = W(a, b - t).                      (1.49)

         Scaling-
        ／入／入／\/\／八7



                                      r 1     i't\ 1       / a b\
                                  1'／少 1 누＝/ 1- J I = W ( TT ' j                      (1.50)
                                       LV (y \CXJJ      \LX (XJ

         for a > 0.

         Wavelet shifting-Let i (t) = 砂(t - r). Then

                                    .W[ f (t)J = W(a, b + at).                        (1.51)

         Observe that the CWT obtained by shifting the wavelet is different from the
         one obtained by shifting the signal.

         Wavelet scaling-Let      (t) = [r (t/ 川J可 . Then

                                       끼)寸［f(t)] = W(aa力）·                           (1.52)

         This result, which states that the new CWT is a scaled version of the original in
         the a variable, is not surprising because all dilations of the wavelet are actually
         used in obtaining the original CWT.

         Linear combination of wavelets- 코ven two wavelets 吻(t) and 吻(t), their
         linear combination a砂i(t) + 月砂2(t) for scalars a and 月 is also a wavelet. We have

                            끼／뇨吻＋月砂2 [f (t)] =a까7砂1[ f (t)1＋月）'V砂2[/ (i)].           (1.53)


     1.7 Inverse CWT
     Suppose W(a, b) = W少[ f (t)1 for some signal f (t) and wavelet 少(t). A natural
     question to pose is the following: Is it possible to go in the other direction? That
     is, given W(a, b), is it possible to obtain f (t)? In other words, does the CWT have
     an inverse? It is of particular interest to explore the possibility of an expression
     for the inverse transform that bears resemblance to the C人／T of f (t). An analogy
     is provided by the forward and inverse Fourier transforms. Their expressions are
     similar in that the exponential kernel appears in both transformations (the kernel
     in the inverse is the complex conjugate of the one in the forward transform). Is
     it similarly possible to devise an inverse CWT such that it involves translates and
     dilates of the mother wavelet? In fact, if this could be done we would then be able to
                                                                                            Inverse CW    21

interpret the wavelet transform as providing a weighting function for synthesizing
a given function f (t) from translates and dilates of the mother wavelet much as the
Fourier transform provides a weighting function for synthesizing a function from
sine and cosine functions. Fortunately, it is possible to construct such an expression.
If the mother wavelet satisfies the (sufficient) condition that


                                                                                                 (1.54)


and is such that 0 < C < no, then
                                                             cJ的 卄耐，他

                           i f （刃     I.的   ]                    \
                   f (t) = 二 I       I     -=W (a, 功仇. b(t) da db).                              (1.55)
                               =-oo Jb=-oo V기二                   1

The condition in Equation 1.54 is kn曲n as the 肋岫計bili勺 cond沮on on 砂（t) [Dau-
bechies 1990, 1992].
   We now proceed with the derivation of the previous result [Chapa 1995; Kaiser
1994]. Equation 1.35 expresses W(a, b) as the convolution of 1 (b) with 少a,O (- b). In
the frequency domain this becomes



                      f:   ,   W   (a,   b)e i0 db =   \面F    (w)   I1*   (aw)
                                                                                                 (1.56)


where F(w) and W (w) are the Fourier transforms of f (t) and 砂 (t) respectively.
Multiplying both sides of Equation 1.56 by 山(aw)/Ia 3/2 and integrating with respect
to a yields



   L-   /,:, 小m蜘0）
   /,:, L=   a    戶"mdb = F(w)Ja=
                              f:-, I'I'(aw)I
                                                                                       2
                                                                                           da.   (1.57)


It is easy to show that


                    /,:, I4'(：안' da= /,:-, 빠：
                                            ,)I' 如＝
                                                  【                                              (1.58)


where C is the constant from the admissibility condition. Thus,

                          1 !的           (00   1                                 . ,
               F回＝C/,+a:－的巨而W(a, b）山（口m)" ' "d口db.                                               (1.59)


   Taking the inverse Fourier transform on both sides of Equation 1.59, we get the
expression for the inverse CWT in Equation 1.55, which shows that W(a, b)/IaI2
provides the weighting function for constructing f (t) from 砂a, b (t)-the translates
22    Con卄加ous 너／Ovelet Transform

     and dilates of the mother wavelet. While we have let a take both positive and
     negative values in the CWT, it is possible to use only positive a if the wavelet is
     real-valued (see Problem 14).
        The admissibility condition stated here is a sufficient condition that leads to the
     expression in Equation 1.55. It is not a necessary condition to obtain a mapping from
     the set of CWTs back to L2 (R). Another important fact to note is that the range of
     the mapping W. is not the entire set of square integrable functions of two variables,
     but only a subset of it. This means that it is possible to have a function, say X(a, b),
     which when substituted for W(a, b) in Equation 1.55 yields a function, say x (t), such
     that W.[x (t)1 尹 X(a, b). Some of these issues are discussed again in Chapter 7.


     1.8 Problems
       1. Show that the Mexican hat wavelet satisfies the admissibility condition.8
       2. Using the Mexican hat wavelet, derive a closed-form expression for the CWT of the
          function
                                             /(7)                                       ,
                                                                                      ItI< 1
                                             f (t)
                                                     =
                                                                    (1
                                                     =         1.
                                                                         。            。therwise.
       3. Show that the CWT in Example 1.1 tends to 0 as a tends to 0 and as a tends to 士oo.
          Investigate whether this is generally true of CWTs.
       4. Suppose we obtain the function W(a, b) by putting f (t) = 8 (t), the unit impulse or Dirac
          delta function in Equation 1.4. Is this a valid CWT? What happens if Equation 1.55 is
          evaluated with this W(a, b)?
       5. Repeat Problem 4 with f (t) being a sinusoidal signal of arbitrary amplitude, frequency,
          and phase.
       6. Show that if W(a, b) = W,1,[f (t)] for a wavelet that satisfies the admissibility condition,
          then

                                  1If (t)II2＝二／,:, /,:, 삐二？)1'd。db.
          This is a generalization of Parseval's theorem to CWT.
       7. The CWT is often compared to another time-frequency representation-the short-time
          Fourier transform (or STFT)-which can be defined in a form similar to the CWT.



                                  87m  /(!)]：
                                  STFT[ f (t)I   「
                                                 F
                                                         (w,
                                                         （0,
                                                                         7)
                                                                         r)
                                                                              :/,OO
                                                                                                   J f (t)砂混
                                                                                                     ,         (t)
                                                                                                                     dt   (1.60)
         where 仇, 小） = w(t - t)e3mt. The function w(t) is a windowing function, the simplest of
         which is a rectangular window that has a unit value over a finite interval and is zero


     8 The authors thank Dr. Sohail Dianat for Problems I and 2.
                                                                                                               까아1en咨   23


   elsewhere. How do the time and frequency resolution of this transform compare with
   that of the CWT?
 8. Show that the Monlet wavelet does not satisfy the admissibility condition. Note: Even
    though it does not satisfy the admissibility condition, it is stifi possible to recover a
    signal from the CWT using what is called the Moniet algorithm instead of the inverse
    CWT expression in Equation 1.55 [Meyer 1993a].
 9. Obtain the wavelet transform of Example 1.1 for negative a and verify Equation 1.25.
10. Derive an expression for how the first moment of a wavelet 1/r ,(t) varies with the pa-
    rameters a and b. How does the first moment of the Fourier transform of 砂ab(t) vary
    with a and b? Discuss the implications of this on the wavelet and its ability to cover the
    time and frequency ranges.
11. Compute the time-bandwidth product for the Gaussian function given in Equation 1.45.
12. Show that the squared separation between f (t) and 仇b(t) is given by Equation 1.33.
                                                                                        to a
13. A function f (t) is a bandpass function if its Fourier transform F(w) is confined
    frequency interval w1 <   1w <  o2, where  WI  > 0 and  (o2 is finite. Is every bandpass
    function a wavelet?
14. Show that if 砂(t) is a real-value wavelet then a function f (t) can be recovered from its
    CWT W(a, b) as

                            /(,）근L Ja=O  fOo以그윽蜘
                                    /00 Jb＝   mI.-
                                                   , 功也,b(t) da db
    如町．나艸竿  加·,Wh叩n we not use this텬pre蜘耐the岫이．et프co呻，?.
         nas to ao witn tne symmetry oj tne 1-ourier rransyorm 'I' W) of tne wavetet
    1-lint: I tie answer
    about w = 0.
15. The problem in Example 1.1 has an alternative solution that leads to the same answer.
    Define
                                                                            0 r
                                                                                                        <
                                                                               m
                                                                               l
                                                                                                      <
                                                                                                       <
                                                                                                       H
                                                          10
                                         F(t) = 1 t                                1
                                                                            r0 r
                                                Li
                                                                                                       >
                                                                                                           1
     where f (t) is as in Equation 1.11. Then, show that the wavelet transform is

                                                         2F (b + 뜩）              F(b) 小 F(b+ a)
                           W (a, b)
                                      =sgn(a)                  '            '   V向                "

    Here, sgn(a) stands for the signum function defined as

                                                                                t< 0
                                                                                t> 0
                                              （,                        '
                                                                   LU           r= 0.
                                                   ）나；
                                         ，帥
     MATLAB9 routine cwtex distributed with this book uses this approach.


9MATLAB is a trademark of The MathWorks, Inc.
24   Continuous Wavelet Transform

        Tab旭 1.1 DI卜기F Sign（긔ing Code


                                                      Frequency (Hz)
           Signal       697       770       852          941      1209     1336       1477



                          X X X
               l
                                                                   x
               八
               乙
                                                                             x
               그
               口
                                                                                        x


                                    X X X
               4
               1
                                                                   x
               尸
               h
               口

               6
                                                                             x
                                                                                        x


                                              X X X
               n
               /

              8
                                                                   x
                                                                            x
              O
              /
                                                                                        x


                                                          X X X
              木 0
                                                                   x
                                                                            x
              뀨
              卄
                                                                                       x


     16. Touch-tone dialing on telephones uses what is known as dual-tone multifrequen
                                                                                                 cy
         (DTMF) signaling. Each key has a unique pair of frequencies associated with it. (See
          Table 1.1. The pair of frequencies for a given tone are indicated by an "X" in the cor-
         responding row.) Compute the scalogram of the DTMF signal. The DTMF sequence is
         provided on the disk included with this book as the file dtmf . way. This file can be read
         using the MATLAB command wavread. Experiment with different wavelets. Observe
         how the scalogram changes as the wavelet changes. Decode the tones in the signal from
         the scalogram. (Note: This was actually assigned as a classroom project at the Rochester
         Institute of Technology. The students found it useful to filter out the line noise before
         computing the scalogram.)
                          CHAPTER TWO


        Introduction to the
         Discrete Wavelet
     Transform and Orthogonal
      Wavelet Decomposition


2.1 Introduction
We saw in the previous chapter that the CWT maps a one-dimensional function
f (t) to a function W(a, b) of two continuous real variables a and b, which are the
wavelet dilation and translation respectively. The region of support of W(a, b) is
defined as the set of ordered pairs (a, b) for which W(a, b) 尹 0. In principle, the
region of support of a CWT is unbounded; that is, it can be the entire plane defined
by R2, the set of all ordered real pairs. This chapter introduces a type of wavelet
representation that has assumed considerable practical significance because of its
link to digital filtering [Daubechies 1988, 1992; Mallat 1989a, 1989b; Vaidyanathan
1992; Vetterli and Kovacevic 1995]. We take the approach of developing the under-
lying ideas entirely through an example involving the Haar wavelet. A more general
development is presented in Chapter 3.
    The CWT provides a redundant representation of the signal in the sense that the
entire support of W(a, b) need not be used to recover f (t). Consider the function
 f (t) with the Fourier transform given by

                                                          2 드 1n기 <3
                             F (w) = { 八                                       (2.1)
                             -         '   ,       Ii
                                   "               LU
                                                          otherwise.

Suppose we obtain the CWT of f (t) using the wavelet 砂 (t) with the Fourier trans-
form given by

                                                          I 드 Io기 <4
                             W
                                                   i 0 otherwise.              (2.2)
                                                    Ii
                                 (w)           =




                                                         25
26   ｛가screte 너／avelet Transform and O片h아刃n이 너／0velet Decori）尸osition


     Let W(a, b) be the resulting CWT and Wa (cv) its Fourier transform in the b variable
     so that


                                                                                           f:                                                            (2.3)


                                                                                                                          J
                                                             W。           (cv)                        ,   W(a, b)e ' " " " db.

     Because
                F[ ia,   "
                             (t)   ]   =   .,/j   "{   tIi
                                                                  (acv)               ,   we   have
                                                                                                                             2

                                                                                 吼回 =＼기可F（이山（a cv).                                                      (2.4)

     We now use Equation 2.4 to derive the region of support of W(a, b). Figure 2.1A
     shows a plot of F(cv) and Figure 2.IB shows a plot of 山(cv). From the fact that the
     support of W (cv) is 1 드 1cvi 드 4, it follows that the support of 山(aw) for a given a is
     1/ia I 5 ic가 드 4/laL Comparing this support with that of F(cv), we find that the two
     overlap only over the range 1/3 드 lal 드 2, which is illustrated in Figure 2.2. Thus
     the support of this CWT is restricted to that portion of R2 for which 1/3 드 al 드 2.
     However, we also see from Figure 2.2 that for 1/2 드 Ia < 4/3, the support of F(cv)
     is contained entirely within that of W (acv), and therefore

                                                  吼回 =／巨佃佃） 1/2 5 I기 드 4/3.                                                                              (2.5)

     From Equation 2.5 it is seen that F(cv) can be obtained from Wa (cv) or, equivalently,
     f (t) can be obtained from W(a, b) by a simple amplitude scaling of the latter for any
     fixed value of 口 in the range 1/2 5 k기 5 4/3 as F（口D = 吼回八厄 This indicates that
     it is not necessary to use the entire support of W(a, b) to reconstruct f (t). We have
     used a specific function and a specific wavelet to illustrate how redundancy arises
     in a CWT. However, it is possible to generalize the result to any CWT [Daubechies
     1992].
         In this chapter we introduce a type of nonredundant wavelet representation. In
     particular we look into a representation of the form

                                                                                 00        的


                                            f (t) = ＞二 ＞二 d(k, t)2_112砂（2 "t -t)1                                                                        (2.6)
                                                                          k=-o그 t= -oo



        Observe that in contrast to Equation 1.55, which involves a continuum of dila-
     tions and translations, Equation 2.6珽es discrete values for these parameters. The
     J ．·］八1: 八小 1八1_ 八n 1！八1.. 八n 八r 1lm ,1 r八1m小m /r n次 ! . !l4 八14八 1r ：』m -.                                               八斗八mm    A 1 八141! 1:1八1：八1m n丸
     났쁘끈프끄［ La八e> V (lIUC> UI LILe IUIIlL ei -; 二） WILeI亡 人 I:) a                                                          IILLe,eI "   八L airy LIII(lLIUIL 乙 /

     ti百區쁘쁘四，       P筵쁘쯔自takes滋后石f the幻r 2切 hereZ is again an integer.
     The values d(k, Z) are related to values of the wavelet transform W(a, b) = W[ f (t)]
     at a = 2" and b = 2"1. This corresponds to sampling the coordinates (a, b) on a
     grid such as the one shown in Figure 2.3. ( This process is called dyadic sampling
                                                                                        Introduction   27



                    1.5




             F(w)


                    0.5




                                                                                  (A)
                                  1。
                                       5   -3- 2      0      2   3       5   10
                         -0
                                                      U)




                    1.        5




             甲他）


                    0.5




                                                                                  (B)
                          -0      1。       4       --1 0 I           4       10
                                                      U)




        Figure 2.1 Fourier 卄ansf가m of a 針gn기 (A) and a way이et (B).




because consecutive values of the discrete scales as well as the corresponding sam-
pling intervals differ by a factor of two. The two-dimensional sequence d(k. t) is
commonly referred to, as the discrete wavelet transform (DWT) of f (t) [Daubechies
1992; Vetterli and Kovacevic 1995]. Observe that the DWT is still the transform of
a continuous-time signal. The discretization is only in the a and b variables. In this
sense it is analogous to the Fourier series, which involves a discrete frequency do-
main representation of a (periodic) continuous-time signal. For this reason the DWT
28   Discre旭 너／ave/et Transform an（六：가IM7ona/ 너／아이et Decc가까兀硼on




         Figure 2.2 Oven（캬＞ of Fourier transforms c寸 the 針gn이 （그nd （켸아ed ＼사（그＼,elets.




        Figure 2.3 The time-frequency cells that correspond to dyadic sampling
                               Approximations of Vectors in Nested Linear Vector Subspaces   29

has also been referred to as a continuous-time wavelet series [Rioul and Duhamel
1992; Vetterli and Kovacevic 19951. The description and derivation of the DWT is
developed here entirely through an example involving the Haar wavelet as defined
in Chapter 1. This is a precursor to descriptions of the DWT developed in a more
general context in Chapter 3.


2.2 Approximations of Vectors in Nested Linear
    Vector Subspaces
Rer'resentations such as the one in Eciuation 2.6 arise naturally in the context of what
is called꾼｝쁘밧雙얀뜨뜨으프쁘包逃廻브쁘프y, wrucn essenti카玎 amounts to constructing
a hierarchy of approximations to functions in various subspaces of a linear vector
space [Daubechies 1988; Mallat 1989a, 1989b1. We explain the concept of approx-
imating vectors in nested subspaces by going through examples involving simple,
familiar linear vector spaces before establishing the link between MRAs and DWTs.


2.2.1 Example of Approximating Vectors in Nested Subspaces of
      a Finite-Dimensional Linear Vector Space
Consider the set of all N-dimensional, real-valued vectors of the form x = [工i, x2. . . ..
工NI· 끄虹熙．t..fo恥．5 캣쏘d坦쁘嶝雙｝赴塑쁘rv뜨奴J匙筵匙르楚望으魃丑迪
e叫y indepe叩앤t (i奴 necessar匈 ortho肥nal) basis vect毗 카, a각· ·二크迂쁘生쁘少
any vector in this space can be expressed as a linear combination of these上a-
             【小， tI否誌쿄t unique 吼al町5 a:，吻，···，XN such th毗
重廷臾프트 in 。藻；二.
X = a1a1 + a2a2 + . . . + aNaN. Let us call this N-dimensional vector space VN. We
next look at approximating vectors in this N-dimensional space by vectors in a sub-
space of a lower dimension. Suppose we generate all linear combinations of just
N - 1 of the N basis vectors, say a1, a2. . ...aN_i. The set of all such linear combi-
nations is also a vector space. It is of dimension N 口 and every vector in it also
lies in VN. It is thus a vector subspace of VN. Let us call this VN_i. By continuing
to drop the last basis vector at every step, we can similarly construct subspaces
 VN_2. ... .V1 of dimensions N - 2. ....I respectively. The subspace Vi has as its
basis the single vector a1. These vector spaces form a nested sequence of subspaces,
 V1c1今 C . . . （二 VN.                                                "
   Suppose we want to      approximate   a vector x in VN by   a vector in VN_1. The
best possible approximation in the minimum mean-squared error or least squares
sense is made by choosing that vector (say XN-1) in VN_i for which the length of
the error vector eN_i = x - XN-1 is minimized. Such a vector is obtained by solving
幻r eN_i in

                                      (eN_i, ak) = 0                                 (2.7)
30    Discrete Wavelet Transform and Orthogonal Wavelet Decomposition




              Figure 2.4 디nding the bes十 （짜）口roxim（그ting vect아1（그 georr기etric analogy



       where k = 1, 2. . . . .N - 1. To give a geometric analogy, XN-1 is the vector obtained
      by dropping a perpendicular from x to VN_1 as illustrated in Figure 2.4. The vector
       XN-1 is called the orthogonal projec如n of x on VN_1. The error vector eN. i is
       orthogonal; that is, it is at "right angles" to every vector in VN_1.
          Suppose we now continue this process of projecting throughout the entire se-
      quence of subspaces by projecting XN-1 on VN_2 to yield XN-2, and so on. At the
      end of the process we have a sequence of orthogonal projections of x in the sub-
      spaces VN_1, VN_2, . . ., Vi. These are XN-1, XN-2. . . . .Xi respectively. Note that an
      approximating vector Xk is the orthogonal projection of not on!y Xk+1 but also of
     .the vectors Xk-I-2, ..., XN-i and x on Vk. With XN = X let

                                          ek = Xk+1 - Xk                                (2.8)

      for k = I. .. ..N - I, denote the error between the projections on successive sub-
      spaces. Looking at the projections as approximations to the original vector x, we
      would expect the quality of the approximation either to stay the same or to get
      worse as we go from XN-1 to Xi. Another way of stating this is that the subspace
      VN_11 contains the finest approximations to vectors in VN whereas Vi contains the
     coarsest approximations. ！迦크얏 of break迪·브얀쁘크므쁘or into such a hierarcF沙
     으뜨22뜨쯔쁘브竺쁘쁘쯔표唯j匙共立J匹R血
         The sequence of error vectors eN_i. . . . .e1 also has an interpretation. The vector
     eN_i can be seen as the amount of "detail" that is lost in x in going to its
                                                                                     approx-
     imation XN-1 because x寸 帥-1 = 枷-1· 工뇨坦르쁘1흔뜨些敭9珥毁血으恥hat vector
     쁘쁘쁘뜨프J且씻型나雙앗트욘빳프으쁘프如琶쁘1曳地_ . L雙쁘c쁘프唯그旦劈or
     三2旦뜨廻死꼬 The dimension of V匕y_i is one. We say that VN_1 and WN_1 are orthog-
     onal to each other. Furthermore, since any vector in VN can be expressed as the sum
     of a vector in VN卞1 and a vector in WN_1, we call these subspaces the orthogonal
     complements of each other in VN. Similarly, eN_2 is the detail lost in XN-i in going
     to the latter's approximation XN-2 in VN_2, and it comes from the one-dimensional
     subspace WN_2, which consists of all vectors in VN_1 that are orthogonal to VN_2.
                                       A아roxima加ns of Vec幻rs in Nested Linear Vec幻r Sub羽（ices              31


In general, the error vector at any level can be seen as the detail that is lost in
going from a finer to a coarser level or, alternatively, as the detail to be added to
an approximation at one level to move up to a finer level.
   The vectors eN_i, eN_2, . . . , e1, Xi form an orthogonal set; that is. the inner prod-
uct of any pair of these is zero. They belong to the one-dimensional subspaces
 WN_1, WN_2. . . . .W1, and V1 respectively. Moreover,


                                   x= eN_1+ eN_2+ . . .+ei+             X1.                       (2.9)


Thus the original vector is reconstructed from the coarsest approximation xi and
the details at the various levels. Each of these detail vectors is an orthogonal
projection of x on the corresponding one-dimensional subspace W1 where i =
I. . .. .N - 1. Our development shows that every vector in VN can be written in the
form of Equation 2.9; that is, as the sum of one vector apiece from the N subspaces
 WN_I, WN_2. .. . .Wj, and Vi. Also, these vector subspaces are mutually orthogonal.
vve say tnat tne vector space VM iS tne airect sum or tnese suDsvaceS. i nis is written

      "N -   따卄f    / VJH니   尸 Vr4- ..V vvi4- . '4' "Vf "   寸 r1        니"
                                  VN= WN_1 q) WN_2 q) . . . ,W1 q) VI.                          (2.10)
                              '      小八八MVn니八小dN/       \／卜／       m＼   卜／




As we will see, MRAs using wavelets fall into this framework in a natural fashion.
             뇨＋ 如尉1          V碼慌叫 씌켜aM 十咎仁                     9e'br 甲比·
2.2.2 Example of Approximating Vectors in Nested Subspaces of
      an Infinite-Dimensional Linear Vector Space
The concepts of the previous example involving a finite-dimensional linear vector
space can also be extended to infinite-dimensional spaces. Consider the familiar
Fourier series expansion of periodic signals. A real periodic signal of fundamental
period I seconds with finite energy1 over a period can be expressed as a linear
combination of sines and cosines of frequencies that are integer multiples of the
fundamental frequency 1/1 Hz. The set of all periodic signals of period I with
finite energy over a period forms a linear vector space. Let V0 denote the subspace
generated by the constant or "DC" term. Let V denote the subspace generated
by the DC term, the fundamental, and all harmonics up to the nth harmonic. The
basis for V, consists of 2n + I "vectors"; namely, cos(2jrkt / T) for k = 0, 1. . . ..n
and sin(2jrk / T) for k = 1. . . ..n. Thus V is the linear vector space containing the
periodic functions of interest. The basis vectors are mutually orthogonal under the



1 The finite energy requirement leads to a less strict form of convergence than the Dirichiet conditions
quoted in most texts on signal analysis.
32    Discrete Wavelet Transform and Orthogonal Wavelet Decomposition

      definition of the inner product

                                    （!                           ))= pT/2
                                   佃                              ) j                              dt
                                              )，
                                                       『
                                                           （!
                                   (x
                                                   ,              =                                     (2.11)
                                                                      J- T/2
                                                           (t)
                                                                               x
                                                                                             (t)
                                        (t)
                                                       y
                                                                                   (t)
                                                                                         y
     幻r 工（t), y (t) E I／的．
        Here, in the previous example, we have a nested sequence of linear vector sub-
     spaces V0 c V1 c . . .. Also, the concept of detail being gained in going from the
     approximation in Vk to the approximation in Vk+1 applies as well. In fact, this sim-
     ply amounts to adding a harmonic; that is, the sine and cosine functions at the
     harmonic frequency. Thus every periodic signal in V is the sum of the coarsest
     approximation; namely, the DC component and the detail functions that are the
     various harmonics.


     2.3 Example of an MRA
      Our third example of approximations in nested linear vector subspaces involves
      a wavelet and is an MRA [Chui 1992a; Daubechies 1988]. As we go through the
     example, the reader is urged to note the conceptual similarity of the constructs to
      those of the previous two examples. Let f (t) be a continuous, real-valued, finite
     energy signal. We will build approximations to this function at different levels of
     resolution using piecewise constant functions. Somewhere during this process we
     will obtain a representation for f (t) on the lines of the expression in Equation 2.6.
     Let us begin with an approximation that is constant over unit intervals. In other
     words, the approximating function has a constant value over the interval 0 드 t <1,
     a constant value (not necessarily the same value as over 0 < t < 1) over the interval
     1 < t < 2, and so on, to include all intervals of the form Z 5 t < Z + 1 for integer
     Z. Let us call this approximation f0(t) and, further, let us choose it such'that it is
     the best possible approximation in the sense that IIf (t) - fo(t)II2 is minimized. The
     best constant to approximate a function over an interval in this sense is the average
     value of the function over that interval. Thus

                                                   r e+1
                              .to(t) =工
                                      Jt                         f(r) dr, t5 t< t+1                     (2.12)

     for integer values of t. The function f0(t) is an approximation to f (t) in the linear
     vector space, which we will call V01 formed by the set of functions that are piecewise
     constant over unit intervals. Both f (t) and f0(t) lie in L2 (R), the linear vector space
     of square integrable functions. Thus the approximation process can be viewed as
     approximating a function in L2(R) by a function in its subspace V0 using the least
     squares criterion. In fact, as can be shown easily, fo(t) is the orthogonal projection
     of f (t) on V0.
                                                                                                    Exan갸91e of an A川？A    33


   Now consider approximating f (t) in the linear vector space of functions that are
piecewise constant over intervals of length 2; that is, intervals of the form 21 드 t <
21 + 2 for integer 1. Let us call this space Vi. Proceeding as described earlier and
calling the corresponding least squares approximation fi (t), we have

                                 （!                  1 r2,e+2
                                月                             f (r)              21< t< 21+ 2                    (2.13)
                                            )=
                                                     2 j2
                                                                       dr,
                                f1
                                      (t)
                                                 =
                                                     -




for integer values of 1. Observe again that the piecewise constants are average
values of f (t) over corresvondin2 intervals. ComDared to fn(t). the function fi (t)
is a coarser approximation to j t). i\ tiner approximation tnan Jo(f) is proviaea
by fi (t), the least squares approximation in the space V_i of functions that are
piecewise constant over half-unit intervals:



                 /h(!
                 f_
                      1
                          (t)
                                 )=
                                                 1       J
                                                         r,'/2+i/2 f (r) dx,      1/
                                                                                       2 <t <1/2 + 1/2
                                                                                                                ) (2.14)


for integer values of 1, as illustrated in Figure 2.5.
   In general, by proceeding on these lines, a hierarchy of approximations can be
obtained in which each approximation is piecewise constant over an interval with
a length that is an integer (positive or negative) power of 2 [Daubechids 1988]. Let
 Vk, for a given integer k, be the space of functions that is piecewise constant over
intervals of length 2". Then th아의r明Pm如하畔咽프壁單袈와ox岬뺙蜘．坦月t)
is given by
                                   12k (t+i)
                                l                                 -




                                                                                                                  (2.15)
                      Jk (t) 三 =   r         f (r) dx, 2't <t <2 (1+ 1)
                               ＝八 J2叱

 for integer values of 1.
    This structure shares some properties with what we saw in the earlier examples.
 There is a gradation in the quality of approximation. For two integers i and j, i <I,
 the approximation J;(t) is finer than f3 (t). This would suggest that the limiting
 approximation

                                                             烏 (t)           -kil曳fk(t)                           (2.16)


 is the function f (t) itself. Indeed, this is the case (see Problem 2 at the end of this
 chapter). There is also a nesting of subspaces: . . . .c V2 c V1 c V0 c V_i c V_2 c
 . . .c V_아. C L2(R). The coarsest approximation in this case is f (t). We can show
 that our initial requirement that f (t) be square integrable implies that

                                                                  f (t) =0                                        (2.17)
                                                                                                       g




                                                                                                     旨Qm芬 든
                                                                                                          Q<
                                                                                                            m
                                                                                                            市놔 걱Q글q크 Q二Q0굽8gq든Q <m市나둥83乙을긍그




Figure 2.5 Piecewise constant approximations to a function at two different levels of resolution.
(A) O匹批（게 function. (B) N叩roxim帥（)fl over h（기f-un汁 inter\／데s. (C) Appro川n기ation over un汁 inter\／이S
                                                                                  Example of an MRA         35


for all t (see Problem 1). Thus the subspace V contains just this one function that
is identically equal to zero. In vector space terminology, f (t) is the zero vector. As
in the previous two examples we can identify detail lost or gained in going between
approximations at different levels. We define the detail切ction at level k as


  m
Fr。      n
   Equati。2.17   reped
               and
,,,,,,,,, ,., ,,,, 느，   fk-
                          l
                      appli
                         ca
                          t  ,
                            (t)
                            。
                            i n-,
                               。  ,
                                 fk (
                                    t
                                  ,Equ),J,,n,.2.,18,t。
                                         ati。    ,,,,,,,,,,, (2,.,1,8)
                                                     successive
                                                             values
of k, we have

            -c ,ct)= 二, lt) 4 缸）                      m


                   可，的*多,, 仕），요，寸．1(!)=．兄．g1(t).                                                 (2.19)


'"'"，
    '”「“二心斗IC.: (t).,gk                            k= -的
                                                                ff
                                                                                                 (2.20)


2.3.1 Bases for the Approximation Subspaces and
      Hoar Scaling Function
The subspace structure in this example differs from those in the previous two ex-
amples in several of its properties. It is the possession of these differing properties,
in addition to those in common with the previous examples, that makes the struc-
ture of this example an MRA. We have already seen one difference: The coarsest
approximation does not depend on the fi.mction f (t). It is always the zero vector.
Consequently, the only common vector in all the approximation subspaces is the
zero vector. This is expressed in terms of the intersection of the subspaces as
                                               的
                                               n
                                                   Vk = ｛叫                                       (2.21)
                                               如
where the i-p stands for the zero vector.
   Another property is that if a function a(t) E Vk, then a(2t) E Vk_1 and vice versa.2
Yet another very interesting property, which we soon verify, i s that the bases for
all the subspaces in this structure can be名enerated using translations and dilations
of a single function called the scaling function.


2 This means that given a function that is piecewise constant over intervals of a certain length, then
dilating the function by a factor of one half will make it piecewise constant over integrals of half this
length, thus yielding a function in the next finer subspace. Doing the opposite (that is, dilating the
function by a factor of two) will yield a function in the next coarser subspace.
36    Discre旭 너／0velet 了ransform and O片hogan이 너／avelet Decon가DOS洌on

         Next we show that the basis for Vk for any integer k is obtained by translations
      of an appropriately dilated version of the single function given by

                                                      -'               11      0< t< 1
                                                    中（t)          三
                                                                                                                            (2.22)
                                                                        i0
                                                                               otherwise.
                                                                 \/mmM卜H尸＼                    小／   戶누十
                                                    尸＝b




      This function, which is just a rectangular pulse, is known as the Haar scaling function.
      Let



                                               毗，
                                                            『）
                                                                  긍／         ,",' " ' "        /(!   )dt
                                                                                                                            (2.23)

      for some integer k. Using Equation 2.15, c(k, Z) is simply the average value of f (t)
     ;14i. i..-.       口1m] ,k 口 ／戶 1   / nk / 口

     lit"' LILC
                                                    1


           """ "litl.t1
                                                          ] \      1그m nkJ


                   """vai""I. " " . I. "t4" 1" 1)." ""' 돠IJILLlL ILILL 뇨如 -
                                                                             八11 1L 八 r，뇨 小- _1. 八J




                                               砂（2 "t) = 1 土                                U,5t <．乙"                      (2.24)
                                                         tU                                 otnerwise

     ＼人／e have


                                    ）守 辰（t) = ＞二 ((k, Z）砂（2_kt寸t)                                                  ；艸卞t"M 毛 准25)
                                                                                                               어？P和，
                                           m뇨nn八八小乂三二凶，小小小小／\/／卞                                           .    n


     which 如icates that 血m主으쁘迦旦르프立쁘 ir con小in毗on of thP 伽nction 砂（2:
                                                                   ：如
     血nd主뇨뇨끄sla自mSJ孚in1ger山끄止pies of그k 프프唾，                       쁘뜨主久an之func如n in
      Vk can be obtained as a linear combination nLa dilation of 砂 (t) by a factor Qf
     2" and its translations by integer multiples of 2". To show that this set (namely,
     如（2mtt- Z ) : k, Z integers)) is a basis for Vk we have to show that the functions in
     the set are linearly independent. This follows in a straightforward manner from the
     fact that the set is orthogonal,

                                            仲(2기卜 r), 中（2 人r- m)) = 0                                                      (2.26)

     for Z 尹 m because, by Equation 2.24, there is no overlap between 砂 (2 "t -e ) and
     中但가 小 m).
                   ==) 나arr b力，ei寸        금現名il ?
     2.3.2 Bases for the Detail Subspaces and Haar Wavelet
     Just as the basis functions for the subspaces Vk could be obtained using translations
     and dilations of a single function, the basis functions for the subspaces in which the
     detail functions g, (t) reside can be obtained using translations and dilations of a sin-
     gle function, which in this case is a wavelet. In fact, the connection between MRAs
                                                                                                                Example of an 八川？A   37

and wavelets lies in being able to represent the detail functions in this manner. Let
us generate the basis functions for the details by first taking a look at

                                                  go(t) 三 /1l(D- 而(t).                                                      (2.27)

Because the subspaces are all nested, the basis at one level should be expressible
in terms of the basis at the next finer level. In particular, the basis for V0 must be
expressible in terms of the basis for V_i. That this happens, follows from the fact
that
                                           ///1




                           t 砂（r),"＝中（2t)＋砂（2t中1). 力／(4k) 十그f（心" )
                                /     \
                                                                                                                            (2.28)
                                     +        士                十恥唯-
Consider the unit time interval 0 드 t < 1. Over this interval,



, , ,,,.,,,,,,,,',:；三滋拉朴
                       ，，쓰，
                          ,", ' ,,
                             ,,,,，小，    ,""
                                   ,, ,,",,,,
汁紫盒撰茫烈恣打器就烈烈崙，’"" ""'"""'"
                                                   兀（t) = c(0, 0）中（t).                                                      (2.30)

＼사e have

                             0        Pt
                                              1                                                             )
                                            = 三［C(mL 2t) + c(- 1, 2t + 1)].
                         C
                                                                                                                            (2.31)
                                                       ,




                                 1J                                                                         \




In other words, the piecewise constant values that constitute fo (t) can be obtained
as the averages of two consecutive piecewise constant values of f_ i (t). In particular,


                             c
                                      (0, 0)       =       二  [c   (-   1,   0) +   c   (-   1,   1)   ].                   (2.32)

Substituting Equations 2.28, 2.29, 2.30, and 2.32 in Equation 2.27 yields

                                                   go(t) = d(0, 0)砂(t)                                                      (2.33)

for 0 < t < I where                                                'n H C (.．이 /c&t)
                                             ，꿈的= m 나的nHM口t) +CC니d）如

                                           砂（t) 三 ［中（2t)                      砂（2t - 1)1                                    (2.34)

and

                                                           月
                                                           l HD
                                                              二
                                                                             0                    l
                                                                   C         l          C         l
                             d(0, 0) 三                                                                                      (2.35)
38   Discrete Wavelet Transform and Orthogonal Wavelet Decomposition

     The function 砂(t) (shown in Figure 2.6) is the Haar wavelet. It is given by


                                               1 I   O5t< 1/2
                                   砂(t) = 1 -I       1/2 5t< I                     (2.36)
                                          [ 0        otherwise.

       As is required, 砂(t) integrates to zero. With

                                         1 ,



                              d(U, t ) 三 5[c(- 1, 24) - c(- I, 2t + UI             (2.37)




            Figure 2.6 Haar functions: (A) Scaling function. (B) Wavelet.
                                                                               Example 아 an 人IRA   39

玖／e have

                                                   的

                               go(t) = ＞二 d(O, t）砂（t -1)                                  (2.38)
                                               t= 1以）



which shows that go (t) can be expressed as a linear combination of integer translates
of the Haar wavelet. Following the same steps as for go(t) we have the general result
for any integer k,

                                               的

                           gk(t) = ＞二 d化Z）岬가그）                                            (2.39)


＼人／
  here

                                                       )
                                   工 H2
                     k
                                   d
                                   1
                     d
                     \
                     r    口t   三          C   t        (
                                               -1, 2t) -c (k- 1, 2t+ 1)].                 (2.40)


From Equations 2.23, 2.34, 2.36, and 2.40 we have

                                      l       12"(t+l) -       -
                       d(k, t) =三 f2kt                  f (t)砂(2 't -t ) dt.              (2.41)


Also,

                               似(2가                t), 砂（2가 H刃i)) = 0                     (2.42)

for t 尹 m. Equations 2.39 and 2.42 imply that for a specified integer k, the set
(, (2 "t - : Z integers}, obtained by dilating the wavelet 少 (t) by a factor of 2k and
translating by integer multiples of 2", provides a basis for the space containing the
detail function gk(t). Let us call this subspace Wk. Because Wk contains vectors
(again, piecewise constant functions) obtained as differences between vectors in
Vk_1 and Vk, we express this symbolically as

                                              w= v1ev.                                    (2.43)

Alternatively,

                                              Vk_1 = Vk 4) Wk.                            (2.44)

This is read "Vk...1 is the direct sum of Vk and Wk" and it simply means that every
vector in Vt_i can be obtained as the sum of a vector from Vk and a vector from
40    Discrete Wavelet Transform and Orthogonal Wavelet Decomposition

      Wk. Note that Wk C Vk_1. Recall that the vectors in Vk are orthogonal projections
      of vectors in Vk_1. Consequently, the subspace Wk of details of the form g, (t) is
      orthogonal to Vk; that is, every vector in Wk is orthogonal to every vector in Vk.
      Each of these two subspaces is said to be the orthogonal complement of the other in
      Vk_1. Carrying out the direct sum decomposition in Equation 2.44 further on Vk,
      Vk+1, and so on, we have



                                             Vk_1 =q）珌                                  (2.45)

      which says that Vk_ j is the direct sum of the linear vector subspaces Wk, Wk+1, and
      so on. Repeated application of the argument used to explain the orthogonality of
      Vk and Wk leads to the conclusion that the detail subspaces Wk, k = 0, 士1, 士2, and
      so on, are all mutually orthogonal. The same conclusion would also follow directly
      from the fact that


                                  他 (2寸kt -Z), 砂（2까 -n))=0                              (2.46)


      for k 尹 m regardless of whether Z = n. The reader should notice the difference
      between Equations 2.42 and 2.46. The latter indicates that Haar wavelets with two
      different dyadic dilations are orthogonal regardless of their positions on the dyad c
     스웬d. This result is quite easy to verify. For example, if we consider k = 0 and
     k = 1, we see that the product of 砂 (t - Z ) and 少(2퍄 - n) always integrates to
      zero by virtue of the fact that the product is itself zero when the two functions
      do not overlap or, when they do for a pair of values (t, n), the product is either
      砂 (t - 1) or its negative. The two equations together imply that the set of functions
      { r (2 "t - t ) : k, t integers}, consisting of dyadic dilations and translations of the
     Haar wavelet, is an orthogonal set. Finally, when we put together Equations 2.20
     and 2.39 we have

                                        00    的


                               f (t) = ＞二 ＞二 d(k, t）砂（2 't -Z).                        (2.47)
                                      k=-oc 2=-야그




     Equation 2.47 has a form identical to the one in Equation 2.6, indicating that we
     have obtained what we set out to do; namely, express the function f (t) in terms of
     a discrete wavelet representation. The orthogonality of the set of dyadically dilated
     and translated wavelets further makes this, by definition, an orthogonal wavelet
     decomposition or orthogonal MRA.
니＝垣回H따a
       dio叭）
                                                                                          (＼柚杓心W序：ti0仙   DYM(t/\\Ye.

 Ld뜨2)中aG>a
        侄）尸 C(0·匈                                                                          h   '         \
                                                                                                    Exan가DIe 아 anMRA    41

   2.3.3 Digital Filter Implementation of the                                                                   .
         Haar Wavelet Decomposition
   As we have seen, the coefficients of the expansion of the approximation at any
   level in terms of its basis functions are simply average values of the function f (t)
   over corresponding intervals. These are called approximation coefficients, and are
   obtained formally through the integration in Equation 2.23. Similarly, the detail
   coefficients d(k, t) can be obtained from Equation 2.41. However, as we will show, it
   is not necessary to perform the integration of the continuous-time function at every
   level. Given the coefficients at one level of approximation, the coefficients at the
   next coarser level of approximation, and by extension the coefficients at all coarser
   approximations, can be obtained by a digital filtering scheme [Daubechies 1988].
      Generalizing Equation 2.31, the average value over a given interval at one level
   of approximation is merely the average of the two piecewise constant values of the
   next finer approximation over this same interval,

                                   1
                                                             2n + 1)]
                         c(k, n) 三 三Lc(k - 1, 2n) + c(k - 1,                                                  (2.48);
                                     ,




   where n indicates the sample number or discrete time. Now suppose we were to
   pass the sequence c(k - 1, n) through a digital filter with impulse response

                                 h(n         =       ![   '8r   'm   '   + 8m+ ln
                                                                                "     .                       (7.49)'


                                         '           2          '    '     '    ' '




   Denoting the filter output by y(k - 1, n), we then have

                                       l
                        v (k - 1, n) = :[ c(k - 1, n) + c(k -1, n + 1)1.                                      (2.50)
                                                 .




                                       Z

   N야e that

                                    c(k, n) = y(k - 1, 2n).                                                   (2.51)

   This is a result that says that c(k, n) is obtained by passing c(k - 1, n) through the
   digital filter of impulse response h (n) and then retaining only alternate samples of
   the output. This process of reta如呼 毗帥iate samples is referred to as旦앉빳프쯔깬聖
   bi a factor of two. The combination of fi1terin2 and downsamplin2 is called decimation.
   :>1m11ar1y, irom tquauon 乙L싸, witn


                                 쁘크므쓰브                                                                        位52)
   we can show that d(k, n) is obtained from c(k -1, n) by passing the latter through a
   digital filter with impulse response , (n) and then downsampling by a factor of two.
                                                                         4a   m
42   Discrete 너／0velet ／尺IflS幻rm and Orth아iona/ 너幻velet Decon四Os川（9n


        Let us refer to the two previous digital filters as the H and G filters respectively.
     It is instructive to look at their frequency responses. The frequency response of
     月 is3

                                            斤佃）= e3을 cos(w/2)                                      (2.53)

     whereas the frequency response of G is

                                          G(w) = -jej을 sin(w/2).                                   (2.54)

        From the frequency response magnitudes plotted in Figure 2.7 we see that the
     H and G filters are (albeit poor) low-pass filters (LPFs) and high-pass filters (HPFs)
     respectively. From Equations 2.53 and 2.54 we have

                                        1月m川2 + 口7(n) + 兀기2 = I

                                        四(川2 + IG(w + 7r기2 = 1                                     (2.55)
                                              H(w)I2+ IG(w)I2 = I.

        Being a real digital filter,4 H satisfies

                                         나／（兀 + O)기 = 1 H (7r- w기．                                 (2.56)

     Similarly,

                                         IG（兀 + 幼1 == IG(jr -O)）卜                                  (2.57)

     Substituting w = 兀/2 - w into the first two equations of Equation 2.55 and using
     Equations 2.56 and 2.57 gives

                                   1月（兀／2 + O끼2 + 1月伽／2- w기2 = 1
                                                                                                   (2.58)
                                   IG(r/2+ w)I2+ IG(jr/2- w)I2 = 1.

     Because the previous equations indicate a mirroring of the squared frequency re-
     sponse magnitudes about w = 兀/2 (known as the quadrature frequency in various
     engineering applications), filters satisfying Equation 2.58 are called quadrature mirror
     filters or QMFs [Daubechies 1988; Mallat 1989a, 1989b].


     3The notation here is that 月 without the argument w refers to the filter, whereas 月 with the argument
     denotes the frequency response function. The same is true of G.
     4By a "real filter" we mean that its impulse response is real-valued.
                                                                            Exan가：)Ie of an 凡까？A   43




     Figure 2.7 Frequency response magnitudes of the 月 (A) and a (B) filters. The
                range of the horizontal axis only covers 0 드 w 5 7t because the filters are
                d呵t(기 \with re이 in）口ulse responses.



   The process of starting with a sequence of the approximation coefficients at some
level of resolution and then generating the approximation and detail coefficients
at coarser levels through decimation is referred to as a decomposition or analysis of
the sequence. The reverse process of combining the coarser approximation and
detail coefficients to yield the approximation coefficients at a finer resolution can
be performed by digital filtering as well, and is referred to as reconstruction or
synthesis. Let us develop the filtering construct for reconstruction by first looking
at how c(- 1, n) is obtained from the coarser coefficients c (0, n) and d(0, n).
44   ／가scre旭 以we旭t 灰加計아rn and O片hogon이 너／avelet Decon가)OS川on                                                            .   .
                                                                    I 戶小 n=1 - - r ' - r 1 .fl\    .r_ i  .11.i- I } 1
                                                                ,. c '. u.:-1 - - 1 r 1 H시 1 +LJ 戶 뇨 -' , ／中＼/ 1 r / 니
                                                       .-       ,        V\                    +   V '-＼니
                                                                                                            V




       From Equations 2.쿠1 and 2.
                                 37, it f。
                                         ll。
                                           ws that
                cc' 厄）：奴已心놔 CC니，琨＋D]

                                                                                                                                (2.59)
                                     c(- 1, 2n+ 1) = c(0, n) -d (0, n).

     Consider two filters called H and G with impulse responses given by

                                                     h(n) =8(n) +8(n -1)
                                                                                                                                (2.60)
                                                     g(n) = 8(n) -8 (n -1)


     respectively. Now suppose we have sequence p(n) defined as

                                                                    I (0,                                   n even
                                                                                                                                (2.61)
                                                                                           2)
                                                            =
                                               （4)                            c       n/
                                                            =
                                                                                                            n odd.
                                                                    t。
                                       「       (n)
                                       p
     That is, the sequence p(n) is obtained by inserting zeros between two successive
     values of c(0, n). This process is called upsampling by a factor of two and is depicted
     in Figure 2.8.
        Let q (n) be a similarly upsampled version of d(0, n):

                                       . .   Id(0, n/2)                                                     n even
                                      q(nJ = 1 rl                                                                               (2.62)
                                             Lu                                                             n odd.

       Let r(n) be the output of filter H with p(n) as its input. Then from Equation 2.60,

                                                     r(n) = p(n) + p(n - 1).                                                    (2.63)



                                                          C（川

                         /1 =   ()

                           0 .             .          .                  .        .        .           .        .   .



                           0 O 0 O S O 0 O 0 o 0 O

                                                        尸fl




             F勾마e 2.8 뱌＞sam口ting by a factor of two.
                                                                                    Ex（그／7갸Die 아an 人4只／\   45


From Equation 2.61 (see also Figure 2.8) we see that p(n) is zero for odd values of
72. Therefore, Equation 2.63 simplifies to



                                   r(n）出已）
                                                                    n even
                                                                                                 (2.64)
                                                                    n odd.

Putting Equation 2.61 in Equation 2.64 we get



                            r(n）十(0,
                                 (。,띤，)／기                               n even
                                                                                                 (2.65)
                                                                        n odd.

The relationship expressed between r(n) and c(0, n) in Equation 2.65 simply amounts
to creating r(n) by repeating each of the values of c(n) twice in succession. For
example, r(0) - c(0, 0), r(1) = c(0, 0), r(2) = c(0, 1), r(3) = c(0, 1), and so on.
Suppose s(n) is the output of filter G with q(n) as its input. Then, following steps
similar to those that led to Equation 2.65, we arrive at

                                                 (0n/                   n even
                                                                                                 (2.66)
                            (n)    -   {d
                                                  (。2)            /2)   n odd.
                        s
                                   -        -d     ,   (n-   1)
This means that s(n) is a sequence obtained from d(0, n) by repeating each of the
values of d(0, n)s twice, but with alternating signs. For example, s(0) = d(0, 0),
s(1) = -d(0, 0), s(2) = d(0, 1), s(3) = -d(0, 1), and so on. We now add the outputs
of the H and G filters:


             r(n)+s的十出아紫品，(, -,)／기
                                                                                 n even
                                                                                                 (2.67)
                                                                                 n odd.

Let us try out a few values of n to understand the implication of Equation 2.67.
Putting n = 0, 1, 2, 3 we get

                                  r(0) +s(0) = c(0, 0) +d(0, 0)
                                  r(1) +s(1) = c(0, 0) -d (0, 0)
                                                                                                 (2.68)
                                  r(2) +s(2) = c(0, 1) +d(0, 1)
                                  r (3) +s(3) = c(0, 1) -d (0, 1).

Observe from Equation 2.59 that these values are c(- 1, 0), c(- 1, 1), c(- 1, 2), and
c(- 1, 3) respectively. Thus,

                                       c(- 1, n) = r(n) + s(n).                                  (2.69)
46   Discre旭 너／0velet 了rans幻rm and Orthogc）尿7/ 너／亡n'elet Deco／그r)pos洌on


            c(O,n)                                                     d (l, n)
                     >   可（n)
                                                                                                       叫             ？(n)
                                      c(1,n)                            fl 2.／了 1                   C( I ,n)
                                                 .   八 1
                                                      .       ,            ,



                                                                                       日（n j
                                -4-
                                      -
                                                默n) 夕甘커                                        1+          A+
                                                                                                                \/
                         枷）
                 니
                                                                                       h (ii




         Figure 2.9 A two-level decomposition and reconstruction system.


     In summary, the result states that c(- 1, n) is obtained by adding the outputs of the
     filters H and G with the upsampled version of c(0, n), and d(O, n) respectively as
     their inputs. The process of upsampling followed by filtering is called interpolation.
         The［瓦 GI pair is called the decompos餌毗 or a｝帥厚寸砒r pa却 and the［玘 G] pair
     is called the reconstruction or synthesis pair. The two filter sets are related by

                                                      h(n) =2h(- n)
                                                                                                                            (2.70)
                                                      g(n) = 2g(- n)

     from which it follows that these filters are also of the QMF type. The block diagram
     of a two-level decomposition and reconstruction arrangement is shown in Figure 2.9.
     Starting with c(0, n), we work down to c(2, n) and then back up to c(0, n), with
     intermediate detail coefficients d(1, n) and d(2, n) being generated in the process.
     Such filtering schemes and their relation to wavelet transforms are discussed in
     much more detail in Chapter 3. We conclude Chapter 2 by providing an example
     MRA using the Haar wavelet.

     Example 2.1
           Consider the function

                                                 f (t) = exp(-t/4)u(r)                                                      (2.71)

           where u(t) is the unit step function

                                                                               t20
                                                                                                                            (2.72)
                                                                  {l
                                               u (t       드
                                                                   tU
                                                                    0          Otllel
                                                                               otherwise.
                                                                         Exan갸91e 可an 凡IRA        47




Figure 2.10 (A-F) 卜,1RA using the Ha（가 낚／（그＼ ／이et. F기（Dt A shows the r이아 아 ex口(- t/4).
            Plots B through F show piecewise constant approximations over
            intervals of length 1/4, 1/2, 1, 2, and 4 respectively.


The average value of this function over the interval a 5 t <b for any a 之 0 and
                                                                                b>a
is given by


             b 小 (i   fb
                           e的／
                                 4) 小은，帥如-                  exp(- 恥）
                                                                   ］·
                                                                                         (2.73)
48   Discrete 너／0ve/et 了尺7n計0rm and Orthogon이 Wave旭t Decompos／加n


                      0.05


            肛他）


                     -0.05                                                   I    I    I         (A)
                             0     2       4        6     8                  10   12   14   16


                       0.1


             g0(t)

                                                                             1    1    1         (B)
                                           4        6     8                  10   12   14   16




             幻（t)




                                                                             I    I    I         (C)
                                                          8                  10   12   14   16




             g2(t)




                     -0.2                                                         1    1
                             0                            8                  10   12   14


         Figure 2.11 (A-D) Detail functions g ] (t) through g2(t). .. \ 1}
                                                               卦步' J왁下）小V
                                                              .   .   -"C-




                                                  G水汕冬냥也
          Then, by our definition in Equation 2.23, we have


                                           4      / 2切＼ r      / 少＼]
                                 c(k. Z) = 4i ext니 =;1I I1- e사니 H十 I I .                               (2.74)
                                  ' "      2k ' \    4! L   -r \ 4) J

          The approximation fk(t) at resolution level k is given by


                                   fk (t) = c(k, t ),   2kf < r < 2k(t + 1).                           (2.75)
                                                                     Example 아an 凡IRA        49




  F勾바e 2.12 (A-E) Err아 between the origin（계 functi아）（가）d the 야：)pro川mations
            shown in Figure 2.10.



Figure 2.10 shows these approximations over the range 0 드 t < 16 for values k =
누2. -1. 0. 1, 2. The detail functions are shown in Ficure 2.11. whereas the approxima-
tion error netween tne originai runction j (t) ana tne approximations at various levels
are shown in Figure 2.12. By simply looking at the amplitude swings of the error
plots it is possible to see that the approximation error increases with increasing k; that
is, with increasing coarseness. We have also included the mean squared error corn-
uuted over the interval 0 < t < 16 alongside the plots, which again reveal the increas-
ing nature or tne error as a runction or K.                                             -
50   Discrete Wavelet Transform and Orthogonal Wavelet Decomposition

     2.4 Problems
       1. Let f (t) be a continuous, finite-energy function and let fk (t) be its least squares approxi-
          mation using a function that is piecewise constant over intervals of length 2'. Show that
          f (t) = 0 for all t.
       2. Based on Problem 1, show that the claim in Equation 2.16 that f_ (t) = f (t) is true.
          It is simple to prove what is known as pointwise convergence; that is, fk (to) 수 f (to) as
          k 수 H的 幻r any t = to.

       3. Suppose in Problem 2 that the function f (t) is discontinuous and the number of discon-
          tinuities is finite. Then show that f_ (t0) 尹 f (t0) if f (t) is discontinuous at t0. Further,
          show that the integral of the squared error between f (t) and f_m(t) is still zero. This
          form of convergence is known as convergence in the mean-squared sense.
     (4. jLet fk(t) be piecewise linear approximations to a continuous, finite-energy signal f (r)
     뇨"over intervals of length 2". Let tk, e 三 2k for integer values of k and t. Then fk (t) =
          [(/ (ik, f+l) - f (tk,e)]/(tk,f+l 나 tk,t)/f (t0,0). Can you find a function 中(t) such that its integer
          translates form a basis for fo (t)? What would be the basis for fo (t)? Hint: Unlike the
          Haar scaling function, which has support over 0 5 t 5 I and whose integer translates
          were used to generate the basis functions for f0(t) in Equation 2.22, the function 中(t) for
          this problem has support over 0 5 r 5 2.
       5. Suppose the input to the LPF decimator at level zero in Figure 2.9 consists of a sequence of
          length eight, say x(0), x(1). .. . .x(7), and the output after downsampling at level one are
          the four values denoted y(0), y(l), y(2), y(3). If we write y = hx for some matrix i I, what
          is fi ? Here, x = [x(0), x (1). . . . .x(7)JT andy = [y(0), y(l), y(2), y(3)IT. Now suppose that
          the y values are interpolated back to level zero using the LPF interpolator to yield the
          eight values we call z(0), z(l). .. . .z(7). Let z = Hy where z = Fz(0), z(1). .. ..z(7)IT. What
          is H? What is the relationship between the two matrices?
                        CHAPTER THREE


        MRA, Orthonormal
       Wavelets, and Their
    Relationship to Filter Banks



3.1 Introduction
Chapter 2 introduced the concept of the DWT. What is common to the two forms
of the wavelet transform seen so far (the CWT in Equation 1.55 and the DWT in
Equation 2.6) is the fact that the given signal is expressed in terms of translations
and dilations of a single mother wavelet. Indeed, the theme of this book is that
for anything to be discussed in the wavelet transform setting, these two elements
must be present. In other words, no translation and no dilation means no wavelets.
The introduction to the concepts of DWT and MRA in Chapter 2 was through a
particular wavelet-the Haar wavelet. DWTs would not be of much use if only
this one wavelet existed. It is natural, therefore, to pose questions such as: Are
there mother wavelets other than the Haar that can be used to express a function
using Equation 2.6? How would one go about constructing such wavelets? Is
there always an interpretation in terms of a multiresolution decomposition for such
a DWT? The purpose of this chapter is to address these questions by deriving
results that characterize all orthogonal wavelet decompositions. An understanding
of this chapter will enable the reader to comprehend the material on applications
in subsequent chapters.
   Chapter 2 showed a link between the DWT and subband filtering. A fuller
development of that link is provided in this chapter. The derivations have been
kept as simple as possible and key results are presented in italics. This was done to
let the reader who chooses to focus on the results, and not worry about the detailed
derivations, do so without much inconvenience. Also, some of the steps in certain
derivations are not presented within the main body of the text but are posed as
exercises at the end of the chapter.

                                         51
52       MRA, Orthonormal Wavelets, and Their Relationship to Filter Banks

         3.2 Formal Definition of an MRA
         First we provide a precise definition of an MRA by its defining properties or axioms.
         As we have seen, an MRA involves approximation of functions in a sequence of
         nested linear vector spaces. Not every sequence of nested vector spaces yields an
         MRA. We saw in Chapter 2 that in addition to the nesting property, the vector
         spaces need to satisfy certain other conditions. We formalize these conditions here
         [Daubechies 1988, 1992; Mallat 1989a, 1989b].
            The definit油i of an N恨A is the 向lowing十nII喚스三엣덫些更쁘쁘雙叱 linear
         V뜨tor叩畔斗：C Vi c如드.1勻（二二．.St.lch寸빤


     1
     t呼1. The union of these subspaces is dense in the space of square integrable functions
          .
              L2
                       (R)        L.   ,   .        .               ,                 ,                       ,       ,,




     1
     1    乙. i ne .intersection or tnese suospaces is a singieton set containing m1le all-zero
          .   runcuon or zero ve. to.          .c       r   .   ,                 ,




     1（兮There
       二： exists a function (called a scaling 加nction) 砂 (t)
       3. If f (t) E Vk then f (2t) E V1_1, and vice versa
             J( 「 ‘1 ' " " ". /( ‘『J「 ‘．'d   " " " " ". ' " ' "."
                                                                                  that 1{ 0 ((tr -H 凡
                                                                           such [1lat               k)J :
                                                                    , '       ,           .   .   .   .   ,   .   .        ,   .
     L나t.     1l1lere eXlS[S a nlllCnO1l (Caneq a SCqnng rnnCn（刀iJ 0 ( i j S1lC1l
                   ,                                                      "
                             'J
              k integer) is a basis for V0
         There are alternative logically equivalent axioms that can be used to define an MRA
         [Vaidyanathan 19921. We next examine the meaning of these statements.
            The first axiom mentions one set being dense in another. For a rigorous treatment
         of the concept of denseness the reader is referred to texts on mathematical analy-
         sis or topology (see, for example, Royden [19781 and Rudin [1976]). We provide a
         simple explanation of the concept that, although not very rigorous, should suffice
         for an understanding. Suppose A and B are two sets of real numbers such that
         A C B. The set A is said to be dense in B if for every element b E B we can find an
         element in A that is as close to b as we please. The most straightforward example of
         this notion is provided by the set of rational numbers Q and the set of real numbers
         R. The set Q is dense in R since for every real number x, it is possible to find a
         rational number that is as close to x as desired. Stated another way, it is possible to
         find a sequence of rational numbers ql, q2, and so on, such that as n 수 oo we have
         qn 수 x. It is important to observe that although qn E Q for any n, the real number
         x does not have to be rational. A classic example is provided in the definition of e,
         the base of the natural logarithm, as


                                                                    (＝無（따）"                                                (3.1)
         where the limit is taken as n steps through positive integer values. The right-hand
         side of Equation 3.1 is a rational number for any finite n, but the limit e is not. The
         fact that Q is dense in R lets us make approximations to irrational numbers with
         rational numbers in practical situations, such as numeric computation. For example,
                                                                Construction of a General Orthonormal MRA   53


we do not use the true values of 兀 or V三 when we perform computations on digital
machines. In this sense, density lets us treat Q as being almost as good as R,
although mathematically the t사o sets are very different in their properties [Royden
1978]. Thus the first axiom of the MRA definition implies that the union of all nested
linear vector spaces yields a space (let us call this set V_的) that is not the same as the
space of signals with finite energy, L2(R), but is dense in it. In other words, for every
signal f (t) e L2(R) there is a signal in V的 that is as close to f (t) as we please.
Here the closeness of two signals is measured by the energy in their difference.
Thus, we can regard V_ as being as good as L2(R) for all practical purposes.
   The second property states that the only signal common to all the vector spaces
is the all-zero signal or the zero vector. The third property brings in dilation and
states that a factor-of-two dilation of a vector belonging to a subspace at a certain
level yields a vector in the next coarser subspace. Conversely, dilating by a factor
of one half yields a function in the next finer subspace. It should be noted that the
notion of coarseness here has been generalized from the Haar example in Chapter 2.
Vector space V is coarser than Vj' if i > j. The final property requires that there be a
scaling function 中(t) such that the set { (t - n) : n integerl is linearly independent,
and any function fo (t) e V0 is expressible as
                                                     的

                                  九（t) = ＞二 口（O, n）如- n)                                            位2)
                                           fl = -00


for a sequence of scalars a(O, n) where n = 0, +1, 士2, and so on. It should be noted
that the statement does not call for the set of 中(t) and its integer translates to be
orthogonal. However,.an important class of MRAs results when they are orthogonal
[Daubechies 19881. Also, there is no mention of a wavelet in the definition of an
MRA. Yet, as shown in this chapter, an MRA provides a natural setting for the DWT.
Chapter 2 first presented an MRA and then derived the bases for the approximation
subspaces. In Section 3.3 we do the opposite. We start with the scaling function
and then construct an MRA that satisfies the properties listed at the beginning of
this section.

3.3 Construction of a General Orthonormal MRA
3.3.1 Scaling Function and Subspaces

놨姓沚므更些쁘竺雙竺典셋史少g:
G）뇐必映빳D只瑛’:
                                                     'OO
                                                 1
                                                                                                    位3)
                                            J-             O0




lAlthough we explicitly state this requirement, it actually follows from the next two requirements and
Equation 3.10.
54   八4RA, Orthonorm이 Wavele朽，and The仁 尸이at幻nsh徊 幻 F肝er B（加ks


     (\ It has unit energy:


                                         II (t)II2   =     ：岫
                                                                （D1' dt     =   1.                   (3.4)


     G: he set c。的蜘可蛔 耐ts in呼r tran針計帥毗岫na!2:
                                                仲(t), 中（t- n)) = 8(n).                               位5)

        Because a set of orthogonal vectors is linearly independent, the set t中(t - k) :
     k integer) consists of linearly independent vectors. Therefore, it serves as a basis
     for a linear vector space that we will call V0. Substi뺘ing 2_kt for t in Equation 3.5
     we get

                                      ( (2H't), 中(2켜 Hn)) =2"8(n)                                    (3.6)

     which indicates that the set

                                          佃（2hb- t) : Z integer)                                     (3.7)

     is also an orthogonal set for a given integer k. Let us call the linear vector space

     g톈甲抛．d by t址s set平斗呼巾t뇨sub和『“「出he Haar wavelet decomposition
     in L nar兀er 乙／ Vk is 쓰뜨쯔쁘jvecror space man vk.4.
        丁5,-' .끼'. 5. .끼1m八nnt시 1J_ 1J 1/       八. . 1 i斗r\ 八14 n八14n1뇨.3
        느뜨 口LtIJi＞나札口） " " ' ! V -I. VU.. V 1   m끄-A- aI.) UJ.IJ afl工上크1y




                                         廻三Ji父工므즈끄二느                                                 (3.8)

     Suppose we now add the condition

                                                     V0 c V_1.                                       (3.9)

     The condition in Equation 3.9 requires every vector in V0 to belong to V_i as well.
     In particular 中(t), which is in V0, must also be in V_1. Thus it should be possible
     to express 中(t) as a linear combination of the basis for V_1, namely, { (2t - n) :
     n integer). With this additional property, 中(t) qualifies as a scaling function. This
     property is stated as the following dilation equation [Daubechies 1988; Mallat 1989a,


     2 In this particular instance we have a specialized form of orthogonality called orthonormality, which
     refers to the fact that, in addition to orthogonality, we have set I1中（i 中 k)I I = I in Equation 3.4.
     3Read the symbol ＜수 in Equation 3.8 as "implies and is implied by."
                                                                                           （力ns却（火사jot) 아 (7Gener이 O寸honorm이 /＼까？A   55


                  1989b; Strang 19891: There is a sequence of scalars c(n), n = 0, 士1, +2, and so on, such
                  th（갸


   ( f씨쓰쩍月                 =1                                                                                               (3.10)

   " ' 亡佃毗 工二伽坤'班' 닢
                  In Equation 3.10 we have used the fact that the basis for V_1 is given by translates
              1
                  of 中(2t) by integer multiples of half-unit intervals. Since 砂 (t) is expressed in terms
                  of its own dyadic dilation and translation, Equation 3.10旭r받쁘르叱0쿄旦크逆i쁘塑
                  越프뼛0毛ox깐塑匙叱啣亥쁘e프쁘딴室끄 [Daubechies 1992; Daubechies and Lagarias
,'.IC (。) IdLfA.?21, 1992].
        J T ' 十“們RePlaCing t in Equation 3.10 by 2 't, we have
         LI
         r                                                            m

                                             中（2 't) = ＞二 c(n）中（2 (k'')t 中n)                                                (3.11)
 " 工 ( (+t) =2.                                                 n = 1oO



                  which implies that the basis for Vk is contained in Vk_1. In other words, 地 J                                ear
                  叱c加r 욘paces · · ·m V, V_1, ..迦 쯔쯔뜨쁘翅雙뜨드

                                                                                                                            (3.12)

                  Thus the condition in Equation 3.9 is equivalent to a nesting of all the subspaces
                  mlv아ved.
                     The union of the subspaces is dense in L2(R). The steps involved in the proof of this
                  statement are presented as an exercise (see Problem 2 at the end of this chapter). At
                  this stage we have an MRA because all the axioms for one are satisfied. Observe that
                  the initial set of properties of 砂 (t), along with the dilation equation, was sufficient
                  to arrive at an MRA.
                                                                        \                             小또戶入    裨M\
                  3.3.2 Implications of the Dilation Equation and Orthogonality
                  A constraint on the coefficients: By integrating both sides of the dilation equation,
                  Equation 3.10, with respect to t and canceling the common terms we get

                                                                      以）


                                                                 Zc             (n)        =   2.
                                                                                                                            (3.13)
                                                                n=    _ 的
                                                            八小小／＼八／                   7느小H



                  From Equations 3.6 and 3.10 we have

                                         (4) (t) 4)(t
                                               ,        -       ))    =     ,5( ),                                          (3.14


                                         ""'"' "'겉쿄느""""" ""                                                                '"""
                                                            -               I         t-


                                                                                  m= 卜 的
56    MRA, O片honorn）이 Wave旭枉 (7nd Their Re/ationsh徊 幻 F肝er Banks

     Define

                                       R(r) 三 ( (t), 砂 (t - r))                                  (3.16)

     the autocorrelation function of 中(t). Equation 3.14 states that R(r) is zero for all
     integer arguments except r = 0. Let

                                            m(w) 三 下m(t)]                                        (3.17)

     be the Fourier transform of 中(t). Then, the orthonormality condition in Equa-
     tion 3.14 has the frequency domain equivalent

                                        的

                                       ＞二 呻（w+ 2兀t)I2= 1 t4，回                                   (3.18)
                                     二느쓰 ／나                         止
     which is referred to as the Poisson summation for刃iula [Chui 1992a].
       Equation 3.15 says something about the autocorrelation sequence of the coefficient
     sequence c(n). Defining the autocorrelation sequence

                                                的

                                     r (t) 三 Z c(m)c(m - t)                                     (3.19)

     we have, according to Equation 3.15,

                                            乙（2Z) 三 28(e)                                       (3.20)

     which says that the autocorrelation sequence of c(n) is zero at even lags except lag zero
     [Daubechies 1988; Strang 1989]. Let us now look at a corresponding frequency
     domain interpretation. Let



                                      C(w) 三    ＞二    c
                                                          (n)
                                                                e 3' "
                                                                                                (3.21)


     be the Fourier transform of the sequence c(n). Then the frequency domain equiva-
     lent of Equation 3.20 is4

                                    1C(co)12 + IC(w+ 71)I2 =4.                                 (3.22)


     唾更쁘孼           뇨뺘 艸 畔M岫r. T呵엥.叫昭，帥. 恤．S岫艸，,:.If.X（小，蜘．如町
     transrorm or a cuscrete time
                             signai 工 (n力 [nen me rouner 口ansrorm or XILfl) is L人 "WI句 十 AW／乙 十 兀'-I／乙．




                                                                                                          ＼노
                                                                             Constri石加n of （그 (3eneral C＞寸honorm이 加仄A                57


   This is often called the power cornplernentarity condition [Vaidyanathan 1990, 1992;
Vetterli and Herley 1992; Vetterli and Kovacevic 1995]. Suppose we have a 血nction
f (t) from which we obtain fk(t), k = 0, 士1, 士2, and so on, the orthogonal projections
of f (t) on the subspaces Vk, k = 0, 士1, 士2, and so on. Let us represent fk (t) in terms




of   the   basis   functions       in   Equation
                                         fk   =    7 asm,
                                                n= -的
                                               (t)      3.                       :｝드’   -   :
                                                                                            n)   .     -" '
                                                                                                     工2蜘뼈     仄作，m) 口囚
                                                                                                                         (3.23)
                                                                                                                            cCk,' '）사喜

T小que岫 毗.) 耐he co如岫帥 .oe蜘誌業벎. 값낢늠喆디bf t盞 呵’
functions fk (t) in terms of their respective basis functions. We refer to fk (t) as the
approximation at level k. Let us now establish a relationship between the coefficients
at one level of approximation and the next. We start with the particular case of fi (t)
and fo(t). From Equation 3.23

                                                              的

                                        山 (t) = ＞二 口（-1, n）中（2t - n)                                                       (3.24)


                                              而（t) =         >        n(0，兀）砂（i- n).                                       (3.25)
                                                             n==1的



Because Jo (t) is the orthogonal projection of fi (t) on V0. the error or detail function

                                                     go(t) 三 兀1(t) - 九（t)                                                (3.26)

is orthogonal to the subspace V0 and, in particular, to its basis. Therefore,

                                              (f_1(t) - f0(t), 中(t - n)) = 0                                             (3.27)

for integer n. Equivalently,

                       (f0(t), 中(t - n))                                                                   노3弓싱          (3.28)
                           3，寸I
From Equation 3.25 and the orthonorma                                         of 砂 (t), and its integer translates in
Equation쿄5, it follows that the left-hand si                                   of Equation 3.28 is given by
      ＜戶t),+(t小）＞二3(M)
                                               （九아中(t             -    n力＝    C>                                         位29)
Next we evaluate the right-hand side of Equation 3.28.
  From Equation 3.10, db
                                劍 俉尹耐毗r)
                               仲（t)，砂（2t- m))= ＞二 c(n)（中（2t -刃2)，砂（2t - n))                                              (3.30)
                                                             n= -oo
58   A／仄A. Orthonormal Wavele朽. and Their Re／아幻nsh徊 幻 F肝er Banks

     Using Equation 3.6 in the right-hand side of Equation 3.30 we have
     4凶吻如多m)>                                                                                                                      1J
            ＝소熙m)                                           （吏姓色으느；끄끄＝曾                                                                                                                               (3.31)
                                                                      느뇨           \/..                                                            '



     From Equation 3.24,                                          그 (1미便呼，叫 , ？釘）十卜mD >

                                                                                      凹

                      (f_1(t)，中（t小兀）) = ＞二 口(-1, m艸t二끄뉴砂侮卞刊）                                                                                                                                          (3.32)
                                                                                   m= -的                                                                                                 m   ,



     which, in combination with Equation 3.31, yields

                                                                                                           的

                                                                                                                                                                                                      (3.33)
                            (/
                            (fj                     ,   中（!           -              )= m=-oo
                                                                                          =                                                                                    2
                                                                                                                                                                                   2
                                   (!                                         4)
                                                                      -
                                               )，
                              [1
                                                                                                                                                                    c
                                   (t)                                        n)                                                                                                   2n)
                                                                                                    斗Hm)                                                                (m-
                                                            (t
                                                                                                                     a        (-        1,             m)
     Substituting Equations 3.29 and 3.33 in Equation 3.28 we get


                                         a
                                         .(0        (0, ,   n)
                                                            .)=           =         乞         a
                                                                                              .(-          (-   l
                                                                                                                1,   ,   m)
                                                                                                                         m)             c    (m-
                                                                                                                                                            1
                                                                                                                                                            ,   ,        2n)
                                                                                                                                                                                                      (3.34)


        Our derivation started with the particular case of f_1(t) and f0(t), and led to
     the relationship between a (0, n) and a (- 1, n) in Equation 3.34. Starting with the
     more general case of fk_1(t) and fk(t), and following the previous steps, leads to
     the relationship                                          出小 '

        9eV全 K며＼杭e人 d                                             ,                뜨
                                         斗(k-I,寸＝'"
     삔未y" \                        "「"「『
                                                                                                                                                                                                 \,
                                                                                                                                                                                                      位35)
                                                                              m=＋的
                 寸t
     where a(k, n) are coefficients of the expansion of fk(t) in terms of the basis for Vk
     as in Equation 3.23. Equation 3.35 reveals that with knowledge of the coefficients c(n) in
     Equation 3.10 it is possible to obtain the coefficients a(k, n) at one level using the coefficients
     at the next finer level. The interpretation of the operation in Equation 3.35 is discussed
     in greater detail in Section 3.5.


     3.4 A Wavelet Basis for the MRA
     We now turn our attention to the spaces containing the detail functions. Define

                                                                      歇(t) 三 /i_1(t) - 九(t)                                                                                                           位36)

     as the detail function at level k. The functions gk(t) and fk(t) are orthogonal to each
     other. Recall that in the case of the Haar wavelet decomposition, the detail function
                                                                                     A 14七刃0旭t Basis 幻r The 凡仄A   59

at a particular level was expressed in terms of translates of a dilated version of the
Haar wavelet. We now try to construct a similar expression for the general case.
   Suppose 少 (t) is a function in V_1 satisfying the following:



                           \
                               \
                                        ／巴少（t) dt==0 기
                                        J-
                                    (* (t),
                                               ooi



                                               叭t
                                                     (t)   『 dt
                                                            -   n)
                                                                       =
                                                                     ) =
                                                                           1

                                                                           (n)
                                                                                 \
                                                                                 j                       (3.37)


                                   L （叭n蚊二낀） = U.
                                        Je白I中弓 Cm姃 유帥小
The function 少 (t) is a wavelet that provides the DWT corresponding to this MRA. The
rest of this section is devoted to establishing this fact.


3.4.1 Two-scale Re山tion 化r 奴t)

The second and third requirements in Equation 3.37 state that 砂 (t) and its integer
translates form an orthonormal set. Also, the last condition in Equation 3.37 requires
砂(t) to be orthogonal to all vectors in V0. Because 少(t) is in V_1, it can be expressed
in terms of the basis of the subspace [Daubechies 1988]. Let d(n), n = 0, 士1, 士2,
and so on, be the corresponding coefficients so that

                                                    凹

                                   砂（D= ＞二 d(n）中（2t - n)                                                 (3.38)
                                               n＝小的



                                                ale,,,,.,, , , 砂（,).
*,,,,*, similar ,, ,,,,,,,,,, ,, 由,,,, , 搖磊尸껍竺fYi)
There are constraints on d(n) that follow from these conditions. Integrating both
sides of Equation 3.38 and using the fact that the integral of 砂 (t) is required to be
zero leads to

                                               的

                                             ＞二 d（兀）=0.                                                  位39)
                                             n == 小的



Similar to Equation 3.15 we have

 )                             1 1떡
                                                                                                         位40)
                               三, 느d伽)d(m -2Z) =8(t)
which means that the autocorrelation of d(n) is zero at all even lags except at lag
zero EDaubechies 1988; Strang 1989]. Using Equations 3.10 and 3.38 along with the
60    凡4只A. Orthonormal Wavele朽. and Their Re/at幻nsh徊 幻 F肝er Banks

      mutual orthogonality of 少 (t) and translates of 中(t) we have, by proceeding on lines
      similar to the derivation of Equation 3.15,


                                                              (1r (t), 中(t -t) ) = 0
                                                                                                                                                     (3.41)
                                                                                               I      우＼
                                                                                                      的


                                                                                            = 三, 느m川"伽- 2Z)
      which implies that the cross-correlation between d(n) and c(n) is zero at even lags
      [Daubechies 1988; Strang 1989]. Equations 3.15, 3.40, and 3.41 imply that the set of
      sequences formed by the even shifts of c(n) and d(n) is an orthogonal set.
        We now move to the frequency domain. Defining

                                                                                               的

                                                                              D(w）三 ）二 d（凡）e1' '                                                     (3.42)
                                                                                             n= -.的



     we have the frequency domain equivalent of Equation 3.40 as


                                                                             ID(o川2 + 1D(w + 7r기2 = 4                                                (3.43)

     and that of Equation 3.41 as


                                                              C(w)D*(w) + C(w + Jr)D*(w + 兀) =0.                                                     (3.44)

     : , , , .,, ,        CCtM)   .
                                                 +\C.
                                                         (쓰
                                                                      3.
                                                                           44 can     be
                                                                                                     mpactly in matrix
                                                                                            written c。                                  f。
                                                                                                                                             rm as


                     [C
                       (w)                              C(o+     兀)
                                                                            1[   C*
                                                                                      (w)
                                                                                                      D*
                                                                                                           (w)
                                                                                                                      1   =   [4
                                                                                                                                    0
                                                                                                                                                     (3.45)
                     LD(w)                              D(w+ 2r) JLC*(w+ Jr)                          D (w+ Jr) J             LU    4        ·
     By interchanging5 the matrices on the left-hand side of Equation 3.45 we have


                                                                           D' 佃）            卄C(w)                C(w＋兀）]=[4                          位46)
                            [C
                                      '
                                          (co)
                            L C '(w + 7r)                                  D*(w+ Jr) JLD(w)                      D(w+ ir) J        LU        40

     which is known as the paraunitarli condition EBurrus, Gop岫th, and Guo 1997;
     Vaidyanathan 1990, 1992; Vetterli and Kovacevic 1995]. Carrying out the matrix


     5Although matrix multiplication is not commutative in general, it works when the product is a multiple
     of the identity matrix, as in this case.
                                                                                                      A Wavelet Basis for the MRA   61

multiplication on the left-hand side of Equation 3.46 and equating it to the right-
hand side, we get the following6:

                                                             1C(n川2 + ID（口川2 = 4                                           (3.47)
                              （少（w)C(w + 7r) + D*佃)D佃 + 兀）= 0.                                                             (3.48)

On taking the inverse Fourier transform of Equation 3.48 we get the corresponding
time domain equivalents:

                                  m
                                        \                                   的

                                             c(n)c(n +e) + : ii: d(n)d(n +Z) = 48(t)                                       (3.49)
                                  느     rm
                                                                         n= -的
                                                                       件1口m小1/       m小1八m1\         ／느V小口／   m/   m


                   00                                              的


                 ＞二 (-1)'c(n)c(n +Z) + ＞二 (-1)"d(n)d(n +Z) = 0.
                 n=-00            4 -        ,-. -    -      n=-oo
                                                                                                                           (3.50)


In deriving Equation 3.50 from Equation 3.48 we have used the fact that translating
the Fourier transform by 7r radians in the frequency domain is equivalent to multi-
plying the corresponding time domain sequence by (- 1)". Adding Equations 3.49
and 3.50 yields      - ., . . "小.-. ,. ,.  . '- - S寸 , 工，
         ' . ..     (m.",1 入뿌t如싸고. m.,(b V m舍小佯代


                  1                                              1
            米黎r 的                                                  的

                        ＞二c(2n)c(2n+t) + ＞二 d(2n)d(2n+ f) z48(t).
                   1 n= -oo                                  n= -的
                    戶＼
                     ／느八八小amm戶m11八入八小1戶느尸八／                                      \




3.4.2 Basis for the Detail Subspaces
Let


                        v(t) = 左：
                               多:＆그 呼뇨＋n)
                                     乙
                                          + 左：
                                            多  d（三"）砂（t+n).
                                             ：瓦 乙
                                                                                                                           (3.52)


Using Equations 3.10 and 區鈿趣 the right-hand side of Equation 3.52 we get
           （卉t):. _2卜 C (b1) 카JtJn7                       r 甲伊J= ?m - d (oi ) 功／그t==4八）
            T"    ）二m仄）       "                      ＝小                  勿r二7         "        r '       /
                                        以）           以）     n/ n . 4\

                          v(t) = 1m1
                                 '5小 느日
                                     5m 느쑤勻伽欣갸＋2n寸0+
                                                               z
                                  m= -00 fl= -的
                                                                                                                           (3.53)

                                  ，立,立"「？’                              d(m)中(2t+ 2n -m)



6 Even though the matrix multiplication yields four equations, only two of these results are independent.
62   MRA, Orthonormal Wavelets, and Their Relationship to Filter Banks

     which expresses v(t) as a linear combination of 中(2t) and its translates. Substituting
     m = 2n + Z in Equation 3.53 we obtain


            v(t) =
                     ，희，
                       ＞小아d(2n)d(2n+2t)]卜／）· (3.54)
                     l Hn
                     4  乙




     Substituting Equation 3.51 in Equation 3.54 we see that

                                                  v(t) = 砂 (2t).                        (3.55)

     Thus 中(2t) is the same as the function v(t) defined in Equation 3.52, indicating that
     0 (2t) (and hence any of its translates by half-unit intervals) is a linear combination
     of integer translates of 中(t) and 砂 (t). Since 佃(2t -Z) : Z integer} is the basis for V_1,
     the implication then is that every vector in V_i is expressible as a linear combination
     of integer translates of 0(t) and 砂 (t). That is, in general, fi (t) can be expressed as

                                     00                            的

                            f_i (t) = ＞二 口（0，兀）中（rHn) + Zb (0，兀）少（t小n)                  位56)
                                   fl= -00                    fl= -的



     for some pair of sequences a(0, n) and b(O, n). The first sum in Equation 3.56 is fo(t)
     as given in Equation 3.25. By Equation 3.26, the second sum is go(t); that is,

                                                   00

                                      go(t) = ＞二 b(0, n）砂（t - n)·                       位57)
                                                 n= _ 的



        Just as f0(t) is in the space V0 spanned by 中(t) and its unit translates, g0(t) is
     in the subspace spanned by 少 (t) and its integer translates. This subspace can be
     regarded as the difference between the subspaces V_i and V0. Although we have
     established a relationship between a (0, n) and a(- 1, n) in Equation 3.34, we have
     not done so for b(0, n). We next derive a relationship between a (,-1, n) and b(0, n).
        Taking the inner product of both sides of Equation 3.56 with respect to 砂 (t - n)
     玖／e have

                                 (f_1(t), 少(t - n)) = (go(t), 砂(t - n)).                (3.58)

     The term involving f0(t) drops out because of the orthogonality of 中(t) and its
     translates to 少(t) and its translates. From Equation 3.57 and the orthonormality of
     砂(t) and its integer translates, it follows that the right-hand side of Equation 3.58
     is given by

                                          (go(t), 砂(t - n)) = b(0, n).                  (3.59)
                                                                                                A 너/aveiet B（羽台 幻r the 凡仄A   63

We next evaluate the left-hand side of Equation 3.58.
 From Equation 3.38,


                 他(t)，中（2t -m))= ＞二 d(n)（中（2t小m)，中（2t -兀）).                                                         位60)
                                       n= -的



Using Equation 3.6 in the right-hand side of Equation 3.60 we have

                                                   d(m)
                               （少(t), 中（2t- m)) == =;                                                               (3.61)
                                                                     2         "




From Equation 3.24,

                                       oc
               (f_ j(t), 少(t - n)) = 兄 .（寸1, m)（少（t놔n)，砂（2t- m))                                                    (3.62)
                                     m＝寸的



which, in combination with Equation 3.61, yields

                                               的                           _7I__.                ' ...\

                     (f_i (t), 少 (t- n)) =                                                                          位63)
                                             ，읖    "   (-   1，      川" "" '                ;"       '"



Substituting Equations 3.59 and 3.63 in Equation 3.58 we get

                                       的                         Il. ...           'h..\

                          b (0，刃）= ＞二 口（-1, m）띠"'，1二"I.                                                             (3.64)
                                                                           乙
                                     m= - 的



Observe the similarity between the results in Equations 3.34 and 3.64. By general-
izing the result we have


                         也，弓）=，斗(k-1,m)""' ;'""                                                                     (3.65)


3.4.3 Direct Sum Decomposition
Let W0 be the linear vector space that has the set {i,tr(t - n) : n integer) for its basis.
According to Equation 3.57, W0 is the vector subspace of detail functions at level
zero. Equation 3.56 implies that every vector in V_1 can be expressed as the sum of a
vector in V0 and a vector in Wo. Also, the two subspaces V0 and Wo are orthogonal
complements of each other in the space V_1 [Daubechies 1988, 1992; Strang and
Nguyen 19961. Using the direct sum notation of Chapter 2 we can write

                                     1乙l = V0 ) 仍b.                                                                 位66)
64   MRA, O斤honorm이 Wavele朽. and Th이r Rek力ionsh徊 幻／카ter Banks

     The result is generalized easily to other levels as

                                                     Vk 1 = Vk q) Wk                              位67)

     where Wk is the subspace generated by the set {i/r (2 "t - n) : n integer) for a given
     integer k. Applying the direct sum recursively we have [Daubechies 1988, 1992;
     Strang and Nguyen 19961

                                                                             的


                                                     Vk_l =q) W1.                                 (3.68)
                                                                             j=k

     If we let k -* -的 in Equation 3.68,

                                                                             苡）


                                                     V_ = q) 까.                                   (3.69)
                                                                            3= -以）



     In other words, given a square integrable function f (t), we have
                                                     00                 的

                                f_ (t) = Z ＞二 b(k, t)少(2'"t -Z）·                                  位70)
                                                   k=-cc t =-以
                                                                         /?
     It is clear from the discussion in Section 3.2 that Equation 3.70 gives the best possible
     approximation to the given input function f (t). In fact, for most signals of interest,
     f (t) = f_a그(t). Thus, 砂(t) is a wavelet for the MRA associated with 中(t). The
     dyadic dilates and translates of 砂 (t) form an orthogonal basis for a linear vector
     space that is dense in L2(R). Such a basis is called a Riesz basis7 of L2(R).


     3.5 Digital Filtering Interpretation
     3.5.1 Decomposition Filters
     Let

                                                                              c(n')
                                                   / 九（n) 三 슈：2m：尸
                                                                '   "
                                                                                                  (3.71)

                                               I        . .    d(n)
                                          /    /      g tri) 三 H; H
                                                      ,                           乙
                                                                                                  (3.72)

                                          \h
                                                          (n)           三     h   (-   n)
                                                                                                  (3.73)

                                                      g(n) 三 g（十n)                                (3.74)


     7A formal definition of a Riesz basis and a related discussion are provided in Appendix B.
,       , , , , , ,, , , , , , ,, , , , , , , , , , , , , , ,                 , ,, , , , ,            , , , , , , , , , , Digital, Filtering                              65
                                                                                                                                                             C 'n)
                                                                                                                                                 InterpretatiW仙      c/
where           c   (n)
                                and d   (n)                  efficients 。f the tw。
                                                        are c。                               -scale            relati。ns   Equati。
                                                                                                                             in
                                                                                                                                 ns 10ti             3.
                                                                                                                                                                          (444)
3.38 respectively.                                 We       can now rewrite Equations                    3.   35 and 3.65 as         1988
                                  f
                                                                                                                                   [Daubechies
                          'ic
                                              。!        )
                                                                        的

                                                             a(k, n) = ＞二 .(k小1, m）万（2n - m)                                                              (3.75)
                                                                      刃1=1的


                                                                       的

                                                            b(k, n) = >二 a(k- 1,m)g(2n- m).                                                               (3.76)
                                                                     m＝小的



Equation 3.75 shows that a (k, n) is obtained from a (k - 1, n) by convolving the
latter with the sequence h (n) and retaining only the even indexed samples. In other
words, by passing a (k - 1, n) through a digital filter with impulse response h(n)
and retaining every other sample, we obtain a(k, n). As mentioned in Chapter 2,
this process is called decimation by a factor of two. Similarly, b(k, n) is obtained by
convolving a (k - 1, n) with the sequence g(n) and downsampling by a factor of two
to retain only the even indexed samples.
    We continue to use the notation of Chapter 2 of using the same uppercase letter
as the impulse response to denote the filter. For example, H stands for the filter
with an impulse response of h(n), H stands for the filter with an impulse response
of h (n), and so on. Let us now examine properties associated with H and H. By
Equation 3.13 and the definition of h(n),


                                                                           ＞二九（玎）      =     1.
                                                                                                                                                          (3.77)


We deliberately left the limits unspecified in the summation in Equation 3.77. If
H is an infinite impulse response (IIR) filter, then the limits could conceivably extend
from -oo to oo, in which case the filters would be noncausal. If the filter is of the
finite impulse response type, then the summation extends over a finite range of
values of n. Let

                                                                    H(w) 三 ) ' h(n)ejm"                                                                   (3.78)
                                                                                  11




be the frequency response of the filter H. Then, by Equation 3.77,

                                                                            H(O) = 1                                                                      (3.79)

which says that the frequency response at DC is unity. Also, from Equation 3.22,

                                                                  IH(w)12 + 田佃＋玔2 = 1.                                                                    (3.8아
66   MRA. Orthonorm이 Wave旭枉 and The方 Rek少ionsh徊 to F肝er Banks




              Figure 3.1 Squared magnitude frequency responses of H(w) and H(w + yr).

                                         蜘，  如如爬 忖小" 섞蜘 .
     Equation 3.80 implies that // is a Q｝뇨4F; that is, 田佃 + 兀기 is a reflection of 田佃）1
     about the quadrature frequency (namely, w = 兀/2). However, not every QMF
     satisfies the power complementarity property. A QMF that satisfies that property
     is known as a perfect reconstruction quadrature mirror filter (PRQMF) for reasons soon
     to be explained. The PRQMF nature of H is a direct consequence of the dilation
     equation and the orthogonality of the set { (t 中 n) : n integerl. An example of the
     squared magnitude frequency response of such a filter is shown in Figure 3.1 along
     with IH(w + 7r)I2. Since h(n) is a reflection of h(n) about n = 0, the magnitude
     frequency response of H is the same as that of H, and we have

                                      1月m끼2 + 1月佃 + 兀기2 = 1.                                     (3.81)

     Thus H is also a PRQMF. Using H(0) = H(0) = 1 in Equation 3.81 yields

                                           月伽）= H(ir) = 0.                                       位82)

     Based on the fact that their DC gain is unity and the frequency response at w = 7r
     is zero, we might conclude that H and 月 have the characteristics of LPFs.8 The
     condition in Equation 3.81 is also known as the halfband condition. A filter with a
     frequency response equal to IH(w) 2 is said to be a halfband filter.


     8 As we saw in the Haar case, they need not be good LPFs. See Figure 2.7 for plots of corresponding
     filter frequency responses for the Haar case.
                                                                          Digital Filtering Interpretation   67

    Equation 3.76 shows that the sequence b(k, n), like a(k, n), is also obtained by
filtering a(k - 1, n) with the filter G and downsampling the filtered sequence by a
factor of two. The G and G filters are also QMFs on the basis of Equation 3.43 and
the definition of g(n) and g(n); that is,

                              IG(w)I2 + IG(w + 兀기2 = I                                             (3.83)
                              IG(o川2 + IG(w + 7r기2 = I.                                            (3.84)

From Equation 3.39 and the definition of G and G,

                                       G(0) = G(0) = 0                                             (3.85)

which, in conjunction with Equations 3.83 and 3.84, yields

                                     IG@r)I = IG(兀)I = 1.                                          (3.86)

Equations 3.85 and 3.86 show that the G and G filters have the characteristics of
HPFs. Expressing Equation 3.44 in terms of the filter frequency responses we have

                       H(w)G非（w) + H佃 + 兀）G*(w + jr) = 0
                                                                                                   (3.87)
                      H(w)G*(w) +H(w+ 兀)G*(w+ 7r) =0.

Also, from Equations 3.47 and 3.48,

                                                   田佃平 + IG(w)I2 = 1
                       H*(o4H(w+ Jr) +G*(口）)G(w+ 兀) = 0
                                                                                                   (3.88)
                                                   1月(U끼2 + IG回2 := I
                       甘（w)H(w + 兀） +（芦（w)G(w + 兀） = 0.

It is important to observe that the sequences b(k, n) in Equation 3.71 are in fact the
coefficients of the DWT in Equation 3.70.
    The time domain equivalent of Equation 3.87 is obtained by substituting Equa-
tions 3.71 and 3.72 in Equations 3.15, 3.40, and 3.41:


                         /=h          (n)h(n+ 2k) =                8(k)                            (3.89)

                               t小                 I
                               ) . g(n)g(n+ 2k) = ;d(k)                                            (3.90)
                                                      +




                                nd                            乙


                         \\   ＞二h(n)     g   (n+      2k) =   0.                                   (3.91)
68   八川？A. C가／honormal Wavele朽. and Their Re/a加nsh徊 ta F肝er Banks

     The equations imply that the LPF impulse response h (n) is orthogonal to even
     translates of itself, the HPF impulse response g(n) is orthogonal to even translates
     of itself, and h(n) is orthogonal to g(n) and its even translates. A similar set of
     conditions holds for h(n) and j (n) because they are proportional to reflections of
     h(n) and g(n) about the origin respectively.


     3.5.2 Recon針ructing the 없gn이
     From Equation 3.56 and the two-scale relations for the scaling function 砂 (t) and
     wavelet 少(t), we have

                                      00   的

                       工1(t) = ＞二 ＞二 a(O, t)c(m）中（2t+ 2Z - m) +
                                  片i==ma그 t==H仗）

                                      00   的
                                                                                    (3.92)
                                   ＞二 ＞二 b(O, t)d(m）砂（2t - 2t - m).
                                 m= -oo f= -00



     Substituting n = 2t + m in Equation 3.92 we get


                        兀1(t) = ＞二 ＞二 a (O, Z )c(n小2Z）中（2t - n) +
                                   n= -仗）t＝니刃

                                      00   的
                                                                                    (3.93)

                                      ＞二 Zb(O, t)d(n - 2t)中(2t - n).
                                   n= -以）t=＝니乂




     "'"' """"援：客蹄茸밖                                      ，
                    a(-1,n) = ＞二 a (O, t)c(n- 2Z) + Z b(O, Z)d(n- 2t)               (3.94)
                                t= U0 )                   e==e아그



     which can be rewritten in terms of h(n) and g(n) as

                                 00                          的
                                                                    他
                                                                    b       m
                                                                            g   끄
                  a(-1, n) = 2 >二 a(O, t)h(n - 2t) + 2 Z b(O, t)g(n - 2t).          (3.95)
                                                                        P
                                                                        L                    H
                                                                                                 )
                                                                                                 /
                               肛＝-00                       t= H以）



     Let


                                 a(O, n) =     ＞二 .(0, Z )c(n中2t)
                                               e= m以）

                                                   的
                                                                                    (3.96)
                                 b(O, n) = Z b(O, Z)d(n - 2t)
                                               t= 1 (X)
                                                                        미아이F肝e月四 幻向pretc批on                 69


  Now consider the expression for a (0, n) in Equation 3.96. Expanding the right-
hand side of this expression we get

        a(0, n) = . . .+a(0, 0)c(n) +a(0, 1)c(n -2) +a(0, 2)c(n -4) +. ...                       (3.97)

This can be rewritten as

        a (O, n) = . . .+a(0, 0)c(n) +0c(n -1) +a(0, 1)c(n -2) +0c(n -3) +
                                                                                                  (3.98)
                    a(0, 2)c(n -4) + . . . .

Equation 3.98 can be interpreted as inserting zeros between adjacent samples of
the sequence a(0, n) and filtering the resulting sequence with c(n). As described
in Chapter 2 this process of zero insertion is called upsampling and is depicted in
Figure 2.8. An alternative interpretation is that of interpolating a(0, n) using the
filter H, followed by scalar multiplication by a factor of two.9 We refer to this
process as interpolating a (0, n) with 2H. In a similar fashion, the sequence b(n)
can be obtained by a factor of two interpolation of b(0, n) using G, followed by
scalar multiplication by two. Let us refer to this process as interpolating b(0, n)
with 2G. Therefore by Equation 3.94, a(- 1, n), the sequence of coefficients used
for expanding f_1(t) in terms of the basis for V_1, can be obtained from a (0, n) and
b(0, n) by summing their scaled interpolations using the H and G filters respectively.
Equations 3.95 and 3.96 can be generalized to any integer k:

                           '7 a(k, n) =2a(k+ 1, n) +2b(k+ 1, n)                                  (3.99)

where

                                               的

                       /     a(k+ 1, n) 三 ＞二 a(k+ 1, Z)c(n - 2t)
                                             t＝中以）
                                               m
                                                                                                (3.100)
                       / 石（k+ 1, n) 三 ＞二 b(k+ 1, Z)d(n - 2t).
                                             t= -oo


  Figure 3.2 shows the general structure of decomposition and reconstruction. The
H and G filters that are associated with decomposition form what is known as the
analysis filter bank. Similarly, the H and G filters that effect reconstruction form
the synthesis filter bank. Because the sequence going into the analysis filter bank is


9Some authors define 九（n) = c(n)／시恒了 and g(n) 프 d(n)/,./臣了. With 石（n) 三 力（-n) and g(n) 三 g(- n),
this definition leads to decomposition being effected using the 月 and G filters, and reconstruction being
carried out with the H and G filters without a factor of two multiplication.
70   MRA, O片honorma/ 너／dvelets, and Their Re/a加nsh徊 幻 F肝er 的nks




                                                            2
                   n(k   1. n)                      a(k,n) r
                                 > I?( -ii)   >      >   >      H+   助（'I
                                                                                       Li（大   1.ii)




                                          )                     나
                                                                     2g
                                                    b伐, 7i) \7
                                                                                   -




                                                                             1   b (k」川
                                                                       (n)
                             寸       （.
                                                             2


                             Analysis bank                   Synthesis bank


             Figure 3.2 An이ys捻 and synthe이S 셰ter banks.



     recovered perfectly by the synthesis bank, these filters form a perfect reconstruction
     pair (hence the name perfect reconstruction quadrature mirror filter banks).


          d\r：起
     3.6 Examples of Orthogon이 的引s-Generating Wave回＄
     So far we have seen one concrete example of a wavelet that can provide an orthog-
     onal decomposition-the Haar wavelet. But there is an infinite number of wavelets
     that can provide an orthogonal basis. Associated with these wavelets are scaling
     functions. As in the general development of the previous sections, the scaling func-
     tion defines the MRA and the associated filters H and H. More importantly, the
     wavelet is derived in a simple manner from the scaling function, as we show next.
        Suppose we have a scaling function 砂(t) that satisfies all the properties associated
     with the scaling function of Section 3.3. Then, from the definition of the frequency
     response of H and Equation 3.82,


                                              二 H) " 九（n) = 0.                                        (3.101)
                                               /1



     Suppose we set


                                                                                                      (3.102)


     Then, Equation 3.102 and the fact that H and H satisfy power complementarity
     imply that G and G also satisfy this property and hence are QMFs EMintzer 1985;
                                                Exam히es可On'h四on（카助諸-Gener아奴7Wavele朽                 71
                                Table 3.1 LPF Coefficients for D4


                                      fl               h(n)
                                      0             (1 + V互）/8
                                      I             (3 + \／중）/8
                                      2             (3- .J)/8
                                      3             (1- /)/8


Smith and Barnwell 1986; Vaidyanathan 1992]. Furthermore, Equations 3.87 and
3.88 are also satisfied. Finally, the wavelet 砂 0') is obtained using Equation 3.38 as

                                               的

                                 少（t) = 2 兄 g(n）中（2t- n)                                  (3.103)
                                              n=-느的




3.6.1 Daubechies D4 Scaling Function and Wavelet
The plot of the D4 wavelet [Daubechies 1988, 1992] shown in Figure 3.3 is perhaps
the picture that is most associated with the term wavelet.10 The LPF associated with
this wavelet is of the finite impulse response (FIR) type of length four (hence the term
D4). The nonzero coefficients of the impulse response are listed in Table 3.1. The
corresponding HPF g(n) is obtained from Equation 3.102. Figure 3.3 also shows the
D4 scaling function. Neither the scaling function nor the wavelet has a closed-form
expression. They are both of finite extent; that is, they are identically zero outside of
a finite interval on the time axis. Such f끄lctions are said to be supported
                                                                              compactly.
Figure 3.1 shows the squared magnitude frequency response of the H and G filters
corresponding to D4 (IG(w)I = 1H(w) + 川).


3.6.2 Bandlimited Wavelets
The orthonormal basis-generating wavelets seen so far, Haar and D4, are both
supported compactly in time. It is possible to have orthonormal basis-generating
wavelets that are bandlimited; that is, their Fourier transforms are supported com-
pactly in frequency [Meyer 1993a]. Let us begin with a simple example. Let


                                           中（t) =   sin兀t.                               (3.104)
                                                      7i 1




10 Some authors use the term D2 instead of D4. The reason for the use of t曲 terminology
                                                                                        wil比ecome
clear in Chapter 7. A formal method for designing the LPFs associated with the Daubechies scaling
functions is presented in Chapter 7.
72   八月／?A. （가than아m이 너／Ovelets. and 了he肛 尸el<그tionsh徊 to 尸／ter Banks




              Figure 3.3 Scaling function (A) and wavelet (B) generated using the D4
                         filter



     Its Fourier transform, given by

                                             Ii       1口71 드 兀
                                      中nm' = { m                                       (3.105)
                                        "       10
                                                      otherwise

     is bandlimited to the frequency range -7r 三 cv 드 7r. It also satisfies the Poisson
     summ仙n 的rm岫. in Equatio心．孕mnd可ing th"쁘（t) and. its mnt텍르『 t『켓「lat「，「
     are orthogonal. In tact, qt) satisnqs tne ortnonormamy concunon in nquation 그 .
                                                            7\
                                                                          Exam히es可O川）ogonal的弱＜3ener<川ng 너／'avelets                              73

        If it were also to satisfy the two-scale relation, it would qualify as a scaling function.
        Let us verify that it does by substituting Equation3뀨 into Equation,
                                                                            3.10,
        transrorming it into me rrequency aomain. vv e are iooKing ror a niterj   and, then
                                                                                ii witn an
        impulse response h   (n)
                                          such that                                                 .
                                                                                                        +    .    -   Ctm)
                                                                                                    yvn) 二            {:m
                                                                                                                                 1四
                                                      砂（t) = 2＞二九（n）中（2t -兀）.                                                ' " ' "+ (3.106)
                                                                          n


        Equation 3.106 can be rewritten as


                                                  中띠2) =2Z蜘欣t- 札）.                                                                     位107)

        By taking the Fourier transform of both sides of Equation 3.107 we obtain the fre-
        quency domain equivalent of the two-scale relation

                                                            中(2w) = H(w)4) (w)                                                        (3.108)

        where H(w) is the frequency response of H. All we now need is a function H(w)
        that satisfies Equation 3.108. Rewriting Equation 3.108 as

                                                                     （2幼
                                                             H(w) = 으          14J ( (iJJ
                                                                                                                                      (3.109)

  and using Equation 3.105 we have the required H(w) as



                         \
                                                  月
                                                      （w)
                                                             =
                                                                     {    d
                                                                          l

                                                                          n
                                                                          U
                                                                              Ic기 드 吾
                                                                              즉 < I끼 三 7r
                                                                                                                                      (3.110)

which
      is an ideal LPF      cut 。ff fre uency
                                   with
                                                It can   verified that H   satisfies
                                                                                   r/
                                                                                               2.
                                                                                                             be
the PRQMF property.
                                                                                                                                (w)
                                                                 q
   Now that we know that 砂 (t) is a scaling function, what about the corresponding
wavelet? We again operate in the frequency domain to find the wavelet. By taking
the Fourier transform of both sides of Equation 皿？, we have its frequency domain
equivalent:                                                                        和）＝더r岫川
                                                      G(w) = e_.boH* (w +兀).                                                          (3.111)

For our ideal H(w),

                                                      (w)I-                                             7r
                                                                                                                                      (3.112)
                                                                     {1
                                                                                        <IwI
                                                                          。
                                             IG
                                                             -                wj
74   MRA, Orthonorma! Wavele厄 and The／시？e／아幻nsh徊 幻 F肝er Banks

     which is an ideal HPF. The G filter is also a PRQMF. With 山(w) being the Fourier
     transform of the wavelet, the           domain version of Equation 38 is given by    3.
                                                                      ?        d( i '
                                   frequency
                                                                                  ?#tt)
                                                                                       [小

                                                                     知）＝曾' "三；
     Substituting Equations 3.105 and 3.111 in Equation 3.113 yields
                                                                             ‘茹1，貫4

                               山（.）니？
                                    i．글 !，디이，
                                            드2ir       U     O[1ler1VlSe   '
                                                                                               (3.114)


     The scaling f끄lction and wavelet are shown in Figure 3.4. Because of the association
     of the sinc function with sampling theory, the scaling function shown in Figure 3.4
     is known as the Shannon scaling function, and the wavelet is known as the Shannon
     wavelet in honor of Claude Shannon, who played a pioneering role in the devel-
     opment of the theory associated with reconstructing continuous-time signals from
     their samples [Daubechies 1992; Shannon 1949; Zayed 1993].
        The first orthonormal wavelets were constructed by Meyer E1993a1 and they were
     bandlimited. Although the construction is often presented using trigonometric poly-
     nomials, we take a simpler approach here [Chapa 1995; Vetterli and Kovacevic 1995].
     Iet (t) be a real-valued function with a Fourier transform 中(w) that satisfies the
     幻如wing:

      1. It is real and positive in the range 1wi 드 47r/3 and is zero at frequencies outside
         this range. Because 1 (w) has been assumed to be real, 中(t) is symmetric about



                                                                                                         {
         the origin. It also follows that 中(w) is itself symmetric about w = 0.

      2. It is smooth in the sense that 中(w) is differentiable.

                                               m 上
                                               l m
      3.
                                                                    0 < wi <2r/3
                       呻佃）2 =                        小 呻（2兀 -U끼2    2ir/3< k끼 < 由r/3           (3.115)
                                                0
                                                                    other汭／ise.

     This type of function satisfies the Poisson summation formula in Equation 3.18.
     Thus, 中(t) and its integer translates form an orthonormal set. It can be shown that
     any bandlimited scaling function necessarily satisfies the Meyer bandlimit [Chapa
     19951 (see Problem 7). The function H(w) obtained by substituting such a 中(w)
     in Equation 3.109 is the frequency response of an LPF with cutoff frequency 2ir/3
     rad. Furthermore, it is real-valued and satisfies the PRQMF property. Thus, its
     impulse response serves as the coefficient sequence of the dilation equation for
     中(t), indicating that it is a scaling function for an orthonormal MRA.
                                       Examples of Orthogonal Basis-Generating Wavelets   75




     l




                                                                               (A)
                 -10         -   5       0          5          10       15




                                 1       1          1          1               (B)
                 니0
                             -5          0          5          10       15
                                         r


Figure 3.4 The Shannon scaling function (A) and wavelet (B).
76    MRA, Orthonormal Wavelets, and Their Relationship to Filter Banks

        The Fourier transform W (cv) of the corresponding wavelet is generated using
      Equations 3.111 and 3.113. Combining these two equations,

     命力： 可；WU (t4十it)
     耳如昑 q（勤 ' 致劫
                                                                山        （cv)         ＝     可     jw/   ‘   2H*           （을＋                           7)           m   (cv/       2)      .
                                                                                                                                                                                                     (3.116)

      Because H has a real-valued impulse response as well as a real-valued frequency
      response,

                                                                                      H(7r + cv) = H(7r - cv).                                                                                       (3.117)

      Substituting Equation 3.117 in Equation 3.116 we have


                                                                山回 =/"/'月G 욜）中畔）·                                                                                                                    (3.118)


      Substituting
                             Equatio               3.       109 in Equation                                          3.
                                                                                                                            118 we                            get
                             11W) 七

                                                            )11                                         j0/2 cI:          (2, jr                    cv
                                                                                                                                                              ) (cv/                                 (3.119)
                                                                                                                                      -,
                                                                                                                                                             2)
                                                                                             e_
                                                                                                                                                                    2)
                                             玉b.                           (w)        -                                                                             c1
                                                                                      -                                    r-              cv       /                                   .




      Using the properties presented earlier for 中(cv), Equation 3.119 yields for cv 三 0

                                                                    [ e_3w/2中（2兀 1 向I)                                                              27r/3 < 1n기 5 由r/3
                                  山   （cv)         =        I               可 '   '
                                                                                           '2m (IcvI/           2)                                  47r/3 < 1n기 드 勘r/3                               (3.120)
                                                                    (0                                                                              otherwise.

      The inverse Fourier transform of 山(cv) is the Meyer wavelet 少 (1) associated with
      the function 中(cv).
      Example 3.1
                     Let


                                                                                                        , ;.，』 , ,
                                                    뽀（W) = 1 드0s＝寸                                                                                                                                   (3.121)
                                                                                      11                                        으5，         尸드2兀／                               3   .           ,.




                                                        :   .        .

                                                                                                                                UT/i5삔542T/i
                                                                                      Lu                                        k끼 三 4Jr／三


                     This function satisfies all the properties of the Fourier transform of a Meyer scaling
                     function. Its inverse Fourier transform is the scaling function 中(t), shown in Figure 3.5.
                     Also shown in Figure 3.5 is the wavelet obtained by the inverse Fourier transform of
                     w .cv), wrncn is ootainea rrom tiquanon 三 IUU.                                         -

           We see that the Meyer wavelet is bandlimited to the frequency range 2ir/3 5
      Icv I <8ir/3. Therefore, the corresponding wavelet 砂 (t) is of infinite duration in time,
      although its amplitude decays rapidly, as seen in Figure 3.5. As a consequence, the
                                          Examples of Orthogonal Basis-Generating Wavelets   77




Figure 3.5 The Meyer scaling function (A) and wavelef (B).



H and G filters are of the noncausal h1R type. This has been seen as a disadvantage
in using Meyer scaling functions and wavelets in practical applications. However,
there are several situations related to sampling theory when Meyer-type scaling
functions arise naturally [Bopardikar, Raghuveer, Adiga 1997a, 199Th]. One such
application, related to the choice of signaling waveforms for bandlimited digital
communication channels [Jones 1994; Jones and Dill 1998a, 1998b], is discussed in
Chapter 6.
78    MRA, O斤honorma/ 너／avele朽. and Their Rek少幻nsh徊 幻 F肝er Banks

      3.7 Interpreting Orthonormal MRAs for
          ［기＄crete-Time 이gn이＄
     In Section 3.4 we showed that a DWT can be associated with an MRA. The MRA
     itself consists of nested vector spaces of continuous-time functions. In many appli-
     cations the signal to be wavelet transformed is a discrete-time signal. The practice
     is to perform decimation as described in Section 3.5 on this discrete-time signal and
     offer the resulting sequences (the ones corresponding to b(k, n) of Equation 3.76) as
     the "wavelet transform." Let us call such a transform a discrete-time wavelet transform
     (DTWT) EVaidyanathan 1992]. We now pose the following questions:

       1. Can the DTWT be reconciled with our development of the DWT as a repre-
          sentation of a continuous-time signal using discrete (that is, dyadic) dilations and
          tr跏쁘竺프L끄쁘地Q끄邑迦姐虹
       2. Is there an equivalent MRA interpretation for the resulting sequences?

     3.7.1 Continuous-Time MRA Interpretation for the DTWT

     To answer the first question, let us begin with a discrete-time signal, say f (n).
     Define

                                                 的

                                    f (t）三 Z f (n）中（r1兀）                              (3.122)
                                              n==H的


     where 中(t) is a scaling function that gives rise to an orthogonal MRA of the type
     discussed so far. Let fk (t) denote the projection of f (t) on the subspace Vk. Then,
     玖／ith

                                p(k, n) 三 2_k(f (t), 中(2_kt - n))                     (3.123)

     we have

                                          的

                                且（t) = ＞二 p(k, n）砂（2 "t - n).                         (3.124)
                                        n= - 的


     In particular,

                                         f (n) =p (O, n)                              (3.125)

     which implies that f (t) E V0. In turn, by the nesting of the subspaces, it follows
     that

                                              f (t) E Vk                             (3.126)
                                                    Interpreting Orthonormal MRAs for Discrete-Time Signals        79

for k < 0. Let ,k(t) be the detail function at level k, and q(k, n) be the coefficients
of its expansion11 in terms of the appropriately dilated and translated wavelets. As
we have seen, the sequence p(k, n) is the output of the H filter at the kth level.
Similarly, q(k, n) is the output of the G filter at level k. By Equation 3.126,

                                                       gk(t) =O                                     (3.127)

for k < 0, which implies that

                                                     q(k, n) =0                                     (3.128)

for k < 0. Therefore,

                                               00       的

                               f (t) = 51 Y ' q(k, Z )砂 (2_lct - t)
                                           k= H以）t==m以）

                                           以J        （刃
                                                                                                    (3.129)
                                       = ＞二 ＞二 q(k, Z）砂（2_kt -t).
                                           k= 1 t =-아그



Thus the DT사T of f (n), which essentially consists of the sequences q(k, n) for
k > 0, can be interpreted as the DWT of the continuous-time signal f (t) defined in
Equation 3.122.


3.1.2 Discrete-Time MRA
We now provide an MRA interpretation for the DT사T of f (n). Let fi(1, n) and
4(1, n) respectively be the outputs at level one of the reconstruction filters 2H and
2G (Figure 3.6). Substituting k = 0 along with an appropriate change of variables
in Equations 3.99 and 3.100,


                                  m끄
                                       l   n         1
                                                     /\ /m \ /m                                               )=
                                                     n
                                                     乙
                                                               p(l, Z )h(n - 2t)
                                                     즈＼     즈＼ 1
                                       1




                                       曲                      m
                                                              /
                                  m
                                  口1
                                                       ＝나rL    q(1, Z)g(n - 2t)                               =

                                                              二 L
                                                              n r




and (see also Equation 3.125)

                                 f (n) = p(O, n) = 戶(1, n) + 4 (1, n).                              (3.132)



llHere, p(k, n) and q(k, n) play the roles of a(k, n) and b(k, n), respectively, discussed in Section 3.5.
80   MRA, O片加norn何 Way이e加. and Their Relationsh徊 to F肝er Banks




       Figure 3.6 테ter bank s打ucture 向ra three-Iev이 D1WT. (A) An데ys恰 的nk.
                  (B) Syn卄）es恰 bank.


        The sequences 戶(1, n) and 4 (1, n) are orthogonal to each other since h (n - 2Z)
     and g(n - 2t) are orthogonal sequences according to Equation 3.91. Suppose we
     carry out the DT사T decomposition down to K levels. Figure 3.6A shows decom-
     position for K = 3. The resulting DTWT coefficient sequences (that is, the outputs
     of the decomposition filter bank) are the sequences q(1, n), q(2, n). . . . .q(K, n), and
     p(K, n). Let 5(K, n) be the final output of the synthesis filter bank with all the
     q(k, n), k = 1, . . ., K forced to zero. See the illustration for K = 3 in Figure 3.7A.
     The sequence 戶(K, n) can be regarded as the coarse approximation at level K to the
     input f (n). Similarly, let 4 (m, n) denote the final output of the synthesis filter bank
     with p(K, n) and all the other q(k, n) (that is, for 1 <k < K; k 尹 m set to zero [see
     Figure 3.7B1). The sequence 4 (m, n) is the mth level discrete detail of f (n). By the
     linearity of the synthesis filter bank,
                                              K

                                   f (n) => 批，n)＋可兀n)                                 (3.133)
                                          k=1

     Letting 尺 수 00
                                         00            的


                                /（凡）=＞二4 (k,n) = ＞二 q（凡n)                             (3.134)
                                        k=1           k＝尸以）
                                     Interpreting Orthonormal MRAs for Discrete-Time signals   81




    Figure 3.7 Ex（그n）히es of generation 아 appn功(ima加n and det게 functions 幻r
               a DT\NT for 戶(3, n) (A) and 4 (2, n) (B).



where

                                       4 (k, n) 三 0                                 (3.135)

for k 드 0. Also, because p(k, n) is obtained as the sum of an interpolation of the
sequence p(k +1, n) with the filter 2H and an interpolation of the q (k + 1) sequence
with the filter 2G.

                           戶(k, n) = 4(k+ 1, n) + 戶(k+ 1, n).                       (3.136)

Again, the sequences 戶(k, n) and q(k, n); k = I. . . . .K are mutually orthogonal
because of the orthogonality of h(n - 2Z) and g(n - 2t).
   Let v0 be the linear vector space of all discrete-time signals with finite energy (that
is, the space containing the input f (n)), Vk be the space containing the approximation
sequences at level k (such as the sequence 戶(k, n)), and Wk be the linear vector space
containing the detail sequences at level k (such as 4 (k, n)). As we have seen, the
sequences 4 (k, n) are mutually orthogonal for different values of k. It follows that
the vector spaces wk are also mutually orthogonal [Soman and Vaidyanathan 19931.
82   MRA, Orthonormal Wavelets, and Their Relationship to Filter Banks

     Then, by Equation 3.134



                                                     的 ＋向
                                                            k
                                              VO =
                                                            功                        (3.137)


     which is the MRA corresponding to the DTWT. Notice the similarity of structure
     between this MRA and the MRA in Equation 3.68.


     3.7.3 Basis Funct伯ns 佃r the DT叩T                    즈 n . . , ,=," .D \
                      i和泳mt坰 = 1數k) , i (Lm) = n口恥Il)下"“們V7
     From Equations'3 90 and 3.131 we see Ihat g(n) nd its even translates form an
     orthogonal basis for w1. However, by substituting k = 0 in Equation 3.90, we
     see that the norm of g(n) is 1/v'2. Therefore, it follows that the set of sequences
     h厄g(n- 2k) : k integer} is an orthonormal basis for wl. The basis for w2 is found
     by looking at how the sequence 4 (2, n) is expanded in terms of a basis. From
     Figure 3.7 it is seen that 4 (n) is obtained by two stages of interpolation of the
     sequence q (2, n)-flrst with the ifiter 2G and then with the filter 2H. Applying the
     interpolation expressions in Equation 3.96 twice,

                            t (2, n) =4Zq(2, k) Zg(e- 2k)h(n- 2t).                   (3.138)
                                         k           Z


     Define

                                      gi(n) = ＞二g(t）九（n- 2t).                        (3.139)


     Substituting Equation 3.139 in Equation 3.138,

                                  4(2, n) =4> q(2, k)瓠小 的．                           (3.140)
                                                k


     We see that the sequences gl(n) and its translates by integer multiples of four (let us
     call these the fourth translates) form an orthogonal basis for w2-the vector space
     that contains 4 (2, n). Because IIg(n)II = IIh(n) f I = 1/\/2, we require 2g1(n) and its
     fourth translates to ensure orthonormality. The definition of g1(n) in Equation 3.139
     shows that 2gl (n) is obtained by upsamp血lg ./g (n) by a factor of two and then
     cony아ving it with /死的．
        Thus, the orthonormal basis for w1 is provided by .Jig(n) and its even trans-
     lates. The basis for w2 is provided by fourth translates of the sequence obtained by
     upsampling /g (n) by a factor of two and convolving with vih(n). Generalizing
     the result, an orthonormal basis for Wk (n) consists of 2" translates of the sequence
     generated by upsampling .Jg(n), and convolving it with /h (n), then upsampling
                                       m t아re肋g 아thonon기of MRA$ 幻r｛가scre洽加e 띄on（카s                  83

the result and again convolving it with ./h (n), and so on, repeating the process
k -1 times. In other words, there is a total of k - 1 upsampling operations and k -1
convolutions involving one stage of .Jg(n) and k - I stages of /h (n). Fi엣re 3.8
shows the generation of sequences with 2' translates that yield orthonormal basis
functions for Wk. In Figure 3.8, -...三g(n) is itself initially generated as the impulse
response of a filter.
   What about a basis for vk? The process of generating basis functions for Vk follows
on lines very similar to those for generating basis functions for Wk. Recall that vk
is the subspace containing 戶(k, n), which is generated (see Figure 3.7) by passing
p(k, n) through a chain of interpolators. But for one level of interpolation, both
戶(k, n) and 4 (k, n) use the same LPF interpolator chain for a given k. The first stage
of interpolation for 4 (n) is with the filter 2G, whereas for 戶(k, n) it is with 2H.
Thus, orthonormal basis functions for Vk are obtained as in Figure 3.9 by replacing
the g(n) of the basis generation process for wk with h(n). An orthonormal basis
for the space of all square summable functions is provided by the collection of the
basis functions of Wk, k = I. . . . .K and VK for any K 之 1. Examples of such basis
functions for the D4 filters are given in Figure 3.10.




                                                  Even.translates of output are basis
                                                  Tunctions 01w1
             a(n)
                            Ig   (n)

                                           (A)

                                                         Fourth translates of output are basis
                                                         functions of w



                    Jg(n)
                                           (B)


                                                                               Eighth translates.
                                                                               9101프？11 게下 oasis
                                                                               tunctions or w3


                                                                      厄的D
                                           (C)

Figure 3.8 Generation of sequences with even translates that yield orthonormal
           bases for Wi (A), w2 (B). and w3 (C).
84    八／仄A, Orthonorm이 Wavelets, and Their Re/c川onsh徊 幻 F肝er Banks



                                                                    Even.translates of output are basis
                                                                    tUflCt1OflS 05 V1




                                                         (A)


                                                                                   Fourth translates of output are basis
                                                                                   functions of v,


                         -1h
                               (n)                             万的D

                                                         （助


                                                                                                          Ejghth trans14tes.
                                                                                                          01 OUq)UL are oasis
                                                                                                          tundilons 05 V3


                                                                          0                )




     Figure 3.9 Gener그쒸on of sequences \A／什h even fran引afes th（카 닌이d (＞什hon아nY引 的ses
                for v] (A), v2 (B), and V3 (C).




     3.8 Miscellaneous Issues Related to
         PRQMF Filter Banks
     We have shown that an orthonormal dyadic wavelet decomposition leads naturally
     to a PRQMF bank approach to finding the approximation and detail coefficients at
     subsequent levels after we have the approximation coefficients at a given level of the
     MRA. However, perfect reconstruction filter bank theory was developed indepen-
     dently of the wavelet transform. By simply starting with the structure in Figure 3.2
     and requiring that the output at the reconstruction end be equal to the input at the
     decomposition end, one arrives at the paraunitary condition [Vaidyanathan 1990,
     1992] (see Problem 14).


             [H*
                   (w)
                                     G*
                                          (w)
                                                11t1
                                                   (w)
                                                                H
                                                                    (w+
                                                                              兀)
                                                                                      1=
                                                                                               [i
                                                                                                                      (3.141)
             L I不(w + 7r)            G' (w+ Jr) JLG(w)          G(w+ 7r) J                     [U    0I   ·




     This also includes the power complementarity condition, as can be seen by substi-
     tuting the relationship from Equation 3.111 in Equation 3.141.
                                            Miscellaneous Issues Related to PRQMF Filter Banks        85



      l

                                                          0




    0.5




      0



                                    0




   -0.5                                                                                    0 (A)
          l        1.   5           2          2.5         3            3.5                4
                                                                                     n +




    0.8        1            1   1       1
                                                      0


    0.6


    0.4
                                               0


    0.2




                                                                              A)
      0
              1                                                (b
                                        0
  -0.2


   -0.4

                                                                    0
   -0.6                                                                                         (B)
          0   l             2   3       4      5      6        7    8         9            10
                                                                                   n1+
Figure 3.10 Functions with tran訊카es 十h아 化什i) the 1：泊S's 向r i刃］ (A) and W2 (B).
86   八4尸A, Orthonormal Wavele朽. and Their Re/a加nsh徊 幻 F肝er Banks


              a   '
                                1                 1
                                                                  0


                                                          0
              0.4
                                                  0


              0.2



                                         I I
                          '古nn!,                                              !            '                 "
                  0                                                                            ,   早，
            -0.2



            -0.4




             U"U0              5              10                          \       15               20                     25 ' V'
                                                                                                                     n+


                           1                      1                   1           1    1                1        1




                                                                  0
                                                              0
                                                          0
                                                      0
                                                  0

                                             C)                       0

                                         0



                                         우                                우                .., d9. . ..
                      "놔堀싸싸！,!                                            古            F"                   "'"


                      0    5   10   15        20                  25              30   35          40        45           50
                                                                                                                     n+



         F勾we 3.10 (continued) Functions ＼八／
                                           ith 加耐아邰 th아 幻rm the ba引Sf아 功3 (C) and
                   W4 (D).
                                         凡까scellaneous Issues Related to 끼？Q八席 F肝erBanks   87




    Figure 3.10 (con力nued) Functions with 的n訊그tes th（카 幻rm the t刃sis 幻r v4 (E).



   The orthogonality condition in Equation 3.20 rules out the possibility of FIR filters
of odd length for H. We show this by a simple example using a length-three filter.
Suppose h(n) has values a, b, and c for n = 0, 1, 2 respectively, and zero for all other
values of n. Then, by the requirement that the autocorrelation sequence of h(n) be
zero at even lags (see Equation 3.19), we have ac = 0, which leads us to set either
a = 0 or c = 0, rendering the filter length even. The example is generalized easily
to all other odd values larger than three. Also, the orthogonality condition leads
to trivial filters if we insist on linear-phase FIR filters. The linear-phase property
is equivalent to requiring symmetry. Consider, for example, a symmetric filter of
length four, say with impulse response values (a, b, b, a). Again, the requirement
of the autocorrelation of the impulse response being zero at even lags leads to the
condition ab = 0 at lag two, which means b = 0. Thus, the filter has only two
nonzero coefficients-a result that can be generalized to symmetric filters of other
lengths.
   As explained in Section 3.5, one level of the DTWT of a given sequence is corn-
puted by passing the input sequence through the H and the G filters, and downsam-
pling the results by two. Now, let the input x (n) be an N-sample sequence. Also,
suppose that H and G are FIR filters of length L. Then the convolution of x(n) with
the H and G filters will give low-pass and high-pass sequences of N + L -1 samples
88   MRA, Orth아力rmal W亡yvelets, and Their Relationsh徊 幻 F肝er Banks


     each. Downsampling these sequences gives two sequences of length f(N+ L - 1)/2]
     where [.1 rounds the argument to the next higher integer. Clearly, the total number
     of samples at the output is greater than the total number of samples of the input
     sequence. Thus, the DT사T based on the linear convolution does not conserve the
     number of samples. In applications involving finite-length signals or images, it is
     necessary to conserve the total number of samples [Smith and Eddins 19901. One
     way of doing this is by replicating the signal at the boundary. In other words, we
     create a sequence i (n) such that


                       i (n + pN) = x(n)                         0 5 n 5 N - 1, p, integer.        (3.142)

     This is known as a circular or periodic extension of the input sequence [Karlsson
     and Vetterli 1989; Smith and Eddins 1990]. Convolution now amounts to finding
     the circular convolution of the input sequence with the H and G ifiters [Oppenheim
     and Schafer 1989]. This type of extension is shown in Figure 3.11. The output of
     the H and G filters for such an input would also be N-periodic. Downsampling
     these sequences would give two sequences that are N/2-periodic. Thus, only N/2
     samples of each of these sequences need to be retained. This preserves the number
     of samples. The synthesis of the original sequence involves upsampling of the



                                          工（n)




                                                                                              >
                                                                                              fl


                                                                 (A )



                                            \ (fl




                         1n
                                     1
                                     ii
                                                    ,ii
                                                                                              >
                                                          liii
                                                                                              '7
                              liii
                                          11I
                                                                 (B)

          Figure 3.11 Origin이 이gn이 (A) （긔）d circul아 exten針on of the sign이 (B).
                          Genera枷g Sc에ng Func掖 'ns and Wavele朽 from F肝e八力e所口ents         89


two N/2-periodic sequences to give N-periodic sequences, passing these N-periodic
sequences through the H and G filters and adding the results. This gives i (n) from
which x(n) can be extracted. Note that for the circular extension process to work,
it is necessary that the input sequence x(n) have an even length. If this is not the
case then the downsampled sequences will not be N/2-periodic and the number of
samples will not be conserved [Smith and Eddins 19901. Extending our analysis
from the one-level decomposition case to M-levels we find that at the kth level the
sequences are N/21-periodic. At each level it is necessary that the sequences be
divisible by two, so that the next level of decomposition can be effected. Thus, it
is necessary that the length of the input sequence to an M-level filter analysis bank
be divisible by 2M


3.9 Generating Scaling Functions and Wavelets
    from Filter Coe州cien朽
Repeated application of Equation 3.108 leads to

                           1' (w) = H(w/2) H(w/4) .. . H(0)                   (3.143)

where we have set 中(0) = 1. Suppose we are given the coefficients of the impulse
response of a discrete-time filter h (n) satisfying the paraunitary conditions. The
sequence 2h (n) can serve as the set of coefficients for the dilation equation to gen-
erate a potential scaling function 中(t) for an orthonormal decomposition. In fact,
if substitution of the frequency response H(w) in the right-hand side of Equation
3.143 leads to a function 中(w), then its inverse Fourier transform is such a scaling
function. There is a simple time-domain iteration method based on this result. The
steps of the algorithm are EDaubechies 1988; Strang 1989]:

 1. Set c(n) = 2h(n).
 2. Let the initial scaling function be the Haar scaling function:

                                                  0< t< 1
                                中叭t) = { ,l
                                 .   .   .   11
                                       Lu         otherwise.

 3. At iteration n set

                              仇(t斥＞二c(t）仇크m 그
                                             f

    In other words, use the dilation equation to generate the scaling function of the
    next iteration.
90   八1RA, Orthonormal Wavele朽. and Their 尸elat幻n計）徊 to F肝er Banks


      4. Iterate until either divergence is established or the desired convergence is ob-
         tamlled. If there is convergence, the scaling function is given by

                                          中(t) = uirn 4) (t).                 」        (3.144)
                                                  n-+oo

        The issue of whether one can test for convergence even before the algorithm is
     applied is addressed in Chapter 7. The basis for the algorithm is actually given by
     Equation 3.143. Transforming the iteration to the frequency domain, at the end of
     the first iteration,

                                     1i(W) = H(w/2)c10(w/2)                            (3.145)
     where CI, (w) denotes the Fourier transform of the scaling function at the nth itera-
     tion. The function b0 (w) is the Fourier transform of the Haar scaling function. After
     the second iteration we have

                                (lh(nD = H(w/2)H(w/4)中o(w/4).                          (3.146)
     Repeated iteration eventually leads to Equation 3.143. Figure 3.12 presents a
     MATLAB program that can be used to generate the scaling function and wavelet
     given the filter coefficients h(n).


        % m file to generate scaling function and wavelet from the h filter.
        % specify $h (n) $ in array called h and then call this m file.
        % For D4 use h in Table 3.1.
        sizeh=length (h) ;
        co=2*h; do= (_ l) . 八 (O: sizeh_ l) .*co (sizeh_ (O: sizeh_ l) ) ;
        sampunit=32; sizphi=sampunit* 佃izeh4l) ; sizpsi= sizphi;
        phi=zeros (l, sizphi) ; psi=zeros (l, sizpsi) ;
        phi (l: sampunit) =ones (l, sampunit) ;figure (1) ;plo七 (phi) ;
        phitemp= zeros (l, sizphi/ 2) ; psitemp=phitemp;
        for k=l: sampunit,
            phitemp = phi (1: 2: sizphi) ;phi= zeros (1, sizphi) ;
            for l= O: sizeh-1,

       phi (sampunit/ 2*1+1: sampunit/ 2*l+ sizphi/ 2) =phi (sampunit/ 2*l+ l: sampunit/ 2*
       l+ sizphi/ 2) +co (l+ l) *phitemp;
       end
       if   (rem (k, 2) == O) figure (l) ;plot ( (O: length (phi) -l) /sampunit,phi) ;
          end
       end
       phitemp = phi (l: 2: sizphi) ;
       for 1=O: sizeh-1,
       psi (sampunit/ 2*1+l: sampunit/ 2*l+ sizphi/ 2) =psi (sampunit/ 2*l+ l: sampunit/ 2*
       l+ sizphi/ 2) ido (1+l) *phitemp;
       end
       figure (2) ;plot ( (0: length (psi) -1) /sampunit, psi) ;


     디gure3.12 Codef아 generc그卄ng scaling functic가기 （가）d 낚／O\／쉬et.
                    Generating Scaling Funct幻ns and 너／avele朽 /rom F肝e八力e所dents   91




Figure 3.13 Cu作）ut of fi田十 three 汁era枷＞nS 向rthe D4 Sc에ng function.
92   MRA, Orthonorm이 Wavele旭 <7nd The／기徊에on的徊 幻 F肝er Banks

       Outputs of the first few iterations for the D4 scaling function are shown in Fig-
     ure 3.13. After the scaling function is generated, the wavelet is obtained from
     Equations 3.38 and 3.102 with d(n) = 2g(n).


     3.10 Problems
      1. As mentioned in the text, set A is said to be dense in B if for every element b e B, we
         can find an element in A that is arbitrarily close to b. The example in the text shows
         how the set of rationals is dense in the set of reals. Can you give two more examples of
         one set being dense in another?
      2. Show that the union of the subspaces..., V1, V0. V_1, and so on in Equation 3.12, is dense
         in the space of square integrable functions L2(R).
      3. Using axioms 3 and 4 of MRA, show that if f (t) E %, then f (t - 2卜3n) E V for integer n.

      4. Suppose we attempt to form a vector in Vk for some k using a sequence a(k, n) as

                                                    的


                                        fk(t) = Z a(k, n) (2 "t - n)
         where 中(t) is the scaling function associated with an orthonormal MRA. Show that fk(t)
         has finite energy if and only if the sequence a (k, n) has finite energy; that is, it is square
         S1끄1끄nab1e:


                                              ＞二Ia(k,   n)   ' ＜的·




     （鉀， 昞,如t i,f (t) 帥이뜨inte畔, tr叩蜘sf帥 叩 耐伽rmal set-th計 is, 佃（!),
      끼V甲（J - t刀 = o(t) -tnen it sausnes tne roisson summation rormuja

                                             (X그


                                             Z 呻（아2兀t)I2 =I
                                            t= H的



         where 中(w) is the Fourier transform of 中(t). Hint: The autocorrelation of 中(t) given
         by R(r) = (中(t), 砂(t - r)) when converted to a discrete-time sequence by sampling at
         unit lags is, by orthonormality, the discrete unit impulse function. Use the result from
         sampling theory that relates the Fourier transform of the sampled signal to the Fourier
         transform of the original continuous-time signal.
      6. Show that the converse of Problem 5 is also true: If a function satisfies the Poisson
         summation formula then the set of its integer translates is orthonormal.
      7. Show that any bandlimited scaling function that satisfies the dilation equation (Equa-
         tion 3.106) is bandlimited to the frequency range I끼 드 47r/3 (the Meyer bandlimit)
         [Chapa 19951.
      (3If X (w) is the Fourier transform of a discrete-time sequence x(n), show that the Fourier
         transform of its downsampled version x(2n) is [(X(w/2) + X(w/2 + 兀)1/2.
                                                                                                Problems     93


             G)Derive Equation 3.22 using the result of Problem 8.
         10. In this problem we generalize the dyadic case to the M-adic case. Suppose we had a
             scaling function that satisfies the dilation equation

                                              叭t) = M＞二九（k）中（凡ft -七）·

                This scaling function would have M - 1 corresponding wavelets 吻 (t). ... . 砂M_1(t) that
                would satisfy similar M-adic dilation equations:

                                             吻（t) = M＞二g,(k）中（Mt - k).
                                                         Ac


                The scaling 血nction 中(t) and the wavelets *(t) , I = 1. ... .M - I are orthogonal to
                their integer translates. Derive the corresponding paraunitary conditions satisfied by the
%4
     }t'U9      filtersh(n) andgi(n),i= 1. ... .M 小1.
        /ii) Suv1）。se 小(t) is a scaIin2 functi。
                                              n that gives rise t。an 。rth。
                                                                         n。rmal MRA. W。uld y。u
         나 then say that 中(- t) also gives rise to an orthonormal MRA? How about 中0 - m) where
             m is an integer?
       原        If 砂(r) is a wavelet ass。ciated with an 。rth。
                                                            n。rmal MRA. can we then ret1ace 砂(t) by
       V        -砂(r) and still get the same MRA? Repeat the problem for 少(- t) and 砂(t - m) where
                m is an integer.
         13. Show that
                                                              00

                                                呻（co)I2=＞二呻（2/cw)I2
                                                              k=1


                Hint: First show that

                                             呻佃）12= 1 t (2w)l2 + IAcIJ(2w)I2.

         14. Consider the analysis and synthesis ifiter bank system shown in Figure 3.2. As noted in
             Section 3.8 we can arrive at the perfect reconstruction conditions for this arrangement
             without invoking its connection to wavelet transforms and MRAs. Let x (n) be the input
             and x,(n) be the output. Express the Fourier transform X,-(w) of the output Xr (fl) of the
             system in terms of the filter frequency responses H(w) and G(w) and input signal Fourier
             transform X(w). Show by equating Xr(W) to X(w) that the necessary and sufficient
             conditions for perfect reconstruction are the paraumtary conditions of Equations 3.87
             and 3.88. You will find that the transfer function contains an aliasing term, due to the
             presence of X(w + sr), that is canceled when the paraunitary conditions are satisfied.
         (B) Run anal given in the disk provided with this book with the input sequence

                                                                    "'256
                                                      f (n) = e                                    (3.147)

                0 드 n <255, to generate a DT人／T of that sequence down to four levels. Verify perfect
                reconstruction by running synth.
94   MRA, Orthonormal W口vele加，and The肛 Re/c力幻nsh徊 to F肝er Banks

     (ia Using the DTWT c。  efficients 。btained in Pr。
                                                     blem 15. generate the discrete multires。
                                                                                            lu-
         tion approximations and detail sequences at vanous levels as in Figure 3.1. use synth
         for this purpose. Compare details and approximations at various levels with the input
         signal.
     G)   Run  MATLAB c。 synth
                          de        with  impulse inputs   as
                                                            in   Figures 9 and 3.10 t。
                                                                       3.             generate
          the basis functions for the DTWT for a three-level decomposition.




                                                                                                  ＼뇨
                           CHAPTER FOUR


               Alternative Wavelet
                 Representations


4.1 Introduction
 Chapter 3 developed a framework for the DWT of a one-dimensional signal using
 orthogonal MRA. In this framework, the square integrable continuous-time function
 whose DWT is to be found is projected onto orthogonal linear vector spaces to create
 what are called detail functions, which also happen to be the difference between
projections of the given function onto approximation subspaces of the MRA at two
adjacent levels. The basis functions for the approximation subspaces are translations
of the dyadically dilated scaling function, and the bases for the detail subspaces are
translations of the dyadically dilated wavelet. After the coefficients of expansion at
a particular level of approximation in terms of the corresponding basis are found,
the coefficients for coarser levels of approximation and detail can be found using a
bank of perfect reconstruction multirate filters, whose main component is a pair of
low-pass and high-pass decimation filters. When, as is usual in practice, the signal
at hand is a discrete-time signal, digital filtering is the only choice available. This
chapter examines alternative frameworks involving the DWT of one- limensional
and two-dimensional signals. The material from this chapter and from Chapter 3
provides the setting for many applications of the DWT.


4.2 미아thogon이 Wavelet Bases
In examining the properties of the filters associated with orthogonal decompositions
in Chapter 3, we found that it is not possible to have symmetric HR ifiters. Sym-
metry in an FIR filter guarantees linear characteristics for its frequency response
phase-a very desirable property in several applications. In fact, it is so desirable
that early efforts in subband filtering were directed toward filter design that main-
tamlled this property at the cost of perfect reconstruction. Using the MRA framework,
it can be shown that perfect reconstruction linear-phase FIR filters can be obtained
if we give up orthogonality and accept biorthogonality instead.

                                         95
96   Alternative Wavelet Representations

        We introduce the concept of biorthogonality using a simple, two-dimensional
     vector space. Consider the linear independent pair of vectors a1 = [2 1] and a2 =
     [1 2]. These are not at right angles to each other but they do form a basis for a
     two-dimensional linear vector space. Any vector x = [xi, x21 can be expressed as a
     linear combination of a1 and a2; that is,

                                           x= a1a1+ a2a2                              (4.1)

     for scalars a1 and a2. Because a1 and a2 are not orthogonal, these scalars cannot
     be found as simple projections of x on a1 and a2 respectively. They are found by
     solving a pair of linear equations instead. The convenience of projecting the given
     vector on the basis vectors to determine the coordinates of the vector is definitely
     lost. However, it is possible to find an alternative basis b1 and b2 such that the
     scalars al and a2 in Equation 4.1 are obtained as projections of x on them, rather
     than as projections on a1 and a2. The conditions imposed are

                                            (a1, bi) = I
                                            (a2, b2) = I
                                                                                      (4.2)
                                            (ai, b2) = 0
                                            (a2, bi) = 0.

     For the chosen values of a1 and a2, these conditions yield b1 = [2/3, -1/3] and
     b2 = [-1/3, 2/31. The pairs a1-a2 and b1-b2 are said to be biorthogonal bases. They
     are sketched in Figure 4.1. Observe that b1 and b2 can be obtained by rotating each
     vector of the pair a1-a2 individually by 90 degrees (either clockwise or counterclock-
     wise as the case may be) and then scaling. Using the conditions of Equation 4.2 in
     Equation 4.1 we find

                                            a1 =(x, b1)                               (4.3)

     i= 1, 2; which shows that the coordinates required to express x in terms of the
     basis vectors a1 and a2 can be obtained as orthogonal projections on the alternative
     basis vectors b1 and b2. The process is illustrated in Figure 4.1. Although the
     biorthogonal bases in this example generate the same two-dimensional linear vector
     space, it is possible to have them generate separate spaces. For example, a1-a2
     and b1-b2 are biorthogonal for a1 = [1, -1, 2], a2 = [0, 1, 0], b1 = [1, 1, 0], and
     b2 = [1, 0, 0]. However, each pair generates a separate two-dimensional subspace
     of a three-dimensional Euclidean space.
        The idea of using biorthogonal bases can be carried over to the wavelet world
     [Cohen, Daubechies, and Feauveau 1992; Daubechies 1992]. Let 中(t) and 中(t) be
                                                                               B/o片hogonal Wavelet Bases   97




                                                 ,   ,        /           a2




                                                 a2a2




                                       b2   卜g
                                                              /
                                                                       iiai             "'
                                                 口］
                                                         \\       b1




 Figure 4.1 텨or十hogonc引 b（그ses for the two＜出men引C가）（미 \iector sp（그Ce.


two scaling functions, each of which satisfies a dilation equation:

                               中（t) = 2＞二力（兀）砂（2t- n)
                                                                                                  (4.4)
                               a(t) = 2＞二石（n)a(2t-n).
                                            n


Further, let

                                  (0(t), 中(t - k)) = 8 (k)                                        (4.5)

 for integer values of k. In Equation 4.4 the two sequences h(n) and h(n) may
have only a finite number of values that are nonzero, in which case they serve as
impulse responses of FIR filters as seen later. Let the two scaling functions generate
MRAs with subspaces that are labeled Vk and Vk respectively. The basis for V0 is
given by 砂(t) and its integer translates, whereas that for V0 is given by 砂(t) and
its integer translates. For any other subspace of either MRA the basis is given
by translations of an appropriate dilation of 中(t) or 中(t). Equation 4.5 makes the
98   Alternative Wavelet Representations

     basis of Vk biorthogonal to that of Vk. Therefore, the two MRAs are said to be
     biorthogonal to each other. Also, the scaling f끄lction t (t) is called the dual of the
     scaling function 中(t).
        Suppose f (t) is a square integrable function for which we want to find ap-
     proximations in the MRA of the subspaces V1. In Chapter 3 such approximations
     were obtained by orthogonal projections of f (t) on these subspaces. However with
     biorthogonal MRAs, we do something different. Consider fo(t)-the approximation
     of f (t) in the subspace V0. We form fo(t) as
                                                  的

                                    fo(t) = ＞二 口（0, n）中（iH兀）                           侄6)
                                             n= - 的


     where

                                     a(0, n) = (f (t),砂(t - n)).                       (4.7)

     Thus, the coefficients of the expansion are obtained by projecting f (t) not on V0 but
     rather on V0. which is simply a generalization of our introduction to biorthogonality
     provided earlier in this chapter with a pair of finite-dimensional vectors. In general,
                                              的

                                  人（t) = ＞二 a(k，兀）中（2"t - n)                           (4.8)
                                            n==11的


     where

                                 a(k, n) = 2_ c(f(t), a(2 't - n)).                    (4.9)
     Generating approximations in this fashion has the nice property (also seen with the
     orthogonal MRA of Chapter 3) of yielding the same approximation to the function
     f (t) at a certain level whether we use the original function f (t) or one of its ap-
     proximations at a finer level. We illustrate this using the particular case of fo(t)
     and f_1(t).
        From Equation 4.8,
                                               的

                                 五1(t) = ＞二 a(-1, n）中（2t -凡）                          (4.10)
                                            n= -的


     where

                                   a(- 1, n) = 2(f (t), 中(2t - n)).                   (4.11)

     Suppose we were to start with fi (t) instead of f (t). Then, similar to Equation 4.6,
     we would form its approximation in V0 as


                                   ＞二 (f_1(t),a(t -兀））中（t - n)                        (4.12)
                                   n ==1的
                                                            B/orthogonal Wave/et Bases   99

whereas if we used f (t) directly, we would form its approximation as f0(t) in Equa-
tion 4.6 with the coefficients given by a(0, n) in Equation 4.7. From Equation 4.4,

                                       的

                       多（t - n) = 2 ＞二 石（m)a(2t - 2n - m).                     侄13)
                                      m= -的



Using Equation 4.13 in Equation 4.7 we have

                     口（0，凡）=2＞二石（m)(f(t), a(2t - 2n - m)).                     (4.14)
                                  m



From Equations 4.9 and 4.14 we have

                          叩m) =Z枷) a(크2n＋川                                     (4.15)

which can be rewritten as

                          a(0, n) =＞二口（-1, m）石（m - 2n).                        侄16)


It can be shown that the quantity (f. i (t), 中(t 中 n)) in Equation 4.12 is also equal
to the right-hand side of Equation 4.16, thus showing that by using Equation 4.8,
whether we approximate f (t) in V0 or f_i (t) in V0. we get the same function.
   Observe from Equation 4.16 that (as in the orthogonal case) coefficients at one
level can be obtained by filtering and downsampling the coefficient sequence at the
next finer level. The filter in question has impulse response h(- n). How does one
associate wavelets with a biorthogonal MRA? Not surprisingly, given that there
are two scaling functions, we also have two wavelets that are duals of each other
[Cohen, Daubechies, and Feauveau 1992; Daubechies 19921. Let 少 (t) and 少 (t) be
two functions that integrate to zero, with the additional properties that

                       (/i (t), 砂(t- n)) = 8 (n)
                       (fr (t), 中(t - n)) = 0
                       （砂（t), 砂（r H 7i)) = 0                                    (4.17)

                                   砂（t) = 2＞二g(n）中（2t 小 n)

                                   可(t) = 2＞二g(n）多（2t - n).

Also, let 砂(t) and its integer translates, and 砂(t) and its integer translates, span
subspaces denoted by W0 and W0 respectively. With these properties, 少 (t) and 砂 (t)
100   Alterna加e 너／avelet尸e尸resentat幻ns

      serve as a wavelet and its dual, respectively, for the biorthogonal MRA. Properties
      2 and 3 in Equation 4.17 require the wavelet to be orthogonal to the dual scaling
      function and its integer translates, and require the dual wavelet to be orthogonal
      to the scaling function and its translates. This means that the subspace W0 is or-
      thogonal to subspace V0. and the subspace Wo is orthogonal to V0. Analogous to
      the orthogonal MRA, the subspaces Wo and W0 are the detail subspaces and they
      are biorthogonal to each other by property 1 in Equation 4.17. Properties 4 and 5
      require the wavelets to satisfy two-scale relations with coefficient sequences g(n)
      and g(n).
         Following steps similar to those in Chapter 3 showing that the detail function
      at any level is expressible as a linear combination of translations of an appropriate
      dilation of the wavelet, it can be shown that the detail functions

                                     歇(t) 三 /k寸1(t) - 九（t)                           (4.18)

      for the biorthogonal decomposition can be expressed as a linear combination of
      translations of a dilation of 少 (t):

                                          的

                                gk (t) = ＞二 b(k, n)少(2_Icr_ n).                      (4.19)


      Furthermore, the coefficients b(k, n) can be obtained by decimating a(k - 1, n). We
      show this by first considering

                                  g0(t) = 兀m)卜 九(t)
                                                                                     (4.20)
                                         = ＞二 b(0, n）少（t寸n).


      From Equation 4.20 and the relationship between 少 (t) and 砂 (t - n) in Equation 4.17,
      it follows that

                         b(0, n) = (go(t), 少(t - n))

                                = （工1(t) - /M吐 砂（1- n))                              (4.21)

                                = (f_1(t), 少(t - n)) - (f0(t), 少(t - n)).

      The last term in Equation 4.21 (namely, (fo(t), 少 (1 - n))) is zero because, as we
      have seen in Equation 4.6, f0(t) is a linear combination of 中(t - n), n integer, and
      ( 'i(t), (t - n)) is zero by Equation 4.17. Thus

                                   b(0, n) = (f_i (t), 砂(t - n)).                    (4.22)
                                                                            B/o片hogonal Wavelef Bases   101

Using Equation 4.10 and the two-scale relation for 少(t) in Equation 4.22 along with
the biorthogonality of 中(2t) and 中(2t), we get

                                           的

                           b(0, n) =    乞 a(-l,m)g(m- 2n)
                                       m= - 的
                                                                                               侄23)


which indicates that b(0, n) can be computed from a(- 1, n) by decimating it by a
factor of two using a filter with an impulse response of 츙(- n). The result can be
generalized to

                                       的


                         b(k,n) = Z a(k- 1,m)g(m- 2n).
                                   m= -的
                                                                                               (4.24)

For any continuous square integrable function f (t) we have

                                                    的

                                   f (t) = ＞二 gk(t)                                            (4.25)
                                                   k= H的




which, because of Equation 4.19, leads to

                                  00           的

                          f(t) = ＞二 Z b(k, n）砂（2"kt卜n)                                         (4.26)
                                k＝니X그 fl= -00




which is the reconstruction expression for the DWT of f (t) with respect to the
wavelet 砂 (t).
   We conclude this section by deriving the synthesis filtering arrangement for the
biorthogonal DWT. We have


                  f_1(t) = fo(t) +go(t)                                                        (4.27)
                                                                    0
                                                                                r                             )
                                                                的
                                                                    \
                                                                    r
                        = ＞二 口（0, n）砂（t - n) +                                                 (4.28)
                                                                        n           n
                                                                    =
                                                                            吻
                                                                                                          H

                                                                                                              !\
                                                                Z
                                                                    b
                                                                            J
                                                            n
                                                                如
On substituting the respective two-scale relations in Equation 4.28 we have

           00                                  凹

          ＞二 a(-1, n）中（2t- n) =2 ＞二 ＞二口（0, t）九（m）中（2t - 2t - m) +
         n=＝寸00                            t＝二m（刃       m

                                               的
                                                                                               (4.29)
                                        2 ＞二 ＞二b(0, Z)g(m）砂（2t -2t- m).
                                           t= 1以그       m
l02   A片ernative W아이et尸e尸resenta加ns




        Figure 4.2 Decomposition and reconstruction liter banks for the biorthogonal case.



      Substituting n = 2t + m in the right-hand side of Equation 4.29 leads to

                  的                              的

                 ＞二 a(-1, n）中（2t- n) = 2 ＞二 ＞二a(0, t）九（n - 2t）中（2t - n) +
                n==1的                           t= U야그   n

                                                 的
                                                                                             (4.30)
                                            2 ＞二 ＞二b(0, t)g(n - 2t）中（2t - n).
                                                t= 4的    n



      From Equation 4.30,

                      a(-1, n) = 2＞二 a(0, Z )h(n - 2t) + 2＞二b(0, Z )g(n - 2t)                (4.31)
                                    e                        f

      which shows that a(- 1, n) is the sum of two sequences: one, an interpolation by a
      factor of two of a(0, n) using the filter with impulse response 2h (n); and the other,
      an interpolation by a factor of two of b(0, n) using the filter with impulse response
      2g(n). The combined decomposition and reconstruction is depicted in Figure 4.2.


      4.3 Filtering Re山tionsh巾 化rB伯rthogon이 Filters
      We next derive expressions relating the various filters to each other in both the time
      and frequency domains. Equations 4.4 and 4.5 yield

                 ( (t), 砂(t - n)) = 8 (n)

                                  =4兄＞二h(p派列 (2t -加(2t - 2n - q))                            (4.32)
                                        p   q

                                  = 2Z Z仰)h(q)8(p＝小 q)
                                     p q
                                                                       Filtering Relationship for Biormogonol Filters   103

from which it follows that
                                              ｛小                   y         8伽）
                                                                                                             (4.33)
                                              수九（m + 2n）九（m) = 万二'
In the frequency domain the corresponding relationship is

                                  H*(w)H(w) + H*(w + ir)H(w + it) =1.                                        (4.34)

Similarly, from Equation 4.17 we have

                                                           y.g伽 似啼（m) = 한민
                                                           =;1
                                                            m            z
                                                                                                              (4.35)
                                  G半（w)G(w) + G' 佃 + 기G佃 + 兀） = I

and

                                                            ＞二九（m +2n)g(m) = 0

                                   // ' 佃）G(w) + H* (w + 兀）G(w + 兀） == 0
                                                                                                              (4.36)
                                                            ＞二石（m +2n)g（川 = 0

                                  H佃）G*(w) + 月佃 + 兀）G*(w + 兀） = 0.

   The filter equations presented in this section have been derived as necessary
consequences of biorthogonal decomposition. They can be represented compactly
in matrix form as


                    G(w：二：]［名之, ) G*：之, )]=1
               ［客：? H(w                                                                                      低37)
where I is the two-by-two identity matrix. Interchanging the order of multiplication
of the two matrices in Equation 4.37 gives

                f     H
                            (w)      ,    )    G*   (w)    * , )   1[1 (w)     H + it
                                                                                   (w
                                                                                       )   1 I               (4.
                                          )    G*            ir) JLG(w)        G(w+ ir) J
                                                                                              =
                LH*         (w+      it             (w+
                                                                                                                38)
which gives rise to the set of equations

                                                          H*(w)H (w) + G*(w)G(w) = I

                          砂（a) + ir)H (w + 兀） + （芦（a) + ir)G(w + 兀） = 1
                                                                                                              (4.39)
                                          伊（w)H (w + 兀）十（芦（w)G(w + 兀） = 0

                                          H*(w + jr)H (w) + G*(w + jr)G(w) = 0.

Note that Equations 4.34, 4.35, 4.36, and 4.39 are all biorthogonal generalizations
of the paraunitary conditions mentioned in Chapter 3. As in the orthogonal case,
104   Alterna加e 너／Ovelet Represen幻r幻ns

      the satisfaction of the paraunitary conditions by the analysis and synthesis filter
      banks in the biorthogonal case are necessary and sufficient conditions for perfect
      reconstruction. Lastly, consider the following relationships between the H and G
      filters

                                       G(w) = eJmH*(w+,r)
                                                                                             (4.40)
                                       G(w) = 可Jo)月km + 兀）.

      It is easy to see [Cohen, Daubechies, and Feauveau 1992] that these relationships
      between the H and G filters satisfy automatically the conditions given in Equations
      4.34, 4.35, and 4.39. The equations for the orthogonal filters follow as a special case
      if we replace h (n) by h (n), 月(w) by H(w), and so on (that is, if we simply remove
      the tildes).


      4.4 Examples of Biorthogonal Scaling Functions
          and Wavelets
      The B-splines are examples of scaling functions with underlying, symmetric FIR
      filters. An N tap B-spline LPF has the impulse response


                                                                                             (4.41)


      for n = 0, 1, . . . , N- i. Substituting this filter in the dilation equation yields a scaling
      function. The higher the value of N, the smoother the scaling function. Thus, for
      N = 2 we get the Haar filter and scaling function. Table 4.1 gives h(n) for N = 3,
      4, and 5. A dual filter h (n) can be obtained using the biorthogonality relationship
      given in Equation 4.33. The filter h (n) is also symmetric. This fact along with
      Equation 4.33 gives a set of linear equations that yield the coefficients of h(n) (see
      Problem I at the end of the chapter). The scaling functions corresponding to these
      B-spline filters are shown in Figure 4.3. These were generated using the MATLAB
      routine presented in Chapter 3 for solution of dilation equations.

               Table 4.1 B-Spline Filter Impulse Responses

                  No. of Taps         B-Spline Type          Impulse Response h (n)
                        3                 Linear                  作 ｛글｝
                         4              Quadratic                ｛寺 긍릅급｝
                        5                  Cul月c                 儡｛冬｛슈｝
                            Ex아까91es of B幻片hogonal Scaling Func加ns and Wavelets   105




Figure 4.3 Scaling functions corresponding to linear (A), quadratic (B), and
           cubic (C) B-spline f咐ers
106   Alternative 너／口V이아尸epresen幻加ns

         化b伯 4.2 An（기＼isis 테ter 師nks 山ed by the FBI


              Filter Type       Right-side Filter Coefficients       Filter Length
              Lo＼사 pass        老x (0.853, 0.3774, 卞0.11062,                 9
                                -0.023849, 0.03783}

              High pass        金x (0.7885, -0.4181, -0.04069,              7
                                0.06454)



         Another example of biorthogonal analysis and synthesis filters is the one em-
      ployed by the Federal Bureau of Investigation (FBI) for fingerprint image compres-
      sion. The coefficients of the right half of the analysis bank are given in Table 4.2.
      The left side of the filter is generated by making use of the symmetry of the filters.
      The synthesis bank is generated using the following relations that can be obtained
      as an inverse discrete-time Fourier transform of the relationships in Equation 4.40:


                                     g(n) = (- 1尸H" 力（1- n)
                                                                                      (4.42)
                                     h(n) = (- 1)ng(1 - n).

      The scaling functions and wavelets corresponding to these filters are shown in Fig-
      ure 4.4.
         A method of designing practical biorthogonal ifiters EHerley 1993; Vetterli and
      Herley 1992] involves first designing a halfband filter to desired specifications. Let
      P (w) be the frequency response of the halfband filter. Standard filter design meth-
      ods, such as the Parks-McClellan algorithm [Oppenheim and Schafer 19891, can be
      used to obtain P (cv) subject to the halfband constraint

                                      P(cv) + P（口）＋兀） = 1                             (4.43)


      and other passband and stopband constraints. The function P(w) can then be fac-
      tored as

                                       P(w) = H*(w)H(cv)                              (4.44)

      to give a pair of biorthogonal filter frequency responses H(cv) and H(cv). For the
      specific case when P(cv) is of the form 田(c川2 = H* (cv)H(cv), we can factor it
      to yield H(w) and H(cv) = H*(cv), resulting in a PRQMF bank for an orthogonal
      decomposition. Other methods for the design of biorthogonal scaling functions and
      wavelets such as the lifting scheme and biorthogonal generalization of the Meyer
      construction are presented in Chapter 7.
                                    Exam例e$ 아Biort加卯nal Scaling Funct跏s and Wave囹S            107




Figure 4.4 Scaling functions and wavelets corresponding to FBI filter coefficients given in
           Table 4.2. Scaling function (A) and wavelet (B) corresponding to the analysis
           께ters.
108   Alternative Wavelet Representations




       Figure 4.4 (continued) Scaling function (C) and wavelet (D) corresponding to the
                  syn卄冷粥 셰ters.
                                                                             Two-［沖7그ensi（가）（그／너／avek升＄       109


4,5 Two-Din伯n引on이 Wave旭ts
Let f (x, y) be a square integrable function in the two variables x and y. Let 中(t)
be a one-dimensional scaling function that gives rise to an orthogonal MRA. This
function would be of the kind seen in Chapter 3. Consider the two-dimensional
function

                                       蜘（工，y) 三 砂（工）中（y).                                          (4.45)

Using the orthonormality of 中(t) to its integer translates, it is easy to show that the
set of two-dimensional functions {s中中 (x - k, y 中 0 : k, Z integers) is orthonormal.1
Let fo (x, y) be the projection of f (x, y) on the linear vector space V0 generated by
this orthogonal set. Then


                         fo（工，y) = ＞二 ＞二 口0(i, j)s加（工- i, y尸j)                                     侄46)
                                      1= -以） J=＝니刃




where

                              ao(i, j) = (/（工， y),s中中（兀 -i, y- j)).                                (4.47)

Let Vk, for any integer k, denote the linear vector space generated by the set
{s加(2 'x - m, 2 "y - n) : m, n integer). The sequence of linear vector spaces
. . 니V1 C V0 C V_i, and so on, is an MRA in the space of all square integrable
two-dimensional functions. Let us denote the approximation of f (x, y) in Vk by
fk (x, y). The difference between two successive levels of approximation is a de-
tail function. However, unlike the one-dimensional case, such a detail can be split
into three functions [Daubechies 1988, 1992] that lie in three separate linear vector
spaces, as we show next.
    Consider
                                       00     的


                      f-i（工，y）三 Z           ＞二 a_1(i, j)s加（2工- i,2y- j).                           (4.48)
                                     1= -以） /=H이그




Using the definition of s加(x, y) in Equation 4.48 we have

                                      00     的

                      兀I（兀， y) = ＞二 ＞二 a_1(i, j）中（2工                 i)中（2y- /）·                   (4.49)
                                    1= -C그 3==-CO




lThe definition of the inner product of two-dimensional functions f (x, y) and g(x, y) is a straightforward
extension of the one-dimensional definition and is given by (f, g) 三 f: m fOO CO f (x, y)gt(x, y) dx dy.
110   Alterna加e 너幻V이e시？epresen幻加ns


      Let

                                                        00

                                    f-I（工，/) 三 ＞二 a_1(i, J）砂（2工 小i).                                 (4.50)
                                                    1=-的



      Then2

                                                      的

                                   兀1（工，y) = Z 工I（工，J）中（2y- j).                                      (4.51)
                                                   J= 4的



      Let us use3 Vk to denote the subspace at level k of the one-dimensional MRA with
      an underlying scaling function of 中(t). Let Wi, denote the subspace for the detail
      functions at the corresponding level. The function fi (x, j) lies in the linear vector
      space v_1. It can therefore be split into two orthogonal functions; that is, it can
      be expressed as the sum of a function fo(x, j) E v0 and go(x, j), which lie in the
      orthogonal complement of v0 in v_1. We thus have

                                                        的

                                     而（工，/）三 Z 勻，0(fl）砂（工- n)                                        (4.52)
                                                    n=＝的

                                                        的

                                     g0（兀 j) 三       ＞二 勿，0(fl）砂（兀 -n)                               (4.53)
                                                    7i =14的



      for some pair of sequences a,o (n) and b1,0 (n). The sequence aJ,o (n) is obtained from
      a_1(i, j) by filtering and downsampling along i for a given j using the H filter.
      Similarly, b ,0 (n) is obtained by decimating a_1(i, j) along j with the G filter. Thus

                                       00                          凹

                       f-i（兀，/)= Z 四，0（兀）中（x -n) + ＞二 b3,o(n）少（x- n).                                侄54)
                                     n= -00                      n= -的



      Putting Equation 4.54 in Equation 4.51,

                                              00    的

                          工l（兀，y) = ＞二 ＞二 勻，0（兀）中（工 ，2）中（2y1j) +
                                         /=    00 fl= -00

                                              00    的
                                                                                                     (4.55)
                                            ＞二 乞 勿，o(n）砂（工- n）砂（2y- j).
                                         J＝니刃 n＝寸以）




      2 The functions fi (x, y) and fi (x, j) are different. The former has two continuous arguments whereas
      the latter has its first argument continuous and its second ar돋ument discrete.
      3Observe that "v" is lowercase here. The uppercase symbol is used to denote the two-dimensional MRA.
                                                               Two-Dimensional Wavelets   111

Define

                                       的

                         兀1(n, y) 三 乞 四，0(n）砂（2y- j)
                                     J=1以）

                                      的
                                                                                 (4.56)

                        肛1（兀y) 三 Z 勿，0(n）砂（2y- j).
                                    J= -oo




Then

                         00                        的

            兀I（兀， y) = ＞二 局 (n, y沖仁- n) + >               冬1(n, y）少（工尸兀）·        低57)
                       n= -oo                     n= -的




  Like f_1(x, j), the functions f_仰, y) and g_i (n, y) are both in the linear vector
space v_1 and are expressible as the sum of mutually orthogonal functions as


                          f_1(n, y) = Ao(n, y) + Bo(n, y)                        (4.58)

                          g_i (n, y) = Co(n, y) + Do(n, y)                       (4.59)


where

                                       m

                         Ao(n, y) 三 ＞二 ao(n, p）砂（y- 끄）                           (4.60)
                                     p= -以）

                                       的

                         Bo(n,y) 三 Z bo(n, p)砂(y- p)                             (4.61)
                                     P=e아그

                                       的

                         Co（兀y) 三 ＞二 co(n, p）中（y - p)                            (4.62)
                                     p= -的




                         Do(n, y) 三 ＞二 do(n, /)）砂（y- p).                         (4.63)
                                     P==H的




The sequences ao(n, p) and bo(n, p) are obtained by decimating the sequences a1,o(n)
along I using the H and G filters respectively. Recall that a,o(n) is itself obtained
by decimating the rows of a (i, i) with the H filter. Thus the sequence a0 (n, p)
is obtained by first decimating a (i, I) along its rows with the H filter and then
decimating the columns of the result with the same filter. The other sequences are
obtained in a similar fashion as summarized in Table 4.3.
112   Alternative Wavelet Representations

          Table 4.3 Derivation of the 口0, b0, c0. and d0 Sequences

                                                                          Common
             Sequence                  Decimation Order                  Termin아ogy
              alj(n, p)       Rows of a(i, j) with H followed by            LL
                                columns of result with H
              b0(n, p)        Rows of a (i, J) with H followed by           LH
                                columns of result with G
               CO（兀 p)        Rows of a (i, J) with G followed by           HL
                                columns of result with H
              do (n, p)       Rows of a(i, j) with G followed by            HH
                               columns of result with G

           LL = low-low; LH = low-high; HL = high-low; HH = high-high.




        Putting everything together we have


                                       00     凹

                          兀1（工，y) = ＞二 ＞二 口o(n, p）中（工H兀）中（y - p) +
                                     n= -茯） p＝니乂

                                       00      的


                                      ＞二 ＞二 bo(n，尸）中（工- n）少（y - p) +
                                     n= H仗） p＝寸凹

                                       00     的
                                                                                      (4.64)

                                       Z Zco(n,p）砂（工- n）中（y - p) +
                                     n= -（乂 p= -以그

                                       OO      的

                                      ＞二 ＞二 do（兀／)）少（工- n）少（y- p).
                                     fl= -00 p= -00




      Defining



                                            S中砂 = 中（工）少（y)                            (4.65)

                                            S寸中 = 砂（工）中（y)                            佩66)

                                            S少砂 = 砂（功砂（y)                             侄67)
                                                                Two-Dimensional Wavelets     113

we have

                                00       的


                 兀l（兀，y) = ＞二 ＞二 .o(n, p)s加（工- n, y - p) +
                              fl ==-00 p= -oo

                                00       的


                               Z ＞二 bo(n,끄）S中少
                              n==4以그 p＝니乂
                                             （工H兀y - p) +
                                00       的
                                                                                   (4.68)

                               ＞二 ＞二 CQ(fl, p)s少中（工H兀，y - p) +
                              fl = -0 (그 p＝寸的

                                00       00


                               ＞二 ＞二 do(n, p)s砂少（工H兀y - p).
                              n= -以） p＝叫的




The first term in Equation 4.68 is nothing but fo(x, y), whereas the other three terms
make up the deta且 The functions s加（工， y), 蜘仇 y), s中中（工， y), and s中砂（兀 y) and
their integer translates along x and y are all orthogonal to each other. Thus 1i (x, y)
is the sum of its projections on four linear vector spaces rather than just two, as in the
one-dimensional case.
   Let the detail functions corresponding to coefficient sequences bo (n, p), c0 (n, p),
and do(n, p) be called gbo(x, y), gco(x, y), and gdo(x, y) respectively. To refer to the
previous subspaces, let us adopt the following nomenclature: the low-resolution
approximation belongs to the subspace V0 or Wa0, and the detail functions belong
to subspaces Wb0, W0, and Wd0 respectively. For the low-resolution approximation
and the detail functions at some level k, the notation is the same, with k replacing
zero.
    Generalizing the previous result, we have


                             Vk I = Vk e Wb,k q) W,k 4) Wd,k                       (4.69)


the repeated application of which leads to



                                           k今q) n9,k
                         Vk l = q) n뇨eq) n二，
                                  j=k           j=k     j=k
                                     的
                                                                                    (4.70)
                              = 由 (wb,k e W,k 田 Wd,k) .
                                  j=k



Letting k 수 - oo leads to the conclusion that any two-dimensional square integrable
function can be expressed as a linear combination of dyadic translates and dilates
114    Alternative 너幻v이計Represen幻加ns

       of three two-dim帥如nal wavelets-namely, s加仇 y), s加（兀
                                                                                       y), and s砂砂（工， y):


                   /（兀y) = 二 Z Z Z 匈(n, p)s中砂
                                            （2'"工m兀2"'y - p) +
                                k= -（乂 1=-ce n＝니X그 p＝니)0

                                  00     00     00      的

                                 ＞二 ＞二 ＞二 ＞二 Ck（凡，p)s砂中（2 "兀- n, 2'1y卞p) +
                                k＝卞00 1==-的 n= -00 p= -이）
                                                                                                            (4.71)


                                 ＞二 ＞二 ＞二 乞 d （兀 끼蜘（2人
                                k= -oo 느- 00 fl= -00 p＝니乂
                                                                                     n, 2 'v - p).


      The formulation we have here for the two-dimensional DWT is separable (that is, the
      wavelets have been expressed as the products of two one-dimensional functions, as
      in Equation 4.45). Also, even though we used the same scaling function 中(t) along
      the x and y directions in the definition of s (x, y), it is possible to do otherwise.
      In other words, one can have two separate scaling functions, say 幽(t) and 勿(t), so
      that

                                              蜘（兀 y) = 幽仁）吻（y)                                             (4.72)

          When the datum of interest is a digital image, say x(m, n), an interpretation ex-
       ists for DWT operations that is similar to what was provided for one-dimensional
       discrete-time signals in Section 3.7. The given image is treated as the sequence
       ao(m, n) of Equation 4.46. Subsequent levels of decomposition are obtained by the
       one-dimensional row-column filtering of Table 4.3. Because what we have is the
       one-dimensional approach of Chapter 3 applied separately to the rows and columns
      of the image, the reconstruction follows lines similar to what we saw in that chapter.
      Figure 4.5 shows the block diagram for a one-level decomposition and reconstruc-
      tion. Note the terminology for the filter outputs after the column filtering. They
      are called low-low (LL), low-high (LH), high-low (HL), and high-high (HH), as
      indicated in Table 4.3. LL indicates that the image corresponds to the subband
      obtained by low-pass filtering and downsampling both the rows and the columns.
      Figure 4.6 shows a three-level decomposition of an image using the D4 filters. Ob-
      serve the similarity of the low-resolution image to the original. In fact, this is a
      blurred version of the original because it results from low-pass filtering and down-
      sampling the latter. Also, observe the tendency of the other images-the so-called
      detail images4-to retain edge information. In particular, vertical edges appear in
      the LH images whereas horizontal edges appear in the HL images. This is due to
      the high-pass nature of the G filter.


       ' These images are actually the coefficients that are associated with the expansion of the detail functions
      in terms of the continuous dilated and translated wavelets in the two-dimensional MRA.
                                                       Nonsepari갔!e Mu川（抑pensiona/ 너／Ovelets   115


                                        columns
                                                           HPF decimate        high-high


                       HPF decimate

                                                           LPF dec血Late        high-low
          rows


    Input image
                                        columns            HPF decimate         low-high


                       LPF decimate

                                                            LPF decimate        low-low

                                             (A)



          columns
    high-high         HPF interpolate       ro꿔S

                                                    HPF interpolate
          columns
    high-low    나     LPF interpolate

                                                                             output image
          columns
    low-high    -,-   HPF interpolate       rows

                                                    LPF interpolate
          columns
    low-low           LPF interpolate

                                              (B)

 Figure 4.5 테ter bank stru아내ef아 a one-Iev쉬 decon耳）O섧tion (A) and reconstruc卄on (B) of
            a two＜北nen如nal 針gn（미．



  Figure 4.7 shows a three-level decomposition of another image. Again, notice
how vertically oriented features such as the hair show up in the LH images whereas
the horizontally oriented features such as the lips show up in the HL images.



4.6 Nonseparable Multidimensional Wavelets
For the two-dimensional separable case, we saw that the approximation subspace
V0 was spanned by the integer translates of the scaling function s中,中(x, y) in the x
116   Alter,）아加eW아elet Representa加ns




      Figure 4.6 (A) The "plus image.'


      and y directions. The scaling function itself was composed of two one-dimensional
      scaling functions 幽(x) and 勿(y), as in Equation 4.45.
         We also saw how an MRA analysis is generated using this scaling function. Using
      the two-scale difference equation we can write s中, 中(x, y) as


                        S中小功＝Zm（的(2小昑二幻(k）吻（2y- k).                               侄73)

      Equation 4.73 can be written as


                          S加（毛 y) = ＞二 Z岫(n,k)s ,0(入 - n,勾 나）                     佩74)
                                         n   k


      where

                                         hi,2(n,k) = h1(n)h2(k).                  (4.75)
                                                       Nonseparable Multidimensional Wavelets     117




Figure 4.6 (continued) (B) The "plus image." Three-level wavelet decomposition



No＼八／let

                                                X
                                                                                          [
                                                                                          n
                                         t      V                                      (4.76)
                                                                                          1
                                                                                              =




for real x and v, and



                                              n1L
                                                n 1n
                                          n
                                                                                       (4.77)


for integer n and k. Using Equations 4.76 and 4.77 we can rewrite Equation 4.74 as


                             s 1,(t) =Z h12(n)s (Dt - n)                               (4.78)
118    Alter,刃加e 너／OveletRe尸resentations




      Figure 4.7 (A) The "girl" image. "（引rl with H（카" photogr갸）h Cc＞口yright 匣） 卜네chele（긔ement.



      ＼人／
        here



                                                                                           (4.79)


      This is called the dilation matrix. Thus, the dilation factor in the one-dimensional
      case is replaced by the dilation matrix for the multidimensional case. Note that the
      dilation matrix in Equation 4.79 for the separable case is diagonal. The main diag-
      onal entries, namely 2 and 2, represent the dilation factors along the x- and y-axes.
      For the nonseparable case, the scaling function cannot be represented as a prod-
      uct of two one-dimensional functions as in Equation 4.45, and the dilation matrix
                                                   Nonseparable Multidimensional Wavelets   119




Figure 4.7 (continued)(B) The "girl" image. Three-level wavelet decomposition




should be nondiagonal. It should, however, represent a dilation in both the x and
 y directions. To this end the dilation matrix should satisfy the following properties
(see Cohen and Daubechies [1993],Kovacevic [1991], Kovacevic and Vetterli [1922],
and Vetterli and Kovacevic [1995P:


 1. The product Dn should map a vector n that has integer entries to another vector
    p that also has integer entries. This implies that the dilation matrix should have
    integer entries.
120   Alternative Wavelet Representations


       2. The absolute values of the eigenvalues of the dilation matrix should be strictly
          greater than one. This ensures that D effects a dilation along both the x- and
          the 少axes.

         The number of wavelets corresponding to the MRA defined by D is given by
      Idet(D)1 - 1 where det(D) is the determinant of D. Thus, for the dilation matrix
      given in Equation 4.79, the number of wavelets associated with the MRA is three.
         The dilation matrix D also defines the lattice on which the two-dimensional plane
      is sampled. For example, the dilation marix in Equation 4.79 represents down-
      sampling a two-dimensional sequence by two on a rectangular grid. As another
      example, consider the matrix

                                                           I
                                            .0=                                            (4.80)
                                                  [:
                                                       -
                                                           1

      This matrix is the dilation matrix for a nonseparable case when the sampling is
      on what is known as a quincunx lattice. This lattice is shown in Figure 4.8. Quin-
      cunx sampling can be regarded as downsampling each row (or column) of a two-
      dimensional sequence by a factor of two in a staggered fashion. The absolute value




            Figure 4.8 G）내ncunx san非캐ng laffice. The S에d （永＞ts represen十 the S（가n히es th아
                       are 口（그r十 of the Ia卄ice.
                                                                      너／avelet Packe朽    121

of the determinant of this matrix is two, and hence only one wavelet is associated
with this MRA. As in the one-dimensional case, this wavelet can be obtained using
the HPF g1,2(n) and the two-scale dilation equation

                           少（t) =＞二g1,2(n)s砂，中（DQt - ii).                       (4.81)

   The properties of nonseparable scaling functions and wavelets are a generaliza-
tion of the properties of their one-dimensional counterparts. The general dilated
scaling function in this case is

                                    S中,中（D'仕 小 n).

As in the one-dimensional case, the scaling function at a scale m is orthogonal to its
D-'i translates. Thus

                    (s中, 中（I少t 小 n), s中, 中（I少t- k)) =2m8(n- k).                 他82)

The wavelets are orthogonal across scales. Also the scaling function and the wavelet
are orthogonal to each other; that is,

                                (s , (t), 砂(t - n)) = 0.                        (4.83)

   Lastly, similar to the one-dimensional case, the set {2_mI2砂 (Dmt尸n), m integer),
with t and n as defined in Equations 4.76 and 4.77, forms an orthonormal basis for
the two-dimensional space. The discussion in this section concentrates on the two-
dimensional case. The extension to multiple dimensions is a straightforward ex-
tension of the two-dimensional case. Nonseparable wavelets and scaling functions
have found a variety of applications in the fields of computer vision and pattern
recognition [Daugman 19971, and image and video representation and coding [Ko-
vacevic 1991].


4.7 Wavelet Packets
It was shown in Chapter 3 that practical implementation of the DWT can be inter-
preted as starting with a function fo (t) at level vo in an MRA and then obtaining the
coefficients for the detail functions at coarser levels. The given digital signal, say
f (n), can be regarded as forming the coefficients of the expansion of f0(t) in terms
of the scaling function 0(t) and its integer translates. The analysis or decomposition
filters yield the coefficient sequences for other functions of the MRA. In particular,
the output of the LPF at level k yields the coefficients for expressing fk(t) in terms
of {0 (2_kt - n)1, and the output of the corresponding HPF yields the coefficient Se-
quence required to express the detail function gk(t) in terms of t '仁"t - n)). Also,
122   Alternative Wavelet Representations



                                                          1eV0

                                                         A
                                                      fIEVI   g1cW1

                                                    ／八
                                              乃eV2        g2EW2

                                             A
                                        f3EV3         g3EW3


               F勾ure 4.9 DWT 卄ee for （그 three-Iev이 decon가＞(＞읽tion.




       we would not be generating all the infinite number of detail functions in practice.
      Instead, the decomposition filter would consist of a finite number of stages, leav-
       ing us with one coarse approximation and a finite number of detail functions. For
       example, if we were to have three stages of filtering, we would end up having the
      coarse approximation f3(t) and the detail functions gi(t), g2(t), and g3(t). The entire
       decomposition corresponds to the tree in Figure 4.9. Observe in Figure 4.9 that at
      every level save the third, only the left node has two branches, whereas the right
      node is a terminal node (that is, it does not branch further). This is simply a repre-
      sentation of the fact that in the DWT, only the output of the LPF is subject to further
      levels of decomposition, which is in itself a consequence of the fact that an MRA
      is interpreted as the result of repeatedly projecting the approximation to a function
      on other subspaces to generate coarser approximations. The question arises as to
      whether one can generate alternative decomposition trees that allow branches on
      the right nodes, and whether such a decomposition has an interpretation in terms
      of basis functions for linear vector spaces of functions. It is in the answer to this
      question that the concept of wavelet packets arises.
         Suppose we have a two-level decomposition that yields the functions f2(t), g2(t),
      and gi(t). We have

                                                的

                                  gi(t) = ＞二 b(1, n）砂（t/2 -兀）

                                  g2 (t) =   ＞二 b(2, n）砂（t/4 - n)                     (4.84)
                                             n= - 的

                                                的

                                  力(t) =     ＞二 口（2，刃）中（1/4- n)
                                             n= -的
                                                                                     Wave/et Packets   123

and

                            九（t) = 力（t) + g2(t) + gi(t).                                      侄85)

Let


                             「1,   1,   .(!        ):       二砂
                                                                     （t/   2-   n)
                                          1
                              /72,0,4(D 三 4中（t/4- n)                                          (4.86)

                              P2工.            (!   )三       ｛砂
                                                                     （t/   4－   까

The functions pi,i,n(t), p2,o,n(t), and p2,1, n(t) form an orthogonal set. Equations
4.85 and 4.86 indicate that these functions form a basis for vo. Let us now express
these functions in terms of 中(t). Doing so leads to the notion of wavelet packets
[Wickerhauser 19941.
   The dilation equation is given by

                             砂（t) = 2＞二力（n）砂（2t 中 n).                                         (4.87)


Replacing t by 2t in Equation 4.87 yields

                            中（2t) = 2＞二力（兀）中（4t -n) ·                                         侄88)
                                                        n


Putting Equation 4.88 in Equation 4.87 yields

                     中（t) = 4＞二 ＞二力（n）九（m）砂（4t - 2n - m).                                     (4.89)
                               n              m


Replacing t by t/4 in Equation 4.89 we have


                P2,叩小 和(t/4) 스二如帥口小）.               n            m
                                                                                              (4.90)


Now the two-scale relation for the wavelet is given by

                            砂（t) =2＞二g（兀）中（2t -n) .                                           (4.91)


Using Equation 4.88 in Equation 4.91 we have

                      少（t) = 4＞二 ＞二g（兀）力（m）中（4t -2刃 -m)                                       (4.92)
]24    Alterna加e Way이a시把口resent力ions

       from which it follows that

                                  I          r八   t小
                      p2,1,0(t) =. -砂(t/4) = 느m戶
                                              ) . H) . g(n)h(m)中(t - 2n - m).      (4.93)
                                        4
                                                         n   m




      Also

                             m\


                                        (
                                        0
                                        i
                                        0
                                              !．如2) = 2) '蛔                        侄94)
                              )
                                  小 1



                                                                       (t- n).
                                               乙                 1H
                                                                  n




      Let us examine p2,0,0(t) and p2,1Q(t) further. Putting t = 4n + m in Equation 4.90
      we have


                            p2,0,0(t) = Z >t h(n)h(t - 2n) (t -Z)
                                                   n
                                                                                   (4.95)
                                                       A (C）中（t - t)


      where


                                            A (l）三＞二九（n）方（Z- 2n)·                 他96)


      Observe that the sequence A(n) is obtained by first upsampling (that is, inserting
      zeros on alternate samples) h (n) and then convolving it with itself. Similarly,


                           p2,1,0(t) = 二 ＞二g(n川- 2n)的 나）
                                               'I
                                                                                  (4.97)
                                            = 二 B(Z汭卜 Z)
                                               t




      where


                                            B(t) 三 ＞二g（兀）九（t H2川                  他98)


      which is obtained by convolving the upsampled version of h (n) with g(n). Thus of
      the three functions defined in Equation 4.86, two of them have been expressed in
      terms of 中(t) and its integer translates using a sequence generated by convolving
      an upsampled version of h(n). The question that arises is whether similar linear
      combinations of 中(t) and its translates using sequences generated by filtering up-
                                                                        너／Ovelet Packe朽    125


sampled versions of g(n) lead to something meaningful. The answer is that they
do. Let

                              C(t) = ＞二九（n)g(Z- 2n)
                                                                                 (4.99)
                              D(t) 三 ＞二g(n)g(t - 2n)

and

                             p2,2,0 (t) 三            (e) b(t   -



                                                 f
                                            ZC
                             p2,3,0(t) = >二 D(t)中(t -Z)
                                                 e
                                                                                (4.100)
                             P2,2.n (t) 三 p2,2,o(t- 4n)

                             p2,3,n(t) 三 p2,3,0(t - 4n).


Then p2,i , n(t), i = 0, 1, 2, 3, forms an orthonormal basis for v0. As we have seen,
pi,i,n(t), 力,o,n(t), and p2, l ,n(t) are bases for W1, V, and W2 respectively. The func-
tions p2,2,n(t) and p2,3, (t) serve to split Wi into two orthogonal subspaces, which
we will call W20, and W21 respectively. Projecting fo(t) on these subspaces gives
two functions, which we will call g2o (t) and g21(t). Let

                             g20 (t) =           c(2, n)p2,2, n(t)
                                                                                 (4.101)
                             g21(t) = 兄 d(2, n)p2,3, (t).

The sequences c(2, n) and d(2, n) are obtained by decimating b(1, n) using the H and
O filters exactly as a (2, n) and b(2, n) are obtained from a (1, n). With this further
decomposition of Wi, we have the tree structure of Figure 4.10. Thus by splitting the
right nodes using the same LPF-HPF combination as for the left nodes, it is possible
to generate various combinations of orthonormal bases. The basis functions that
result in such decompositions are called wavelet packets. It is possible to create
arbitrary tree structures that range from the wavelet tree shown in Figure 4.9 to
balanced trees in which every nonterminal node has two branches [Wickerhauser
1994]. An example of an arbitrary tree decomposition is shown in Figure 4.11. The
wavelet packet basis functions for a three-level decomposition using the D4 filters
are shown in Figure 4.12. The key advantage of wavelet packet decomposition is
the flexibility it offers. Rather than confining ourselves to the extremes of dyadic
decomposition or a full subband decomposition, we can choose intermediate forms.
This is particularly useful in applications such as data compression (see Chapter 5),
126   Alternative 너幻ye廚尸epresen幻加ns


                                                                            H        p3,7,0(t)


                                                     H


                                                                            L        p3.6,0(t)
                              H
                                                                            H        p3.5,0(t)



                                                     L


                                                                            L        p3,4,0(t)


                                                                           H         p3,3,0(t)


                                                     H


                                                                            L        p3,2,0(r)
                              L
                                                                           H         p3,1,0(t)



                                                     L


                                                                           L         p3,0,0(t)


        Figure 4.10 B（계anced tree 幻r 낚八加이et 口ackef decon耳）osition. Here. 나epresents
                    low-pass filtering and H represents high-pass filtering. p3,1,0(r), i = 0. . .. .7 are
                    the basis functions (shown in Figure 4.12) with translates that span each of
                    the eight subspaces.



      where one way of attaining compression is by discarding wavelet subbands with
      very low activity. Either the dyadic decomposition or the subband decomposition
      may yield subbands that have partial activity. Rather than retaining such a subband
      in its entirety, we would be better off splitting it further to confine the activity to
      most of a smaller subband and discarding other subbands.


      4.8 Problems
       1. Construct a biorthogonal perfect reconstruction filter bank with h(n) = {1/16, 1/4, 3/8,
          1/4, 1/16} for n = -2, -1, 0, 1, 2 respectively. This is the impulse response of the cubic
          B-spline filter. You have to use Equation 4.33, and there are infinitely many solutions.
                                                                                       Pr乂刃ems      127


                                                  H


                                    H   H

                                                                       I-   I
                                                               H
                                                                       L
                                                   L
                                                                       H
                                                               L--
                                                                       L




                                    L


       Figure 4.11 A way이et p（그cket tree effecting an 아bi似가y decori갸,osition.
                   L = low-p（그ss f咐0巾也 H = 볘gh下＞（그ss filtering.



2. Repeat Problem I with the additional constraint that the dual-ifiter impulse response
   h (n) is s戶llmetric.

3. Repeat Problems I and 2 for the quartic B-spline h(n) = {1/32, 5/32, 5/16, 5/16, 5/32, 1/32).

4. Determine the filter coefficients h(n) for the scaling function of Problem 4 of Chapter 2.
   Plot the frequency response magnitude of the filter and compare it with that of the Haar
   filter. Construct a perfect reconstruction biorthogonal filter bank with this filter. Plot the
   resulting wavelet, dual scaling function, and dual wavelet. You can use the MATLAB
   routine biscwav in the accompanying disk for generating the plots.

5. Verify that the FBI filters in Table 4.2 satisfy the conditions for a perfect reconstruction
   biorthogonal filter bank.

6. Compute the multiresolution approximations and the detail sequences of the input se-
   quence


                                            f (n) = e ' '256                             (4.102)


  0 5 n <255 for biorthogonal filters. To do this use the routine anaiw (which uses odd-
  length biorthogonal filters) or analh (which uses even-length biorthogonal ifiters). The
  corresponding synthesis routines are synthw and synthh respectively. Filter options
  are provided in the routines. Compare your results with those obtained in Problem 16
  of Chapter 3. As in that problem decompose the sequence down to four levels.

7. Compute the two-dimensional four-level DTWT of the "barbara" image provided on
   the disk. The routine anal2d (which uses orthonormal filters) can be used for this
   purpose. Reconstruct the image using the synthesis routine synth2d and verify perfect
   reconstruction.
128   Alterna力ye Way이et肋presenta加ns




                                                  (   」＼   )




            0.6 -



            0.4 -



            0.2 -




          -0.2 -



            0.4 中


                                                  (B)


        Figure 4.12 Wavelet packets derived from the D4 filter for a three1evel balanced tree
                    for p3,0,0(t) (A) and p3.1,0(t) (B).
                                                                                ／가C놨＞bec石   ] 29




Figure 4.12 (continued) Wavelet packets derived from the D4 f咐er for a three-level
            b（미（그nced tree 幻r /)3그0(t) (C) and p3,3,0(t) (D).
130   Alternative Wavelet Representatians




       F勾ure 4.12 (con打nued) W（그V쉬et 口ackets derived from 十he D4 filter for a 十hree니evel
                  b데（그nced 打ee for p3,4,0(t) (E) and 尸3毛0(t) (F).
                                                                                       까야len衿   131




                                                   6




                                              \\
                                            (（引




                                                       /
                                                                      h스三
                                            (H)


Figure 4.12 (continued) Wavelet packets derived from the D4 filter for a three-level
            b（그k그nced 卄ee 化rp3,o,0(t) (G) and p3.7,0(t) (H)
132   Alt아na加a 너／ave/at Represent豺幻ns

       8. Compute the multiresolution approximation images of the "barbara" image using anal2d
          and synth2d images for a four-level decomposition. Similarly compute the multireso-
          lution approximation images using the routines analw2d and syntw2d, and analh2d
          and synthh2d. Compare the results of each of these routine pairs.
       9. Use the routine wpanal to effect a three-level balanced wavelet packet decomposition.
          Verify perfect reconstruction using the corresponding wavelet packet synthesis routine
          'S四syn七h.
      10. Construct wavelet packet basis functions for a two-level balanced tree starting with the
          Haar scaling function and wavelet. Note that the bases thus obtained are the Walsh
          functions of length four.
                          CHAPTER FIVE


         Wavelet Transform and
          D아a Compres引on



5.1 Introduction
The most widespread application of the wavelet transform so far has been for data
compression. This is related to the fact that the DWT is tied closely to subband
decomposition, and the latter was already being used for compression by the time
the connection between the two was established by Mallat [1989a, 1989b]. This
chapter provides the motivation for using the DT사T for compression, and describes
subband techniques for image, audio, and video compression. We begin with an
overview of common issues related to compression.
   Compression in the context of speech compression, image compression, and so
forth, connotes the process of starting with a source of such data in digital form
(usually either a data stream or a stored file) and creating a representation for it
that uses fewer bits than the original. The aim is to reduce storage requirements or
transmission time when such information is communicated over a distance. Ideally,
we want the compression process to be reversible. That is, given the compressed
data, we would like to be able to recreate the original. When it is possible to do
so, the compression is said to be lossless; otherwise, we have lossy compression.
Suppose a discrete-time signal s (n) is compressed and then reconstructed (that is,
the inverse of the compression process is performed) to yield a signal 3 (n). The
error signal is defined as

                                e(n) = s(n) - 3(n).                            (5.1)

The reconstructed signal can be seen alternatively as an additive noise-contaminated
version of the original by rewriting Equation 5.1 as

                                3(7D= s(n) + w(n)                              (5.2)

                                       133
134   너／ave旭t Transform and Do六7Con）尸旭ss幻n


      where w(n) 三 -e(n) is the noise. For lossless compression, e(n) is identically zero.
      For lossy compression, an objective measure of distortion or figure of merit for
      the quality of the reproduced signal or image is the mean squared value of e(n).
      Alternatively, one might use the related measures of signal-to-noise ratio (SNR) or
      peak signal-to-noise ratio (PSNR) defined as

                                                            squared s (n)
                                    引 == ] () 1ny. n mean
                              S사R (d／                                                    (5.3)
                                  "         mV口lU mean squared e(n)

      and

                                            peak absolute squared value of s(n)
                    P,SNR(dR' = 101ncr. 八                                                (5.4)
                          "      --h口lU             mean squared e(n)

      respectively.
          However, such objective measures may not be satisfactory perceptually; that is,
      they do not necessarily reflect the magnitude of distortion as perceived by our
      senses. We illustrate this with an image example. Figure 5.1 shows an image
      represented using 8 bits per pixel. Figure 5.2 shows a low-frequency noise pattern.
      Figure 5.3 shows the original image with the low-frequency noise pattern added to
      it. Figure 5.4 shows a high-frequency noise pattern with the same total energy as the
      low-frequency noise pattern in Figure 5.2. Figure 5.5 shows the original image with
      this high-frequency noise pattern added to it. Even though the SNRs are the same
      for the images in Figures 5.3 and 5.5, the latter appears closer to the original than
      the former. This is attributed to visual perception being inherently more sensitive
      to low-frequency variations than to high-frequency variations.
          Compression has been characterized as the removal of redundancy and irrele-
      vancy [Jayant and Noll 1984]. The former results in lossless compression whereas
      the latter results in lossy compression. To illustrate the removal of redundancy,
      consider Figure 5.6, which shows a finite-length discrete-time signal x(n). The sig-
      nal has more than 16 distinct levels, which indicates that we need at least 5 bits per
      sample to represent the data. However, if we form the difference signal

                                       y(n) = x(n) - x (n - 1)                           (5.5)

      we see that there are only six distinct values (Figure 5.7), indicating that y(n) can be
      represented accurately using only 3 bits per sample. This implies that x (n) can be
      represented using only 3 bits per sample as well, because it can be obtained from
      y (n) as

                                      x(n) =y(n) +x(n -1).                               (5.6)
                                                                             Introduction   135




   Figure 5.1 Original "girl" image.


   The key theoretical result related to the maximal amount of lossless compression
possible for a given source is related to the entropy rate-an important concept in
information theory [Cover and Thomas 19911. Suppose we have a memoryless source
S of random data that puts out one of M possible values or symbols, a1, a2, .. ., aM
with probabilities pi, P2 . . . , PM respectively. The entropy of the source in units of
bits per symbol is defined as

                                           M

                                 H(S) = - ＞二 Pm log2 Pm.                          (5.7)
                                          m=1


Suppose we now collect blocks of N consecutive samples of the source output and
form a vector bN = Wi, b2, . . . , bN1. Each such block can be viewed as a symbol
136   Wavelet Transform and Data Compre訶on




        Figure 5.2 Low-frequency noise.




      coming from a source of random vectors which we will call SN. There are M's' such
      vectors in 5N, which is called an extended source. Let



                              qi = P(b1 = al, b2 = ai, ., bN = ai)

                              q2 = P(b1 = a1, b2 = a1, ., Z7N = a2)
                                                                                  (5.8)


                            qMN = P(b1 = aM, b2 = aM, ., bN = aM)
                                                                                    Introduction   137




   Figure 5.3 The "girl" image with the low-frequency noise of Figure 5.2 added to it,



where P() denotes "probability of." The entropy of the extended source in bits per
symbol (the extended source's symbol) is given by

                                              Mi
                                                   "


                                 月（SN) = H ＞二qm log2 q,                                   (5功
                                             m=1


The entropy rate of a source S (memoryless or otherwise) in bits per symbol is
defined as


                                     H=
                                     // = lilll
                                          hm H(SN)                                       (5.10)
                                          N-＋以）        N
]38   Wavelet Trans幻rm and D아a Co쨔加到on




         디gure 5.4 네gh-frequency n이Se.


      In the special case when successive symbols from the source S are independent, the
      probabilities q,, in Equation 5.8 are products of the probabilities pm. For example,
      ql= /7lN, q2 = /7lN-1J72, and so on. Consequently, for such a memoryless source,

                                          H(SN) = NH(S)                                  (5.11)

      and the entropy rate

                                             H = H(S).                                   (5.12)

         A fundamental result in information theory, known as Shannon's theorem for
      noiseless coding, is that the average number of bits required to represent the symbols of
      the source S by lossless compression is always greater than or equal to the entropy rate H
                                                                                Introduction   139




   Figure 5.5 The "girl" rn（그ge \A／汁h 十he 볘gh升equency n이se of 日gure 5.4 added to it.



of the source. The closer a lossless compression technique gets its representation to
the limit imposed by the entropy rate, the more efficient or better it is. Since the
principal aim of lossless coding is to achieve bit rates close to this limit, lossless
coding is also referred to as entro끄／coding. Examples of entropy coding techniques
are Huffman coding, arithmetic coding, and Ziv-Lempel coding [Sayood 19961.
   Removing irrelevancy is possible with data because often there is more informa-
lion than required. This is illustrated in Figure 5.8. Figure 5.8A shows an image
that has 62 levels. We can thus use 6 bits per pixel. Figure 5.8B shows an image
obtained by rounding off the gray values in Figure 5.8A to the nearest of 32 fixed
values. Visually there is no difference between the two pictures. But the differences
are clearly seen when one views the algebraic difference between the two as in Fig-
ure 5.8C. Thus, purely from the point of view of visual perception, one might do
140   Wavelet Transform and Data Compression




              Figure 5.6 C川gn이（계screte-time 引gn（긔．



      just as well with Figure 5.8B, requiring 5 bits per pixel, as with Figure 5.8A, which
      requires more bits. We conclude that the extra detail conveyed by Figure 5.8A is
      irrelevant. This example illustrates the subjective nature of defining irrelevancy.
         In most data compression situations we see the use of both iossy and lossless
      components. A key operation in lossy compression is quantization. A scalar quan-




                                         OO               O   O


                                                                                       O



                                                      卄            旴        冊 우

                                O


                                                                       OO

                        小30          5           10           15       20              25
                                                                             n   -+-
             Figure 5.7 The difference signal.
                                                                         幻却od（火夕ion   141




                                    (A)




                                    （助


Figure 5.8 Example to illustrate irrelevancy in an image. (A) Original image
           quantized at 6 bits per pixel. (B) Same image quantized to 5 bits
           口er pixel.
142   너／0velet 了尺,ns幻rm and O아a Con가9ression
                                                                          Transform Coding         143


                                                           A
                                                                  y
                                                               (output)




                                                 \’드   H




   '                                  y4   I               '    0
                                                                                (in츰Ut)
                                               Y2 -


                                               -'I     -




                                                           V




Figure 5.9 Ex（가1갸引e of a quantizer.



such as digitized speech samples. Suppose we create N-dimensional vectors from
these by taking blocks of N consecutive samples. These vectors are obviously in an
N-dimensional linear vector space. Let x = [Xi, x2. ....xNIT be a vector of the origi-
nal data samples. We can view the values Xi, x2, . .. , XN as being the coordinates of
x with respect to the standard or usual basis of an N-dimensional Euclidean space.
That is, if a1, a2. . . . .aN are the basis vectors then


                                                           N
                                                           Z向                             (5.16)         =




with a1 = [1, 0. . . . .01T, a2 = [0, 1. . . . .01T, and so on. Suppose we now choose to
use a different set of basis vectors b11; n = 1. . . . .N to represent x as


                                       X                   N
                                                           Z由   V
                                                                J
                                                                 n   b
                                                                     n                    (5.17)
144   Wavelet 刀an＄幻rm and D아（7（力mpre弱Ian

      for values Yi, Y2. ... .YN, which are the coordinates of x with respect to this new
      basis. Then

                                               x = By                                     (5.18)
      where B is the matrix with columns that are the basis vectors b1 through bN:

                                        B= [b1, b2. . . . .bN}                            (5.19)

      and

                                        y= [yl, y2. . ...YN]T.                            (5.20)

      Alternatively,

                                               y= Tx                                      (5.21)

      where T = B-1. Equation 5.21 is a linear transformation of vector x. Thus a coor-
      dinate transformation of the type described is equivalent to a linear transformation
      of the input data vector. The first step in transform coding is the transformation of
      the input vector x to y. We expect the transformation to accomplish the following
      objectives:

       1. To create a representation for the data in which there is less correlation among the
          coefficient values. This is often referred to as decorrelating the data. Thus, in
          Equation 5.21, we would like to choose a transformation matrix T that would
          produce a representation y such that the correlation among its components
          yi, . .. , YN is less than the correlation among the components of the x vector
          (namely, xl. . . . . 工N). In fact, the ideal transformation is one that results in zero
          correlation among the transform coefficients. The transformation that accom-
          plishes this is the Karhunen-Loeve transform (KLT). However, the KLT is consid-
          ered an impractical transform because it is signal dependent in the sense that
          the corresponding matrix I has to be derived from the statistical characteris-
          tics of the input vector. Therefore, in practice we settle for transforms with
          data-independent matrices that attempt to reduce the correlation among the
          transformed coefficients as much as possible rather than eliminate the correla-
          tion completely. The purpose of decorrelation is to reduce redundancy, which
          enables us to quantize each coefficient independently of the others.
       2. To have a representation in which it is possible to quantize different coordinates with
          different precision. This in effect amounts to making certain coordinates more
          important than others. For example, if we were to choose a transformation T
          such that most of the energy in the transform vector y is concentrated in the
          first two or three coefficients, then we can afford to quantize these coefficients to
          greater precision while quantizing other coefficients using less precision. Matrix
          transformations that seek to achieve objective I tend to achieve objective 2 as
                                                                                  加ns幻rm Coding        145


   S（川
                                                                                         三（n)
                                                                        Inverse
                   Trans化I-In                                          Transfonn


                                                               CN 1




 Figure 5.10 텨ock diagn그mc寸 a iossy 加nsform co（계ng scheme.


   well. For example, the KLT is the best transform there is in terms of packing
   most of the energy into the 丘rst few transform coefficients.

   In keeping with objectives I and 2, the step that follows the transformation is
scalar quantization of the transformation coefficients. This involves the formation
of the vector

                                       $,=E91. ..9N]T                                       (5.22)

where

                                         ;i= Q{yJ

for i = 1, . . ., N. The function Q, is the quantization characteristic for coefficient
y1. It is determined to a large degree by objective 2. Quantization is followed
usually by a lossless coder (for example, a Huffman coder). At the receiver end, an
approximation of the original x vector, denoted by *, is reconstructed from 5 as

                                          文 = T19.                                          (5.23)


This procedure is depicted in Figure 5.10.
Example 5.1
     We illustrate the concepts in obje虹ves 1 and 2 with the aid of Figure 5.11, which shows
     a data set that consists of points in a two-dimensional vector space. It is possible to
     represent these points using coordinates with respect to either the X-Y pair or the
     A-B pair of orthogonal axes. Suppose we initially represent the data using X-Y. Then
     the coordinates of the points a through f are (0.5,0.0), (2.0,0.6), (1.0,1.0), (- 0.6,0.0),
     (- 1.2,-0.6), and (- 1.3, -1.4) respectively. It is a simple matter to transform these
     coordinates to those with respect to A-B and vice versa. With respect to the A-B axes,
     the coordinates of the points a through fare (0.4, -0.25), (1.9, -0.7), (1.4,0.3), (- 0.5,0.3),
     (- 1.3刀］5), and (- 1.9, -0.4) respective竝．가te dist小毗on 可 the points with res恥ct to
     the A-B axes suggests that a lower value is possible for the cross-correlation between
      the coordinates of the points with respect to this pair of axes than for the X-Y axes.
      As it turns out, using the values of the coordinates given with respect to the two
146    Way이ef 加nsform and /力幻 Con）尸ression




                                            ,   \d \ V          寸／
                                                                        0b
                                                브六十．,                           ,
                                   )./
                                                         \\
           디gure 5.11 Anex（그m디e to illus打ate the r이e （그f 打ansforma卄ons in con갸＞re＄針on.



           coordinate axes, the cross-correlation1 figures are 5.14 for the X-Y axes and -0.395 for
           the A-B axes. Thus we see that this transfor끄［lation does reduce the cross-correlation
           for the given set of points. Also, we see that compared to the A-coordinates, the
           B-coordinates of the points have lower values, which suggests that the B-coordinate
           values can be quantized more severely than the A-coordinate values. For example,
           suppose we rounded off all the A-coordinate values to zero. All the points would
           then be aligned along the B-axis. On the other hand, if we zero out the B-coordinate
           values, all points would be aligned along the A-axis. The attendant shift from their
           original positions is far less than the shift accompanying the zeroing out of the A-
           coordinates. Thus we can use different precision to quantize different coordinates, and
           the objectives of transformation listed earlier are met in transforming the data from the
           X-Y-coordinates to the A-B-coordinates. '                                              1


      Example 5.2
           Transform coding based on frequency domain transformation such as the discrete co-
           sine transform (DCT) takes advantage of the differential sensitivity of perception to
           frequencies. For the DCT, the basis vectors in Equation 5.17 are given by

                                         1_l1 三 rim
                                         LJ            Vn,1l ,... . , 하，
                                                LUnO,, Zh          .On,N-1J
                                                                        N4liT                (5.24)


      lThe de鈿i如如k螂炚orrela如 可 the coordinates is C刈 = ＞二i 工jyj where 工iand
                                                                           yi represent the
      coordinates of each point with respect to the chosen set of axes.
                                                                       DTWT for Image Compression           147


     where

                                                              k= O. ....N- i
                     》，:,*
                             ：   品的cos
                                              ' " 「，
                                                   ,“
                                                        " "

                                         I
                    ce(n) =                                   n= O
                                         Vi
                             =
                                 1                             otherwise.

     The transform vector components y, of Equation 5.17 are given by


                                    Yn=和喀如'欠；"""                                                 (5.25)


        The DCT can be extended to transform two-dimensional signals as well. This can be
     done in a separable manner by first computing the one-dimensional DCT of individual
     rows of the two-dimensional signal and then computing the one-dimensional DCT of
     each colurrm of the signal. If x(k, t ) is the two-dimensional signal of size M x N, then
     the tw아dimensional DCT of the signal is



             玩，교和）蜘）巽如 Os       c。s(2'二""" ·
                      6(2' 品" r 09                                                               (5.26)
     Figure 5.12 shows the DCT of the image in Figure 5.1. Note that most of the energy
     is concentrated in the low-frequency coefficients. Consequently, as noted in objective
     2, these coefficients can be quantized to greater precision. Also, it is well known that
     the DCT approximates the KLT [Ahmed, Natrajan, and Rao 19741 for sources with a
     decaying spectrum. Most images have this type of a spectrum and hence the DCT
     coefficients in general have substantially lower correlation compared with the original
     image. The advantage of transformation is that coefficients associated with perceptually
     less important basis functions can be quantized more coarsely. In other words, we can
     allow for greater reconstruction error in these regions, whereas those associated with
      perceptuany more important oasis tunctions can oe quantizea flneiy.                  -




5.3 DTWT for Image Compression
As discussed in Chapter 3 and shown in Figure 3.9, basis functions of an orthog-
onal DTWT2 are related to the impulse responses of the PRQMF banks used for
decomposition and reconstruction. Suppose we now have a four-level DT汀 per-
formed using the D4 filters. The basis sequences a, (n) for such a DTWT are shown
in Figure 3.11.


2 Recall that the DWT provides an expansion for a continuous-time signal in terms of a basis, whereas the
DTWT does the same for a discrete sequence. We regard an image to be a two-dimensional sequence
and therefore use the term DTWT throughout the book.
148    Wavelet Transform and Data Compression




      Figure 5.12 T＼小／O-（계men針on이 DCI of the "girI' irn（그ge.



           Observe that the basis functions in Figure 3.11 differ in their size or scale, im-
      plying that the DTWT splits or decomposes the given signal into components of
       different scales. Thus the grounding of wavelet transforms in multiscale decompo-
       sitions would seem to provide a justification for its use in image compression and
      analysis. This property assumes significance in light of the work by Marr [19821 and
      others [Marr and Hildreth 1980; Wandell 19951 in vision, where it has been shown
      that a multiresolution or multiscale model provides a good description of
                                                                                        early
      visual processing. In particular, our perception of edges, a crucial image feature,
      appears to be based on their detectability at multiple scales.
          Observing the DT사T of the image in Figure 4.7, we see that the detail images
      contain the edge information in line with the results in human vision research to
      which we alluded earlier. The preponderance of dark regions indicates that most
      of the wavelet coefficients in the details have very low values. Consequently, most
      of these can be quantized to zero without affecting the perceived quality of the
      reconstructed image significantly. All wavelet-based image compression techniques
      take advantage of this phenomenon. Theoretical results have been obtained to show
                                                            ／万WT幻r image Compre訶on        149

that wavelet bases are unconditional bases [Daubechies 1992; Meyer 1993a] for several
spaces, including the space of square integrable sequences [Donoho 1993]. This
makes them near optimal for compressing data in certain types of spaces.


5.3.1 Image Compression Using DTWT and Run-Length Encoding

In general, transform-based image compression schemes follow the process shown
in Figure 5.10. We now describe a scheme that uses the DTWT as the transform,
a quantizer that is similar to the one specified by the FBI [Hopper, Bnslawn, and
Bradeley 19931 for their fingerprint compression scheme, run-length encoding, and
lastly Huffman encoding before storing or transmitting the data. The DTWT and
its computations have been described in Chapters 1 through 4. For this example,
we decomposed the image to five levels using the linear-phase biorthogonal filters
listed in Table 4.2, which were used by the FBI for their scheme. We now describe
 the quantizer and the Huffman coding blocks in detail.

5.3.1.1   Quantizer

As mentioned, each subband is quantized differently depending on its importance,
which is often based on its energy content or variance. Thus, low-variance/energy
subbands would be allocated fewer bits and consequently they would be quantized
in a coarser manner, whereas higher variance subbands would be allocated a larger
number of bits and hence would be quantized in a finer fashion. This is done under
the constraint of compressing an image to a certain compression ratio and hence to
a specified number of bits. This gives us a bit rate (average number of bits per pixel)
to work with and hence we are required to allocate a certain number of bits to each
 subband to achieve this bit rate as an average over all subbands. At the same time
it is important that we allocate bits to each subband to minimize some cost function
related to distortion. The cost function we use is a measure of the sum of the
 quantization error variance of the subbands and is given by [Jayant and Noll 19841

                                      N

                                     ＞二a
                                     i= 1
                                            a   2'
                                                      2r,
                                                                                 (5.27)


 where N is the number of wavelet subbands, r, is the bits allocated to the ith sub-
 band, 아 is the standard deviation of the ith subband, and a, is the number of coef-
 ficients in the ith subband divided by the total number of coefficients in the image.
     Assume that we need to compress the image to R bits per pixel. We must then
 minimize this cost function under the constraint


                                     R= )   Z
                                            NH        吼
                                                     a1r1                        (5.28)
150    Wavelet 刀（)flS幻rm and D아a Cc가npre弱ion

       to obtain the number of bits, r,, for each subband. Minimizing [Panchapakesan
       1996], we get

                                                                                                             寸比
                                                                               l 4n
                                                                               4  =
                                )
                                                                                                   (
                   +                                                                  b
                                                                                      勘                                                   凡
                        尸
                                                                    r1= : log) I _ ,, ' L. I + R.
                                                                                               1
                                                                                                                       2
                                                                                                                                 m                        (5.29)
                    l
                            /
                                                                                                                   아
                                                                                           \
         The quantizer used by the FBI is a nonuniform quantizer with a larger zero-bin
       width. For the subband i, the bin width is given by

                                                                                      -l                 2ycr
                                                                                      1/i = 二11
                                                                                            =                ' 1
                                                                                                                                                          (5.30)

      where y is called the loading factor and specifies the range of the quantizer. The
      zero-bin width is then given by


                                                                                      Zi= C, Q1                                                           (5.31)

      where C, is a constant normally chosen to be in the range 1.2 to 1.5. The subband
      coefficients a (m, n) are quantized according to the following rule:


                              I L (a' (m, ,
                                         n)-Z1/2) +1], a (m, n) >Z,/2
                   q,(m, n) = { 0, . , . '             -Z,/2 <a1(m, n) <Z1/2                                                                              (5.32)
                                                       I r ("''他'笭"z'/2)
                                                         [(a
                                                                     /')
                                                                    (m·
                                                                          n+
                                                                                                       l],
                                                                                                       11,         m(m,
                                                                                                                   a,   n) <
                                                                                                                           < 1Zi/2
                                                                                                                           (m,
                                                                                                                                     n)
                                                                                                                                            -
                                                                                                                                                Z,
                                                                                                                                                     /2
      where qj (m, n) are the quantized subband coefficients, L ] represents the largest
      integer less than or equal to the argument, and 11 represents the smallest inte-
      ger greater than or equal to the argument. At the decoder end, these quantized
      coefficients are dequantized as follows


                                                         [ (qk(m, n) - K) Q1 + Z,/2,                                                      吼（m, 兀） > 0
                                    a   (m,
                                              n)
                                                   =    i      0,
                                                                                                                                          qk (m, n) = 0   (5.33)
                                                         I. (qk (m, n) + K) Q, - Z,/2,                                                    吼（m, 兀） < 0.

      The value K determines the reconstructed value of自佃i, n). A value K = 1/2 would
      place the reconstructed value exactly at the center of that quantization bin.

      5.3.1.2 Huffman Coding
      As mentioned, most wavelet coefficients in the detail regions have very low values.
      As a result, after quantization most of the wavelet coefficients in these regions have
      a value equal to zero. This property is exploited in the Huffman coding of the detail
      regions. To build a Huffman code we collect statistics in the following manner:
                                                            DT너T for Image Compression     151

 1. We define categories into which to group the nonzero data. A coefficient Cm,n
    belongs to category i if it lies in the ranges H2" + I 드 Cm,n 5 _2t_1 or 2;l 5
    Cm,n 5 2" - 1. For this example, eight categories are used.

 2. Next we define a zero-run as the number of consecutive zeros before encounter-
    ing a nonzero value. For our example we chose a total of 31 zero-runs consisting
    of 0 to 30 zeros.

 3. We then collect statistics for the pair of zero-run and category while scanning
    through the detail subbands in a subband-by-subband manner.

 4. Lastly, we note special cases, such as when a zero-run terminates at the end of
    a subband instead of at a nonzero value. This is the end-of-block (EOB) case.
    Another special case occurs when a nonzero value does not belong to any of the
    specified categories or the zero-run exceeds the specified limit (in our case, 30).
    Another special case to consider is when a given subband has a zero variance
    or all constant values after quantization.


For our example, this gives a total of 31 x 8 + 3 = 251 code words. After the code
words have been generated, they are stored or transmitted along with the offset
from the base value of the category for the nonzero value that has terminated the
run. The base value is defined as the smallest value in that category. For the ith
category, this value is -2k + 1. Note that the code word specifies the zero-run
and the category. The various special cases are treated as follows: If the zero-run
exceeds the specified limit or if the nonzero terminating character does not belong to
a specified category, then the code for this case is transmitted, followed by the actual
values of both. Similarly, for the EOB case, the EOB code is followed by the zero-
run value. Lastly, for the zero-variance case, the zero-variance code is transmitted,
followed by the constant value of the pixels in the subband. This scheme is very
similar to the scheme used in JPEG (Joint Photographic Experts Group).
   Note that the low-pass subband is coded separately. Here, the Huffman table
and the code are generated simply by collecting the statistics of the band in the
normal fashion. The compression results for this scheme are shown in Figure 5.13.



5.3.2 Embedded Tree Image Coding

Generally, most of the energy in an image is concentrated in the low-frequency re-
gion. Typically an image is assumed to have a spectrum that decays with increasing
frequency. Hence, one expects that in general these properties of an image would
manifest themselves in the DTWT of an image. Suppose we effect an n-level decom-
position of an image. Then the lower levels of decomposition would correspond to
the higher frequency subbands. In particular, level one would represent the highest
152    너／0velet Trans幻rm and D아a（力叫가a到on




         Figure 5.13 Compression results for the D1八／r-quantizer-Huffman coding scheme for the
                     'girl" image (A). The compression ratio is 7.5:1.



       frequency subbands and would be the finest level of resolution. Conversely, the nth
      level would correspond to the lowest frequency subbands and would correspond
      to the coarsest resolution. Thus, as one moves from higher levels to lower levels
      (equivalently, from lower resolution to higher resolution) of a subband decomposi-
      tion, one would expect to see a decrease in the energy content of a subband. Also,
      if the DTWT coefficients at a particular level have a small magnitude, then it is ex-
      pected that the DTWT coefficients at lower levels corresponding to the same spatial
      position would have smaller values. This is seen to be generally true in practice.
      In addition, it is seen that there are spatial self-similarities across subbands. For ex-
      ample, consider the DTWT of the image shown in Figure 4.7. The contours (edges)
                                                                DTWT／아劤age C（가n尸ress/on   153




   Figure 5.13 (continued) (B) The compression ratio is 14:1,


of the girl are seen in each subband at the lower levels along with a coarse ver-
sion of the image in the low-pass subband. Also, note the spatial position of these
similarities across the subbands. In each subband, or equivalently at different res-
olutions, they occupy the same spatial position. The embedded zero-tree wavelet
coding algorithm, introduced by Shapiro [19931, exploits these properties to give
excellent compression results. Another algorithm that exploits these properties is
the set partitioning in hierarchical trees (SPIHT)-based algorithm proposed by Said
and Peariman [1996]. Both these methods produce an embedded bit stream; that is,
a bit stream at a lower rate is contained in a higher rate bit stream.
   We describe the SPIHT algorithm shortly, but first we illustrate a form of coding
called tree coding, which forms the basis of the SPIHT approach. Let us use the
154   Wavelet Transform and Data Compression




         Figure 5.13 (continued) (C) The compression ratio is 18:1.


      coding of a one-dimensional vector for illustration. Let b = [b1, b2, . . ., b8] be an
      eight-component vector. Suppose each component bi, i = 1, .. . , 8, took one of three
      possible values: -1, 0, or 1. Thus for the vector as a whole there are 38 or 6,561
      possible combinations. Suppose we want to create a binary representation for these
      vectors by using a fixed number of bits for each vector. In other words, let us say
      that we want to enter the vectors into a lookup table and we associate each vector
      with its corresponding binary address in the lookup table. A 13-bit address will
      suffice because 2l3 = 8,192, which is of course much more than the 6,561 values we
      need.
         Suppose we now look into an alternative binary representation, which works as
      幻lb ＼仍：
                                                              DTW／幻rIrn四e Corn口ression   ]55




 Figure 5.13 (continued) (D) The compression ratio is 25:1.


1. Arrange the components of the vector b as in Figure 5.14, where b1 is set apart
   from the rest, that are formed into a binary tree with b2 as the root.
2. If b1 = 0, make the first bit of the binary representation 0. If b1 = 1, make the
   first two bits of the representation 10. If b1 = -1, make the first two bits 11.
   Thus anytime we want to code the value of a single component, we code it to
   0 if it is 0, or else we code it to 10 or 11 if it is I or -1 respectively.

3. Append the code for b2 to the code for b1, again coding b2 to one of the three
   possible combinations as explained in the previous step.
4. If all components beyond b2 are 0, append a 0 to the bits generated at the end
   of step 3 and stop; or else, append a I and go to the next step.
156   너／0velet 刀ansform （그nd Data Compres針on


                                 b1                    b,
                                 S                      I
                                               h   ,
                                                       戶／    \
                                               「D                 I,
                                                                      b,
                                              戶／ \        戶／ \
                                          .            0 5     S
                                         b5            b6        b7            b8   (A)




                                  1                         0
                                   I                         0

                                               0.
                                               U0
                                                       / \H
                                                          S.
                                                                           '




                                               戶／
                                                       \\   戶／ \
                                           I             0 0     0
                                          0              0 0       0                (B)


              디gure 5.14 (A. B) Exan갸늬e illu針ra쉬ng the conce口ts involved in zero-tree
                         Co（小ng.


       5. Code the values of b3 and b4 in succession, and append them to the represen-
          tation at the end of step 4.
       6. If the remaining four components b5 through b8 are all 0, then append a 0 to
          the representation obtained thus far and stop; or else, append a 1 and go to the
          next step.

       7. Append the codes for b5 through b8 to the representation at the end of the
          previous step and stop.

        To illustrate how this coding works, let us consider the binary representation for
      b = [1, 0, 0, -1, 0, 0, 0, 01. The following will be the output of each step:

       1. The vector components are arranged as in Figure 5.14.
       2. Code b1 to 10.
       3. Code b2 to 0 and append it to the output of the previous step. The code now
          reads 100.

       4. Append a I to the current representation because there is at least one nonzero
          component (b4) beyond b2. The code now reads 1001.
       5. Append codes for b3 (0) and b4 (11) to the code to yield 1001011.
       6. Because all the remaining components are 0, append a 0 and stop. The final
          representation is 10010110, which consists of 8 bits.
                                                             DTWT f(그시(1그（7ge Cc가71口ress/on   157


It is easy to decode this binary representation back to the original vector [1, 0, 0, -1,
0, 0, 0, 01 simply by retracing the coding procedure. For example, the fact that the
leading (leftmost) bit is a 1 clearly indicates that b7 is not equal to 0. It has to be
I or -1. The next bit in the code is 0. Thus the first two bits 10 let us decode b1
to 1. The third bit being a 0 lets us set b2 = 0. The fourth bit is a 1, indicating that
there is at least one nonzero component beyond this point. The fifth bit is 0, which
means that b3 = 0. The sixth bit being a 1 tells us that b4 尹 0. The sixth and seventh
bits together give us 11, which makes b4 = -1. The eighth bit is 0, implying that b5
through b8 are all 0.
    This representation is of variable length. Shorter length representations are ob-
tamlled for vectors with only zeros at the end, and longer representations are obtained
when the components are overwhelmingly nonzero. The two extreme lengths are
obtained for the case in which all components of b are zero and for the case when
every component of b is nonzero. In the former case, the representation is 3 bits
long-000. In the latter case, assuming for illustration that all components are equal
to 1, the representation, which is 101011010110101010, is 18 bits long. Comparing
this with the previous code that uses a fixed length of 13 bits, we see that the
variable-length code uses far fewer bits for some combinations and many more bits
for others. When is it advantageous to go for the second representation? It is advan-
tageous if the source generating these vectors has inherently a lopsided distribution
that makes the components of the vector more likely to be zero than nonzero. In
particular, we would want the probability of a component being zero increasing as
we move from b1 toward b8. The fact that the DTWTs of typical images conform to
such lopsided characteristics (that is, the pixel values in the detail images are more
likely to be closer to zero than to higher values) lets us achieve high compression
ratios with techniques such as SPIHT.
    We now look into the workings of the SPIHT algorithm. Broadly the method
adheres to the following steps:

 1. Obtain the DTWT of the input image and represent the wavelet transform coef-
    ficients using a finite number of bits, which results in a very fine quantization of
    the DTWT image. For the sake of illustration, let us assume the representation
    to be a 16-bit signed magnitude (that is, the leading bit represents the sign and
    the next 15 bits represent the magnitude). Thus the pixels can have values from
    m(2l5 小 1) to 215 - 1.

 2. Quantize the coefficients to 0, 1, or -1 with the threshold magnitude set to 214.
    In other words, if a wavelet coefficient has a value less than _214, it is set to
    -1; if it has a value greater than 214, it is set to 1; and it is set to 0 otherwise.
    Thus nonzero quantized values are obtained for those coefficients with a second
    most significant bit (MSB) that is a 1. Observe that at this stage the quantized
    wavelet image resembles the data vector of the previous tree-coding example.
158   Wavelet Transform and Data Compression

          The resulting image is called a significance map because it tells us whether or not
          a coefficient is significant with respect to the threshold.

       3. The significance map is tree encoded using the spatial orientation trees described
          later.

       4. The threshold is lowered to 213 and the coding procedure is repeated on the
          pixels considered insignificant in the previous step (that is, on pixels that were
          quantized to zero previously). The resulting binary code is appended to the
          code of the previous step. A binary string of the next MSB in the representation
          of the pixels in the significance maps of the previous steps is now appended to
          the code.

       5. The previous steps are repeated with successively decreasing thresholds 212, 211,
          and so on.

         At every decrease in threshold the total number of bits used to represent the
      image increases, as does the quality of the reconstructed image. In the decoding
      process, one can first reconstruct the image corresponding to just the first threshold,
      then follow it with a reconstruction at the second threshold, and so on. The effect is
      what many would have experienced in downloading images from the Worldwide
      Web, where the image quality goes from coarse to fine right in front of our eyes.
      This is called progressive transmission.
         We now describe the coding procedure in detail. The DT사T coefficients are first
      organi乙ed into spatial orientation trees. Fig工re 5.15 illustrates how these trees are
      formed. The image is assumed to be decomposed to two levels. The LL2 or the
      low-pass subband contains the coarse low-pass approximation of the original image.
      The pixels in this subband are formed into groups of 2 x 2 pixels. One such group is
      shown in Figure 5.15. Out of these, the top left pixel of each group (pixel 1) will not
      be a part of any tree. The other three pixels of each group (pixels 2, 3, and 4) have
      four "offspring" (also called descendants or children) in groups of 2 x 2 in subbands
      LH2, HL2, and HH2 respectively. These are shown in Figure 5.15 by the arrows.
      In this manner, the first stage of the tree is constructed. To grow the tree further,
      the subbands LH2, HL2, and HH2 are linked with subbands LH1, HLI, and HHI
      respectively in a somewhat similar manner. Each pixel (i, i) from the former set of
      subbands acts as a root for pixels (2i, 2)), (2i + 1, 2)), (2i, 2) + 1), and (2i + 1, 2) +1)
      in LHI, HL1, and HH1 respectively. For a general n-level decomposition, this is
      the rule that links pixels of the adjacent subbands starting from LHn, HLn, and
      HHn respectively. Thus a given pixel can act as a root for a spatial tree formed by
      successive branching of its descendants. Note the differences between the first and
      the subsequent steps of tree formation. In the first step, the pixels in the low-pass
      subband are linked with pixels of the three high-pass subbands at the same level.
      Also, as can be seen from the previous description, not all pixels of the low-pass
                                                                 DTW for Image Compression   159


           1 3                              >
           2 4




                   \\

       Figure 5.15 Relationship between pixels in spatial orientation trees, The pixels
                   have been shaded to clarify the 햐＞（그ti（기 r이ationsh巾 across
                   subbands.


subband are involved in tree formation (that is, not all of them serve as roots for
a tree). On the other hand, in subsequent steps, all the pixels of a subband are
involved in the tree-forming process. The pixels in each subband are linked to the
pixels of the adjacent subband at the next lower level as explained. The branching
stops at the first level because there are no further subbands.
   At each threshold except the first, the coding consists of two passes-the sorting
pass (where the significance map is tree encoded) and the refinement pass (where the
next MSB of each pixel found to be previously significant is appended). Only the
sorting pass is made for the first threshold. To elaborate, given an integer n, all
coefficients greater in magnitude than 2' are considered significant and all others
are considered insignificant. The pass involves going through the data several times
and selecting coefficients such that 2" 5 1Ci, /1 드 2"+1, with n being decremented at
each pass. The sorting pass divides the pixels into partitioning subsets and then
tests each of these subsets for significant pixels. On finding that some pixels in the
160   너／0velet／尺ins幻rm and Data Con）尸ression

      subset are significant, it divides the subset into smaller subsets in accordance to
      some predetermined rule. This process continues until all the pixels in that subset
      have been tested for significance.
         The refinement pass involves transmitting the nth MSB of all the coefficients
      found to be significant when compared with 2n+1. These bits are transmitted in
      the same general order as used to transmit the significance map during the sorting
      pass.
         For the implementation of the algorithm, the following three lists are used: list of
      insignificant pixels (LIP), list of significant pixels (LSP), and list of insignificant sets (US).
      At the end of each sorting pass, the LSP contains the coordinates of all those pixels
      found to be significant at that threshold. Obviously this includes coefficients found
      to be significant at previous thresholds as well. The entries in the US are again
      coordinates of pixels used as representatives for certain pixel sets. These entries
      can be of either type A or type B. A type A pixel represents all its descendents. A
      type B pixel represents all its descendants from its grandchildren onward. Let c ,j
      represent the DTWT image. The algorithm consists of the following steps:

       I. Initialization: In this step we output n = [log2 (max(I,J) c,키)]. Here L j repre-
          sents the largest integer less than Ici,j I. This initializes the value of n for testing
          significance of pixels and constructing the significance map. The LSP is set as
          an empty list. The U1S is initialized to contain all the pixels in the low-pass
          subband that have descendents and hence act as roots of spatial trees. All these
          pixels are assigned to be of type A. The LIP is initialized to contain all the pixels
          in the low-pass subband.

       2. Sorting pass: Each entry of the LIP is tested for significance with respect to n
          (as explained previously). If it is significant then a I is transmitted, a sign bit
          representing the sign of that pixel is transmitted, and the pixel coordinates are
          moved to the LSP. If it is not significant a 0 is transmitted. In this manner
          a significance map is transmitted. Next, each entry of the US is tested for the
          existence of significant descendents. If there are none, then a 0 is transmitted. If
          the entry has at least one significant descendent then a I is transmitted and each
          of the immediate descendants are tested for significance. If significant, a I and
          a sign bit are transmitted and the pixel coordinates are appended to the LSP.
          If not significant, a 0 is transmitted and the pixel coordinates are appended to
          the LIP. Thus a significance map of the immediate descendants is transmitted.
          If the pixel has more descendents (that is, grandchildren and beyond), then
          it is moved to the end of the LIS as an entry of type B. If an entry in the
          U1S is of type B, then its descendents-grandchildren onward-are tested for
          significance. If at least one of them is significant, then this entry is removed
          from the list and its immediate descendents are appended to the end of the list
          as entries of type A.
                                                                                DTW자아伽（7ge Corn尸ression   161


 3. Refinement pass: The nth MSB of the magnitude of each entry of the LSP, except
    those added in the current sorting pass, is transmitted. Note that at the end of
    the first sorting pass, no bits would be transmitted as a part of the refinement
    pass because the LSP contained no pixels prior to the current sorting pass.

 4. Quantization step update: n is decremented by 1 and the procedure is repeated
    from step 2 onward.


   Note that all the entries added at the end of the US are evaluated before going
on to the refinement stage. Also, since coding takes place in a bitwise manner, it
can be stopped at any point, as soon as some desired criterion such as required
bit rate or distortion measure is met. As seen from the previous explanation, the
coding algorithm follows a very definite path and the bits are also sent in a very
definite order. Thus, at the decoder end it is possible to retrace the coding path
and retrieve the significance maps transmitted. Based on this, appropriate values
can be allocated to each pixel position, noting that the mid value of the signifi-
cance range ([2' +1 - 2'1/2) is added to every significant pixel. In this manner an
approximation of the subband-decomposed image is reconstructed. Finally, tak-
ing the inverse DT사T of this subband image gives a lossy version of the original
image.
   Figure 5.16 shows an example of two-level wavelet decomposition. We use this
example to demonstrate a couple of iterations of the algorithm.




                                0                              4   5        6       7

                            62      34    18      17      -4       l    -   2       6

                            -31 24       -15      14      小11      0        4   寸       l

                            42      20   -35      10       29      10       6       9

                        3   -12 15       -9       15      -    1   9        5   13

                        4       4   45    13      -   1    26 -21           3       l

                                3   0    -2       21      -    1   0        7       9

                                0   13        4       5        4   5        6       0

                        7   -   1   7    -11          3        0   8        2       7


        Figure 5.16 A two나ev이 낚／（그＼ielet decori耳兀S出on of a 16 >< 16 irn（그ge to
                    demonstrate the SF가HI士）（그sed 이gorithm.
162   Wavelet Transform and Dat八力끼가e訶on


                                           [IS           LIP           LSI'

                                         (0,1)-A         (0,0)
                                         (1,0)-A         (0,1)
                                         (I，나A           (1,0)
                                                         (1,1)




              Figure 5.17 Initialization of the lists for the SPIHT-based algorithm.



         The pixel coordinates are labeled as (row,column). Because the maximum pixel
      value in Figure 5.16 is 62, the threshold is chosen as n = [1Og2(maxj,j Ici,.j I)] =
      L1Og2(62)j = 5. Using Figure 5.16 the process can be described as follows:

       1. The lists are initialized as follows: The US contains the pixel coordinates (0,1),
          (1,0), (1,1) as type A entries. The LIP contains the coordinates: (0,0), (0,1),
          (1,0), (1,1). The LIS is initialized to be an empty list. The status of the three
          lists after initialization is shown in Figure 5.17.

       2. The elements in the LIP are tested for significance and, if found significant,
          are moved to the LSP. A I and a bit representing the sign of the pixel are
          transmitted. In our case, (0,0) and (0,1) are found to be significant and are
          removed to the LSP. A bit sequence of 1,0, representing the significance and the
          sign (positive), respectively, is transmitted for each. If some elements are found
          to be not significant, a 0 is transmitted for them as in the case of (1,0) and (1,1).
          The status of the lists at the end of this stage is shown in Figure 5.18.
       3. Now the elements of the U1S are tested for significant descendents. If none are
          found, then a 0 is transmitted for that case. Thus, for the entry (0,1) a 0 is
          transmitted. If there are some significant descendents, then a I is transmitted




                                   [IS             LIP           LSP      Transmit



                                                                 벎
                                 (0,1)-A                                  ) 1,0
                                 (1,0)-A                                  ) 1.0
                                 (1,1)-A           (1
                                                     으：
                                                   (1：
                                                                          > 0
                                                                          > 0




              Figure 5.18 Status of the lists after checking the contents of the LIP for
                          significance.
                                                                                    DTWT for Image Compression   163

  for that entry and its immediate descendents are tested for significance. In our
  example, (1,0) has significant descendents, so a 1 is transmitted. Its immediate
  descendents-(2,0), (2,1), (3,0), (3,1)-are now tested for significance. (2,0) is
  found to be significant and is appended to the LSP. The bit sequence (1,0),
  representing the significance and the sign (positive), respectively, is transmitted.
  The other three pixels are insignificant with respect to the current threshold and
  their coordinates are appended to the LIP while a 0 is transmitted for each of
  these. Next, (1,0) is moved to the bottom of the US as type B because it has
  descendents beyond its immediate offspring. An identical procedure is followed
  for the pixel (1,1) and it is moved to the bottom of the US as type B. The status
  of the lists at the end of this step is shown in Figure 5.19.

4. Now the algorithm encounters (1,0) as a type B pixel and examines if it has any
   significant descendents, grandchildren onward. Since it does, a 1 is transmitted,
   its immediate descendents (children)-(2,0), (2,1), (3,0), (3,1)-are appended to
   the U1S as type A entries and the entry (1,0) is removed. This is denoted by
   " x " placed across that entry in the LIS in Fi암lre 5.19. Because (1,1) does not
   have any significant descendents, grandchildren onward, a 0 is transmitted. The
   entries in the three lists at the end of this step are shown in Figure 5.20.

5. Finally, (2,0), (2,1), (3,0), (3,1) are tested for significant descendents. (2,0) has
   a significant descendent located at (4,1), so a I is transmitted and the signifi-
   cance information of its children is transmitted. Because it does not have any




                              LIS         LIP        LSP               Transmit



                                                     벎
                            (0,1)-A -                                      0
                          Hbd-A-
                                                                          1,
                                                                         1,0
                           夕田寸中          (1,0)                            0
                                         (.      )                        0
                          누（1,0)-B
                                          i2J.
                                                               1느              r}
                                                               戶P              U
                          누（1,1)-B                             1느
                                                               戶
                                                                               =
                                                                               1
                                                     (2,0) -   누         1,0
                                         (2,1) -               누          0
                                         (3,0)                 ,          0
                                         (3,1)                 >          0
                                                               戶          1
                                                     (2,2)     )'        1,1
                                         (2,3)                 )'              0
                                         (3刀                       '           0
                                         (3,3)                 >               0



       Figure 5.19 Status of the lists after going through the initial type A entries
                   of the LIS.
164   너／0velet Tran計orm and 0아（7Corn尸re弱ion



                                 I-   Is   LIP   LSP   Transn血
                        DTWT for Image Compression   165




U1S   LIP   LSP   Transmit
166   Wavelet Transform and Data Compression

          pixels (0,2) and (0,3) are found to be significant, and a I along with a 0 (rep-
          resenting the sign) are transmitted for each of them while appending them to
          the LSP. The other two descendents, (1,2) and (1,3), are insignificant and thus
          are appended to the LIP and a 0 is transmitted for each of them. Since (0,1) has
          descendents, grandchildren onward, it is also moved to the end of the LIS as an
          entry of type B. Now we encounter the pixel (1,1)as a type B entry and hence its
          descendents, grandchildren onward, are tested for significance. Because there
          are significant pixels among these descendents, the offspring of (1,1)-namely,
          (2,2),(2,3),(3,2),and (3,3)-are appended to the end of the U1S as type A pixels.
          The next pixel in the list is (2,1) as a type A pixel. Its immediate descendents
          are (4,2),(4,3),(5,2),and (5,3),and out of these, pixel (5,3) is significant. So, a 1
          is transmitted to signify this and its immediate descendents are tested for sig-
          nificance. Since pixels (4,2),(4,3),and (5,2) are insignificant, they are appended
          to the LIP and a 0 is transmitted for each of these. Pixel (5,3) is significant and
          so it is appended to the LSP, and a 1 along with a 0(for the sign) is transmitted.
          Because (2,1) does not have any descendents beyond its offspring, it is removed
          from the list. The next pixel(3,0)does not have any significant descendents and
          hence a 0 is transmitted. The rest of the pixels in the US can be seen to belong to
          one of the types described earlier and hence are treated in a similar manner. Fig-
          ure 5.23 shows the process and the final status of the three lists after this step.
       3. The next pass is the refinement pass. In this pass the fourth bit of the entries
          in the LSP prior to the last sorting pass is transmitted. These entries are pixels
          (0,0),(0,1),(2,0),(2,2),and (4,1), and the bit stream transmitted is 1,0,1,0,1.

      This process continues until some stopping condition such as the required bit rate
      is met.
         The compression results for the SPIHT-based algorithm are shown in Figure 5.24.


      5.3.3 Comparison with JPEG
      A popular scheme for lossy image compression is the DCT-based scheme known as
      JPEG. For a grayscale image, the procedure consists broadly of the following. The
      image is partitioned into blocks, each 8 x 8 pixels in size. An 8 x 8 DCT of each block
      is obtained. By working with the DCTs of these blocks rather than with a single DCT
      of the entire image, it is possible to obtain localization of information in space and
      frequency rather than frequency alone. This is similar to the reasoning supporting
      the STFT. Each 8 x 8 DCT is quantized. The higher frequencies are quantized more
      severely than the lower frequencies in accordance with perceptual considerations.
      It is typically found that quantization forces most of the high-frequency coefficients
      to zero. The quantized values are then entropy coded. Reconstruction is done
      by entropy decoding followed by the inverse DCTs of the blocks. Because of the
DTW了for Image C（가기口ression   167
168   Wavelet Transform and Data Compression




        Figure 5.24 Compression results with the SPIHT-based algorithm, (A) The results are
                    shown for the compression ratio 10:1.



         Yet another example is provided in Figure 5.26 in which a comparison between a
      JPEG-compressed and a wavelet-compressed color image is made. For the wavelet
      case, the original image available in red-green-blue (RGB) format was first con-
      verted to a YCb Cr image using the transformation



                                                                            RGB
                         [ }' 1  [ 0.2990          0.5870      0.1140'
                         1C, 1 = 1 -0.1687        -0.3313      0.5000                         (5.34)
                         L Cr]   L 0.5000         -0.4187      0.0813 -

      where Y represents the grayscale or luminance component whereas C, and Cr rep-
      resent the color or chrominance components [Rao and Hwang 19961. Each of these
                                                               DTWT for Image Compression   169




   Figure 5.24 (con加）ued) (B) The resu必 are sho＼八／n 幻rthe compr眺如nr（그ti（그 20:1.



components was compressed separately using the SPIHT algorithm and transformed
back to the RGB format using the following relationships


                        R = Y + 1.42Cr - 178.753                                  (5.35)
                       G = Y - 0.3441Cb - 0.7141Cr + 134.93                       (5.36)
                       B = Y+ l. 772Cb- 225.93                                    (5.37)

for display and printing. Observe from Figures 5.26 that at this compression ratio
both JPEG and SPIHT tend to smooth out the grainy regions of the image.
                                                                           How-
ever, the JPEG-compressed image also exhibits blocking artifacts. Wavelets have
170   Wavelet Transform and Data Compression




        Figure 5.24 (continued)(C)The results are shown for the compression ratio 40:1



      been combined with other techniques such as trellis-coded quantization [Sriram
      and Marcellin 19951 to obtain good quality images at high compression ratios.


      5.4 Audio Compression
      The DTWT or subband decomposition techniques are used for the compression
      of audio and wideband speech signals. There seems to be a perceptual basis in
      audio perception for using such decomposition. The frequency range for human
      hearing extends to 20 kHz. Consequently, when an analog audio signal is sampled,
      the sampling frequency has to be greater than 40 kHz. In applications such as
      audio recording on conventional compact disk (CD),the sampling rate is 44.1 kHz.
                                                                         Audio Compression   171




   Figure 5.24 (continued)(D)The results are shown for the compression ratio 50:1.



Since the sampled data are stored in digital form, only a finite number of levels,
determined by the number of bits allotted per sample, can be used to represent
the signal. In audio CDs, 16 bits per sample are used. This allows for 216 or
65,536 levels. This representation of audio signals by 16-bit words, which are then
decoded to one of 65,536 levels when played, is called pulse code modulation (PCM).
The starting point for audio compression is PCM data.
   In terms of demand placed on data-handling requirements, that of audio is
minuscule compared with imagery. A 640 x 480 image at 24 bits of color re-
quires 7,372,800 bits. If transmitted at 30 images per second, this amounts to
approximately 28 Mbits per second. For a single channel of audio at 44,100 sam-
ples per second and 16 bits per sample, we have 705,600 bits per second. For
172    Wavelet ／仄insform and Da幻（力m尸re弱ion




      Figure 5.25 Comparison between a SPIHT-compressed and JPEG-compressed image at a
                  compression ratio of 37: ]. (A) Original image.



      a two-channel recording, as on a conventional audio CD, this translates to less
      than 2 Mbytes per second. Indeed, even after a high degree of compression, im-
      agery imposes greater demands on data than does uncompressed audio. Never-
      theless, it is worth resorting to audio compression. Benefits of audio compres-
      sion include being able to accommodate more recording time on a storage de-
      vice of given capacity and simultaneous transmission of multiple channels with-
      out increase in transmission rate requirements. The key issue in lossy compres-
      sion schemes is the minimization of distortion. What is exciting about perceptual
                                                                Audio Compression    173




Figure 5.25 (continued)(B) JPEG-compressed image




coding schemes is that the quantization distortion introduced is such that the us-
tener does not perceive the distortion. In other words, the listener is unable to
distinguish between the perceptual coded signal and the input high-bit rate PCM
signal.
   How does one decide that the original and coded versions are perceptually sim-
ilar? Such an evaluation is done by statistical surveys involving computation of
mean opinion scores. Reliable results have been shown to be obtained with triple
stimulus/hidden reference/double-blind tests. The subject is tested on three sig-
]74    너／avelet 加ns向기 andD아（7Compression




      Figure 5.25 (continued) (C) SPIHT-compressed image. Note the differences in the types of
                  at十ifa（나S.



      nals, called A, B, and C, where A is the original unprocessed signal (for
                                                                                  example,
      studio-quality analog audio or 16-bit PCM) whereas one of B and C is the coder un-
      der test, and the other is a reference (for example, 16-bit PCM). Neither the subject
      nor the person administering the test knows which of B and C is the coder under
      test. The subject has to decide which one is the reference and grade the other on
      a five-point scale. A value of five means that the perceived test piece is as good
      as the original and a value of one means that it is very annoying. Intermediate
F勾ure 5.26 A（兀mpa띠加e ex（가T昨引e of con耳Dies읽（)fl of （그 C이（가 image （그t a compres引on
ra加 of 40: 1 . (A) On이n（기 irn（그ge
F gure 5.26 (continued)(B)JPEG-compressed image.
Figure 5.26 (continued)(C)SPIHT-compressed image.
                                                                        Audio Compression   175

values indicate various degrees of perceived differences between the piece and the
original.


5.4.1 Audio Masking
At the heart of current efforts in audio compression is the psychoacoustic phe-
nomenon called masking. The phenomenon has a frequency domain explanation or
description and is easiest to understand when described in terms of tone masking
noise or noise masking tone. Let us begin by looking at very early experiments in
auditory perception in which the threshold of audibility of a pure tone immersed
in white noise was studied. Suppose we have a pure tone of frequency fo Hz im-
mersed in narrowband noise with a spectrum width of Af that is centered at the
tone frequency as shown in Figure 5.27.
   As can be expected, if the energy of the tone is much below that of the noise,
the tone is inaudible. However, as the energy of the tone (its sound pressure level
[SPLI) is increased, it will become audible in due course. The minimum SPL at
which the tone becomes audible is called the threshold. If the SPL of the tone is
below the threshold, we say the noise masks the tone. Of course, the threshold
is a function of the noise SPL. However, over a wide range of SPL, the difference
between the threshold and the SPL of the noise in decibels is a constant. If we
start with a small value of 八f and then increase it while keeping the height of
the noise power spectrum density the same, we find that the threshold increases
in proportion to the bandwidth if until it reaches a certain maximum beyond
which the threshold stays constant. This maximum bandwidth is called the crit-
ical bandwidth [Noll 1993; Scharf 19961. One interpretation of the result has been
that when a tone is masked by white noise, only that portion of the noise power



                                            人




                                           lb                     frequency +



                                         HA／니
        Figure 5.27 Spectrum of pure tone in bandlimited noise.
176   너／avelet Transfort기 (,ndD아a（力mpre訶on




              Figure 5.28 Mask for pure tone.




      spectrum that lies in the critical band contributes to the masking. The critical band-
      width is fairly constant over a wide range of SPLs. However, it varies as a function
      of the center frequency. Also, it depends on the subject and there are variations
      from trial to trial. Researchers have arrived at values for average critical bands
      after experimenting with many subjects. The critical bands have small bandwidths
      (about 500 Hz) for low frequencies and high bandwidths (about 5,000 Hz) at higher
      frequencies [Scharf 19661. This is very much along the lines of the variation of
      center frequency and bandwidth of the wavelet filters as seen in Chapter TI. Al-
      though this experiment involved noise masking a tone, the opposite holds as well.
      A pure tone can mask other tones and wideband signals. Given a pure tone, a
      threshold curve can be drawn such that any other signal with a spectrum fully
      contained within this curve is inaudible or is masked by the tone. An example is
      shown in Figure 5.28. The curve is the masking profile of the tone. Again, it has
      been found that the mask shows a sudden drop at the boundaries of the critical
      band.
         The principle of masking as used in audio compression follows from these phe-
      nomena. The spectrum of a given segment of an audio signal can contain tonal (lines
      in the spectrum) and nontonal components. For each of these components, there is
      a mask such that any extraneous noise falling within the mask is rendered inaudible
      by this component. Thus, if the signal is quantized such that the quantization noise
      spectrum falls under the net masking profile of all components, then the quantized
      signal is indistinguishable perceptually from the input signal [Brandenburg and
      Stoll 1964; Scharf 19961.
                                                                     Audio Compression     177

5.4.2 Standards Specifying Subband Implementation:
      ISO/MPEG Coding 伯r Aud伯
The Moving Picture Experts Group (MPEG) has set audio compression standards.
At this time there are two sets: MPEG-I and MPEG-2. Both sets deal with cod-
ing in three layers referred to simply as layers one, two, and three respectively
[Brandenburg and Stoll 1994; Noll 19931. The coder complexity increases from the
lower to the higher layers with attendant improvement in quality for a given bit
rate. The standards support sampling rates of 32, 44.1, and 48 kHz. The bit rates
range from 32 kbits per second to 192 kbits per second for a single (mono) channel
and 64 kbits per second to 384 kbits per second for a stereo channel. The operating
modes supported by MPEG-i include single channel, dual channel, stereo, and joint
stereo. MPEG-2 supports these modes. In addition it deals with limited bandwidth
and low-bit rate applications at lower sampling rates (16, 22.05, and 24 kHz). It
also supports other modes of operation involving more channels. There is forward
and backward compatibility between MPEG-i and MPEG-2. Forward compatibility
means that an MPEG-2 decoder is able to decode MPEG-i data. Backward com-
patibility means that MPEG-i is able to decode any MPEG-2 data conforming to
the modes supported by MPEG-i. All layers use perceptual coding based on audio
masking. The standards specify the decoder. The encoders are left undefined. Since
the masking is a frequency domain operation, coding is done on isolated bands of
the frequency spectrum of the input signal using subband coding. There are many
common features in encoding at layers one and two. These common features are
described first. For each channel, the input audio samples, commonly in 16-bit
PCM format, are passed through subband filters that provide a decomposition into
32 bands of equal bandwidth. This would mean that for a sampling rate of 48 kHz,
 the bands are each 750 Hz wide. Also, the attendant decimation leaves us with a
sampling rate of 1.5 kHz per band. In parallel with the filtering operation, a fast
Fourier transform (FFT) operation is performed to obtain the spectrum of a segment
of data. This spectrum is used to generate a threshold mask so that the quantization
noise is confined inside this mask.
    In layer one, for every 384 input samples, 12 samples of each subband are col-
lected into blocks. Simultaneously, a 512-point FFT is carried out. For each of these
blocks, a scale factor is determined. The scale factor is simply the maximal value
of the block. From the FF1 a threshold mask is determined for the psychoacous-
 tic masking effect. The threshold mask decides the number of bits that are to be
 allotted to each block. If there is not sufficient energy in a subband, the number
 of bits allotted might actually be zero. Depending on the bit allocation, one of 15
 quantizers is selected. Four bits are used to indicate the quantizer. Six bits are used
 to indicate the scale factor for those bands that have nonzero bit allocations. These
bits are transmitted as side information. The number of bits per sample of the block
 depends on the quantizer chosen for the block. Quantizer one uses 0 bits, whereas
178    Wavelot Transform and Data Cornpress/on

           Audio
           input                                             Scaler and
                     Analysis
                    filter banl                              quantizer
                                                                                                Coded

                                                                              MUX
                                                                                                output
                                                                                                >
                                                        '   Bit allocation
                                  -*-   Threshold   >
                                        \
                       FFT
                                                              and scale
             H小＋




                                          mick
                                                            fa야or codii培
             HPEQ 尸工 (9쇳伊 t )


           Audio
           output
                       Synthesis
                                                              Dequantizer
                       filter bank


                                                                                    DEMUX
                                                                                                 Coded
                                                                                                 input
                                                                                            (
                                                              Bit and scale
                                                                  factor
                                                                decoding



      디gure 5.29 Enc（그der （가心 decoder 伯r layers one and two.


       quantizers two through 15 use as many bits as the number of the quantizer (in other
       words, quantizer two uses 2 bits, quantizer three uses 3 bits, and so on). At the
       decoder, the reverse process is performed.
          Layer two proceeds on similar lines. However, rather than transmitting the scale
       factor for each block, three successive blocks of 12 samples each for a given band
      are considered. If the scale factors do not differ appreciably, then only one of these
      values is transmitted. If they all differ, then all three are transmitted. For situations
      in between, only two of these values are transmitted. While this process introduces
      delay, it also results in savings in the number of bits used. Furthermore, a finer
      masking threshold is generated by using a 1,024-point F丁 rather than a 512-point
      FFT as in layer one. The layer two decoder is identical to the layer one decoder. In
      layer three, the subband transformation is followed by a modified discrete cosine
      transform (MDCT), which provides a finer frequency resolution. Each of the 32-
      band outputs are fed into an 18-point DCT block. The MDCT output is quantized
      and Huffman coded. Figure 5.29 shows the encoder and decoder for layers one and
      two, whereas Figure 5.30 shows the same for layer three.


      5.4.3 Wavelet-Based Audio Coding

      An obvious way of using wavelets in the previous coding scheme is to use wavelet-
      based digital filters in subband decomposition. In effect, this is what is done
      by proposed wavelet schemes. Sinha and Tewfik [1993] describe a scheme in
                                                                                   Audio Compression         179



    Audio input                                            Scaler/Quantizer/
       H           Analysis filter          MDCI       -                       -



                       bank                                Huffman coding
                                                                                                    Coded

                                                                                    MUX
                                                                                                    output




                                                                 Side
                                            Thresh아d
                                                             information
                                              mask

                                        瓦



    Audio output                                               Descale/
                   Synthesis filter                    (     Dequantize/    (
                                    <       IMDCT




                                                                                     D EM U X
                       bank                                Huffman decoding




                                                                     I
                                                                                                     Coded
                                                                                                     input
                                                                                                (




                                                            Side information




Figure 5.30 Encoder and decoder for layer three. IMDCT = inverse modified discrete cosine
            transform.




which the wavelet packet decomposition of audio frames is obtained and then
quantized to keep the distortion below the masking threshold for the frame. The
wavelet packet tree used is shown in Figure 5.31 and is chosen such that the sub-
bands have bandwidths that correspond approximately to the critical bands de-
scribed in Section 5.4.1. The technique relies on choosing adaptively the most
appropriate wavelet from a library of wavelets that are smooth3 and compactly
supported. For each frame, this scheme first computes a measure of the distortion
between the coded and the uncoded frame as a function of the wavelet used, and
chooses that wavelet for which this distortion is minimized. Thus the procedure can
be interpreted as choosing an optimal wavelet from the library of wavelets. Good
results have been demonstrated by the authors for several different types of music
signals.




3The notion of smoothness or regularity of wavelets is explained in Chapter 7.
180    Wavelet Transform and Data Compression




      FIgure 5.31 Wavelet packet tree used in the audio coding algorithm by Sinha and Tewflk
                  (1993). The numbers in the figure refer to the lower and the higher cutoff
                  frequencies of each subband.
                         Video Coding Using 人lu川resok片幻n Techniques: A 別ef쎄roduc加n     181

5.5 Video Coding Using Multiresolution Techniques:
    A Brief Introduction
In this section we give a brief overview of some of the wavelet-based techniques
being investigated for the compression of video signals. Wavelet-based methods
are currently being investigated for several low- and very low-bit rate applications
(such as video telephony and video conferencing) as well as for high-definition
television (HDTV) [Kovacevic 1991; Martucci, Sodagar, Chiang, and Zhang 1997;
Rao and Hwang 1996].
   With the evolution of digital television and HDTV, video or image sequence
coding has become a topic of intense research [Kunt 1995a, 1995b; Zhan, Li, and
Lian 1995]. The main motivation for this comes from the fact that these emerging
technologies put a strain on the available communication bandwidth, and the bit
rate needs to be extremely high (on the order of gigabits per second, as pointed out
in Section 5.4) to transmit the required amount of information. Thus, compression
of image sequences assumes great significance. Digitized video can be represented
as consecutive frames in an image sequence and denoted by v(m, n, k) where m
and n are spatial coordinates and k represents the frame index or the temporal
coordinate [Tekaip 19951. Typically, consecutive frames in an image sequence are
highly correlated. Most video coding methods take advantage of this correlation.
These methods fall under the broad heading of interframe coding [Calzone, Chuang,
Divakaran, et a!. 1997; Tekalp 1995].
   The underlying assumption for interframe coding is that image segments in con-
secutive frames are related to those in the adjacent frames by means of simple
operations such as translation, rotation, and scaling [Tekalp 1995; Vetterli and Ko-
vacevic 19951. Consequently, motion compensation is an important component of
most interframe methods. These methods predict the motion in the current frame
based on the previous frames and code the prediction error. Motion compensation
is performed on a block-by-block basis by dividing the images in the sequence into
blocks of equal size or segmenting based on certain criteria [Calzone, Chuang, Di-
vakaran, et a!. 1997]. Often the prediction error is transformed, quantized, coded,
and transmitted. The DCT is most commonly used for this purpose. It has recently
been proposed that the DTWT can be used instead [Martucci, Sodagar, Chiang,
Zhang 1997]. The general system is shown in Figure 5.32.
   Another method is the spatiotemporal pyramid scheme [Uz, Vetterli, and LeGall
19911. This involves two processes: spatial pyramidal coding and temporal down-
sampling. Spatial pyramidal coding involves low-pass filtering a frame and down-
sampling it to give a low-resolution version of the frame. This process is applied
successively. At each step the higher resolution version of the frame is predicted
and the prediction error is coded. Simultaneously, at each level, the temporal image
sequence is downsampled by two.
]82    w아이et 加ns幻rm and D아a Compression




        Figure 5.32 General block diagram of the transform-based motion compensation scheme.


          The key step in this scheme is the interpolation of the intermediate frame using
       the two adjacent frames. The motion in this frame is predicted using these two
       frames. Normally objects in the image are assumed to be rigid and the motion is
       assumed to be translational. Prediction is often carried out in a blockwise manner
      using the low-resolution versions of the frames. The solution is refined successively
       for higher resolution until full resolution is reached. This method is computationally
      less complex and also more robust.
          A generalization of the separable two-dimensional DTWT to three dimensions is
      often used for isotropic data such as multispectral images or tomographic images.
      For video, too, this strategy can be used. Methods based on both separable [Vetterli
      and Kovacevic 1995] and nonseparable filters EKovacevic 1991; Vetterli and Kovace-
      vic 1995] have been proposed. For the separable case, very short filters need to
      be used for temporal filtering to prevent blurring of motions in the low-frequency
      bands and to prevent creating high-frequency artifacts in the high-pass band. Nor-
      mally the DTWT is taken over four to six frames. Vetterli and Kovacevic [1995] note
      that although the low-pass-filtered subband is similar to the original, the only other
      subband with substantial energy is the one that has been subjected to high-pass
      temporal filtering followed by low-pass filtering in the spatial dimensions. This
      channel contains energy whenever there is substantial motion, and it can be used
      as a motion indicator [Vetterli and Kovacevic 1995].
                            CHAPTER SIX


            Other Applications of
             Wavelet Transforms


6. 1 Introduction
As seen in Chapter 5, the wavelet transform of real-world signals tends to create
low-value coefficients at the finer scales. This property makes it possible to devise
compression schemes that quantize the fine-scale coefficients more severely than co-
efficients at other scales. Let us now examine some other applications of the wavelet
transform that exploit its properties, such as correlation parameterized by position
and dilation, the multiresolution nature, and the orthogonality or biorthogonality of
its basis functions. Several of these applications are at an exploratory stage at this
time and, because many of them rely on heuristic approaches, quantitative results
are not always available.


6.2 Wavelet Denoising
There have been several investigations into additive noise suppression in signals
and images using wavelet transforms. The principal work is that of Johnstone and
Donoho [Donoho 1992; Donoho and Johnstone 19921, which is based on threshold-
ing the DWT of an image and then reconstructing it. The method relies on the fact
that noise commonly manifests itself as fine-grained structure in the image, and
the wavelet transform provides a scale-based decomposition. Thus, most of the
noise tends to be represented by wavelet coefficients at the finer scales. Discarding
these coefficients would result in a natural filtering out of the noise on the basis of
scale. Because the coefficients at such scales also tend to be the primary carriers
of edge information, the method of Donoho and Johnstone 119921 thresholds the
wavelet coefficients to zero if their values are below a threshold. These coefficients
are mostly those corresponding to noise. The edge-related coefficients, on the other
hand, are usually above the threshold. An alternative to such hard thresholding is
soft thresholding, which leads to less severe distortion of the object of interest. Sev-
eral approaches have been suggested for setting the threshold for each band of the

                                         183
184   0ther A尸p仄二a加ns of너／ave旭t Trc가）S幻rn省

       wavelet decomposition. A common approach is to compute the sample variance a2
       of the coefficients in a band and set the threshold to some multiple of the standard
       deviation a. Thus, if we want a soft threshold of the DTWT coefficients for a partic-
       ular wavelet band, we would threshold the coefficients of that band as in Figure 6.1.
          The inverse wavelet transform of the thresholded transform coefficients is the
       denoised image. It has been found that such denoising is effective in that although
       the noise is suppressed, edge features are retained without much damage. We
      provide two examples of denoising.
          The first example uses a one-dimensional signal. Consider the signal in Figure 6.2.
      The signal shows a sharp discontinuity or edge about which its magnitude falls
      off exponentially in either direction. We now add noise to the signal. Figure 6.3
      shows the result of adding white Gaussian noise of variance 0.1 to the signal. Let
      us first attempt a reconstruction using a method that does not rely on wavelets.
      In particular, let us try the FF1' approach. The FF1     ' magnitude of the original
      signal is shown in Figure 6.4A, whereas that of the noise-added signal is shown in
      Figure 6.4B. The central "noisy" part of Figure 6.4B is referred to as the noise floor
      in some areas of signal analysis. One approach to denoising is to replace the noise
      floor in the FF1 ' with zero values and then take the inverse FF1
                                                                      '. The block diagram
      for this approach is shown in Figure 6.5. Such an approach involves the setting of
      a threshold so that only values above the threshold are retained and the rest are



                                                   Output coefficient




                                                            an          Input coefficient




             Figure 6.1 Soft threshold characteristics.
        Wave/et Denoising   185




:   1
186   Other A尸尸lications （少 Wave/et 加ns幻rms




             F勾ure 6.4 FF1 magnftude of (/\) 引gn（긔 and (B) 틔gn데 F이us noisE느



      the coefficients with values less than 8 are in the noise floor, and all values greater
      than 8 correspond to coefficients of the FFT of the original signal with high values
      for the magnitude (see Figure 6.4A). Therefore, we set the threshold to 8. The result
                                                                           Wavelet Deno/sing   187



         Signal + Noise -3rn-   FFT
                                         升L
                                                 H
                                         Threshold
                                                         1마     如毗d           Signal



      Figure 6.5 Block diagram for the FF1-based denoising scheme. 1FF1 = inverse FF1,



of applying the threshold to the FFT magnitude is seen in Figure 6.6B. The inverse
FFT of the signal is shown in Figure 6.7. Although the zeroing out of the noise floor
has reduced the noise, it is seen that because part of the signal FF1 ' is unavoidably
removed as well, the edge is not as sharp in the reconstruction as it was in the
original. It is blurred. There is also an attendant ringing to the reconstruction.
The FFF-based method just described is essentially a low-pass filtering technique.
Underlying the application of the technique is the supposition that in the frequency
domain, the signal occupies a definite portion of the spectrum, most of the noise is
outside this range of frequencies, and therefore removal of noise over a wide range
of frequencies results in a denoised signal.
    A drawback of the FF1   ' is the fact that the edge information is spread across
frequencies because of the basis functions not being localized in time or space, and
hence the low-pass filtering results in the smearing of the edge. Let us next illustrate
how the localized nature of wavelet basis functions results in denoising with edge
preservation.
    The result of a three-level decomposition of the original signal with Haar filters
is shown in Figure 6.8. The outputs of the HPFs have high values at samples cor-
responding to the location of the edge. The leftward movement of the peaks as
we go from the level one HPF to the level three HPF is due to the factor of two
downsampling at each stage. The compact nature of the DTWT basis functions
as opposed to the expansive nature of the sinusoidal basis functions of the FF1'
results in the localization of the edge information in the DTWT. Figure 6.9 shows
the three-level decomposition of the noise-contaminated signal in Figure 6.3. As is
to be expected, the decomposition appears noisy. However, the peaks in the HPF
outputs are well preserved. Let us set thresholds for each HPF output using its
standard deviation. The computed standard deviations for levels one through three
are 0.12, 0.052, and 0.05 respectively. Figure 6.10A shows the result of the recon-
struction after hard thresholding of the high-pass outputs with the threshold at each
level set to the output's standard deviation. Figure 6.IOB shows the reconstruction
with the thresholds twice as high as in Figure 6.IOA. The edge preservation is quite
apparent. However, notice the jaggedness of the reconstruction elsewhere. This is
due to the discontinuous nature of the Haar basis functions of the DTWT. Also, there
is some residual noise. The higher the threshold, the lower the residual noise. How-
ever, noise removal is always accompanied by some degradation in the underlying
188    OtherA尸f川C아ion＄可以刃e旭t刀ans幻rrr巧



                    80



                   61)



                   40



                   20




                                         4          6         8         10            12
                                              FFT magnitude
                                                   (A)


                    I ()
                                                                                 IT
                     K         .




                     6


                     4


                     )     ,




                     0
                                   50        10          15       20            25
                                                                       FFT index -+
                                                   (B)


              Fig바e6.6 (A) H酎ogram （少 FF1 magnitude of sign이 1긔us n（긔S包 (B) FF1
                       ma아咐ude after thresh（긔ding.



      signal, and increasing the threshold results in more of the signal component being
      zeroed out along with the noise. Soft thresholding minimizes the contribution of
      the residual noise to some extent by reducing the amplitude of the residual noise in
      the thresholded HPF outputs. Figure 6.11 shows a soft-thresholded reconstruction
      effected using the thresholds in Figure 6.IOB. The result is a smoother reconstruction.
         The smoothness of the reconstruction is affected by the smoothness of the ba-
      sis functions. This is brought out in Figure 6.12 where D4 filters, which lead to a
                              Speckle Removal   189




                 /\
0.   1

     0
         \/\n\in/\1,/
         '   l        .   I   ．」
]90   C가herA尸口／ications of Wavelet 加n計orms


                   0
           H
                -  1 0.
                                    m




                -0.2                n




                -0.3                1




                -0.4                m




                -0.5                e




                -0.6                m




                -0.7                m




                -0.8                m




                -0.9                느




                   l                                                                          (A)
                                        20       40       60   80   100      120


                 0.05
                                             7        \
                                                                                n   -+
                    0
               -0.05                1




                -0.1                m




               -0.15                H




                -0.2                m




               -0.25                e




                -0.3                m




               -0.35                1




                -0.4
                                                                                              （助
                                    1




                                        20       40       60   80   100      120
                                                                               n+
                    0. 1
                          0   H7\        '




                -   0.    1
                -0.2
                -0.3
                -0.4
                -0.5
                -0.6                                                                          (C)
                                        20       40       60   80   100      120
                                                                               n=        =+




                 0.5
                 0.4
                 0.3
                 0.2
                 0. 1
                   0
                -0.1
                -0.2
                -0.3
                -0.4                                                                          (D)
                                        20       40       60   80   100       120
                                                                                n +




          디gure 6.8 Three-Iev이 decom口O引tion of 炚）n이 U덟ng H（그（그1W（그velet. (A) Out口U十 C寸
                    竹st-Iev이 HPF. (B) O먀口ut of second-Iev터 HPF. (C) Output of third너evel
                    HPF. (D) O마put of 卄ir(：卞1ev터 LPF.
                                                                               Speckle Removal         191




        -0.2
                   0
                       VM싸／
                          1
                               抑YV
        -0.4

              n <




                                        1
        -0.
              -8   1                                                                     (A)
                          20     40         60         80         100        120
                                                                               n-   +.
         0.1


                         h
        0.05
           0
       -0.05
        -0.1
       -0.15
        -0.2
       -0.25
        -0.3
       -0.35
        -0.4
                                                                                         （固
                          20     40         60         80         100        l 20
                                                                               n+




    Figure 6.9 가ree나e\／쉬 decom口osition of 引gn（계 1：긔us ri이se 岫ng Hoar w（그＼     ,elet.
               (A) Output of first-level HPF, (B) Output of second-level HPF.


because of constructive and destructive superposition of reflected components with
differing phase delays. A digital image of a speckled object is usually peppered
with bright and dark spots, as shown in Figure 6.14A. A multiplicative model for
speckle was proposed by Goodman [Dainty 19841. The model holds for digitized
speckle images that are sampled far enough apart such that the speckle degradation
at a pixel is independent of the degradation at other pixels. Thus

                                I (m, n) = O(m, n)S(m, n).                                     (6.1)

Taking the logarithm, we have

                               I (m, n) = O(m, n) +S(m,n)                                      (6.2)

where the tildes indicate the logarithms of the quantities in Equation 6.1. As shown
by Arsenault and April [1976], the log-speckle S(m, n) is Gaussian when the image
intensity is integrated by a finite aperture. Thus the framework in Equation 6.2 is
192   （가her App//ca加ns可w아이et加n計am咨



                      0   UV띠小 '
             -   0.   1
             -0.2

             -0.3
             -0.4
             -0.5         -   1     ,




                                                                                  (C )
                                    20   40   60       80        100       120
                                                                            n+




              0.5
              0.4
              0.3
              0.2




                          fl
              0.1
                0
             -0.1              m.    ,
             -0.2
             -0.3
             -0.4                                                                 (D)
                                    20   40   60        80       100       120
                                                                             n+



          디gure 6.9 (c口川hued) (C) O마p먀 아 third-lev이 HPF. (D) Output of third-Iev이 LPF.



      identical to the additive noise removal problem considered in Section 6.2, with the
      log-speckle playing the role of additive noise.
         Guo and colleagues [19941 propose application of the DTWT-based denoising
      to the log-transformed image. The steps involved are finding the DTWT of the
      log image, applying thresholds as in the previously described denoising example,
      computing the inverse wavelet transform, and applying the inverse logarithm. The
      inverse logarithm is simply an exponentiation. The block diagram of a despeckling
      system is shown in Figure 6.15. The despeckled image is shown in Figure 6.14B.


      6.4 Edge Detection and Object Isolation
      The edge-preserved denoising described in Section 6.2 lends itself to a wavelet-
      based procedure for edge detection. We observed in Figure 6.8 that the edge in the
      signal gave rise to peaks in the HPF outputs or the detail subbands at concordant
      locations. This is characteristic of the DTWT. In other words, edges give rise to
                                                           Edge Det配加n and C洵ec시S이（카幻n     193




                   l
               0.8
               0.6
               0.4




                                                     나
               0.2


              -0.2
                   0 A八나J
                           山                   f/J
                                                            나I
                                                                       나小니
              -0.4
              -0.6


                                         1
              -0.8

                                                                                     (A)
                             50          100         150         200         250
                                                                           n+




               0.8
               0.6
               0.4
               0.2
                   0 11JH＝ 入H=H
              -0.2
              -0.4
              -0.6
              -0.8
               小   l
                             50
                                         ]
                                         100
                                                      .


                                                     150
                                                                  ,


                                                                 200        250
                                                                                ,-   （助
                                                                           n- 片



        Figure 6.10 Denoised reconstruction with Hoar filters. (A) Thresholds set to
                    stand（그rd de너（그tions of HPF outpu十s. (B) Thresh이ds se十 to twice
                    the 計and（그rd de너ations of HPF ou十Pu十S.



peaks across several levels of detail at coordinate values that move to the left by a
factor of one half at every transition from a finer scale to a coarser scale. Also, the
stronger the edge (that is, the steeper the edge slope), the higher the peaks in the
DTWT. Consequently, an edge can be found from the wavelet transform by iden-
tifying peaks at concordant locations [Mallat and Hwang 1992]. The requirement
194   OtherAp;川cc豺ions of너/C刃이et Tran計am省




                     0.6

                     0.4

                     0.2                             -   .1




                       0 :J=Jm           \                    그＼九nJ1그JU
                    -0.2

                    -0.4

                    -0.6

                    -0.8
                                   50
                                               1
                                               100            150      200         250


              Figure 6.11 Denoised reconstruction with Haar filters. Thresholds set to twice
                          the st（그ndard de＼기（a枷＞ns of HPF outF乂片S. 鈿ft threshc永계ng has
                          been employed.



      of concordance is useful in discounting spurious noise-induced peaks that might
      show up in individual subbands. Let us now apply this method to edge detection
      in the one-dimensional object in Figure 6.3. The detail subbands of this object in
      Figure 6.9 show strong peaks at samples (indices along the horizontal axis) 50, 25,
      and 12 at levels one, two, and three respectively. Let us regard these as concordant
      locations, since 12 is one of two nearest integers to 25/2. To illustrate the edge
      detection graphically, we zero out the HPF outputs except at these three locations,
      where we set the values to -1, consistent with the negative orientation of the peaks.
      The LPF output at level three is zeroed out as well. The HPF and LPF outputs are
      then provided as inputs to a three-level reconstruction filter bank. The correspond-
      ing reconstruction superimposed on the noisy signal is shown in Figure 6.16. As
      we see, the reproduced edge coincides with the edge in the noisy signal.
         Object isolation or segmentation in an image is the grouping of its pixels into
      several disjointed sets on the basis of certain criteria. The process is useful for
      automatic detection and classification of objects in an image. The sensitivity of the
      wavelet transform to the scale of an object or parts of an object can be exploited for
      object isolation. For example, consider the image "Adel" in Figure 6.17A. This image
      was taken using an infrared camera in the context of detecting weapons concealed
      under a person's clothing. The scene is of a person with a concealed handgun
      under moderately heavy clothing. A three-level DTWT of the mean subtracted
      input image was obtained and is shown in Figure 6.17B. The LPF is the Daubechies
      four-tap FIR filter. It shows that the noise and several objects that clutter the scene
      such as the subject's limbs, name tag, and so forth, tend to be isolated in the outer
                                                           Ec勺eD計ec加n and（殉ect／自에on             195




              0.8
              0.6
              0.4
              0.2
                0
             -0.2
             -0.4
             -0.6
             -0.8

                                                                                          (A)
                             50          100         150        200            250
                                                                           n   m+
               0.6

               0.4

               0.2

                0

             -0.2

             -0.4

             -0.6

             -0.8
                                                                                          (B)
                             50          100        150         200            250
                                                                           n        -+-
        Figure 6.12 Denoised reconstruction with D4 filters. Thresholds set to twice
                    the standard de＼기ations of HPF out口uts. (A) 나가d 十hresh이네ng.
                    (B) 鈿什 threshok加g.


or first two levels of detail. Consequently, several other objects stand highlighted
in the low-resolution approximation. In other words, there is increased contrast in
the residual after stripping away noise and fine detail.
   기hresholding an image on the basis of partitioning its histogram into two distri-
butions is a common technique for object isolation. Typically the threshold is set at
a valley or valleys in the histogram. For the image in Figure 6.17A, the histogram
196   （가her Ap川Ca加ns of 너／ave/ct ／仄7nsforms




                                                （그sed im（그ge denoising. (A) C川이n이 irn（그ge.
            Figure 6.13 An exam이e of 낚／（그＼,elet士）
                        (B) 什s two냐ev쉬 D찌VT.
                                               Edge Detection and Object Isolation   197




                                              難
                                              燕口
                                  姓照器瑟畔                         轟煎璘懈蔑蘿撰籌m

F勾바e6.13 (con卄nued) (C) Recons卄uc쉬on （그f十er h（그rd thresh이ding. (D) Edge
         ex卄（水二卄on from origin이 image.
198   C가herA口尸／/（그가／ons of 너／eyelet 加仍幻r기＄




             Figure 6.13 (continued) (E) Edge extraction from denoised image.



      shows a single valley, as shown in Figure 6.17C. Thresholding the image on the
      basis of this valley yields the image in Figure 6.17D. The DT사T in conjunction with
      scale filtering can be used to accentuate partitions in the histogram. In fact, the
      object isolation problem in this example is related to the edge detection discussed
      in Section 6.2. The role of the edges is that of something that confounds the task
      rather than helping, because the relevant object (namely, the concealed weapon)
      possesses an infrared imprint that has a boundary that is diffuse rather than sharp.
      The edges are associated with other objects. This is brought out by the image in
      Figure 6.17E, which is the Lap1acian1 of ADEL. There is no trace of the weapon
      itself. Since most of the DTWT pixels have gray values close to zero, we regard
      those with nonzero values as being indicative of significant activity in the image.
      As seen in edge detection using DTWT, prominent values in the detail subbands
      correspond to sharp edges. Therefore, rather than setting a single threshold and re-
      tam1ling only DT人／T pixels with magnitudes greater than this threshold (as was done
      for edge detection), a reconstruction that retains pixels with values over a smaller
      range has a better chance of reconstructing the object. A histogram of the DTWT
      away from the peak at zero reveals several valleys for the image. Setting thresholds


      lThe Laplacian of I (x, y) is defined as 821/8尸 + 021/8y2. It is one operation, among others, that is used
      to highlight edges.
                                             Edge Detect幻n and 아羽C치S이a加n   199




Figure 6.14 (A) Speckled image. (B) Despeckled image. From (Guo 1994)
            匣）1994 IEEE.
200   OtherA尸口／ications C寸 Wavelet 了ran＄幻r,기S


                                log(signal) + Iog(noise)




        Speckled Signal *
                            -

                                   mg     냐
                                           1         DWT Denoising   H+   1

                                                                              log니
                                                                                     -




                                                                                         Despeckled Signal




      Figure 6.15 A DTWT-based despeckling scheme




                Figi玎e 6.16 Reconstructed edge su口erirr）口osed on origin（긔 n이sy 引gn（乂


      at two of the valleys (- 2.1 and 0.5 in this case) and computing the inverse wavelet
      transform of the portion in between reveals the concealed object, as shown in Fig-
      ure 6.17F. Superimposing a level slice of the object on the original yields the image
      in Figure 6.17G.


      6.5 Image Fusion
      Information about events in time or location of objects in space is often obtained
      using multiple sensors. For example, if we were to image a scene with a record-
      ing device at just one location, it would be impossible to obtain depth information.
      However, with two images taken with the recording device (or two devices) sit-
      uated at offset locations, it is possible to gauge depth using a process known as
                                                                         Image Fusion   201




 Figure 6.17 (A) Infrared image of person with concealed weapon.



stereogr刃7imetry. In fact, stereogrammetry of information from both eyes is the prin-
cipal cue to our perception of depth. The process of combining data from multiple
sensors to obtain a better understanding of the data source is called data fusion.
Stereogrammetry is just one example.
   Suppose we have two images of an object imaged by different means. For ex-
ample, we could use two different sensors-one operating in the visible spectrum
and the other operating in the infrared spectrum. The two images are bound to
differ in what they highlight. Unlike the visible-range sensor, the infrared sensor
essentially generates a thermal profile of the scene. The aim of fusion would be
to generate an image that captures the salient features of both. The ability of the
wavelet transform to localize information as a function of space and scale comes
in handy in fusing information from the two images. The methods proposed for
effecting fusion using the DTWT take the following form:

    1The two images are first normalized so that they contain the same amount of
     energy and hence can be compared fairly.
202   O加아A尸尸／ica卄ons of Way이et Transforms




      Figure 6.17 (continued) (B) Three-level D1WF of the image. (C) Histogram of the image in A.
                                                                       Image Fusion   203




        Figure 6.17 (continued)(D) Thresholded image




    1The images are wavelet transformed using the same wavelet, and transformed
     to the same number of levels.

   . In each subband,individual pixels or groups of pixels of the wavelet transform
     of the two images are compared using some criterion that serves as a measure
     of activity at that particular scale and space. Examples of such measures are
     absolute values of pixel gray values, maximum absolute gray value of the
     group of pixels being compared, and the variance.

   . A fused wavelet transform is created by taking pixels from that wavelet trans-
     form that shows greater activity at the pixel locations.

   . The inverse wavelet transform is the fused image.


   An example of wavelet-based image fusion of a magnetic resonance imaging
(MRI) image of a section of the brain with one taken from a positron emission
tomography (PET) scan [Li, Manjunath, and Mitra 1994, 19951 is shown in Fig-
ure 6.18. Li, Manjunath, and Mitra [1995] reported that wavelet transform-based
fusion worked better than the other techniques against which it was tested.
204    아her App北아ions 可 Wavelet Transforms




            Figure 6.17 (continued) (E) Laplacian of the image


      6.6 Object Detection by Wavelet Transforms
          of Projections
      Suppose we have a finite energy signal f (t) and an observation g(t) of it in a dilated
      and shifted form



                                      g
                                      ?（
                                           (t)
                                                 『）
                                                      ：
                                                      _
                                                          士
                                                          ,,,   f
                                                                    (t_
                                                                          a。
                                                                              ,bo\
                                                                                     /                            (6.3)


      If it is required to determine a0 and b0 from g(t), we could correlate g(t) with all
      possible dilated and shifted versions of f (t), and pick those values of the dilation
      and shift for which the correlation is a maximum. The basis for this procedure is
      provided by the Cauchy-Schwartz inequality [Chapa 19951:


                 / . . . I , (t_ b\ \ 2                                   I          ft 尸 b"\ 2
                 \gUJ1 戶J ( 1HH 11 5 ng (r）下
                 \       vu \ a / /                                       7訂（;U/                  = 11f (t)1i4.   (6.4)
                                       O可a升 O아叱加n by Wavelet Tran加rms O叩呵ec加ns               205




 Figure 6.17 (continued) (F) Reconstruction after thresholding the DTWT. The object in the
             middle is the concealed handgun.



We have used the fact that IIg(t)II = IIf (t)II and Il f (냥))II = IIf (t)II. The maxi-
mum value of the left-hand side or equality in Equation 6.4 is attained only for a = a0
and b = bo. Since the wavelet transform is correlation parameterized by shift and di-
lation, we can use the wavelet transform. If the signal f (t) is not a wavelet itself, we
might then choose a wavelet 砂 (t), which is close to or matches 1 (t). As described
in Chapter 7, there are procedures for generating wavelets to match a specified
function, and wavelets so generated can be used. The scale and time coordinates
of the peak value in the CWT of g (t) are the estimates of a0 and b0 respectively.
    The wavelet transform-based correlation procedure can be extended to automatic
detection of objects in images. If the presence of a specific object is to be detected, a
training procedure is first performed with the object using projections onto straight
lines. The projection of an object 0 (x, y) onto a straight line is obtained by inte-
grating 0 (x, y) along the normal to the straight line. Consequently, the projection
is a one-dimensional function. In the training phase, the projections of the object
onto straight lines at various angles are obtained using a clean image. Matching
206   C가her A／刃片cations of Wavelet 加席幻rn百




       Figure 6.17 (continued) (G) Superimposition of a level slice on the original image.



      wavelets are generated for each projection. It has been found with most objects that
      the matching method described later in Section 7요3 yields the same wavelet for all
      projections. The only difference as a function of the projection is the scale or width
      of the matching wavelet. A vector of these widths is formed. This vector, called the
      reference scale vector, has the property of yielding a circular shift on rotation of the
      object through an integer multiple of the angular resolution of the projections. Also,
      a zooming or scaling of the object produces a corresponding scaling of the vector.
      To see how this can happen, consider the example of a rectangle of which we take
      only two projections, as shown in Figure 6.19. The projection on the horizontal axis
      has length a, whereas that on the vertical axis has length b. A wavelet dilated to fit
      these projections best would have dilation or scale factors that are proportional to
      a and b respectively, say Wa and Wb. The reference scale vector is [W口, Wbl. Suppose
      we rotate the rectangle by 90 degrees. The maxima of the wavelet transforms of the
      horizontal and vertical projections now have scale coordinates that form the vector
      [Wb, wa]1a circular shift of one of the reference scale vectors. If we were to zoom
      the rectangle by a factor of a, the scale vector now becomes [a Wa, a Wb]. Similar
      properties hold for scale vectors formed from multiple projections.
                                         O히ect D計ec加n by Wave旭t Tran加肋如叩回ec加ns                      207




Figure 6.18 Image fusion using the DTWT. (Le什 to right) MRI image, PET image, and fused
            image. D1사Fs of each of these images is displayed below them. From (Li 1994)
            匣）1994 IEEE.


   Consequently, after training, the detection of the object in a test image is per-
formed by projecting the image onto straight lines and wavelet transforming each
projection with the matched wavelet. A vector of scales is extracted from the wavelet
transforms by locating the peak position in scale. A comparison with the reference
scale vector yields the rotation and scaling for a best fit.
Example 6.1
      Wavelet transformation using matched wavelets was used with one-dimensional pro-
      jections of a two-dimensional object to provide object detection along with position,
      orientation, and size information [Chapa 1995; Chapa and Raghuveer 1995, 1996b].
      Figure 6.20 shows the test object (image of an airplane). In the training phase, eight
      projections onto straight lines at angles of 0 degrees through 157.5 degrees in steps of
      22.5 degrees were obtained. The wavelet matching algorithm was run on each of these
      projections. Figure 6.21 shows the projections and the matched wavelets. Observe that
      the matched wavelet is the same for each projection. However, the scale of the wavelet
      that best fits the projection does depend on the projection, and provides a measure of
      the "width" of the object as seen in this direction. The eight-dimensional vector of these
      best scales after normalization by the maximum value is used to estimate the size and
      orientation of the object. A rotation of the object causes this vector to shift circularly,
      whereas a zooming simply changes the normalization factor. Figure 6.22 shows the
208    Other Ap冽Ca加ns可Way이et加ns幻rms




           Figure 6.19 Illustration of reference scale vector formation.


            object with an oval superimposed on top of it. This oval was generated by taking the
           DTWT of each projection, locating the peak, thresholding the DTWT to retain the peak
            and to zero out other values, reconstructing the projection, backprojecting all recon-
            structed projections, and thresholding the result. The backprojection of each reconstruc-
           lion here is done simply by creating a swath along the projection direction, with every
            cross-section of the swath being the one-dimensional reconstruction of the projection.
           These backprojections intersect in the area where the object is located. The orientation
           and size of the oval coincides with the object. Figure 6.23 shows a rotated, shifted, and
           zoomed (1.5 times) version of the same object in white noise (SNR, 2.1 dB) along with
           the backprojection of the thresholded wavelet transforms. The oval from this backpro-
           jection shows a new orientation, size, and position consistent with that of the test object.
           This provides a visual portrayal of the ability of the feature vector described to provide
           information regarding location, orientation, and size of the object. The fundamental
           advantage of using wavelets in such an application is in the fact that they adapt natur-
           ally幻曲ations, a命there的re they are付旬suited f아zoo'帥variant丘oce輛g. 1


      6.7 Communication Applications
      6.7.1 Scaling Functions as Signaling Pulses
      The fact that wavelets can be used to construct orthogonal basis functions for signal
      spaces and subspaces can be taken advantage of in the transmission of data over
      channels. In digital communication, a stream of information symbols is modulated
                                                           C（가rmun／的加n Ap冽Ca加ns          209




        FIgure 6.20 Tes十 image c寸 an 이rr이one.


onto a waveform for such transmission. Let us use baseband pulse amplitude
modulation to describe the process. We wifi see that wavelet theory (in particular,
Meyer scaling functions) fits naturally.
   Suppose we have a source of binary symbols 0 and 1. Suppose we group k of
these bits at a time to form a new "symbol." There are M = 2" such symbols. Each
such symbol is mapped to a number. Let am, m = 1, .. . , M be these numbers, called
symbol amplitude. Usually these values are spaced uniformly and symmetrically
about 0. Suppose the binary source has a bit rate of 1/ Tb (that is, the binary digits
arrive Tb seconds apart). The symbol interval T = k Tb seconds. The data are
transmitted over an analog channel by amplitude modulating a transmit pulse p(t)
by the symbol amplitude. Thus, given the symbol stream, the transmit waveform
takes the form

                                s(t) = >二dkp(t - kT)                             (6.5)
                                        k

where dk is one of {al. .. . .aM}. This waveform is transmitted over a channel that
is usually modeled as a linear, time-invariant (LTI) system. Suppose we model the
210    OTherA尸p北아ions 可w刃的사回衿幻rms




      Figure 6.21 Dilated projections and their associated matched wavelets.


      channel as having the frequency response

                                      ,,. .   11     1口기 <2兀w
                                      '-（띠J = l 0                                  (6.6)
                                                     otherwise.

      The channel is said to be bandlimited to W Hz. Let c(t) be the impulse response of
      the channel and let

                                          力（t) = p(t) 半c(t)                        (6.7)
      where * denotes convolution. Then the received signal is

                                       r(t) = > dkh(t - kT).                       (6.8)
                                               k
      At the receiver we have to recover the sequence dk from r(t) and then map each
      recovered symbol to k bits. The signal r(t) is sampled every T seconds for this
      purpose.
                                                                          Comi加川ca加n Ap히吼片幻ns    211




        Figure 6.22 The airplane image with an oval generated by the
                    backprojection of the thresholded wavelet transform.


  Suppose we look at the sample of r(t) taken at time instant t = mT:

                              r   (mT)   =   ＞二dk力
                                              k
                                                 （(m    寸   k)   T)   .
                                                                                         (6.9)


Expanding Equation 6.9,

                          r(mT) = dmh(O) +＞二 dm_kh(kT).                                 (6.10)
                                                  k尹m


Ideally we would like to have r(mT) = dm. This would require

                                             h(0) =1                                    (6.11)

and the second term ＞二k尹m dm_kh(kT) (called the intersymbol interference fIST]), to
be identically zero. It is possible to have zero ISI if

                                             h(kT) =O                                   (6.12)
212    Other Appilca加ns可Wavelet了仄7ns幻rms




              F勾마e 6.23 Rotc그ted, 計iifted, and zoomed airF이（그ne image in wh汁e noise
                        along with the backprojection of the thresholded wavelet
                        transform.


      for k 尹 0. Thus the condition for no ISI can be summarized as choosing p(t) such
      that

                                                 h(kT) = 6(k).                        (6.13)

      Let H(w) be the Fourier transform of h(t). Then, Fourier transforming Equation 6.13,
      we get the frequency domain equivalent


                                      于
                                     , 1日
                                     尺＝r-   QQ
                                                 H
                                                     (m+
                                                     \
                                                           \
                                                               2兀k "
                                                               T
                                                                   /
                                                                       /
                                                                           =   T      (6.14)


      which is identical to the Poisson summation condition we have seen before in the
      context of orthogonal bases. Let

                                                   I    /W\
                                            G(m) = 1/ / 1 = 1 .                       (6.15)
                                                   T    \T!
                                                           Cot川1끼nic아ion Ap尸在Ca加ns       213


Then
                                 的

                                ＞二 G(w+ 2兀丸）=1.                                 (6.16)
                                k=-oo



Thus if G(co) is equal to 呻(w) 2 or 凹(w)12 for some scaling function 中(t) or wavelet
砂(t) yielding orthonormal translates, then the condition for no 1ST is satisfied natu-
rally.
   Let us delve a little further into the choices we have for h(t), and hence p(t).
The fact that C(w) is bandlimited to W Hz forces the same bandlimiting on H(w)
because it is the product of P(w)-the Fourier transform of p(t)-and C(w). The
function G(w) is bandlimited to WT Hz. Thus, in addition to Equation 6.16, we
have the condition that G(w) be zero for wi > 2兀 WT. This implies that if

                               2兀 WT < 27了 -2兀 WT                               (6.17)


or, equivalently,

                                        1/ T> 2W                                (6.18)

then the condition of Equation 6.16 cannot be satisfied and there will be ISI. This
translates to the statement that for no 1ST a necessary condition is that the symbol
transmission rate be less than twice the channel bandwidth. Suppose we do have
1/ T <2 W. Let

                                  八w= 2ir WT- ,r.                               (6.19)

To satisfy the condition of Equation 6.16 we require

                                        G(w) =1                                 (6.20)

幻r k끼 드 7T 十 Aw. In the range 7r - Lw <w 5 7r + Aw we require

                               G(w) + G(2兀 - cv) =1.                            (6.21)

Letting G(w) be symmetric about the origin, this condition becomes very similar
to the condition we had for constructing Meyer scaling functions in Chapter 3. In
fact, if 스w 드 兀/3, the condition in Equation 6.21 is identical to the condition of the
squared magnitude of the Fourier transform of the Meyer scaling function, which
suggests that P(w) be a suitably dilated squared magnitude of a Meyer scaling
function Fourier transform. In practice, rather than having a pulse waveform at the
214    OtherAr冽加月ons of Wavelef刀an加rms

       transmit end only, as in Equation 6.5, it is preferable to have transmit and receive
       pulses-PT (t) and PR (t) respectively-so that the transmit waveform becomes

                                            s(t) = ＞二 dkpT(t - kT)                                     (6.22)
                                                      k

       and the received waveform has the same expression as in Equation 6.8, with

                                          h(t) = 勿 （t) 木 c(t) 水 抑 (t).                                 (6.23)

      Now, to make h(t) obey the no ISI requirement, we can make 勿(t) and pR(t)
      the same Meyer scaling function if 八w 5 jr/3 (that is, if 1.5 W 드 lIT < 2 W).
      For further reading on this topic and its generalization to other cases, see Gandhi
      [1995a, 1995b1; Gandhi, Rao, and Pappu [19941; Jones [19941; Jones and Dill [1998a,
      1998b]; and Raghuveer [19951.


      6.7.2 Discrete Wavelet Multitone Modulation
       Multicarrier modulation (MCM)2, also known as discrete multitone transmission
       (DMT) or orthogonal frequency division multiplexing (OFDM), involves the use
       of several carriers and an associated partition of the given channel into narrower
      bands or subchannels. This arrangement allows efficient utilization of the channel
       especially when the channel's power spectrum is unevenly distributed [Akansu,
      Duhamel, Lin, and de Courville 19981. MCM allows subchannels with better power
      levels to be treated more favorably than others. Optimal modulation and coding
      techniques can be used independently for each subchannel to ensure efficient use
      of the fullband channel capacity.
          The general block diagrams of an M-channel MCM transmitter and receiver sys-
      tems are shown in Figures 6.24A and 6.24B respectively. At the transmitter end, the
      input is assumed to be in time-division multiplexed (TDM) form. This means that
      the input data stream is made up of symbols originating from different sources that
      are interleaved to form a composite data stream [Proakis and Salehi 19941. This data
      stream is then passed through a serial-to-parallel converter. The serial-to-parallel
      converter distributes the symbols constituting the data stream one after another to
      M subchannels. Thus, the data rate at the input of each subchannel is 1/M times
      the overall input data rate. The inputs to the M channels now modulate bandpass
      carriers, fj (n), n = 0, 1. . . . .M - 1, of each of the channels. Each carrier occupies
      a different center frequency and pass band in the frequency domain. These carri-
      ers are typically bandpass pulses and are often chosen to be the basis functions of
      orthogonal transforms such as the DFT or the DT사T [Akansu, Duhamel, Lin, and


      2 Some familiarity with communication systems is assumed on the part of the reader for this subsection.
                                                            Communical幻nA／갸川cations       215

de Courville 1998; Bingham 1990]. The M subchannels are then combined to form
a composite signal that is passed through a digital-to-analog converter and trans-
mitted. The formation of the composite sequence is known as frequency division
multiplexing (FDM) [Proakis and Salehi 1994]. In this manner, a DMT transmitter
converts a TDM signal into a FDM signal, and hence, can be looked upon as a
transmultiplexer system [Akansu, Duhamel, Lin, and de Courville 19981.
     At the receiver end, the transmitted signal is first recovered and then passed
through a demodulator. The demodulator recovers the M subchannels using the
inverse of the orthogonal transform used at the transmitter. This is represented by
the functions fi (n), n = 0, 1, . .., M-1 in Figure 6.24. The recovered subchannels are
passed through a parallel-to-serial converter to give the original TDM data stream.
     Several transforms have been proposed for MCM systems. The most popular
one is the DFT. In this case the carrier for each channel consists of a rectangular
pulse modulated by a sinusoid whose frequency corresponds to the center fre-
quency of that subchannel [Sandberg and Tzannes 1995]. The disadvantage of this
method is that there is considerable spectral overlap between adjacent subchannels.
Consequently, the 1ST introduced during transmission is severe. An equalizing or
predetection filter is employed at the receiver end to minimize the 1ST.
     Discrete wavelet multitone modulation (D사MT) has recently been proposed as
an alternative to the DFF-based DMT system. Here, the data streams modulate the
filters of an M-channel orthogonal synthesis filter bank. The M-channel filter bank
is a generalization of the 2-channel filter bank discussed in Chapter 3 [Vaidyanathan
19921. These filters can be designed to minimize spectral overlap between adjacent
channels. Note that this minimization leads to longer filters in the sense of having
longer impulse responses. Thus the current output of the transmitter depends on
several previous inputs in addition to the present input. The demodulator at the
receiver is the corresponding M-channel analysis filter bank. The modulator and
the demodulator filter banks are shown in Figure 6.25. One of the features of
 the DWMT system is that the presence of a predetection filter is not essential at
 the receiver. Good performance can be obtained even without it. Because each
 filter in the DWMT modulator occupies a narrow band in frequency with respect
 to the channel spectrum, the distortion in a subchannel can be approximated by
a single amplitude scaling and a delay [Gracias 1994]. Consequently, detecting
 the signal at each subchannel would involve determining this delay, compensating
 for it, then down-sampling the output of each of the analysis filters [Gracias 1994]
(see Figure 6.25B). This form of equalization falls in the category of post-detection
equalization. It has greater complexity than the predetection procedure previously
 described. The down-sampled sequence of each subchannel can now be passed
 through a decision device before it is interleaved to give the symbols of the sequence
input at the transmitter. In general, DWMT systems are seen to be more robust to
ISI than DMT systems [Sandberg and Tzannes 1995].
216   C가her A尸尸I/c아幻ns 可 너／Ovele/ 加n計（가／TJS




                                                   愆n)




                                   Serial          月（n)
                                     to                                            To D/A
            Input Data -*-.
                                                                                   Converter
                                 Parallel
                                Convet妃r




                                              1兆if 入4odulator

                                                    (A)




                                                         枷


                                                         伽
                                                                     Parallel
        From A/D                                                        to       뇨 Output      +
        Converter             Equalizer                                            Data
                                                                      Serial
                                                                    Converter



                                                   h M
                                                          n
                                                          r
                                                          \  \
                                                                                                   l
                                                             J
                                              DMT Demodulator

                                                    (B)


      디gure 6.24 텨ock （계agrt그m of a gener이 DMT system: (/\) 如nsm附er and (B) receiver,
                                                          Commu配아跏A댜가匕아幻ns         217




Figure 6.25 帥＞ck diagr가T) 아汁he (A) mod네ator and (B) demod내aft가 in a DW卜肝 system.
                              CHAPTER SEVEN


                 Advanced Topics


7.1 Introduction
We now explore some of the deeper issues of wavelet transform theory. As de-
scribed in previous chapters, the wavelet transform resembles and yet differs from
other well-known mathematical transforms such as the Fourier transform. For ex-
ample, while the inverse Fourier transform is a one-to-one operator (that is, two
different functions of frequency differ in their inverse Fourier transforms), the in-
verse CWT is a many-to-one operator. Then, too, there is the issue of the wavelet
itself in a wavelet transform. Unlike the Fourier transform, which is uniquely de-
fined using the complex exponential function, the wavelet transform is a function
of the wavelet used. How does the choice of a wavelet affect the transform? Can
one design wavelets to match specific criteria? These are some of the issues that
this chapter addresses in detail.


7.2 CWTs Revisited

7.2.1 Parseval's Identity for the CWT

Recall from Equation 1.55 that if F(a, b) is the CWT of a function f (t), then the
inverse CWT is given by

                              I      f以） C以）           1
                    f (t ' = -      I    I            1= F(a ' h'hI,. ' Jt ' (1口 ih."    (7.1)
                   " "          C Ja=O Jb=-以） 기2 - ' " ' ' r U ' " " '              ."

The CWT is an inner product parameterized by scale and shift:

                                    F(a, b) = (f (t), 砂a,b(t)).                          (7.2)

Putting Equations 7.1 and 7.2 together we have


                          l C
                                    的       m
                                                     I
                                n
                                        n



                                 m
                f (t) =   1
                                1
                                九
                                /
                                        九
                                        ／


                                            1   m
                                                           ，砂a,b(t)）吼力（t) da db.
                                                    伍戶（J (t)
                                                                                         (7.3)


                                                      219
220   Advanced Top/cs

        Let V(a, b) and W(a, b) be the C人／Ts of two functions v(t) and w(t) respectively
      with respect to a mother wavelet 少 (t). We define the inner product as


                   (V(a,b), W(a,b)）砂三二．／的 /00 측V(a, 功W(a, 加a db
                                                           L/ 1／口＝=o Jb=-仗）／시n
                                                                                                                          (7.4)
      in the wavelet domain. An equivalence between the inner products of the functions
      and their CWTs is now established. From Equation 7.3,


                        v   (t나00,         a=O       b=
                                                      00-。。         IaI2佃따仇,        1               b   (t)     )蜘岫』「     (7.5)
      Therefore,

                              I f以그 f 00   1
                (v(t). w(tY = 三 I   I    -- (v(t)'. 砂口.'b(ti (w(t)'. 小口.',.(t1 da db.                                     (7.6)
                ' " " ' "     CJa=OJb=_。。 l기2 ' ' " ' " " ' " " ' ." "                                                    "

      From Equations 7.2 and 7.6 we have

                                          (v(t), w(t)) = (V(a, b), W(a, b))砂                                              (7.7)

      which might be seen as the CWT version of Parseval's theorem. A related conse-
      quence is

                                     IIf (t)112 = llF(a, b)屹三 (F(a, b), F(a, b))砂                                         (7.8)

      where F(a, b) is the CWT of f (t); that is,

                                               1 (00 (以） 1
                                     Ilf (t川' =C/，교＝   ．的而냥"(" ' b기' da db.                                               (7.9)


      Thus the quantity IF(a, b)I2/ClaI2 is the energy density of f (t) in the time-scale
      domain.

      7.2.2 Inverse CWT Is a Many-to-One Operation
      Let W (a, b) be the wavelet transform of a wavelet 少 (t) with respect to itself:

                                                    山（a, b) = （少（t), 砂口, b(t)).                                          (7.10)

      The wavelet transform of the dilated and translated wavelet by amounts u and v
      respectively is then given by

                                         （仇， 。(t)      ，
                                                           仇，   6
                                                                               (!       ))=   .(;   ，     흐二，   므）   ·
                                                                                                                         (7.11)
                                                                             CWTs Revisited   221

We introduce the following notation:

                                                 .):,(:
                                                                                    (7.12)
                                             ,
                                        （.
                                    『
                                                                   U으）   ·
                              吼
                                                              b-
Then, by Equations 7.2 and 7.7,

                   F(u, v) = (f (t), 少n, U(t)) = (F(a, b), '4'n,U(a, b))小           (7.13)

Thus if F(a, b) is the CWT of some function, then its wavelet inner product with
ii뇨, U(a, b) yields itself. Consider the set of all two-dimensional functions F(a, b)
for which Equation 7.13 is satisfied. This set (let us call it V少) forms a linear
vector subspace within the space of all two-dimensional functions that are square
integrable in the sense of IIF(a, b)II , being finite. Equation 7.13 shows that for a
function F(a, b) to be the CWT of a one-dimensional signal, a necessary condition is

                                                 F(a, b) EV吻                        (7.14)

Equation 7.14 turns out to be a sufficient condition as well, as we show next.
  Suppose Equation 7.14 is satisfied for some function F(a, b). Let

                                  f (t) = 伊(a, 끼，砂口, b(t)）步                         (7.15)

Now, the CWT of f (t) is given by

                                                 (f (r), 仇, 小）).                    (7.16)

Using Equation 7.15, we get

                     (f (t工 仇,小）)= ((F（口，b), 仇, b (t力小 也‘ . V(t)).                  (7.17)

This can be written as

                     (f (t工 仇, 小）) = 伊（口，功，（仇, b(t), 仇, dD)）砂                       (7.18)

which gives

                         (f (t), 少n, U(r)) = 伊（口，b), 山n, U((i,b)）小                  (7.19)

But by virtue of F(a, b) being in V少, the right-hand side of Equation 7.19 is F(u, v).
Thus

                                   F(a. b) = CWT of f (t)                           (7.20)
222   Advanced／아가Cs

      which proves the sufficiency of F(a, b) to be in V砂 for it to be the valid CWT of a
      signal.
         A function that is not in V少 is not the CWT of a signal. Suppose G (a. b) is one
      such function; that is,

                                  F(u, v) = (G(a, b), 'I'n, (a,b))少                       (7.21)

      where G(u, v) 尹 F(u, v). Thus G(a, b) is not the CWT of any function. However,
      by taking the inverse CWT of G(a, b) we get a function g(t) that in turn has a CWT
      G(a, b) (actually, as we soon show, its CWT is the F(a, b) in Equation 7.21). The
      inverse CWT of G(a, b) is also g(t), thus showing that the inverse CWT is a many-
      to-one operation, meaning that several different two-dimensional functions might
      have the same inverse CWT.


      7.2.3 Wavelet Inner Product as a Projection Operation
      Suppose G(a, b) is a function not in V砂; that is, its wavelet inner product with
      山n,1,(口, b) is a function F(a, b) that is not equal to G(a, b), as in Equation 7.21. We
      show that this F(a, b) is in V小 Consider

                                  F(u, v) = (G(a, b),山n,U(a, b))吻                         (7.22)

      We want to evaluate

                                       伊他v), 山c,d(U, v)）小                                 (7.23)

      Using Equations 7.22 and 7.23 we can show that

         ((G（口，b), q'H, U(a, b)）小 山C.d(U, v)）砂 = (G(a, b),（山n, U((i, b), 山C,d(u, v)）砂）小   (7.24)

      From Equations 7.22 and 7.24,

                   伊(u, v), 山C,d(ii, v力砂 = (G（口，b), （山U, U（口，b), 山c.d(U, v)）砂）小           (7.25)

      Using the fact that

                             山C,d(a, b) = （砂口,b (t）砂c,d(t)) = 山口, b(C, d)                 (7.26)

      we have

                       （山H, U((i,b), 1yC,d佃，v)）少 = （山口, b（兀 v), 山c,d（兀 v)）小               巴27)
                                                B月dging the G아）Be知／een C너／Ts and D너／乃   223

Also, because the inner products in the time and wavelet domain are equal (Equa-
lion 7.7), we can write

              （山口, j,(u, 毗 'F뇨(u, 끼）少 = （砂口, b (t), 少c,d(t)) = 山C,d(a, b).     (7.28)

Substituting Equation 7.28 in Equation 7.25 gives

                    伊他 미，山c,d（兀 v)）少 = (G（口，b), 山.,d(a, b)）少                   (7.29)

which yields, along with Equation 7.22,

                           (F(u, v),山c,d(u, v))中 = F(c, d)                     (7.30)

confirming that F(a, b) is in V砂.
   It also shows that the wavelet inner product operation with respect to W, (a, b)
is a projection operation onto the space V砂. Furthermore, note that F(a, b) is an
orthogonal projection of G(u, v) onto V吻 To see this, we simply need to take the
inner product of the error term G(u, v) - F(u, v) with 'I'a,b(U, v). This gives

 (G(a, b)-F（口，b), i1/. ,.((i, b)）砂 = (G（口，b), 山』, 小i力力r伊(a, b), 山., .（口，b)）吻 (7.31)

From Equations 7.20 and 7.21 we have

              (G(a, b) - F(a, b),WH, U(a力))砂 = F(u, v) - F(u, v) =0.           (7.32)

Thus, the error term is orthogonal to 'P, (a, b), which proves that F(a, b) is the
orthogonal projection of G(a, b) onto the vector space V.


7.3 Bridging the Gap Between CWTs and DWTs

7.3.1 CWTw什h 口n Orthonormal 的S祐-Gener베ng Way이et

Suppose we have a wavelet 砂 (t) that yields an orthonormal wavelet decomposition
of a signal f (t) as

                       f (t) = 2k12 ＞二＞二d（丸，n）砂（2_ ct - n)                     (7.33)
                                      k   n


where k and n are integers and

                         d(k,n) = (f (t),2_k12叭2_1ct - n)).                    (7.34)
224   Advanced Tc갸가Cs


      Observe that Equation 7.33 is the same as Equation 3.70, but for the scaling factors
      of 2小1d12. Suppose we now compute a CWT using the same wavelet

                                                                W(a, b) = (f (t), 砂a,b(t))                                                                     (7.35)

      where 仇,b(t) = (1/\"jai{)砂(t - b/a), and a and b are real. Sampling W(a, b) over a
      dyadic grid defined by a = 2' and b = 2kn for integer values of k and n, we obtain

                                                            W(21c, 2kg) = (f (t), 仍k ,2k (t)).                                                                 (7.36)

      Comparing Equations 7.36 and 7.34 we observe that

                                                                 d(k, n) = W(2k, 2kg).                                                                         (7.37)

      We thus see that the wavelet coefficients for an orthonormal DWT are simply the
      samples of the C사T on the dyadic grid.
        We can now relate the CWT to the DWT by using Equation 7.33 in Equation 7.35.
      We have



                                        b)   =                   2         k       n        d(k,        *(2_kt           -            *
                                                                                                                                                               (7.38)
                                                                                                                                                    (t)
                                                                                                                                                b
                                                                                                                                           a,
                                                                                                                                  ,
                        W   (a,                                                                                              n)
                                                     (2k/             二二                           n)
                                                                                                                                                          ).
      Interchanging the inner product and the summations gives

                            W     (a,   b)       =          > >d(k, (2_
                                                            k    7i
                                                                                       n)      k/2.     I/   ,(2_   kt   -   n)   ,   仇,        b   (t)
                                                                                                                                                          ).   (7.39)


      If we now denote (2田2砂口b - n), 仇,b(t)) by A(a, b; k, n), we can write

                                             w（口，b) = ＞二＞二d(k,n)A（口，b; k,n).                                                                                   (7.40)
                                                                               k       n


      Observe that for values of a and b on the dyadic grid, A(2HZ, 2etm; k, n) = 8(k -
      Z)a(77i- n).

      1.3.2 A Trous Algorithm
      Let us now look at the discrete approximation to a C叭／T. Suppose we take the
      CWT of a continuous-time signal f (t) with respect to wavelet 砂 (t) to yield F(a, b)
      as in Equation 7.2. A discrete approximation to F(a, b) at dyadic scales and shifts
      is obtained by computing EShensa 1992]

                                                                                   l         C,                     /n                     \
                                                                                                                                                               (7.41)
                                             叩（2, 2'm）三西i4/'("）少（三k叫
                                                  Bridging the Gap Between C너／了S and DVVTs   225


where f (n) is f (t) sampled at integer t. The rate of sampling of 少 (t) varies with
the scale. The coarser the scale, the more the number of samples of 少 (t) per unit
time. For example, when k = 0 (that is, when the scale factor is one) we use 砂 (t)
at integer samples of t, whereas when k = 1 we use samples of 少(t) at values of
t that are integer multiples of 1/2. Rather than storing sampled values of 砂 (t) at
multiple sampling rates, we might choose to start with samples at one rate and then
fill in approximate values for higher sampling rates. This filling in is done through
an interpolating or a trous (literally, with holes) filter of impulse response h(n). For
example, given 砂 (n),

                               寸（;)＝工少（i)力（n- 2i)                                  (7.42)


as depicted in Figure 7.1. To have


                                    畔)=唯）                                          (7.43)

for even ii, we require

                                      九（2미 = 8(n).                                 (7.44)

Similarly,


                           可（赤）＝각由小2i).                                            (7.45)


The limiting form of this operation as k 수 以） gives a function 'cfr(t), which is an
approximation to 少 (t). The a trous algorithm computes an approximate wavelet
transform through Equation 7.41 using the 'cit function rather than samples of 砂 0').
For example, at k = 1 we form


                          印（2加) =다미戶）                                               (7.46)



                                仁／的可'了' ）·                                          (7.47)




        디gure 7.1 Ir卄erp이ating 十he s（그('l耳)led wa四let u計'ig the a 加us 꿰ter.
226   Advanced Topics

      Using Equation 7.42, Equation 7.47 becomes

                          印（2, 2m) = Z            Z    f (i)叭助따2m- 却）                  (7.48)
                                          I       P



                                      = Zi Zm叭아 川싸 -2q).                               (7.49)
                                                  q


      Further simplification yields

                            印（2, 2m) =＞二砂（q- m)＞二／(i）九（i- 2q).                         (7.50)
                                          q                       i

      Let

                                      口（n) = ＞二／(i）九（i - 2n).                          (7.51)


      The sequence cl(n) is the result of filtering the sequence f (n) by a filter of impulse
      response h(- n) followed by downsampling by a factor of two. We then have

                                 印（2, 2川 = Z蜘 1 枷i(q).                                (7.52)
                                                      q

      Thus the approximate wavelet transform at scale two is a filtering of the sequence
      cl(n) by a filter of impulse response 砂 (- n).
         The approximation at subsequent scales can be expressed similarly as the filtering
      of decimated sequences. Let us derive the result for the next scale-namely, k = 2.
      We have

                               W(4, 4m)       수二／(i) （三 m)                             (7.53)

                                                                           44m)
                                              =       二f(m)   斫       (1
                                                                                       (7.54)


      From Equation 7.45,


                                  川）수如-2i)叱）·                                         (7.55)


      From Equations 7.42 and 7.55,


                            川卜 二口小2i)小抑伽）                                              (7.56)


                                   = Z Z蜘 H 싸따 2m)Vi回．                                 (7.57)
                                                                Bridging if)이拍p Be加een CW而 and 매刀s    227

Using Equation 7.57 in Equation 7.54 we get

               w（속刎＝Z ZZ加) h(小鈿- 2q）蜘口끼蜘）.                                                  (7.58)

Rearranging,

               w（生4川＝二加乞＞그(n - 4m -刎 （아2p)f（까                                               巴59)
                            p               ii   q



Putting 2m + q = r, we simplify Equation 7.59 to

               W(4, 4m) = ＞二砂伽）＞二h(r -2m口끼Z蜘- 2r)f (n)                                       (7.60)

                         = ＞二砂(p)＞二 h(r - 2(m + p))cl(r)                                     (7.61)

                         = :叭아川乞蜘4枷Kr）·                                                      (7.62)

Let


                                C2   (fl)   =    ＞二  ci   (i)   h(i   -   2n)   .           (7.63)

Then

                                w（由4川＝兄蜘1枷如）                                                (7.64)
                                                     q


which is a result of the same form as Equation 7.52. This process, called the decimated
a trous algorithm, can be generalized to other scales, as depicted in Figure 7.2. The
algorithm can be summarized as follows [Shensa 19921:

 1. Initialize f (n) = co(n).
 2. Convolve c1(n) with h(n).
 3. Downsample the result to give c1+i (n).
 4. Convolve c,+i with 砂(n) to give W(2i+1, 2i+lm).

The a trous structure is very similar to the DTWT computation of previous chapters
with the difference that there is no decimation following the filtering with the 少
filter, and the filters involved do not necessarily possess the perfect reconstruction
property.
228   AdvancedT야가Cs



              f (n) = C0(n)                c1                    c2(n)                c3
                                      2                     2                    2
                                                (n)
                                                                                           (n)
                                    0                 F(川                 F(n)   0
                                           山（n)                  山(n)                 11(n)



                                           I
                                          W(2,2m)
                                                                 1
                                                                W(4,4m)              w偶8m)


            F勾바e 7.2 The decim아ed a frous（계gorithm t키（Dck diagram.



         The decimated a trous algorithm is a time-varying algorithm in that any time
      shift in the original signal causes the wavelet transform to change its shape. If we
      want the approximation to be time invariant, then the CWT has to be computed
      at uniformly separated time shifts even though the scale sampling may be dyadic.
      The a trous algorithm can be modified to compute the wavelet transform at uniform
      shifts. To do this we use the noble identities (see Appendix A), which let us move
      the downsampling blocks around as shown in Figure 7.3. The undecimated wavelet
      transform coefficients are now obtained at the points indicated in Figure 7.3, which
      are located at uniformly separated time shifts.




      Figure 7.3 Moc獅C（그tion of the decimated a 加哨 이gorlthm using the n야긔e identities. The
                 unde（시mated way이아 卄ansform is obtained before the d（그니ins（그mF이ers （그5
                 indicated.
                                                             Regularity and Convergence   229

7.4 Regularity and Convergence
A scaling function has to satisfy the dilation equation


                              中（t) = 2＞二九（k）中（2t中k).                             巴65)
                                        k


Also, as we have seen, the DWT can always be implemented with multirate perfect
reconstruction filters. Suppose we reversed the order. In other words, rather than
starting from scaling functions and wavelets, if we started with a set of filters that
satisfy the necessary conditions for perfect reconstruction and solved the two-scale
relation, would the solution converge to smooth, continuous wavelets and scaling
functions? The answer is: not always.
   It is important that the iteration converge first to a function before we discuss
smoothness or regularity, as it is called in the wavelet literature. Let us deal with
the orthogonal case only. Recall that orthogonal wavelet decompositions are based
on PRQMFs that satisfy

                             1H(w)I2 + IH(w + 7r) 12 = 1.                        (7.66)


Suppose we have a PRQMF with the additional condition that

                                      H(O) = 1.                                  (7.67)

The latter is a necessary condition arising from the dilation equation on the filter
coefficients. Let us examine the solution to the dilation equation using frequency
domain iteration with the initial scaling function being the Haar.
  At the nth iteration we have


                           包(cv)＝中H(w/2")！如（劫                                    (7.68)

                                  = H(w/2)ct뇨如)/2)                               (7.69)

where 中H (cv) is the Fourier transform of the Haar scaling function. What we are
examining here is whether as n 나 以, the function J 佃) converges to a reasonable
function. Recall that our frame of reference has always been the set of square
integrable functions. Let us therefore test whether the iteration converges to a square
integrable or finite energy function. We do this using the Poisson summation. We
have


                             1 1i(2w)I = 1H(w)I VI）了(cv)I.                       (7.70)
230   Advanced 1갸가cs

      Putting w = w + 2k兀 and summing the squared magnitudes we have

                    刃이2w +4k兀기2 = 刃H(w+ 2k兀泊中如＋2bi-기2                                                          (7.71)
                     k                                k

                                             = 田佃）2                                                            (7.72)

      where we have used the facts that H(w) is 27r-periodic and that the Poisson sum
      for the Haar scaling function is identically equal to one. Similarly, putting w =
      w + 2k兀 + 兀 in Equation 7.70 and summing the squared magnitudes we get

                               刃叫2w +4k兀平 = 田佃＋兀기2·                                                            (7.73)
                                 k


      Summing Equations 7.72 and 7.73, and simplifying, we get the result

                                      刃包（아 2k兀기2 = I                                                           (7.74)
                                        k


      which shows that the Poisson sum of the first iteration is one. This implies that
      the scaling function after the first iteration forms, along with its integer translates,
      an orthonormal set. Using the same argument as Equation 7.74 with subsequent
      iterations, it follows that at every iteration we have a function that has unit energy
      and that forms an orthonormal set along with its translates. Thus, as n - 的 at
      least the finite energy condition is maintained if the PRQMF property is satisfied.
         The question now is whether there is convergence to a smooth, continuous func-
      tion. We list two sufficient conditions. One sufficient condition for pointwise con-
      vergence is that I H(w) I 5 I for w 尹 0. Yet another sufficient condition [Daubechies
      1988] is that if



                                 H(w)
                                 月（0)   -
                                        =    (
                                             (1   " " ' (_ "
                                                   +exP
                                                       2
                                                                g    (   "   fw)   '        7N
                                                                                                 )
                                                                                                               (7.75)


      then
                                        -                                                            R   (w)
                                            maxlR(w)I <2N-1.                                                   (7.76)

         Generally, the more zeros that H(w) has at w = ir [Daubechies 1988, 1992], the
      better the possibility of a regular scaling function and wavelet. This is so because the
      smoothness of the wavelet is related to the number of zeros of H(w) at w = 7r. Let
      us now establish the relationship between smoothness and zeros at 兀 for orthogonal
      wavelets. As we know, any wavelet 砂 (t) satisfies


                                                  f   i   (t)       dt =               0.                      (7.77)
                                                                                  Regularity and Convergence   231

The smoothness of the wavelet is increased if it satisfies [Daubechies 1992]


                                      f     t'砂         （t dt     =       0                           (7.78)

for several integer values of k, say 0 드 k < K. The wavelet is then said to have K
vanishing moments. From the properties of Fourier transforms we have


                        下［!' 砂（!)] =            /    加 (t) exp(- jwt) dt
                                                                                                      (7.79)
                                                .   k Ak山   （w)
                                                J
                                                         aw'
                                      =
where W (w) is the Fourier transform of the wavelet. From Equations 7.78 and 7.79 it
follows that the vanishing moment condition is equivalent to the frequency domain
condition

                                      d"W (w)
                                                                          0                           (7.80)
                                          dw"
                                                                  =
                                                          w=O


for 0 드 k < K. The wavelet satisfies the two-scale relationship

                             砂（t) = 2＞二g(k）中（2t - k)                                                  (7.81)
                                                    k


or its frequency domain equivalent,

                               W (w) = G(w/2)中(w/2)                                                   (7.82)

for a high-pass digital filter with impulse response g(n) (frequency response G(w))
and a scaling function 中(t) (Fourier transform 中(w)). We have


                            G(w) =＞二 g(n) exp(-jwn).                                                  (7.83)

Let


                                 小）       (w）           三 d佃，         巴   ）   .
                                                                                                      (7.84)

From Equations 7.80, 7.82, and 7.84, the vanishing moment condition is equivalent to

                                          G(k)(0) = 0                                                 (7.85)

幻rO < k << 尺．
232   Advanced Top/cs


         Equation 7.83 shows that G(cv) is a polynomial in exp(- jw). Such a polynomial
      is called a trigonometric polynomial. The fact that G(0) = 0, implies that G(w) can be
      written as1

                                         G(w) = (exp(- jw) 小 1)Q(w)                                     (7.86)

      for some polynomial Q(w) in exp(- jw). Differentiation of Equation 7.86 yields

                         G(1)(w) = (exp(- jw) - 1) Q(1)(w) - j (exp(- jw))Q(w)                          (7.87)

      where Q(1)(w) is the first derivative of Q(w). From Equations 7.85 and 7.87, Q(0) =
      0, which implies that (exp(- jw) - 1) is a factor of Q(w), which in turn implies (see
      Equation 7.86) that G(w) can be written as

                                        G(w) = (exp(- jw) - 1)2Qi(w)                                    (7.88)

      for some polynomial Qi (w) in exp(小jw). Thus we see that the fact that G(w) and its
      first derivative have zeros at the ori얹n translates to there being a zero of multiplicity
      two at the origin for G(c小 Continuing the derivation along similar lines leads to
      the conclusion that having the first K - 1 derivatives of G(cv) equal to zero at the
      origin is equivalent to G(w) having a zero of multiplicity K at the origin. Since
      the LPF frequency response H(cv) has a magnitude characteristic along the cv axis,
      which is a mirror image of that of G(w) about cv = 7r/2, this is equivalent to having
      K zeros for H(cv) at cv = 兀. Thus the more zeros H(cv) has at cv = 7r, the more the
      number of vanishing moments for the wavelet and hence the smoother the wavelet.


      7.5 Daubechies Construction of Orthonormal
          Scaling Functions
      Earlier we provided examples of compactly supported scaling functions and wavelets
      such as the Haar, D4, cubic B-spline, and so forth. Of these, the Haar and D4 pro-
      vide orthogonal wavelet decompositions. Both the Haar and the D4 belong to a class
      of compactly supported, orthonormal basis-generating wavelets constructed using
      an approach due to Daubechies [1988, 1992]. Let us first examine the necessary con-
      ditions on the H and G filters underlying an orthonormal decomposition. Suppose
      h(n) is the impulse response of the H 丘［ter or LPF in an orthogonal decomposition.
      Let

                                            p(k) 三 (h(n), h(n + k)).                                    (7.89)


      lWe are using what is called the factorization theorem, which says that if f (x) is a polynomial with root
      xo, then x - xo is a factor of f (x). In the present case we have a polynomial in exp(- jw) with a root at
      w = 0 (that is, at exp(- jc力 = 1).
                                Daubechies（力ns却叱加no八거加norm이 Scaling Func加ns              233

As we have seen, the PRQMF condition is equivalent to

                                 p(2k) = (1/2)8(k).                             (7.90)

Let P(w) = F{p(n)}. Then P(w) is the squared magnitude frequency response of
H(w) (however, P(w) is the power spectrum of h(n)):

                                  P(w) = IH(w)尸.                                (7.91)

Also, the frequency domain equivalent of Equation 7.90 is given by

                               P(w) + P(w + 7r) = 1.                            (7.92)

Recall that the property in Equation 7.92 makes P (w) the frequency response of a
halfband filter. In terms of the z-transform we have

                                  P(z) + P(- z) = 1                             (7.93)

＼人／
  here

                                 尸（z) = H(z)H(z小                                (7.94)

and

                                P(w) 三 P（之）1z=exp(jw)·                          (7.95)

That is, P(w) is P(z) evaluated on the unit circle. Apart from the perfect reconstruc-
tion condition, from Equation 3.77, we require that

                                    ＞二九（n) = 1.                                 (7.96)


   Thus, the thing to do would be to find a function P(z) that satisfies the PRQMF
property in Equation 7.93 and then obtain a function H(z) by factorizing P(z), as
in Equation 7.94. The inverse z-transform h (n) of this H(z) potentially yields an
orthonormal scaling function when used in Equation 7.65. The Daubechies tech-
nique provides an elegant approach to designing FIR filters based on such spectral
factorization. The idea is to have P (z) such that it is of the form

                            P(z) = (1 + z_1)k (1 + z)kR(z)                      (7.97)

with 2k zeros at cv = 兀. For a given k, a corresponding R(z) (essentially a polynomial
in z and z小 is determined such that it has the fewest possible terms and such that
234   Advanced ／야가cs

      P (z) is a power spectrum on the unit circle satisfying the PRQMF condition. The
      procedure yields HR filters of even lengths and is illustrated with examples.
      Example 7.1
           Let k = 1. Then

                                        P(z) = (z + 2 +戶)R(z).                                 (7.98)

           It is enough to set R(z) = 1/4 to make P(z) + P(- z) = 1. P(z) then factors to [(1/2) +
           (I/2)z][(1/2) + (1/2)z11. Choosing the causal factor leads to H(z) = (1/2) + (1/2)戶,
           the transfer function of the LPF for the Haar scaling function.                      U

      Example 7.2
           Let k = 2. Then

                                 P(z) = (z2 + 4z + 6 + 4z1 + zm2)R(z).                         (7.99)

           In this case, it is not enough to set R(z) to a constant to make P(z) + P(- z) equal to 1.
           Let

                                         R(z) = 口乙 + b + a乙-1.                               (7.100)

           Notice that the coefficients of R(z) e月ibit symmetry about the constant coefficient. It is
           necessary to choose the coefficients of R(z) in this manner because they are supposed
           to form an autocorrelation sequence. Then

       P（기 = a寸 + (4a + b)/ + (兀 + 4b)z+ (鈿 + 6b) + (7口 + 4b）尸 + （知 + 功d + 毗H3. (7.101)

           From Eauation 7.93 P0) = 1/2 and the other even-indexed values of v(n) are zero.
           Equation 7.101 leads to the equations

                                               8a + 2b == 0
                                                                                              (7.102)
                                            16a+ 12b = 1.

           The solution is a = -1/32 and b = 1/8. This leads to a factorization of R(z) as



                         R(z)=[1了"+ ' 8q [ ' y "『 '；二'］·                                     (7.103)


           The second factor, which is the causal term in combination with (1 + z1)2, gives us



                       帥）=['了"『 " 8+,J" -1『 " 8/"r'『 ' 戶_3]                                  (7.104)


           which co什esponds to the D4 coefficients. Because .k =2 in this example, some authors
           rerer to mese as me UL scaiing runction coerncients lnstea3 O IJ仕.                     -

                                                         岺 胄 字＼
                                           Daubechies Construction of Orthonormal Scaling Functions   235

   Daubechies gives a general method to compute an R(z) that has the fewest pos-
sible terms for a given number, N, of zeros at w = 兀, and gives a P(z) that satisfies
the PRQMF conditions. This R(z) is given by [Daubechies 1988, 19921



                        R(z)＝旨' 丁')(' - 4-")"                                              (7.105)


   This is a symmetric polynomial in z and z 1. It is important to note that if zo is a
zero of R(z), then so is l/ Zo. Similarly, since the coefficients of R(z) are real, if zo is
a complex zero of R(z) then so is 硝, where * denotes the complex conjugate. Thus,
the zeros of R (z) would occur in groups of two (that is, as z0 and zi1, if Zo is real)
and in groups of 4 (that is, as zo, z, l/ zo, and l/ z各, if zo is complex).
   By factorizing R(z) (that is, by choosing one of a pair of zeros in the real case and a
pair of zeros in the complex case) we obtain another polynomial Q(z), which can be
used to obtain H(z). Note that R(z) = Q(z) Q(z小. Thus, to ensure real coefficients,
zeros that are complex conjugates can be chosen out of the four complex zeros.
Example 7.3
     Consider N = 2. Then


                                           砒）= (2츨뭉）·                                       (7.106)


      The zeros of this polynomial are 2 - .,/互 and 2 + './. Thus R (z) can be written as


                        R(z）乙二'VI三
                                 （: (2- V互）
                                          )(:.'- (2－而））·                                    (7.107)


      We can therefore choose

                                    Q(z) = \/J3 -11（戶 （2 Vi))
                                                                                            (7.108)
                                           = !q"l + V自'7 1 + 1 - V自'.
                                             2          ' '        -       '-   1




     Using the Q(z) in Equation 7.108, we have


              帥）    =   ( ; )
                          "'   '      '"       '   ;(
                                                        (1   1
                                                         『而） 『1-
                                                              z-
                                                                 'V 듕） /
                                                                                            (7.109)
                    극小偈+ (3小z 1 + (3『而）z2 + (1+ V三）z3).

      This is, the. D4 scaling function (actually, it is a flipped version of the scaling function
      presenteu in iquiuon         / . UJ吐).                                                     -
236   Advanced T아가Cs

                  相b旭 7.1 Daubechies Sc（기ing Func恤＞nO（그efficients for
                          N = 2, 3, 4, and 5

                    N         Coefficients         N            Coefficients

                             0.48296291314                    -0.187034811719
                             0.83651630374                     0.030841381836
                             0.22414386804                     0.032883011667
                            -0.12940952255                    -0.010597401785
                             0.33267055295                     0.160102397974
                             0.80689150931                     0.603829269797
                             0.45877502118                     0.724308528438
                            -0.13501102001                     0.138428145901
                            -0.08544127388                    -0.242294887066
                             0.035226291882                   -0.032244869585
                             0.230377813309                    0.077571493840
                             0.714846570553                   -0.006241490213
                             0.630880767930                   -0.012580751999
                            -0.027983769417                    0.003335725285


        For higher orders of N, the factorization would have to be carried out numeri-
      cally. Table 7.1 shows the Daubechies coefficients for N = 2, N = 3, N = 4, and
      N = 5. The corresponding scaling and wavelet functions are shown in Figure 7.4.



      7.6 Bandlimited Biorthogonal Decomposition
      The Meyer class of wavelets is regarded as among the first construction of nontrivial
      wavelets, which generate orthonormal bases for L2(R) with scaling and shift param-
      eters on a dyadic grid. These wavelets are bandlimited. It is possible to generalize
      the Meyer construction to biorthogonal scaling functions and wavelets.
         Suppose 中(t) is a scaling function and 中(t) is its dual, as in Chapter 4. Let their
      Fourier transforms be 中(w) and 中(w) respectively. Let

                                       A(w) = 中（nJ)(ld(0)).                          (7.110)

      Suppose H(w) is the frequency response of a real digital filter such that
                                      中（2w) = //（이中m小                               (7.111)

      Equation 7.111 is the dilation equation for the scaling function in the frequency
      domain. We have H(0) = 1. We assume H(兀) = 0. Given these properties and the
      27r periodicity of H(w), it can be shown that for integer k with k 尹 0,

                                          中(2irk) = 0.                               (7.112)
                                                   的nc物咐ed日orthogonal Decomposition   237



         1




    0.8


    0.6


    0.4


    0.2


         0                             V\
                                             \
                                                           //\/H
  -0.2
                                                 ＼了
  中U. 냐
             0   0.5         1         1.5            2            2.5        3
                                                                         r+

    1 <




    11   1
             0   0.5         I         1.5
                                                      N2           2.5        3
                                                                         r+


Figure 7.4 (A, B) Scaling functions and wavelets corresponding to Daubechies
           filters h：升 八／ =2
238   Advanced Topics




                       1




                0.8


                0.6


                0.4


                0.2




                                               V
                   0


             -0.2


             1m tJ 1니1

                           0   0.5   I   1.5   2   2.5   3     3.5    4     4.5        5
                                                                                  i+

               ]   n




             eU.   O

                           0   0.5   1   1.5   2   2.5   3     3.5    4     4.5        5
                                                                                  r+


          Figure 7.4 (continued) (C. D) Scaling functions and wavelets corresponding to
                     Daubechies filters for N = 3.
                                               Bandlimited B/orthogonal Decomposition   239




Figure 7.4 (continued) (E, F) Scaling functions and wavelets corresponding to
           D（그ubec볘es filters 化rN == 4.
240   Advanced Topics




                               /\
                  1노 O
                                   1       1       1       1       1       1       1       1




                  0.6



                 0.4




                                       小
                 0.2                                                                                        .




                       1
                       0



             -0.2
                                                                                                        .




             1   1L벼

                           0   1       2       3       4       5       6       7       8                9
                                                                                               r+
                       1




                                                               L
                           - n卜 -
                           .
                                                                                                    ,




            1== 1J10

                           0   1       2       3
                                                       \
                                                       4       5       6       7       8            9
                                                                                               r+

         Figure 7.4 (continued) (G. H) Scaling functions and wavelets corresponding to
                    Daubec볘es fi什ers 幻rN = 5,
                                                  Band加刊ted Blorthogona! Decomp仍片幻n       241

  Let H(w) be a frequency response similarly associated with 巾(口）); that is,

                                中（2w) = H佃沖(小                                  (7.113)


The dual scaling function also satisfies the property in Equation 7.112:

                                      中（2兀k) == 0.                             (7.114)


  From Equation 4.34 we have

                                ＞二A(w+ 27rk) = 1.                              (7.115)
                                  k


Using Equations 7.112 and 7.115 we get

                                      A(27rk) = 8(k).                          (7.116)


   D可me

                            G(w) = exp(- jw)H(w+ 兀)
                                                                               (7.117)
                            G(w) = exp(- jw)H(w+ ir).


We then have a wavelet 砂 (t) and its dual 少 (r) with associated Fourier transforms
山(w) and 山(w) respectively such that

                                山（2w) == G(o小하w)
                                                                                (7.118)
                                山（2w) == G(o小b(n小



7.6.1 Scaling Function Pair Construction
Let 中(t) and 中(t) be symmetric, dual, dyadic scaling functions. Suppose their
Fourier transforms 中(w) and 小(w) are bandlimited to w0 rad with no zeros in
the range 이 < w0. It has been shown elsewhere EChapa 1995] that under these
conditions it necessarily follows that 兀 5 w0 5 47r/3. Let 中(w) and 1(w) indeed be
bandlimited to 47r/3 rad:

                                         中（w) === 0
                                                                                (7.119)
                                         中（w) = 0
242    Advanced Topics

       for Iw > 47r/3. For Equation 7.115 to be satisfied we then require


                                          A (w) =l      I끼 드 27r/3
                            A(w) +A(2ir- w) =l          27r/3< w< 47r/3                    (7.120)
                          A(w) + A(- 27r - w) = 1       -47r/3 <w 三 -27r/3.

      Since 中(w) and 中(w) are real because of the symmetry of the corresponding time
      domain functions, A(w) is also real. An immediate consequence of Equation 7.120
      is that


                                              A(ir) = 1/2.                                 (7.121)

         Theorem: If a continuous function A (w) bandlimited to 47r/3 rads satisfies the properties
      in E甲ation 7.120 w斛z no zeros over its su까70rt, then ai끄／ sp娩 of A (w) in加 a 尸a打 中 and
      中'satisfying Equations 7.110 and 7.119 yields Fourier transforms of a pair
                                                                                         of scaling
      functions that are biorthogonal duals of each other.
         Proof: Let us first show that 中(w) and 小(w) are scaling functions (that is, they
      satisfy dilation equations). It suffices to do this for 中(w) since the corresponding
      result for (1'(w) follows in a similar fashion. Define


                                        B(w) == 中（2w)／中（w).                                (7.122)

      ＼사e have


                                        B(w) = 0 w > 27r/3.                                (7.123)

      Define


                                      H(w) = y       B(w+ 27rk).                          (7.124)
                                                 k


      The function H(w) serves as the frequency response of a frequency domain dilation
      equation for 中(w), because by Equations 7.122 and 7.124, Equation 7.111 is satisfied.
      It therefore follows that 中(t), the inverse Fourier transform of 中(w), is a scaling
      function. That the inverse transform of 1(w) is a scaling function is similarly proved
      by defining a function H(w) on the lines of Equation 7.124. The duality of 由(w)
      and 中(w) follows directly from the assumption that Equations 7.110 and 7.120 (and
      hence Equation 7.115) are satisfied.
                                                                                             的nd加汁ted Biorthogonal Decom口Os作幻n    243

7.6.2 Wavelet Pair Construction
Putting together Equations 7.111, 7.113, 7.117, 7.118, and 7.124 we get dual wavelet
Fourier transforms 山(w) and 山(w):

                                                                                    中（2兀 -U小t (w/2)
                       山( (,)' =       pyn(- irn/ 7노
                                   ／                                  ,                  :    /
                                                                                        (P yr - 引
                        1   \1戶나       V1   =   1寸   \   1/   -            -,                        r .   노 \



                                                                                                                       (7.125)
                                                                                     t (2兀 - w)(1)(w/2)
                        \1rr/n\ =      Pyn(_ ih)I7 'I
                                   /                 '                                        /      ," \
                                                                                        (4J (7r H iJ
                        1   \M/
                                       느戶J1r             .'   1/ 1/   '-        /        未




Because we have assumed real-value Fourier transforms for the scaling functions, we
have dispensed with the complex conjugation required in Equation 7.110. The two
wavelets are bandlimited to 2i173 < 1wi <8ir/3 rad. The inverse Fourier transforms
少(t) and 少(t) of 41(w) and 山(w) respectively are the dual wavelets.
  We now proceed to show that a particularly simple structure arises if we let

                                       中（w) = 1 lo기 < 2ir/3.                                                           (7.126)

Then, from Equations 7.110 and 7.120 it follows that

                                       4 (w) =1                                     i(이 드 2ir/3                        (7.127)

as well. Equation 7.125 becomes


               41(w）나：咎芻喆已；' )                                                                    2ir/3 5 w 5 4n73
                                                                                                  4兀／3 5 w 드 8ir/3
                                                                                                                        (7.128)

               也(w)={：客芻搗’石' )
                                                                                                  2r/3 5 w 5 4jr/3
                                                                                                  4兀／3< w 드 8r/3.

Observe that for the wavelet Fourier transform, the section over 2jr/3 5 w < 42173
is made up of the section of the dual scaling function's Fourier transform from
w = -4兀/3 to w = -27r/3, and the section over 4兀/3 <w < 8r/3 is a dilated version
of the section of the scaling function Fourier transform from w = 2i173 to w = 4r/3.
In the case of the dual wavelet's Fourier transform, the scaling and dual scaling
function Fourier transforms switch positions.
Example 7.4
     We let
                                                                3
                                                     A (w) =--w+                              2                         (7.129)
                                                               ZJr

     for 2i173 5 w 5 4n/3. Elsewhere A(w) satisfies Equation 7.120. For 2兀/3 三 w 드 4n/3,
     中(w) is chosen to be the top, right quarter of the ellipse centered at w = 2ir/3 with its
244    Advanced Topics


                           ]
                           1




                                                                                                                        \
                      0.9

                  0.8

                                                 =7                                                                    \ \
                                        I                       I              I           T         I       I                 I
                                   .
                                                 /7
                                                                                                                                   '




                                                                        P(w)



                                         //
                  0.7

                  0.6

                                        I /1
                                                                                                                        \\\\
                                       7r/                                                                                  N\\1 :
                  0.5                                                                畝叫                          \d\
                 0.4

                 0.3

                 0.2
                               ,
                                                                    A(w)


                                       n                                                                                      \1
                       '
                                            /+
                 U.
                       C'               '              I    .              I           I         I
                       tJ                                                                                I              I

                       -5              -4             -3   -2          -1              0         1       2              3     4    5
                                                                                   w (radians)


              Figure 7.5 Function A(w) and the spectra of its factors 中(w) and 小(w).


            minor axis running from (2jr/3, -1) to (2ir/3,1) and its major axis running from (0,0)
            to (4兀/3, 0). Elsewhere, 中(cv) is symmetric and it satisfies Equation 7.126. Obviously,

                                                                    中（cv) := A (cv)／中（口)).                                             (7.130)

           Figure 7.5 shows A (口), 中(w), and 中(w). Figure 7.6 shows the scaling function and its
           dual. Figure 7.7 shows the wavelet and its dual obtained by inverse Fourier transform-
           ing Equation 7.128.                                                                 U



      7.7 De引gn and Selection of Way이이＄
      Several methods have been proposed to design wavelets and wavelet bases to spec-
      ifications. Let us look at three such methods.


      7.7.1 The Lifting Scheme

      The lifting scheme [Sweldens 1994, 1996a, 1996b] provides a simple method for cus-
      torn designing biorthogonal wavelets. It characterizes all possible sets of biorthogo-
      nal filters having the same H filter [Cohen, Daubechies, and Feauveau 1992; Herley
                                                              Design and Selection of Wavelets   245


                       1.   2




                       0.8


                       0.6
               砂（t)
                       0.4


                       0.2




                      -0.2                                                    (A)
                         -50                     0                       50



                       1.2




                       0.8


                       0.6
               中（t)
                       0.4


                       0.2




                      -0.2
                                          기尸M                                 (B)
                        -50                      0                       50
                                                 r


        Figure 7.6 (A, B) The scaling function (A) and its dual (B).




19931. Suppose {H, H, G, G) form a set of biorthogonal filters as in Chapter 4.
The perfect reconstruction conditions for the biorthogorial case are given by Equa-
tions 4.37 and 4.38. The filter frequency responses are related as


                                 G(w) = e_JOJH* (w+ 兀)                                 (7.131)

                                 G(w) = ejo)H* (w+ 7r).                                (7.132)
246   Advanced Top/cs




              Figure 7.7 (A, B) The wavelet (A) and its dual (B).


      The lifting scheme constructs new biorthogonal filter sets starting from a given set
      as explained next. Let 中(t) be a compactly supported scaling function and let H be
      the FIR filter associated with it. Let 斤 and H0 be two dual filters biorthogonal to H
      that satisfy all the requirements for perfect reconstruction (see Equations 4.37 and
      4.38). Thus,


                              H*(w)月（nD + i/ ' 佃＋끼I／佃＋兀）= 1                         (7.133)
                                                       Design and Selection of Wavelets   247

and

                     H' 佃）月아w) + 月' 佃 + 兀）月0(m + 兀） = 1.                       (7.134)

Filters H(w) and H0 (co) are then related to each other as

                       月回 = 月0(w) + 可加／/ ' 佃 + 兀）S*(2w)                        (7.135)

where S(w) is a 2ir -periodic trigonometric polynomial. Conversely, if one of H and
月o is biorthogonal to H and they are related through Equation 7.135, then the other
is orthogonal to H as well. The proof of Equation 7.135 hinges on the fact that for
perfect reconstruction filters, H(w) and H(w +兀) cannot go to zero simultaneously,
as seen from Equation 4.34. Therefore,

                          A < 田佃平＋田佃＋쩨2 < B                                    (7.136)

for two positive constants A and B.
   Let

                                d(n) = 石（n) - 石O(7)                            (7.137)

or, equivalently,

                               D(co) = //（口D- 吼佃）.                             (7.138)

Because H and H0 are each biorthogonal to H, from Equations 7.133 and 7.134 we
have

                       D(w)H* (co) + D(w + 兀)H* (cv + 7r) = 0.                 (7.139)

Now if we choose

                         D(cv) = exp(Hjco)H* (cv + Jr)S*(2o)                   (7.140)

where S(w) is a 2ir-periodic trigonometric polynomial, then we see that this choice
of D(cv) satisfies Equation 7.139. Using Equation 7.138 in Equation 7.140 gives
Equation 7.135.
   Using Equation 7.131, Equation 7.135 can be written as

                           月＠) = 斤0(w) + G(w)S*(2幼．                            (7.141)
248    Advanced 了야9/cs

       Substituting Equation 7.141 in Equation 7.132 we have

                         G(w) = e_jmHO*(w) - e_JmG* 佃 + 7r)S(2w + 2jr).                (7.142)

       Given the 27r periodicity of S(幼 and from Equation 7.132, Equation 7.142 simpli-
       fies to

                                   G(w) = G0(cv) - H(cv)S(2w).                         (7.143)

      Equations 7.141 and 7.143 serve as a basis for creating new biorthogonal pairs
      (H, H, C, G} using an existing set of biorthogonal filters {H, H0, G, G0} to some
      given specifications; say, for example, increased smoothness. This is done by choos-
      ing a suitable S(cv) in Equations 7.141 and 7.143 to get a new set of biorthogonal
      filters. Recall from Section 7.4 that smoothness is related to the number of vanishing
      moments [Herley 1993; Sweldens 1996a]. Now suppose that our initial set of filters
      are the Haar filters. Choosing S(cv) = -j sin (co)/4 would give a new set of flu-
      ters that have two vanishing moments and therefore higher smoothness [Sweldens
      1996a]. Other specifications could include better frequency selectivity or matching
      the spectrum of a given signal.

      7.7.2 Be針 Bas忖 $election
      The best basis algorithm seeks to represent a given signal in some optimal manner
      by choosing an orthonormal basis to represent that signal from a collection of basis
      functions [Coifman and Wickerhauser 1992]. This means that we represent the
      signal using a basis such that the representation minimizes some cost function.
      The cost function itself is required to satisfy certain criteria so that it describes or
      characterizes some feature of the signal. Specifically, the cost function should satisfy
      the following:

       1. It should be a measure of the number of coefficients required to describe the
          signal accurately. For example, the cost function should be large when all the
          coefficients have almost the same magnitudes and small if only a few coefficients
          are significant.
       2. It should be additive. The cost function of a sequence should be a summation
          of the cost function applied to the individual samples of the sequence.

         These requirements suggest that one of the definitions for an appropriate cost
      function could be similar to that of entropy in information theory. For a sequence
      x, we define this entropy cost function as

                                     肛（｛跏 = 스＞노pfl                                    (7.144)
                                                          Design and Selection of Wavelets    249


where

                                             1工n12
                                                                                   (7.145)
                                     pn= ＞二江n2 '

    Now, denote the sequence xi as a vector x and denote the transformed vector by
t = Bx where B is the basis for the transformation. Then, the best basis relative to
/t for a signal x is the basis chosen from a set of possible basis functions for which
the transformed signal t has the least cost ji(t).
    In general, the library of possible basis functions could include all possible bases.
It is possible to search through all of these and come up with a transform that gives
the least possible value (the global minimum) for the given cost function. However,
in practical applications it is necessary that the search be of low complexity and that
the basis be rapidly computable. As a result, the search is typically restricted to a
smaller subset of rapidly computable basis functions. As explained in Chapter 4,
wavelet packets provide a flexible basis with efficient algorithms for implementa-
tion. A wavelet packet transformation involves projecting a signal onto a number
of orthogonal subspaces Wj,小 In other words, the signal space V is decomposed
into orthogonal subspaces such that V = 今 j, n wj,, where i denotes the level of de-
composition and n denotes the nth subspace at that level. Each subspace 11;,. can be
decomposed into two orthogonal subspaces-namely, W(j+1), 初 4) W(汁l), 伽+1)· This
flexibility can be exploited to determine the optimal wavelet packet representation
of the signal with respect to the cost function. The best basis algorithm for wavelet
packets is as follows:


 1. Choose I as the maximal number of levels of decomposition.

  2. While the level of decomposition is less than 1, for each subspace WI,,, do the
     following:

      1 Compute the cost function for the transform coefficients on that subspace-
        尸（WI,4).
      1 Decompose                                     ,+l), and compute /.t(W(j+l), 2n) and
                      Wi,n into W(i+l),2n and W(I+l),(2,
        M(V%+n, (2n+l) ).
      . If /2(W,,) > /i(W(i+l),2n) + /L(W(j+l),(2fl+l)), then retain IL(W(I+l),2n) and
        尸( W(i+l),(2n+1) ); otherwise, retain M(까,n).


This algorithm has been used in applications such as audio and image compression
with remarkable results [Coifman and Wickerhauser 1992; Wesfreid and Wicker-
hauser 1993; Wickerhauser 1994].
250    Advanced Topics

       7.7.3 Wavelet Matching

      We now describe a method that, starting from a specified function, generates a
      mother wavelet 砂 (t) such that the latter is as close as possible to the specified
      function in some optimal sense while generating an orthonormal basis. First, let us
      review the construction of the Meyer-type scaling function and wavelet since it is
      used in the derivation of the matching algorithm. Let 中(t) be a real-value function
      of time and 中(w) be its Fourier transform. Further, let cb (w) be bandlimited to
      1wi <4ir/3 such that


                                                                                        (7.146)

      0 <w <2jr/3 and


                                   呻（兀 + Ct)平 + 呻（7r _w)12 = I                         (7.147)

      for 1wi < 兀/3. By virtue of the fact that 中(t) is real-valued, it follows that 11 (w)i is
      s戶llmetric about the origin.
        It can be shown that the function 4 (w) satisfies the Poisson summation formula,


                                       ＞二 陣(w+ 2兀k)I2 = 1                              (7.148)
                                        k

      thus indicating that {中(t - k) : k integer} is an orthonormal set. The function 中(t)
      serves as a scaling function in an orthonormal MRA. The corresponding wavelet
      amplitude spectrum Itl1(w)I is bandlimited to 2兀/3 < wi 5 87r/3 and is given by

                                                           乃
                                                               mm          乃乃
                                                      兀


                            니就寸
                                                                     兀 兀

                          凹（w） "1
                                                      n
                                                      二                                             <
                                                                                                    H           <
                                                                     4
                                                                     4 8               (7.149)
                                                       兀                                                    H
                                                       4
                                                       1                                        <
                                                                                                        <
                                                                                            H
                                                                                                    1
      An interesting consequence is that

                                  W (47r/3 - w) i = 卜P(4ir13 +2w)I                     (7.150)

      for 0 <w <27r/3.
         Let F(w) be the Fourier transform of the specified signal. We address the prob-
      lem of generating a function I'I' (w) I such that it satisfies the conditions of a Meyer
      wavelet while minimizing the squared norm of the function IF(w)12 - I'I' (w)I2
      [Raghuveer and Chapa 1996a, 1996c]. Let


                                         IG(o川 = 陌佃）2                                  (7.151)
                                                                 Design and Selection of Wavelets     251

and

                                     1A(w)I = IW (w)I2.                                  (7.152)

  We minimize


                                J=    f[   G(w)   -   A(w)]2dw                           (7.   153)
subject to the condition that A (w) is bandlimited to 2兀/3 5 이 드 8ir/3 and


                                                           0 0
                                                                         3
                                                                  mm
                   A (lr- w)2+ A(兀+ w)2= c
                            <
                            ＜
                            小
                            H
                                                                        小찌               (7.154)
                   A (4兀/3 -w) = A (47r/3 +2w)
                            <
                            <
                            H
                            1
Here, C is a constant. The idea is first to minimize the cost function with C as a
free parameter and then to minimize further with respect to C to get the minimum.
   An observation that helps us get a closed-form solution is that for any w in the
range 0 to 8ir/3 there are four values of A (w) that affect the cost function. For
example, if we considered a value of w, say A such that 2ir/3 < A < it, then A(시
enters the constraints along with (and only with) A (2ir - A), A (4兀 中 2入), and A (2入).
Thus the minimum is obtained if a four-parameter optimization is performed for
every w [Raghuveer and Chapa 1996a, 1996c].
   Let

                                     Fa 三三 G（시                                            (7.155)

                                     Fb 三 G(2兀 卞 入）                                       (7.156)

                                     Fc 三 G(2시                                            (7.157)

                                     Fd 三 G(4兀 寸2시.                                       (7.158)

Also, let

                                      a 三 A (A)                                           (7.159)

                                       b 三 A (2jr + 入）.                                   (7.160)

The minimization problem for these values becomes

               mmll J= (Fa- a)2+ (Fb- b)2+ (Fc- b)2+ (Fd- a)2                            (7.161)

subject to

                                           a+ b= C.                                       (7.162)
252   Adv口nced T야)iCS

         The solution is

                               a = C/2 + (Fa - Fb - Fc + Fd)/2                        (7.163)
                               b = C/2 - (Fa - Fb - Fc + Fd)/2.                       (7.164)

      Extending this to the entire function yields

               A(w) = C/2 + [G(w) - G(2兀 - w) - G(2w) + G(4兀 - 2w)]/2                (7.165)

      for 2m/3 5 w 드 4兀/3. For the range 4기3 5 w 5 8兀/3 we simply use Equation 7.154.
         A further minimization of the cost function with respect to C yields

                                i   r r4兀／3             l     r Slt/3   1
                           C =石 [J,/. G(w)dw + 2 J,/. G(w)dco].                      (7.166)
      7.8 Perfect Reconstruction Circular Convolution
          Filter Banks
      In Chapter 3 we established a connection between orthonormal wavelets and perfect
      reconstruction filter banks. These filters satisfy what are known as the power com-
      plementarity conditions and the paraunitary conditions given in Equations 3.43 and
      3.45, respectively. In this section we look at what we call perfect reconstruction cir-
      cular convolution (PRCC) filter banks [Bopardikar 1995; Bopardikar, Raghuveer, and
      Adiga 1997a, 199Th; Vaidyanathan and Kirac 1997]. These filter banks are designed
      entirely in the discrete Fourier transform (DFT) domain and satisfy perfect recon-
      struction properties in the discrete frequency domain. The formulation of these
      filter banks is made on the assumption of a finite-length input sequence of length
      N. In addition, all the operations associated with the filter bank implementation
      (namely, filtering, downsampling, and upsampling) can be implemented entirely in
      the discrete frequency domain. To see how this can be done, we first interpret the
      processes of downsampling and upsampling in terms of the DFT. Note that during
      this discussion we use the notations X(k) and X(e12兀kIN) interchangeably to denote
      the DFT of an N-length sequence x (n).


      7.8.1 Downsampling

      Consider Figure 7.8, which shows an M-fold downsampler. The input to an M-fold
      downsampler is a sequence x(n) of N samples. The output of the downsampler,
      denoted by y(n), is given by [Vaidyanathan 1992]

                                              y(n) = 工（兀fn)                          (7.167)
                                                                               Perfect Recons什uction Circular C이刃（7幻加nF肝er Banks                                253




        Figure 7.8 An M-f이d downsan갸이er.



where the sequence y(n) has N/M samples. It is assumed that N is an integer
multiple of M.
  To obtain an expression for the DFT of the output sequence y(n), we first define
an N-length intermediate sequence

                                                                                                     multiple of M
                           r4 r77) =                                                                                                                  (7.168)
                                                                x                         n=
                                                                         (n)
                                                              Eu-                         （江ner＼
                                                                                          ot--    人／ -
                                                                                                   ise.
                                                                                               ---w-   -.


  Clearly

                                                         y(n) == 工（凡fn) = 幻（Mn).                                                                      (7.169)

Now the DFT of y(n) is

                                                                                         N/M-1
                           Y     (ei                 "   kI(NtM)
                                                                               )   =      ＞二
                                                                                          n=o
                                                                                                     y          (n)         e日" k/(N/4i)
                                                                                                                                                      (7.170)


k = 0, 1. . . . .N/rn - 1. Substituting Equation 7.169 into Equation 7.170 gives

                                                                                    ／믹M-I
                       y   (ej             "   k/(N/4i)
                                                                    )=                   ＞二
                                                                                         n=O
                                                                                                 xi      (Mn)                     e_   "kI    (N/M)
                                                                                                                                                      (7.171)


k = 0, 1. . . . .N/M - 1. Because xi(n) is zero at all n except when n is a multiple of
M, Equation 7.169 is equivalent to

                                                                                               N-I
                                       y       (e/        "   k/(N/4i)
                                                                                    )=          二
                                                                                               m=O
                                                                                                     xi               (m)        eU    "     k/N
                                                                                                                                                      (7.172)


k = 0, 1. . . . .N/M - 1. Now, to represent xl(n) in terms of x(n), we define a comb
sequence


                                                                                          l祈     m二山
                                                                                                         (?／兀／ M
                                                          CM (fl)                  ＝二
                                                                                                                            n/
                                                                                                                                                      (7.173)
254   Advanced ／아가cs


      Observe that CM(fl) is the inverse DFF of a sequence of M ones and hence is periodic
      with a period of M. Thus,


                                          尸11rn\
                                          1r in \r r /
                                                       =       !! otherwise.
                                                               IU
                                                               1
                                                                U
                                                                   rl   兀＝
                                                                         1 1
                                                                        Ot1ler1VlSe.
                                                                                       m프itiple            of M                 (7.17幻


      Using Equations 7.173 and 7.174 we can now write

                                                           工i (n) = CM伽）工(n)                                                    (7.175)

      or

                                                                             ]         쯔二:1

                                                工i(n)＝工（n）言   2; ej"'"/M·
                                                          ='= 1==0
                                                                                                                                (7.176)


           Substituting Equation 7.176 into Equation 7.172 gives

                                                                    ]   쓰므                        坦크
                          Y   (e12    '   1N1M)
                                                     )     =       言)
                                                                   1'= n=0
                                                                             x   (n)
                                                                                                  1=0
                                                                                                                                (7.177)


      k = 0, 1. . ...N/M - 1, which can be simplified to


                                                                         l而
                                                                                 mZ山              X    Uh       刹 川
                                     Y(ej2兀d1(Ih1M) ) = 二 '5:-.' x (ei2i(k_ 伊)1I)
                                                                                                                        /

                                                                                 M
                                                                                                                    )
                                                                                                            q
                                                                                                                                (7.178)
                                                                                                                            H

                                                                                                                    J
                                                                                                            \
                                                                                                   1
                                                                                                                    /
                                                                                                   \
      k = 0, 1. ....N/M -1. This derivation is very similar to that presented by Vaidyana-
      than [1992] for general sequences. Note that Y(k) is N/M-periodic. In other words,
      the inverse DFT (IDFT) of the first N/M samples of Y(k) gives the downsampled
      version of the input sequence. From Equation 7.178 we see that the DFT of the
      downsampled sequence Y(k) is a sum of M coefficients of the DFT of the input to
      the downsampler, X(k), spaced N/M coefficients apart. For example, when M = 2,
      the steps involved are the following:

       1. Take the DI丁 of 工（n).
       2. Add the DFT of x(n) and its N/2 rotated version. This makes use of the N
          periodicity of X(k).
       3. Divide the resulting sequence by two.
       4. Take the IDFT of the first N/2 samples.

      This creates the 川2-point downsampled sequence y(n).
                                                Perfect Rec（기iS机兀f幻ci Circular Cony이岫on F肝erBanks   255


                                                           L
                               x(n)                             m叫H+    yin)



         Figure 7.9 An L-f（긔du口S（그m이er,



7.8.2 Upsampling
The block diagram of an upsampler is shown in Figure 7.9. An L-fold upsampler,
where L is an integer, takes an input sequence x (n) of N samples and produces an
output

                          . .              I x(n/L)        n = multiple of L
                         )\7iJ = 1 rl                      -,                            (7.179)
                                 t (J                      otnerwise.

The output sequence y(n) has NL samples. The DFT of y(n) is given by

                                                         NL-i
                          y（
                           「j2' k/(NL))= ＞二 y伽）e"j2' k"/(NL)                             (7.180)
                                                         n=O

k= 0, 1. . ...NL- l. NotingthatonlyeachLnth, n= 0, 1, ...,N- lsampleofthe
upsampled sequence is nonzero, we can write Equation 7.180 as

                                                         N- i
                           y
                               (ej2
                                       '   k/(NL)
                                                    )=
                                                         ＞二 (Ln)
                                                         n==0
                                                                y
                                                                    eUht "   /"T
                                                                                         (7.181)

k = 0, 1, . . ., NL - 1. This can be simplified to

                                      y (ej2兀k/(NL) )= X(eJ2兀k/N)                        (7.182)
k = 0, 1. . . . .NL - 1. In words, the NL-length DFT of the upsampled sequence
Y(ej'兀k111") ) is nothing but a concatenation of L DFTs of x(n). The derivation of
Equation 7.182 is again along lines very similar to the derivation given in Vaidyana-
than [1992] for an infinite sequence.

7.8.3 Procedure for Implementation
PRCC filter banks are filter banks designed and implemented completely in the
discrete frequency domain, and satisfy the conditions for perfect reconstruction over
a discrete set of frequencies. The operations of downsampling, upsampling
                                                                                , and
filtering are carried out entirely in the discrete frequency domain. The basic proce-
dure for their implementation can be understood by referring to Figure 7.10. The
analysis side of the system is shown in Figure 7.IOA. Here we first take the DFT of
the N-length input signal x(n). Next, we multiply this DFT, X(k), pointwise with
256   Advanced Topics




             Figure 7.10 PROC filter bank system. (A) Analysis filter bank. (B) Synthesis
                         filter bank.




      a sequence H0(k), which is the DFT of an N-length sequence ho(n). This amounts
      to convolving circularly sequences h0(n) and x(n). The resultant sequence is then
      downsampled by two as explained in Section 7.8.1. The procedure is repeated for
      the lower branch with H (k),the DFT of h1(n). In this manner, we decompose the
                                                                 Pet伯아 尸econ計띠아幻n （긔rc내아（力fly이ut/on F肝or Banks                             257

input sequence into two sequences of length N/2 with DFTs denoted by Vo(k) and
 V1(k) respectively.
    The synthesis side of the system is shown in Figure 7.10B. Here we upsample
the sequences V0(k) and V1(k) as explained in Section 7.8.2. This gives us two Se-
quences U0(k) and U1(k) of length N. These are then multiplied pointwise with
Fo(k) and F1(k), which are the DFTs of N-length sequences fo(n) and fi (n) re-
spectively. They are the synthesis filters corresponding to the analysis filters ho(n)
and hi(n) respectively. The output of the synthesis ifiter bank is thus given by
 XR(k) = Fo(k)U0(k) + F1(k)U1(k). The reconstructed signal is then the IDFF of
 XR(k)-namely, XR (n).
   Note that the PRCC filter bank is a framework based in the discrete frequency
and is different from the work proposed by several previous authors on fast imple-
mentation of FIR filter banks based on the FFT [Rioul and Duhamel 1992]. We next
present the conditions for perfect reconstruction for the PRCC banks.

7.8.4 Conditions for Perfect Reconstruction
Because the input sequence is of length N, it follows from Section 7.8.3 that the
analysis and the synthesis bank filters also have a support of N samples. Fur-
thermore, we assume that N is even, and that all of the sequences and filters are
real-valued. The transfer function of the analysis-synthesis system and conditions
for perfect reconstruction in this case are obtained in a manner similar to that de-
scribed in Vaidyanathan [1992]. They are cyclic counterparts of the corresponding
linear relationships. Using Equations 7.178 and 7.182, the transfer function of the
analysis-synthesis system is given by

     文（/' "   ",   )=        ;［札
                                          （／ " ）凡（.加，
                                                瓦
                                                    "                         )＋局
                                                                                      （a"   ",   ）月（  「肛，   k/N) ]X   (ei2lrk/   N)


                        =    ;iib
                                           (-   ／包
                                                          "    ）凡（ 《肛k/       N) +
                                                                                                                                 (7.183)

                             月l(Hej27rt/N)Fi(e12兀k/N)]X(_ e32兀k/ sl)

for k = 0, 1. . . . .N 小 1. The second term in Equations 7.183 is the alias term. To
cancel this term we choose

                                                        尻（eihFd1'N) = mGej2兀k/N)                                                 (7.184)
                                                        瓦（ej2兀k/N) = m／而（-e'2兀k/N).                                              (7.185)

In addition, substituting Equations 7.184 and 7.185 into Equation 7.183 gives


                            文（ '    「j   " ",   ）글帥肛，                     "         ）局（- 缸，
                                                                                       e） "      )-
                                                                                                                                 (7.186)
                                                                          (- eh "川）]X(ej2兀k/N).
                                                              Hi (ej2兀互川）H。
258   A加anced／야Jics

      Thus for perfect reconstruction we require

             蜘(ej2兀k川川i(- e2 '川）- Hj(ej2兀k川）玭(- ej2兀k/N) = ce小j2兀L/N                    (7.187)

      k = 0, 1. . . . .N - 1. Here c is a real constant and L corresponds to a circular shift.
        Following Vaidyanathan [19921, we require that Ho(ei2兀k川) satisfy the power
      complementarity condition given by

                                나而（ej2兀k/N)12 + Il而（-ej2兀k/N)12 = 2                     (7.188)

      k = 0, 1, . .., N- I. In other words, we require that IHo(e32兀Ic/N)I2 be a halfband filter
      or an equiripple filter (that is, antisymmetric about w = 7r/2 or equivalently n = N/4).
      For perfect reconstruction we choose

                               Hj (ej2兀k川） = 1ej2兀k/N局）(He4j2兀k/N).                     (7.189)

      Using Equation 7.189 in Equations 7.184 and 7.185 we get

                                凡（ej2兀k/N) = ej2兀k/N1而（e/2兀k/N)                         (7.190)
                                Fi(ej2i1'1") = ei2兀k/ IH1(eei2兀ld!').                   (7.191)

         Equations 7.188, 7.189, 7.190, and 7.191 ensure that the filters satisfy the equivalent
      of paraunitary conditions in this domain [Bopardikar 1995; Vaidyanathan 1992] and
      hence satisfy the cyclic orthogonality relationships given by

                       N-I
                       ＞二瓦伽）九j((n+ 2t) mod N) =8(i, f）各（2t mod N, 0)                    (7.192)
                       n=0

      where Z is an integer and i, j = 0, 1. Note that these are the cyclic equivalents of sim-
      ilar relationships satisfied by orthogonal or paraunitary filter banks [Vaidyanathan
      1992].


      7.8.5 Procedure for Constructing PRCC Filter Banks
      To obtain the filters H1(ej2兀k川), F0 (ej2兀k1' '), and F1(eJ2兀k/N), we first need to design
      the prototype filter Ho(ei?.兀k/N). For this we require the halfband filter H(e12兀"")
      defined as

                               H(ejh'/ ') = 怖（ej2 川胤化-j2r町N)                            (7.193)
                                                      I!卄erpok그／or$ 八／latched 九＞ the In口ut Process      259

k = 0, 1. ....N - 1. Note that H(eJ2兀k11") is a zero-phase filter. Thus, the design
of H1(ej2兀k") or H(k) is equivalent to assigning a value to each DFT coefficient as
follows. Assuming 0 5 H(k) 5 1 for some H(k),

 1. H(N- k) =H(k)
 2. H(N/2 - k) = I - H(k)

 3. H(N/2+ k) = H(N/2 -k)

Ho(k) can now be designed by taking into account the fact that

                                H (ej2兀k/N) = 1J而（e12兀k/N)12.                               (7.194)

Therefore,

                               I!而（ej2兀k/N)1 = 月（ej2兀k/N)1/2.                               (7.195)

Given that, in general, Ho(ej2兀t川) has the form

                              月0(ej2兀k/N) = 田0(ej2兀k/N기e加（k)                                (7.196)

we can now add the phase term (t). Because we require that ho(n) be real, 中(k)
is antisymmetric about N/2. The filters H1(k), F0 (k), and F1(k) can now be derived
using Equations 7.189, 7.190, and 7.191.
Example 7.5
     Suppose N = 8. Let H(0) = 0.75, then H(4) = 0.25. Let H(1) = 0.37, then H(7) = 0.37
     and H(3) = H(5) = 0.63. Finally, H(2) = I - H(2) = H(6) = 0.5. Thus, H(k) =
     {0.75, 0.37, 0.5, 0.63, 0.25, 0.63, 0.5, 0.37), and hence h(n) = {0.5, 0.0166, 0.0, 0.1084, 0.0,
     0.1084, 0.0, 0.0166). Note that the nonzero, even-indexed points of h(n) have a value of
     zero. From Equation 7.195, this gives us IHo(k)I = {0.866, 0.6082, 0.7071, 0.7937, 0.5,
     0.7937, 0.7071, 0.6082). Let us choose 砂(k) = {0, 1.1168, 0.2302, -2.6746, 0.0, 2.6746,
     -0.2302, -1.1168). This gives ho(n) = {0.2355, 0.2746, 0.2215, -0.1162, 0.4565, -0.13721,
     -0.2305, 0.1618). 가is completes the design of H0(k). The ifiters H1(k), F0(k), and F1(k)
     can now be determined. Note the flexibility and ease of design that this method offers
     for designing filters to specification.                                                      U


7.9 In恒巾이a伯rs M아ched to the Input Process
The formulation of the PRCC filter bank structure was motivated in part by the
search for efficient methods to implement the DWT for the bandlimited scaling
function and wavelets. There are several scenarios in the fields of communications,
signal analysis, and pattern recognition in which bandlimited scaling f끄lctions and
260   Advanced Topics

      wavelets could be better suited compared with the scaling function and wavelets as-
      sociated with compact support. One example of the utility of bandlimited wavelets
      was given in Section 7.7.3. In this section we give another example of a possible
      scenario in which a bandlimited scaling function or a function derived from it could
      be useful.


      7.9.1 Interpo山tion 鈿m帥ng

      The interpolation sampling system [Aidroubi and Unser 1994] is shown in Fig-
      ure 7.11. Here we consider a wide sense stationary (WSS) process 1 (r) sampled at
      integer t to give the sequence f (n) : f (n) = f (t)l,=., n, integer. Let the interpolating
      filter be t (t). Then the reconstructed process is given by

                                                                     的

                                           fa(t) = ＞二 f (n)t(t - n).                                                                 (7.197)


        We look for t (r) that will be optimal in the mean-squared error sense. In other
      words, we look for t (t) that minimizes

                          MSE(t) = E[(f (t) - 1O(r))2]
                                                                                                                                     (7.198)




                                                                                                                       )]
                                                                 (!                  『（4)
                                                                                   ,，立

                                                                 (t)                  f (n)
                                       =    2        [     (7        ).                       /(!             '   4)
                                       =   E         [(1                  -                   t     (t        -   n)   )2
      Differentiating Equation 7.198 with respect to Z (t - k) and equating the result to
      zero gives


                                   I            /                         쮸，                                      rn
                        8Z(t- k)   L   "
                                                \f         (r)   _            느f         (n)t (t_        n)
                                                                                                                  ) ])      =   0.   (7.199)




              Figure 7.11 Systen) 幻r ir卄erp이ation san갸케ng.
                                                                     Interpolators Matched to the Input Process       261

By interchanging the expectation and the differentiation operators we get



                40-k)(（『.）上似！-n)) )i                                                                   = 0 (7.200)



        E[(f(t）上仙미小住仙-n)i                                                                              = 0 (7.201)



                    [(f       ) ]         E           (t)    -   ,，立        f (n)『(t   -   n)
                                                                                                f(k)
                                                                                                       = 0. (7.202)


This now simplifies to

                                                  的


                          R(t- k) =              乞 R(n- k)t(t-
                                                n= -00
                                                                                  n)                        (7.203)

where R(v) = E[f (t)f (t + r)1 is the autocorrelation of f (t). Taking the continuous
Fourier transform of both sides we get



                             L   (w)      =     Z느       ,   풍： )    ,
                                                                     )   *: , ,
                                                                                                            (7.204)


where S(w) = F (R(r)) is the power spectral density of the process and L(w) is the
Fourier transform of t (t). Note that we have used the relation

                            00                                   的

                           ＞二 R（兀）eU " = ＞二S（回＋2兀k)
                          n＝尸00
                                                                                                            (7.205)
                                                             k:＝以）



in getting the result in Equation 7.204. From Equation 7.204,

                                         的

                                        兄       L(w +2兀n) = 1.                                              (7.206)
                                       n ==m的



It follows from the discussion of Poisson summation in Chapter 3 that

                                                Z (n) = 8(n).                                               (7.207)

In other words, t (t) is zero at all nonzero integer points as is required of an inter-
polation function.
262   Advanced 了아加S

        Consider the case when S(w) is bandlimited to 1w = Jr. In this case, from
      Equation 7.204,

                                      L(w) =1      IwI 5ir
                                                                                       (7.208)
                                            = 0    otherwise.

      The interpolating function is thus an ideal brick-wall ifiter. This corresponds to the
      classical sampling theorem [Daubechies 1992; Shannon 1949].
         Now consider the case when S(w) is bandlimited to 끼 = 4ir/3. For this case,
      L(w) is bandlimited to 4兀/3. Also, from Equation 7.206 we see that

                                     L（兀 + 미 + L（兀 - a) = 1                            侃209)

      for al < 兀/3. Thus, L(w) satisfies all the conditions satisfied by 呻(w)已 the power
      spectrum of the Meyer scaling function. In addition, it is matched to the power spec-
      trum of the input bandlimited process. This has the consequence of minimizing the
      mean square error between the interpolated signal and the input signal [Bopardikar,
      Raghuveer, and Adiga 1997a, 199Th].
         An impediment to more widespread use of bandlimited wavelets has been their
      infinite time support that makes the corresponding filters of the h1R type, usually
      without a finite order difference equation. To get around this, an appropriately
      truncated version of the time response can be used. This results in a loss of the
      bandlimitedness property. For the DWT, it also means loss of invertibility and
      perfect reconstruction. The PRCC filter bank structure provides a simple and flex-
      ible framework for a frequency-sampled implementation of the bandlimited scaling
      functions and wavelets while guaranteeing perfect reconstruction. This process is
      explained in the next section.

      7.9.2 Frequency-Sampled Implementation of
            Bandlimited DWTs
      The power spectrum of the Meyer scaling function 陣(w)12 satisfies the conditions
      of an interpolating filter in that it is antisymmetric about w = 兀. It follows that if it
      is properly sampled in the frequency domain then these properties can be retained
      and a halfband filter can be obtained. To determine the rate at which it needs to be
      sampled, it is important to note that the function needs to be sampled symmetrically
      about the angular frequency of Jt units. This means that if the required filter size is N
      samples, where N is assumed to be even, then the samples should be Aw = 47r/N
      units apart in frequency so that the samples are antisymmetric about N/4. As
      explained earlier, the square root of these samples gives the samples of the LPF
      H0(k), which can now be used in the PRCC framework. The shape of the LPF and
      the HPF thus obtained are shown in Figure 7.12.
                                                  II卄erp이ato店 M아ched to the In尸（it／가ocess   263




Figure 7.12 LPF (A) and HPF (B) responses obtained by frequency sampling the power
            spectrum of the Meyer scaling function.
264   Advanced 厄口七S

      7.10 The 鈿aling Operation and Se作＄imi七rS勾n이＄
      A distinguishing feature of the wavelet transform is the dilation or scaling operation.
      Let us now examine various properties of this operation in detail.

      7.10.1 LTI Systems and Eigenfunctions
      As a prelude to examining the dilation operation, let us look at some aspects of a
      more familiar system model (namely, LTI systems). From a mathematical viewpoint,
      a continuous-time LII system is a transformation T[ I that maps any continuous-
      time signal x (t) to another continuous-time signal y (t),

                                                         y(t) = T[x(t)I                              (7.210)

      with the properties of linearity

                          T[a1x1(t) + a2x2(t)] = a1 T[xi (t)] + a2T[x2(t)]                           (7.211)

      (for all scalars ai and a2 and all signals xi(t) and x2(t)) and time-invariance

                                              T[x(t - t0)] = y(t - t0)                               (7.212)

      (for all time shifts t0).
         Associated with such an LTI system is its impulse response h(t), relating the
      input and output through the convolution integral


                                         y   (t)     =    f   h(r)   x   (t   -   r)   dr.
                                                                                                     (7.213)


      Suppose we provide as input to this LTI system the complex exponential signal

                                                   x(t) = Aoexp(jczot).                              (7.214)

      The output signal is

                                     y(t) = A0H(Q0) exp(j2ot)                                        (7.215)

      ＼人／
        here

                                                                                                     (7.216)
                             H(Q)   ：下              [h(t)1 =    f』       （t) 8xp(_       JQt)   dt

      is the frequency response of the system. Equation 7.215 tells us that whenever we
      feed a complex exponential signal (essentially two sinusoidal signals of the same
                                                                The Scaling Operation and Self-Similar Signals   265

amplitude and frequency but phased 90 degrees apart, forming the real and imag-
mllary parts) into an LTI system, the output is the same as the input except for a
scaling factor obtained by evaluating the frequency response function at the input
frequency. When an input to a system results in merely an amplitude-scaled version
of itself as the output, we say the input is an eigen切iction of the system TEl. Thus,
complex exponential signals are eigenfunctions of LTI systems. The correspond-
ing amplitude-scaling factors (that is, terms of the form H(52o) in Equation 7.215)
are called eigenvalues of the system. While the complex exponential signals are
eigenfunctions for any LTI system, the set of eigenvalues (the frequency response
function) is unique to the system.


7.10.2 Continuous-Time Linear Scale-Invariant System

Most of the traditional signal processing applications are based on the LTI system
model [Poularikas and Seely 1991] described in the previous section. It is assumed
that the fundamental characteristics of the signal do not change with respect to time
shift. Although this framework is appropriate for the modeling of a large variety of
signals, there are signals that require other types of modeling. In particular there are
signals that are self-similar, in that segments of such signals are similar in some sense
to the whole signal. In other words, the temporal scaling (dilation or contraction) of
the signal simply reproduces the signal itself (in the deterministic case) or its funda-
mental statistical characteristics (in the stochastic case). Examples of such signals are
fractional Brownian motion [Crilly, Earnshaw, and Jones 1991; Feder 1988; Hastings
and Sugihara 1996; Mandelbrot and Van Ness 19681, fractional Gaussian noise [De-
riche and Tewfik 1993a, 1993b], 1/f noise [Keshner 1982], and homogeneous signals
[Wornell 1996b; Wornell and Oppenheim 1992a, 1992b]. The study of these signals
requires a different signal processing approach than that typified by Lii models.
The role of scale (dilation) in defining self-similarity provides the basis for exploring
the concept of scale-invariant systems. A linear scale-invariant (LSI) system [Wornell
1996b] is a linear system operator S with an output that is invariant to scale changes
of the input signal. In other words, if the input is scaled by a specific scaling factor,
the output of the system will also be scaled by the same amount. Thus,

                                          S[x(t/a)] = y(t/a)                                          (7.217)

for any constant a > 0. Observe that we have given up time invariance for scale
invariance. We can no longer describe the input/output relationship using the
convolution integral as in Equation 7.213. However, the fact that linearity is still
preserved lets us write



                                y   (t)     =   jg   (t,   r)    x   (r)   dv                         (7.218)
266   Advanced Topics

      where g(t, r) is called the system kernel. It is a two-dimensional function character-
      izing linear, time-varying system. As described by Wornell [1996b], the necessary
      and sufficient condition for a kernel g(t, r) to correspond to an LSI system is that it
      satisfies

                                                g(t, t) = ag(at, at).                     (7.219)

      One possible way of ensuring Equation 7.219 is to have

                                                  ..   .           九（t/ t)
                                                 gV! I) =                                 (7.220)
                                                                         t


      where r 尹 0. At each instance of r, g(t, r) is actually a scaled (by a factor of r)
      version of the same one-dimensional function h(t). This provides a simple and
      convenient way of constructing a two-dimensional kernel for the continuous LSI
      system from an arbitrary one-dimensional function.
        The output of the system is given by


                                          y(t) = ／乙(t)h帥）竺                                (7.221)
                                                     J- 以）                            1



      or, by a change of variables,



                                      y   (t)    =   J:  x   (t/    r)       h(t) r
                                                                                 츠.
                                                                                          (7.222)


      If the input is a random process X(t), the autocorrelation function of the output
       Y(t) is

                        Ry(t, t') = E[ Y(t)Y(t')]


                                 = E[f X(r)h(t/r)竺 f, X(r')h(t'/r')罕］                     (7.223)

                                 = f j E[X(t)X(v')]h(t/r )h(t'/r')drdt
                                                                    tn '
                                 =f j
                                  /,/,,mm:'
                                       R (t, r')）』（!
                                                 h(t/r)h(t
                                                    /:)*(!'/:/)
                                                           /r)dtdr'
        Let us now provide a definition of self-similarity of signals across scales. Let x (t)
      be a deterministic signal with the property that

                                                 兀（t) = 口-I／工（口t)                         (7.224)
                                                                        The Sca勿g（功帥力幻n and Se邱枷化小igna台    267

or, equivalently,
                                            工（t/a) ＝口-I／工（r)                                     (7.225)

for a > 0. Such a signal is said to be self-similar. In particular, it is said to be a
homogeneous signal of degree H. A random process X(t) is statistically self-similar
in the wide sense if its mean M (1) and autocorrelation R (t, s) are homogeneous:

                             Mx(t) 三 E[X(t)] = a卞"Mx(at)
                                                                                                 (7.226)
                      RX(t, s) 드 E[ X(t)X(s)] = a2月Rx(at, as).

  From Equations 7.221 and 7.223 it is easy to verify that the continuous LSI system
has the following properties:

    1If the input is a homogeneous function with degree H, the output of the
     system will also be a homogeneous function with degree H.
    1If the input is statistically self-similar with degree H, the output will also be
     statistically self-similar with degree H.

Therefore, a continuous LSI system produces a self-similar output if the input signal
is self-similar. Thus, LSI systems can be used to model natural phenomena that
exhibit self-similar behavior.
Example 7.6
     Let W(t) be zero-mean white noise with autocorrelation function R(r) = Na (r). We
     have R(r, s) = NS(t - s) and R(at, as) = N8(a(t - s)). Equation 7.226 is satisfied by
     R(t, s) and R(at, as) with H = -1/2. This is verified by inte으rating the two functions
     wun respect to r ano s.                                                             口

   By virtue of these properties, it follows that by passing W(t) through a continuous
LSI system, we are able to generate a self-similar random process. The following is
a related theorem.
   Theorem: If the input to a continuous LSI syste刃i is zero-mean white noise, the output
of the system is nonstationary and statistically self-similar.
   Proof: According to Equation 7.223, because the input has the autocorrelation
function

                                            Rx(t, t') = 8(t - t')                                (7.227)

the autocorrelation function of the output is


                    Ry(t,t') = f f,3(r - t')h(t/drr)h(t'/r')drdt'                                (7.228)
                                                         h(t
                                                                        ')
                              =        (h
                                              (t/   r)         '/   r
                                  Jr
268   Advanced Tap/cs

      As R (t, t') is, in general, dependent on both t and t' and not on t - t' alone, the
      output signal is nonstationary. Also, we have


                             사（U.
                             Ry        (t/         a,        ,   t
                                                                 !'/   '/        a)
                                                                                 .)        =
                                                                                           =       f
                                                                                                   /，   》［!
                                                                                                        /i[        t/             (ar)]-1.
                                                                                                                           :)］』［7 (.7)
                                                                                                                         (at)]h[
                                                                                                                        /(.      t   '/
                                                                                                                                     '/]dr
                                                                                                                                                              (7.229)


      By a change of variable with r' = ar, the integral becomes



                                  Ry         (t/        a,             t    '/        a)       =        a     f,        h(t/r ') h(t      '/   r ')
                                                                                                                                                  )   dr7 '   (7.230)
                                                                                               = aRy(t, t').


      Thus the output is statistically self-similar with H = -1/2.



      7.10.3 Scaling in Discrete Time
      Generally the scaling (again, we mean temporal scaling and not amplitude scaling)
      operation of a discrete-time signal x(n) by an arbitrary factor is not well defined.
      It is difficult to obtain an interpretation of scaling in the discrete-time domain that
      is as unambiguous as that in the continuous-time domain. Operations such as
      upsampling, interpolation, downsampling, and fractional sampling rate alteration
      [Vaidyanathan 19921 can have a scaling interpretation. However, such operations
      cannot handle all possible scaling factors. We present here a different approach
      [Zhao and Rao 1997] to discrete-time scaling that can handle continuous scaling fac-
      tors. Based on the fact that scaling operations in continuous time are well defined,
      we define the discrete-time scaling operation in a way that effectively amounts to
      converting x (n) into a continuous-time signal through invertible mapping, applying
      the scaling operation to the continuous-time signal, and finally inverse transform-
      ing the signal back to the discrete-time domain. The actual definition is based on
      operations in the frequency domain.
          Let f (t) be a continuous-time signal and F(Q) be its Fourier transform:



                                             /(!)｝丁노加_jQtdt
                                       F( )＝下｛                                                                                                                (7.231)
      where -以）< 52 <+的. If f (t) is scaled by a (a > 0), its Fourier transform becomes


                                                                            下｛f (t/a月 = 口F（口52)                                                               (7.232)
                                                       了he Sc에ng Ope向ion and Se肛針T)徊rS切10台    269


        工（n)            X(w)
                                        scale by
                                                   口；Y(n52)   口X[f '（口／(w))I
               Dii- !          I        口> 0



    Figure 7.13 Block diagram of the discrete-time, continuous scaling operation.



-的 < 52 < +0工 Thus, for a continuous-time signal, a scaling in time can be
accomplished in principle by a frequency scaling of its Fourier transform in the
opposite direction along with an amplitude scaling. Now, consider a discrete-time
sequence x(n) with a Fourier transform


                                   X(w）三g{x(n)} =＞二工（n)eU' " 1                      (7.233)


The function X(cv) is 2兀-periodic. If we try to define a discrete-time scali名 oper-
ation by adapting Equation 7.232 to Equation 7.233, it will only work for integer
values of a because of the 2兀-periodicity requirement on the Fourier transform of
a discrete-time signal. This corresponds to upsampling the discrete-time signal by
an integer factor of a. The frequency interval -Jr 5 cv 5 兀 is usually specified as
a representation of the discrete-time frequency spectrum. We define a continuous
scaling of a discrete-time signal [Zhao and Rao 1997] by first mapping the discrete-
time signal uniquely to a continuous-time signal, performing the dilation on this
continuous-time signal, and then mapping it back to a discrete-time signal as follows
(see Figure 7.13):


 1. Given is a discrete-time signal x(n) with (the 27r-periodic) Fourier transform
    X(w).

 2. Map the principal interval cv E [-ir, 兀］ to continuous frequency 2 (the real line)
    through an invertible transformation c = f (w). The function f is called the
    凹arping／뇨口ict幻n.

 3. Dilate Y(52) 드 X(fH1(52)) by the required dilation factor a to form Ya(c) 三
    1미y(n52).

 4. Form 兀佃）三三 }2(/ [n)]).

 5. The sequence Xa (n) resulting from the inverse Fourier transformation of Xa佃)
    is the continuous dilation of x(n) by factor a


                                     Xa(fl) = agH1(X[fH' (af (w))l}.                (7.234)
270   Ad比nced 了아沈S

            Some examples of f (w) include

             . Bilinear transform: 됴2 = f (cv) = 2 tan(co/2)

                w-reciprocal trallSfOrnl:
             .1 m-reCiPrOCal transform: Q 52 = f/(n)
                                                  (cv) -

             · Log-based transform: c = f (w) = sgn(cv) In (금可)

         In addition, there are other properties of the discrete-time continuous scale op-
      erator. Let Sa[x(fl)] denote the dilation by factor a of the sequence x(n) using the
      discrete-time, continuous scaling operator that we just defined. Based on this, the
      following properties hold true:

       I.
             S口 is a linear operator; that is, ＆佃xl(n) + a2n2(n)) = a18口｛工1(n)) + 口2＄口｛工2(n))
             幻r any al 尹 0 and a2 尹 0.
       2.
             Sa (a ；亡 1) is a time-varying operator. A shift n in the input sequence will
             not produce an output shifted by the same amount; that is, Sa {x (n - n') } ;E
             y(n - n') when y(n) = 5O(x(n)}. This is due to the time-varying property of the
             continuous-time scaling operation.
       3. Si{x(n)} = x(n), as is to be expected. This corresponds to the nonscaling case.
          The input sequence simply reproduces itself.
       4. The inverse operator S;1(x (n)) = Si/a (x (n) } is also a discrete-time scaling oper-
          ation with parameter 1/a. This is also what we would expect.
       5. Commutativity:

                                    Sa{Sb{工(n)}) = SbtS뇨｛工（n)}) == Sab｛工（n月．           (7.235)

       6. If the input discrete-time Fourier spectrum in the main period E-7r, 兀I is a
          function of f (w); that is,

                                                  X(co) = T[f (w)]                     (7.236)

             for some T(x) that satisfies

                                                 T(cv) = C(a) T(x)                     (7.237)

             where C(a) is a function of a, then the system output has the following spec-
             trum:

                                             昆佯((功｝ == 口C（口）X(cv)                      (7.238)
                                                            The Sc에四 O口era加n andS帥Sim相r的n이b    271


w E [-ir, 兀]. Property 6 provides some interesting insights into the discrete-time
scaling operation. It implies that if the inverse Fourier transform of the function
T[ f (w)] exists, the corresponding time sequence represents an eigenfunction of the
system with aC(a) as the eigenvalue. As an example, if

                                           T(w') = (w')"                             (7.239)

for some real r, then C(a) = ar, and

                              X (w) = T[ f (w)} = [f (w)]T.                          (7.240)


7.10.4 Discrete-Time LSI Systems

We construct discrete-time linear scale-invariant systems using the continuous-time
definition in Equation 7.222 as a guide. Equation 7.222 shows that the output of
the LSI system is obtained by integrating dilations of the input x (t) by r along with
the weighting provided by h(r). Fourier transforming both sides of Equation 7.222
with respect to t we have


                                   (O) =                  h(r)                       (7.241)
                                                                            dr.
                                                                     (tO)
                                                                 X
                                            f:
                               7
                                                 -   。O



In Equation 7.241 the dilation is now expressed in the frequency domain. Given a
sequence h (n) we construct a discrete-time LSI system by having

                                                     的

                                    Y(w) =＞二 h(k)Xk(w)                               (7.242)
                                                     k=1


where Y(w) = Q[y(n)] is the Fourier transform of the output sequence, h(n) = 0
for n < 1, and Xk(w) is the Fourier transform of SkEx(n)l. The system so defined is
linear. It is also scale invariant in the sense that if y(n) is the output with a sequence
x(n) as input, then the output corresponding to the input Sa[x(n)] is Sa[y(n)]. The
operator Sa lets us define self-similarity for the discrete-time case. A deterministic
signal x(n) is self-similar or homogeneous of degree H if

                                    ＆田미H口＋x(n).                                      (7.243)

For a random sequence X(n), self-similarity of degree H in the wide sense is de-
fined as

                              SaEEtX(fl)I] = ae"E(X(n)}                              (7.244)
272    Advanced Topics




              Figure 7.14 System diagram of the discrete-time LSI system



      and


                              ＆陌佯佃X(k月］ = aH2月E(X(n) X(k)}                           (7.245)

      where Sa[x(m, n)] for a two-dimensional sequence x(m, n) is defined as the dila-
      tion of both the m and n coordinates by a using a mapping of discrete-to-analog
      frequencies as for the one-dimensional case.
         Figure 7.14 shows the block diagram of a discrete-time LSI system. In Figures 7.15
      through 7.17 we show examples of discrete-time, deterministic, self-similar functions
      that are derived from the discrete-time Fourier spectrum for various types
                                                                                   of 1 (w),
      namely the bilinear, 1/w-based and log-based transforms, respectively. In each case,
      the function generated is the inverse Fourier transform of



                                   Y(w）十썲：：岩                                        (7.246)


      By Equation 7.240, these functions all serve as eigenfunctions of our discrete-time
      scaling operator and hence are eigenfunctions of the discrete-time LSI system.
        It is shown by Zhao and Rao [19971 that a stationary random signal X(n) with
      power spectrum density of the form


                                            . .       If (w)I'
                                                                                    (7.247)
                                         rxlw)    =
                                                      If   '
                                                               (w)
                                                                     I
                                                 The S以物g（加erc川on and Se爪S加iIar S切向5              273


          1.u

          0.5

          0.0      }H                        人w小W小                                  듣
     -0. 5
     _1 Cl                                                                                  (A)
                   0              50                     100                        150
                                                                              n 斗




      I .D
      1.0 三                                  1                                      ;
      0.5
      0.0
     -0.5
                   三山mW蜘叫M' 加m的mmWm                                                 j
         0 三                             1                                          三
                                                                                            (B)
      -   1.
      寸   1 <

                   0              50                     100                        11.50
                                                                              n 斗




          1>
                   L                         1                                      j
               .




          1.0


                   弘W쌔가／//////////////：』』1，
       0.5
       0.0
      -0.5
                                         了I/Il"／付N!싸机mW,WA                              j
        0 三＋                             1                                          三
     1 1c                                                                                   (C)
          1.
      -
                   0              50                     100                        150
                                                                              n +



   Figure 7.15 Eigenfunctions of the discrete-time scaling system with respect to bilinear
               的nsform. These are 卄me sequences \A／汁h 네screte十me 比urier S口ectra
               that are sgn(w)(2tan(I끼/2))r for -1 < r < 1. (A) r = 0.1 . (B) r = 0.5. (C)
               r = 0.7.


is a statistically self-similar signal of degree H = -(r + 1)/2. Figure 7.18 shows
such a random signal generated using f (w) of the bilinear transform for different
values of r.
274   Advanced／아比S




                                                                                                三
                     I .U




                         !
                     0.5
                     0.0
               -0.5
                in
                                  m니小艸小
                     1 11J                                                                                  (A)
                             ()           50                     100                                1 10    「       '




                                                                                       n        -




                 1.1.1
                             二                      1                                                二

                0.5


           -0.5
                0.0
                             如娜MMm加川川'jM mwAwmA                                                     三
            in               二                  1                                                   二
                                                                                                            (WI
                             0            50                     100                                1=.10   「   '




                                                                                       n +




             l >     .



             1.0 三                                  1                                               三
            0.5
            0.0
           -0.5
                             抑mm幽W幽m:＝加幽빠娜M싸脚M                                                      -:
           -
               0 三
                1.
                                               1                                                    二
                ic
                                                                                                            (C)
                             0            50                     100                                150
                                                                                       n   口＋
        Figure 7.16 Eigenfunctions of the discrete-time scaling system with respect to
                    1/w-based transform. These are time sequences with discrete-time Fourier
                    spectra that are sgn(w)(lwl/(兀 니wl))' for -1 < r < 1 . (A) r = 0.1. (B) r = 0.5.
                    (C) r = 0.7.
                                           The Scaling Operation and Self-Similar Signals     275




   r노 r
   tJJJ
              三                     1                                          三
   0.4
   0.2
   0.0
  -0.2
           三小如m叫’ 加枷小小如                                                    三
  -0.4                                                                              (A)
    r\ <                                                                            \ /
  1口1JaJ
           0                 50                    100                        150
                                                                         n+


    1l <
    u.u



                                                                               j
   0.4
   0.2
   0.0        和m山W叫小加mmWm
  -0.2
  -0.4                                                                               (Bi
    rl <
              0              50                     100                        150
                                                                         n +




              如빼쌔吃m싸-쌔 j
     1.u
     0.5
     0.0
  -0.5
     in
                                                                                     r（기
                                                                                     \ 11 /
    1 J 11J

              0              50                     100                    150
                                                                         n-누


디gure 7.17 日genfunctions of the 비screte-tin冶 $C（에ng S吟怡m with res口ect to a
           log-based transform. These are time sequences with discrete-time Fourier
           spectr이h아are sg如山nG듦）] ' 幻r「 > -1· (A)『 =0.5. (B)「 = 1.0.
           (C) r = 2.0.
276   Advanced Top/cs




                             月
                            HP
                            2

                   -2
                            0
                                 如州娜刪岫枷岫娜娜MM州蜘                                                        j
                  =m늬
                            月
                                                                                                            (A)
                                 0    100   200   300         400         500                        6()0
                                                                                    n            -




                        月
                        니




                                 亘빠恤肺m蜘沁빠布叫州州加
                        2

                 -2
                        0
                            J
                                                                                                     三      (B)
                                 ()   100   200
                 -&t
                                                  300         400         500                        600
                                                                                    n        -




                            J
                        '

                        2

             -2
                        0        押如때螂啼州小們艸州加加枷                                                       三
                                                                                                            (C)
                                 0    100   200
             U斗
                                                  300         400         500                        6()0
                                                                                   n        ->
                        月
                        냐

                        2

            -2
                        0        如fr甲W們脚小伊伽W幽艸m加卜                                                    j
            1戶斗
                        月
                                                                                                            (D)
                                 0    100   200   300         400         500                        600
                                                                                   n    -             -




         Figure 7.18 Examples of discrete-time, stationary, self-similar random processes for
                     the case of bilinear transform. (A) Zero-mean人hite noise. (B) r = 1.8,
                     H = -1.4. (C) r = 0.8, H == -0.9. (D) r = -0.2, H = -0.4.
                                               了／伯 Sc에ng Operat跏 and Se爪S/rn向 Signa台           277




            4
           1+


           2
           0
           2
                  k和，싸W뇨싸m汕小／甲m／끼나加小小                                              三
                                                                                         (E)
      -
            月
           'f

                  0    100   200         300         400         500               600
                                                                          n   -




                  如m뇨岫凸뇨mmm小 三
           i+


           2
           0
           2
                                                                                         (F)
      -
            月
           1+

                  0    100   200         300         400         500               600
                                                                          n   m+
          J 'J



          卜d/ m뇨小小小MH                                                              三
            5
            0
            5
                                                                                         (G)
      -
          1n
  -       lu
                  0    100   200         300          400        500               600
                                                                          n +




                  i/                                                               j
          (+U




                               /\
    20
     0
   -20
           月 r\                                                                          (H)
          'PU

                  0    100   200         300          400        500               600
                                                                          n +




Figure 7.18 (continued) (E) r = -0.8, H = -0.1. (F) r = -1.2, H =0.1. (G) r = -1.8,
            H = 0.4, (H) r = -2.8, H = 0으
                             APPENDIX                A


                 Fundamentals of
                 Multirate Systems


In this book, multirate filter banks have been studied in the specialized context of
implementing DTWTs. The processes of downsampling and upsampling have been
restricted to the special case of a factor of two. This appendix describes the more
general case of downsampling and upsampling by an integer factor. It also de-
scribes the so-called noble identities that have been used in Chapters 3 through 5 to
determine equivalents of several multirate systems, and in the construction of bases
corresponding to DTWT decompositions. A detailed exposition and mathematical
derivations are given in Crochiere and Rabiner [1983] and Vaidyanathan [19921.


A.1 The Downsampler
The downsampier is also called the sampling rate compressor and the subsampier. Fig-
ure A.1 shows an M-fold downsampler. It takes an input sequence x (n) and pro-
duces an output sequence

                                     y(n) = x(Mn)                              (A.1)

where M is an integer. In other words, a downsampler by M retains only those
samples of x(n) that occur at times that are multiples of M. Figure A.2 shows how
the downsampler acts on a sequence for the case of M = 2. In the transform domain,




        Figure A.1 An /1i-foId downsampler.


                                          279
280    Fundam帥幻台아Mt肋아eS四帥沾




               Figure A.2 Demonstration of a downsampler for the case of M =2.
                          (A) Original sequence, (B) The downsampled sequence. Note
                          that the samples with solid dots are retained.


      Y(z), the z-transform of the output of the downsampler, can be written as


                                                                                        (A.2)
                                     小諱！
                                                          (zh1MWo)
      where w = e_J2兀1M. In terms of the discrete-time Fourier transform, Equation A.2
      can be written as

                                         I 望二？
                                 Y化力' = 1 . > . X((w- 2兀k) /M).                        (A.3)
                                  "     AU'-
                                        4 "1 k=O' "      ,,
      From Equations A.2 and A.3 the downsampling process can be described as follows
      in the frequency domain. First, X(w) is stretched by a factor of M to obtain X(w/M).
      This stretched version is now shifted uniformly by successive M -1 multiples of 27r.
      These M - 1-shifted versions are added to X(w/M) to give a 27v-periodic spectrum.
      Fi昏lre A.3 illustrates these steps for the case of M = 2. Note that downsampling
      gives rise to aliasing unless the signal is sufficiently bandlimited.


      A.2 The Upsampler
      The upsampier is also called a sampling rate expander or simply an expander. Figure A.4
      shows an L-fold upsampler. It takes an input sequence x(n) and produces an output
      sequence

                        . .    I x (nIL)   if n is an integer multiple of L
                       只fl) = 1 r\
                              I u
                                            .l     .
                                           O[1lerVVlSe1
                                                                     V                 (A.4)
                                                                           The U尸sari갸)Ier   281




Figure A.3 Effect of downsampling on the spectrum of the sequence. (A) Original sequence
           spectrum. (B) Spectrum of the sequence after being downsampled by two.



Thus, upsampling by a factor of L involves inserting L - I zeros between consec-
utive samples of the input sequence. The process of upsampling is demonstrated
in Figure A.5 for L = 2. In the z-transform domain, the relation between x (n) and
y(n is given by

                                     Y(z) = X(z').                                  (A.5)

In terms of the discrete-time Fourier transform, Equation A.5 can be written as

                                    Y(w) = X(Lw).                                   (A.6)

Thus, Y (w) is an L-fold-compressed version of X (w) and it contains L-compressed
copies of X(w). These are called images. Figure A.6 shows the spectrum of a signal
upsampled by a factor of three.



                                           L
                           工（n)                          y(n)


        Figure A.4 An L-fold upsampler or expander.
282    Fundam帥幻台 of A仙月rote S,計帥衿




                                                  1
                                                                                          工（n)


                            I
                                 T
                                        ?
                                            3
                                                         !                                  >    7i
                            0   1      2          4      5
                                             I,
                                                              (A)




                                                                             I
                                                                                         y (n)



                                                  I                 6
                                                                                     f     >

                                                                1
                                                                                 S               .
                            0   1      2    3     4      5              S7
                                                                             8   9   10


                                                              (B)

               Figure A.5 Demonstration of upsampling for the case of L = 2. (A) Original
                          sequence. (B) Upsampled sequence.




                                                             X(w)




                                                             Y(w)




                    /\/＼入八八八／\
                     -2,r            -jr -2r/3 -yr/3 0        ,r/3 2ir/3 7r                2ir


      Figure A.6 Effect of upsampling on the spectrum of the original sequence. (A) Spectrum of
                 the original sequence. (B) Spectrum of the sequence upsampled by a factor of
                 three.



      A.3 Noble Identities
      The noble identities are useful in simplifying and interpreting multirate systems.
      Specifically, they help us describe the effect of moving dowsamplers or upsamplers
      across systems or transfer functions. We have used these identities in Chapters 3
                                                                                                          N야)Ie Iden桁les       283



              M                                                                                        M
                                                    (n)
                                                                           兀（n)                               Y2(7)
                          G(w)                                                         G(Mw)
                                              y
                         (A)                                                               (B)

                                                                                       L
                                                  y3(fl)                    x(n)                              y4(fl)
                  G(w)                                                                            G(Lw)
     '늬   「
  Figure A.7 (A-D) The noble identities.



through 5 to come up with equivalent filter banks corresponding to tree-structured
systems and hence basis functions for these systems. The noble identities are best
explained with the help of a figure. Let G(w) be a rational function. Then Figures
A.7A and A.7B are equivalent, and Figures A.7C and A.7D are equivalent. We now
prove these two equivalencies.
   Consider Figure A.7A. From Equation A.3, the output of the downsampler is



                                                                     (（小27r) /M)                                       (A.7)
                                        M 凡＝=u
                                        ！뿌x                                        .



                                                          {-                 "




Then the output of G(w) will be


                                       I      乍二？
                               Y1(w) = 而 G(w) j X((w - 2ir)/M).                                                        (A.8)
                                                                     k=O



Now consider Figure A.7B. The input to the downsampler is G(Mw)X(w). The
output of the downsampler Y2(w) is then given by




                  「小            諱G                             (（佃如M)/M)如-                 2ir)   /川                   (A.9)

                           = 去G(w）브X(（小2r)/M)
                                 i ri
                                                               k=O



where we have made use of the 27r periodicity of G(w). Note that Equation A.9 is
the same as Equation A.8. This proves the first noble identity.
284   反／ndamenta台 of,.'次咐／I.,計e Systems


        To prove the second noble identity, consider Figure A.7C. The input to the up-
      sampler is G(w) X(w). The output of the upsampler is then

                                          Y3(w) = G(Lw) X (Lw).                (A.10)

      Now consider Figure A.7D. The output of the upsampler will be X(Lw) and the
      output of the system therefore will be Y4(w) = X(Lw)G(Lw), which is the same as
      Equation A.10. This proves the second noble identity.
                               APPENDIX                 B


                  Linear Algebra
                and Vector Spaces


A few concepts in linear algebra and vector spaces relevant to the material in the
text are reviewed here. More details can be obtained from any standard linear
algebra book such as Anton [1981], Finkbeiner [1986], Hoffman and Kunze [1971],
and Strang [1988].


B.1 Brief Review of Vector Spaces
A vector space V is a set that consists of objects called vectors. Let u, v, and w be
vectors in V. The following axioms then define a vector space:

 1.   it u and v are objects in V, tnen U + V is also an ooject in V.

 2.
      Commutativity: u + v = v + u.

 3.
      Associativity: u + (v + w) = (v + u) + w.

 4.   Existence of a zero vector: There is a unique vector 0 in V such that u + 0 = u.

 5.
      Existence of an additive inverse: Each vector u has an additive inverse -u such
      that u + (- u) = (- u) + u = 0.

 6.   If a is a scalar and u is any vector in V, then au is also in V.
 7.
      Distributive property: a(u + v) = au + av.
 8.
      Given two scalars a and b, we have (a + b)u = au + bu.

 9. a(bu) = (ab)u.
10. lu= u.

   It is easy to see that R3 satisfies all these axioms and hence is a vector space. The
addition of two points in R3 also lies in R3. Similarly, the result of scalar multiplica-
tion also belongs to R3. Thus, R3 is said to be closed under the operations of addition

                                           285
286    Linear Algebra and Vector Spaces

       and scalar multiplication and hence form a vector space. Other examples of vector
       spaces are the space of all continuous functions and the space of all polynomials of
       degree n.


       B.i .1 Vector Subspace

      A subset W of a vector space V is called a vector subspace of V if it is a vector
      space in its own right under the operations of addition and scalar multiplication as
      defined on V. An example of a vector subspace is the x-y plane in R3. The vectors
      in this plane have the general form p = (x, y, 0). It is easy to see that these vectors
      satisfy the axioms of a vector space under the operations of addition and scalar
      multiplication defined on R3.


      Li .2 Linear Independence and Bases
      A vector v in V is said to be a linear combination of a set of vectors v1, v2. ....vll in
      V provided there exist constants a1, a2, .. . , an such that


                                              V       N
                                                      Z너
                                                       V
                                                       n   1l     놔 1


                                                                                             (B.1)


      A set of vectors v1, v2. . . . .v11 is said to be linearly dependent if there exist constants
      al, a2, .. . , a7i not all zero such that the linear combination


                                                 N
                                                 Z너
                                                  V
                                                  n        O                          =
                                                                                             (B.2)


      A set that is not linearly dependent is linearly independent. In other words, none
      of these vectors can be represented as a linear combination of the others. Thus, v1
      cannot be written as a linear combination of v2, v3. .. ..vl1; and v2 cannot be written
      as a linear combination of v1, v3. ....vt and so on.
         Linear independence is a prerequisite for a set of vectors to be a basis of a vector
      space. Another requirement is that every vector in the vector space should be
      expressible as a linear combination of members of this set. In other words, the basis
      vectors should span the vector space. Thus, if b1, b2, and so on, are the basis of a
      vector space V. then a vector v in V can be represented as


                                             V        N
                                                      Z너
                                                       n
                                                                                             (B.3)


      The number of vectors in any basis of a finite-dimensional vector space gives its
      d加wns加n.
                                                                                  Inner Product Spaces   287

   An example of basis vectors is the standard basis of R3-namely, b1 = (1, 0, 0),
b2 = (0, 1, 0), and b3 = (0, 0, 1). Another example is the set of functions 1, x2, x3,
and so on, that forms the basis for the space of all polynomials.


B.2 Inner Product Spaces
An inner product on a vector space V is a rule that associates a real number, denoted
by (u, v) with each pair of vectors u and v in V.
  The following axioms are satisfied by the inner product for all vectors u, v, and
win V:

 1. Symmetry: (u, v) = (v, u).
 2. Additivity: (u + v, w) = (u, w) + (v, w).

 3. Homogeneity: (ku, v) = k (u, v), if k is a scalar.
 4. Positivity: (v, v) > 0 and (v, v) = 0 if and only if v = 0.

   A vector space with an inner product defined on it is called an inner product space.
An example of the inner product is the dot product of the vectors in R3. Suppose we
are given two vectors, PI = (xi, Yi, ZI) and P2 = (x2, Y2, z2), in R3. The dot product
of these two vectors is defined as

                             (p1, p2) = 工l工2 + YIY2 + Zi乙2.                                     (B.4)

  Another example of an inner product space is the space of all polynomials of
degree n. If f (x) and g(x) are two polynomials in this space, then
                                                  )):
                                                        j f (x)
                                                        too
                           (/
                           (f (x)
                              (1)                  )                        dx.                 (B.
                                            (!
                                    ,              =
                                                                                                   5)
                                                                      (x)
                                            (x)
                                        8
                                        g
                                    ,
                                                                  g
                                                        -   C。


  If V is an inner product space and if u is a vector in this space, then the norm of
u denoted by HuH is defined by

                                            Hul l = (u, u)112.                                  (B.6)

Thus, the squared norm is basically an inner product of a vector with itself. In
this manner, the inner product operation induces a norm. The norm satisfies the
following properties. Let u and v be two vectors in V and let c be a constant. Then,

 1. lcuH = i가 1lull.
 2. H t工n > 0 幻ru 尹 0.
 3. Triangle inequality: llu+ vll 5 h1ul l + 巾川.
288   Linear Algebra and Vector Spaces

        Based on the definition of the norm of a vector, the distance between t사o vectors
      u and v in an inner product space is defined as

                                         d(u, v) = ilu- vil.                          (B.7)

      Note that for the space R3, this is the Euclidean distance between two vectors in that
      space. Finally, we end this section by mentioning an important inequality called
      the Cauchy-Schwarz inequality. If u and v are two vectors in an inner product space
      then the Cauchy-Schwarz inequality states that

                                         !(u, v)l < hull lvii                          (B.8)

      with equality when u = kv where k is a scalar.


      B.3 Hubert Space and Riesz Bases
      An inner product space that is complete with respect to this norm is known as
      a Hilbert space. To understand what completeness means, we need to consider
      infinite sequences of vectors v1, v2, and so on, in the vector space V. We say that
      this sequence is convergent if there is a vector v in V such that

                                             lim v71 = v.                              (B.9)

      A Cauchy sequence is one that has the property that as n 수 的, successive points
      tend to be closer together. Mathematically, we state this property as follows: Given
      e > 0 there exists a positive integer n0 such that for m, n > n0, l ivn - Vmhi < C,
      where 11.11 is the norm defined on V. A convergent sequence must be a Cauchy
      sequence [Franks 1969]. However, the converse is not true. Every Cauchy sequence
      is not necessarily convergent because the element to which the sequence tends may
      not be in V. There are certain inner product spaces where every Cauchy sequence
      does converge to a vector in that space. Such vector spaces are called complete. An
      example of a Hilbert space is the space of all square integrable functions, L2(R).
         Now consider a vector space V with basis functions b1, b2, and so on. This basis
      is said to be unconditional if it satisfies the following three conditions [Daubechies
      1992]:

       1. Let c1, c2, and so on, be real constants. If the linear combination ＞二 c,』b, is in

          V, then so is ＞二 lc ib.

       2. Let El, e2, and so on, be a sequence in which each E randomly takes a value of
          士1. Then, if the linear combination Z c,b小 in V. so is ＞二Qqbm

       3. The order in which the basis vectors are taken does not matter.
                                                              Hube片 Space and Riesz Bases    289

In a Hulbert space, the unconditional basis is also called a Riesz basis. The Riesz
basis can also be characterized by the inner product defined on V. Let v be a vector
in V. Then there exist constants a > 0 and fi < 茯） such that

                            이V下드刃他놔노帥下1                                            (B.10)

This condition is not sufficient. It is required that the basis functions also be linearly
independent. For example, the orthonormal wavelet basis described in Chapter 3
is a Riesz basis for L2(R).
                               BIBLIOGRAPHY




   Ahmed, N., T. Natrajan, and K.R. Rao. Discrete cosine transform. IEEE Transactions on
      Computers 1974;23:88-93.

米 Akansu, A.N., P. Duhamel, X. Lin, and M. de Courvifie. Orthogonal trans-multiplexers in
     communication: a review. IEEE Transactions on Signal Processing 1998;46(4):979-995.

   Akansu, A.N., and R.A. Haddad. Multiresolution signal decomposition: Transforms, subbands,
      wavelets. San Diego, CA: Academic Press, 1992.

   Aidroubi, A., and M. Unser. Sampling procedures in function spaces and asymptotic equiv-
       alence with Shannon's sampling theory. Numerical Functional Analysis and Optimization
       1994;15:1-21.

   Anton, H. El日7ientary linear algebra. New York: John Wiley and Sons, 1981.

   Apostol, T.M. Mathematical analysis. Reading, MA: Addison-Wesley, 1957.

   Arsenault, H.H., and C. April. Properties of speckle futegrated with a finite aperture and
       logarit노llically transformed. Journal of the Optical Society of America 1976;66:1160-1163.

   Bertrand, O., J. Bohorquez, and J. Pernier. Time-frequency digital ifitering based on an
       invertible wavelet transform: An application to evoked potentials. IEEE Transactions on
       Biomedical Engineering January 1994;41(1):77-88.
   Beylkin, G., R. Coifman, and V. Rokhlin. Fast wavelet transforms and numerical algorithms.
       Communications in Pure and Applied Mathe刃4atics 1991;44:141나183.

   Bingham, J.A.C. Multicarrier modulation for data transmission: an idea whose time has come.
       IEEE Communications Magazine 1990:5-14.

   Bopardikar, A.S. Speech encryption using wavelet packets. Master's thesis. Bangalore, India:
      Indian Institute of Science. 1995.

   Bopardikar, A.S., M.R. Raghuveer, and B.S. Adiga. Perfect reconstruction circular convolution
      filter banks and their application to the implementation of bandlimited discrete wavelet
      transform. In: Proceedings of the IEEE International Conference on Acoustics, Speech and
      Signal Processing. Munich: April 1997a:3665-3668.
   Bopardikar, A.S., M.R. Raghuveer, and B.S. Adiga. PRCC filter banks: Theory, implemen-
      tation and application. In: Aldroubi, A., A.F. Lamle, and M. Unser, eds. Proceedings
      of SPIE, wavelet applications in signal and image processing V. San Diego: August 199Th;
      3169:410-421.

   Brandenburg, K., and G. Stoll. ISO-MPEG-i audio: A generic standard for coding high-
       quality digital audio. Journal of Audio Engineering Society October 1994;42(10):78小792.

                                               291
292   Bib幻（7n까Thy

      Brislawn, C.M. Classification of symmetric wavelet transforms. Technical report. Los Alamos,
           NM: Los Alamos National Laboratory, 1993.

      Burrus, C.S., R.A. Gopinath, and H. Guo. Introduction to wavelets and wavelet transforms: A
          primer. Englewood Cliffs, NJ: Prentice-Hall, 1997.

      Caire, G., R.L. Grossman, and H.V. Poor. Wavelet transforms associated with finite cyclic
          groups. IEEE Transactions on Infor刃iation Theory July 1993;39(4):1157-1166.
      Calzone, S., C.C. Chuang, A. Divakaran, et al. Video compression by mean-corrected motion
          compensation of partial quadtrees. IEEE Transactions on Circuits and Systems for Video
          February 1997;7(1):86-96.

      Chapa, J.O. Matched wavelet construction and its application to target detection. PhD thesis.
         Rochester, NY: Rochester Institute of Technology, 1995.

      Chapa, J.O., and M.R. Raghuveer. Constructing wavelets from desired signal functions. In:
         Proceedings of 1994 Workshop on Information Theory and Statistics. Alexandria, VA: October
         1994.

      Chapa, J.O., and M.R. Raghuveer. Optimal matched wavelet construction and its application
         to image pattern recognition. In: Szu, H.H., ed. Proceedings of SPIE, wavelet applications
         II. Vol. 2491. April 1995:518-529.

      Chapa, J·O., and M.R. Raghuveer. Constructing MRA from desired wavelet functions. In:
         Twenty-eighth Asilo刃iar Conference on Signals, Syst臼7is and Computers. Vol. 2. Pacific Grove,
         CA: 1996a:1109-1113.

      Chapa, J.O., and M.R. Raghuveer. Matched wavelets-their cons如ction, and application to
         object detection. In: IEEE International Conference on Acoustics, Speech and Signal Processing.
         Atlanta, GA: April 1996b.

      Chui, C.K. An introduction to wavelets. San Diego: Academic Press, 1992a.

      Chui, C.K. Wavelets: A tutorial in theory and applications. San Diego: Academic Press, 1992b.

      Cohen, A., and I. Daubechies. Nonseparable bidimensional wavelet bases. Rev. Math. Thero-
         americana 1993;9(1):51-137.

      Cohen, A., I. Daubechies, and J.C. Feauveau. Biorthogonal basis of compactly supported
         wavelets. Communications in Pure and Applied Mathematics 1992;45:485-560.

      Coifman, R., and M.V. Wickerhauser. Entropy-based algorithms for best basis selection. IEEE
          Transactions on Information Theory March 1992;38(2):713-718.

      Combes, A., A. Grossmann, and P. Tchamitchian, eds. Wavelets, time-frequency methods and
         phase space. New York: Springer-Verlag, 2nd ed., 1991.
      Cooklev, T., A. Nishihara, M. Kato, and M. Sablatash. Two-channel multifilter ba川Ks and
         multiwavelets. In: Proceedings of IEEE International Conference on Acoustics, Speech, and
         Signal Processing. Atlanta: May 1996:2769-2772.

      Cooklev, T., A. Nishihara, and M. Sablatash. Regular orthonormal and biorthogonal wavelet
         filters. Signal Processing March 1997;57(2):121-137.
                                                                                  Bibliography    293

Couch II, L.W. Digital and analog communication systems. Upper Saddle River, NJ: Prentice-
   Hall, 1997.

Cover, T.M., and J.A. Thomas. Elements of information theory. New York: Wiley Interscience,
   1991.

Crilly, A.J., R.A. Earnshaw, and H. Jones. Fractals and chaos. New York: Springer-Verlag,
     1991.

Crochiere, R.E., and L.R. Rabiner. Multirate digital signal processing. Englewood Cliffs, NJ:
    Prentice-Hall, 1983.

Dainty, J.C., ed. Speckle and related phenomena. New York: Springer-Verlag, 1984.

Daubechies, I. Orthonormal bases of compactly supported wavelets. Communications in Pure
   and Applied Mathematics November 1988;41:909-996.

Daubechies, I. The wavelet transform, time frequency localization and signal analysis. IEEE
    Transactions on Information Theory 1990;36(5):961-1005.

Daubechies, I. Ten lectures on wavelets. CBMS series. Philadelphia: SIAM, 1992.

Daubechies, I. Where do wavelets come from? A personal point of view. Proceedings of the
   IEEE 1996;84(4):510-513. [Special issue on wavelets.]

Daubechies, I., and J.C. Lagarias. Two-scale difference equations I. Existence and global
   regularity of solutions. SIA入4 Journal of Mathematical Analysis 1991;22:1388-1410.

Daubechies, I., and J.C. Lagarias. Two-scale difference equations II. Local regularity, infi-
   nite products of matrices and fractals. SIAM Journal of Mathematical Analysis July 1992;
   24(24):1031小1079.

Daubechies, I., S.G. Mallat, and A. Willsky, eds. Special issue on wavelets and multiresolution
   analysis. IEEE Transactions on Information Theory March 1992;32.

Daugman, J. Neural image processing strategies applied in real-time pattern recognition.
   Real-Time Imaging 1997;3:157-171.

Deriche, M., and A. Tewfik. Maximum likelihood estimation of the parameters of discrete
    fractionally differenced Gaussian noise process. IEEE Transactions on Signal Processing
    October 1993a;41:2977-2989.

Deriche, M., and A. Tewfik. Signal modeling with filtered discrete fractional noise processes.
    IEEE Transactions on Signal Processing September 1993b;41(9):2839-2849.

Divakaran, A., and W.A. Pearlman. A new family of orthonormal wavelet bases. In: Pro-
    ceedings of the IEEE-SP International Symposium Time-Frequency and Time-Scale Analysis.
    Victoria, BC: October 1992:331-334.

Divakaran, A., and W.A. Pearlman. Information-theoretic performance of quadrature mirror
    filters. IEEE Transactions on Info力7iation Theory November 1995;41(6):2094-2100.

Divakaran, A., and W.A. Pearlman. A closed form expression for an efficient class of quadra-
    ture mirror filters and its FIR approximation. IEEE Transactions on Circuits and Systems
    끄: Analog and Digital Signal Processing March 1996;43(3):207-219.
294   Bibliography

      Donoho, D.L. De-noising via soft thresholding. Technical report 409. Stanford, CA: Department
         of Statistics, Stanford University, November 1992.

      Donoho, D.L. Unconditional bases are optimal bases for data compression and for statistical
         estimation. Applied and Computational Har刃ionic Analysis December 1993;1(1):100-115.
      Donoho, D.L., and I.M. Johnstone. Ideal spatial adaptation via wavelet shrin初ge. Technical report
         400. Stanford, CA: Department of Statistics, Stanford University, November 1992.
      Duhamel, P., P. Flandrin, T. Nishitani, A.H. Tewfik, and M. Vetterli, eds. Special issue on
         wavelets and filter banks. IEEE Transactions on Signal Processing December 1993;41,
      Feder, J. Fractals. New York: Plenum Press, 1988.
      Finkbeiner II, D.T. Introduction to matrices and linear transformations. New York: W.H. Freeman,
          1986.
      Franks, L.E. Signal theory. Englewood Cliffs, NJ: Prentice-Hall, 1969.
      Gandhi, P.P. Continuous-time si앉lal analysis using wavelets. In: Szu, H., ed. SPIE Interna-
         tional symposium on Aerospace/Defense Sensing and Dual Use Photonics (Wavelet Applications
         for Dual Use). Vol. 2491. Orlando, 瓦, April 1995a:968-979.
      Gandhi, P.P. Wavelet sampling of continuous-time signals. In: IEEE 1995 Conference on
         Information Sciences and Syst臼7is. Baltimore, March 1995b.
      Gandhi, P.P. JPEG-based image compression for low bit rate coding. In: Stevenson, R.L.,
         A.!. Dorukarev, and T.R. Gardos, eds. Proceeding of the SPIE, Still-image compression II.
         Vol. 2669. San Jose, January 1996:82-94.
      Gandhi, P.P., S.S. Rao, and R.S. Pappu. Wavelets for baseband coding of waveforms. In:
         IEEE GLOBECOM. San Francisco, November-December 1994:363-367.

      Gersho, A., and R.M. Gray. Vector quantization and signal compression. Boston, MA: Kiuwer
          Academic Publishers, 1992.

      Gracias, S.D. Channel equalization using wavelet packets (master's thesis). Bangalore, India:
          Indian Institute of Science, 1994.
      Gradshteyn, I.S., and I.M. Ryzhik. Table of integrals, series, and products. San Diego: Academic
         Press, 1980.

      Grossman, A., and J. Morlet. Decompositions of hardy functions into square integrable
          wavelets of constant shape. SIAM Journal of Mathematical Analysis July 1984;15(4):723-
          736.

      Guo, H., J.E. Odegard, M. Lang, R.A. Gopinath, I.W. Selesnick, and C.S. Burrus. Wavelet
         based speckle reduction with applications to SAR based ATD/R. In: Proceedings of 1st
         International Conference on Image Processing. Vol. 1. Austin, TX, November 1994:75-79.
      Hastings, H.M., and C. Sugihara. Fractals: A user's guide for the natural sciences. New York:
          Ox的rd University Press, 1996.
      Herley, C. Wavelets and filter banks. PhD thesis. New York: Columbia University, 1993;
      Hernandez, E., and G. Weiss. A first course on wavelets. Boca Raton, FL: CRC Press, 1996.
                                                                                   Bibliography    295

Hoffman, K., and R. Kunze. Linear algebra. Englewood Cliffs, NJ: Prentice-Hall, 1971.

Hopper, T., C. Brislawn, and J. Bradeley. WSQ gray-scale fingerprint image compression specifi-
   cation. Washington, DC: Criminal Justice Information Services, Federal Bureau of Inves-
   tigations, February 1993.

Jayant, N.S., and P. Noll. Digital coding of waveforms. Englewood Cliffs, NJ: Prentice戶Hall,
    1984.

Jones, W.W. A unified approach to orthogonally multiplexed communications using wavelet basis
    and digital filter bank. PhD thesis. Athens, OH: Ohio University, 1994.
Jones, W.W., and J.C. Dill. The square root raised cosine wavelet and its relation to the Meyer
    functions. IEEE Transaction on Signal Processing (submitted for publication).

Jones, W.W., and J.C. Dill. An analog definition for DWMT modulation. IEEE Transaction on
    Communications (submitted for publication).

Jordan, E.C., ed. Reference data for 臼igineers: Radio, electronics, computer and communications.
    7th ed. Indianapolis, IN: Howard W. Sams, 1986.

Kaiser, G. A friendly guide to wavelets. Boston: Birkhauser, 1994.
Karisson, C., and M. Vetterli. Extension of 伯aite length signals for sub-band coding. Signal
    Processing June 1989;17(2):161-168.
Keshner, M.S. 1/f noise. Proceedings of the IEEE March 1982;70(3):212-218.
Kovacevic, J. Filter banks and wavelets: Extensions and applications. PhD thesis. New York, NY:
   Center for Telecommunications Research, Columbia University, 1991.

Kovacevic, J., and I. Daubechies, eds. Special issue on wavelets. Proceedings of IEEE March
   1992;84.

Kovacevic, J., and M. Vetterli. Nonseparable multidimensional perfect reconstruction filter
   banks and wavelet bases for R". IEEE Transactions on Infor刃iation Theory March 1992;
    38(2):533-555.

Kunt, M., ed. Special issue on digital television. Part 1: Technology. Proceedings of the IEEE
   June 1995a;83.
Kunt, M., ed. Special issue on digital television. Part 2: Hardware and applications. Proceed-
   ings of the IEEE July 1995b;83.
Li, H., B.S. Manjunath, and S.K. Mitra. Multi-sensor image fusion using the wavelet transform.
     In: Proceedings of IEEE Inter刃ational Conference on Image Processing. Austin, TX, November
     1994:51-55.
Li, H., B.S. Manjunath, and S.K. Mitra. Multisensor image fusion using the wavelet transform.
     Graphical Models and Image Processing May 1995;57:235-245.
Mallat, S.C. Multiresolution approximations and wavelet orthonormal bases of L2(R). Trans-
    actions of American Mathematical Society 1989a;315:69-87.
Mallat, S.C. A theory of multiresolution signal decomposition: The wavelet representation.
    IEEE Transactions on Pattern Analysis and Machine Intelligence July 1989b;11:674七93.
296   Bibliography

      Mallat, S.G., and W.L. Hwang. Singularity detection and processing with wavelets. IEEE
          Transactions on Information Theory March 1992;37:617-643.

      Mandeibrot, B.B., and J.W. Van Ness. Fractional Brownian motions, fractional noises and
         applications. SIA入i Review October 1968;10(4):422-437.

      Marr, D.A. Vision: A computational investigation into the human r刃resentation and processing of
         仇51在11 呵0力nation. New York: Freeman, 1982.
      Marr, D.A., and E. Hildreth. Theory of edge detection. Proceedings of the Royal Society of
         London, B 1980;207:187-217.

      Martucci, S.A., I. Sodagar, T. Chiang, and Y.-Q. Zhang. A zerotree wavelet video coder. IEEE
          Transactions on Circuits and Syst臼7is for Video February 1997;7(1):109-118. (Special issue
          on 入PEG-4. See also other papers in the issue.)

      Meyer, Y. Wavelets and operators. New York: Cambridge University Press, 1993a. Translation
         of Ondellettes et operatuers. Paris: Hermann, 1990.

      Meyer, Y. Wavelets: Algorithm and applications. Philadelphia: SIAM, 1993b.
      Mintzer, F. Filters for distortion-free two-band multirate filter banks. IEEE Transactions on
          Acoustics, Speech and Signal Processing June 1985;33:62今630.

      Noll, P. Wideband speech and audio coding. IEEE Communications Magazine November 1993;
          31(11):34-44.

      Oppenheim, A.V., and R.W. Schafer. Discrete-time signal processing. Englewood Cliffs, NJ:
         Prentice-Hall, 1989.

      Panchapakesan, K. A study of trellis coded quanti끄7tion for image compression. Master's thesis.
          New York: Rochester Institute of Technology, 1996.

      Papoulis, A. Signal analysis. New York: McGraw-Hill, 1977.
      Papoulis, A. Probability, random variables, and stoch口stic processes. 2nd ed. New York: McGraw-
         Hill, 1984.

      Poularikas, A.D., and S. Seely. Signals and systems. Boston: PWS-KE寸T, 1991.

      Proakis, J.G., and M. Salehi. Communication syst臼7is engineering. Upper Saddle River, NJ:
          Prentice-Hall, 1994.

      Prost, R., C. Diab, and R. Goutte. Exact subband image decomposition and reconstruction in
          discrete space and discrete frequency domains. Signal Processing: Image Communication
          July 1995;7(3):249-257.

      Raghuveer, M.R. Wavelets as signalling waveforms over partial-response channels. In:
         Raghuveer, M.R,, S.A. Dianat, S.W. McLaughlin, and M. Hassner, eds. Proceedings of
         SPIE, coding and signal processing for information storage. Vol. 2605. Philadelphia, PA, De-
         cember 1995:2上卜28.

      Raghuveer, M.R. Image enhancement and denoising by wavelet transform for concealed
         weapon detection. In: Proceedings of SPIE Conference on Investigative Image Processing.
         Boston, November 1996:112-122.
                                                                                   Bibliography    297

Raghuveer, M.R., and J.O. Chapa. Algorithms to design adaptive biorthogonal MRA gener-
   ating wavelets. In: Szu, H.H., ed. Proceedings of SPIE, wavelet applications III. Vol. 2762.
   Orlando, FL, March 1996a:40-44.

Raghuveer, M.R., and J.O. Chapa. Design of biorthogonal MRA generating wavelets matched
   to specified signal. In: International Conference on Acoustics, Speech, and Signal Processing
   Atlanta, May 1996.

Raghuveer, M.R., and J.O. Chapa. Object detection through matched wavelet transform. In:
   Szu, H.H., ed. Proceedings of SPIE, wavelet applications III. Orlando, FL, March 1996:45-50.

Raghuveer, M.R., and Szu, H.H. Novel biorthogonal MRAs using compact wavelet and
   bandlimited dual pairing. In: Szu, H.H., ed. Proceedings of SPIE, wavelet applications III.
   Orlando, FL, April 1996:282-284.

Rao, K.R., and J.J. Hwang. Techniques and standards for image, video and audio coding. Upper
    Saddle River, NJ: Prentice-Hall PTR, 1996.

Rioul, O., and P. Duhamel. Fast algorithms for discrete and continuous wavelet transforms.
    IEEE Transactions on Information Theo그／March 1992;38(2):569-586.

Rioul, O., and M. Vetterli. Wavelets and signal processing. IEEE Signal Processing Magazine
    October 1991;8(4):14-38.

Royden, H.L. Real analysis. New York: McMillan, 1978.

Rudin, W. Principles of mathematical analysis. 3rd ed. New York: McGraw-Hill Book Company,
   1976.

Sablatash, M., and T. Cooklev. Compression of high-quality audio signals, including recent
    methods using wavelet packets. Digital Signal Processing April 1996;6(2):96-107.
Sablatash, M., J.H. Lodge, and W.F. McGee. The design of filter banks with specified mmll-
    imum stopband attenuation for wavelet packet-based multiple access communications.
    In: Proceedings of 18th Biennial Symposium on Communications. Kingston, Ontario, June
    1996a:5多56.

Sablatash, M., J.H. Lodge, and W.F. McGee. Equivalence between vestigial sideband (VSB)
    and offset quadrature phase shift keyed (OQPSK) modulations and relationships to
    wavelet packet based multiplexing. In: Proceedings of 18th Biennial Symposium on Commu-
    nications. Kingston, Ontario, June 1996b:339-342.
Said, A., and W.A. Pearlman. A new fast and efficient image codec based on set partitioning
    in hierarchical trees. IEEE Transactions on Circuits and Systems for Video Technology June
    1996;6(6):243-250.

Samar, V.J., H. Begleiter, 1.O. Chapa, M.R. Raghuveer, M. Orlando, and D. Chorlain. Matched
   Meyer wavelets for clinical and experimental analysis of auditory and visual evoked
   potentials. In: Ramponi, G., G.L. Sicuranza, S. Carrato, and S. Harsi, eds. ELISIPCO.
   Trieste, Italy, September 1996:387-390.
Samar, V.J., G. Kulkarni, K.P. Swartz, I. Parasnis, M.R. Raghuveer, and V. Udpikar. Concise
   and scale-specific extraction of biomedically relevant information from visual evoked
   potential signals: Combining factor analysis with wavelet decomposition. In: Lamle,
298   Bibliography

          A.F., and M.A. Unser, eds. Proceedings of SPIE, wavelet applications in signal and image
          processing 끄 Vol. 2303. October 1994:49今507.

      Samar, V.J., M.R. Raghuveer, K.P. Swartz, S. Rosenberg, and T. Chaiyaboonthanit. Wavelet
         decomposition of event related potentials: Toward the definition of biologically natu-
         ral components. In: IEEE Sixth SP Workshop on Statistical Signal and Array Processing
         Conference Proceedings. Vol. 247. Victoria, BC, 1992:481-483.

      Samar, V.J., K.P. Swartz, and M.R. Raghuveer. Multiresolution analysis of event related
         potentials by wavelet decomposition. Brain and Cognition 1995;27(3).

      Sandberg, S.D., and M.A. Tzannes. Overlapped discrete multitone modulation for high speed
          copper wire. IEEE Journal on Selected Areas in Communications December 1995;13(9):1571-
         1585.

      Sarkar, S., and H.V. Poor. Finite field wavelet transforms and multilevel error protection.
          In: Proceedings of 1995 IEEE International Symposium on Information Theory. Whistler, BC,
          September 1995:17-22.

      Sayood, K. Introduction to data compression. San Francisco, CA: Morgan Kaufman Publishers,
          1996.

      Scharf, B. Critical bands. Technical report, special re刃ort. Syracuse, NY: Laboratory of Sensory
          Communication, Syracuse University, 1966.

      Shannon, C.E. Communications in the presence of noise. Proceedings of the IRE. January 1949;
         40:10-21.

      Shapiro, I. Embedded image coding using zerotrees of wavelet coefficients. IEEE Transactions
         on Signal Processing December 1993;41(12):3445-3462.

      Shensa, M.J. Wedding the a trous algorithm and Mallat algorithm. IEEE Transactions on Signal
          Processing October 1992;40(10):2464-2482.

      Si血a, D., and J.D. Johnston. Audio compression at low bit rates using a signal adaptive
         switched filter bank. In: IEEE International Conference on Acoustics, Speech and Signal
         Processing. Munich, April 1997.
      Sinha, D., and A. Tewflk. Low bit rate transparent audio compression using adapted wavelets.
          IEEE Transactions on Signal Processing December 1993;41(12):3463-3479.

      Smith, M.J.T., and T.P. Barnwell. Exact reconstruction techniques for tree structured subband
          coders. IEEE Transactions on Acoustics, Speech and Signal Processing June 1986;34(3):434-
          441.

      Smith, M.J.T., and S.L. Eddins. Analysis/synthesis techniques for subband image coding.
          IEEE Transactions on Acoustics, Speech and Signal Processing August 1990;38(8):1446-1456.

      Soman, A.K., and P.P. Vaidyanathan. On orthonormal wavelets and filter banks. IEEE
         Transactions on Signal Processing March 1993;41(3):1170-1183.

      Sriram, P., and M.W. Marcellin. Image coding using wavelet transforms and entropy-
           constrained trellis-coded quantization. IEEE Transactions in Image Processing 1995;4(6):
           725-733.
                                                                                             1




                                                                                     Bibliography    299

Stone, D.J. Wavelet estimation. Proceedings of the IEEE October 1984;72(10):139午1402. [Special
    issue on seismic signal processing.1

Strang, G.S. Linear algebra and its applications. San Diego: Harcourt Brace Jovanovich, 1988.

Strang, G.S. Wavelets and dilation equations. SI入4 Review 1989;31:613-627.

Strang, G.S. Wavelet transforms versus Fourier transforms. Bulletin of American Math臼7iatical
    Society 1993;28:288-305.

Strang, G.S., and T.Q. Nguyen. Wavelets and filter banks. Wellesley, MA: Wellesley-Cambridge
    Press, 1996.

Sweldens, W. Construction and application of wavelets in numerical analysis. PhD thesis. Leuven,
   Belgium: Department of Computer Science, Katholieke Universiteit, 1994.

Sweldens, W. The lifting scheme: A custom design construction of biorthogonal wavelets.
   Journal of A까lied and Computational Harmonic Analysis 1996a;3(2):186-200.
Sweldens, W. Wavelets and the lifting scheme: A 5 minute tour. Zeitschrif f7r Angewandte
   Math日7iatic und Mechanik 1996b;76(Suppl. 2):41-44.

Tekalp, A.M. Digital video processing. Englewood Cliffs, NJ: Prentice Hall, 1995.
Tsatsanis, M., and G. Giannakis. Principal component filter banks for optimal wavelet anal-
    ysis. IEEE Transactions on Signal Processing August 1995;43(8).

Unser, M. On op血llality of ideal filters for pyramid and wavelet signal approximation.
   IEEE Transactions on Signal Processing December 1993;41(12):3591-3596. [Special issue on
   wavelets and signal processing.]

Uz, K.M., M. Vetterli, and D. LeGall. Interpolative multiresolution coding of advanced tele-
    vision with compatible subchannels. IEEE Transactions on Circuits and Systems for Video
    March 1991;1(1):86-99.

Vaidyanathan, P.P. Multirate digital filters, filter banks, polyphase networks, and applica-
    lions: A tutorial. Proceedings of the IEEE January 1990;78:56-93.

Vaidyanathan, P.P. Multirate systems and filter banks. Englewood Cliffs, NJ: Prentice-Hall,
    1992.

Vaidyanathan, P.P., and A. Kirac. Theory of cyclic filter banks. In: IEEE International Conference
    on Acoustics, Speech and Signal Processing. Munich, April 1997:2449-2452.

Ve仕erli, M., and C. Herley. Wavelets and filter banks: Theory and design. IEEE Transactions
   on Signal Processing September 1992;40:1414-1429.

Vetterli, M., and J. Kovacevic. Wavelets and subband coding. Englewood Cliffs, NJ: Prentice-
    Hall, 1995.

Wandell, G.A. Foundations of vision. Sunderland, MA: Sinauer Associates, 1995.

Wesfreid, E., and M.V. Wickerhauser. Adapted local trigonometric transforms and speech
   processing. IEEE Transactions on Signal Processing December 1993;41(12). [Special issue
   on wavelets and signal processing.]
300   Bibliography

      Wickerhauser, M.V. Adapted wavelet analysis: From theory to software. Boston: A.K. Peters, 1994.

      Wornell, G.W. Emerging applications of multirate signal processing in digital communica-
         tions. Proceedings of IEEE April 1996a;84(4).

      Wornell, G.W. Signal processing with fractals. Upper Saddle River, NJ: Prentice-Hall, 1996b.
      Wornell, G.W., and A.V. Oppenheim. Estimation of fractal signals from noisy measurements
         using wavelets. IEEE Transactions on Signal Processing March 1992a;40:611七23.

      Wornell, G.W., and A.V. Oppenheim. Wavelet-based representations for a class of self-similar
         signals with application to fractal modulation. IEEE Transactions on Information Theory
         March 1992b;38(2):785-800.

      Zayed, A.I. Advances in Shannon's sampling theory. Boca Raton, 凡: CRC Press, 1993.
      Zhan, Y.Q., W. Li, and M.L. Lian, eds. Special issue on advances in image and video corn-
         pression. Proceedings of the IEEE February 1995;83.
      Zhao, W., and R.M. Rao. Discrete-time self-similar signals and scale-invariant systems. Technical
         Report TR-Zhrao-97-01. Rochester, NY: Center for Imaging Science, Rochester Institute
         of Technology, October 1997.
                                       INDEX




Additive inverse, 285                                 audio compression and, 179
Additivity, 287                                       critical, 175나176
Admissibility condition, 21-22                        frequency selectivity and, 12, 15-17
Algorithms                                            RMS (root mean square) bandwidth, 16-
  a trous algorithms, 224느228                           18
  best basis algorithms, 248-249                      signaling pulses and, 212
  Mon1et algorithm, 23                                video coding and, 181
  Parks-McClellan algorithm, 106                    Bases, 286-287
  SPIH1' algorithm, 153-154, 157, 166, 168-         Basis functions, 36-37
     169                                            Best basis algorithm, 248-249
anal2d routine, 127, 132                            Biorthogonol decomposition, 236-241
analh routine, 127                                  Biorthogonal filters, 102-104, 127, 149-150
analh2d routine, 132                                Biorthogonal scaling functions, 104-108, 241-
analw2d routine, 132                                     244
anaiw routine, 127                                  Biorthogonal wavelet(s), 104-108
Analysis ifiter banks, 69小70, 104                     bases, 95-102
Approximation coefficients, 41, 42                    designing, 244尸248
Arithmetic coding, 139                              Biorthogonality, 95-96
Associativity, 285                                  biscwav routine, 127
Audio compression, 133, 170-178. See also           Blocking artifacts, 169
     Compression                                    Blurring, 167, 169
  audio masking and, 175-176                        Brick-wall filters, 262. See also Shannon
  coding, wavelet-based, 178-179                         scaling function
  image compression and, comparison of,
     171-172
  standards, 177-178
Audio CDs (compact discs), 171-173                  Cauchy-Schwartz inequality, 10, 204-205,
Autocorrelation functions, 267                          288
Autocorrelation sequences, 56, 87, 267              CDs (compact discs), 171-173. See also Au-
                                                        dio compression
                                                    Chrominance components, 168-169
B-splines, 104, 105-106                             Circular convolution filter banks, 252-259
Bandlimited biorthogonol decomposition,             Circular extension, of input sequences, 88尸
    236-그41                                             89
Bandlimited biorthogonal scaling functions,         Coefficients
    241-244                                           approximation coefficients, 41, 42
Bandlimited wavelets, 71寸77                           data compression and, 144-147, 150
Bandpass functions, 12-13                             Daubechies filter, 234, 236
Bandwidth                                             edge-related, 183

                                              301
302    Index

       Coefficients (cont.)                             as a correlation, 子11
          generating scaling functions and wavelets     DWTs and, brid얹ng the gap between,
              from, 89-92                                  223-그28
          PRCC filter bank, 259                         inverse, as a ma呵寸O田ne 叩아餌on, 220-
          quantized subband coefficients, 150              222
          regularity and, 229                           with orthonormal basis-generating wavelets,
          transformation coefficients, 144-147             223-224
          wavelet denoising and, 183-189                Parseval's identity for, 23, 217-223
       Coherent imaging, 189-190                      Convergence, 50, 229-232
       Column filtering, 114                          Converters
       Compression                                      parallel-to-serial, 216
          for audio versus for images, comparison       serial-to-parallel, 214, 216
             of, 171-172                              Correlation
          color, 168-169                                CWT as a, 8-11
         DCT (discrete cosine transform) compres-       procedures, 205-206
             sion 釵：hemes, 146-147, 16今170, 178,      Cost functions, 248-249, 251
             181                                      Critical bandwidth, 175-176
         DTWT for, 147-151
                                                      Critical bands, average, 176
         embedding tree image coding for, 151-        Cross-correlational interpretation, 10, 11
             166
                                                      Cubic B-spline filters, 10乍106
         Huffman coding and, 139, 145, 149, 150-
                                                      Cubic B-spline wavelets, 2, 10午106, 126
             152, 179
                                                      CWT. See Continuous wavelet transform
         lossless compression, 133-134, 138-139
         iossy compression, 133-134, 140-141, 173
         nonseparable multidimensional wavelets
            and, 121                                  D4 filters, 83, 114, 128-131
         quantization and, 140-141                      data compression and, 147
        run-length encoding and, 149-151                Daubechies constructions and, 232-233,
         Shannon's theorem and, 138-139                    234, 235
         transform coding and, 142-147                  wavelet denoising and, 188-189
         wavelet packets for, 125, 126, 178-180,      D4 scaling functions, 71, 83, 91-92
            249                                       Data compression. See Compression
      Communication applications, 208-217             Data fusion, 201
      Commutativity, 270, 285                         Daubechies four-tap FIR filter (D4), 194
      Computation, of mean opinion scores, 173-       Daubechies constructions, 232-236
            174                                       DC term, 31-32
      Conditions, for perfect reconstruction, 256中    DCT (discrete cosine transform) compres-
            258                                            sion schemes, 146-147, 166-170, 178,
      Constant Q-factor filtering interpretation,          181
            11-19                                     Decimated a trous algorithms, 224-228
      Continuous scaling, 269                         Decimation, 41, 65
      Coi寸inuou乎time                                  Decomposition, 43, 46
        functions, 41                                  bandlimited biorthogonal, 236-241
        time linear scale-invariant systems, 265-      best basis algorith江ls and, 249
            268                                        biorthogonal wavelet bases and, 102, 106
        wavelets, 1-3                                  data compression and, 151-152, 161-162
      Continuous wavelet transform (CWT)               小rect sum, 63七4
        a trous algorithms and, 224-228                filters, 64-65, 102
        basic description of, 1-8                      Haar wavelet, 25, 41-49, 59
                                                                               Index     303

  t사o-dimensional wavelets and, 114            signals, data compression and, 133-134,
  using the Haar wavelet, 187-189, 190           140
  wavelet packets and, 121-126               Discrete-time wavelet transform (DTWT),
Decorrelating data, 144                          78-84, 93-94
Denoising, 183-193                             audio compression and, 170
  applying, to speckle removal, 189-192        basis functions for, 81-84
Dense unions, of subspaces, 52                 continuous-time MRA interpretation for,
Design, of wavelets, 244-252                     78-89
  best basis algorithms and, 248-249           data compression and, 133, 147-151, 157-
  lifting schemes and, 244-248                   161, 181-182
Despeck血lg schemes, 198-200                    data fusion and, 201-204, 207
Detail coefficients, 41                        discrete multitone transmission (DMT)
Detail functions, 35, 56, 95                      and, 21牛＝215
Detail subspaces, 61七3                         edge detection and, 184, 187, 198, 192-
Detection, edge, 192-200                         194, 201-204, 207, 214-217
DVFs                                           for image compression, 147-151
  discrete multitone transmission (DMT)        run-length encoding and, 149-151
     and, 214-216                              tree image coding and, 151-152, 157-161
  PRCC filter banks and, 252, 25牛口256, 259     video coding and, 181, 182
                                               wavelet denoising and, 192
Dialing, touch-tone, 23
                                             D始口ete 恥ravelet multitor祀 modul計ion (D＼사入'IT),
Digital filtering interpretation, 64-70
                                                  215, 217
Digital ifiter implementation, of the Haar
                                             Discrete wavelet transform (DWT), 25-49,
     wavelet, 41-49
                                                  51, 59
Dilation, 4, 13
                                               C叭／Ts and, bridging the gap between,
  biorthogonal wavelet bases and, 97, 100
                                                  223-그28
  discrete wavelet transform and, 26, 35-
                                               data compression and, 133尸182
     36, 40
                                               frequency-sampled implementation of,
  frequency selectivity and, 17                   262-263
  matrices, 118-121
                                               interpolation sampling systems and, 261
  MRAs and, 53-58, 74, 78, 91, 93              nested linear vector subspaces and, 29中
  orthogonal wavelets and, 74                     32
  scaling function and, 35-36                  two-dimensional wavelets and, 114
  two-dimensional wavelets and, 113-114,       wavelet denoising and, 183
     118-120                                   wavelet packets and, 121
Direct sum                                   Distortion, minimization of, 173
  decomposition, 63-64                       Distributive property, 285
  of subspaces, 31                           DMT (discrete multitone transmission), 214-
Discrete cosine transform (DCT) compres-          217
     sion schemes, 146-147, 166-170, 178,    Downsampler, 271-272, 282-284
     181                                     Downsampling, 41, 65, 67, 93. See also
Discrete frequency domains, 255-256              Sampling
Discrete mul出one transmission (DMT), 214-      biorthogonal wavelet bases and, 99
     217                                       discrete multitone transmission (DMT)
Discrete time                                    and, 215
  inte叩reting orthonormal 入lR如 幻r, 78-         DTWT and, 88, 89
     84                                        PRCC ifiter ba川f;s and, 252-255
  LSI systems, 271-277                         scaling interpretations and, 268
  scaling in, 268-271                          two-dimensional wavelets and, 110, 114
304   Index

      DTMF (dual-tone multifrequency signal-             cubic B-spline filters, 104-106
         ing), 24                                        CWTs and, 226
      DTWT. See Discrete-time wavelet transform          D4 filters, 83, 114, 128-131, 147, 188-189,
      Dual scaling functions, 100                            232-233, 234, 235
      Dual-tone multifrequency signaling (DTMF),         Daubechies constructions and, 233
         24                                              discrete multitone transmission (DMT)
      DWMT (discrete wavelet multitone mod-                 and, 215
         ulation), 215, 217                              FBI (Federal Bureau of Investigation) flu-
      D叭汀. See Discrete wavelet transform                    ters, 106, 107, 127, 149-150
      Dyadic sampling, 26-28                             FIR (血ite impulse response) filters, 71,
                                                            87, 95, 97, 104, 233-234, 244-246, 256
                                                         halfband ifiters, 106
      Edge detection, 192-200                            HPFs (high-pass filters), 42, 68, 71, 74,
      Edge-related coefficients, 183                        115, 121-122, 125, 187-189, 190, 192-
      Eigenfunctions, 264-265, 273-278                      200, 262- 263
      Embedded bit streams, 153                          hR (infinite impulse response) filters, 65,
      Entropy, 135, 137-139, 248-249                        77
      EOB (en小可小lock), 151                              implementation, of the Haar wavelet, 41-
      Equalization, post-detection, 215, 216                49
      Error(s)                                           interpolation sampling systems and, 261
        between original functions and approx-           lifting schemes and, 244-248
          imations, 49                                   linear B-spline filters, 104-106
        vectors, 30-31                                   LPFs (low-pass 丘［ters), 42, 50, 66, 68, 71,
        video coding and, 181, 182                          74, 83, 104, 115, 121, 122, 125, 194,
      Euclidean space, 143-144, 288                         232-233, 234, 262-263
      Expanders, 280-282                                 PRQMFs (perfect reconstruction quadra-
      取perime址s, in audio percept帥，175-176                  hire mirror filters), 66, 73-74, 84-89,
      Extension, of input sequences, 88-89                  106, 147, 229, 230, 233-235
                                                         QMF (quadrature mirror filters), 42-43,
                                                            46, 66-67, 70-71
      Factorization, 232, 234                            quadratic B-spline filters, 104-106
      FBI fingerprint compression scheme, 106,           two-dimensional wavelets and, 110, 111-
           107, 127, 149-150                                112, 114
      FDM (frequency division multiplexing), 215         video coding and, 182
      I下r (Fast I恤rier transform) 叩era如n, 177-           wavelet denoising and, 187-189
           178, 184-189. See also Fourier trans-         wavelet packets and, 122, 124-125
           幻rm                                        Filter banks, 51-94. See also Filters
        inverse, 187                                     analysis filter banks, 69-70, 104
        PRCC filter banks and, 256                       circular convolution filter banks, 252-
         wavelet denoising and, 184-187                     259
      Filter(s). See also Filter banks                   convolution ifiter banks, 252-259
        biorthogonol decomposition and, 236-            PRCC (perfect reconstruction circular con-
           241                                              volution) filter banks, 252-259, 262
        biorthogonal wavelet bases and, 99, 101,         synthesis filter banks, 69-70, 80, 104
           102, 103-104                               Fingerprint image compression (FBI filters),
        brick-wall filters, 262                             106, 107, 127, 149-150
         coefficients, generating scaling functions   Finite-dimensional vectors, 98
           and wavelets from, 89-92                   Finite-length discrete-time signals, 134卞135
                                                                                     Index    305

FIR (finite impulse response) ifiters, 71, 87,     Haar scaling functions, 35寸36, 89, 90,
     95, 97, 104                                     104
  Daubechies constructions and, 233-234            Meyer scaling functions, 74, 76寸77, 213-
  可ting schemes and, 244-246                         214, 261, 262-263
  PRCC filter banks and, 256                       one-dimensional functions, 118-119
Fourier transform, 11-12, 106                      orthogonal functions, 111, 113
  audio compression and, 177-178                   orthonormal scaling functions, 232-240
  biorthogonal scaling functions and, 242          probability density functions, 16
  discrete wavelet transform and, 25-26,           Shannon scaling functions, 74-75
     28                                            sinc function, 74
  discrete-time LSI systems and, 272               square integrable functions, 64, 101
  frequency selectivity and, 16小17                 transfer functions, 282-284
  interpolation sampling systems and, 261          unit step function, 6, 46
  inverse C叭丁 and, 21-22                           Walsh function, 132
  MRAs and, 56, 61, 72-73, 76-77, 90, 91,
     93
  orthogonal wavelets and, 56, 61, 72-73,
     76-77, 90, 91, 93                           Gaussian functions, 3, 11, 19
  regularity and, 231                            Gaussian noise
  scaling interpretations and, 26多271              self-similar signals and, 265
  short-time, 22, 166                              wavelet denoising and, 184, 191-192
  signaling pulses and, 212-214                  Geometric analogies, 30
  upsampler and, 281                             "Girl with Hat" photograph, 118-119, 127,
  wavelet matching and, 250                          132, 139, 148, 15午155, 162, 168-169
  wavelet pair construction and, 243
Fractional sampling rate alternation, 268
Frames, video, 182
Frequency                                        Haar scaling functions, 35-36, 89, 90, 104
  division multiplexing (FDM), 215               Haar wavelet, 6, 70-77
  domain equivalents, 5令57, 60                     Daubechies constructions and, 232-233,
  domain explanations, 175                           234
  sampled implementation, of bandlimited           decomposition, 25, 41-49, 59
     DWTs, 262-263                                 digital filter implementation, 41-49
  selectivity, 11-19                               discrete wavelet transform and, 29, 36-
Functions                                            49
  autocorrelation functions, 267                   MRAs and, 46-47, 51, 58-64
  bandlimited biorthogonal scaling func-           regularity and, 229-230
     tions, 241-244                              Halfband constraint, 106
  bandpass functions, 12-13                      Halfband filters, 106
  basis functions, 3今37                          HDTV (high definition television), 181
  biorthogonal scaling functions, 104-108,       Hilbert space, 288-289
     241-244                                     Histograms, 195-199
  continuous-time functions, 41                  Homogeneity, 287
  cost functions, 24肛249, 251                    Homogeneous signal, 267, 271
  D4 scaling functions, 71, 83, 91-92            HPFs (high-pass filters), 42, 68, 74, 187-
  detail functions, 35, 56, 95                       189, 190
  dual scaling functions, 100                      DWTs and, 262-263
  eigenfunctions, 264-265, 273-278                 edge detection and, 192-200
  Gaussian functions, 3, 11, 19                    orthogonal wavelets and, 71
306   Index

      HPFs (cont.)                                    International Standards Organization (ISO)
       two-dimensional wavelets and, 115                    standards, 177-178
       wavelet packets and, 121-122, 125              Interpolation expressions, 46, 81, 83
      Huffman coding, 139, 145, 149-152, 179             biorthogonal wavelet bases and, 102
                                                         scaling interpretations and, 268
                                                      Interpolation sampling system, 260-262
      Identity matrices, 103                          Interpolators, 259-260
      IDFF (inverse DFT), 252, 256                    Inverse CWT, 20-22
      IFFF (inverse FFF), 187                         Irrelevancy, removal of, 134-135, 141
      h1R (infinite impulse response) filters, 65,    ISI (intersymbol interference), 211-215
            77                                        ISO (International Standards Organization)
                                                           standards, 177-178
      Image(s)
         detec如n of objects in, 205-206
         fusion, 200-204, 207
         "Girl with Hat" photograph, 118-119,         JPEG (Joint Photographics Expert Group)
            127, 132, 139, 148, 154-155, 162, 168-       images, 151, 166-170, 173. See also Im-
            169                                          ages
        HH (high-high) images, 114-115
        HL (high-low) images, 114-115
        infrared images, 201
                                                      KLT (Karhunen-Loeve transform), 144, 147
        JPEG (Joint Photographics Expert Group)
            images, 151, 166느170, 173
        LH (low-high) images, 114-115
        LL (low-low) images, 114-115                  Lifting schemes, 106, 244-248
        log-transformed images, 192                   Linear. See also Linear vector space
        representation, 118-121                         algebra, 285-289
      Image compression, 133-170. See also Com-         B-spline filters, 10午106
            pression                                    convolution, 87山88
        best basis algorithm and, 249                   independence, 286-287
        DTWT for, 147-149                             Linear vector space
         JPEG compression, 151, 166-170, 173            biorthogonality and, 96
         transform coding and, 142-147                  finite-dimensional, 29-30
         tree image coding and, 151-152                 discrete wavelet transform and, 29-49,
      Implementation procedures for PRCC, 255-             52-53, 5牛-55
            256                                         two-dimensional wavelets and, 110-111,
      Inequality, Cauchy-Schwartz, 10, 204-205,            113
            288                                       Linear-phase property, 87
      Infinite-dimensional linear vector space, 31-   LIP (list of insignificant pixels), 160, 162-
            32                                             164, 166
      Information theory, 248-249                     LIS (list of insignificant sets), 160-164, 166
      Infrared images, 201                            Loading factors, 150
      Initialization, of lists for the SPIHT algo-    Localization
            rithm, 161-162                               frequency, 18-19
      Inner products, 牛9, 222-223, 287-288               time, 18-19
      Input process, interpolators matched to,        Log-transformed images, 192
            259-260                                   Lookup tables, 154
      Interference, intersymbol (ISI), 211-215        Lossless compression, 133-134, 138-139. See
      Interframe coding, 181                               also Compression
                                                                                    Index    307

Lossy compression, 133-134, 140-141, 173.         discrete wavelet transform and, 29-49
    See also Compression                          example of, 32-49
LPFs (low-pass filters),42, 50                    formal definition of, 52-53
  biorthogonal wavelet bases and, 104             Haar scaling function and, 35-36
  Daubechies constructions and, 232-233,          orthonormal, 53-58, 78-84
    234                                           two-dimensional wavelets and, 109-115
  DWTs and, 262-263                               wavelet basis for, 58-64
  edge detection and, 194                         wavelet matching and, 250
  orthogonal wavelets and, 66, 68, 71, 74,        wavelet packets and, 121-126
    83                                          MRI (magnetic resonance imaging), 203,
  two-dimensional wavelets and, 115                 207
  wavelet packets and, 121, 122, 125            MSBs(most significant bits),157, 158, 160,
LSI (linear scale-invariant) systems, 265-          161, 164
    266, 271-277                                Multiplicative models, for speckle, 191
LSP (list of significant pixels), 160, 162-     Multirate systems, 279-284
    163, 166                                    Multiresolution analysis. See MRA
LTI(linear-time-invariant)system,209,264-       Multiscale decompositions, 148
    268
Luminance components, 168-169
                                                N-dimensional Euclidean space, 143-144
                                                N-dimensional vectors, 143-144
Matching wavelets, 250-252                      Nested linear vector subspaces,29-49,52-
Matrix transformations, 144-145                     55
MCM (multicarrier modulation),214-217           Noble identities, 282-284
MDCT(modified discrete cosine transform),       Noise floors, 184-185
    178, 179                                    Noiseless coding, Shannon's theorem for,
Memoryless source, 135, 138                         138-139
Metrics, quantitative, for time and frequency   Noise power spectrum density, 175
    resolution, 15-16                           Nonseparable multidimensional wavelets,
Mexican hat wavelet, 11-15, 22                      115-121
Meyer scaling functions, 74, 76-77, 261         Nonterminal nodes, 125
  frequency-sampled implementations of          Normalization factors, 4, 207
    DWTs and, 262-263
  signaling pulses and, 213-214
Meyer wavelet, 76-77, 106, 250                  Object
Monlet algorithm, 23                              detection, 204-208
Monlet wavelet, 3, 5                              isolation, 192-200
Mother wavelets, 2, 4-6, 15-16, 18, 22          OFDM (orthogonal frequency division mul-
Motion compensation, 181                            tiplexing),214-217
MPEG(Moving Picture Experts Group)stan-         Operator, CWT as an, 19-20
    dards, 177-178                              Orthogonal complements, 40
  MPEG-i standard, 177-178                      Orthogonal frequency division multiplex-
  MPEG-2 standard, 177-178                          ing (OFDM),214-217
MRA (multiresolution analysis),29-31,51-        Orthogonal functions, 111, 113
    94                                          Orthogonal sets, 36, 40
  biorthogonal wavelet bases and,98-102         Orthogonal wavelet(s)
  decomposition and, 63-64, 84, 89                decomposition, 25-49
  detail subspaces and, 61-63                     the dilation equation and, 55-57
308   Index

      Orthogonal wavelet(s) (cont.)                   Power complementarity property, 66
        examples, 70-77                               PRCC (perfect reconstruction circular con-
       nonseparable multidimensional wavelets              volution) filter banks
          and, 121                                      basic description of, 252-259
        signaling pulses and, 208-214                   conditions for reconstruction and, 256-
        wavelet packets and, 123, 125                      258, 262
      Orthonormal basis-generating wavelets, 223-       downsampling and, 252-255
          224                                           implementation procedures and, 255-256
      Orthonormal MRAs. See also MRA (mul-              interpolation sampling systems and, 261
          tiresolution analysis)                        procedures for constructing, 258-259
        construction of, 53-58                          upsampling and, 255
       interpreting, for discrete-time signals, 78-   Probability density functions, 16
          84                                          Product spaces, inner, 8-9, 222-223, 287-
      Orthonormal scaling functions, 232-240               288
      Orthonormal wavelets, 51-94                     Progressive transmissions, 158
                                                      Projection(s)
                                                        operations, wavelet inner product as, 222-
      Packets, wavelet, 121-126                            223
      Paraunitary conditions, 60, 84, 93, 103-104       wavelet transforms of, 204-208
      Parks-McClellan algorithm, 106                  PRQMFs. See Perfect reconstruction quadra-
      Parseval's identity, for CWTs, 217-223               ture mirror filters
      Parseval's theorem, 22
      Pattern recognition, 121
      PCM (pulse code modulation) signals, 171,       QMF (quadrature mirror filters), 42-43, 46,
           173, 174                                       66-67
      Perfect reconstruction quadrature mirror         orthogonal wavelets and, 70-71
           filters (PRQMFs), 66, 73-74                 power complementarity property, 66
        biorthogonal wavelet bases and, 106           Quadratic B-spline filters, 104-106
        data compression and, 147                     Quantitative metrics, 15-16
        Daubechies constructions and, 233-235         Quant也ation, 140-142, 161
        MRAs and, 84-89                                audio compression and, 173, 176, 177-
        regularity and, 229, 230                          178, 179
      Periodic extension, of input sequences, 88-      image compression and, 166
           89                                          noise spectrum, 176
      Periodic trigonometric polynomials, 247          scalar, of transformation coefficients, 145-
      PET (positron emission tomography) scans,           146, 152
           203, 207                                   Quantizer, 149-150
      Pointwise convergence, 50                       Quincunx lattice, 120-121
      Poisson summation formula, 56, 72, 74, 92,
           212
        interpolation sampling systems and, 261
        regularity and, 229-230                       Random vectors, 136-137
        wavelet matching and, 250                     Reconstruction, 43, 46, 68-70, 142
      Polynomials, trigonometric, 232                   biorthogonal wavelet bases and, 102
      Positron emission tomography (PET) scans,         filter banks, 102, 126
           203, 207                                   Redundancy, 134-135, 144
      Positivity, 287                                 Reference scale vectors, 206
      Power complementarity condition, 57, 84         Refinement passes, 159-160, 161, 166
                                                                                     Index      309


Regularity, 229-232                              orthogonal wavelets and, 52-54, 68-70,
Resolution. See also MRA (multiresolution           72, 93
     analysis)                                   two-dimensional wavelets and, 114
  data compression and, 178, 181-182           Scalograms, 8, 10, 14-15, 24
  digital ifitering and, 43                    Selection, of wavelets, 244-252
  levels of, approximations to a function      Separable formulations, 114
     at, 34                                    Shannon, Claude, 74
  multi-, techniques, 181-182                  Shannon scaling function, 74中75. See also
  providing finer, 178                              Brick-wall filters
  山lle-frequency, 11-19                        Shannon's theorem, 138-139
   two-dimensional wavelets and, 113           Shannon wavelet, 74尸75
   video coding and, 181-182                   Shift parameters, 10
RGB (red-green-blue) images, 168-169           Short-time Fourier transform (STFr), 22,
Riesz basis, 64, 289                                166
RMS (root mean square) duration, 16-18         Signaling pulses, 208-214
Run-length encoding, 14多151                    Significance maps, 158, 160, 161
                                               Sinc function, 74
                                               Sorting passes, 159, 160, 165, 166
Sampling. See also Downsampling                Sound pressure level (SPL), 175-176
  dyadic, 26-28                                Spatial orientation trees, 158小159
  frequencies, 170-171                         Spatiotemporal pyramid schemes, 181
  lattice, 120-121                             Speckle removal, 189-192
  rate compressor, 271尸272                     Spectral factorization, 233
  rate expander, 28아282                        SPIHT algorithm, 153-154, 157
Scaling functions, 35-36, 38. See also Scal-      compression results for, 166, 168
     ing operations                               JPEG compression and, 169
  bandlimited biorthogonal, 241-244               lists for, initialization of, 161-162
  biorthogonal decomposition and, 236-          SPL (sound pressure level), 175-176
     241                                        Square integrable functions, 64, 101
  biorthogonal wavelet bases and, 97-98,        Stationary random signals, 272-273
     100, 104-108
                                                Statistically self-similar processes, 267
  Daubechies constructions and, 232-240
                                                Statistical surveys, for mean opinion scores,
   frequency-sampled implementations of              173
     DWTs and, 262-263
                                                STFT (Short-time Fourier Transform), 22,
   generating, from filter coefficients, 89-         166
      92
                                                Streogrammetry, 201
   Haar scaling functions, 35-36, 89, 90,
                                                Subsampler, 271-272. See also Downsam-
      104
                                                    pling
   Meyer scaling functions, 74, 76-77, 213-
      214, 261, 262-263                         Symbol amplitude, 209
                                                synth2d routine, 127, 132
   orthonormal scaling functions, 232-240
   Shannon scaling functions, 74-75             Synthetic aperture radar, 189
                                                Synthesis filter banks, 69-70, 80, 104
   as signaling pulses, 208-214
Scaling operations, 261, 264-271. See also      synthh2d routine, 132
      Scaling functions                         synthh routine, 127
   in discrete time, 268口271                    synthw2d routine, 132
   nonseparable multidimensional wavelets       synthw routine, 127
      and, 115寸116, 121                         System kernels, 266
310    Index

       Tables, lookup, 154                           Unconditional bases, 149
       TDM (time-division multiplexed) forms, 214-   Unit step function, 6, 46
            215                                      Upsampler, 280-284. See also Upsampling
       Thresholds, 178, 183-188, 195-198             Upsampling, 69, 255, 280-284
       Time-division multiplexed (TDM) forms,         digital ifitering and, 43
            214-215                                   DTWT and, 82-83
       Time domain                                    scaling interpretations and, 268
          equivalents, 67                             wavelet packets and, 124
          sequences, 61
       Time-frequency
         cells, 18-19, 26-28                         Vector(s). See also Vector spaces
         resolution, 11-19                              approximations of, in nested linear sub-
       Touch-tone dialing, 23                              spaces, 29-49, 54-55
       Transfer functions, 282-284                      binary representations and, 154-156
      Transform-based motion compensation scheme,       DCT (discrete cosine transform) and, 146-
            181-182                                       147
      Transform coding, 142-147                         subspaces, basic description of, 286
      Translation, 4, 17, 20, 85-87                     transform coding and, 145
         biorthogonal wavelet bases and, 100         Vector spaces. See also Vectors
         discrete wavelet transform and, 40            brief review of, 285-287
         DTWT and, 82                                   complete, 288
         parameters, discrete wavelet transform        discrete wavelet transform and, 29-49,
            and, 26-27                                    52-53, 54-55
         scaling functions and, 35-36                  finite-dimensional, 29-30
         two-dimensional wavelets and, 113-114         in丘nite-dimensional, 31-32
      Transmission rates, 173                          linear algebra and, 285-289
      Transmultiplexer system, 215                     nested linear, 29-49, 52-53, 54-55
      Tree(s)                                        Video compression, 133, 181-182. See also
        image coding, embedding, 151-166                  Compression
         spatial orientation, 158-159
         wavelet packet, 180
      Trigonometric polynomials, 74, 232             Walsh function, 132
      Triple stimulus/hidden reference/double-       ＼人／hite n아卵／ 176, 267
           blind tests, 173-174                      Wideband speech signals, compression of,
      T1사아dim이怜幻nal wavelets, 109中115                     170-175
      Two-scale difference equation, 55              WSS (wide sense stationary) process, 260
      Two-scale relations, 59-61, 73, 101-102


                                                     Zero factors, 35, 53
      Ultrasound radiation, 189                      Zero-tree coding, 153, 156-157
      Uncertainty principle, 19                      Ziv-Lempel coding, 139
                                                              Hube片 Space and Riesz Bases    289

In a Hulbert space, the unconditional basis is also called a Riesz basis. The Riesz
basis can also be characterized by the inner product defined on V. Let v be a vector
in V. Then there exist constants a > 0 and fi < 茯） such that

                            이V下드刃他놔노帥下1                                            (B.10)

This condition is not sufficient. It is required that the basis functions also be linearly
independent. For example, the orthonormal wavelet basis described in Chapter 3
is a Riesz basis for L2(R).
