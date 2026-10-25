---
source_url: /run/media/yutae/Data/Introduction_Wavelets_and_Transforms.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: f6d6da27e1e3a72ff4b46494646f7e27932b73de4de1353fa18f7cc776798e31
---
# Introduction to Wavelets and Wavelet Transforms: A Primer (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출 (~945,432 chars). 일부 토큰은 인식 오류로 깨짐 (한/영 혼용 OCR 산출). 원문 PDF(`books/Introduction_Wavelets_and_Transforms.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Introduction to Wavelets and Wavelet Transforms: A Primer
- authors: C. Sidney Burrus, Ramesh A. Gopinath, Haitao Guo (Rice University)
- additional material/programs: Jan E. Odegard, Ivan W. Selesnick
- edition: 1st (International Ed.)
- year: 1998
- publisher: Prentice-Hall International (Simon & Schuster / A Viacom Company)
- pages: 282 (pdfinfo)
- isbn: 0-13-888702-0
+ source file: `Introduction_Wavelets_and_Transforms.pdf` (sha256: `f6d6da27e1e3a72f…`)
+ extract: `pdftotext -layout` @ 2026-10-25, 945,432 chars

## Chapter structure (from TOC)
| # | topic | page |
|---|-------|------|
| 1 | Introduction to Wavelets — Haar systems, DWT overview | 1 |
| 2 | Multiresolution Formulation — signal spaces, scaling/wavelet functions | 10 |
| 3 | Filter Banks and the DWT — analysis/synthesis, lattices & lifting | 31 |
| 4 | Bases, Orthogonal/Biorthogonal Bases, Frames, Unconditional Bases | 41 |
| 5 | Scaling & Wavelet Coefficients — conditions, cascade algorithm, parameterization | 50 |
| 6+ | Remaining chapters: applications & programs (282p total) | ~70-282 |

## Original text (all 283 pages)

     Introduction to Wavelets
      and Wavelet Transforms


                         A Primer




C. Sidney Burrus, Ramesh A. Gopinath, and Haitao Guo


             with additional material and programs by

              Jan E. Odegard and Ivan W. Selesnick


         Electrical and Computer Engineering Department
        and Computer and Information Technology Institute
                          Rice University
                          Houston, Texas
                           csb@rice.edu




                             盈
                 Prentice-Hall International, Inc.
This edition may be sold only in those countries to which it is consigned by Prentice-Hall International. It is not
to be re-exported, and it is not for sale in the U.S.A, Mexico, or Canada.




Acquis札幻ns Editor: 끄刃71 J切bbins
Production Editor: Sha깬1 Vitrano
Edito卜it卜（갔iief Marci口 月b忖on
Managing Editor: Bayani Mendoza DeLeon
Copy Editor: Irwin Zucker
Cover Designer: Bruce Kenselaar
Director of Production and Manufacturing: David W. Riccardi
Manufacturing Buyer: Donna Sullivan
Editorial Assistant: Nancy Garcia
Composition: PR甘IX, INC.




             匣） 1998 by Prentice-Hall, Inc.
             Simon & Schuster / A Viacom Company
             Upper Saddle River, New Jersey 07458




The author and publisher of this book have used their best efforts in preparing this book. These efforts include
the development, research, and testing of the theories and programs to determine their effectiveness. The
author and publisher make no warranty of any kind, expressed or implied, with regard to these programs or the
documentation contained in this book. The author and publisher shall not be liable in any event for incidental
or consequential damages in connection with, or arising out of, the furnishing, performance, or use of these
programs.




All rights reserved. No part of this book may be reproduced, in any form
or by any means, without permission in writing from the publisher.




Printed in the United States of America

10   9   8   7   6   5   4   3   2   1

ISBN         1J- 13- 888702- O

Prentice-Hall International (UK) Limited, London
Prentice-Hall of Australia Pty. Limited, Sydney
Prentice-Hall Canada Inc., Toronto
Prentice-Hall Hispanoamericana, S.A., Mexico
Prentice-Hall of India Private Limited, New Delhi
Prentice-Hall of Japan, Inc., Tokyo
Simon 8乙 Schuster A針a Pte. Ltd., Sii四띠刃7毛
Editora Prentice-Hall do Brasil, Ltda., Rio de Janeiro
Prentice-Hall, Inc., Upper Saddle River, New Jersey
                                                                    Contents


Preface                                                                       xi

                                                                               寸
                                                                               l
1   Introduction to Wavelets
                                                                               n
                                                                               乙
    1.1 Wavelets and Wavelet Expansion Systems
                                                                               n
                                                                               乙
         ＼人／hat is a ＼人／avelet Expax娼ion or a Wavelet I노ax娼如rm?
                                                                               9
                                                                               口
         What is a Wavelet System?
                                                                               n
                                                                               J
         More Specific Characteristics of Wavelet Systems
                                                                               二
                                                                               U
         Haar Scaling Functions and Wavelets
                                                                               =
                                                                               U
         What do Wavelets Look Like?
                                                                               n
                                                                               0
         ＼人／by is 砥ravelet Analys始 E珏ective?
                                                                               力
                                                                               1
                                                                               1
    1.2 The Discrete Wavelet Transform
                                                                               8
    1.3 The Discrete-Time and Continuous Wavelet Transforms

                                                                               0
                                                                               V 0
                                                                                 J
    1.4 Exercises and Experiments
    1.5 This Chapter

2   A Multiresolution Formulation of Wavelet Systems                          10
    2.1 Signal Spaces                                                         10
    2.2 The Scaling Function                                                  11
        Multiresolution Analysis                                              12
    2.3 The Wavelet Functions                                                 14
    2.4 The Discrete Wavelet Transform                                        17
    2.5 A Parseval's Theorem                                                  18
    2.6 Display of the Discrete Wavelet Transform and the Wavelet Expansion   18
    2.7 Examples of Wavelet Expansions                                        20
    2.8 An Example of the Haar Wavelet System                                 23

3 Filter Banks and the Discrete Wavelet Transform                             31
  3.1 Analysis - From Fine Scale to Coarse Scale                              31
       Filtering and Down-Sampling or Decimating                              32
  3.2 Synthesis - From Coarse Scale to Fine Scale                             36
       Filtering and Up-Sampling or Stretching                                36
  3.3 Input Coefficients                                                      37
  3.4 Lattices and Lifting                                                    38

                                                                              V
vi                                                                                     Contents


     3.5   Different Points of View                                                         38
           Multiresolution versus Time-Frequency Analysis                                   38
           Periodic versus Nonperiodic Discrete Wavelet Transforms                          38
           The Discrete Wavelet Transform versus the Discrete-Time Wavelet Transform        39
           Numerical Complexity of the Discrete Wavelet Transform                           40

4 Bases, Orthogonal Bases, Biorthogonal Bases, Frames, Tight Frames, and Un-
  conditional Bases                                                          41
  4.1 Bases, Orthogonal Bases, and Biorthogonal Bases                        41
      Matrix Examples                                                        43
      Fourier Series Example                                                 44
      Sinc Expansion Example                                                 44
  4.2 1吐ames and 끄ght 짜ames                                                  45
      Matrix Examples                                                        46
      Sinc Expansion as a Tight Frame Example                                47
  4.3 Conditional and Unconditional Bases                                    48

5    The Scaling Function and Scaling Coefficients, Wavelet and Wavelet Coeffi-
     cients                                                                     50
     5.1 Tools and Definitions                                                  50
          Signal Classes                                                        50
          Fourier Transforms                                    .               51
          Refinement and Transition Matrices                                    52
     5.2 Necessary Conditions                                                   53
     5.3 Frequency Domain Necessary Conditions                                  54
     5.4 Sufficient Conditions                                                  56
          Wavelet System Design                                                 57
     5.5 The Wavelet                                                            58
     5.6 Alternate Normalizations                                               59
     5.7 Example Scaling 恥nctions and Wavelets                                  59
          Haar Wavelets                                                         60
          Sinc Wavelets                                                         60
          Spline and Battle-Lemari6 Wavelet Systems                             62
     5.8 Further Properties of the Scaling Function and Wavelet                 62
          General Properties not Requiring Orthogonality                        63
          Properties that Depend on Orthogonality                               64
     5.9 Parameterization of the Scaling Coefficients                           65
          Length그 Scaling Coefficient Vector                                    65
          Length-4 Scaling Coefficient Vector                                   66
          Length-6 Scaling Coefficient Vector                                   66
     5.10 Calculating the Basic Scaling Function and Wavelet                    67
          Successive Approximations or the Cascade Algorithm                    67
          Iterating the Filter Bank                                             68
          Successive approximations in the frequency domain                     68
          The Dyadic Expansion of the Scaling Function                          70
CONTENTS                                                                                 vii


6 Regularity, Moments, and Wavelet System Design                                         73
  6.1 K-Regular Scaling Filters                                                          73
  6.2 Vanishing Wavelet Moments                                                          75
  6.3 Daubechies' Method for Zero Wavelet Moment Design                                  76
  6.4 Non-Maximal Regularity Wavelet Design                                              83
  6.5 Relation of Zero Wavelet Moments to Smoothness                                     83
  6.6 Vanishing Scaling Function Moments                                                 86
  6.7 Approximation of Signals by Scaling Function Projection                            86
  6.8 Approximation of Scaling Coefficients by Samples of the Signal                     87
  6.9 Coiflets and Related Wavelet Systems                                               88
       Generalized Coifman Wavelet Systems                                               93
  6.10 Minimization of Moments Rather than Zero Moments                                  97

7   Generalizations of the Basic Multiresolution Wavelet System                           98
    7.1 Tiling the Time-Frequency or Time小Scale Plane                                     98
        Nonstationary Signal Analysis                                                     99
        Tiling with the Discrete-Time Short-Time Fourier Transform                       100
        Tiling with the Discrete Two-Band Wavelet Transform                              100
        General Tiling                                                                   101
    7.2 Multiplicity-M (M-Band) Scaling Functions and Wavelets                           102
        Properties of M-Band Wavelet Systems                                             103
        M-Band Scaling Function Design                                                   109
        M-Band Wavelet Design and Cosine Modulated Methods                               110
    7.3 Wavelet Packets                                                                  110
        Full Wavelet Packet Decomposition                                                110
        Adaptive Wavelet Packet Systems                                                  111
    7.4 Biorthogonal Wavelet Systems                                                     114
        Two-Channel Biorthogonal Filter Banks                                            114
        Biorthogonal Wavelets                                                            116
        Comparisons of Orthogonal and Biorthogonal Wavelets                              117
        Example Families of Biorthogonal Systems                                         118
        Cohen-Daubechies-Feauveau Family of Biorthogonal Spline Wavelets                 118
        Cohen-Daubechies-Feauveau Family of Biorthogonal Wavelets with Less Dissimilar
                Filter Length                                                            118
        Tian-Wells Family of Biorthogonal Coiflets                                       119
        Lifting Construction of Biorthogonal Systems                                     119
    7.5 Multiwavelets                                                                    122
        Construction of Two-Band Multiwavelets                                           123
        Properties of Multiwavelets                                                      124
        Approximation, Regularity and Smoothness                                         124
        Support                                                                          124
        0rthogonality                                                                    125
        Implementation of Multiwavelet Transform                                         125
        Examples                                                                         126
        Geronimo-Hardin-Massopust Multiwavelets                                          126
        Spline Multiwavelets                                                             127
Viii                                                                             Contents


       Other Constructions                                                           127
       Applications                                                                  128
   7.6 Overcomplete Representations, Frames, Redundant Transforms, and Adaptive Bases128
       Overcomplete Representations                                                  129
       A Matrix Example                                                              129
       Shift-Invariant Redundant Wavelet Transforms and Nondecimated Filter B什nks    132
       Adaptive Construction of Frames and Bases                                     133
   7.7 Local Trigonometric Bases                                                     134
       Nonsmooth Local Trigonometric Bases                                           136
       Cor坮缸uction of Smooth 砥lind이vs                                                136
       Folding and Unfolding                                                         137
       Local Cosine and Sine Bases                                                   139
       Signal Adaptive Local Trigonometric Bases                                     141
   7.8 I万screte 入4ultires아ution Analys坮） the I万screte-Time 砥ravelet
       Transform, and the Continuous Wavelet Transform                               141
       Discrete Multiresolution Analysis and the Discrete-Time Wavelet Transform     143
       Continuous Wavelet Transforms                                                 144
       Analogies between Fourier Systems and Wavelet Systems                         145

8 Filter Banks and Transmu此iplexers                                                 148
  8.1 Introduction                                                                  148
       The Filter Bank                                                              148
       Transmultiplexer                                                             150
       Perfect Reconstruction-A Closer Look                                         150
       Direct Characterization of PR                                                150
       Matrix characterization of PR                                                152
       Polyphase (Transform-Domain) Characterization of PR                          153
  8.2 Unitary Filter Banks            .                                             155
  8.3 Unitary Filter Banks-Some Illustrative Examples                               160
  8.4 M-band Wavelet Tight Frames                                                   162
  8.5 Modulated Filter Banks                                                        164
       Unitary Modulated Filter Bank                                                167
  8.6 Modulated Wavelet Tight Frames                                                168
  8.7 Linear Phase Filter Banks                                                      169
       Characterization of Unitary H (z) - PS Symmetry                              173
       Characterization of Unitary H (z) - PCS Symmetry                              174
       Characterization of Unitary H (z) 叫 Linear-Phase Symmetry                    174
       Characterization of Unitary H (z) 中 Linear Phase and PCS Symmetry            175
       Characterization of Unitary H (z) - Linear Phase and PS S戶llmetry            175
  8.8 Linear-Phase Wavelet Tight Frames                                              176
  8.9 Linear-Phase Modulated Filter Banks                                            177
       DCT/DST I/Il based 2M Channel Filter Bank                                     178
  8.10 Linear Phase Modulated Wavelet Tight Frames                                  178
  8.11 Time-Varying Filter Bank Trees                                               179
       Growing a Filter Bank Tree                                                   182
       Pruning a Filter Bank Tree                                                   182
CONTENTS                                                                              ix


         Wavelet Bases for the Interval                                              183
         ＼자avelet Bases for 1尸（[0，以）))                                               183
         ＼자avelet Bases 的r 夕 ((- 因이）                                                 184
         Segmented Time-Varying Wavelet Packet Bases                                 185
    8.12 Filter Banks and Wavelets呻Summary                                           186

9   Calculation of the Discrete Wavelet Transform                                   188
    9.1 Finite Wavelet Expansions and Transforms                                    188
    9.2 Periodic or Cyclic Discrete Wavelet Transform                               190
    9.3 Filter Bank Structures for Calculation of the DWT and Complexity            191
    9.4 The Periodic Case                                                            192
    9.5 Structure of the Periodic Discrete Wavelet Transform                         194
    9.6 More General Structures                                                      195

10 Wavelet-Based Signal Processing and Applications                                  196
   10.1 Wavelet-Based Signal Processing                                              196
   10.2 Approximate FFT using the Discrete Wavelet Transform                         197
        Introduction                                                                 197
        Review of the Discrete Fourier Transform and FFT                             198
        Review of the Discrete Wavelet Transform                                     200
        The Algorithm Development                                                    201
        Computational Complexity                                                     203
        Fast Approximate Fourier Transform                                           203
        Computational Complexity                                                     203
        Noise Reduction Capacity                                                     204
        Summary                                                                       204
   10.3 Nonlinear Filtering or Denoising with the DWT                                 205
        Denoising by Thresholding                                                     206
        Shift-Invariant or Nondecimated Discrete Wavelet Transform                    207
        Combining the Shensa-Beylkin-Mallat- trolls Algorithms and Wavelet Denoising 209
        Performance Analysis                                                          209
        Examples of Denoising                                                         210
   10.4 Statistical Estimation                                                        211
   10.5 Signal and Image Compression                                                 212
        Findamentals of Data Compression                                             212
        Prototype Transform Coder                                                    213
        Improved Wavelet Based Compression Algorithms                                215
   10.6 Why are Wavelets so Useful?                                                  216
   10.7 Applications                                                                 217
        Numerical Solutions to Partial Differential Equations                        217
        Seismic and Geophysical Signal Processing                                    217
        Medical and Biomedical Signal and Image Processing                           218
        Application in Communications                                                218
        Fractals                                                                     218
   10.8 Wavelet Software                                                             218
x                                                                  Contents



11 Summary Overview                                                   219
   11.1 Properties of the Basic Multiresolution Scaling Function      219
   11.2 Types of Wavelet Systems                                      221

12 References                                                         223

Bibliography                                                          224

Appendix A. Derivations for Chapter 5 on Scaling Functions            246

Appendix B. Derivations for Section on Properties                     253

Appendix C. Matlab Programs                                           258

Index                                                                 266
                                                                                  Preface


This book develops the ideas behind and properties of wavelets and shows how they can be used
as analytical tools for signal processing, numerical analysis, and mathematical modeling. We try
to present this in a way that is accessible to the engineer, scientist, and applied mathematician
both as a theoretical approach and as a potentially practic出 method to solve problems. Although
the roots of this subject go back some time, the modern interest and development have a history
of only a few years.
     The early work was in the 1980's by Morlet, Grossmann, Meyer, Mallat, and others, but it was
the paper by Ingrid Daubechies [Dau88a] in 1988 that caught the attention of the larger applied
mathematics communities in signal processing, statistics, and numerical analysis. Much of the
early work took place in France [CGT89, Mey92a] and the USA [Dau88a, RBC*92, Dau92, RV91}.
As in many new disciplines, the first work was closely tied to a particular application or traditional
theoretical framework. Now we are seeing the theory abstracted from application and developed
on its own and seeing it related to other parallel ideas. Our own background and interests in
signal processing certainly influence the presentation of this book.
     The goal of most modern wavelet research is to create a set of basis functions (or general
expansion functions) and transforms that will give an informative, efficient, and useful description
of a function or signal. If the signal is represented as a function of time, wavelets provide efficient
localization in both time and frequency or scale. Another central idea is that of multiresotution
where the decomposition of a signal is in terms of the resolution of detail.
     For the Fourier series, sinusoids are chosen as basis functions, then the properties of the
resulting expansion are examined. For wavelet analysis, one poses the desired properties and then
derives the resulting basis functions. An important property of the wavelet basis is providing
a multiresolution analysis. For several reasons, it is often desired to have the basis functions
orthonormal. Given these goals, you will see aspects of correlation techniques, Fourier transforms,
short-time Fourier transforms, discrete Fourier transforms, Wigner distributions, filter banks,
subband coding, and other signal expansion and processing methods in the results.
     Wavelet-based analysis is an exciting new problem-solving tool for the mathematician, scien-
tist, and engineer. It fits naturally with the digital computer with its basis functions defined by
summations not integrals or derivatives. Unlike most traditional expansion systems, the basis
 functions of the wavelet analysis are not solutions of differential equations. In some areas, it is the
 first truly new tool we have had in many years. Indeed, use of wavelets and wavelet transforms
requires a new point of view and a new method of interpreting representations that we are still
learning how to exploit.


                                                                                                     xi
xl '                                                                                        Preface


    More recently, work by Donoho, Johnstone, Coifman, and others have added theoretical
reasons for why wavelet analysis is so versatile and powerful, and have given generalizations that
are still being worked on. They have shown that wavelet systems have some inherent generic
advantages and are near optimal for a wide class of problems [Don93b]. They also show that
adaptive means can create special wavelet systems for particular signals and classes of signals.
     The multiresolution decomposition seems to separate components of a sign싫 in a way that is
superior to most other methods for analysis, processing, or compression. Because of the ability
of the discrete wavelet transform to decompose a signal at different independent scales and to do
it in a very fle虹ble way, Burke calls wavelets "The Mathematical Microscope" [Bur94, Hub96].
Because of this powerful and flexible decomposition, linear and nonlinear processing of signals in
the wavelet transform domain offers new methods for signal detection, filtering, and compression
[Don93b, Don95, Don93a, Sai94b, WTWB97, Guo97]. It also can be used as the basis for robust
numerical algorithms.
     You will also see an interesting connection and equivalence to filter bank theory from digital
signal processing [Vai92, AH92]. Indeed, some of the results obtained with filter banks are
the same as with discrete-time wavelets, and this has been developed in the signal processing
community by Vetterli, Vaidyanathan, Smith and Barnwell, and others. Filter banks, as well
as most algorithms for calculating wavelet transforms, are part of a still more general area of
multirate and time-varying systems.
     The presentation here will be as a tutorial or primer for people who know little or nothing
about wavelets but do have a technical background. It assumes a knowledge of Fourier series
and transforms and of linear algebra and matrix theory. It also assumes a background equivalent
to a B.S. degree in engineering, science, or applied mathematics. Some knowledge of signal
processing is helpful but not essential. We develop the ideas in terms of one-dimensional signals
[RV91] modeled as real or perhaps complex functions of time, but the ideas and methods have
also proven effective in image representation and processing [5A92, Mal89a] dealing with two,
three, or even four dimensions. Vector spaces have proved to be a natural setting for developing
both the theory and applications of wavelets. Some background in that area is helpful but can
be picked up as needed. The study and understanding of wavelets is greatly assisted by using
some sort of wavelet software system to work out examples and run experiments. MATLABTM
programs are included at the end of this book and on our web site (noted at the end of the
preface). Several other systems are mentioned in Chapter 10.
     There are several different approaches that one could take in presenting wavelet theory. We
have chosen to start with the representation of a signal or function of continuous time in a series
expansion, much as a Fourier series is used in a Fourier analysis. From this series representation,
we can move to the expansion of a function of a discrete variable (e.g., samples of a signal) and
the theory of filter banks to efficiently calculate and interpret the expansion coefficients. This
 would be analogous to the discrete Fourier transform (DFT) and its efficient implementation. the
 fast Fourier transform (FFT). We can also go from the series expansion to an integral transform
called the continuous wavelet transform, which is analogous to the Fourier transform or Fourier
integral. We feel starting with the series expansion gives the greatest insight and provides ease
in seeing both the similarities and differences with Fourier analysis.
     This book is organized into sections and chapters, each somewhat self-contained. The earlier
chapters give a fairly complete development of the discrete wavelet transform (DWT) as a series
expansion of signals in terms of wavelets and scaling functions. The later chapters are short
descriptions of generalizations of the DWT and of applications. They give references to other
Preface                                                                                        xiii


works, and serve as a sort of annotated bibliography. Because we intend this book as an intro-
duction to wavelets which already have an extensive literature, we have included a rather long
bibliography. However, it will soon be incomplete because of the large number of papers that are
currently being published. Nevertheless, a guide to the other literature is essenti出 to our goal of
an introduction.
    A good sketch of the philosophy of wavelet analysis and the history of its development can be
found in a recent book published by the National Academy of Science in the chapter by Barbara
Burke [Bur94]. She has written an excellent expanded version in [Hub96], which should be read
by anyone interested in wavelets. Daubechies gives a brief history of the early research in [Dau96].
    Many of the results and relationships presented in this book are in the form of theorems and
proofs or derivations. A real effort has been made to ensure the correctness of the statements of
theorems but the proofs are often only outlines of derivations intended to give insight into the
result rather than to be a formal proof. Indeed, many of the derivations are put in the Appendix
in order not to clutter the presentation. We hope this style will help the reader gain insight into
this very interesting but sometimes obscure new mathematical signal processing tool.
    We use a notation that is a mixture of that used in the signal processing literature and that
in the mathematical literature. We hope this will make the ideas and results more accessible, but
some uniformity and cleanness is lost.
    The authors acknowledge AFOSR, ARPA, NSF, Nortel, Inc., Texas Instruments, Inc. and
Aware, Inc. for their support of this work. We specifically thank H. L. Resni毗 who first
introduced us to wavelets and who proved remarkably accurate in predicting their power and
success. We also thank W. M. Lawton, R. 0. Wells, Jr., R. G. Baraniuk, J. E. Odegard, I. W.
Selesnick, M. Lang, J. Tian, and members of the Rice Computational Mathematics Laboratory
for many of the ideas and results presented in this book. The first named author would like to
thank the Ma咀eld and Oshman families for their generous support. The students in EE-531
and EE-696 at Rice University provided valuable feedback as did Bruce Francis, Strela Vasily,
Hans Schflssler, Peter Steffen, Gary Sitton, Jim Lewis, Yves Angel, Curt Michel, J. H. Husoy,
Kjersti Engan, Ken Castleman, Jeff Trinkle, Katherine Jones, and other colleagues at Rice and
elsewhere.
    We also particularly want to thank Tom Robbins and his colleagues at Prentice Hall for theii
support and help. Their reviewers added significantly to the book.
    We would appreciate learning of any errors or misleading statements that any readers dis-
cover. Indeed, any suggestions for improvement of the book would be most welcome. Send
suggestions or comments via email to csb@rice.edu. Software, articles, errata for this book, and
other information on the wavelet research at Rice can be found on the world-wide-web URL:
http://www-dsp.rice.edu/ with links to other sites where wavelet research is being done.

C. Sidney Burrus, Ramesh A. Gopinath, and Haitao Guo
Houston, Texas, Yorktown Heights, New York, and Sunnyvale, California
xiv                                                                                       Preface


Instructions to the Reader
Although this book in arranged in a somewhat progressive order, starting with basic ideas and
definitions, moving to a rather complete discussion of the basic wavelet system, and then on to
generalizations, one should skip around when reading or studying from it. Depending on the
background of the reader, he or she should skim over most of the book first, then go back and
study parts in detail. The Introduction at the beginning and the Summary at the end should
be continually consulted to gain or keep a perspective; similarly for the Table of Contents and
Index. The MATLAB programs in the Appendix or the Wavelet Toolbox from Mathworks or other
wavelet software should be used for continual experimentation. The list of references should be
used to find proofs or detail not included here or to pursue research topics or applications. The
theory arid application of wavelets are still developing and in a state of rapid growth. We hope
this book will help open the door to this fascinating new subject.
Chapter 1


                               Introduction to Wavelets


This chapter will provide an overview of the topics to be developed in the book. Its purpose is
to present the ideas, goals, and outline of properties for an understanding of and ability to use
wavelets and wavelet transforms. The details and more careful definitions are given later in the
book.
    A wave is usually defined as an oscillating function of time or space, such as a sinusoid.
Fourier analysis is wave analysis. It expands signals or functions in terms of sinusoids (or,
equivalently, complex exponentials) which has proven to be extremely valuable in mathematics,
science, and engineering, especially for periodic, time-invariant, or stationary phenomena. A
wavelet is a "small wave", which has its energy concentrated in time to give a tool for the
analysis of transient, nonstationary, or time-varying phenomena. It still has the oscillating wave-
like characteristic but also has the ability to allow simultaneous time and frequency analysis with
a flexible mathematical foundation. This is illustrated in Figure 1.1 with the wave (sinusoid)
oscillating with equal amplitude over -以） 드 t 5 :: and, therefore, having infinite energy and
with the wavelet having its finite energy concentrated around a point.




                                                           가             뇨HH
                       (a) A Sine Wave                 (b) Daubechies' Wavelet 砂D2o

                              Figure 1.1. A Wave and a Wavelet



   We will take wavelets and use them in a series expansion of signals or functions much the
same way a Fourier series uses the wave or sinusoid to represent a signal or function. The signals
are functions of a continuous variable, which often represents time or distance. From this series
expansion, we will develop a discrete-time version similar to the discrete Fourier transform where
the signal is represented by a string of numbers where the numbers may be samples of a signal,

                                                                                                 1
2                                                              Introduction to Wavelets and Transforms   Ch. 1



samples of another string of numbers, or inner products of a signal with some expansion set.
Finally, we will briefly describe the continuous wavelet transform where both the signal and the
transform are functions of continuous variables. This is analogous to the Fourier transform.


1.1    Wavelets and Wavelet Expansion Systems
Before delving into the details of wavelets and their properties, we need to get some idea of their
general characteristics and what we are going to do with them [Swe96b].

What is a Wavelet Expansion or a Wavelet Transform?
A signal or function f (t) can often be better analyzed, described, or processed if expressed as a
linear decomposition by
                                           f(t) = ＞二仰吻（t)                                                (1.1)
                                                     e

where Z is an integer index for the finite or infinite sum, at are the real-valued expansion coe玗i-
cients, and 吻（t) are a set of real-valued functions of t called the expansion set. If the expansion
(1.1) is unique, the set is called a basis for the class of functions that can be so expressed. If the
basis is orthogonal, meaning

                       佃小） （t))=
                              ，吻            ／仇   （t）吻（t) dt= .               （尹   『，
                                                                                                         (1.2)

then the coefficients can be calculated by the inner product

                                                                                                         (1.3)
                                   따 =   (/(!）肋小）)       三／   /(!）仇（t) dt.
One can see that substituting (1.1) into (1.3) and using (1.2) gives the single ak coefficient. If
the basis set is not orthogonal, then a dual basis set 仇(t) exists such that using (1.3) with the
dual basis gives the desired coefficients. This will be developed in Chapter 2.
    For a Fourier series, the orthogonal basis functions 仇(t) are sin(kwot) and cos(kwot) with
frequencies of kw0. For a Taylor 's series, the nonorthogonal basis functions are simple monomials
tk, and for many other expansions they are various polynomials. There are expansions that use
splines and even fractals.
    For the wavelet expansion, a two-parameter system is constructed such that (1.1) becomes

                                         f(t) = ＞二＞二a3,k砂j,k(t)                                          (1.4)
                                                 k   j

where both j and k are integer indices and the 砂 j,k (t) are the wavelet expansion functions that
usually form an orthogonal basis.
   The set of expansion coefficients a7, 丸 are called the discrete wavelet transform (DWT) of 1 (t)
and (1.4) is the inverse transform.

What is a Wavelet System?
The wavelet expansion set is not unique. There are many different wavelets systems that can be
used effectively, but all seem to have the following three general characteristics [Swe96b].
Sec. 1.1. Wavelets and Wavelet Expansion Systems
                                                                                                     3


   1. A wavelet system is a set of building blocks to construct or represent a signal or function.
      It is a tw아dimensional expansion set (usually a basis) for some class of one- (or higher)
      dimensional signals. In other words, if the wavelet set is given by 砂i,k (t) for indices of
      j, k = 1, 2,..., a linear expansion would be 1 (t) = i2k >23 a3,k砂3,k(t) for some set of
      coefficients a3,k.

   2. The wavelet expansion gives a time-frequency localization of the signal. This means most
      of the energy of the signal is well represented by a few expansion coefficients, a3,k.

   3. The calculation of the coefficients from the signal can be done efficiently. It turns out
      that many wavelet transforms (the set of expansion coefficients) can calculated with O(N)
      operations. This means the number of floating-point multiplications and additions increase
      linearly with the length of the signal. More general wavelet transforms require O(Nlog(N))
      operations, the same as for the f戚 Fourier transform (FFT) [BP85].

Virtually all wavelet systems have these very general characteristics. Where the Fourier series
maps a one-dimensional function of a continuous variable into a one-dimensional sequence of
coefficients, the wavelet expansion maps it into a two-dimensional array of coefficients. We will
see that it is this two-dimensional representation that allows localizing the signal in both time and
frequency. A Fourier series expansion localizes in frequency in that if a Fourier series expansion
of a signal has only one large coefficient, then the signal is essentially a single sinusoid at the
frequency determined by the index of the coefficient. The simple time-domain representation of
the signal itself gives the localization in time. If the signal is a simple pulse, the location of that
pulse is the localization in time. A wavelet representation will give the location in both time and
frequency simultaneously. Indeed, a wavelet representation is much like a musical score where
the location of the notes tells when the tones occur and what their frequencies are.

More Specific Characteristics of Wavelet Systems
There are three additional characteristics [Swe96b, Dau92] that are more specific to wavelet
expansions.

  1. All so-called first-generation wavelet systems are generated from a single scaling function
     or wavelet by simple scaling and translation. The two-dimensional parameterization is
     achieved from the function (sometimes called the generating wavelet or mother wavelet)
     砂（t) by
                               吻，小） = 23/2砂（23t -丸）            3, 丸EZ                      (1.5)
     where Z is the set of all integers and the factor 23/2 maintains a constant norm independent
     of scale j. This parameterization of the time or space location by k and the frequency or
     scale (actually the logarithm of scale) by j turns out to be extraordinarily effective.

  2. Almost all useful wavelet systems also satisfy the multiresolution conditions. This means
     that if a set of signals can be represented by a weighted sum of o(t - k), then a larger set
     (including the original) can be represented by a weighted sum of 99(2t - k). In other words,
     if the basic expansion signals are made half as wide and translated in steps half as wide,
     they will represent a larger class of signals exactly or give a better approximation of any
     signal.
4                                                                       Introduction to Wavelets and Transforms   Ch. 1


    3. The lower resolution coefficients can be calculated from the higher resolution coefficients
       by a tree-structured algorithm called a filter bank. This allows a very efficient calculation
       of the expansion coefficients (also known as the discrete wavelet transform) and relates
       wavelet transforms to an older area in digital signal processing.

    The 아光r毗油瑁 可 translation and scaling seem 的 be basic to ma파 practical signals and signal-
generating processes, and their use is one of the reasons that wavelets are efficient expansion
functions. Figure 1.2 is a pictorial representation of the translation and scaling of a single
mother wavelet described in (1.5). As the index k changes, the location of the wavelet moves
along the horizontal axis. This allows the expansion to explicitly represent the location of events
in time or space. As the index j changes, the shape of the wavelet changes in scale. This allows
a representation of detail or resolution. Note that as the scale becomes finer (j larger), the
steps in time become smaller. It is both the narrower wavelet and the smaller steps that allow
representation of greater detail or higher resolution. For clarity, only every fourth term in the
translation (k = 1, 5, 9, 13, . . .) is shown, otherwise, the figure is a clutter. What is not illustrated
here but is important is that the shape of the basic mother wavelet can also be changed. That
is done during the design of the wavelet system and allows one set to well-represent a class of
signals.
    For the Fourier series and transform and for most signal expansion systems, the expansion
functions (bases) are chosen, then the properties of the resulting transform are derived and

                  .7
                                                                    1       1        1        1



              3            人                 人            八                                       人   \\
                       \       \＼뇌               \\           \＼늬




                           1         1




              2




              1

                                                                                                           丸
                       1         2       3            4             5           6        7        8

             Figure 1.2. Translation (every fourth k) and Scaling of a Wavelet 砂D4
Sec. 1.1. Wavelets and Wavelet Expansion Systems                                                    5


analyzed. For the wavelet system, these properties or characteristics are mathematically required,
then the resulting basis functions are derived. Because these constraints do not use all the degrees
of freedom, other properties can be required to customize the wavelet system for a particular
application. Once you decide on a Fourier series, the sinusoidal basis functions are completely
set. That is not true for the wavelet. There are an infinity of very different wavelets that all
satisfy the above properties. Indeed, the understanding and design of the wavelets is an important
topic of this book.
    Wavelet analysis is well-suited to transient signals. Fourier analysis is appropriate for periodic
signals or for signals whose statistical characteristics do not change with time. It is the localizing
                                                                                               with a
property of wavelets that allow a wavelet expansion of a transient event to be modeled
small number of coefficients. This turns out to be very useful in applications.

Haar Scaling Functions and Wavelets
The multiresolution formulation needs two closely related basic functions. In addition to the
wavelet 砂 (t) that has been discussed (but not actually defined yet), we will need another basic
                                                                                          details of
function called the scaling function p(t). The reasons for needing this function and the
the relations will be developed in the next chapter, but here we will simply  use it in the wavelet
expansion.
   The simplest possible orthogonal wavelet system is generated from the Haar scaling function
and wavelet. These are shown in Figure 1.3. Using a combination of these scaling functions and
wavelets allows a large class of signals to be represented by
                                    00                   00       m


                         1(t) = Z CkO(t中k) + ＞二 ＞二d3,k砂（23t -丸）·
                                                       k= -아그 j= o
                                                                                                 (1.6)
                                  k= H以）


Haar [Haal0l showed this result in 1910, and we now know that wavelets are a generalization of
his work. An example of a Haar system and expansion is given at the end of Chapter 2.

 What do Wavelets Look Like?
 All Fourier basis functions look alike. A high-frequency sine wave looks like a compressed low-
                                                                                         takes a
 frequency sine wave. A cosine wave is a sine wave translated by 90O or ir/2 radians. It




                                                                       1                t
                                                   t                                1

                    0                                         0




                               (a) 中（t)                               (b) 砂（t)

                            Figure 1.3. Haar Scaling Function and Wavelet
6                                                                Introduction to Wavelets and Transforms   Ch. 1


large number of Fourier components to represent a discontinuity or a sharp corner. In contrast,
there are many different wavelets and some have sharp corners themselves.
    To appreciate the special character of wavelets you should recognize that it was not until the
late 1980's that some of the most useful basic wavelets were ever seen. Figure 1.4 illustrates four
different scaling functions, each being zero outside of 0 < t < 6 and each generating an orthogonal
wavelet basis for all square integrable functions. This figure is also shown on the cover to this
book.
    Several more scaling functions and their associated wavelets are illustrated in later chapters,
and the Haar wavelet is shown in Figure 1.3 and in detail at the end of Chapter 2.


                                                          1.2
                                                            1
                                                          0.8
                                                          0.6
                                                          0.4
                                                          0.2
                                                           0
                                                         -0.2
                                                         -0.4
                                                             0        1       2   3     4      5
                  (a) 中C石 : a == 1.3598戶 = -0.7821         (b) 中D6 : a = 1.1468, 乃 = 0.42403

                  1-
                0.8 ,

                0月,

                0.4-

                0.2 ,

                  0-

               -0.2-
                   0      1     2     3         4    5            1       2       3    4       5

                        (c) a 亡 릉긍r, 8 = -古7r                     (d) a = 和万 = 長7r
      Figure 1.4. Example Scaling Functions (See Section 5.8 for the Meaning of a and 3)




Why is Wavelet Analysis Effective?
Wavelet expansions and wavelet transforms have proven to be very efficient and effective in
analyzing a very wide class of signals and phenomena. Why is this true? What are the properties
that give this effectiveness?

    1. The size of the wavelet expansion coefficients a3,k in (1.4) or d3,k in (1.6) drop off rapidly
       with j and k for a large class of signals. This property is called being an unconditional
       basis and it is why wavelets are so effective in signal and image compression, denoising, and
       detection. Donoho [Don93b, DJKP95b] showed that wavelets are near optimal for a wide
       class of signals for compression, denoising, and detectkn.
                                                                                                 7
Sec. 1.2. The Discrete Wavelet Transform


   2. The wavelet expansion allows a more accurate local description and separation of signal
      characteristics. A Fourier coefficient represents a component that lasts for all time and,
      therefore, temporary events must be described by a phase characteristic that allows cancel-
      lation or reinforcement over large time periods. A wavelet expansion coefficient represents
      a component that is itself local and is easier to interpret. The wavelet expansion may allow
      a separation of components of a signal that overlap in both time and frequency.

   3. Wavelets are adjustable and adaptable. Because there is not just one wavelet, they can
      be designed to fit individual applications. They are ideal for adaptive systems that adjust
      themselves to suit the signal.

   4. The generation of wavelets and the calculation of the discrete wavelet transform is well
      matched to the digital computer. We will later see that the defining equation for a wavelet
      uses no calculus. There are no derivatives or integrals, just multiplications and additions中
      operations that are basic to a digital computer.

While some of these details may not be clear at this point, they should point to the issues that
are important to both theory and application and give reasons for the detailed development that
follows in this and other books.


1.2     The Discrete Wavelet Transform
This two-variable set of basis functions is used in a way similar to the short-time Fourier trans-
form, the Gabor transform, or the Wigner distribution for time-frequency analysis [Coh89, Coh95,
HB92]. Our goal is to generate a set of expansion functions such that any signal in L2(R) (the
space of square integrable functions) can be represented by the series

                                       f (t) = Z呼 少砂偕卜 丸）                                      (1.7)
                                                   2大


 or, using (1.5), as
                                           f (t) = ＞二口j,k砂3,k (t)                              (1.8)
                                                             3小

 where the two-dimensional set of coefficients a3,k is called the discrete wavelet transform (DWT)
 of f (t). A more specific form indicating how the a3,k 's are calculated can be written using inner
 products as
                                     1(t) =＞二 (砂j,k(t), 1(t))砂j,k(t)                           (1.9)
                                                   3小

 if the 砂j,k (t) form an orthonormal basis1 for the space of signals of interest [Dau92]. The inner
 product is usually defined as
                                                                                              (1.10)
                                       佃(t)   ,y
                                                   (t)
                                                         )   =    fx*
                                                                        (t)
                                                                              y
                                                                                  (t)
                                                                                        dt.

    1Bases and tight frames are defined in Chapter 4.
 8                                                                  Introduction to Wavelets and Transforms           Ch. 1


     The goal of most expansions of a function or signal is to have the coefficients of the expansion
 a3,k give more useful information about the signal than is directly obvious from the signal itself.
 A second goal is to have most of the coefficients be zero or very small. This is what is called
 a sparse representation and is extremely important in applications for statistical estimation and
detection, data compression, nonlinear noise reduction, and fa就 algorithms.
     Although this expansion is called the discrete wavelet transform (DWT), it probably should
be called a wavelet series since it is a series expansion which maps a function of a continuous
variable into a sequence of coefficients much the same way the Fourier series does. However, that
is not the convention.
     This wavelet series expansion is in terms of two indices, the time translation k and the scaling
index j. For the Fourier series, there are oniy two possible values of k, zero and ir/2, which give
the sine terms and the cosine terms. The values j give the frequency harmonics. In other words,
the Fourier series is also a tw아dimensional expansion, but that is not seen in the exponential
form and generally not noticed in the trigonometric form.
     The DWT of a signal is somewhat difficult to illustrate because it is a function of two variables
or indices, but we will show the DWT of a simple pulse in Figure 1.5 to illustrate the localization
of the transform. Other displays will be developed in the next chapter.




                                                          (           r




                      I   I   I   I   I   I   I   .   .
                                                          I   1111111I    I   I   I   1   I   I   I   r   I   I   1


Figure 1.5. Discrete Wavelet Transform of a Pulse, using 砂D6 with a Gain of \／牙 for Each
Higher Scale.




1.3    The Discrete-Time and Continuous Wavelet Transforms
If the signal is itself a sequence of numbers, perhaps samples of some function of a continuous
variable or perhaps a set of inner products, the expansion of that signal is called a discrete-time
Sec. 1.4. Exercises and Experiments                                                                           9


wavelet transform (DTWT). It maps a sequence of numbers into a sequence of numbers much the
same way the discrete Fourier transform (DFT) does. It does not, however, require the signal to
be finite in duration or periodic as the DFT does. To be consistent with Fourier terminology, it
probably should be called the discrete-time wavelet series, but this is not the convention. If the
discrete-time signal is finite in length, the transform can be represented by a finite matrix. This
formulation of a series expansion of a discrete-time signal is what filter bank methods accomplish
[Vai92, VK95] and is developed in Chapter 8 of this book.
   If the signal is a function of a continuous variable and a transform that is a function of two
continuous variables is desired, the continuous wavelet transform (CWT) can be defined by


                                                                                                      毗
                                        「    （.       力）   =
                                                               //(!        ）『           （늑프）
with an inverse transform of


                                      /(!)        =    /／「力）          （.        ?（늑므）          （扼db
                                                                                                          (1.12)

where w(t) is the basic wavelet and a, b E R are real continuous variables. Admissibility conditions
for the wavelet w(t) to support this invertible transform is discussed by Daubechies [Dau92], Heil
and Walnut [HW89], and others and is briefly developed in Section 7.8 of this book. It is analogous
to the Fourier transform or Fourier integral.


1.4     Exercises and Experiments

As the ideas about wavelets and wavelet transforms are developed in this book, it will be very
helpful to experiment using the Matlab programs in the appendix of this book or in the MATLAB
Toolbox [MMOP96]. An effort has been made to use the same notation in the programs in 4
Appendix C as is used in the formulas in the book so that going over the programs can help in
understanding the theory and vice versa.


1.5     This Chapter
This chapter has tried to set the stage for a careful introduction to both the theory and use of
wavelets and wavelet transforms. We have presented the most basic characteristics of wavelets
and tried to give a feeling of how and why they work in order to motivate and give direction and
structure to the following material.
    The next chapter will present the idea of multiresolution, out of which will develop the scaling
function as well as the wavelet. This is followed by a discussion of how to calculate the wavelet
expansion coefficients using filter banks from digital signal processing. Next, a more detailed
development of the theory and properties of scaling functions, wavelets, and wavelet transforms
is given followed by a chapter on the design of wavelet systems. Chapter 8 gives a detailed
development of wavelet theory in terms of filter banks.
    The earlier part of the book carefully develops the basic wavelet system and the later part
develops several important generalizations, but in a less detailed form.
 Chapter 2


           A Multiresolution Formulation of
                           Wavelet Systems


Both the mathematics and the practical interpretations of wavelets seem to be best served by
using the concept of resolution [Mey93, Mal89b, Ma189c, Dau92} to define the effects of changing
scale. To do this, we will start with a scaling function 甲(t) rather than directly with the wavelet
  (t). After the scaling function is defined from the concept of resolution, the wavelet functions
 will be derived from it. This chapter will give a rather intuitive development of these ideas, which
will be followed by more rigorous arguments in Chapter 5.
    This multiresolution formulation is obviously designed to represent signals where a single
event is decomposed into finer and finer detail, but it turns out also to be valuable in representing
signals where a time-frequency or time-scale description is desired even if no concept of resolution
is needed. However, there are other cases where multiresolution is not appropriate, such as for
the short-time Fourier transform or Gabor transform or for local sine or cosine bases or lapped
orthogonal transforms, which are all discussed briefly later in this book.


2.1    Signal Spaces

In order to talk about the collection of functions or signals that can be represented by a sum of
scaling functions and/or wavelets, we need some ideas and terminology from functional analysis.
If these concepts are not familiar to you or the information in this section is not sufficient, you
may want to skip ahead and read Chapter 5 or [VD95].
    A function space is a linear vector space (finite or infinite dimensional) where the vectors are
functions, the scalars are real numbers (sometime complex numbers), and scalar multiplication
and vector addition are similar to that done in (1.1). The inner product is a scalar a obtained
from two vectors, 1 (t) and g(t), by an integr毗 It is denoted



                                a =   (f(t)   ,g
                                                   (t)
                                                         )   =   f   f*
                                                                          (t)
                                                                                g
                                                                                    (t)
                                                                                          dt   (2.
                                                                                                     1)
with the range of integration depending on the signal class being considered. This inner product
defines a norm or "length" of a vector which is denoted and defined by


                                         11111 = ＼기(f,f)I                                      (2.2)

10
 Sec. 2.2. The Scaling Function                                                                  11

 which is a simple generalization of the geometric operations and definitions in three中dimensional
Euclidean space. Two signals (vectors) with lion-zero norms are called orthogonal if their inner
product is zero. For example, with the Fourier series, we see that sin(t) is orthogonal to sin(2t).
     A space that is particularly important in signal processing is call L2(R). This is the space of
all functions 1 (t) with a well defined integral of the square of the modulus of the function. The
 "L" signifies a Lebesque integral, the "2" denotes the integral of the square of the modulus of
the function, and R states that the independent variable of integration t is a number over the
whole real line. For a function g(t) to be a member of that space is denoted: g E L2(R)
                                                                                           or simply
g E L2.
    Although most of the definitions and derivations are in terms of signals that are in L2, many
of the results hold for larger classes of signals. For example, polynomials 缸e not in L2 but
                                                                                                 can
be expanded over any finite domain by most wavelet systems.
    In order to develop the wavelet expansion described in (1.5), we will need the idea of an
expansion set or a basis set. If we start with the vector space of signals, S, then if any 1 (t) E S
can be expressed as 1 (t) = ）二k ak cc'k(t), the set of functions Ok (t) are called an expansion set
for the space S. If the representation is unique, the set is a basis. Alternatively, one could start
with the expansion set or basis set and define the space S as the set of all functions that can be
expressed by 1 (t) = ＞二k ak pk (t). This is called the span of the basis set. In several cases, the
signal spaces that we will need are actually the closure of the space spanned by the basis set.
That means the space contains not only all signals that can be expressed by a linear combination
of the basis functions, but also the signals whi血 are the limit of these infinite expansions. The
closure of a space is usually denoted by an over-line.


2.2     The Scaling Function

In order to use the idea of multiresolution, we will start by defining the scaling function and then
define the wavelet in terms of it. As described for the wavelet in the previous chapter, we define
a set of scaling functions in terms of integer translates of the basic scaling function by

                              CPk (t) = 甲（t - 丸）           丸 EZ       97E L2.                  (2.3)

The subspace of L2(R) spanned by these functions is defined as

                                             V0 = Span{ o丸(t)}                                (2.4)
                                                      Ic

for all integers k from minus infinity to infinity. The over-bar denotes closure. This means that


                                  f (t) =Z akcak(t)        forany   f(t) EV0.                 (2.5)
                                         k

One can generally increase the size of the subspace spanned by changing the time scale of the
scaling functions. A two-dimensional family of functions is generated from the basic scaling
function by sealing and translation by

                                         P3,k(t) = 2j/2甲(2jt - k)                             (2.6)
12                                                                      A Multiresolution Formulation    Ch. 2


whose span over k is

                               vi = Span{ ,k (2it)} = Span{y)j,k(t)}                                     (2.7)
                                       k                     k


for all integers k E Z. This means that if 1 (t) E V3, then it can be expressed as


                                     f (t) = Z ak,(2j나k).                                                (2.8)
                                               k


    For j > 0, the span can be larger since coj,k (t) is narrower and is translated in smaller steps.
It, therefore, can represent finer detail. For j < 0, cpj,k (t) is wider and is translated in larger
steps. So these wider scaling functions can represent only coarse information, and the space
they span is smaller. Another way to think about the effects of a change of scale is in terms of
resolution. If one talks about photographic or optical resolution, then this idea of scale is the
same as resolving power.


Multiresolution Analysis
In order to agree with our intuitive ideas of scale or resolution, we formulate the basic requirement
of multiresolution analysis (MRA) [Mal89c] by requiring a nesting of the spanned spaces as

                           · · .cV_ 2cV_1cV0cV1cV2c. . ·cL2                                              (2.9)

or

                                     V3CV+1        forall    jEZ                                        (2.10)

with

                                  VH乂 = {0},                V生. = L2.                                   (2.11)

The space that contains high resolution signals will contain those of lower resolution also.
   Because of the definition of V, the spaces have to satisfy a natural scaling condition


                                  f (t) E V3   件      f (2t) E V+i                                      (2.12)

which insures elements in a space are simply scaled versions of the elements in the next space.
The relationship of the spanned spaces is illustrated in Figure 2.1.
    The nesting of the spans of 甲(2jt - k), denoted by V3 and shown in (2.9) and (2.12) and
graphically illustrated in Figure 2.1, is achieved by requiring that 甲(t) E V1, which means that if
99(t) is in Vo, it is also in V1, the space spanned by 甲(2t). This means 99(t) can be expressed in
terms of a weighted sum of shifted 甲(2t) as


                             甲(t) = >二h(n) v'2甲(2t - n),           nE Z                                 (2.13)
Sec. 2.2. The Sca'ing Function                                                                     13



                                                               V3 j V2 D V1 J V0




               Figure 2.1. Nested Vector Spaces Spanned by the Scaling Functions


where the coefficients h(미 are a sequence of real or perhaps complex numbers called the scaling
function coefficients (or the scaling filter oi the scaling vector) and the /2 maintains the norm
of the scaling function with the scale of two.
    This recursive equation is fundamental to the theory of the scaling functions and is, in some
ways, analogous to a differential equation with coefficients h(n) and solution 甲(t) that may or
may not exist or be unique. The equation is referred to by different names to describe different
interpretations or points of view. It is called the refinement equation, the multiresolution analysis
(MRA) equation, or the dilation equation.
    The Haar scaling function is the simple unit-width, unit-height pulse function 99(t) shown in
Figure 2.2, and it is obvious that 99 (2t) can be used to construct 甲(t) by


                                        甲(t) = 甲(2t) + Y7(2t - 1)                              (2.14)


which means (2.13) is satisfied for coefficients h(O) = i/ \/, h(1) = 1/ v' .
   The triangle scaling function (also a first order spline) in Figure 2.2 satisfies (2.13) for h(O) =
功5, h(1) =          , h(2) = 沅, and the Daubechies scaling function shown in the first part of




                 砂（t) = 砂（2t) + 中（2t - 1)             中（t) = 如位나 可갸 -1) + 如（2t -2)

                   (a) Haar (same as 99i)2)                  (b) Triangle (same as 'si)

                          Figure 2.2. Haar and Triangle Scaling Functions
14                                                                          A Multiresolution Formulation         Ch. 2


Figure 6.1 satisfies (2.13) for h = {0.483, 0.8365, 0.2241, -0.1294} as do all scaling functions for
their corresponding scaling coefficients. Indeed, the design of wavelet systems is the choosing of
the coefficients h(미 and that is developed later.


2.3    The Wavelet Functions
The important features of a signal can better be described or parameterized, not by using c77,k (t)
and increasing j to increase the size of the subspace spanned by the scaling functions, but by
defining a slightly different set of functions 砂j,k (t) that span the differences between the spaces
spanned by the various scales of the scaling function. These functions are the wavelets discussed
in the introduction of this book.
    There are several advantages to requiring that the scaling functions and wavelets be orthog-
onal. Orthogonal basis functions allow simple calculation of expansion coefficients and have a
Parseval's theorem that allows a partitioning of the signal energy in the wavelet transform do-
main. The orthogonal complement of V in V3+1 is defined as W. This means that all members
of V3 are orthogonal to all members of W3. We require


                          佃恥
                               （!
                                    )，吻．
                                             小）)   =
                                                       ／吻，   (
                                                                 (!
                                                                      ）吻小）dt= .                             (2.
                                                                                                                   15)


for all appropriate j, k, f E Z.
    The relationship of the various subspaces can be seen from the following expressions. From
(2.9) we see that we may start at any V3, say at j = 0, and write

                                            V0CV1CV2C · · ·CL2.                                             (2.16)

We now define the wavelet spanned subspace Wo such that

                                                 V1 = V0 qW0                                                (2.17)

which extends to
                                              V2 = V0 e Wo 由끼11.                                            (2.18)

In general this gives
                                            L2 = % 由 wo 由 比 由 · . ·                                         (2.19)

when V0 is the initial space spanned by the scaling function 甲(t - k). Figure 2.3 pictorially shows
the nesting of the scaling function spaces V3 for different scales j and how the wavelet spaces are
the disjoint differences (except for the zero element) or, the orthogonal complements.
   The scale of the initial space is arbitrary and could be chosen at a higher resolution of, say,
j = 10 to give
                                           L2 = V1。由끼710田Wi1田· · ·                                          (2.20)

or at a lower resolution such as j = -5 to give

                                           L2 =｝乙5e14乙5由）A乙4由· · ·                                          (2.21)
Sec. 2.3. The Wavetet Functions
                                                                                                  15


                           功／2 JWi 上 }'120 上 V0                  V3 D V2 D Vi D Vo




                     Figure 2.3. Scaling Function and Wavelet Vector Spaces


or at even j = -以） where (2.19) becomes

                           L2 = · · · 4) )A乙2 由 )'1乙1 侄） wo 4) 'vi 田 m72 任）· . ·               (2.22)

eliminating the scaling space altogether and allowing an expansion of the form in (1.9).
    Another way to describe the relation of Vo to the wavelet spaces is noting

                                         w以）由 ' · · 田 )'v-i = V0                               但23)

which again shows that the scale of the scaling space can be chosen arbitrarily. In practice, it is
usually chosen to represent the coarsest detail of interest in a signal.
   Since these wavelets reside in the space spanned by the next narrower scaling function, Wo C
                                                                                            (2.13)
V1, they can be represented by a weighted sum of shifted scaling function p(2t) defined in
by
                                  砂(t) = >二h1(n) /o (2t- n),         nEZ                       (2.24)
                                          n



for some set of coefficients h1(n). 价om the requirement that the wavelets span the "difference"
                                                                                           wavelet (or
or orthogonal complement spaces, and the orthogonality of integer translates of the
scaling function), it is shown in the Appendix in (12.48)    that the  wavelet  coefficients (modulo
translations by integer multiples of two) are required by orthogonali ty to be related  to the scaling
ftinction coefficients by
                                      hi(n) = (- 1)'h (1 - n). .                                (2.25)

One example for a finite even length-N h(n) could be

                                      hi(n) = (- 伊九(N 寸 1 - ii).                               (2.26)

The function generated by (2.24) gives the prototype or mother wavelet 砂(t) for a class of ex-
pansion functions of the form
                                  砂3,k(t) = 23/2 砂（23t 寸 丸）                             (2.27)
16                                                                                                                                                                             A 1너너tires히ut向n Formulat向n     Ch. 2


where 2j is the scaling of t (j is the log2 of the scale), 2-ak is the translation in t, and 23/2
maintains the (perhaps unity) L2 norm of the wavelet at different scales.
   The Haar and triangle wavelets that are associated with the scaling functions in Figure 2.2 are
shown in Figure 2.4. For the Haar wavelet, the coefficients in (2.24) are h1(O) = i/ /,   hi(1) =
-1/ V'亘 which satisfy (2.25). The Daubechies wavelets associated with the scaling functions in
Figure 6.1 are shown in Figure 6.2 with corresponding coefficients given later in the book in
Tables 6.1 and 6.2.




             砂（t) = 砂（2t) - 砂（2t - 1) 尸
                                                                                                                 砂（t) = m如位）H 如位 H 기 + 砂m 小 1)
                  (a)
                        Haar
                                         (same
                                                                   as                                                                                 (b) Triangle (same

                                                       Figure 2.4. Haar and Triangle Wavelets


   We have now constructed a set of functions 甲k (t) and 砂j,k(t) that could span all of L2(R).
According to (2.19), any function g(t) E L2(R) could be written
                                                                        00                                                       00               的


                                g(t) = >                                       c(k) 'Pk(t) +＞二 乞 'd(j小）吻，k (t)                                                                                              (2.28)
                                                                   k= -oc                                                  j= 0k= -以

as a series expansion in terms of the scaling function and wavelets.
    In this expansion, the first summation in (2.28) gives a function that is a low resolution or
coarse approximation of g(t). For each increasing index j in the second summation, a higher or
finer resolution function is added, which adds increasing detail. This is somewhat analogous to
a Fourier series where the higher frequency terms contain the detail of the signal.
    Later in this book, we will develop the property of having these expansion functions form
an orthonormal basis or a tight frame, which allows the coefficients to be calculated by inner
products as



and
                                c
                                                 (k)
                                                           =
                                                                   匈     (k)
                                                                               =        (g
                                                                                                   (t)
                                                                                                         ,
                                                                                                             k
                                                                                                                     (t)
                                                                                                                                  )       =           f    g
                                                                                                                                                               (t)
                                                                                                                                                                           k
                                                                                                                                                                               (t)
                                                                                                                                                                                           dt


                               따（   ()
                                                       =
                                                               d
                                                                   (j小）        =   (g
                                                                                             (t)
                                                                                                         肋,      k
                                                                                                                           (t)
                                                                                                                                      )       :       Jg
                                                                                                                                                                     (t）
                                                                                                                                                                           吻，        ,(!
                                                                                                                                                                                           ）毗·
    The coefficient d(j, k) is sometimes written as d3 (k) to emphasize the difference between the
time translation index k and the scale parameter j. The coefficient c(k) is also sometimes written
as c3 (k) or c(j, k) if a more general "starting scale" other than j = 0 for the lower limit on the
sum in (2.28) is used.
 Sec. 2.4.   The Discrete Wavelet Transform
                                                                                                                         1T

     It is important at this point to recognize the relationship of the scaling function part of the
 expansion (2.28) to the wavelet part of the expansion. From the representation of the nested
 spaces in (2.19) we see that the scaling function can be defined at any scale j. Equation (2.28)
 uses j = 0 to denote the family of scaling functions.
     You may want to examine the Haar system example at the end of this chapter just now to
 see these features illustrated.


 2.4     The Discrete Wavelet Transform

 Since
                                            L2 = vi. 또） W。e3仍, +1 田 · · ·                                            (2.31)
using (2.6) and (2.27), a more general statement of the expansion (2.28) can be given by
                                                                                                 的

                    g(t) 스그小）230/2甲但上 - k) +＞二 ＞二 d3徇 23/2叩it - 丸）                                                   (2.32)
                             k                                                         丸     j= jo
or

                              g(t) =Z出目協，
                                        幽＋> Zdj（枷Mt)                                                                 但33)
                                            k                                          k   j= jo
where jo could be zero as in (2.19) and (2.28), it could be ten as in (2.20), or it could be negative
infinity as in (1.8) and (2.22) where no scaling functions are used. The choice of j0 sets the
coarsest scale whose space is spanned by 97 j。  ,k (t). The rest of L2(R) is spanned by the wavelets
which provide the high resolution details of the signal. In practice where one is given only the
samples of a signal, not the signal itself, there is a highest resolution when the finest scale is the
sample level.
    The coefficients in this wavelet expansion are called the discrete wavelet transform (DWT) of
the signal g(t). If certain conditions described later are satisfied, these wavelet coefficients corn-
pletely describe the original signal and can be used in a way similar to Fourier series coefficients
for analysis, description, approximation, and filtering. If the wavelet system is orthogonal, these
coefficients can be calculated by inner products


                                                                                                                     但34)
                                  白
                                      （丸）
                                                =
                                                    (g
                                                         (t)
                                                               ,
                                                                   7恥   （:
                                                                             )=
                                                                                  fg
                                                                                           (t）
                                                                                                     吻，
                                                                                                          ,(!
                                                                                                                ）毗
and
                                 따（劤 = (g(t), 砂i,k (t) = / g(t）砂j,k(t) dt.                                           (2.35)
                                                                                  J
If the scaling function is well-behaved, then at a high scale, the scaling is similar to a Dirac delta
function and the inner product simply samples the function. In other words, at high enough
resolution, samples of the signal are very close to the scaling coefficients. More is said about this
later. It has been shown [Don93b] that wavelet systems form an unconditional basis for a large
class of signals. That is discussed in Chapter 5 but means that even for the worst case signal in
the class, the wavelet expansion coefficients drop off rapidly as j and k increase. This is why the
DWT is efficient for signal and image compression.
    The DWT is similar to a Fourier series but, in many ways, is much more flexible and in-
formative. It can be made periodic like a Fourier series to represent periodic signals efficiently.
18                                                                    AM미tires이ution Form미ation   Ch. 2



However, unlike a Fourier series, it can be used directly on non-periodic transient signals with ex-
cellent results. An example of the DWT of a pulse was illustrated in Figure 3.3. Other examples
are illustrated just after the next section.


2.5      A Parseval's Theorem
If the scaling functions and wavelets form an orthonormal basis1, there is a Parseval's theorem
that relates the energy of the signal g(t) to the energy in each of the components and their wavelet
coefficients. That is one reason why orthonormality is important.
    For the general wavelet expansion of (2.28) or (2.33), Parseval's theorem is


                               /Ig（테2毗＝드 Ic(1)I2戊 드 同（(）尸
                                              i=H（刃      j= O k=-oo
                                                                                                  但36)


with the energy in the expansion domain partitioned in time by k and in scale by j. Indeed, it
is this partitioning of the time-scale parameter plane that describes the DWT. If the expansion
system is a tight frame, there is a constant multiplier in (2.36) caused by the redundancy.
    Daubechies [Dau88a, Dau92] showed that it is possible for the scaling function and the wavelets
to have compact support (i.e., be nonzero only over a finite region) and to be orthonormal. This
makes possible the time localization that we desire. We now have a framework for describing sig-
nals that has features of short-time Fourier analysis and of Gabor-based analysis but using a new
variable, scale. For the short-time Fourier transform, orthogonality and good time-frequency res-
olution are incompatible according to the Balian-Low-Coifrnan-Semmes theorem [Dau90, Sie86].
More precisely, if the short-time Fourier transform is orthogonal, either the time or the frequency
resolution is poor and the trade-off is inflexible. This is not the case for the wavelet transform.
 Also, note that there is a variety of scaling functions and wavelets that can be obtained by
choosing different coefficients h(n) in (2.13).
    Donoho [Don93b1 has noted that wavelets are an unconditional basis for a very wide class
of signals. This means wavelet expansions of signals have coefficients that drop off rapidly and
 therefore the signal can be efficiently represented by a small number of them.
     We have first developed the basic ideas of the discrete wavelet system using a scaling multiplier
of 2 in the defining equation (2.13). This is called a two-band wavelet system because of the two
channels or bands in the related filter banks discussed in Chapters 3 and 8. It is also possible to
 define a more general discrete wavelet system using 97(t) = > h(n) .砥乂Mt - n) where M is
 an integer [SHGB93]. This is discussed in Section 7.2. The details of numerically calculating the
DWT are discussed in Chapter 9 where special forms for periodic signals are used.


2.6      Display of the Discrete Wavelet Transform and the Wavelet Expansion
It is important to have an informative way of displaying or visualizing the wavelet expansion and
transform. This is complicated in that the DWT is a real-valued function of two integer indices
and, therefore, needs a two-dimensional display or plot. This problem is somewhat analogous to
plotting the Fourier transform, which is a complex-valued function.
     There seem to be five displays that show the various characteristics of the DWT well:
     tor a tight frame defined in Chapter 4
Sec. 2.6. Display of the Discrete Wavelet Transform and the Wavelet Expansion                    19


   1. The most basic time-domain description of a signal is the signal itself (or, for most cases,
      samples of the signal) but it gives no frequency or scale information. A very interesting
      property of the DWT (and one different from the Fourier series) is for a high starting scale
      jo in (2.33), samples of the signal are the DWT at that scale. This is an extreme case, but
      it shows the flexibility of the DWT and will be explained later.

   2. The most basic wavelet-domain description is a three-dimensional plot of the expansion
      coefficients or DWT values c(k) and d (k) over the j, k plane. This is difficult to do on a
      tw아dimensional page or display screen, but we show a form of that in Figures 2.5 and 2.8.

   3. A very informative picture of the effects of scale can be shown by generating time functions
      f3(t) at each scale by summing (2.28) over k so that


                                              1(t) = 13。+＞二f3(t)                              (2.37)
                                                                3

      where
                                              力. =     :嗣미卜丸）                                 (2.38)
                                                       k

      and
                                        力（t) = ＞二d3（丸）2)12砂（23t -丸）.                          (2.39)
                                                   丸

      This illustrates the components of the signal at each scale and is shown in Figures 2.7 and
      2.10.

   4. Another illustration that shows the time localization of the wavelet expansion is obtained
      by generating time functions fk (t) at each translation by summing (2.28) over k so that


                                                  f(t) = 乞 fk(t)
                                                            k

      where
                               九（t) = C（丸）甲（t- 丸）+ ＞二d （丸）2)12砂（23t - 丸）.
                                                            3

      This illustrates the components of the signal at each integer translation.

   5. There is another rather different display based on a partitioning of the time-scale plane as if
      the time translation index and scale index were continuous variables. This display is called
       'tiling the time-frequency plane." Because it is a different type of display and is developed
      and illustrated in Chapter 9, it will not be illustrated here.

   Experimentation with these displays can be very informative in terms of the properties and
capabilities of the wavelet transform, the effects of particular wavelet systems, and the way a
wavelet expansion displays the various attributes or characteristics of a signal.
20                                                                      A Mu仕什es이ution Form너ation   Ch. 2


2.7    Examples of Wavelet Expansions

In this section, we will try to show the way a wavelet expansion decomposes a signal and what
the components look like at different scales. These expansions use what is called a length-8
Daubechies basic wavelet (developed in Chapter 6), but that is not the main point here. The
local nature of the wavelet decomposition is the topic of this section.
    These examples are rather standard ones, some taken from David Donoho's papers and web
page. The first is a decomposition of a piecewise linear function to show how edges and constants
are handled. A characteristic of Daubechies systems is that low order polynomials are completely
contained in the scaling function spaces V3 and need no wavelets. This means that when a section
of a signal is a section of a polynomial (such as a straight line), there are no wavelet expansion
coefficients d (k), but when the calculation of the expansion coefficients overlaps an edge, there
is a wavelet component. This is illustrated well in Figure 2.6 where the high resolution scales
gives a very accurate location of the edges and this spreads out over k at the lower scales. This
gives a hint of how the DWT could be used for edge detection and how the large number of small
or zero expansion coefficients could be used for compression.




          Skyline             1    J       /1                 尸NU
            而作）                        1
                                           T                        '    "




            毗（劤

            山（劤

            南（川

            吻（劤

            山（k)
                                   1

            而（k)          1
                                   1
            co(k) I
                                                1   1
                                                                                  1
Figure 2.5. Discrete Wavelet Transform of the Houston Skyline, using 砂D8' with a Gain of \／牙
for Each Higher Scale




   Figure 2.6 shows the approximations of the skyline signal in the various scaling function spaces
V3. This illustrates just how the approximations progress, giving more and more resolution at
higher scales. The fact that the higher scales give more detail is similar to Fourier methods, but
the localization is new. Figure 2.7 illustrates the individual wavelet decomposition by showing
Sec. 2.7. Examples of Wavelet Expansions                                                                   21


the components of the signal that e虹st in the wavelet spaces W3 at different scales j. This shows
the same expansion as Figure 2.6, but with the wavelet components given separately rather than
being cumulatively added to the scaling function. Notice how the large objects show up at the
lower resolution. Groups of buildings and individual buildings are resolved according to their
width. The edges, however, are located at the higher resolutions and are located very accurately.


                0.08

                0.06

                0.04

                0.02

                  0

               -0.02

               -0.04

               -0.06

                   0     2（兀       4（刃   6（刃   800   1아刃         200         衣)0        6（刃   6凹

                        (a) Projection onto V0                  (b) Projection onto V1
                0.08

                0.06                                                    ＼八
                0.04

                0.02

                  0

               -0.02

               -0.04

               -0.06
                                                                              /U
                   0     2（刃       400   以刃    800   1伽          200         400        600   600   1000

                        （이 Pr이ection onto V2                    (d) Projection onto V3
                0.08

                0.06

                0.04

                0.02

                  0

               -0.02-



                               1
               m0. 4.                                            丁1
               -0.06

                   0     200       4（刃   600   以X)   1南0         2（兀         400        600   800   1以)0

                        (e) Projection onto V4                  (f) Projection onto V5
                0.08-

                0.06-

                0.04-

                0.02

                   0
                                               Pr
               -0.02-

               -0.04-
                                   ,/\
                                                                             了＼     e



               -0.06-

                         200       衣刃    이刃    며刃    1000   0     2(刃         4（刃       600   8的    1餉

                        (g) Projection onto V6                  (h) Projection onto V7

         Figure 2.6. Projection of the Houston Skyline Signal onto V Spaces using 砂D8'
 22                                                                            A Multiresolution Formulation   Ch. 2




                       2的     400   600     的0   1啣             0     2（刃    4（刃    以10   800

                      (a) Projection onto                           (b) Projection onto Wo

                                                         0.06 ·

                                                         0.04

                                                         0.02-

                                                            0

                                                        -0.02-

                                                        -0.04 ·

                 0     200   4（刃    6（刃     帥    1000        0        2여）    4凹     600   8凹

                     (c) Projection onto W1                         (d) Projection onto W2

                                                         0.（滔




                                                                      20()   丑x)   仗刃     8여）   1町）

                     (e) Projection onto W3                         (f) Projection onto W4

              0.06

              0.04

              0.02




                                                                     '1r '
                                                 1啣         0        201)    求10   以10    800   1000

                     (g) Projection onto W5                         (h) Projection onto W6

       Figure 2.7. Projection of the Houston Skyline Signal onto W Spaces using 砂D8'



     The second example uses a chirp or doppler signal to illustrate how a time-varying frequency
is described by the scale decomposition. Figure 2.8 gives the coefficients of the DWT directly as
a function of j and k. Notice how the location in k tracks the frequencies in the signal in a way
the Fourier transform cannot. Fi叩res 2.9 and 2.10 show the scaling function approximations
and the wavelet decomposition of this chirp signal. Again, notice in this type of display how the
 "location" of the frequencies are shown.
Sec. 2.8. An Example of the Haar Wavelet System                                                23


          Doppler



             南(k) 十印卄小

             南 (k) 끼1」’」’．J·
                         」小


             d4(k)

             南（k)
                                    1

                                                      1
             山（k)
                                        1
                                        1                     1
                                                              1                 1   1
                                                                      1     1


Figure 2.8. Discrete Wavelet Transform of a Doppler, using 砂D8' with a gain of './        for each
higher sca뇨




2.8     An Example of the Haar Wavelet System
In this section, we can illustrate our mathematical discussion with a more complete example. In
1910, Haar [llaalol showed that certain square wave functions could be translated and scaled to
create a basis set that spans L2. This is illustrated in Figure 2.11. Years later, it was seen that
Ha.ar뇽 system is a particular wavelet system.
   If we choose our scaling function to have compact support over 0 드 t 드 1, then a solution to
(2.13) is a scaling function that is a simple rectangle function

                                            甲
                                                (t)       =   {   1 if0< t< 1
                                                                  0 otherwise
                                                                                            (2.42)

with only two nonzero coefficients h(0) = h(1) = i/ \/ and (2.24) and (2.25) require the wavelet
to
   be                                    (1     f。
                                                 r0< t< 0.5
                                 砂 (t) = 4 -1 for 0.5 <t < 1                              (2.43)
                                         10     。therwise
with only two nonzero coefficients h1(0) = i/ \/牙 and h1(1) = -1/ v'易.
    Vo is the space spanned by 甲(t - k) which is the space of piecewise constant functions over
integers, a rather limited space, but nontrivial. The next higher resolution space V1 is spanned
by 甲(2t - k) which allows a somewhat more interesting class of signals which does include V0.
As we consider higher values of scale j, the space V3 spanned by 甲(2it 小 k) becomes better able
to approximate arbitrary functions or signals by finer and finer piecewise constant f끄lctions.
24                                                             AM미tiresolt北油n Formulat油n   Ch. 2


         0．아

         0.02

            0

       -0.02

       -0.04

       -0.此
             0        200   400   600   800   1呵）      2（刃   400    6的    800

                 (a) Projection onto V0              (b) Projection onto V1

        0.041

        0.02

           0

       -0.02



                                                       1
       -0.04-

       -0.06 -
                      2（刃   4（兀   6（刃   800   1000     200   400   600    800   1000

                 (c) Projection onto V2              (d) Projection onto V3

                       1




           마




                  2(刃       4（刃   B（刃   8（刃   1       2（兀    求刃    6（刃    800   1（狀）

                 (e) Projection onto V4              (f) Projection onto V5



                  r


                  200       400   600   800   1000    2刃     400   600   800    1000

                 (g) Projection onto V6              (h) Projection onto V7

     Figure 2.9. Projection of the Doppler Signal onto V Spaces using 砂D8'
Sec. 2.8. An Example of the Haar Wavelet System
                                                                                                                       25




                                                                                      200   400    eoo     800   1啣

                             (a) Projection onto Vo                                 (b) Projection onto
                0.05                                                    0.05



                                                                                       1



                                                                           0   小／
              느005 -                                         4         -0.05 -
                  0               200   400   600   800   1000              0         200   400   6（均     800    1啣

                            (c) Projection onto Wi                                  (d) Projection onto W2
               0.05                                                     005




                  0
                             1,
                                   ..




              -0.05                                                -0.05 -
                   0              200   400   600   8（刃   1啣            0             200   400   以刃      800    1啣

                            (e) Projection onto W3                                  (f) Projection onto W4
               0.05                                                    0.05




                      伊
                      1d뇨
              -0.05
                   0         200        400   600   800   10刃
                                                                 -0.
                                                                         05占         200    400   6（刃     800    1町）

                            (g) Projection onto W5                                  (h) Projection onto W6

          Figure 2.10. Projection of the Doppler Signal onto W Spaces using 砂D8'
26                                                                                 A Mu比ires이ut油n Formulat向n      Ch. 2



Haar showed that as j - 以, V3 - L2. We have an approximation made up of step functions
approaching any square integrable function.
    The Haar functions are illustrated in Figure 2.11 where the first column contains the simple
constant basis function that spans V0, the second column contains the unit pulse of width one
half and the one translate necessary to span V1. The third column contains four translations
of a pulse of width one fourth and the fourth contains eight translations of a pulse of width
one eighth. This shows clearly how increasing the scale allows greater and greater detail to be
realized. However, using only the scaling function does not allow the decomposition described in
the introduction. For that we need the wavelet. Rather than use the scaling functions 甲(8t - k)
in V3, we will use the orthogonal decomposition

                                                V3       =    V2 甲）시2                                          (2.44)

which is the same as

                   Span{cp(8t - k)}         =    Span{甲(4t - k)} 由 Span{砂(4t - k)}                             (2.45)
                       k                                 k                     k

which means there are two sets of orthogonal basis functions that span V3, one in terms of j = 3
scaling functions, and the other in terms of half as many coarser j = 2 scaling functions plus the
details contained in the j = 2 wavelets. This is illustrated in Figure 2.12.


                                                             中（27t - 丸）
                             0                       1                    2                    3

                                                                                         口n
             0                      1   I            I
                                                                                                          1
             1                                                  1
                                                                                   匕                          J
              n
              二


              n
              D

              4
              1


              =
              U

              n
              b

              n
              /                                                                                      r기
                             V0                      V1                   V2                  V3


                           Figure 2.11. Haar Scaling Functions that Span V3

     The V2 can be further decomposed into

                                                V2       =    V1 田W1                                           (2.46)

which is the same as

                   Span{ o(4t - k)}         =    Span{y7(2t - k)} q) Span{砂(2t - k) }                          (2.47)
                       丸                                 k                     k
Sec. 2.8. An Example of the Haar Wavelet System                                                     27


                                  3                                          j= 2

                                 口



                                                                                 砂（4t- k)   V2




               V3   砂（8t - 丸）

                                                            그
                                                      F斗
                                                      H-－니1m
                                                                                 砂（4t 中 丸） w2
                                                                -J
                                                                     r
                                                                         I

                                            V3 = V2 4) W2


            Figure 2.12. Haar Scaling Functions and Wavelets Decomposition of V3


and this is illustrated in Figure 2.14. This gives V1 also to be decomposed as

                                            V1    =        V0 由W0                                (2.48)

which is shown in Figure 2.13. By continuing to decompose the space spanned by the scaling
function until the space is one constant, the complete decomposition of V3 is obtained. This is
symbolically shown in Fi叩re 2.16.


                                                                             j= o
                                  1                   1                      i   砂（t- 丸）    V0
               V1   砂（2t - 丸）
                                                  1   1                      1   砂（t斗丸） wo

                                            V1 = V0 $ W0


            Figure 2.13. Haar Scaling Functions and Wavelets Decomposition of V1
28                                                                      AM내tires이ution Formu冶tion   Ch. 2



    Finally we look at an approximation to a smooth function constructed from the basis elements
in V3 == V0田니0田34在今）시2 . Because the Haar 如兀ti이瑁 form an orthog아好1 ba駁s in ea血 subspace,
they can produce an optimal least squared error approximation to the smooth function. One can
easily imagine the effects of adding a higher resolution "layer" of functions to W3 giving an
approximation residing in V4. Notice that these functions satisfy all of the conditions that we
have considered for scaling functions and wavelets. The basic wavelet is indeed an oscillating
f끄lction which, in fact, has an average of zero and which will produce finer and finer detail as it
is scaled and translated.
    The multiresolution character of the scaling function and wavelet system is easily seen from
Figure 2.12 where a signal residing in V3 can be expressed in terms of a sum of eight shifted scaling
血nctions at scale j = 3 or a sum of four shifted scaling functions and four shifted wavelets at
a scale of j = 2. In the second case, the sum of four scaling functions gives a low resolution
approximation to the signal with the four wavelets giving the higher resolution "detail". The
four shifted scaling functions could be further decomposed into coarser scaling functions and
wavelets as illustrated in Figure 2.14 and still further decomposed as shown in Figure 2.13.
    Figure 2.15 shows the Haar approximations of a test function in various resolutions. The
signal is an example of a mixture of a pure sine wave which would have a perfectly localized
Fourier domain representation and a two discontinuities which are completely localized in time
domain. The component at the coarsest scale is simply the average of the signal. As we include
more and more wavelet scales, the approximation becomes close to the original signal.
    This chapter has skipped over some details in an attempt to communicate the general idea of
the method. The conditions that can or must be satisfied and the resulting properties, together
with examples, are discussed in the following chapters and/or in the references.




                            j= 2                               2    =   1

                                                  I       1
                                                                        砂（2t- k)    V1
                                                                1
              V2   砂（4t - k)


                                                                        砂（2t- k)    W1
                                          r1
                                                                1

                                         V2 = V1 田 )47l


           Figure 2.14. Haar Scaling Functions and Wavelets Decomposition of V2
Sec. 2.8. An Example of the Haar Wavelet System                                                             29

                                                                            Approximation in V6
                 Test Fun아向n


  0.5                                              0.5

    0

 -0.5                                             -0.5


                2          4           6                                      2          4              6
                                                   e1。
              Approximation in V5                                           Approximation in V4



  0.5                                              0.5

    0   ,
                                                               0

 e0.5 .                                           -0.5


                2          4            6                           0         2          4              6
              Approximation in V3                                           Approximation in   V2
                                                                                                    1
                                                   0.5

                                                                    0   ,




                                                  -0.5


                 2          4           6                           0          2          4
                                                         -1
               Approximation in V1                                           Approximation in V。
                                                                    1

                                                         0.5

                                                                    0

                                                   -0.5


                  2          4           6                                      2         4             6
                                                              m1。
                          Figure 2.15. Haar Function Approximation in V3
30                                                               A 1너미tireso山tion Form미ation   Ch. 2


         j= 3                j= 2             j= 1              j= O

     中（8t -虎） V3     中（4t - 丸） V2         砂（2t - 丸） V1     中（t小丸） V0
     口               1   1                1     1          1            1   中
                                                                            （t- k)      V0

                     H.J      L                 1      f   1            1   砂（t叫丸） wo

     -J그                                  1
                                                                            砂（2t - 丸）    Wi
                                                1
                                                       1

                    다J

                                                                            砂（4t - 丸） w2




                                    V3 = VU 0 Wo ) 끼／1 由 )'V2


         Figure 2.16. Haar Scaling Functions and Wavelets Decomposition of V3
Chapter 3


                   Filter Banks and the Discrete
                              Wavelet Transform


In many applications, one never has to deal directly with the scaling functions or wavelets. Only
the coefficients h(미 and hi(n) in the defining equations (2.13) and (2.24) and c(k) and d3(k) in
the expansions (2.28), (2.29), and (2.30) need be considered, and they can be viewed as digital
filters and digital signals respectively [GB92c, Vai921. While it is possible to develop most of the
results of wavelet theory using only filter banks, we feel that both the signal expansion point of
view and the filter bank point of view are necessary for a real understanding of this new tool.


3.1    Analysis 中 From Fine Scale to Coarse Scale
In order to work directly with the wavelet transform coefficients, we will derive the relationship
between the expansion coefficients at a lower scale level in terms of those at a higher scale.
Starting with the basic recursion equation from (2.13)

                                   p(t) = >   h(n) /    (2t - n)                               (3.1)


and assuming a unique solution exists, we scale and translate the time variable to give

          甲仁"卜히스그(n) /西(2(2t - k) 什미万）回而沁"+1卜胱- n)                                             (3.2)
                         n                                 n


which, after changing variables m = 2k + n, becomes

                             甲（23t叫丸）=＞二／i(7n寸2丸） \／巨甲(2j+'t- m).                              (3.3)
                                         m


   If we denote V3 as
                                    V3 = Span{2j12 Y7(2jt - k)}                                (3.4)
                                          k
then
                   f(t) E V3+l    쑤     f(t) =＞二 c3+i (k) 2("+l)/2甲（2'"+lt - k)                (3.5)
                                                k

                                                                                                 31
 32                                                                                                   Filter Banks and the Discrete Wavelet Transform                          Ch. 3


 is expressible at a scale of j + 1 with scaling functions only and no wavelets. At one scale lower
 resolution, wavelets are necessary for the "detail" not available at a scale of j. We have

                     f(t) =                            向 23/2 (23t - 川 + Z d3(k) 2j/2叭23t 寸 丸）                                                                           (3.6)
                                               k                                                           k

where the 23/2 terms maintain the unity norm of the basis functions at various scales. If 甲j
                                                                                              ,k (t)
and 砂7,k(t) are orthonormal or a tight frame, the j level scaling coefficients are found by taking
the inner product

                                 c
                                     (k)
                                                   =   (f(t)      ,
                                                                          吻，
which, by using (3.3) and interchanging the sum and integral, can be written as
                                                                               k
                                                                                   (t)
                                                                                               ):   f f (t)    23/
                                                                                                                     『
                                                                                                                     2
                                                                                                                                   (23t
                                                                                                                                           -       k)
                                                                                                                                                             dt          (3.
                                                                                                                                                                                 7)
                       c
                           (k)
                                           =
                                                   >    h
                                                            (m
                                                                      -        2k)        ff
                                                                                                    (t) 2(3 ') /2        『
                                                                                                                             (2i
                                                                                                                                          't   -        m)
                                                                                                                                                                  dt
                                                                                                                                                                         位8)

but the integral is the inner product with the scaling function at a scale of j + 1 giving


                                                       c3 (k) = > h(m- 刈아伽2).                                                                                           位9)


The corresponding relationship for the wavelet coefficients is


                                                       따（丸）= ＞二九i(7m - 2丸）cj+i(m).                                                                                     (3.10)


Filtering and Down-Sampling or Decimating
In the discipline of digital signal processing, the "filtering" of a sequence of numbers (the input
signal) is achieved by convolving the sequence with another set of numbers called the filter
coefficients, taps, weights, or impulse response. This makes intuitive sense if you think of a
moving average with the coefficients being the weights. For an input sequence x(n) and filter
coefficients h(n), the output sequence y(n) is given by

                                                                                         N- i
                                                                 y（미 = ＞二 九（k) x(n- k)                                                                                 (3.11)
                                                                                         k=O

There is a large literature on digital filters and how to design them [PB87, OS89J. If the number
of filter coefficients N is finite, the filter is called a Finite Impulse Response (FIR) filter. If the
number is infinite, it is called an Infinite Impulse (IIR) filter. The design problem is the choice
of the h(n) to obtain some desired effect, often to remove noise or separate signals [OS89, PB87].
    In multirate digital filters, there is an assumed relation between the integer index n in the
signal x(n) and time. Often the sequence of numbers are simply evenly spaced samples of a
function of time. Two basic operations in multirate filters are the down-sampler and the up-
sampler. The down-sampler (sometimes simply called a sampler or a decimator) takes a signal
 Sec. 3.1. Analysis - From Fine Scale to Coarse Scale
                                                                                                    33


                                                                    x (2川


                             Figure 3.1. The Down Sampler or Decimator




  x(n) as an input and produces an output of y(n) = x(2n). This is s戶llbolically shown in
 Figure 3.1. In some cases, the down-sampling is by a factor other than two and in some cases,
  the output is the odd index terms y(n) = x(2n + 1), but this will be explicitly stated if it is
 important.
     In down-sampling, there is clearly the possibility of losing information since half of the data is
 discarded. The effect in the frequency domain (Fourier transform) is called aliasing which states
 that the result of this loss of information is a mixing up of frequency components [PB87, OS89}.
 Only if the original signal is band-limited (half of the Fourier coefficients are zero) is there no
 loss of information caused by down-sampling.
     We talk about digital filtering and down-sampling because that is exactly what (3.9) and
 (3.10) do. These equations show that the scaling and wavelet coefficients at different levels of
scale can be obtained by convolving the expansion coefficients at scale j by the time-reversed
recursion coefficients h(- n) and hi(- n) then down-sampling or decimating (taldng every
                                                                                                 other
 term, the even terms) to give the expansion coefficients at the next level of j - 1. In other
words, the scal町 coefficients are "filtered" by two FIR digital filters with coefficients h(- n)
and h1(- n) after which down-sampling gives the next coarser scaling and wavelet coefficients.
These structures implement Mallat's algorithm [Mal89b, Mal89c] and have been developed in
the engineering literature on filter banks, quadrature mirror filters (QMF), conjugate filters, and
perfect reconstruction filter banks [SB86a, SB87, Vet86, VG89, .Vet87, Vai87a, Vai92I and are
expanded somewhat in Chapter 8 of this book. Mallat, Daubechies, and others showed the
relation of wavelet coefficient calculation and filter banks. The implementation of equations (3.9)
and (3.10) is illustrated in Figure 3.2 where the down-pointing arrows denote a decimation or
down-sampling by two and the other boxes denote FIR filtering or a convolution by h(- n) or
hi(- n). To ease notation, we use both h(n) and ho(n) to denote the scaling 血nction coefficients
for the dilation equation (2.13).




                                                    h1
                                                         (-
                             cj+i


                                                1             HH+     cj




                                Figure 3.2. Tw아Band Analysis Bank
34                                                           Filter Banks and the Discrete Wavelet Transform    Ch. 3




                                   (-
                              h1
           勻＋1H                                                                         h1   (-
                                                                                                   3寸1


                              h0   （中
                                                             p




                                                                           p.
                                                                                             (-
                                                                                        h0
                        Figure 3.3. Tw아Stage Two-Band Analysis Tree

     As we will see in Chapter 5, the FIR filter implemented by h(- n) is a lowpass filter, and the
one implemented by hi(- n) is a highpass filter. Note the average number of data points out of
this system is the same as the number in. The number is doubled by having two filters; then it is
halved by the decimation back to the original number. This means there is the possibility that no
information has been lost and it will be possible to completely recover the original signal. As we
shall see, that is indeed the case. The aliasing occurring in the upper bank can be "undone" or
cancelled by using the signal from the lower bank. This is the idea behind perfect reconstruction
in filter bank theory [Vai92, Fli94].
     This splitting, filtering, and decimation can be repeated on the scaling coefficients to give the
two-scale structure in Figure 3.3. Repeating this on the scaling coefficients is called iterating the
filter bank. Iterating the filter bank again gives us the three-scale structure in Figure 3.4.
     The frequency response of a digital filter is the discrete-time Fourier transform of its impulse
response (coefficients) h(n). That is given by
                                                     m

                                        且佃） =   ＞二
                                                n=   -   _
                                                                 九   （n)        etcm.
                                                                                                               (3.12)


The magnitude of this complex-valued function gives the ratio of the output to the input of the
filter for a sampled sinusoid at a frequency of w in radians per seconds. The angle of H (w) is the
phase shift between the output and input.
     The first stage of two banks divides the spectrum of c+i (k) into a lowpass and highpass band,
resulting in the scaling coefficients and wavelet coefficients at lower scale c (k) and d (k). The
second stage then divides that lowpass band into another lower lowpass band and a bandpass
band. The first stage divides the spectrum into two equal parts. The second stage divides the
lower half into quarters and so on. This results in a logarithmic set of bandwidths as illustrated
in Figure 3.5. These are called "constant-Q" filters in filter bank language because the ratio of
the band width to the center frequency of the band is constant. It is also interesting to note
that a musical scale defines octaves in a similar way and that the ear responds to frequencies in
a similar logarithmic fashion.
     For any practical signal that is bandlimited, there will be an upper scale j = J, above which
the wavelet coefficients, d (k), are negligibly small [GOB94]. By starting with a high resolution
description of a signal in terms of the scaling coefficients cj, the analysis tree calculates the DWT
Sec. 3.1. Analysis - From Fine Scale to Coarse Scale                                                     35




              V3




                                  Figure 3.4. Three-Stage Two-Band Analysis Tree



                   1/
                        /（口J) 1

                         'V0            Wo        Wl                                 W2




                                                                                                     w

                         0         It        즈4                         즈2                      7r
                                   8




                                  Figure 3.5. Frequency Bands for the Analysis Tree



down to as low a resolution, j = j0, as desired by having J - jo stages. So, for f (t) E Vj, using
(2.8) we have


                             f (t)      =    ＞二Cj
                                             k
                                                  丸）
                                                  （    (PJ,   k   (t)
                                        = ＞二Cf_i（丸）(pj_ i,k(t) +＞二dJ_1(k）砂J_i,k(t)
                                             k                                   k
                                                                                        J_ i

                                        = ＞二CJ_2（丸）甲J寸2,k(t) +＞二 ＞二 따（k）砂j,k(t)
                                             k                                   k     3=J- 2
                                                                                J_ i

                                        = 二m川吼嗣＋ZZ娜）蜘(t)
                                              丸                              k i= jo



which is a finite scale version of (2.33). We will discuss the choice of jo and J further in Chapter 9.
 36                                                    Filter Banks and the Discrete Wavelet Transform     Ch. 3


 3.2    Synthesis 中 From Coarse Scale to Fine Scale
As one would expect, a reconstruction of the original fine scale coefficients of the signal can be
made from a combination of the scaling function and wavelet coefficients at a coarse resolution.
This is derived by considering a signal in the j + 1 scaling function space f (t) E V3+1.
                                                                                              This
function can be written in terms of the scaling function as


                                  ／떠 = 乞아嗣 싸1)/2 甲（2+ ' - k)                                             (3.17)
                                         k

or in terms of the next scale (which also requires wavelets) as


                       f(t) = ＞二勻（丸）23/2 甲(23t 中 丸）+ ＞二d3（丸）23/2砂（23t - 丸）·                              (3.18)
                              k                               k

Substituting (3.1) and (2.24) into (3.18) gives


/(D = ZCj（히 三如 싸1)/2 (2j+'卜胱-n汁Z可川＞二M미 싸1)/2 (2i싸- 2卜n).
         k         n                                      k           n
                                                                                           (3.19)
Because all of these functions are orthonormal, multiplying (3.17) and (3.19) by t' (23+'t
                                                                                            - k')
and integrating evaluates the coefficient as


                       Cj+i（丸）= Z c3(m) h伍 口川 + Z따回M卜 刎·                                                 (3.20)
                                    in                            m




Filtering and Up-Sampling or Stretching
For synthesis in the filter bank we have a sequence of first up甘sampling or stretching,
                                                                                        then filtering.
This means that the input to the filter has zeros inserted between each of the original
                                                                                            terms. In
other words,

                                  y(2n) = x(n)   and    y(2n + 1) = 0                                    (3.21)

where the input signal is stretched to twice its original length and zeros are inserted.
                                                                                             Clearly
this up-sampling or stretching could be done with factors other than two, and the two equation
above could have the x(n) and 0 reversed. It is also clear that up-sam
                                                                            pling does not lose any
information. If you first up-sample then down-sample, you are back where you started. However,
if you first down-sample then up-sample, you are not generally back where you started.
     Our reason for discussing filtering and up-sampling here is that is exactly what the synthesis
operation (3.20) does. This equation is evaluated by up-sampling the j scale coefficient
                                                                                          sequence
c3 (k), which means double its length by inserting zeros between each term, then convolving
                                                                                                  it
with the scaling coefficients h(n). The same is done to the j level wavelet coefficient
                                                                                          sequence
and the results are added to give the j + 1 level scaling function coefficients. This structure is
illustrated in Figure 3.6 where 90(n) = h(n) and gi(n) = hi(n). This combining process
                                                                                                can
be continued to any level by combining the appropriate scale wavelet coefficients. The resulting
two-scale tree is shown in Figure 3.7.
Sec. 3.3. Input Coefficients
                                                                                               37



                                          2    91（미

                                                                         Cj + i


                                               go（미




                               Figure 3.6. Two-Band Synthesis Bank




                                                         -.
                                                              91（미

             dj -'                 gi（미                                           Cj + i


                                                              90
                                                                   (n)
             Cj l                  90（미




                           Figure 3.7. Tw아Stage Two-Band Synthesis Tree



3.3     Input Coefficients
One might wonder how the input set of scaling coefficients c3+i are obtained from the signal
to use in the systems of Figures 3.2 and 3.3. For high enough scale, the scaling functions act
as "delta functions" with the inner product to calculate the high scale coefficients as
                                                                                          simply a
sampling of 1 (t) [GOB92, OGB92]. If the samples of 1 (t) are above the Nyquist rate, they
                                                                                               are
good approximations to the scaling coefficients at that scale, meaning no wavelet coefficients
are necessary at that scale. This approximation is particularly good if moments of the scaling
function are zero or small. These ideas are further explained in Section 6.8 and Chapter 9.
    An alternative approach is to "prefilter" the signal samples to make them a better appro姓-
mation to the expansion coefficients. This is discussed in [Str86].
    This set of analysis and synthesis operations is known as Mallat's algorithm [Mal89b, Mal89cI.
The analysis filter bank efficiently calculates the DWT using b町lks of digital filters and down-
samplers, and the synthesis filter bank calculates the inverse DWT to reconstruct the signal from
the transform. Although presented here as a method of calculating the DWT, the filter bank
description also gives insight into the transform itself and suggests modifications and general-
izations that would be difficult to see directly from the wavelet expansion point of view. Filter
banks will be used more extensively in the remainder of this book. A more general development
of filter banks is presented in Section 7.2.
38                                                  Filter Banks and the Discrete Wavelet Transform   Ch. 3


    Although a pure wavelet expansion is possible as indicated in (1.7) and (2.22), properties of
the wavelet are best developed and understood through the scaling function. This is certainly
true if the scaling function has compact support because then the wavelet is composed of a finite
sum of scaling functions given in (2.24).
    In a practical situation where the wavelet expansion or transform is being used as a compu-
tational tool in signal processing or numerical analysis, the expansion can be made finite. If the
basis functions have finite support, only a finite number of additions over k are necessary. If the
scaling function is included as indicated in (2.28) or (3.6), the lower limit on the summation over
j is finite. If the signal is essentially bandlimited, there is a scale above which there is little or
no energy and the upper limit can be made finite. That is described in Chapter 9.


3.4    Lattices and Lifting

An alternative to using the basic tw아band tree-structured filter bank is a lattice-structured filter
bank. Because of the relationship between the scaling filter h(미 and the wavelet filter h1(h) given
in (2.25), some of the calculation can be done together with a significant savings in arithmetic.
This is developed in Chapter 9 [Vai92].
    Still another approach to the calculation of discrete wavelet transforms and to the calculations
of the scaling functions and wavelets themselves is called "lifting." Although it is related to several
other schemes [Mar92, Mar93, DM93, K592], this idea was first explained by Wim Sweldens as a
time-domain construction based on interpolation [Swe951. Lifting does not use Fourier methods
and can be applied to more general problems (e.g., nonuniform sampling) than the approach
in this chapter. It was first applied to the biorthogonal system [Swe96a] and then extended to
orthogonal systems [DS96a}. The application of lifting to biorthogonal is introduced in Section 7.4
later in this book. Implementations based on lifting also achieve the same improvement in
arithmetic efficiency as the lattice structure do.


3.5    D肝erent P이nts of View
Multiresolution versus Time-Frequency Analysis
The development of wavelet decomposition and the DWT has thus far been in terms of mul-
tiresolution where the higher scale wavelet components are considered the "detail" on a lower
scale signal or image. This is indeed a powerful point of view and an accurate model for many
signals and images, but there are other cases where the components of a composite signal at
different scales and/or time are independent or, at least, not details of each other. If you think
of a musical score as a wavelet decomposition, the higher frequency notes are not details on a
lower frequency note; they are independent notes. This second point of view is more one of the
time-frequency or time-scale analysis methods [Coh89, Coh95, HB92, Boa92, LP89] and may be
better developed with wavelet packets (see Section 7.3), M-band wavelets (see Section 7.2), or a
redundant representation (see Section 7.6), but would still be implemented by some sort of filter
bank.

Periodic versus Nonperiodic Discrete Wavelet Transforms
Unlike the Fourier series, the DWT can be formulated as a periodic or a nonperiodic transform.
Up until now, we have considered a nonperiodic series expansion (2.33) over -的 <t < 以） with
Sec. 3.5. Different Points of View                                                                               39


the calculations made by the filter banks being an on-going string of coefficients at each of the
scales. If the input to the filter bank has a certain rate, the output at the next lower scale will
be two sequences, one of scaling function coefficients C3_1,k_ 1 and one of wavelet coefficients
d3_1,k_1, each, after down-sampling, being at half the rate of the input. At the next lower scale,
the same process is done on the scaling coefficients to give a total output of three strings, one
at half rate and two at quarter rate. In other words, the calculation of the wavelet transform
coefficients is a multirate filter bank producing sequences of coefficients at different rates but with
the average number at any stage being the same. This approach can be applied to any sign毗
finite or infinite in length, periodic or nonperiodic. Note that while the average output rate is
the same as the average input rate, the number of output coefficients is greater than the number
of input coefficients because the length of the output of convolution is greater than the length of
the input.
     An alternative formulation that can be applied to finite duration signals or periodic signals
(much as the Fourier series) is to make all of the filter bank filters cyclic or periodic convolution
which is defined by
                                                   N寸 l
                                          y（미 = ＞二 九（t) Z(n 小Z),                                               位22)
                                                    Z=0
for ii, Z = 0, 1, . . . , N - 1 and all indices and arguments are evaluated modulo N. For a length
N input at scale j = J, we have after one stage two length N/2 sequences, after two stages, one
length N/2 and two length N/4 sequences, and so on. If N = 2 ', this can be repeated J times
with the last stage being length one; one scaling function coefficient and one wavelet coefficient.
An example of how the periodic DWT of a length 8 can be seen Figure 3.8.

             c3   (k)
                         따 (k)       由＋l (k)   叱＋i (k+1)   d+2 (k)   d7+2 (k+ 1)   dj+2 (k+ 2)   dj+2 (k+ 3)




                                 Figure 3.8. The length-8 DWT vector


    The details of this periodic approach are developed in Chapter 9 showing the aliasing that
takes place in this system because of the cyclic convolution (3.22). This formulation is particularly
clean because there are the same number of terms in the transform as in the signal. It can be
represented by a square matrix with a simple inverse that has interesting structure. It can be
efficiently calculated by an FFT although that is not needed for most applications.
    For most of the theoretical developments or for conceptual purposes, there is little difference
in these two formulations. However, for actual calculations and in applications, you should make
sure you know which one you want or which one your software package calculates. As for the
Fourier case, you can use the periodic form to calculate the nonperiodic transform by padding
the signal with zeros but that wastes some of the efficiency that the periodic formulation was set
up to provide.

The Discrete Wavelet Transform versus the Discrete-Time Wavelet Transform
Two more points of view concern looking at the signal processing methods in this book as based on
an expansion of a signal or on multirate digital filtering. One can look at Mallat's algorithm either
as a way of calculating expansion coefficients at various scales or as a filter bank for processing
40                                                  Filter Banks and the Discrete Wavelet Transform   Ch. 3



discrete-time signals. The first is analogous to use of the Fourier series (FS) where a continuous
function is transformed into a discrete sequence of coefficients. The second is analogous to the
discrete Fourier tra坍form (DFT) where a discrete function is transformed into a discrete function.
Indeed, the DFT (through the FFT) is often used to calculate the Fourier series coefficients, but
care must be taken to avoid or minimize aliasing. The difference in these views comes partly
from the background of the various researchers (i.e., whether they are "wavelet people" or "filter
bank people"). However, there are subtle differences between using the series expansion of the
signal (using the discrete wavelet transform (DWT)) and using a multirate digital filter bank on
samples of the signal (using the discret今time wavelet transform (DTWT)). Generally, using both
views gives more insight into a problem than either achieves alone. The series expansion is the
main approach of this book but filter banks and the DTWT are also developed in Chapters 7.8
and 8.

Numerical Complexity of the Discrete Wavelet Transform
Analysis of the number of mathematical operations (floating-point multiplications and additions)
shows that calculating the DTWT of a length-N sequence of numbers using Mallat's algorithm
with filter banks requires O(N) operations. In other words, the number of operations is linear
with the length of the signal. What is more, the constant of linearity is relatively small. This is in
contrast to the FFT algorithm for calculating the DFT where the complexity is O(N log(N)) or
calculating a DFT directly requires O(N2) operations. It is often said that the FFT algorithm is
based on a "divide and conquer" scheme, but that is misleading. The process is better described as
a "organize and share" scheme. The efficiency (in fact, optimal efficiency) is based on organizing
the calculations so that redundant operations can be shared. The cascaded filtering (convolution)
and down-sampling of Mallat's algorithm do the s加ale thing.
    One should not make too much of this difference between the complexity of the FFT and
DTWT. It comes from the DTWT having a logarithmic division of frequency bands and the FFT
having a uniform division. This logarithmic scale is appropriate for many signals but if a uniform
division is used for the wavelet system such as is done for wavelet packets (see Section 7.3) or the
redundant DWT (see Chapter 7.6), the complexity of the wavelet system becomes O(N log(N)).
   If you are interested in more details of the discrete wavelet transtbrm and the discrete-time
wavelet transform, relations between them, methods of calculating them, further properties of
them, or examples, see Section 7.8 and Chapter9.
 Chapter 4


               Bases, Orthogonal Bases,
      Biorthogonal Bases, Frames, Tight
       Frames, and Unconditional Bases


Most people with technical backgrounds are familiar with the ideas of expansion vectors or basis
vectors and of orthogonality; however, the related concepts of biorthogonality or of frames and
tight frames are less familiar but also important. In the study of wavelet systems, we find that
frames and tight frames are needed and should be understood, at least at a superficial level.
One can find details in [You80, Dau92, Dau90, HW89J. Another perhaps unfamiliar
                                                                                      concept is
that of an unconditional basis used by Donoho, Daubechies, and others [Don93b, Mey90, Dau92]
to explain why wavelets are good for signal compression, detection, and denoising {GOL*94b,
GOL*94a]. In this chapter, we will very briefly define and discuss these ideas. At this point,
you may want to skip these sections and perhaps refer to them later when they are specifically
needed.


4.1    Bases, Orthogonal Bases, and Biorthogonal Bases

A set of vectors or functions fk (t) spans a vector space 下 (or F is the Span of the set) if any
element of that space can be expressed as a linear combination of members of that set, meaning:
Given the finite or infinite set of functions fk (t), we define Spank{ fk} = F as the vector
                                                                                             space
with all elements of the space of the form


                                         g(t) = 二 ak fk(t)                                         (4.1)
                                                  k

with k e Z and t, a E R. An inner product is usually defined for this space and is denoted
(f (t),g(t)). A norm is defined and is denoted by 11111 = v"TJ.
    We say that the set fk (t) is a basis set or a basis for a given space F if the set of {ak} in (4.1)
are unique for any particular g(t) e F. The set is called an orthogonal basis if (fk (t), f (t)) = 0 for
all k 尹 Z. If we are in three dimensional Euclidean space, orthogonal basis vectors are coordinate
vectors that are at right (90O) angles to each other. We say the set is an orthonormal basis if
(fk (t), f (t)) = d(k - Z) i.e. if, in addition to being orthogonal, the basis vectors are normalized
to unity norm: Ifk (t) I1 = 1 for all k.

                                                                                                    41
42                                                          Bases, Frames, and Unconditional Bases   Ch. 4


   From these definitions it is clear that if we have an orthonormal basis, we can express any
element in the vector space, g(t) E F, written as (4.1) by


                                   g(t) =       (g(t), fk(t)) fk(t)                                  (4.2)
                                            无


since by taking the inner product of fk(t) with both sides of (4.1), we get

                                         ak = (g(t), fk(t))                                          似3)

where this inner product of the signal g(t) with the basis vector 1k (t) "picks out" the corre-
sponding coefficient ak. This expansion formulation or representation is extremely valuable. It
expresses (4.2) as an identity operator in the sense that the inner product operates on g(t) to
produce a set of coefficients that, when used to linearly combine the basis vectors, gives back the
original signal g(t). It is the foundation of Parseval's theorem which says the norm or energy
can be partitioned in terms of the expansion coefficients ak. It is why the interpretation, stor-
age, transmission, approximation, compression, and manipulation of the coefficients can be very
useful. Indeed, (4.2) is the form of all Fourier type methods.
    Although the advantages of an orthonormal basis are clear, there are cases where the basis
system dictated by the problem is not and cannot (or should not) be made orthogonal. For these
cases, one can still have the expression of (4.1) and one similar to (4.2) by using a dual basis set
九 (t) whose elements are not orthogonal to each other, but to the corresponding element of the
expansion set
                                     (ft(t), 九떠） = d(Z 小 k)                                          (4.4)

Because this type of "orthogonality" requires two sets of vectors, the expansion set and the dual
set, the system is called biorthogonal. Using (4.4) with the expansion in (4.1) gives


                                   g(t) = ＞二(g(t), !k(ti' fk(t)                                      (4.5)
                                            k


Although a biorthogonal system is more complicated in that it requires, not only the original
expansion set, but the finding, calculating, and storage of a dual set of vectors, it is very general
and allows a larger class of expansions. There may, however, be greater numerical problems with
a biorthogonal system if some of the basis vectors are strongly correlated.
    The calculation of the expansion coefficients using an inner product in (4.3) is called the
analysis part of the complete process, and the calculation of the signal from the coefficients and
expansion vectors in (4.1) is called the synthesis part.
    In finite dimensions, analysis and synthesis operations are simply matrix-vector multiplica-
tions. If the expansion vectors in (4.1) are a basis, the synthesis matrix has these basis vectors
as columns and the matrix is square and non singular. If the matrix is orthogonal, its rows and
columns are orthogonal, its inverse is its transpose, and the identity operator is simply the matrix
multiplied by its tra四pose. If it is not orthogonal, then the identity is the matrix multiplied by
its inverse and the dual basis consists of the rows of the inverse. If the matrix is singular, then
its columns are not independent and, therefore, do not form a basis.
Sec. 4.1. Bases, Orthogonal Bases, and B向rthogonal Bases                                                                 43


卜ilatr江 Exam미es
Using a four dimensional space with matrices to illustrate the ideas of this chapter, the synthesis
formula g(t) = 드k ak fk(t) becomes



                                                             力nnn
                                                                      0
               g(0) '                  九（0)                                                  九（0)         I 巾（0) ]
                                            [
                                                                 /
                                                                 (
                                                                 ]
                                                                 1 n  乙 9  d
                                                                                                    『미 茹 1
               g(1)
                                                                 \
                             0         九（1) +                                      a         九（1)
                             O          1




                                                  + a1                                 n
                                                                                       d
                                                                                                                       (4.6)
               g(2)                    九（2)                                                  九（2)
                                        1
                                            1
                                                                 /11\ /11\ /
                                                                           1\
               g(3)                    九（3) L
                                                                                             九（3)         [, 九（3) ]

which can be compactly written in matrix form as

                         ' g(0) '   I 九（0)                 fi (0)               九（0)       月（0)     0 l
                                                                                                    O O
                           g(1)   = 1 九（1)                 fi (1)               九（1)       九（1)
                                                                                                    e
                                                                                                    O
                                                                                                    q                  (4.7)
                           g(2)     1 九（2)                 f (2)                九（2)       九（2)
                                                                                                    O
                                                                                                    U
                                                                                                    Q
                         . g(3) -   [. 九（3)                力（3)                 九（3)       九（3)

The synthesis or expansion equation (4.1) or (4.7) becomes

                                                          g = Fa,                                                      他8)

with the left-hand column vector g being the signal vector, the matrix F formed with the basis
vectors fk as columns, and the right-hand vector a containing the four expansion coefficients, ak.
   The equation for calculating the kt九 expansion coefficient in (4.6) is

                                                 ak = (g(t), 且（t)) = f]己g                                              似9)

which can be written in vector form as



                             q O O
                                 n n
                                 0
                                                .0(0)
                         r
                                                         .o(l)            fo(2)        小(3) ] f g(0)
                                 二
                         1
                         [
                                 l
                                                力（U)     力（1)             力（2)         力（3) 1 1 9(.l)
                                   J
                                   n
                                                                                                                      似10)
                         1
                         1
                                                和（0)     끄（1)             和（2)         f2(3) 1 1 9(2)
                                                九（0)     九（1)             九（2)         九（3) ] [. g(3) 中

where each ans an inne印roduct of the kt九 row of恥 毗h g and analy曲 or coeffi毗nt equat油1
(4,3) or (4.10) becomes
                                        a== iT
                                            ET g                                (4.11)
                                                                                   ll)

which together are (4.2) or
                                                         = FiTT g.
                                                        g=                                                            (4.12)
                                                                                                                      (4.l2)

Therefore,
                                                         iT
                                                         ET = Fl '                                                    (4.13)
                                                                                                                         l3)
is how the dual basis in (4.4) is found.
    If the columns of F are orthogonal and normalized, then

                                                         F FT = I.                                                    (4.14)
44                                                                            Bases, Frames, and Unconditional Bases         Ch. 4


This means the basis and dual basis are the same, and (4.12) and (4.13) become

                                                       g= FFTg                                                         (4.15)
and
                                                        ET = FT                             (4.16)
which are both simpler and more numerically stable than (4.13).
    The discrete Fourier transform (DFT) is an interesting example of a finite dimensional Fourier
transform with orthogonal basis vectors where matrix and vector techniques can be informative
as to the DFT's characteristics and properties, That can be found developed in several signal
processing books.

Fourier Series Example
The Fourier Series is an excellent example of an infinite dimensional composition (synthesis) and
decomposition (analysis). The expansion formula for an even function g(t) over 0 < x <2ir is

                                             g(t)＝三 ak cos(kt)                                                         (4.17)
                                                           k

where the basis vectors (functions) are

                                                      fk (t) = cos(kt)                                                 (4.18)
and the expansion coefficients are obtained as


                           따＝    (g
                                      (t)
                                             ,   1k
                                                      （小訂,        ITg   (t)
                                                                                c。
                                                                                 s  （胱）
                                                                                          」乞
                                                                                                                       (4.
                                                                                                                              19)
The basis vector set is easily seen to be orthonormal by verifying

                                            (ft(t), fk(t)) = d(k - Z).                                                 (4.20)
These basis functions span an infinite dimensional vector space and the convergence of (4.17)
must be examined. Indeed, it is the robustness of that convergence that is discussed in this
section under the topic of unconditional bases.

Sinc Expans向n Exam미e
Another example of an infinite dimensional orthogonal basis is Shannon's sampling expansion
[Mar9ll. If f (t) is band limited, then


                                1(t) = ＞二／(T川 '""｛社
                                                  ，：劤  丸            I
                                                                                                                       (4.21)

for a sampling interval T < 命 if the spectrum of 1 (t) is zero for w > W. In this case the
basis functions are the sinc functions with coefficients which are simply samples of the original
function. This means the inner product of a sinc basis function with a bandlimited function will
give a sample of that function. It is easy to see that the sinc basis functions are orthogonal by
taking the inner product of two sinc functions which will sample one of them at the points of
value one or zero.
 Sec. 4.2. Frames and Tight Frames
                                                                                                  45

 4.2    Frames and Tight Frames

While the conditions for a set of functions being an orthonormal basis are su田cient for the
representation in (4.2) and the requirement of the set being a basis is sufficient for (4.5), they
are not necessary. To be a basis requires uniqueness of the coefficients. In other words it requires
that the set be independent, meaning no element can be written as a linear combination of the
others.
   If the set of functions or vectors is dependent and yet does allow the expansion described in
(4.5), then the set is called a frame. Thus, a frame is a spanning set. The term frame comes from
a definition that requires finite limits on an inequality bound 1Dau92, You80] of inner products.
   If we want the coefficients in an expansion of a signal to represent the signal well, these
coefficients should have certain properties. They are stated best in terms of energy and energy
bounds. For an orthogonal basis, this takes the form of Parseval's theorem. To be a frame in a
signal space, an expansion set Pk (t) must satisfy

                                      A加112스 I(p丸,g)I25 Bflgf                                  (4.22)
                                                k

for some 0 <A and B < 以） and for all signals g(t) in the space. Dividing (4.22) by
                                                                                   19112 shows
that A and B are bounds on the normalized energy of the inner products. They "fr帥le" the
normalized coefficient energy. If
                                                    A= B                                       (4.23)
then the expansion set is called a tight frame. This case gives

                                         게1이2 = 易仇功尸                                           (4.24)
                                                      七

which is a generalized Parseval's theorem for tight frames. If A = B = 1, the tight frame becomes
an orthogonal basis. From this, it can be shown that for a tight frame [Dau92]

                                     g(t) = A"'＞二 (ak(t),g(t)) cpk(t)                         (4.25)
                                                 k

 which is the same as the expansion using an orthonormal basis except for the A ' term which is
a measure of the redundancy in the expansion set.
    If an expansion set is a non tight frame, there is no strict Parseval's theorem and the energy in
the transform domain cannot be exactly partitioned. However, the closer A and B are, the better
an approximate partitioning can be done. If A = B, we have a tight frame and the partitioning
can be done exactly with (4.24). Daubechies [Dau92] shows that the tighter the frame bounds
in (4.22) are, the better the analysis and synthesis system is conditioned. In other words, if A
is near or zero and/or B is very large compared to A, there will be numerical problems in the
analysis-synthesis calculations.
    Frames are an over-complete version of a basis set, and tight frames are an over-complete
version of an orthogonal basis set. If one is using a frame that is neither a basis nor a tight
frame, a dual frame set can be specified so that analysis and synthesis can be done as for a
non-orthogonal basis. If a tight frame is being used, the mathematics is very similar to using an
orthogonal basis. The Fourier type system in (4.25) is essentially the same as (4.2), and (4.24) is
essentially a Parseval's theorem.
46                                                                                           Bases, Frames, and Unconditional Bases    Ch. 4


     The use of frames and tight frames rather than bases and orthogonal bases means a certain
amount of redundancy exists. In some cases, redundancy is desirable in giving a robustness to
the representation so that errors or faults are less destructive. In other cases, redundancy is
an inefficiency and, therefore, undesirable. The concept of a frame originates with Duffin and
Schaeffer [DS521 and is discussed in [You80, Dau90, Dau92]. In finite dimensions, vectors can
always be removed from a frame to get a basis, but in infinite dimensions, that is not always
possible.
     An example of a frame in finite dimensions is a matrix with more columns than rows but with
independent rows. An example of a tight frame is a similar matrix with orthogonal rows. An
example of a tight frame in infinite dimensions would be an over-sampled Shannon expansion. It
is informative to examine this example.

Matrix Examples
An example of a frame of four expansion vectors fk in a three-dimensional space would be

                                                                                                                      a0
                       f g(0) ]   I 九（.0)                                    f (0)        九（．
                                                                                            이      /3(0) ]
                                                                                                                      a1
                       1 g(1) 1 = 1 九（1)                                     !i (1)       九（1)     九（') I                             (4.26)
                                                                                                                      a2
                       [. g(2) j  [. 九（2)                                    fi (2)       九（2)     九（2) ]
                                                                                                                      a3

which corresponds to the basis shown in the square matrix in (4.7). The corresponding analysis
equation is



                                  O O O n
                                      0


                                      l


                                      八
                                      1
                                      1
                                                                                                                                      (4.27)
                                      Q
                                      U
                                             1=
which corresponds to (4.10). One can calculate a set of dual frame vectors by temporarily
appending an arbitrary independent row to (4.26), making the matrix square, then using the
first three columns of the inverse as the dual frame vectors. This clearly illustrates the dual
frame is not unique. Daubechies [Dau92] shows how to calculate an "economical" unique dual
frame.
    The tight frame system occurs in wavelet infinite expansions as well as other finite and infinite
dimensional systems. A numerical example of a frame which is a normalized tight frame with
four vectors in three dimensions is


                                                                                                                   0 l 2 3
                                                                                                     lll
                                                                                      l
                                                                                      1
                                                                                                               e
                                                                               l
                                                                                             l l
                                                                                                           m

                           F g(0) 1
                                                                         戶
                                                                         [
                                                                                                               1
                                                                                                               [
                                                                             1
                                                                             ]                             1


                                                                                       l l
                                                                                                                   O O O O
                                                  j
                                                                                                               1
                           I     ,-.              I        1   .1
                                                                         1
                           I 9(1) I = =＝三                                                                                             (4.28)
                                                                                             l
                                                                                             1
                                                                                                           1
                                                                                                               1
                                      /l\ /3                                   l
                                                                         1
                                                                                                               1
                                (2)
                                                                                                           J
                           Lg
which includes the redundancy factor from (4.25). Note the rows are orthogonal and the columns
are normalized, which gives




                                                           ]
                                                                                   l
                                                                                                                    l
                                                                                                                    4        0
                                            l l
                                                                                                                       0 0

                                                                                                                                 4H
                                                                                                                                  3
                                                      1上                                                   1
                                                                                                           4
                           1                                                   l
                                                                               ]                                           l
                                                                                                                           d           四
                                                      l              1                                                     0           4
     FFT=                  1                                                     l
                                                                                 4                             小
                                                                                                               n
                                                                                                               d         i
                                                                                                                         1
                                l
                                ]                                                                                        0 0
                       -
                  [1
                                                      4
                                                      11
                           1                                   \／죵
                                                                                   l
Sec. 4.2. Frames and Tight Frames                                                                                                                       47


or
                                                                                1                               m:

                                                                            g= i Fln ' g                                                             (4.30)

which is the matrix form of (4.25). The factor of A = 4/3 is the measure of redundancy in this
tight frame using four expansion vectors in a three-dimensional space.
    The identity for the expansion coefficients is
                                                                                             F              T   F
                                                      =                         a
                                                                                            l A
                                                                                            卄
                                                                                                                     a
                                                                                                                                                     (4.31)

which for the numerical example gives




                              ml ]l l l
                    ]
                    l     1
                          1
                          1
                          1
                                                                                        -1/ 3『                             f  1       1/3     1/3


                                                          r 1 1 1 1 L
                                                                                    1
                                                                                    l                   1
                                                                                                        l            m
                                                                                                                     l
                    l     ]
                          l                                             1               1




       꺄
                                                                                        1




                                                  1                                      1/3                             = I 1/3       1     -1/ 3
            l
 I汀                                                                     1
                                                                        上           d
                                                                                    l                   4
                                                                                                        l            m
                                                                                                                     l
                                                                                                    H




                    m
                    l     l
                                                                                                        小




                                                                        ]
                                                                        l           ]
                                                                                    l    1/3            ]
                                                                                                        l
                                                                                                            H



                                                                                                                     m
                                                                                                                     l     I 1/3     -1/ 3     1
                    ］
                    工     l
                          l
                                            \/g
                                                                                          1
            而
                                                                                                    H       1

                                                                                                                             -1/ 3    1/3     1/3
                                                                                            (4.32)
Although this is not a general identity operator, it is an identity operator over the three-
dimensional subspace that a is in and it illustrates the unity norm of the rows of FT and columns
of F.
    If the redundancy measure A in (4.25) and (4.29) is one, the matrices must be square and the
system has an orthonormal basis.
    Frames are over-complete versions of non-orthogonal bases and tight frames are over-complete
versions of orthonormal bases. Tight frames are important in wavelet analysis because the restric-
tions on the scaling function coefficients discussed in Chapter 5 guarantee not that the wavelets
will be a basis, but a tight frame. In practice, however, they are usually a basis.

Sinc Expansion as a Tight Frame Example
An example of an infinite-dimensional tight frame is the generalized Shannon's sampling e자）an-
sion for the over-sampled case [Mar91]. If a function is over-sampled but the sinc functions
remains consistent with the upper spectral limit W, the sampling theorem becomes


                                    g(t) = 뿌＞二9但미"캄료半                                                                                                (4.33)


or using R as the amount of over-sampling

                                                          R仍／ =                         冗7      ,               forR> 1                              (4.34)

we have

                                          g(t)                          去＞二g(T미 "' 烈名）)
                                                                            n
                                                                                                                                                     (4.35)


where the sinc functions are no longer orthogonal now. In fact, they are no longer a basis as they
are not independent. They are, however, a tight frame and, therefore, act as though they were
an orthogonal basis but now there is a "redundancy" factor R as a multiplier in the formula.
48                                                        Bases, Frames, and Unconditional Bases    Ch. 4


    Notice that as R is increased from unity, (4.35) starts as (4.21) where each sample occurs
where the sinc function is one or zero but becomes an expansion with the shifts still being
t = Tn, however, the sinc functions become wider so that the samples are no longer at the zeros.
If the signal is over-sampled, either the expression (4.21) or (4.35) could be used. They both
are over-sampled but (4.21) allows the spectrum of the signal to increase up to the limit without
distortion while (4.35) does not. The generalized sampling theorem (4.35) has a built-in filtering
action which may be an advantage or it may not.
    The application of frames and tight frames to what is called a redundant discrete wavelet
transform (RDWT) is discussed later in Section 7.6 and their use in Section 10.3. They are also
needed for certain adaptive descriptions discussed at the end of Section 7.6 where an independent
subset of the expansion vectors in the frame are chosen according to some criterion to give an
optimal basis.


4.3    Conditional and Unconditional Bases
A powerful point of view used by Donoho [Don93b] gives an explanation of which basis systems
are best for a particular class of signals and why the wavelet system is good for a wide variety of
signal classes.
    Donoho defines an unconditional basis as follows. If we have a function class F with a norm
defined and denoted n · I I下 and a basis set f, such that every 血nction g E F has a unique
representation g = ＞二k ak 1k with equality defined as a limit using the norm, we consider the
infinite expansion

                                     g(t) = ＞二Tflk ak ／小）·                                         (4.36)
                                              k

If for all g e F, the infinite sum converges for all ImkI 5 1, the basis is called an unconditional
basis. This is very similar to unconditional or absolute convergence of a numerical series [Don93b,
You80, Mey90]. If the convergence depends on mk = 1 for some g(t), the basis is called a
conditional basis.
    An unconditional basis means all subsequences converge and all sequences of subsequences
converge. It means convergence does not depend on the order of the terms in the summation
or on the sign of the coefficients. This implies a very robust basis where the coefficients drop
off rapidly for all members of the function class. That is indeed the case for wavelets which are
unconditional bases for a very wide set of function classes [Dau92, Mey93, Gri93].
    Unconditional bases have a special property that makes them near-optimal for signal process-
ing in several situations. This property has to do with the geometry of the space of expansion
coefficients of a class of functions in an unconditional basis. This is described in [Don93b].
    The fundamental idea of bases or frames is representing a continuous function by a sequence
of expansion coefficients. We have seen that the Parseval's theorem relates the L2 norm of the
function to the Z2 norm of coefficients for orthogonal bases and tight frames (4.24). Different
 function spaces are characterized by different norms on the continuous function. If we have an
unconditional basis for the function space, the norm of the function in the space not only can
be related to some norm of the coefficients in the basis expansion, but the absolute values of the
coefficients have the sufficient information to establish the relation. So there is no condition on
the sign or phase information of the expansion coefficients if we only care about the norm of the
 function, thus unconditional.
Sec. 4.3. Conditional and Unconditional Bases
                                                                                               49


   For this tutorial discussion, it is sufficient to know that there are theoretical reasons why
wavelets are an excellent expansion system for a wide set of signal processing problems. Being
an unconditional basis also sets the stage for efficient and effective nonlinear processing of
                                                                                               the
wavelet transform of a signal for compression, denoising, and detection which are discussed in
Chapter 10.
Chapter 5


       The Scaling Function and Scaling
      Coefficients, Wavelet and Wavelet
                             Coe什ic陀nts


We will now look more closely at the basic scaling function and wavelet to see when they exist
                                                                                                the
and what their properties are [DD87, Mal89b, Law90, Law91b, Law91a, LR91, Dau92]. Using
same approach that is used in the theory of  differential equations, we will examine the properties
                                                                                             (2.13)
of 97(t) by considering the equation of which it is a solution. The basic recursion equation
that comes from the multiresolution formulation     is


                                  甲(t) =＞그回 扼a小 n)                                             (5.1)


                                                                                                 this
with h(n) being the scaling coefficients and y(t) being the scaling function which satisfies
equation which is sometimes called the refinement equation, the dilation equation,      or the  mul-
tiresolution analysis equation (MRA).
    In order to state the properties accurately, some care has to be taken in specifying just what
classes of functions are being considered or are allowed. We will attempt to walk a fine line to
                                                                                                   A
present enough detail to be correct but not so much as to obscure the main ideas and results.
few of these ideas were presented in Section 2.1 and a few more will be given in the next section. A
                                                                       s  to [VK95,  Wic95, Koo931,
more complete discussion can be found in [VD951, in the introduction
or in any book on function analysis.



5.1    Tools and Definitions
Signal Classes
There are three classes of signals that we will be using. The most basic is called L2 (R) which
contains all functions which have a finite, well-defined integral of the square: f E L2         斗
                                               because it is a generalizati on of normal Euclidean
f f (t)I2 dt = E < 凹. This class is important
geometry and because it gives a simple representation of the energy in a signal.
   The next most basic class is L1(R), which requires a finite integral of the absolute value of
the function: I E L1 수 f If (t)I dt = K < 的. This class is important because one may

 50
Sec. 5.1. Tools and Definitions                                                                                                                    51


interchange infinite summations and integrations with these functions although not necessarily
with L2 functions. These classes of function spaces can be generalized to those with intlf (t)iP dt =
K' <oc and designated L.
    A more general class of signals than any L!7 space contains what are called dist鹿butions.
These are generalized functions which are not defined by their having "values" but by the value
of an "inner product" with a normal function. An example of a distribution would be the Dirac
delta function d(t) where it is defined by the property: f (T) = f f (t) 8(t - T) dt.
    Another detail to keep in mind is that the integrals used in these definitions are Lebesque
integrals which are somewhat more general than the basic Riemann integral. The value of a
Lebesque integral is not affected by values of the function over any countable set of values of
its argument (or, more generally, a set of measure zero). A function defined as one on the
rationals and zero on the irrationals would have a zero Lebesque integral. As a result of this,
properties derived using measure theory and Lebesque integrals are sometime said to be true
 "almost everywhere," meaning they may not be true over a set of measure zero.
    Many of these ideas of function spaces, distributions, Lebesque measure, etc. came out of
the early study of Fourier series and transforms. It is interesting that they are also important
in the theory of wavelets. As with Fourier theory, one can often ignore the signal space classes
and can use distributions as if they were functions, but there are some cases where these ideas
are crucial. For an introductory reading of this book or of the literature, one can usually skip
over the signal space designation or assume Riemann integrals. However, when a contradiction
or paradox seems to arise, its resolution will probably require these details.

Fourier Transforms
We will need the Fourier transform of 99(t) which, if it exists, is defined to be

                                       .                      =
                                                                                                            e_        "t
                                                                                                                                      dt         (5.2)
                                                                    J- 。。
                                                                                               (t)
                                                                        /：『
                                             (w)
and the discrete-time Fourier transform (DTFT) {OS89] of h(미 defined to be
                                                                                  (X)


                                         표         （口J)       =
                                                                        n= - 的
                                                                              ＞二               /i    (n)         eH                  '" "
                                                                                                                                                 (5.3)


where i = \/1i and ii is an integer (ii E Z). If convolution with h(미 is viewed as a digital filter,
as defined in Section 3.1, then the DTFT of h(n) is the filter 's frequency response, [OS89, PB87J
which is 2ir periodic.
   If 面(w) exits, the defining recursive equation (5.1) becomes

                                   令   (w)                =                                                                                      (5.4)
                                                                  寸2且                    （w/               2)    .             (w/          2)
which after iteration becomes


                                  .回小件畔和.）·               丸＝l                 \    ! 1                                     /
                                                                                                                                                 (5司
if 二 h(n) = \／牙 and 令 (O) is well defined. This may be a distribution or it may be a smooth
function depending on H (w) and, therefore, h(미 [VD95, Dau92]. This makes sense only if 호(O)
52                                                                                     The Scaling and Wavelet Functions and Coefficients                Ch. 5


is well defined. Although (5.1) and (5.5) are equivalent term-by-term, the requirement of 重(0)
being well defined and the nature of the limits in the appropriate function spaces may make
                                                                                            one
preferable over the other. Notice how the zeros of H (w) determine the zeros of 4 (w).


Refinement and Transition Matrices
There are two matrices that are particularly important to determining the properties of
                                                                                            wavelet
systems. The first is the refinement matrix M, which is obtained from the basic recursion equa-
tion (5.1) by evaluating Y9 (t) at integers [MP89, DL91, DL92, SN96, Str96a]. This looks like a
convolution matrix with the even (or odd) rows removed. Two particular submatrices
                                                                                           that are
used later in Section 5.10 to evaluate 甲(t) oil the dyadic rationals are illustrated for N = 6 by




                                枷m뇨0 00
                                                                                        00mm뇨0
                                             0M枷k0 0       0枷枷枷 00      00M屈粃0                    000M枷粃
                                                                                                                 0 l 2 3 4 5


                                                                                                                                       甲 甲 甲 甲 甲 甲
                                                                                 寸


                                                                                                                                              0

                                                                                                                                              l

                        而

                                                                                                                 甲 甲 甲 甲 甲 甲
                                                                                                                                              八J乙

                                                                                                                                              口U         侮6)
                                                                                                                                              4

                                                                                                                                              5




which we write in matrix form as

                                                                                                                                                         (5.7)
with M0 being the 6 x 6 matrix of the h(n) and p being 6 x 1 vectors of integer samples of
                                                                                                (t).
In other words, the vector 99 with entries 甲(k) is the eigenvector of M0 for an eigenvalue
                                                                                           of unity.
    The second submatrix is a shifted version illustrated by




                            M枷姚 000       mm뇨 000      0M枷桃0 0       0桃m뇨 00         00Mm桃0   0 0m幻뇨 0
                                                                                                           0 l     4 5
                                                                                                                                                     m




                                                                                                                                     Pl/2

                      而                                                                                                              P3/2


                                                                                                                 U
                                                                                                                 口
                                                                                                                               -     P5/2


                                                                                                           甲 甲 {
                                                                                                               甲
                                                                                                               n m
                                                                                                                 甲 甲 甲
                                                                                                                                                         侮8)
                                                                                                                                     f 7/2
                                                                                                                                     p9/2
                                                                                                                                   - P11/2

with the matrix being denoted M1. The general refinement matrix M is the infinite matrix of
which M0 and M1 are partitions. If the matrix H is the convolution matrix for h(n), we can
denote the M matrix by [t 2]H to indicate the down-sampled convolution matrix H. Clearly,
                                                                                              for
甲(t) to be defined on the dyadic rationals, M0 must have a unity eigenvalue.
   A third, less obvious but perhaps more important, matrix is called the transition matrix T
and it is built up from the autocorrelation matrix of h(n). The transition matrix is constructed
by
                                                                     T = [1. 2]HHT.                                                                      侮9)
This matrix (sometimes called the Lawton matrix) was used by Lawton (who
                                                                                   originally called
it the Wavelet-Galerkin matrix) [Law91a] to derive necessary and sufficient conditions for an
orthogonal wavelet basis. As we will see later in this chapter, its eigenvalues are also important
in determining the properties of 99(t) and the associated wavelet system.
 Sec. 5.2. Necessary Conditions                                                                                                             53

 5.2    Necessary Conditions

 Theorem 1 If y7(t)        乙1 is a soh虎幻n 切 坑eb口sic recurs切n equat幻n (5.1) and if / 甲（t) dt 尹 0,
 then
                                                                               ＞二／1（미 = \／三                                              (5.10)


The proof of this theorem requires oniy an interchange in the order of a summation and integration
(allowed in L1) but no assumption of orthogonality of the basis functions or any other
                                                                                           properties
of 甲(t) other than a nonzero integral. The proof of this theorem and several of the others stated
here are contained in Appendix A.
    This theorem shows that, unlike linear constant coefficient differential equations, not just any
set of coefficients will support a solution. The coefficients must satisfy the linear equation (5.10).
This is the weakest condition on the h(n).

Theorem 2 {/ 甲(t) is an 乙1 solut加n to 坑eb口5比 recurs切n equ口tion (5.1) 凹ith 加 （t) dt = 1,
and
                                                        ＞二甲（t+ t) = ＞二甲（Z) = 1
                                 Z                                                                         t
wit九 令(ir + 2ir丸）；三 0 加r some 丸， 仇en

                                                        ＞그(2미 = ）二 九（2n + 1)
                                                             n                                         n


where (5.11) m口yh口ye 切 be a 硫就I吃but可（7na1 sw-n. Converse匈， {/ (5.12) is sa挽sfied, 坑en (丘11)
is true.

Equation (5.12) is called the fundamental condition, and it is weaker than requiring orthogonali
                                                                                                    ty
but stronger than (5.10). It is simply a result of requiring the equations resulting from evaluating
(5.1) on the integers be consistent. Equation (5.11) is called a partitioning of unity (or the Strang
condition or the Shoenberg condition).
    A similar theorem by Cavaretta. Dahman and Micchelli [CDM91] and by Jia [Jia95] states
that if Y7 e L끄 and the integer translates of 99(t) form a Riesz basis for the space they span,
                                                                                                 then
乙可2n) = 乙小(2n + 1).
Theorem 3 {／甲(t) 可S an 工2nL1 solut加n to (丘1) 口nd 毛／ii工teger tr口nslates of co(t) are
                                                                                    or坑ogonal
as d可沇記 by
                                                                                                                   IE ifk= 0
                           n
                                   (!
                                        )7
                                                   (!
                                                         ．
                                                                     丸）
                                                                               毗 :    月(5        （丸）
                                                                                                               :
                                                                                                                    (0     otherwise,
疏e凡
                               乞如h(n- 2劤 = (5（丸） = f1 ifk= 0
                                                                                                                   10     0坑ei切昭e.

Notice that this does not depend on a particular normalization of (t).
    If Y7 (t) is normalized by dividing by the square root of its energy V'i, then integer translates
of 뚜7(t) are orthonormal defined by


                               f             (t)
                                                   『    (t
                                                                 -        k)
                                                                                dt:    8
                                                                                           (k)
                                                                                                           =       {:
                                                                                                                         if 丸 = 0
                                                                                                                         otherwise.
                                                                                                                                        (5.15)
                                                     The Scaling and Wavelet Functions and Coefficients    Ch. 5
54

    This theorem shows that in order for the solutions of (5.1) to be orthogonal under integer
translation, it is necessary that the coefficients of the recursive equation be orthogonal themselves
after decimating or downsampling by two. If 99(t) and/or h(n) are complex functions, com1lplex
conjugation must be used in (5.13), (5.14), and (5.15).
    Coefficients h(n) that satisfy (5.14) are called a quadrature mzrror filter (QMF) or conjugate
mirror filter (CMF), and the condition (5.14) is called the quadratic condition for obvious reasons.

Corollary 1 Under the assumptions of Theorem 3, the norm of h(n) is automatically unity.

                                          ＞二
                                           n
                                               1九
                                                         （n)
                                                               I2   =   1
                                                                                                          (5.16)


                                                                                         of
Not only must the sum of h(n) equal \／豆 but for orthogonality of the solution, the sum
the squares of h(n) must be one, both independent of any normalizatio n of 甲(t). This unity
normalization of h(n) is the result of the V／亘 term in (5.1).

Corollary 2 Under the assumptions of Theorem 3,


                               口 （2미 : 二h(2n + 1) = 1흐
                                 n                  fl
                                                                                                          (5.17)


This result is derived in the Appendix by showing that not only must the sum of h(n) equal
                                                                                          in h(n)
V' , but for orthogonality of the solution, the individual sums of the even and odd terms
must be l/ V／云 independent of any normalization of (t). Although stated here as necessary for
orthogonality, the results hold under weaker non-orthogonal conditions as is stated in Theorem 2.

Theorem 4 If p(t) has compact support on 0 < t < N- i and if cp(t- k) are linearly independent,
坑en h(미 毗so has corn끄act s2叩POT寸 over 0 드 n 드 N 寸 1:

                                h(n) -oforn<                   oandn> N- 1                                (5.18)

 Thus N is the length of the h(n) sequence.

If the translates are not independent (or some equivalent restriction), one can have h(n) with
infinite support while 甲(t) has finite support [Ron92].
    These theorems state that if 甲(t) has compact support and is orthogonal over integer trans-
                                                                                      one linear
lates, 퓽 bilinear or quadratic equations (5.14) must be satisfied in addition to the
                                                            must  be an  even number.  The num-
equation (5.10). The support or length of h(n) is N, which
ber of degrees of freedom in choosing these N coefficients is then  誓  - 1. This freedom will be
used in the design of a wavelet system developed in Chapter   6 and elsewhere.


 5.3    Frequency Domain Necessary Conditions
 We turn next to frequency domain versions of the necessary conditions for the existence of 99 (t).
 Some care must be taken in specifying the space of functions that the Fourier transform operates
 on and the space that the transform resides in. We do not go into those details in this book but
 the reader can consult [VD951.
Sec. 5.3. Frequency Domain Necessary Conditions                                                   55


Theorem 5 If 甲(t) is a L' solution of the basic recursion equation (5.1), 坑en 坑e 加liowing
equivaleni conditions must be true:

                                         ＞二九（미 = H(0) rrV'                                    伍19)




This follows directly from (5.3) and states that the basic existence requirement (5.10) is equivalent
to requiring that the FIR filter's frequency response at DC (w = 0) be V5.

Theorem 6 For h(n) E Z1, then

                       ＞二九（2미 = ＞二九（2n+ 1) ifando毗yi/ 丑（미 = 0                                  (5.20)



which says the frequency response of the FIR filter with impulse response h(n) is zero at the
so-called Nyquist frequency (w = ir). This follows from (5.4) and (7.7), and supports the fact
that h(n) is a lowpass digital filter. This is also equivalent to the M and T matrices having a
unity eigenvalue.

Theorem 7 ｛加（t) is a soh虎可or工 切 (5.1) in L2 n 尸 口nd 4 (w) is 口 soh虎ion of (5．刃 Si工C／工 th毗
令(0) j三 0, 坑en


                 f (t)『(t-k)dt = 8（劤 *f andon蜘／쭈陣（w+2ir『)I2= 1                                 (5.21)




 This is a frequency domain equivalent to the time domain definition of orthogonality of the scaling
 function [Mal89b, Mal89c, Dau92]. It allows applying the orthonormal conditions to frequency
 domain arguments. It also gives insight into just what time dom曲l orthogonality requires in the
 frequency domain.

 Theorem 8 For any h(n) e Zl,

          ＞二／1(n）九（n - 2k) =6（劤           if and only{/   IH（回）尸 + 1H(w+1)12 = 2               (5.22)
           n




 This theorem [Law90, Hei93, Daia92] gives equivalent time and frequency domain conditions
 on the scaling coefficients and states that the orthogonality requirement (5.14) is equivalent to
 the FIR filter with h(n) as coefficients being what is called a Quadrature Mirror Filter (QMF)
 ESB86a1. Note that (5.22), (5.19), and (5.20) require H (ir/2)I = 1 and that the filter is a "half
 band" filter.
 56                                              The Scaling and Wavelet Functions and Coefficients     Ch. 5

 5.4    Su什icient Con버t向ns
The above are necessary conditions for 99(t) to exist and the following are sufficient. There are
many forms these could and do take but we present the following as examples and give references
for more detail [DD87, Mal89b, Law90, Law91b, Law91a, LR91, Dau92, LLS97b, LLS97a, Law97].

Theorem 9 If 乙小（미 = \／프 口nd h(n) 九口s finite s2／끄port or decays fast enough so 坑口t
刃／  i (n)I(1-- I띠）' < 的 加r some e > 0, 坑en 口 unique (w可thin 口 scalar mu砒刃le) 甲(t) 伽er/ia끄S 口
dist,苞b乞比ion) exis加 that sa挽sfies (5.1) （工rid whose 硫S加-ib2成on毗 只)urzer tr口nsforrn 吼比isfies (5.5).


This [DD87, Law90, Law] can be obtained in the frequency domain by considering
                                                                                 the convergence
of (5.5). It has recently been obtained using a much more powerful approach in the time domain
by Lawton [Law97J.
    Because this theorem uses the weakest possible condition, the results are weak. The scaling
function obtained from only requiring 兄 h(n) = \／易 may be so poorly behaved as to be impos-
sible to calculate or use. The worst cases will not support a multiresolution analysis or provide
a useful expansion system.

Theorem 10 1/ 兄力（2n) = 드nh(2n+ i) = i/ v／易 口nd h（미 脆S／流te su끄끄ort or decays ／口st
eno2坦／i so 坑毗 乞 呵미1(1 + jnI) ' ＜二 以） for some E > 0, 坑en a 甲(t) 伽erhaps a 硫str功毗可on)
that satisfies (5.1) exists, is unique, and is well-defined on the dyadic rationals. In addition, the
dis加吼m挽on口／ sum
                                         ＞二甲(t - k) = i                                               (5.23)
                                          丸
加k加．

This condition, called the fundamental condition [SN96, LLS97b], gives a slightly tighter
                                                                                          result
than Theorem 9. While the scaling function still may be a distribution not in L1 or L2, it is
better behaved than required by Theorem 9 in being defined on the dense set of dyadic rationals.
This theorem is equivalent to requiring H (미 = 0 which from the product formula (5.5) gives
a better behaved m (w). It also guarantees a unity eigenvalue for M and T hut not that other
eigenvalues do not exist with magnitudes larger than one.
    The next several theorems use the transition matrix T defined in (5.9) which is a down-
sampled autocorrelation matrix.

Theorem 11 If the transition matrix T has eigenvalues on or in the unit circle of the complex
p／口ne and 毛／（工ny on 坑e unit circle are multiple, 坑ey h（工ye a corn刃lete set of e四envec切rs, 坑en
甲(t) EL2.
If T has unity magnitude eigenvalues, the successive approximation algorithm (cascade algorithm)
(5.71) converges weakly to 甲(t) E L2 [Law].
Theorem 12 可 仇e tr口I工sit切n m（比7巨x T has a sirn刃／e un可ty eigenvalue a凡t／工 （工／l other eigenval?工es
h（工ving m（四n可tude less 坑an one, 坑en 甲(t) E L2.

Here the successive approximation algorithm (cascade algorithm) converges strongly to 99(t) E
                                                                                              L2.
This is developed in [SN96].
   If in addition to requiring (5.10), we require the quadratic coefficient conditions (5.14), a
tighter result occurs which gives o(t) E 乙2(R) and a multiresolution tight frame system.
 Sec. 5.4. Sufficient Conditions
                                                                                                   57


 Theorem 13 (Lawton) If h(n) has finite support or decaus fast enouah and if 5T.. h(n') = \／牙
 and 可f y,... 九（n) ,山2 H 2肋 = 8（丸）, 疏en 四(t) E L2(R) e娩就s, and qener口tes （工 wa胤et sustem 坑口t
 is a tight frame in L2.

 This important result from Lawton [Law90, Law91b] gives the sufficient conditions for 甲(t) to
 exist and generate wavelet tight frames. The proof uses an iteration of the basic recursion equation
 (5.1) as a successive approximation similar to Picard's method for differential equations. Indeed,
 this method is used to calculate 甲(t) in Section 5.10. It is interesting to note that the scaling
 function may be very rough, even "fractal" in nature. This may be desirable if the signal being
 analyzed is also rough.
     Although this theorem guarantees that 99(t) generates a tight frame, in most practical situ-
 ations, the resulting system is an orthonormal basis [Law91b]. The conditions in the following
 theorems are generally satisfied.

Theorem 14 化aw切n) 1/ 카n) 肋5 corn끄act su까）ort, 乙小（미 = \／확 and 兄小回
                                                                                h(n - 2劤 =
히砒 坑ei工 甲(t - 丸） fo竹ns 口ii or坑ogon口1 set if ai工d onll/ 可／ 坑e tr口nsition m口打4T T 九（工S a sim끄le
un啣 e勾env口lue.

This powerful result allows a simple evaluation of h(n) to see if it can support a wavelet expansion
system [Law90, Law91b, Law91a]. An equivalent result using the frequency response of the FIR
digital filter formed from h(n) was given by Cohen.

Theorem 15 (Co九en) 1/ 표（미 is 坑e DTFT of h（미 凹it九 compact sup끄ort 口nd
                                                                     Z，
                                                                      小(n) = V／牙
wit九 兄小回 九(n- 2肋 = 8（砒and i사1(w) / 0 for -ir/ 3 드 四 드 冗／3, 坑en 坑eo(t- k) 5口tis央／ing
(5.1) gener口扼 an or坑onorm口lb口$招 航 L2.

A slightly weaker version of this frequency domain sufficient condition is easier to prove [Mal89b,
Mal89cJ and to extend to the M-barid case for the case of no zeros allowed in -ir/ 2 <w <ir/ 2
[Dau921. There are other sufficient conditions that, together with those in Theorem 13, will
guarantee an orthonormal basis. Daubechies' vanishing moments will guarantee an orthogonal
bas始．
   Theorems 5, 6, and 15 show that h(n) has the characteristics of a lowpass FIR digital filter.
We will later see that the FIR filter made up of the wavelet coefficients is a high pass filter
                                                                                                and
the filter bank view developed in Chapter 3 and Section 7.2 further explains this view.

Theorem 16 If h(n) has finite support and if o(t) E L1, then o(t) has finite support [Law].

If o(t) is not restricted to L1, it may have infinite support even if h(n) has finite
                                                                                      support.
    These theorems give a good picture of the relationship between the recursive equation coeffi-
cients h(n) and the scaling function o(t) as a solution of (5.1). More properties and characteristics
are presented in Section 5.8.

Wavelet System Design
One of the main purposes for presenting the rather theoretical results of this chapter is to set up
the conditions for designing wavelet systems. One approach is to require the minimum sufficient
conditions as constraints in an optimization or approximation, then use the remaining degrees of
58                                                             The Scaling and Wavelet Functions and Coefficients         Ch. 5


freedom to choose h(n) that will give the best signal representation, decomposition, or compres-
sion. In some cases, the sufficient conditions are overly restrictive and it is worthwhile to use the
necessary conditions and then check the design to see if it is satisfactory. In many cases, wavelet
systems are designed by a frequency domain design of H (w) using digital filter design techniques
with wavelet based constraints.


5.5    The Wavelet
Although this chapter is primarily about the scaling function, some basic wavelet properties are
included here.

Theorem 17 If仇e Sc毗初四 CO町泡飢拓 h(미 S口tis央／ t九e cond可t秀ons for existence and or坑ogonality
0/ 坑e Sc（流ng 加nc蜘n and 仇e i夙ivelet is de／沇ed b!/ 但2刃， 坑en 仇e integer transh虎es of this
wavelet span W0, the orthogonal compliment of V0, both being in V1, i.e., the wavelet is orthogonal
切 仇e Sc口ling function at 坑e sai了ie sca厄


                                    f    (t-
                                                     n)
                                                               砂(t-   m)
                                                                                dt =   0,
                                                                                                                    (5.
                                                                                                                            24)

可／口ad onh/ 寸 仇e coefficients h1（미 are g初en by

                                     hi(n) = 士（-1少h(N 小n)                                                           伍25)


 where N is an arbitrary odd integer chosen to conveniently position h1(n).

 An outline proof is in Appendix A.

 Theorem 18 {／坑e sc毗仇g coe丹icie冗加 h(n) 5口瓦5加 仇e conditions for e娩就卽tce and or仇四아ial畇／
 0/ 坑e sca油四 /unction and 坑e wavelet is de／沇ed by (2.2.4), 坑en 坑e integer 加口nslates of this
 wa胤就 叩an W0! 仇e or仇四onal con叩渤比nt of V0, 切仇 beir四 in V1; i.e., 坑ew（工velet is or仇四onal
 切 仇e Sc（工ling func挽（77i 毗 坑e 馭zme sc口le. If


                                     J         (t-
                                                          n)
                                                               砂(t-        m)
                                                                                 dt = 0
                                                                                                                          侮26)


 坑en
                                      ＞二／i(n) hi(n 小 2k) = 0                                                              伍27)


 which is derived in Appendix A, equation (12.39).
    The translation orthogonality and scaling function-wavelet orthogonality conditions in (5.14)
 and (5.27) can be combined to give

                                ＞二九Z(n）九，.(n- 2k) = d(k) d(Z                                m)                            伍28)


 if ho(n) is defined as h(n).
                                                                                                  59
Sec. 5.6. 시ternate Norn伯lizat向ns


Theorem 19 If h(n) satisfies the linear and quadratic admissibility conditions of (5.10) and
(5.14), then
                                     ＞二九1（미 = 月1(0) = 0,                                       (5.29)

                                      1Hi（回）1 = 田（口7+ ir)I,                                    (5.30)

                                      1표（w)I2+ 田如）尸 =2,                                        他31)
and
                                           ／砂
                                                （!   )dt＝
                                                            『                                  (5.32)


The wavelet is usually scaled so that its norm is unity.
   The results in this section have not included the effects of integer shifts of the scaling function
or wavelet coefficients h(n) or hi(n). In a particular situation, these sequences may be shifted to
make the corresponding FIR filter causal.


5.6    Alternate Normalizations
An alternate normalization of the scaling coefficients is used by some authors. In some ways, it
is a cleaner form than that used here, but it does not state the basic recursion as a normalized
                                                                                             the
expansion, and it does not result in a unity norm for h(n). The alternate normalization uses
ba駁c multiresolution recursive equation  with no  \／牙


                                     甲（t) =Z枷) (2t - n)·                                       侮33)

Some of the relationships and results using this normalization are:

                                   兄丑미 = 2
                                   ＞二nIh(n）尸 = 2
                                    小（미 九(h - 2k) = 25（히
                                   Z，                                                          侮34)
                                    小（2n) = ZJ但n + 1) = 1
                                   Z，
                                   H (0) = 2

                                   田佃甲 뉘且佃 + It기2 = 4

A still different normalization occasionally used has a factor of 2 in (5.33) rather than \／牙 or
                                                                                    places in this
unity, giving 兄 h(n) = 1. Other obvious modifications of the results in other
book can be worked out. Take care in using scaling coefficients h(n)  from the literature as some
must be multiplied or divided by V牙 to be consistent with  this book.


5.7     Example Scaling Functions and Wavelets
Several of the modern wavelets had never been seen or described before the 1980's. This section
looks at some of the most common wavelet systems.
 60                                                  The Scaling and Wavelet Functions and Coefficients    Ch. 5

 Haar Wave1ets
The oldest and most basic of the wavelet systems that has most of our desired properties
                                                                                                is
constructed from the Haar basis functions. If one chooses a length N = 2 scaling coefficient
                                                                                              set,
after satisfying the necessary conditions in (5.10) and (5.14), there are no remaining
                                                                                       degrees or
freedom. The unique (within normalization) coefficients are

                                             i i
                                      h(n) = < ==.              三扼                                        伍35)
                                        "       (,
                                                      \/2
                                                            "




and the resulting normalized scaling function is


                                             Cf六t1
                                    甲（t)= 11 ：                                                            侮36)
The wavelet is, therefore,
                                         11      for0< t< 1/2
                                  砂（t) = < 1 for 1/ 2 < t < 1                                侮37)
                                         10      。therwise.
Their satisfying the multiresolution equation (2.13) is illustrated in Figure 2.2. Haar showed that
translates and scalings of these functions form an orthonormal basis for L2 (R.). We can easily
see that the Haar functions are also a compact support orthonormal wavelet system that satisfy
Daubechies ' conditions. Although they are as regular as can be achieved for N = 2, they are not.
even continuous. The orthogonality and nesting of spanned subspaces are easily seen because the
translates have no overlap in the time domain. It is instructive to apply the various properties
of Sections 5 and 5.8 to these functions and see how they are satisfied. They are illustrated
                                                                                                 in
the example in Figures 2.11 through 2.15.

듸nc Way이ets
The next best known (perhaps the best known) basis set is that formed by the sine functions.
The sinc functions are usually presented in the context of the Shannon sampling theorem, but
                                                                                                we
can look at translates of the sine function as an orthonormal set of basis functions (or, in some
cases, a tight frame). They, likewise, usually form a orthonormal wavelet system satisfying
                                                                                               the
various required conditions of a multiresolution system.
    The sinc function is defined as

                                        sinc(t) = 씌끄                                                      侮38)
where sinc(0) = 1. This is a very versatile and useful function because its Fourier transform is a
simple rectangle function and the Fourier transform of a rectangle function is a sinc function. In
order to be a scaling function, the sinc must satisfy (2.13) as

                              sinc(Kt) = Z如 Si띠砒卜 枷）                                                      伍39)

for the appropriate scaling coefficients h(n) and some K. If we construct the scaling function
from the generalized sampling function as presented in (4.35), the sinc function becomes


                         sinc(Kt) = ＞二sinc(KTn) sinc（台t수미·                                            侮40)
Sec. 5.7. Example Scaling Functions and Wavelets
                                                                                                          61


In order for these two equations to be true, the sampling period must be T = 1/2 and
                                                                                     the
parameter
                                                                 冗互
                                                   K=
                                                                                                       (5.41)

which gives the scaling coefficients as


                                           fltfl) = sinc（크豆fl).                                        (5.42)

We see that 甲(t) = sinc(Kt) is a scaling function with infinite support and its correspondi
                                                                                                 ng
scaling coefficients are samples of a sinc function. It R = 1, then K = ir and the scaling function
generates an orthogonal wavelet system. For R > 1, the wavelet system is a tight frame, the
expansion set is not orthogonal or a basis, and R is the amount of redundancy in the system as
discussed in Chapter 5.
    For the orthogonal sinc scaling function, the wavelet is simply expressed by

                                         砂(t) = 2 p(2t) - 99(t).                                       (5.43)

    The sinc scaling function and wavelet do not have compact support, but they do illustrate an
infinitely differentiable set of functions that result from an infinitely long h(n). The orthogonali
                                                                                                     ty
and multiresolution characteristics of the orthogonal sinc basis is best seen in the
                                                                                             frequency
domnain where there is no overlap of the spectra. Indeed, the Haar and sinc systems are Fourier
duals of each other. The sinc generating scaling function and wavelet are shown in Figure 5.1.


                                              Sinc Sc톄ing Funct幻n




           0.5



                                                                      \/   '   \／八＼
                                                                                  ／八／        \/   -




         -0.5
           -40        -30        日＝20      斗10              0         10         20     30        40

                                                        텨nc Wavelet
               1
                                                             人
          0.5


               0


         -0.5


                1
               -40    -30        -20
           叫
                                           -10              0         10        20      30        40


                         Figure 5.1. Sinc Scaling Function and Wavelet
62                                              The Scaling and Wavelet Functions and Coefficients   Ch. 5


Spline and Battle-Lemari6 Wavelet Systems
The triangle scaling function illustrated in Figure 2.2 is a special case of a more general family of
SPhne
spline SCahng
        scaling fU1lCtiOllS·
                functions. The scaling
                                SCah叩 COe胤蜘t
                                       coefficient SyStelll /t(72) =i i昏 -1 , 1 O} gives rise to the
                                                   system h(n)
piecewise linear, continuous triangle scaling function. This function is a first-order spline, being
a concatenation of two first order polynomials to be continuous at the junctions or "knots".
A quadratic spline is generated from h = {1/4, 3/4, 3/4, 1/4}/\/易 as three sections of second
order polynomials connected to give continuous first order derivatives at the junctions. The
cubic spline is generated from h(n) = {1/16.1/4, 3/8, 1/4, 1/16} /V三 This is generalized to an
arbitrary Nth order spline with continuous (N - 1)th order derivatives and with compact support
of N+1. These functions have excellent mathematical properties, but they are not orthogonal over
integer translation. If orthogonalized, their support becomes infinite (but rapidly decaying) and
they generate the "Battle-Lemari6 wavelet system" [Dau92, SN96, Chu92a, Chu92b]. Figure 5.2
illustrates the first-order spline scaling function which is the triangle function along with the
second-, third-, and fourth-order spline scaling functions.

               1
                                                    0.7

              0.8                                   0.6

                                                    0.5
              0.6
                                                    0.4

              0.4                                   0.3

                                                    0.2
              0.2
                                                    0.1

               0                                     0
                0       0.5      1        1.5   2      0    0.5   1       1.5       2   2.5   3

                     (a) 中si 1st order spline               (b) 中s2 2nd order spline
                                                    0.6-
              0.6
                                                    0.5-
              0.5
                                                    0.4-
              0.4
                                                    0.3-
              0.3
                                                    0.2-
              0.2

              0.1                                   0.1 뇨

               0
                0       1        2        3     4             1       2         3       4     5

                    （이 中S3 3rd order spline                 (d) 中s4 4th order spline

                                Figure 5.2. Spline Scaling Functions




5.8    Further Properties of the Scaling Function and Wavelet

The scaling function and wavelet have some remarkable properties that should be examined in
order to understand wavelet analysis and to gain some intuition for these systems. Likewise, the
scaling and wavelet coefficients have important properties that should be considered.
Sec. 5.8. Further Properties of the Scaling Function and Wavelet                                                              63


   We now look further at the properties of the scaling function and the wavelet in terms of
the basic defining equations and restrictions. We also consider the relationship of the scaling
function and wavelet to the equation coefficients. A multiplicity or rank of two is used here but
the more general multiplicity-M case is easily derived from these (See Section 7.2 and Appendix
B). Derivations or proofs for some of these properties are included in Appendix B.
   The basic recursive equation for the scaling function, defined in (5.1) as

                                              甲(t) =Z h(n) V p(2t - n),                                                    (5.44)
is homogeneous, so its solution is unique only within a normalization factor. In most cases, both
the scaling function and wavelet are normalized to unit energy or unit norm. In the properties
discussed here, we normalize the energy as E = f Iy7(t)I2 dt = 1. Other normalizations can easily
be used if desired.

General Properties not Requiring Orthogonality
There are several properties that are simply a result of the multiresolution equation (5.44) and,
therefore, hold for orthogonal and biorthogonal systems.

Property 1 The normalization of a(t) is arbitrary and is given in (5.13) as E. Here we usually
set E = 1 so 坑毗 坑e basis functions are or才／wnor刃1毗 t工I工d coe月icien招 C（玎1easi匈 be calculated
with inner products.

                                                       ／如       （태'           毗＝             E=            1               (5.45)

Property 2 N야 on自／ 口Zn 仇e sc毗航g funct加n be w仇材en as a weig九ted sum of functions in 仇e
next ／工ig九er scale 斗）ace 口S st毗ed in 坑e bas秀c recursion equ（工tion (5．了刃， 加虎 it can also be exp7毛ssed
in higher resolution spaces:

                                     甲(t) = ＞二 h(j)(n) 2j/2甲(2t - n)                                                       (5.46)


？刃／工ere 九（1)（미 = h（미 口nd for j 2 1

                                    /1 "+l)
                                      (   '     (r工）        =   ＞二九（j)
                                                                    k
                                                                                   （丸）            九（' ")   (n-   2k)   .
                                                                                                                           (5.47)


Property 3 A formula for the sum of dyadic samples of 9)(t)


                                                            Z甲（多）= 2"
                                                                丸
                                                                                                                           (5.48)


Property 4 A '加rti加n of unity " 加lb螂 和on工 (5.48) for J = 0

                                                                ＞二甲     (m)              =        1                        (5.49)


Property 5 A ger工e7끄lized p（工r才ition of unity e娩就s if 甲(t) 可s continuous

                                                            Z印 -m) = 1                                                     (5.50)
                                                                                                                                The Scaling and Wavelet Functions and Coefficients                                                         Ch. 5


Property 6 A 和eq2工ency domain 討atement o/ 坑e 比師c recurs切n eqi工（it勿n 佰．杯)


                                                                                                                                                                                                                                          (5.51)
                                                    .（
                                                               『）
                                                                                      ＝
                                                                                                               弓흐丑
                                                                                                                                                   （w/
                                                                                                                                                                       2)
                                                                                                                                                                                 .         (w/
                                                                                                                                                                                                            2)
Property 7 Successive approximations in the frequency domain is often easier to analyze than
the time domain version in (5.44). The convergence properties of this infinite product
                                                                                       are very
impo?才（工nt.


                                       .(.)：立｛늉副.（이                                                                                                                                                                                      侮52)


This formula is derived in (5.74).

Properties that Depend on Orthogonality
The following properties depend on the orthogonality of the scaling and wavelet functions.

Property 8 The square of the integral of 甲(t) is equal to the integral of the square of Y (t), or
A긍 = E.
                                                         lr                                                               12                                           .

                                                         [/             甲
                                                                                      (t)
                                                                                                                     dtj                      =              J              甲    (t)
                                                                                                                                                                                                 2 dt
                                                                                                                                                                                                                                         侮53)

Property 9 The 可ntegr毗 0/ 坑e wavelet 秀s necess（工I吼！/ zero


                                                                                            ／砂
                                                                                                                          （t）                 毗＝
                                                                                                                                                                            .                                                            (5.54)

T九e fbi꾸no/ 坑e 凹口velet is usu口／ly norm毗初ed 切 one s2工c九 坑at f 1砂（t)I2dt= 1.

Property 10 Not only are integer translates of the wavelet orthogonal; different scales are also
or坑四onm.

                     f 砂(2"
                          2'/2
w／工ere 坑e no？斗no／砂（t) is one.
                                       t        -         k)
                                                                        2
                                                                                 "/
                                                                                             2            砂(2              "t
                                                                                                                                              -
                                                                                                                                                   『) dt:                                        d    (k,
                                                                                                                                                                                                                  /)   5
                                                                                                                                                                                                                           (j   -
                                                                                                                                                                                                                                    ,)
                                                                                                                                                                                                                                         (5.55)



Property 11 The scaling function and wavelet are orthogonal over both scale and translation.



                                 f 砂(2
                                  2'
                                       "
                                           「2
                                                                        "t
                                                                             '
                                                                                                 -                   k)
                                                                                                                           2
                                                                                                                                "
                                                                                                                                         '2
                                                                                                                                                         『
                                                                                                                                                             (2
                                                                                                                                                                            "t
                                                                                                                                                                                       -
                                                                                                                                                                                                 / ) dt= 0
                                                                                                                                                                                                                                         (5.56)

加r all integer 自3小／ where j 드 2.

Property 12 A frequency domain statement of the orthogonality requirements in (5.13) . It also
is a statement of equivalent energy measures in the time and frequency domains as in Parseval's
仇eore刃2, W／工ic九 is tr꼬ze w可th （工n or坑四onal b口5招 set.


                     ＞二陣（w+ 2卄小
                      k
                                                                    '        =
                                                                                                     ..
                                                                                                          ／陣
                                                                                                                           （ 1'     『）
                                                                                                                                                                  如＝
                                                                                                                                                                                                  /
                                                                                                                                                                                                                 （테' dt             1    (5.57)
 Sec. 5.9. Parameterization of the Scaling Coefficients                                                          65

 Property 13 The scaling coe毋Icien拓 C（工n be c口lci工／ated from 坑e or坑四onal or tig砒加me sc毗ing
 functions by


                                             姻＝
                                                            v/
                                                             小
                                                                      （t)
                                                                            (2t    -       n)
                                                                                                     dt.   (5.
                                                                                                                 58)
 Property 14 The wavelet coe肌cients C（工n be calc?工latedfron上 坑e or坑四毗（zl or tig砒／r口I砒 scaling
 functions by

                                                                                                           (5.59)
                                        hi
                                                  (n)
                                                        =
                                                            V프   f砂
                                                                      (t)『   (2t
                                                                                       -        n)
                                                                                                     dt.

    Derivations of some of these properties can be found in Appendix B. Properties in equations
(5.1), (5.10), (5.14), (5.53), (5.51), (5.52), and (5.57) are independent of any normalizatio
                                                                                              n ofY7(t).
Normalization affects the others. Those in equations (5.1), (5.10), (5.48), (5.49), (5.51), (5.52),
and (5.57) do not require orthogonality of integer translates of 甲(t). Those in (5.14), (5.16), (5.17),
(5.22), (5.20), (5.53), (5.58) require orthogonality. No properties require compact
                                                                                      support. Many
of the derivations interchange order of summations or of summation and integration. Conditions
for those interchanges must be met.


5.9     Parameterization of the Scaling Coefficients

The case where 甲(t) and h(n) have compact support is very important. It aids in the time local-
ization properties of the DWT and often reduces the computational requirements of calculating
the DWT. If h(n) has compact support, then the filters described in Chapter 3 are
                                                                                         simple FIR
filters. We have stated that N, the length of the sequence h(n), must be even and
                                                                                          h(n) must
satisfy the linear constraint of (5.10) and the 퓽 bilinear constraints of (5.14). This leaves
                                                                                              퓽- 1
degrees of freedom in choosing h(n) that will still guarantee the existence of 甲(t) and a set of
essentially orthogonal basis functions generated from 99(t).


Length그 Scaling Coefficient Vector
For a length-2 h(n), there are no degrees of freedom left after satisfying the required conditions
in (5.10) and (5.14). These requirements are

                                                        九（0) + 九（1) = \／互

and
                                                        h2(0) +h2(1) = 1

which are uniquely satisfied by



                                  枷2 = 的力（1)} = 俵出｝                                                        侮62)

These are the Haar scaling functions coefficients which are also the length-2 Daubechies coeffi-
cients [Dau92] used as an example in Chapter 2 and discussed later in this book.
66                                                                      The Scaling and Wavelet Functions and Coefficients                          Ch. 5


Length-4 Scaling Coefficient Vector
For the length-4 coefficient sequence, there is one degree of freedom or one parameter that gives
all the coefficients that satisfy the required conditions:

                                  h(0) + h(1) + h(2) + h(3) = \／云                                                                                  (5.63)

                                  h2(O) + h2(1) + h2(2) + h2(3) = 1                                                                                (5.64)
and
                                           h(0) h(2) + h(l) h(3) = 0                                                                               (5.65)
     Letting the parameter be the angle a, the coefficients become

                              h(0) =                   (1卜 cos(ct) + sin(a))/(2\ ')
                              h(1) =                   (1 + cos(a) + sin(a))/(2v牙)
                                                                                                                                                   侮66)
                              h(2) =                   (1 + cos(a) - sin(a))/(2v'죵)
                              h(3) =                   (1 - cos(이 - sin(a))/(2\ /)).

These equations also give the length-2 Haar coefficients (5.62) for a = 0, 7r/2, 3ir/2 and a degen-
erate condition for a = ir. We get the Daubechies coefficients (discussed later in this book) for
a = ir/3. These Daubechies-4 coefficients have a particularly clean form,

                          .           Ii+              V／죵     3+ \／죵                       3_ \/g 1_ /引
                          """ n4'/易 ' 4'/牙 ' 缸／牙 ' 4'/ 了
                                                                                                                                                   侮67)


Length-6 Scaling Coefficient Vector
For a length-6 coefficient sequence h(n), the two parameters are defined as a and /3 and the
resulting coefficients are

        h(0) =   [(1 + cos(a) + sin(a))(1 - cos(13) - sin(/3)) + 2sin(/3) cos(a)1/(4v' )
        h(1) =   [(1 - cos(a) + sin(a))(1 + cos(乃) - sin(3)) - 2sin(/3) cos(a)]/(4v' )
        九（2) =   [1+ cos(（上H／了）+sin(a -/3)]/(2\／죵）
                                                                                                                                                   侮68)
        h(3) =   [1 + cos(a小 i3) - sin(a中 i3)]/(2v'죵)
        h(4) =   l/ \／百 - h(0) 小 h(2)
        h(5) =   1/ v'牙 - h(1) - h(3)

Here the Haar coefficients are generated for any a = 3 and the length-4 coefficients (5.66) result if
/3 = 0 with a being the free parameter. The length-4 Daubechies coefficients are calculated for a =
ir/3 and 3 = 0. The length-6 Daubechies coefficients result from a = 1.35980373244182 and /3 =
-0.78210638474440.
    The inverse of these formulas which will give a and /3 from the allowed h(n) are


                    （上 = arctan   /
                                  \2 (h(1) h(2) - h(0) h(3)) + V2(h(0) - h(1)) J
                                       2   2＋ 九
                                           （   九   （) 1+
                                                       0   )    （＋ 九 )//牙
                                                                    1   )   2       -                     （   九   （란               （   3   )
                                                                                                                                               \   伍69)



                              /3 = a 小 arctan                   /\h(2) +h(3) -1/ V2J
                                                                                九 n     （   2   )   』-九           （    3   )   』
                                                                                                                                                   (5.70)
Sec. 5.10. Calculating the Basic Scaling Function and Wavelet                                    67

As a and 目 range over -ir to 7r all possible h(n) are generated. This allows informative experi-
mentation to better see what these compactly supported wavelets look like. This parameteriza-
tion is implemented in the MATLAB programs in Appendix C and in the Aware, Inc. software,
UltraWave [The89].
    Since the scaling functions and wavelets are used with integer translations, the location of
their support is not important, only the size of the support. Some authors shift h(n), hi(n), 甲(t),
and 砂 (t) to be approximately centered around the origin. This is achieved by having the initial
nonzero scaling coefficient start at n = -퓽 + 1 rather than zero. We prefer to have the origin at
n ＝二 t = 0.
    MATLAB programs that calculate h(n) for N = 2, 4, 6 are furnished in Appendix C. They
calculate h(n) from a and 3 according to (5.62), (5.66), and (5.68). They also work backwards
to calculate a and /3 from allowable h(n) using (5.70). A program is also included that calculates
the Daubechies coefficients for any length using the spectral factorization techniques in [Dau92]
and Chapter 6 of this book.
    Longer h(미 sequences are more difficult to parameterize but can be done with the tec뇨iques
of Pollen [Polarl and Wells [Wel931 or the lattice factorization by Viadyanathan [Vai92]
                                                                                             devel-
oped in Chapter 8. Selesnick derived explicit formulas for N = 8 using the symbolic software
system, Maple, and set up the formulation for longer lengths [Sel97}. It is over the space of these
independent par缸1leters that one can find optimal wavelets for a particular problem or class of
signals [Dau92, GOB94].


5.10     Calculating the Basic Scaling Function and Wavelet
Although one never explicitly uses the scaling function or wavelet (one uses the scaling and
wavelet coefficients) in most practical applications, it is enlightening to consider methods to
calculate 甲(t) and 叭t). There are two approaches that we will discuss. The first is a form of
successive approximations that is used theoretically to prove existence and uniqueness of 甲(t)
and can also be used to actually calculate them. This can be done in the time domain to find
99(t) or in the frequency domain to find the Fourier transform of 甲(t) which is denoted 호(w). The
second method solves for the exact values of y7(t) on the integers by solving a set of simultaneous
equations. From these values, it is possible to then exactly calculate values at the half integers,
then at the quarter integers and so on, giving values of 甲(t) on what are called the dyadic
rationals.

Successive Approximations or the Cascade Algorithm
In order to solve the basic recursion equation (5.1), we propose an iterative algorithm that will
generate successive approximations to (t). If the algorithm converges to a 琡ed point, then that
fixed point is a solution to (5.1). The iterations are defined by

                                                  N- i

                                 甲(k+i)(t) = ＞二九（n) '/ 甲（丸）(2t小n)                             (5.71)
                                                  n=o

for the kth iteration where an initial97(0) (t) must be given. Because this can be viewed
                                                                                          as applying
the same operation over and over to the output of the previous application, it is sometimes
                                                                                               called
the cascade algorithm.
68                                               The Scaling and Wavelet Functions and Coefficients    Ch. 5


     Using definitions (5.2) and (5.3), the frequency domain form becomes


                                令 (k+1)（미 =
                                               加固.""（計                                                侮72)


and the limit can be written as an infinite product in the form



                             鉀）(w)＝回訶釘］鉀如）.                                                           侮73)


If this limit exists, the Fourier transform of the scaling function is



                                 『）=[TiJ知（붊）
                                .（         小（.）·                                                      (5.74)



The limit does not depend on the shape of the initial 甲(0) (t), but only on 令（') (0) = f c,(k) (t) dt =
A0, which is invariant over the iterations. This only makes sense if the limit of 4 (w) is well-defined
as when it is continuous at w ;= 0.
    The MATLAB program in Appendix C implements the algorithm in (5.71) which converges
reliably to 97(t), even when it is very discontinuous. From this scaling function, the wavelet can
be generated from (2.24). It is interesting to try this algorithm, plotting the function at each
iteration, on both admissible h(n) that satisfy (5.10) and (5.14) and on inadmissible h(n). The
calculation of a scaling function for N = 4 is shown at each iteration in Figure 5.3.
    Because of the iterative form of this algorithm, applying the same process over and over, it is
sometimes called the cascade algorithm [SN96, Str96a].


Iterating the Filter Bank
An interesting method for calculating the scaling function also uses an iterative procedure which
consists of the stages of the filter structure of Chapter 3 which calculates wavelet expansions co-
efficients (DWT values) at one scale from those at another. A scaling function, wavelet expansion
of a scaling function itself would be a single nonzero coefficient at the scale of j = 1. Passing this
single coefficient through the synthesis filter structure of Figure 3.7 and equation (3.20) would
result in a fine scale output that for large j would essentially be samples of the scaling function.


Successive approximations in the frequency domain
The Fourier transform of the scaling function defined in (5.2) is an important tool for studying
and developing wavelet theory. It could be approximately calculated by taking the DFT of the
samples of p(t) but a more direct approach is available using the infinite product in (5.74). From
this formulation we can see how the zeros of H佃) determine the zeros of I (口.,). The existence
conditions in Theorem 5 require H (미 = 0 or, more generally, H (w) = 0 for w = (2k + 1)兀.
Equation (5.74) gives the relation of these zeros of H (w) to the zeros of 호 (w). For the index
k= 1, 且佃仁) = 0 at 口7= 2(2丸 + 1）兀 For 丸 = 2, H (w/4) = 0 at w = 4(2丸 + 1）兀 且佃爬) =0
                                                                                                                    69
Sec. 5.10. Calculating the Basic Scaling Function and Wavelet


                 1.5                                            1.5




                 0.5                                            0.5




                ...0.5o      0.5               2   2.5     3   10·5b      0.5     I       1.5    2       2.5
                                    I   1.5

                    （미 中D4(t) Success加e Approx. 1                 (b) 中D4(t) Successive Approx. 2
                 1.5                                            1.5




                  0.5                                           0.5



                                                                  0



                _0.5o                               2.5    3    0.50       0.5    1       1.5    2       2.5    3
                              0.5        1.5

                          c) 中D4(t) Successive Approx. 3              (d) 中D4 (t) Successive Approx. 4
                                                                1.5




                                                                 0.5




                 m5C1         0.5        1.5   2    2.5    3    -0帖 ＝ 늉小小＝ 小i三1三1可弓

                     (e) 中D4(t) Successive Approx. 5                  (f) 中D4(t) Successive Approx. 6
                  1.5                                            1.5




                   0.5                                           0.5



                                                                      0



                   0.
                     5亡10. 弓
                                                                 0.5o       0.5       1    1.5       2    2.5

                        (g) 砂D4(t) Successive Approx. 7                (h) 中D4(t) Successive Approx. 8

                     Figure 5.3. Iterations of the Successive Approximations for 甲D4




 at w = 8(2k + 1)兀 etc. Because (5.74) is a product of stretched versions of H (w), these zeros of
 H (w/ 2J) are the zeros of the Fourier transform of p(t). Recall from Theorem 15 that H (w) has
 no zeros in -ir/ 3 <w < ir/3. All of this gives a picture of the shape of 令 (w) and the location of
 its zeros. 까om an asymptotic analysis of t (w) as w - 以, one can study the smoothness of y7(t).
 70                                                                      The Scaling and Wavelet Functions and Coefficients       Ch. 5


    A MATLAB program that calculates 重(w) using this frequency domain successive approxima-
tions approach suggested by (5.74) is given in Appendix C. Studying this program gives further
insight into the structure of 令 (w). Rather than starting the calculations given in (5.74) for the
index j = 1, they are started for the largest j = J and worked backwards. If we calculate a
length-N DFT consistent with j = J using the FFT, then the samples of H (w/2i) for j = J - 1
are simply every other sample of the case for j = J. The next stage for j = J -2 is done likewise
and if the original N is chosen a power of two, the process in continued down to j = 1 without
calculating any more FFTs. This results in a very efficient algorithm. The details are in the
program itself.
    This algorithm is so efficient, using it plus an inverse FFT might be a good way to calculate
甲(t) itself. Examples of the algorithm are illustrated in Figure 5.4 where the transform is plotted
for each step of the iteration.




                                                                            0.5


                                                                                                                /     』＼\
                                                                               0o
                                                                                                           /
                                                                                               2       3        4

               (a)
              1.5
                     t
                         D4   (睾) I   Successive
                                                         Approx. 1             (b) 1中D4（睾） Successive Approx. 2
                                                                            1.5




               1




              0.5                                                           0.5




               06             2                    4      6          8       a占                                10           15

              （이 1令D4（睾）1Succe田ive Ap마ox. 3                                  (d)
                                                                                   4D畔)   I   Successive
                                                                                                                    Approx. 4
               Figure 5.4. Iterations of the Successive Approximations for 令 (w)



The Dyadic Expansion of the Scaling Function
The next method for evaluating the scaling function uses a completely different approach.
                                                                                                It
starts by calculating the values of the scaling function at integer values of t, which can be done
exactly (within our ability to solve simultaneous linear equations). Consider the basic recursion
equation (5.1) for integer values of t = k

                                                       甲困 = Z坰 V西마 - ),                                                          侮75)
                                                              n

and assume h（미 ；芒 0 如r0< n 드 N- i.
Sec. 5.10. Calculating the Basic Scaling Function and Wavelet                                         71


    This is the refinement matrix illustrated in (5.6) for N = 6 which we write in matrix form as

                                                    入4ocp = 甲．                                    (5.76)

In other words, the vector of c'(k) is the eigenvector of M0 for an eigenvalue of unity. The simple
sum of 乞n h(n) = \／牙 in (5.10) does not guarantee that M0 always has such an eigenvalue, but
乙 h(2n) = 兄 h(2n + 1) in (5.12) does guarantee a unity eigenvalue. This means that if (5.12)
is not satisfied, 甲(t) is not defined on the dyadic rationals and is, therefore, probably not a very
nice signal.
    Our problem is to now find that eigenvector. Note from (5.6) that 甲(0) = 奴N - 1) = 0 or
h(0) = h(N小 1) = 1/ v'牙. For the Har wavelet system, the second is true but for longer systems,
this would mean all the other h(n) would have to be zero because of (5.10) and that is not only
not interesting, it produces a very poorly behaved 甲(t). Therefore, the scaling function with
N > 2 and compact support will always be zero on the extremes of the support. This means that
we can look for the eigenvector of the smaller 4 by 4 matrix obtained by eliminating the first and
last rows and columns of M0.
    From (5.76) we form [M0 - I]으 = 0 which shows that [M0 - 기 is singular, meaning its rows are
not independent. We remove the last row and assume the remaining rows are now independent.
If that is not true, we remove another row. We next replace that row with a row of ones in order
to implement the normalizing equation


                                              ＞二 o(k) = 1                                         (5.77)
                                                k

This augmented matrix, [M0 - Il with a row replaced by a row of ones, when multiplied by
gives a vector of all zeros except for a one in the position of the replaced row. This equation
should not be singular and is solved for 甲 which gives (k), the scaling function evaluated at the
integers.
    From these values of Y)(t) on the integers, we can find the values at the half integers using the
recursive equation (5.1) or a modified form                                                     n

                                      小／2) = 三h(n) v加(k- n)                                       (5.78)


    This is illustrated with the matrix equation (5.8) as

                                                    M1甲 = 'P2                                     (5.79)

Here, the first and last columns and last row are not needed (because 9,o = 甲5 = 'P11/2 = 0) and
can be eliminated to save some arithmetic.
    The procedure described here can be repeated to find a matrix that when multiplied by a
vector of the scaling function evaluated at the odd integers divided by k will give the values at
the odd integers divided by 2k. This modified matrix corresponds to convolving the samples of
'P(t) by an up-sampled h(n). Again, convolution combined with up- and down-sampling is the
basis of wavelet calculations. It is also the basis of digital filter bank theory. Figure 5.5 illustrates
the dyadic expansion calculation of a Daubechies scaling function for N = 4 at each iteration of
this method.
72                                                           The Scaling and Wavelet Functions and Coefficients   Ch. 5


                                                                  1.5




                                                                  0.5


                                                                   0


                                                                 H0'5b   0.5         1.5    2     2.5    3

                      (a) 中i)4(t) eva!. at integers                  (b) 中D4(t) eva!. at half integers
              1                                                   1.5




              0.5                                                 0.5




             小0.50       0.5   1     1.5    2    2.5     3        0帖H＝三         I + + 1.5 小喜中 2늉

              (c) 砂D4 (t) eva!. at quarter integers                (d) 中D4(t) eva!. at eighth integers
                                                                  1.5




                                                                  0.5


                                                                    0


                                                                 _0.5o   0.5         1.5    2     2.5

                  (e) 中D4(t) eva!. at 16th integers                 (f) 中D4(t) eva!. at 32th integers
                                                                  15




                                                                  0.5




             -0.5占＝弓                                             -0.5占H二늉       1    1三1盲中 2 可m三

                    (g) 中D4 (t) eva!. at 64th integers              (h) 中D4(t) eva!. at 128th integers


                        Figure 5.5. Iterations of the Dyadic Expansion for 砂D4



    Not only does this dyadic expansion give an explicit method for finding the exact values of
 '(t) of the dyadic rationals (t = k/ 27), but it shows how the eigenvalues of M say something
about the 甲(t). Clearly, if Y7(t) is continuous, it says everything.
    MATLAB programs are included in Appendix C to implement the successive approximation
and dyadic expansion approaches to evaluating the scaling function from the scaling coefficients.
They were used to generate the figures in this section. It is very illuminating to experiment with
different h(n) and observe the effects on 97 (t) and 砂 (t).
Chapter 6


      Regularity, Moments, and Wavelet
                        System Design


We now look at a particular way to use the remaining 퓽 - 1 degrees of freedom to design the N
values of h(n) after satis如ing (5.10) and (5.14), which insure the existence and orthogonality (or
property of being a tight frame) of the scaling function and wavelets [Dau92, Dau90, Dau93].
    One of the interesting characteristics of the scaling functions and wavelets is that while sat-
isfying (5.10) and (5.14) will guarantee the existence of an integrable scaling function, it may be
extraordinarily irregular, even fractal in nature. This may be an advantage in analyzing rough
or fractal signals but it is likely to be a disadvantage for most signals and images.
    We will see in this section that the number of vanishingmoments of hi(n) and 砂(t) are related
to the smoothness or differentiability of y7(t) and 叭t). Unfortunately, smoothness is difficult to
determine directly because, unlike with differential equations, the defining recursion equation
(5.1) does not involve derivatives.
    We also see that the representation and approximation of polynomials are related to the
number of vanishing or minimized wavelet moments. Since polynomials are often a good model
for certain signals and images, this property is both interesting and important.
    The number of zero scaling function moments is related to the "goodness" of the approxima-
tion of high-resolution scaling coefficients by samples of the signal. They also affect the symmetry
and concentration of the scaling function and wavelets.
    This section will consider the basic 2-band or multiplier-2 case defined in (2.13). The more
general M-band or multiplier-M case is discussed in Section 7.2.


6.1    K-Regular Scaling Filters

Here we start by defining a ui毗ary sea渤刃洸er 切 be an F江R filter with coefficien招 h(미 from the
basic recursive equation (5.1) satisfying the admissibility conditions from (5.10) and orthogonality
conditions from (5.14) as


                       ＞二九（n) =V互 a1ld Z싸川硏2m) =如l).                                           (6.1)
                         n                       k


The term "scaling filter" comes from Mallat 's algorithm, and the relation to filter banks discussed
in Chapter 3. The term "unitary" comes from the orthogonality conditions expressed in filter
bank language, which is explained in Chapter 8.
                                                                                                  73
74                                                                               Regularity, Moments, and Wavelet System Design   Ch. 6



    A unitary scaling filter is said to be K-regular if its z-transform has K zeros at z = e' 兀. This


                                                                    ( 三 ) Q（기
looks like                                             1 \ j(

                                     丑
                                         （/
                                              )=
                                                                        " ：            '
                                                                                                                                  (6.2)

where H (z) = Z, h(n) zm is the z-transform of the scaling coefficients h(n) and Q(z) has no
poles or zeros at z = et . Note that we are presenting a definition of regularity of h(n), not of
the scaling function 甲(t) or wavelet 叭t). They are related but not the same. Note also from
(5.20) that any unitary scaling filter is at least K = 1 regular.
    The length of the scaling filter is N which means H (z) is an N- i degree polynomial. Since the
multiple zero at z = -1 is order K, the polynomial Q (z) is degree N- i- K. The existence of 甲(t)
requires the zeroth moment be \／巨 which is the result of the linear condition in (6.1). Satisfying
the conditions for orthogonality requires N/2 conditions which are the quadratic equations in
(6.1). This means the degree of regularity is limited by

                                              1 < K < 프．
                                                      2         -                  H
                                                                                                                                  (6.3)

Daubechies used the degrees of freedom to obtain maximum regularity for a given N, or to obtain
the minimum N for a given regularity. Others have allowed a smaller regularity and used the
resulting extra degrees of freedom for other design purposes.
    Regularity is defined in terms of zeros of the transfer function or frequency response function
                                                                                                    the
of an FIR filter made up from the scaling coefficients. This is related to the fact that
differentiability of a function is tied to how f戚 its Fourier series coefficients drop off as the index
goes to infinity or how fast the Fourier transform magnitude drops off as frequency goes to infinity.
The relation of the Fourier transform of the scaling function to the frequency response of the
FIR filter with coefficients h(n) is given by the infinite product (5.74). From these connections,
we reason that since H (z) is lowpass and, if it has a high order zero at z = -1 (i.e., w = ir), the
Fourier transform of 甲(t) should drop off rapidly and, therefore, 甲(t) should be smooth. This
 turns out to be true.
     We next define the kth moments of Y)(t) and 砂 (t) as

                                              rn    (k)
                                                                        =   /     tk
                                                                                           (t)
                                                                                                 dt                                (6.
                                                                                                                                           4)
 and
                                              mi          (k)
                                                                        =
                                                                            /!
                                                                                       ' 砂（t）毗                                     (6.5)

 and the discrete 丸t九 moments of ／工（미 and h1（미 as

                                                   /1（丸） = ＞二71k h（미                                                               (6.6)


 and
                                              尸，(k) = ＞二nk 九l(n).                                                                   (6.7)


 The partial moments of h(n) (moments of samples) are defined as

                                 「（瓦Z) = ＞二（2n+ Z)k 九（2ri +Z）·                                                                           (6.8)
                                                                    n


 Note that /2(k) = v(k, 0) + zi(k, 1).
Sec. 6.2. Vanishing Wavelet Moments                                                                            75


   From these equations and the basic recursion equation (5.1) we obtain [GB92b]


                            m   (k)   =       1
                                          (；쓰- I) v2 ;;; \ t J
                                          . ,   ,   .   .I n 二寸           (k   )   肛   （Z)   m   (kH   Z)
                                                                                                             (6.9)


which can be derived by substituting (5.1) into (6.4), changing variables, and using (6.6). Simi-
larly, we obtain
                                                                      .




                                m1（小 古仁 ( 二 ) ILi&) m(k -Z）·
                                                                  k
                                                                                                            (6.10)
                                                            t= 1J


    These equations exactly calculate the moments defined by the integrals in (6.4) and (6.5) with
simple finite convolutions of the discrete moments with the lower order continuous moments. A
similar equation also holds for the multiplier-M case described in Section 7.2 [GB92bJ. A Matlab
program that calculates the continuous moments from the discrete moments using (6.9) and
(6.10) is given in Appendix C.


6.2    Vanishing Wavelet Moments

Requiring the moments of 砂 (t) to be zero has several interesting consequences. The follow-
ing three theorem1ls show a variety of equivalent characteristics for the K-regular scaling filter,
which relate both to our desire for smooth scaling functions and wavelets as well as polynomial
representation.

Theorem 20 (Equivalent Characterizations of K-Regular Filters) A unitary scaling flu-
ter is K-regular if and only if the following equivalent statements are tr工e:

   1. All moments of the wavelet filters are zero, /11(k) = 0, for k = 0, 1, · 4 . , (K 卞 1)

   2. All moments of the wavelets are zero, mi(k) = 0, for k = 0, 1, . · . , (K 小 1)

   3. The partial moments of the scaling filter are equal for k = 0, 1, · · . , (K - 1)

   4. The frequency response of the scaling filter has a zero of order K at w = ir, i.e. (6.2).

   5. The kth derivative of the magnitude-squared frequency response of the scaling filter is zero
      atw= ofork= 1, 2, . . · ,2K- 1.

   6. All polynomial sequences up to degree (K - 1) can be expressed as a linear combination of
      shifted scaling filters.

   7. All polynomials of degree up to (K - 1) can be expressed as a linear combination of shifted
      scaling f?工nctions at 口T四 sca把

This is a very powerful result [SHGB93, Hel95]. It not only ties the number of zero moments to
the regularity but also to the degree of polynomials that can be exactly represented by a sum of
weighted and shifted scaling functions.
76                                                           Regularity, Moments, and Wavelet System Design    Ch. 6


Theorem 21 IfVJ(t) is K-times differentiable and decays fast enough, then the first K- i wavelet
moments vanish /Dau92J; i.e.,
                                               砂
                                              竺耐  1
                                                  L
                                                      < 凹，        0드 丸드K                                      (6끄）

iTT叩／ies
                                              mi(k) = 0.         0< k< K                                      (6.12)



Unfortunately, the converse of this theorem is not true. However, we can relate the differentiability
of 砂 (t) to vanishing moments by

Theorem 22 There exists a finite positive integer L such that if mi(k) = 0 for 0 5 k 드 K - 1
坑en
                                                   dJ>     . .
                                                   규戶叩） < 以）                                                  (6.13)

for L 尸 > K.

For example, a three-times differentiable /(t) must have three vanishing moments, but three
vanishing moments results in only one-time differentiability.


    These theorems show the close relationship among the moments of hi(n), 砂 (t), the smoothness
of H (w) at LU = 0 and it and to polynomial representation. It also states a loose relationship with
the smoothness of o(t) and 砂(t) themselves.


6.3    Daubechies' Method for Zero Wavelet Moment Design
Daubechies used the above relationships to show the following important result which constructs
orthonormal wavelets with compact support with the maximum number of vanishing moments.

Theorem 23 The discrete-time Fourier transform of h(n) having K zeros at w = it of the form
                                                             .     K
                                          月（『）=( ' 二"."）노（미                                                   (6.14)
                                                         1+ e


satisfies
                                          田回尸 + 因佃 + 쩨2 =2                                                    (6.15)
if and only if L(w) = .C(w) 尸 can be written

                                               ／』（回） = 尸（sin2（뇨2/ 2))                                         (6.16)

with K < N/2 where
                                 /(       l

                         /())=（니'「）, "『 )" 요二，)
                                      十




                                 k 二＝0


and R(y) is an odd po勾／nomial chosen so th毗 尸（끼 三 0 for 0 드 !/ 드 1.
 Sec. 6.3. Daubechies' Method for Zero Wavelet Moment Design
                                                                                                                      77

If 1? = 0, the length N is minimum for a given regularity K = N/2. If N> 2 K, the second term
containing R has terms with higher powers of y whose coefficients can be used for purposes other
than regularity.
    The proof and a discussion are found in Daubechies [Dau88a, Dau92J. Recall from (5.20) that
H (w) always has at least one zero at w = ir as a result of h(n) satisfying the necessary conditions
for 甲(t) to exist and have orthogonal integer translates. We are now placing restrictions on
h(ri) to have as high an order zero at w = 冗 as possible. That accounts for the form of (6.14).
Requiring orthogonality in (5.22) gives (6.15).
    Because the frequency domain requirements in (6.15) are in terms of the square of the mag-
nitudes of the frequency response, spectral factorization is used to determine H (w) and therefore
h(ri) from H (w)已 Equation (6.14) becomes

                                                                1 i- e t           2
                                               田(w) j2      =
                                                            -    ..
                                                                          r   2"       1   C
                                                                                               (w)
                                                                                                     I2.        (6.
                                                                                                                      18)

    If we use the functional notation:

                                         M (w) = 因回尸 and L(w) = 1C(q끼2                                          (6.19)
then (6.18) becomes
                                                M (w) = Icos2(w/2)IKL(미.                                       (6.20)
Since M (w) and L(w) are even functions of w they can be written as polynomials in
==n:=n m. n n n / .\   1    fl 小 :=n '2 1. ./n\ n=
                                                                                                           cos(미 and,
                                                   m 1: n 느1 /i그 fl n\ L n n n +1
u:>iiig （工J:5＼나／7 =    1-   ; bill      呼／/ 二J} e（꾸1t1L山1l L1J·乙（J) Ut久;ullles



                                     M (sin2(w/ 2)) = 1 cO52(w/2)小 P(sin2 (w/2))                               (6.21)
which, after a change of variables of y = 5in2(w/2) = 1 - cOs가w/2), becomes

                                                     苾m= (1 _ 功Kp(y)                                           (6.22)
where P(y) is an (N -- K) order polynomial which must be positive since it will have to be
factored to find H (w) from (6.19). This now gives (6.14) in terms of new variables which are
easier to use.
    In order that this description supports an orthonormal wavelet basis, we now require that
(6.22) satisfies (5.22)
                                   1H (w)I2 + I丑（回＋7r）尸 = 2                            (6.23)
which using (6.19) and (6.22) becomes

                            凡1(w) + M (w + 미 = (1 中 끼I口如）+ 9幻m H V) = 2.                                       (6.24)
   Equations of this form have an explicit solution found by using Bezout's theorem. The details
are developed by Daubechies [Dau92}. If all the (N/ 2 - 1) degrees of freedom are used to set
wavelet moments to zero, we set K = N/2 and the solution to (6.24) is given
                                                                               by
                                                         K- i         /       r/   1 , i

                                             P(y) =）二.. U＝十" ) V'
                                                                                               \

                                                                                                               (6.25)
                                                          k=0
                                                                   Regularity, Moments, and Wavelet System Design    Ch. 6
78


which gives a complete parameterization of Daubechies' maximum zero wavelet moment design.
                                                                                           these
It 毗5o gives a very straightforward procedure for the calculation of the h(n) that satisfy
conditions. Herrmann derived this   expression for the design of Butterworth  or maximally   fiat
FIR digital filters [Her71J.
   If the regularity is K < N/2, P(y) must be of higher degree and the form of the solution is




                                      드(                                                      l e
                                                                                                O乙
                                      K小 l       /    中r   '   .     \
                                                 +                                U
                                                                                      K   R          V
                                             中
                                                                                                                    (6.26)
                        P
                            (y)
                                  ＝
                                                     仄＝
                                                               "         )9
                                                                              "
                                      k=O                            '




where R(y) is chosen to give the desired filter length N, to achieve some other desired property,
and to give P(y) 2 0.
    The steps in calculating the actual values of h(n) are to first choose the length N (or the
desired regularity) for h(n), then factor IH(w) 12 where there will be freedom in choosing which
roots to use for H (w). The calculations are more easily carried out using the z-transform form
of the transfer function and using convolution in the time domain rather than multiplication
(raising to a power) in! the frequency domain. That is done in the MATLAB program Din,hini
                                                                                                the
= daub (N) in Appendix C where the polynomial coefficients in (6.25) are calculated from
binomial coefficient formula. This polynomial is    factored with the roots  command   in MATLAB
and the roots are mapped from the polynomial variable yZ to the variable z1 in (6.2) using first
cos(U) = 1- 2Ye, then with is呵미 = v/cos가w) - 1 and &' = cos佃냐 is呵미 we use z = e브
 These changes of variables are used by Herrmann [ller7ll and Daubechies [Dau92].
    Examine the MATLAB program to see the details of just how this is carried out. The program
uses the sort command to order the roots of H (z) H (1/z) after which it chooses the N - 1
                                                                                             set of
 smallest ones to give a minimum phase H (z) factorization. You could choose a different
 N - 1 roots in an effort to get a more linear phase    or even maximum   phase. This choice allows
 some variation in Daubechies wavelets of the same length. The M-band generalization of this is
 developed by Heller in [SHGB93, Hel95]. In [Dau92], Daubechies also considers an alternation
 of zeros inside and outside the unit circle which gives a more symmetric h(n). A completely
 symmetric real h(n) that has compact support and supports orthogonal wavelets is not possible;
 however, symmletry is possible for complex h(n), biorthogonal systems, infinitely long h(n), and
 multiwavelets. Use of this zero moment design approach will also assure the resulting wavelets
 system is an orthonormal basis.
     If all the degrees of freedom are used to set moments to zero, one uses K = N/2 in (6.14)
 and the above procedure is followed. It is possible to explicitly set a particular pair of zeros
 somewhere other than at w = 兀. In that case, one would use K = (N/2) - 2 in (6.14). Other
 constraints are developed later in this chapter and in later chapters.
     To illustrate some of the characteristics of a Daubechies wavelet system, Table 6.1 shows the
  scaling 血nction and wavelet coefficients, h(n) and h1(n), and the corresponding discrete scaling
  coefficient moments and wavelet coefficient moments for a length-8 Daubechies system. Note the
 N/2 = 4 zero moments of the wavelet coefficients and the zeroth scaling coefficient moment of
  尸（0) = \／三
Sec. 6.3. Daubechies ' Method for Zero Wavelet Moment Design
                                                                                                 79



Table 6.1. Scaling         뇨nction and Wavelet Coefficients plus their Discrete Moments for
Dat小echie乎8
           n                   M미                     hi(n)         /1（川         ／工1（川       丸
           0     0.23037781330890       0.01059740178507        1.414213             0       0
           1     0.71484657055292       0.03288301166689        1.421840             0       1
           2     0.63088076792986      -0.03084138183556        1.429509             0       2
           3    -0.02798376941686      -0.18703481171909        0.359097             0       3
           4    -0.18703481171909       0.02798376941686       -2.890773     12.549900       4
           5     0.03084138183556       0.63088076792986       -3.453586    267.067254       5
           6     0.03288301166689      -0.71484657055292       23.909120   3585.681937       6
           7    -0.01059740178507       0.23037781330890



    Table 6.2 gives the same information for the length-6, 4, and 2 Daubechies scaling coefficients,
wavelet coefficients, scaling coefficient moments, and wavelet coefficient moments. Again notice
how many discrete wavelet moments are zero.
    Table 6.3 shows the continuous moments of the scaling function 甲(t) and wavelet 砂(t) for the
Daubechies systems with lengths six and four. The discrete moments are the moments of the
coefficients defined by (6.6) and (6.7) with the continuous moments defined by (6.4) and (6.5)
calculated using (6.9) and (6.10) with the programs listed in Appendix C.



    Table 6.2. Daiibechies Scaling Function and Wavelet Coefficients plus their Moments
              Daubechies N = 6
           Ii              h（미                      hi(n)           p（丸）        pi(k)    丸
            0  0.33267055295008         -0.03522629188571       1.414213            0    0
           1   0.80689150931109         -0.08544127388203       1.155979            0    1
           2   0.45987750211849          0.13501102001025       0.944899            0    2
           3 -0.13501102001025           0.45987750211849      -0.224341     3.354101    3
           4 -0.08544127388203          -0.80689150931109      -2.627495    40.679682    4
           5   0.03522629188571          0.33267055295008       5.305591   329.323717    5
              Daubechies N ＝二 4
           n               h(n)                    hi(n)           尸（劤         /JK川      k
           0  0.48296291314453          0.12940952255126        1.414213           0     0
           1 0.83651630373781           0.22414386804201        0.896575           0     1
           2  0.22414386804201         -0.83651630373781        0.568406    1.224744     2
           3 -0.12940952255126          0.48296291314453       -0.864390    6.572012     3
              Daubechies N = 2
           n                   h（미                    M（川          n（劤         ILl（肋     丸
           0    0.70710678118655        0.70710678118655       1.414213            0     0
           1    0.70710678118655       -0.70710678118655       0.707107     0.707107     1
80                                                 Regularity, Moments, and Wavelet System Design   Ch. 6



     Table 6.3. Daubechies Scaling Function and Wavelet Continuous and Discrete Moments
                             N= 6
                    丸          川劤             /1K시           m(k)           7rM劤
                    0     1.4142135              0      1.0000000              0
                    1     1.1559780              0      0.8174012              0
                    2     0.9448992              0      0.6681447              0
                    3    -0.2243420      3.3541019      0.4454669      0.2964635
                    4    -2.6274948     40.6796819      0.1172263      2.2824642
                    5     5.3055914    329.3237168     -0.0466511     11.4461157
                             N= 4
                    丸          月（丸）          P1仕）            m（劤            m1（劤
                    0     1.4142136              0      1.0000000               0
                    1     0.8965755              0      0.6343975               0
                    2     0.5684061      1.2247449      0.4019238       0.2165063
                    3    -0.8643899      6.5720121      0.1310915       0.7867785
                    4    -6.0593531     25.9598790     -0.3021933       2.0143421
                    5   -23,4373939     90.8156100     -1.0658728       4.4442798




     These tables are very informative about the characteristics of wavelet systems in general as
well as particularities of the Daubechies system. We see the 尸(0) = 扼 of (6.1) and (5.10) that
is necessary for the existence of a scaling function solution to (5.1) and the P1(0) = mi(0) = 0 of
(5.32) and (5.29) that is necessary for the orthogonality of the basis functions. Orthoriormality
requires (2.25) which is seen in comparison of the h(n) and hi(n), and it requires rn(0) = 1
from (5.53) and (5.45). After those conditions are satisfied, there are N/2 - 1 de앉ees of freedom
left which Daubechies uses to set wavelet moments mi(k) equal zero. For length-6 we have two
zero wavelet moments and for length-4, one. For all longer Daubechies systems we have exactly
N/ 2 - 1 zero wavelet moments in addition to the one rni (0) = 0 for a tolal of N/2 zero waelet
moments. Note m(2) = m(1)2 as will be explained in (6.32) and there exist relationships among
some of the values of the even-ordered scaling function moments, which will be explained in (6.52)
 through (6.55).
     As stated earlier, these systems have a maximum number of zero moments of the wavelets
 which results in a high degree of smoothness for the scaling and wavelet functions. Figures 6.1
 and 6.2 show the Daubechies scaling functions and wavelets for N = 4, 6, 8, 10, 12, 16, 20, 40.
 The coefficients were generated by the techniques described in Section 5.9 and Chapter 6. The
 MATLAB programs are listed in Appendix C and values of h(n) can be found in [Dau92] or
 generated by the programs. Note the increasing smoothness as N is increased. For N = 2, the
 scaling function is not continuous; for N = 4, it is continuous but not differentiable; for N = 6, it
 is barely differentiable once; for N = 14, it is twice differentiable, and similarly for longer h(n).
 One can obtain any degree of differentiability for sufficiently long h(n).
     The Daubechies coefficients are obtained by maximizing the number of moments that are
 zero. This gives regular scaling functions and wavelets, but it is possible to use the degrees of
Sec. 6.3. Daubechies' Method for Zero Wavelet Moment Design                                                                   81


                                                                 1.2
                                                                            1
                                                                 0.8
                                                                 0.6
                                                                 0.4
                                                                 0.2
                                                                            0
                                                                -.0.2
                                                                -0.4
                                                                    0                         2            3         4

                                      (a) 砂D4                                                (b) 砂D6




                     0.8
                                                                 0.
                                                                 。8
                     0.6
                                                                       .6       '




                     0.4                                         0,
                     0.2                                         。4    .2
                       0                                                    0

               -0.2                                             -0.2

                                                                _0.4o                             4

                                      （이 中DS                                                 (d) 中D10



                     0.8

                     0.6 '
                                                                  0.5
                     0.4『

                     0.2 ,

                       0

               -0.2

               -0.4
                                       4          8        10   _0.50                                          10        15
                        0

                                      (e) 砂D12

                                                                      0.8 ,

                                                                      0.6

                     0.5                                              0.4




                                                                                        肛
                                                                  0.2 '

                                                                            0       ·




                       5。
                                            10        15                    0           10            20            30
               -0.
                                      (g) 砂D20                                               (h) 中D40



                             Figure 6.1. Daubechies Scaling Functions, N = 4, 6,8, . . . ,40




freedom to maximize the differentiability of 甲(t) rather than maximize the zero moments. This
is not easily parameterized, and it gives only slightly greater smoothness than the Daubechies
system [Dau92].
82                                                                        Regularity, Moments, and Wavelet System Design   Ch. 6




                     0.5              1.5           2        2.5

                               ( ) 砂D4                                                     (b) 砂D6




             0.5




                           2      3             4       5        6                    2        4            6

                               （이 砂D8                                                      (d) 砂D10



             0.5




                                            6           8            10                    5            10           Is

                                                                                           (f) 砂D16
                                                                            0.8

                                                                            0.6
             0.5 느
                                                                            0.4




                                                                                          可
                                                                            0.2



                                                                           -0.2
                                                                                                        介
                                                                           -0.4

                                                                           -0 6
                                                                           -0.8
                           5           10                   15                 0      10           20           30

                               (g) 砂D20                                                    (h) 砂D40

                     Figure 6.2. Daubechies Wavelets, N = 4, 6, 8, . . . ,40




   Examples of Daubechies scaling functions resulting from choosing different factors in the
spectral factorization of IH(w)I2 in (6.18) can be found in [Dau92].
Sec. 6.4. Non-Maximal Regularity Wavelet Design                                                    83


6.4    Non-Maximal Regularity Wavelet Design

If the length of the scaling coefficient filter is longer than twice the desired regularity, i.e., N >
2 K. then the parameterization of (6.26) should be used and the coefficients in the polynomial
R(y) must be determined. One interesting possibility is that of designing a system that has one
or more zeros of H (w) between w = ir/ 2 and w = 冗 with the remaining zeros at ir to contribute
to the regularity. This will give better frequency separation in the filter bank in exchange for
reduced regularity and lower degree polynomial representation.
    If a zero of H (w) is set at w = w0, then the conditions of

                                                        d M (w)
                                 M (wo) = 0       and              =0                          (6.27)
                                                          dw 口)=wo

are imposed with those in (6.26), giving a set of linear simultaneous equations that can be solved
to find the scaling coefficients h(n).
    A powerful design system based on a Remez exchange algorithm allows the design of an
orthogonal wavelet system that has a specified regularity and an optimal Chebyshev behavior in
the stopband of H (w). This and a variation that uses a constrained least square criterion [SLB97]
is described in [LSOB94] and another Chebyshev design in [RD941.
    An alternative approach is to design the wavelet system by setting an optimization criterion
and using a general constrained optimization routine, such as that in the MATLAB optimization
toolbox, to design the h(n) with the existence and orthogonality conditions as constraints. This
approach was used to generate many of the filters described in Table 6.7. Jun Tian used a
Newton's method [Tia96, TW95] to design wavelet systems with zero moments.



6.5    Relation of Zero Wavelet Moments to Smoothness
We see from Theorems 21 and 22 that there is a relationship between zero wavelet moments and
smoothness, but it is not tight. Although in practical application the degree of differentiability
may not be the most important measure, it is an important theoretical question that should be
addressed before application questions can be properly posed.
    First we must define smoothness. From the mathematical point of view, smoothness is essen-
tially the same as differentiability and there are at least two ways to pose that measure. The first
is local (the Holder measure) and the second is global (the Sobolev measure). Numerical alg아
rithrns for estimating the measures in the wavelet setting have been developed by Rioul [Rio92]
and Heller and Wells [I1W94, HW96a] for the HOlder and Sobolev measures respectively.


Definition 1 (Holder continuity) Let p : IR 나 C and let 0 < a < 1. Then the function p is
HOlder continuous of order a if there exists a constant c such that

                             油（끼 H 미玔 5 이T H 3／尸           /or 毗／乞！/ E 표｛                      (6.28)
84                                                            Regularity, Moments, and Wavelet System Design      Ch. 6


Based on the above definition, one observes Y) has to be a constant if a > 1. Hence, this is not
very useful for determining regularity of order a> 1. However, using the above definition, Holder
regularity of any order r > 0 is defined as follows:

Definition 2 (Holder regularity) A function 甲 : 正t -* C is regular of order r = P + a
(0 <a < 1) if 甲 e C ' and its Pth derivative is Holder continuous of order a

Definition 3 (Sobolev regularity) Let Y7 : 正t -* C, then 99 is said to belong to the Sobolev
space of order s (7 e HS) if
                                                                               2
                                                              量（回） dw ＜二 以）                                      (6.29)
                                    JR       늬山
                                              "


    Notice that, although Sobolev regularity does not give the explicit order of differentiability,
it does yield lower and upper bounds on r, the Holder regularity, and hence the differentiability
of 甲 if 99 e L2. This can be seen from the following inclusions:

                                             H+ 112 c CT C HS                                                    (6.30)

   A very interesting and important result by Volkmer [Vol92] and by Eirola [Eir92] gives an
exact asymptotic formula for the H0lder regularity index (exponent) of the Daubechies scaling
function.

Theorem 24 The limit of the HOlder regularity index of a Daubechies scaling function as the


                                         쀼
length of the scaling filter goes to infinity is [Vol92]


                                                                               j
                                                                  (3)
                            lim          =
                                              [1-
                                                        log
                                                                              )1   =                             (6.31)
                                                        2 l。                                 2075.
                                              [i
                                                    -                                  (0.
                           N- .以）                                       (2)                          .   .   )
                                                              g
This result, which was also proven by A. Cohen and J. P. Conze, together with empirical calcula-
tions for shorter lengths, gives a good picture of the smoothness of Daubechies scaling functions.
This is illustrated in Figure 6.3 where the Holder index is plotted versus scaling filter length for
both the maximally smooth case and the Daubechies case.
    The question of the behavior of maximally smooth scaling functions was empirically addressed
by Lang and Heller in [L1196]. They use an algorithm by Rioul to calculate the H0lder smoothness
of scaling functions that have been designed to have maximum Holder smoothness and the results
are shown in Figure 6.3 together with the smoothness of the Daubechies scaling functions as
functions of the length of the scaling filter. For the longer lengths, it is possible to design
systems that give a scaling function over twice as smooth as with a Daubechies design. In most
applications, however, the greater H0lder smoothness is probably not important.
    Figure 6.4 shows the number of zero moments (zeros at w = ir) as a function of the number
of scaling function coefficients for both the maximally smooth and Daubechies designs.
    One case from this figure is for N = 26 where the Daubechies smoothness is SH = 4.005 and
the maximum smoothness is SH = 5.06. The maximally smooth scaling function has one more
continuous derivative than the Daubechies scaling function.
    Recent work by Heller and Wells [HW94, HW96a] gives a better connection of properties of
the scaling coefficients and the smoothness of the scaling function and wavelets. This is done
both for the scale factor or multiplicity of M = 2 and for general integer M.
 Sec. 6.5. Reiation of Zero Wav&et Moments to Smoothness
                                                                                        85


                                 S
                                                                             口




                                 5




                                 4




                                2
                                                무




                                        古




                                0o          5   10     15         20   25   30
                                                     Len口th




Figure 6.3. Holder Smoothness versus Coefficient Length for Daubechies ' (+) and Maximally
Smooth (o) Wavelets.



                                16




                                10




                     ＝茹8自七名툐뷴




                                                +    0        0




                                0
                                    0       5   10     15         20   25   30
                                                     Length




Figure 6.4. Number of Zeros at w = ir versus Coefficient Length for Daubechies' (+) and
Maximally Smooth (o) Wavelets.
86                                                           Regularity, Moments, and Wavelet System Design    Ch. 6

    The usual definition of smoothness in terms of differentiability may not be the best measure
for certain signal processing applications. If the signal is given as a sequence of numbers, not as a
function of a continuous variable, what does smoothness mean? Perhaps the use of the variation
of a signal may be a useful alternative [GB95c, OB96b, Ode961.


6.6    Vanishing Scaling Function Moments

While the moments of the wavelets give information about flatness of H (w) and smoothness of
砂(t), the moments of Y)(t) and h(미 are measures of the "localization" and symmetry character-
istics of the scaling function and, therefore, the wavelet transform. We know from (5.10) that
已h (n) = \／易 and, after normalization, that f (t) dt = 1. Using (6.9), one can show [GB92b]
that for K 2 2, we have
                                          m(2) = m2(1).                                 (6.32)
This can be seen in Table 6.3. A generalization of this result has been developed by Johnson
[JMNK96] and is given in (6.52) through (6.55).
    A more general picture of the effects of zero moments can be seen by next considering two
approximations. Indeed, this analysis gives a very important insight into the effects of zero
moments. The mixture of zero scaling function moments with other specifications is addressed
later in Section 6.9.


6.7    Approximation of Signals by Scaling Function Projection

The orthogonal projection of a signal 1 (t) on the scaling function subspace V3 is given and denoted
by
                              戶｛f (t)} = ＞二（f(t),甲3，丸（t))甲2，丸（t)                               (6.33)
                                              k
which gives the component of f (t) which is in V3 and which is the best least squares approximation
to f (t) in V3.
    As given in (6.5), the Zth moment of 砂 (t) is defined as

                                                                                                              (6.34)
                                       m1   (e)   =
                                                      ftt砂        (t) dt.
We can now state an important relation of the projection (6.33) as an approximation to f (t) in
terms of the number of zero wavelet moments and the scale.
Theorem 25 Ifm1(e) =0for Z= 0, 1,. . . ,L then the L2 error is

                              El=1I f (t) - P3{ f (t)} 112 < (72mj(L+l),                                      (6.35)

where C is a constant independent of j and L but dependent on 1 (t) and the wavelet system
/GLRT90, Uns96].
This states that at any given scale, the projection of the signal on the subspace at that scale
approaches the function itself as the number of zero wavelet moments (and the length of the
scaling filter) goes to infinity. It also states that for any given length, the projection goes to the
function as the scale goes to infinity. These approximations converge exponentially fast. This
projection is illustrated in Figure 6.5.
Sec. 6.8. Approximation of Scaling Coefficients by Samples of the Signal                    87


6.8     Approximation of Scaling Coefficients by Samples of the Signal

A second approximation involves using the samples of f (t) as the inner product coefficients in
the wavelet expansion of f (t) in (6.33). We denote this sampling approximation by

                                    S" {f (t)} = ＞二2"j/2 f(k/23) (Pj,k(t)                (6.36)
                                                           k

and the scaling function moment by

                                                                                         (6.37)
                                                  (
                                                      『)
                                                           =
                                                               fttco
                                                                       (t)
                                                                             dt
                                              m
and can state [Tia96] the following

Theorem 26 If m(Z) = 0 for Z = 1, 2, . . . , L then the L2 error is

                              E2=11 S3{f (t)} - P2{f (t)} 12 드 c2 2- j(L+1),             (6.38)

where C2 is a constant independent of j and L but dependent on 1 (t) and the wavelet system.

This is a similar approximation or convergence result to the previous theorem but relates the
projection of f (t) on a j-scale subspace to the sampling approximation in that same subspace.
These approximations are illustrated in Figure 6.5.




                Figure 6.5. Approximation and Projection of 1 (t) at a Finite Scale

   This "vector space" illustration shows the nature and relationships of the two types of ap-
proximations. The use of samples as inner products is an approximation within the expansion
 88                                                                     Regularity, Moments, and Wavelet System Design          Ch. 6


subspace V3. The use of a finite expansion to represent a signal f (t) is an approximat
                                                                                             ion from
L2 onto the subspace V3. Theorems 25 and 26 show the nature of those approximations, which,
for wavelets, is very good.
    An illustration of the effects of these approximations on a signal is shown in Figure 6.6 where a
signal with a very smooth component (a sinusoid) and a discontinuous component (a square wave)
is expanded in a wavelet series using samples as the high resolution scaling function coefficients.
Notice the effects of projecting onto lower and lower resolution scales.
    If we consider a wavelet system where the same number of scaling function and wavelet
moments are set zero and this number is as large as possible, then the following is true [WZ94,
Tia961:

Theorem 27 If m(Z) = mi (s) = 0 for Z = 1, 2, . . . , L and mi(O) = 0, then the L2 error is

                                      E3=11 f (t) -Sj{ f (t)} Ii2드 C32-j (L+1 ,                                                (6.39)
where C3 is a constant independent of j and L, bnt dependent on f (t) and the wavelet system.

Here we see that for this wavelet system called a Coifman wavelet system, that using samples as
the inner product expansion coefficients is an excellent approximation. This justifies that using
samples of a signal as input to a filter bank gives a proper wavelet analysis. This approximation
is also illustrated in Figure 6.5 and in [WB97].


6.9    Coiflets and Related Wavelet Systems
From the previous approximation theorems, we see that a combination of zero wavelet and zero
scaling function moments used with samples of the signal may give superior results to wavelets
with only zero wavelet moments. Not only does forcing zero scaling function moments give a
better approximation of the expansion coefficients by samples, it causes the scaling function
to be more symmetric. Indeed, that characteristic may be more important than the sample
approximation in certain applications.
   Daubechies considered the design of these wavelets which were suggested by Coifman [Dau92,
Dau93, BCR91]. Copinath [Gop90, GB92bJ and Wells [WZ94, TW95J show how zero scaling
function moments give a better approximation of high-resolution scaling coefficients by samples.
Tian and Wells [Tia96, TW95] have also designed biorthogonal systems with mixed zero
                                                                                       moments
with very interesting properties.
   The Coifman wavelet system (Daubechies named the basis functions "coiflets") is an orthonor-
mal multiresolution wavelet system with


                      f      t'   『
                                      (t)
                                            dt =   m
                                                       (k)
                                                              =   0,
                                                                        for   k= 1, 2, . · . ,L- 1                       (6.40)



                      f (t)
                         t
                             '砂
                                dt = mi     =            k=
                                                        (k)
                                                                   0,
                                                                        for
                                                                                   1,
                                                                                        2,
                                                                                             .
                                                                                               41)
This definition imposes the requirement that there be at least L -1 zero scaling function moments
                                                                                                 .   .   ,L
                                                                                                              -
                                                                                                                  1.
                                                                                                                         (6.
and at least L - 1 wavelet moments in addition to the one zero moment of rn1(0)
                                                                                       required by
orthogonality. This system is said to be of order or degree L and sometime has the additional
requirement that the length of the scaling function filter h(n), which is denoted N, is minimum
[Dau92, Dau93].
Sec. 6.9. Coiflets and Related Wavelet Systems                                                              89


                                                                                  Approximation in
                            Test Function


         0.5                                                    0.5

               0                                                         0

        -0.5                                              -0.5

                                                                尸        1

                           2          4          6                            0     2          4        6
                         Approximation in V5                                      Approximation in V4



         0.5                                                    0.5 ,

                   0                                                     0

        -0.5                                              -0.
                                                                         5了
                            2          4                                      0     2          4
                                                                    －녀
                          Approximation in V3                                     Approximation in V2



          0.5




        -0.5 1

                   1
                    0       2          4         6                                  2          4
           -
                          Approximation in V1                                     Approximation in V。
                   1

          0.5

                   0

         -0.5

                   1
                    0        2          4        6
               -
                        Figure 6.6. Approximations to f (t) at a Different Finite Scales
 90                                                                        Regularity, Moments, and Wavelet System Design                                     Ch. 6

    The length-4 wavelet system has only one degree of freedom, so it cannot have both a scaling
 function moment and wavelet moment of zero (see Table 6.6). Tian [Tia96, TW95] has derived
 formulas for four length-6 coifiets. These are:

                        ,      n3+ v' 卜V7   卜＼
                                        /11 ,
                                               /7 7+ .fl 5+ v' 卜V키
                                              ,1
                        Ti =   I    -   ／브． ,                                  ,         I-,-.   1            /1 1             -   P,- I 1                (6.42)
                               L 16/2            16v'2              8V2             8v'2                 16V2          16v'2 j
 or
                        ,      F - 3- v'7 i+ fl 7+ v'7 7- v7 5- v'7 i+ / 1
                        Ti =   1     ／민1     1         戶   1                   1                 ,            rr   1               Pr       ,           (6.43)
                               L 16v'2
                                                                      尸1                 尸-


                                                 16v'2              8V2            8v'2                  16V2
                                                                                                          -




                                                                                                                       16V2 j
                                                                                                                           -            I
or
               .         f - 3+ vi          i-    1T 3- v'ig 3+ JT 13+ /L 9- v'iigl
               11 = I           - - 戶   1     - P 1      Pr 1                         P              1     - P         ,               』mH I 1          (6.44)
                    L          lGv'2         16v'2             8v'2                8v'2                   16v'2                    16v'2 j
or

               h=
               "    =
                        [      16,/프    '    16 '%/프   '       8/
                                                                     죵     '       8v프
                                                                                                     '    l6V牙         '           16/ 프
                                                                                                                                                ]   '   (t.
                                                                                                                                                              4")

 with the first formula (6.42) giving the same result as Daubechies [Dau92, Dau93I (corrected) and
 that of Odegard [BO96] and the third giving the same result as Wickerhauser [Wic95}. The results
 from (6.42) are included in Table 6.4 along with the discrete moments of the scaling function
                                                                                                   and
 wavelet, /1(k) and pi(k) for k = 0, 1, 2, 3. The design of a length-6 Coifman system specifies
                                                                                                   one
 zero scaling function moment and one zero wavelet moment (in addition to pi(0) = 0), but we,
in fact, obtain one extra zero scaling function moment. That is the result of m(2) = m(1)2 from
 [GB92b1. In other words, we get one more zero scaling function moment than the two degrees
 of freedom would seem to indicate. This is true for all lengths N = 6Z for Z = l, 2, 3, . · . and
is a resu孔 of the interaction between the scaling function moments and the wavelet moments
described later.
     The property of zero wavelet moments is shift invariant, but the zero scaling function moments
缸e shift dependent [BCR91]. Therefore, a particular shift for the scaling function must be used.
This shift is two for the length-6 example in Table 6.4, but is different for the solutions in (6.44)
and (6.45). Compare this table to the corresponding one for Daubechies length-6 scaling 凡nctions
and wavelets given in Table 6.2 where there are two zero discrete wavelet moments - just as many
as the degrees of freedom in that design.
     The scaling function from (6.42) is fairly symmetric, but not around its center and the other
three designs in (6.43), (6.44), and (6.45) are not syrmnetric at all. The scaling 向nction from
(6.42) is also fairly smooth, and from (6.44) only slightly less so but the scaling function
                                                                                                 from
(6.43) is very rough and from (6.45) seems to be fractal. Examination of the freque
                                                                                         ncy response
H (w) and the zero location of the FIR filters h(n) shows very similar
                                                                              frequency responses for
(6.42) and (6.44) with (6.43) having a somewhat irregular but monotonic frequency
                                                                                        response and
(6.45) having a zero on the unit circle at q7 = 兀/3, i.e., not satisfying Cohen's condition [CS93]
for an orthognal basis. It is also worth noticing that the design in (6.42) has the largest Holder
smoothness. These four designs, all satisfying the same necessary conditions, have very different
characteristics. This tells us to be very careful in using zero moment methods to design wavelet
systems. The desi입ls are not unique and some are much better than others.
    Table 6.4 contains the scaling function and wavelet coefficients for the length-6 and 12 desi目ed
by Daubechies and length-8 designed by Tian together with their discrete moments. We see the
Sec. 6.9. Coiflets and R&ated Wavelet Systems                                                                                                                                 91


extra zero scaling function moments for lengths 6 and 12 and also the extra zero for lengths 8
and 12 that occurs after a nonzero one.
    The continuous moments can be calculated from the discrete moments and lower order con-
tinuous moments [BCR91, GB92b, SP93] using (6.9) and (6.10). An important relationship of
the discrete moments for a system with K中 1 zero wavelet moments is found by calculating
the derivatives of the magnitude squared of the discrete time Fourier transform of h(n) which is
H (w) = 兄 h(n) e t ' and has 2K 中 1 zero derivatives of the magnitude squared at w = 0. This
gives {GB92b] the kth derivative for k even and 1 <k < 2K - 1
                                           k

                                                  ( 二)
                                                  /   .    \




                                                                                                                                                                           (6.46)
                                       1=1
                                       Z                                 (-        1)
                                                                                                 'ii&                    )P           (k        -   Z)        =   0.
Solving for p(k) in terms of lower order discrete moments and using /2(0) = /2 gives for k even
                                                                丸-1                                     .


                               /2（向 = 寸仁 ( 二 ) (_1)t/2(t) /2（丸－Z)   t= l                     "                       "
                                                                                                                                                                           (6.47)

which allows calculating the even-order discrete scaling function moments in terms of the lower
odd-order discrete scaling function moments for k = 늑 4, ' · · ,2K - 2. For example:
                                                                                   1
                                                                                                                                                                           (6.48)
                                                                                                                             .



                                       /2
                                                      = 刀y' (1)
                                                                                                            n.
                                            (2)
                                                                               ]

                                       尸（4) = 命帥M斗却"(l)]                                                                                                                   (6.49)


which can be seen from values in Table 6.2.
    Johnson [JMNK96] noted from Beylkin [Bey92] and Unser [Uns96] that by using the moments
of the autocorrelation function of the scaling function, a relationship of the continuous scaling
function moments can be derived in the form

                                 $;(
                                 r=(J
                                                  二)           (_
                                                                              1)        ,-                       m
                                                                                                                         (       『)        m   (k        -   『) =      0   (6.50)

where 0 < k < 2K if K - 1 wavelet moments are zero. Solving for m(k) in terms of lower order
moments gives for k even
                                                          l
                                                      4 k- i                                 .

                               m(k) = !,y
                                      二 =
                                          . r\ ,丸 /) （小1)hi九（Z) rn（丸 -Z)
                                                                    =,                       (
                                                                                                                                                                           (6.51)
                                                          [ == 上



which allows calculating the even-order scaling function moments in terms of the lower odd-order
scaling function moments for k = 끽 4, · . · ,2K - 2. For example [JMNK96I:
                   m(2)    =    m2(1)                                                                                                                                      (6.52)
                   m(4)    =    4m(3) m(1) -3m4(1)                                                                                                                         (6.53)
                   m(6)    =    6rn(5) m(1) + 10m2(3) + 60m(3) m3(1) + 45m6(1)                                                                                             (6.54)
                   im(8)   =    8m(7) m(1) +56m(5) m(3) - 168m(5) m3(1)
                                +2520m(3) m5(1) -840rn(3) m2(1) - 1575m8(1)                                                                                                (6.55)
92                                                  Regularity, Moments, and Wavelet System Design   Ch. 6




     Table 6.4. Coifiet Scaling Function and Wavelet Coefficients plus their Discrete Moments
                      Length-N =6,         Degree L = 2
               n               M미                 /'i(fl)           /1（丸）            /11（川     丸
          -2
                   -0.07273261951285    0.01565572813546        1.414213                 0     0
          -    1    0.33789766245781   -0.07273261951285                0                0     1
               0    0.85257202021226   -0.38486484686420                0        -1.163722     2
               1    0.38486484686420    0.85257202021226       -0.375737         -3.866903     3
               2   -0.07273261951285   -0.33789766245781       -2.872795        -10.267374     4
               3   -0.01565572813546   -0.07273261951285
                       Length-N = 8,        Degree L = 3
               n                h(n)               hi(n)           p(k)             j.ti(k)    丸
          -4        0.04687500000000    0.01565572813546       1.414213                   0    0
          -3       -0.02116013576461   -0.07273261951285              0                   0    1
          -2
                   -0.14062500000000   -0.38486484686420              0                   0    2
          -    1    0.43848040729385    1.38486484686420      -2.994111          0.187868      3
               0    1.38486484686420   -0.43848040729385              0         11.976447      4
               1    0.38486484686420   -0.14062500000000     -45.851020        -43.972332      5
               2   -0.07273261951285    0.02116013576461      63.639610        271.348747      6
               3   -0.01565572813546    0.04687500000000
                      Length-N = 12,        Degree L = 4
               n                h(n)               hi(n)           p（丸）             m（劤        丸
          -4          0.016387336463      0.000720549446       1.414213                 0      0
          -3
                     -0.041464936781      0.001823208870              0                 0      1
          -2
                     -0.067372554722     -0.005611434819              0                 0      2
          -    1      0.386110066823     -0.023680171946              0                 0      3
               0      0.812723635449      0.059434418646              0          11.18525      4
               1      0.417005184423      0.076488599078      -5.911352         175.86964      5
               2     -0.076488599078     -0.417005184423              0        1795.33634      6
               3     -0.059434418646     -0.812723635449    -586.341304       15230.54650      7
               4      0.023680171946     -0.386110066823    3096.310009      117752.68833      8
               5      0.005611434819      0.067372554722
               6     -0.001823208870      0.041464936781
               7     -0.000720549446     -0.016387336463



if the wavelet moments are zero up to k = K - 1. Notice that setting m(1) = m(3) = 0 causes
m(2) = m(4) = in(6) = m(8) = 0 if sufficient wavelet moments are zero. This explains the extra
zero moments in Table 6.4. It also shows that the traditional specification of zero scaling function
moments is redundant. In Table 6.4 m(8) would be zero if more wavelet moments were zero.
     To see the continuous scaling function and wavelet moments for these systems, Table 6.5
shows both the continuous and discrete moments for the length-6 and 8 coifiet systems. Notice
the zero moment m(4) = 尸(4) = 0 for length-8. The length-14, 20, and 26 systems also have
the "extra" zero scaling moment just after the first nonzero moment. This always occurs for
length-N = 6Z + 2 coifiets.
Sec. 6.9. Coiflets and Related Wavelet Systems                                                  93


              Table 6.5. Discrete and Continuous Moments for the Coifiet Systems
                            N= 6,                L= 2
              丸              尸（向                 Ill（目            m(k)           rni(k)
              0      1.4142135623                    0    1.0000000000                0
              1                 0                    0               0                0
              2                 0        -1.1637219122               0   -0.2057189138
              3     -0.3757374752        -3.8669032118   -0.0379552166   -0.3417891854
              4     -2.8727952940       -10.2673737288   -0.1354248688   -0.4537580992
              5     -3.7573747525       -28.0624304008   -0.0857053279   -0.6103378310
                            N= 8,                L= 3
              丸                M川                L1（히            m（히            m1（川
              0      1.4142135623                    0    1.0000000000               0
              1                 0                    0               0               0
              2                 0                    0               0               0
              3     -2.9941117777         0.1878687376   -0.3024509630    0.0166054072
              4                 0        11.9764471108               0    0.5292891854
              5    -45.8510203537       -43.9723329775   -1.0458570134   -0.9716604635




   Figure 6.7 shows the length-6, 8, 10, and 12 coifiet scaling functions 甲(t) and wavelets (t).
Notice their approximate symmetry and compare this to Daubechies' classical wavelet systems
and her more symmetric ones achieved by using the different factorization mentioned in Sec-
tion 6.3 and shown in [Dau92]. The difference between these systems and truly symmetric ones
(which requires giving up orthogonality, realness, or finite support) is probably negligible in many
applications.




Generalized Coifman Wavelet Systems
The preceding section shows that Coifman systems do not necessarily have an equal number of
scaling function and wavelet moments equal to zero. Lengths N = 6Z + 2 have equal number
of zero scaling function and wavelet moments, but always have even-order "extra" zero scaling
function moments located after the first nonzero one. Lengths N = 6Z always have an "extra"
zero scaling function moment. Indeed, both will have several even-order "extra" zero moments for
longer N as a result of the relationships illustrated in (6.52) through (6.55). Lengths N = 6Z - 2
do not occur for the original definition of a Coifman If we generalize the investigation of the
Coifman system to consider systems with approximately equal numbers of zero scaling function
and wavelet moments, all lengths become possible and a larger class of coifiets are available.
    Consider the general Coifman Wavelet System to be the same as stated in (6.40) and (6.41)
but allow the number of zero scaling function and wavelet moments to differ by at most one
[BO96, BO971. That will include all the existing coifiets plus length-10, 16, 22, and N = & - 2.
The length-10 was designed by Odegard [BO96] by setting the number of zero scaling functions
to 3 and the number of zero wavelet moment to 2 rather than 2 and 2 for the length-8 or 3 and 3
94                                                          Regularity, Moments, and Wavelet System Design             Ch. 6




                                                                                                                   5

                            (a)       C6
              1.2 日

                1   戶




              0.8-

              0.6 느

              0.4

              0.2-

                0

             -0.2 戶
                 0                3        4   5   6                         2         3          4   5   6

                            （이 中C8                                               (d) 仇78
              1.2-


              0.8
              0.6




                                                                                  \r
              0.4-
              0.2-
                0
             -0.2-
                                                               -1    。
                 0                4                                      2             4                      8

                            (e) 叭끄0                                              (f) 仇7io
              1.2



              0.8-

              0.6-

              0.4-

              0.2-

                0

             寸0.2 니
                 0      2                              10      m10
                                                                                  4           6       8       10

                            (g) 仇12                                              (h)       'ci2


         Figure 6.7. Length-6, 8, 10, and 12 Coiflet Scaling 恥nctions and Wavelets




for the length-12 coifiets. The result in Table 6.6 shows that the length-b0 design again gives one
extra zero scaling function moment which is two more than the number of zero wavelet moments.
This is an even-order moment predicted by (6.53) and results in a total number of zero moments
between that for length-8 and length-12, as one would expect. A similar approach was used to
design length-16, 22, and 28.
                                                                                                   95
Sec. 6.9. Co出ets and Related Wavelet Systems



                                                    Wavelet Coefficients plus their Discrete
Table 6.6. Generalized Coiflet Scaling Function and
Moments
                Length-N = 4,        Degree L = 1
           n              h(n)               h1（미         IA（丸）       Ii'（劤 k
                                  0.129409522551      1.414213              0 0
           1   0.224143868042
                                                              0   -0.517  638  1
              寸
           0   0.836516303737     0.4829 62913 144
                                            30373 7   0.1894 68    0.1894  68  2
           1   0.482962913144 -0.836516
                                  0.224143868042     -0.776457     0.827225 3
            2 -0.129409522551
               Length-N = 10,        Degree L = 3
           n              h(미                M（미           尸（k)        ILl（劤 丸
                                  0.000233764788      1.414213              0 0
            2   0.032128481856
                                                              0             0  1
                  -
            1 -0.075539271956 -0.000549618934
                                                              0             0  2
                  -
            0 -0.096935064502 -0.013550370057
                                   0.033777338659             0    3.0315  70  3
            1   0.491549094027
                            557    0.3044 13564 385           0   24.674  674 4
             2  0.805141083
                                                                         0052 5
             3  0.304413564385 -0.805141083557 -14.709025 138.98
             4 -0.033777338659     0.491549094027    64.986095 710.373341 6
             5 -0.013550370057     0.096935064502
             6  0.000549618  934  -0.075 539271956
             7  0.000233764788      0.0321 28481856


                                                        N = 10, 16, 22, 28) by using the MATLAS
    We have designed these "new" coifiet systems (e.g.,
                                                     on. Wells and Tian [TW95] used Newton's
 optimization toolbox constrained optimization 血ncti
                                                  6t coifiets up to length 30 [BO96]. Selesnick
 method to design lengths N = & + 2 and N =
                                                          r approach is given by Wei and Bovik
 [SOB961 has used a filter design approach. Still anothe
  [WB96}.
                                                                     , using the one degree of freedom
      Table 6.6 also shows the result of designing a length-4 system
                                                           than one zero wavelet moment as we did
  to ask for one zero scaling function moment rather
                                                        not get any "extra" zero moments because
  for the Daubechies system. For length-4, we do
                                                        we see a direct trade-off between zero scaling
  there are not enough zero wavelet moments. Here
                                                        these new lengths to our traditional coifiets
  function moments and wavelet moments. Adding
  昏yes Table 6工
                                                                    number of zero wavelet moments,
       The fourth and sixth columns in Table 6.7 contain the
                                                                  onality in all of these systems. The
  excluding the mi(0) = 0 which is zero because of orthog
                                                           a nonzero moment for N = 6t + 2 are also
  extra zero scaling function moments that occur after
                                                         lized co沮ets for all even lengths. It shows
  excluded from the count. This table shows genera
                                                              ime achieved and how the total number
  the extra zero scaling function moments that are somet
                                                             "smoothness" as measured by the Holder
  of zero moments monotonically increases and how the
                                                      N and L.
  exponent [Rio93b, LH96, HW96a] increases with
       When both scaling functio  n  and  wavele t mome  nts are set to zero, a larger n그Lmber can be
                                                           s of freedom available. As stated earlier, of
  obtained than is expected from considering the degree
                                                          ients, h(n), one is used to insure e虹stence of
   the N degrees of freedom available from the N coeffic
                                                            used to insure orthonormality through the
   99(t) through the linear constraint (6.1), and N/ 2 are
                                                           s of freedom to achieve other characteristics.
   quadratic constraints (6.1). This leaves N/2 -1 degree
  96
                                                        Regularity, Moments, and Wavelet System Design
                                                                                                         Ch. 6


  Table 6.7. Moments for Various Length-N and Degre
                                                      e-L Generalized Coiflets, where (*) is the
  number of zero wavelet moments, excluding the
                                                mi(O) = 0
              N   L     m= 0 m1= O m = 0 m1 = 0 Total zero                Holder
                         set     set*    actual actual*     moments     exponent
              4    1      1        0        1        0         1          0.2075
              6    2      1        1        2       1          3          1.0137
              8   3        2       2        2        2         4          1.3887
             10   3       3        2        4        2         6          1.0909
             12   4       3       3         4       3          7          1.9294
             14   5       4       4        4        4          8         1.7353
             16   5       5       4        6        4         10         1.5558
             18   6       5       5        6        5         11         2.1859
             20   7       6       6        6        6         12         2.8531
             22   7       7       6        8        6         14         2.5190
             24   8       7       7        8        7         15         2.8300
             26   9       8       8        8        8         16         3.4404
             28   9       9       8       10        8         18         2.9734
             30 10       9        9       10        9         19         3.4083



  Daubechies used these to set the first N/2 - 1
                                                  wavelet moments to zero. From this approach, one
  would think that the coifiet system would allow (N/
                                                        2 - 1)/2 wavelet moments to be set zero and
  the same number of scaling function moments. For the
                                                             coifiets and generalized coifiets described
 in Table 6.7, one always obtains more than this.
                                                        The structure of this problem allows more
 zero moments to be both set and achieved than the
                                                        simple degrees of freedom would predict. In
 fact, the coifiets achieve approximately 2N/3 total zero
                                                              moments as compared with the number
 of degrees of freedom which is approximately N/2,
                                                          and which is achieved by the Daubechies
 wavelet system.
     As noted earlier and illustrated in Table 6.8, these genera
                                                                    lized coifiets fall into three classes.
 Those with scaling filter lengths of N = 61 + 2 (due
                                                         to Tian) have equal number of zero scaling
 function and wavelet moments, but always has "extra
                                                            " zero scaling function moments located
 after the first nonzero one. Lengths N = 61 (due
                                                        to Daubechies) always have one more zero
 scaling function moment than zero wavelet moment
                                                         and lengths N = 61中 2 (new) always have
two more zero scaling function moments than zero
                                                     wavelet moments. These "extra" zero moments
are predicted by (6.52) to (6.55) , and there will be
                                                      additional even-order zero moments for longer
lengths. We have observed that within each of
                                                      these classes, the HOlder exponent increases
monotonically.
     The lengths N = 61 - 2 were not found by earlier invest
                                                                  igators because they have the same
coiflet degree as the system that was just two shorte
                                                           r. However, they achieve two more zero
scaling function moments than the shorter length
                                                      system with the same degree.
     Table 6.7 is just the beginning of a large collection
                                                             of zero moment wavelet system designs
with a wide variety of trade-offs that would be tailore
                                                          d to a particular application. In addition
to the variety illustrated here, many (perhaps all) of
                                                          these sets of specified zero moments have
multiple solutions. This is certainly true for length-6 as
                                                             illustrated in (6.42) through (6.45) and
 Sec, 6.10    卜川n Im注at向n of rv化ments Rather than Zero 卜爪＞rr祀nts
                                                                                                97


Table 6.8. Number of Zero Moments for The Three Classes of Generalized Coifiets (Z = 1, 2, · · ·）,
*excluding 尸i(0) = 0, f excluding Non-Contiguous zeros
                              N            m= ot         ml= 0*       Totaizero
                           Length          achieved      achieved      moments
                          N = & +2        (N - 2)/3     (N - 2)/3    (2/3)(N - 2)
                           N = &             N/3        (N - 3)/3   (2/3)(N - 3/2)
                          N = 6Z -2       (N + 2)/3     (N - 4)/3    (2/3)(N - 1)



 for other lengths that we have found experimentally. The variety of solutions for each length can
have different shifts, different Holder exponents, and different degrees of being approximately
symmetric.
     The results of this chapter and section show the importance of moments to the characteristi万
of scaling functions and wavelets. It may not, however, be necessary or important to use the
exact criteria of Daubechies or Coifman, but understanding the effects of zero moments is very
important. It may be that setting a few scaling function moments and a few wavelets moments
may be sufficient with the remaining degrees of freedom used for some other optimization, either
in the frequency domain or in the time domain. As is noted in the next section, an alternative
might be to minimize a larger number of various moments rather than to zero a few [OB96aJ.
     Examples of the generalized Coiflet Systems are shown in Figure 6.7.


6.10         Minimization of Moments Rather than Zero Moments

Odegard has considered the case of minimization of a larger number of moments rather than
setting N/ 2 - 1 equal to zero [OB97, OB96b, OB96a]. This results in some improvement in
representing or approximating a larger class of signals at the expense of a better approximation
of a smaller class. Indeed, G6tze [GORB96I has shown that even in the designed zero moments
wavelet systems, the implementation of the system in finite precision arithmetic results in nonzero
moments and, in some cases, non-orthogonal systems.
Chapter 7


               Generalizations of the Basic
             Mu出res이U如n Wavelet System


Up to this point in the book, we have developed the basic two-band wavelet system in some detail,
                                                                                            develop
trying to provide insight and intuition into this new mathematical tool. We will now
a variety of interesting and valuable generalizatio ns and extensions  to the basic  system,  but in
much less detail. We hope the detail of the earlier  part of the book  can  be transferred  to these
generalizations and, together with the references, will provide an introduction   to the topics.



7.1    Tiling the Tim于Frequency or Time-Scale Plane
A qualitative descriptive presentation of the decomposition of a signal using wavelet systems
or wavelet transforms consists of partitioning the time-scale plane into tiles according to the
in小ces k arid j defined in (1.5). That is possible for orthogonal bases (or tight frames) because
of Parseval's theorem. Indeed, it is Parseval's theorem that states that the signal energy can be
partitioned on the time-scale plane. The shape and location of the tiles shows the logarithmic
nature of the partitioning using basic wavelets and how the M-band systems or wavelet packets
modify the basic picture. It also allows showing that the effects of time- or shift-varying wavelet
 systems, together with M-band and packets, can give an almost arbitrary partitioning of the
plane.
                                                                                             (4.24).
     The energy in a signal is given in terms of the DWT by Parseval's relation in (2.36) or
 This shows the energy is a function   of the translation index k and the scale index j.



                          /b（테' 毗：立 jc(l)I2*立 立 似（.2，丸尸）
                                         1＝누00          7==O 七＝
                                                              ＝卜仗）
                                                                                               (7.1)



      The wavelet transform allows analysis of a signal or parameterization of a signal that can
                                                                                               the
 locate energy in both the time and scale (or frequency) domain within the constraints of
 uncertainty principle. The spectrogram used in speech analysis is an example of using the short-
 time Fourier transform to describe speech simultaneously in the time and frequency domains.
       This graphical or visual description of the partitioning of energy in a signal using tiling
 depends on the stracture of the system, not the parameters of the system. In other words, the
                                                                                          wavelet
  tiling partitioning will depend on whether one uses M = 2 or M = 3, whether one uses

 98
                                                                                                   99
Sec. 7工 Tiling the 기m于Frequency or 기me尸Sca地 F기ane


packets or time-varying wavelets, or whether one uses over-complete frame systems. It does
                                                                                              or the
not depend on the particular coefficients h(n) or h (n), on the number of coefficients N,
number of zero moments. One should remember that the tiling may look as       if the indices   j and
k are continuous variables, but they are not. The energy is really a function of discrete  variables
in the DWT domain, and the boundaries of the tiles are symbolic of the partitioning. These
                                                                                                   as
tiling boundaries becomlle more literal when the continuous wavelet transform (CWT) is used
described in Section 7.8, but even there it does not mean that the partitioned energy    is literally
confined to the tiles.



Nonstationary Signal Analysis
                                                                                                   For
In many applications, one studies the decomposition of a signal in terms of basis functions.
example, stationary signals are decomposed into the Fourier basis      using the Fourier  transform.
For nonstationary signals (i.e., signals whose frequency characteristics are time-varying like mu-
                                                                                                 ation.
sic, speech, images, etc.) the Fourier basis is ill-suited because of the poor time-localiz
The classical solution to this problem is to use the short-time (or    windowed)  Fourier  transform
 (STFT). However, the STFT has several problems, the most severe being the fixed time-frequency
resolution of the basis functions. Wavelet techniques give a new class of (potentially signal depen-
 dent) bases that have desired time-frequency resolution properties. The "optimal" decomposition
 depends on the signal (or class of signals) studied. All classical time-frequency decompositions
 like the Discrete STFT (DSTFT), however, are signal independent. Each function in a basis can
 be considered schematically as a tile in the time-frequency plane, where most of its energy is
 concentrated. Orthonormality of the basis 血nctions can be schematically captured by nonover-
                                                                                           (i.e., delta
 lapping tiles. With this assumption, the time-frequency tiles for the standard basis
 basis) and the Fourier basis (i.e., sinusoidal basis) are shown in Figure 7.1.




          f                                           f




                              t                                           t
                            (a)                                         (b)


 Figure 7.1. (a) Dirac Delta Function or Standard Time Domain Basis (b) Fourier or Standard
 Frequency Domain Basis
 100                                      Generalizations of the Basic Multiresolution Wavelet System   Ch. 7

 Tiling with the Discrete-Time Short-Time Fourier Transform
 The DSTFT basis functions are of the form

                                    凹3 , 丸（t) = w(t 寸 丸丁b)e_ u3W0t                                      (7.2)
 where w(t) is a window function [Gab46J. If these functions form an orthogonal (orthonormal)
 basis, x(t) = >二j,k (x, wj,k) wj,k (t). The DSTFT coefficients, (X, w3,k), estimate the presence of
signal components centered at (kTo, jwo) in the time-frequency plane, i.e., the DSTFT gives a
uniform tiling of the time-frequency plane with the basis functions {w7,k (t)}. If 스t and 스W are
time and frequency resolutions respectively of w(t), then the uncertainty principle demands that
스t스W < 1/2 [Dau90, Sie86]. Moreover, if the basis is orthonormal, the Balian-Low theorem
implies either 스t or 스W is infinite. Both 스t and 스, can be controlled by the choice of w(t), but
for any particular choice, there will be signals for which either the time or frequency resolution
is not adequate. Figure 7.1 shows the time-frequency tiles associated with the STFT basis for
a narrow and wide window, illustrating the inherent time-frequency trade-offs associated with
this basis. Notice that the tiling schematic holds for several choices of windows (i.e., each figure
represents all DSTFT bases with the particular time-frequency resolution characteristic).




         I                                          I




                            t                                              t
                          (a)                                            (b)


       Figure 7.2. (a) STFT Basis - Narrow Window. (b) STFT Basis - Wide Window.



Tiling with the Discrete Two-Band Wavelet Transform
The discrete wavelet transform (DWT) is another signal-independent tiling of the time-frequen
                                                                                                 cy
plane suited for signals where high frequency signal components have shorter duration than low
frequency signal components. Time-frequency atoms for the DWT, {砂j,k (t)} = {2i'2砂(2Jt - k) },
are obtained by translates and scales of the wavelet function 砂 (t). One shrinks/stretches the
wavelet to capture high-/low-frequency components of the signal. If these atoms form an or-
thonormal basis, then x(t) = Z j ,k (x, 砂j,k) 砂j,k (t). The DWT coefficients, (x, 砂j,k), are a mea-
Sec. 7工 T川ng the 기me-Frequency or 기me尸Sca匣 F기ane                                                 101

sure of the energy of the signal components located at (2小3k, 23) in the time-frequency plane,
giving yet another tiling of the time-frequency plane. As discussed in Chapters 3 and 8, the
DWT (for compactly supported wavelets) can be efficiently computed using tw아channel unitary
FIR filter banks [Dau88a]. Figure 7.3 shows the corresponding tiling description which illustrates
time-frequency resolution properties of a DWT basis. If you look along the frequency (or scale)
axis at some particular time (translation), you can imagine seeing the frequency response of the
filter bank as shown in Figure 3.5 with the logarithmic bandwidth of each channel. Indeed, each
horizontal strip in the tiling of Figure 7.3 corresponds to each channel, which in turn corresponds
to a scale j. The location of the tiles corresponding to each coefficient is shown in Figure 7.4. If
at a particular scale, you imagine the translations along the k axis, you see the construction of
the components of a signal at that scale. This makes it obvious that at lower resolutions (smaller
j) the translations are large and at higher resolutions the translations are small.




                              I




                                                   t

                              Figure 7.3. Two-band Wavelet Basis

    The tiling of the time-frequency plane is a powerful graphical method for understanding the
properties of the DWT and for analyzing signals. For example, if the signal being analyzed were
a single wavelet itself, of the form
                                        f (t) = 砂（4t - 2),                                 倪3)
the DWT would have only one nonzero coefficient, d2(2). To see that the DWT is not time (or
shift) invariant, imagine shifting 1 (t) some noninteger amount and you see the DWT changes
considerably. If the shift is some integer, the energy stays the same in each scale, but it "spreads
out" along more values of k and spreads differently in each scale. If the shift is not an integer, the
energy spreads in both j and k. There is no such thing as a "scale limited" signal corresponding
to a band-limited (Fourier) signal if arbitrary shifting is allowed. For integer shifts, there is a
corresponding concept [GOB94].

General Tiling
Notice that for general, nonstationary signal analysis, one desires methods for controlling the
tiling of the time-frequency plane, not just using the two special cases above (their importance
102                                                            Generalizations of the Basic Multiresolution Wavelet System                   Ch. 7




                二
                肛
                0촌 喜去욘身身身占 횹흩흩흘言흩套 套立立릅촙흡츱훑흩훑훑盲훑츱훑흡
                     “
                                         “
                                                    “
                                                                                    “                         “     “
         f

                d4,o d4,1 d4,2 d4.3 d4,4 d4,5 d4,6 d4,7 d4,8 d4,9 d4,10 d4,11 d4,12 d4,13 d4,14 d4,15




                    d3,0          d3,1                  d3,2          d3,3              d3,4          d3,5              d3,6          d3,7



                           d2,0                                d2,1                            d2,2                            d2,3

                                             d1,0                                                            d1,1
                                                                             d0,0



                                                                             t


                         Figure 7.4. Relation of DWT Coefficients d3,k to Tiles


notwithstanding). An alternative way to obtain orthonormal wavelets 砂(t) is using unitary FIR
filter bank (FB) theory. That will be done with M-band DWTs, wavelet packets, and time-varying
wavelet transforms addressed in Sections 7.2 and 7.3 and Chapter 8 respectively.
     Remember that the tiles represent the relative size of the translations aild scale change. They
do not literally mean the partitioned energy is confined to the tiles. Representations with similar
tilings can have very different characteristics.


7.2    Multiplicity-M (M-Band) Scaling Functions and Wavelets
While the use of a scale multiplier M of two in (5.1) or (7.4) fits many problems, coincides with
the concept of an octave, gives a binary tree for the Mallat f戚 algorithm, and gives the constant-
Q or logarithmic frequency bandwidths, the conditions given in Chapter 5 and Section 5.8 can be
stated and proved in a more general setting where the basic scaling equation (5.1) uses a general
Sec. 7.2. Muttiplicity-M (M-Band) Scaling Functions and Wavelets                             103


scale factor or multiplicity of M [ ZT92b, ZT92a, GB92c, SHGB93, Hel95, GOB92, Vai87b] rather
than the specific doubling value of M = 2. Part of the motivation for a larger M comes from a
desire to have a more flexible tiling of the time-scale plane than that resulting from the M = 2
wavelet or the short-time Fourier transform discussed in Section 7.1. It also comes from a desire
for some regions of uniform band widths rather than the logarithmic spacing of the frequency
responses illustrated in Figure 3.5. The motivation for larger M also comes from filter bank
theory which is discussed in Chapter 8.
    We pose the more general multiresolution formulation where (5.1) becomes

                                    甲（끼스그回V파(Mx -미·                                          (7.4)

In some cases, M may be allowed to be a rational number; however, in most cases it must be an
integer, and in (5.1) it is required to be 2. In the frequency domain, this relationship becomes

                                                                                             (7.5)
                                     .（
                                          『）
                                               =   슈H
                                                         (町川蜘／川
and the limit after iteration is


                                     如＝m古川쓿和이                                                (7.6)


 assuming the product converges and 令 (0) is well defined. This is a generalization of (5.52) and
 is derived in (5.74).

 Properties of M-Band Wavelet Systems
 These theorems, relationships, and properties are generalizations of those given in Chapter 5 and
 Section 5.8 with some outline proofs or derivations given in the Appendix. For the multiplicity-M
 problem, if the support of the scaling function and wavelets and their respective coefficients is
 finite and the system is orthogonal or a tight frame, the length of the scaling function vector or
 filter h(n) is a multiple of the multiplier M. This is N = M C, where Resnikoff and Wells [RW971
 call lvi the rank of the system and C the genus.
      The results of (5.10), (5.14), (5.16), and (5.17) become

 Theorem 28 IfY7(t) is an L' solution to (7.4) and f 甲(t) dt 尹 0, then

                                                   二M미 = 而7·                                  (7.7)


 This is a generalization of the basic multiplicity-2 result in (5.10) and does not depend on any
 particular normalization or orthogonality of o(t).

 Theorem 29 If integer translates of the solution to (7.4) are orthogonal, then

                                          乞枷＋Mm) h（미 = 6(m)·                                  倪8)
 104                                       Generalizations of the Basic Multiresolution Wavelet System           Ch. 7


This is a generalization of (5.14) and also does not depend on any normalization. An interesting
corollary of this theorem is

Corollary 3 If integer translates of the solution to (7.4) are orthogonal, then


                                            刃h
                                                    (n)
                                                          I2=   1.
                                                                                                           (7.
                                                                                                                   9)
    A second corollary to this theorem is

Corollary 4 If integer translates of the solution to (7.4) are or航ogonal, then

                             ＞二九（兀In + m) = 1/ \／而．                   me Z                               (7.10)

This is also true under weaker conditions than orthogonality as was discussed for the M = 2
case.
   Using the Fourier transform, the following relations can be derived:

Theorem 30 IfY7(t) is an L1 solution to (7.4) and f 甲(t) dt 尹 0, then

                                                 且（0) = \/M                                              (7.11)
which is a frequency domain existence condition.

Theorem 31 The integer translates of the solution to (7.4) are orthogonal if and only if

                                      ＞二 陣（回 + 2冗Z）尸 = 1                                                 (7.12)
                                       I


Theorem 32 If甲(t) is an L1 solution to (7.4) and fY)(t) dt 尹 0, then

                                  ＞二九（n + 凡'fmn) 九（미 = d(rn)                                             (7.13)

if and only if

 田佃下 + 田佃 + h胛甲 + 回w + 4ir/Jt떼뇨 · · · + 田佃 + 2冗（M- 1)/M）尸 = M. (7.14)



This is a frequency domain orthogonality condition on h(n).

Corollary 5
                           H (2irZ /M) = 0,         for Z = 1, 2, · . . , M 中 1                          (7.15)


which is a generalization of (5.20) stating where the zeros of H (w), the frequency response of the
scaling filter, are located. This is an interesting constraint on just where certain zeros of H (z)
must be located.
 Sec. 7.2. Multiplicity-M (M-Band) Scaling Functions and Wavelets                                   105
                                                              \

 Theorem 33 {/ 乙小（미 = \／祈, 口nd h(n) 加5／沆te sup끄01才 or decays ／口st enoug九, 坑en 口
 99(t) E L2 坑毗 sa挽sfies (7.4) e娩就S 口nd is unique.

 Theorem 34 If 乙小（미 = \／苾 口nd寸 已枷川小A砒）＝히砒                                              坑en97(t) e缸就5, is
 integr口ble, （工nd gener口tes （工 wavelet system 坑毗 is 口 tig砒 /'rame 仇 r.

    These results are a significant generalization of the basic M = 2 wavelet system that we
discussed in the earlier chapters. The definitions, properties, and generation of these more general
scaling functions have the same form as for M = 2, but there is no longer a single wavelet
associated with the scaling function. There are M - 1 wavelets. In addition to (7.4) we now have
M 卞 1 wavelet equations, which we denote as

                                    吻（t) = >.      v'Mht(n) co(Mt- n)                             (7.16)

幻r
                                            Z = 1, 2, . · · ,M- 1.
Some authors use a notation ho(n) for h(n) and Y o(t) for 砂(t), so that h (n) represents the
coefficients for the scaling function and all the wavelets and 1(t) represents the scaling function
and all the wavelets.
   Just as for the M = 2 case, the multiplicity-M scaling function and scaling coefficients are
unique and are simply the solution of the basic recursive or refinement equation (7.4). However,
the wavelets and wavelet coefficients are no longer unique or easy to design in general.
   We now have the possibility of a more general and more flexible multiresolution expansion
system with the M-band scaling function and wavelets. There are now M - 1 signal spaces
spanned by the M 小 1 wavelets at each scale j. They are denoted

                                        34幻 = Spa머吻（M't + 劤                                       (7.17)
                                               七
幻r Z == L 2r · · 小1- 1. For （八ample 玖rith Al = 4,

                                     V1 = V0 今 34노0 由）기屯,0 q W3,tj                                (7.18)
and
                                     V2 = Vi q) Wi,i q) W2,i 由 W3,i                              (7.19)
or
                       V2 = )7b q) yn,0 0 M吃,0 田 까b,0 q) yn, l q) M吃, l q) ）人73, l .             (7.20)
In the lim代 as,) -) 以기 we have

               L2 = V0 4) }Vl ,0 田 }V2,O 今 끼73,0 由 끼p1,1 0 玖p2,1 由 叭?3,1 + · · · 田 끼／3 ,아y       (7.21)

Our notation for M = 2 in Chapter 2 is W1,3 = W3
    This is illustrated pictorially in Figure 7.5 where we see the nested scaling function spaces V3
but each annular ring is now divided into M - 1 subspaces, each spanned by the M 中 1 wavelets
at that scale. Compare Figure 7.5 with Figure 2.3 for the classical M = 2 case.
106                                                         Generalizations of the Basic Multires이ution Wavelet System                    Ch. 7




                                                                                                                               V2




                                                                                                                               V1




       Figure 7.5. Vector Space Decomposition for a Four-Band Wavelet System, Wj

   The expansion of a signal or function in terms of the M-band wavelets now involves a triple
sum over Z小 and 丸．
                                                                以）       아D 入1- 1

                f(t) = ＞二C（丸）(Pk(t) + ＞二 ＞二 ＞二 凡川2 d1,3(k）吻（M3t出                                                                    (7.22)
                         k                                  k=니oj= O e=1

where the expansion coefficients (DWT) are found by


                                                                 //(!      )7
                                                                                     (:        －        丸）   毗                      (7.23)
                                          .（丸）              :


and

                             吼（,     )=                ff        (t) Mi1 （M3t   '吻                           -       k）   毗·        (7.    24)
We now have an M-band discrete wavelet transform.

Theorem 35 If the scaling function 甲(t) satisfies the conditions for existence and orthogonality
口nd 坑ew口velets are defined by (7.16) and i/ 坑e integer tr（工nsl口tes 0/ 坑ese 凹（ivelets sp（工nYt뇨
the or仇ogonal compliments of V0, all being in V1, i.e., the wavelets are orthogonal to the scaling
戶inction （比 坑e same sc口le; that is, if

                                                                                                                                    (7.25)
                                    fco          (t-            n）      吻（:     -         m）       毗＝            .
加r Z = 1, 2, · · · ,M- 1, 仇en
                                          ＞二九（n) 뇨(n -凡作） = 0                                                                       (7.26)

for all integersk and fort= 1, 2, · . . ,M- 1.

Combining (7.8) and (7.26) and calling ho(n) = h(n) gives

                             ＞二九m(fl) ht(n 中 凡tk) = 冊）히m- Z)                                                                        倪27)
                                n


as necessary conditions on h (미 for an orthogonal system.
Sec. 7.2. Multiplicity-M (M-Band) Scaling Functions and Wavelets                                                107'



                                    H
                                               /2l2    .1.   4


                                               九11     .1.   4


                                               h10           4
                             V2
                                                       .1.
                                                                                  h12


                                                                       V1
                                                                            H     h
                                                h
                                                                                               ＝
                                                             4
                                                                 mH+
                                    HH
                                                       .1.
                                                                            H
                                                                                  h10          뇨
                                                                                  h      .1.       4   -   V0




            Figure 7.6. Filter Bank Structure for a Four-Band Wavelet System, Wt


    Unlike the M = 2 case, for M > 2 there is no formula for hi(미 and there are many possible
wavelets for a given scaling function.
    Mallat's algorithm takes on a more complex form as shown in Figure 7.6. The advantage is
a more flexible system that allows a mixture of linear and logarithmic tiling of the time田cale
plane. A powerful tool that removes the ambiguity is choosing the wavelets by "modulated
cosine" design.
    Figure 7.7 shows the frequency response of the filter band, much as Figure 3.5 did for M = 2.
Examples of scaling functions and wavelets are illustrated in Figure 7.8, and the tiling of the time-
scale plane is shown in Figure 7.9. Figure 7.9 shows the time-frequency resolution characteristics
of a four-band DWT basis. Notice how it is different from the Standard, Fourier, DSTFT and
two-band DWT bases shown in earlier chapters. It gives a mixture of a logarithmic and linear
frequency resolution.




                IH   (cJ)    I
                            V0 W10W20W30         W11                        w21         w31

                                           /



              Figure 7.7. Frequency Responses for the Four-Band Filter Bank, W
108                                             Generalizations of the Basic Multiresolution Wavelet System         Ch. 7


                    0.6
                                                                              0.4-
                    0.5 H

                    0.4 ,                                                     0.2

                0.3-

                0.
                                                                             -0.2
                         1-
                         2-
                    。.
                                                                             -0.4-
                         0
                                                                             -0.6
             -0.1-



                                     (a）   中                                               (b) 砂0



                                                                              0.5 ,



                                                                                      了 V사＼力뇨
                0뫄

                         。F.                                                    0-
             -。.2




                                                                         -0.5



                                                                                                    6

                                     （이 砂1                                                 (d) 砂2

                               Figure 7.8. A Four-Band Six-Regular Wavelet System


   ＼入／e ne玭 define the 丸t九 moments of 吻（t) as


                                               m,   (k)   =   Jt        '吻           （ 毗
                                                                                      (）                      (7.    28)
and the kth discrete moments of ht (n) as

                                               仰(k) =Z nkh (n)·                                               (7.29)
                                                                   71

Theorem 36 (Equivalent Characterizations of K-Regular M-Band Filters) A unitary scal-
ing filter is K-regular if and only if the following equivalent statements are true:
  1. All moments of the wavelet filters are zero, 仰(k) = 0, for k = 0, 1, . . . , (K - 1) and for
     Z = L 2, · · · ,（凡J H l)
  2. All moments of the wavelets are zero, mf (k) = 0, for k = 0, 1, . - - , (K - 1) and for t =
     1, 2, - - - ,(M- 1)

  3. The partial moments of the scaling filter are equal for k = 0, 1, - . - , (K - 1)

  4. The frequency response of the scaling filter has zeros of order K at the Mth roots of unity,
     뇨，= 27r f /Itf 加r f = 1, 2, · · · 小／ _1.

   5. The magnitude-squared frequency response of the scaling filter is flat to order 2K at w = 0.
      This follows from (5.22).
 Sec. 7.2. Multiplicity-M (M-Band) Scaling Functions and Wavelets                              109




                              I




                                                        t

                                  Figure 7.9. 4-band Wavelet Basis Tiling


   6. All polynomial sequences up to degree (K - 1) can be expressed as a linear combination of
      2毗eger-sh洸ed sc口ling filters.

   7. All polynomials of degree up to (K 中 1) can be expressed as a linear combination of integer-
      就沂ed sc（流凹 加nctions for all j.



This powerful result [SHGB93, Hel95J is similar to the M = 2 case presented in Chapter 6. It not
only ties the number of zero moments to the regularity but also to the degree of polynomials that
can he exactly represented by a sum of weighted and shifted scaling functions. Note the location
of the zeros of H (z) are equally spaced around the unit circle, resulting in a narrower
                                                                                         frequency
response than for the half-band filters if M = 2. This is consistent with the requirements
                                                                                              given
in (7.14) and illustrated in Figure 7.7.
    Sketches of some of the derivations in this section are given in the Appendix or are
                                                                                             simple
extensions of the M = 2 case. More details are given in [GB92c, SHGB93, Hel95].


M-Band Scaling Function Design
Calculating values of o(n) can be done by the same methods given in Section 5.10. However, the
design of the scaling coefficients h(n) parallels that for the two-band case but is somewhat more
difficult [Hel95].
    One special set of cases turns out to be a simple extension of the two-band system. If the
multiplier M = 2772, then the scaling function is simply a scaled version of the M = 2 case and
a particular set of corresponding wavelets are those obtained by iterating the wavelet branches
of the Mallat algorithm tree as is done for wavelet packets described in Section 7.3. For other
values of M, especially odd values, the situation is more complex.
110                                       Generalizations of the Basic Multiresolution Wavelet System   Ch. 7



M-Band Wavelet Design and Cosine Modulated Methods
For M> 2 the wavelet coefficients hZ(n) are not uniquely determined by the scaling coefficients, as
was the case for M = 2. .This is both a blessing and a curse. It gives us more flexibility in designing
specific systems, but it complicates the design considerably. For small N and M, the desi因ls can
be done directly, but for longer lengths and/or for large M, direct design becomes impossible
and something like the cosine modulated design of the wavelets from the scaling function as
described in Chapter 8, is probably the best approach [KV92, Ngu92, NK92, Mal92, Mau921
[OGB94, GB95c, GB92a, GB95b, GB93, NH96, RT91, Ngu94, Ngu95a].


7.3    Wavelet Packets
The classical M = 2 wavelet system results in a logarithmic frequency resolution. The low
frequencies have narrow bandwidths and the high frequencies have wide bandwidths, as illustrated
in Figure 3.5. This is called "constant-Q" filtering and is appropriate for some applications but
not all. The wavelet packet system was proposed by Ronald Coifman [Rus92, CW92] to allow a
finer and adjustable resolution of frequencies at high frequencies. It also gives a rich structure
that allows adaptation to particular signals or signal classes. The cost of this richer structure
is a computational complexity of O(Nlog(N)), similar to the FFT, in contrast to the classical
wavelet transform which is O(N).

Full Wavelet Packet Decomposition
In order to generate a basis system that would allow a higher resolution decomposition at high
frequencies, we will iterate (split and down-sample) the highpass wavelet branch of the Mallat
algorithm tree as well as the lowpass scaling function branch. Recall that for the discrete wavelet
transform we repeatedly split, filter, and decimate the lowpass bands. The resulting three-scale
analysis tree (three-stage filter bank) is shown in Figure 3.4. This type of tree results in a
logarithmic splitting of the bandwidths and tiling of the time-scale plane, as shown in Figure 7.3.
     If we split both the lowpass and highpass bands at all stages, the resulting filter bank structure
is like a full binary tree as in Figure 7.10. It is this full tree that takes O(N log N) calculations
and results in a completely evenly spaced frequency resolution. In fact, its structure is somewhat
similar to the FFT algorithm. Notice the meaning of the subscripts on the signal spaces. The first
integer subscript is the scale j of that space as illustrated in Figure 7.11. Each following subscript
is a zero or one, depending the path taken through the filter bank illustrated in Figure 3.4. A
 "zero" indicates going through a lowpass filter (scaling function decomposition) and a "one"
indicates going through a highpass filter (wavelet decomposition). This is different from the
convention for the M > 2 case in Section 7.2.
     Figure 7.11 pictorially shows the signal vector space decomposition for the scaling functions
and wavelets. Figure 7.12 shows the frequency response of the packet filter bank much as Fig-
ure 3.5 did for M = 2 and Figure 7.7 for M = 3 wavelet systems.
     Figure 7.14 shows the Haar wavelet packets with which we finish the example started in
Section 2.8. This is an informative illustration that shows just what "packetizing" does to the
regular wavelet system. It should be compared to the example at the end of Chapter 2. This
is similar to the Walsh-Haddamar decomposition, and Figure 7.13 shows the full wavelet packet
system generated from the Daubechies oDs, scaling function. The "prime" indicates this is the
Daubechies system with the spectral factorization chosen such that zeros are inside the unit circle
Sec. 了3. Way미et Packets                                                                     111



                                                                                  1,v211

                                                                                  w210

                                                                                  功／201

                                                                                  功／2｛兀
            V3
                                                                                  Wi1

                                                                                  Wi0

                                                                                  wo
                                              h0     12
                                                                                  V0




        Figure 7.10. The full binary tree for the three-scale wavelet packet transform.



and some outside. This gives the maximum symmetry possible with a Daubechies system. Notice
the three wavelets have increasing "frequency." They are somewhat like windowed sinusoids,
hence the name, wavelet packet. Compare the wavelets with the M = 2 and M = 4 Daubechies
wavelets.



Adaptive Wavelet Packet Systems
Normally we consider the outputs of each channel or band as the wavelet transform and from
this have a nonredundant basis system. If, however, we consider the signals at the output of each
band and at each stage or scale simultaneously, we have more outputs than inputs and clearly
have a redundant system. From all of these outputs, we can choose an independent subset as a
basis. This can be done in an adaptive way, depending on the signal characteristics according
to some optimization criterion. One possibility is the regular wavelet decomposition shown in



                                                                   V3
                                                                   V2
                                                                   'V1




      Figure 7.11. Vector Space Decomposition for a Al = 2 Full Wavelet Packet System
112                                                          Generalizations of the Basic Multiresolution Wavelet System     Ch. 7



              田佃）1

                                V0        wo       Wio       W11   W200        W201         W210   W211




                                                                                                                    1   口J

                            0                                                                                       冗




      Figure 7.12. Frequency Responses for the Tw아Band Wavelet Packet Filter Bank



Figure 3.3. Another is the full packet decomposition shown in Figure 7.10. Any pruning of this
full tree would generate a valid packet basis system and would allow a very flexible tiling of the
time-scale plane.
    We can choose a set of basic vectors and form an orthonormal basis, such that some cost
measure on the transformed coefficients is minimized. Moreover, when the cost is additive, the


              0.
                                                                          0.8 ·

              。6   .5
                                                                          0.6 ,

                                                                          0.4-

                                                                          0.2-

                                                                              0

                                                                         -0.2-

                                                                          -0．
                                                                            中

                                                                         10
                                1     2        3    4    5                    '6b                           4

                                           (a) 砂                                               (b) 砂0

               0.8                                                         0.8 .                       1
                                                                           0.6
               0.6
                                                                           0.4
              0.4
                                                                           0.2-
               0.2
                                                                              0




                                                                                                   1
                                                                                                           1M
                        0
                                                                                      小八I
                                                                          -0.2
              -0.2                                                        -0.4-

              -0.4                                                        -0.6-
                                                                          -0.8
                                               3    4          6                                   3            4

                                          （이 V 10                                              (d) 砂11


                                     Figure 7.13. Wavelet Packets Generated by 砂DS'
 Sec. 7.3. Wav&et Packets
                                                                                                                                                    113


         V3fl                V2                       V1
                                                               1            1                       V0



             J그                                                                                     wo I
                                                                                                                                                1
                                                           1                                        w빠H
                                                                            f                                                           니
                                                                                                                                       m．




                                                                        CH
                                                                                                1   w"口                                口
                             w2                       W20 r                                         W如
                                        다J                 '       느H   그
                                                                                                             1m
                                                                                                             '        m   mm       _        1
                                        -r                              rm
                                                                                                    니72玎e                                   기
                                                                        '             U4   mJ




                                             J   m小   W2in p                                        w2幻口                                    기

                        -n
                                             다J                         n ［그 W2flr.                      '        _            _            l


                             Figure 7.14. The Haar Wavelet Packet




best orthonormal wavelet packet transform can be found using a binary searching algorithm
[CW92] in O(NlogN) time.
   Some examples of the resulting time-frequency tilings are shown in Figure 7.15. These plots
demonstrate the frequency adaptation power of the wavelet packet transform.




                                  (a)
                                                                                (b)
Figure 7.15. Examples of Time-Frequency Tilings of Different Three-Scale Orthonormal
Wavelet Packet 끄ansforms.
                                           Generalizations of the Basic Multiresolution Wavelet System    Ch. 7
114


   There are two approaches to using adaptive wavelet packets. One is to choose a particular
                                                                                              to be
decomposition (filter bank pruning) based on the characteristics of the class of signals
                                                                          signals. The  other  is to
processed, then to use the transform nonadaptively on the individual
                                                                          process  over the class of
adapt the decomposition for each individual signal. The first is a linear
signals. The second is not and will not obey superposition.
   Let P(J) denote the number of different J-scale orthonormal wavelet packet transforms. We
can easily see that
                         P(J) = P(J 卞 1)2 + 1,                         P(1) = 1.                         (7.30)

So the number of possible choices grows dramatically as the scale increases. This is another reason
for the wavelet packets to be a very powerful tool in practice. For example, the FBI standard
                                                                                        transforms.
for fingerprint image compression [BBH93, BBOH96I is based on wavelet packet
The wavelet packets are successfully used for acoustic signal compression {Wic921.     In  [RV93], a
rate-distortion measure is used with the wavelet packet transform to improve    image  compression
performance.
   M-band DWTs give a flexible tiling of the time-frequency plane. They are associated with
a particular tree-structured filter bank, where the Iowpass channel at any depth is split into
M bands. Combining the M-band and wavelet packet structure gives a rather arbitrary tree-
structured filter bank, where all channels are split into sub-channels (using filter banks with
a potentially different number of bands), and would give a very flexible signal decomposition.
The wavelet analog of this is known as the wavelet packet decomposition [CW92]. For a given
                                                                                           sense) filter
signal or class of signals, one can, for a fixed set of filters, obtain the best (in some
bank tree-topology. For a binary tree an efficient scheme using entropy as the      criterion has been
developed-the best wavelet packet basis algorithm [CW92, RV93].


7.4     Biorthogonal Wavelet Systems
                                                                                              scale gives
Requiring the wavelet expansion system to be orthogonal across both translations and
a clean, robust, and    symmetric    formulation  with a  Parseval's  theorem.    It also  places  strong
limitations on the possibilities  of the system. Requiring  orthogonali   ty uses up  a large number    of
the degrees of freedom, results    in  complicated  design equations,   prevents  linear  phase  analysis
                                                                                                  section
and synthesis filter banks, and prevents asymmetric analysis and synthesis systems. This
                               l wavelet system  using a nonorthogo   nal basis and  dual  basis to allow
 will develop the biorthogona
greater flexibility in achieving   other  goals at the expense  of  the  energy   partitioning  property
 that Parseval's theorem states [CDF92, Wei95, Tia96, WTWB97, NH96, AAU96, Coh92, KT93,
RG95, Swe96a1. Some researchers have considered "almost orthogonal" systems where there is
 some relaxation of the orthogonal constraints in order to improve other characteristics [OB95].
 Indeed, many image compression schemes (including the fingerprint compression used by the FBI
 [BBH93, BBOH96]) use biorthogonal systems.


 Two Channel Biorthogonal Fitter Banks
                                                                                                  are time
 In previous chapters for orthogonal wavelets, the analysis filters and synthesis filters
 reversal of each other; i.e., h(n)    =  h(- ri),  (n) =  g(-  n). Here,  for the biorthogona  l case, we
 relax these restrictions.   However,    in order  to perfectly  reconstruct the input,  these four  filters
 still have to satisfy a set of relations.
Sec. 7.4. Biorthogonal Wavelet Systems                                                          115




                                g                    南（k) -               g


          ci (n)



                                方                             I          h




                         Figure 7.16. Two Channel Biorthogonal Filter Banks


   Let c1(n), n E Z be the input to the filter banks in Figure 7.16, then the outputs of the
analysis filter banks are

                    Co（丸）=＞二万（2k - n)ci(ri),             而（丸）=＞二亘（2丸- fl)Ci(fl).              (7.31)


The output of the synthesis filter bank is

                           自（m) = ＞二 ［九（2丸 -m）匈（丸） +g(2丸 小 m)do（丸）] .                         (7.32)
                                         丸

Substituting Equation (7.31) into (7.32) and interchanging the summations gives

               自的스二汁마如枷丸- n) + g마- m) (2卜小炯·                                                  (7.33)
                            n       k

For perfect reconstruction, i.e., 自(m) = ci(m),Vm E Z, we need

                   디빠小m出胱- n) + g마- m) (2k刊 = (m - n).                                        (7.34)
                     k

Fortunately, this condition can be greatly simplified. In order for it to hold, the four filters have
to be related as [CDF92]

                           9(n) = (- 1)'h (1 - n),       g(n) = (- 1)nh(1 - n),               (7.35)

up to some constant factors. Thus they are cross-related by time reversal and flipping signs of
every other element. Clearly, when h = h, we get the familiar relations between the scaling coef-
ficients and the wavelet coefficients for orthogonal wavelets, g(n) = (- 1) h(1 - n). Substituting
(7.35) back to (7.34), we get
                                     乞枷川n+ 刈 = 冊）.                                          (7.36)
                                             n


In the orthogonal case, we have >二n h(n)h(n + 2k) = 8(k); i.e., h(n) is orthogonal to even
translations of itself. Here h is orthogonal to h, thus the name biorlhogonal.
116                                      Generalizations of the Basic Multiresolution Wavelet System    Ch. 7


   Equation (7.36) is the key to the understanding of the biorthogonal filter banks. Let 's assume
h(n) is nonzero when N1 5 n 5 N2, and h(n) is nonzero when N1 드 ii 5 N. Equation (7.36)
implies that [CDF92I

                     N2- N1= 2k+ 1,        N2- N1= 2k+ 1,               丸，丸 E Z.                       (7.37)

In the orthogonal case, this reduces to the well-known fact that the length of h has to be even.
Equations (7.37) also imply that the difference between the lengths of h and h must be even.
Thus their lengths must be both even or both odd.

Biorthogonal Wavelets
We now look at the scaling function and wavelet to see how removing orthogonality and intro-
ducing a dual basis changes their characteristics. We start again with the basic multiresolution
definition of the scaling function and add to that a similar definition of a dual scaling function.

                                  蛔 = Z枷NM小 미，                                                         (7.38)


                                   a(t) = ＞二万（n)V5a(2t 寸 ii).                                          (7.39)
                                           11


From Theorem 1 in Chapter 5, we know that for 砂 and 中 to exist,

                                  ＞二九（미 = 三風미 = V／豆                                                    (7.40)


Continuing to parallel the construction of the orthogonal wavelets, we also define the wavelet and
the dual wavelet as

                  砂（t) = ＞二g(n)v'加(2t 小 n) = ＞二（-1)" 方（1- n)v'配(2t 小 n),                               (7.41)
                          n                         n


                  am= Z如N璥小미＝ZH)" 九（1中n)V耶r.2t- n).                                                    (7.42)
Now that we have the scaling and wavelet functions and their duals, the question becomes whether
we can expand and reconstruct arbitrary functions using them. The following theorem [CDF92J
answers this important question.

Theorem 37 For h and h satisfying (7.36), suppose that for some C, e > 0,

                    陣（w)I 5 C(1+ w）小1/2-c ,             陣（W) 1 드 C(1+ kJ)el/2 '.                       仁43)

可中 and a defined above 九口ye su끄icient decay in the frequency domain, 坑en 砂j, k 望f23/2砂（23x -
丸）, j, k E Z cons仇tute a frame in L2(R). T九e加 而毗 frame is g切en by 寸j,k 匹f 2j/2寸（23x -
丸）, 3小 E Z; for 口fly / e [2 (1t),

                              / = Z伍屯k) 日j,k
                                 3上
                                                          Z （加jk)寸，
                                                                  3小                                   (7.44)
                                                          3小


where the series converge strongly.
 Sec. 7.4. Biorthogonal Wavetet Systems                                                                                                    117

    Moreo叱r, 坑e 砂3大 口nd 砂3 , 丸 consti仇［te 机uo Riesz bases, with


                                    （砂3小，
                                                 可j7,
                                                              (,
                                                                   )   =      d(j   -
                                                                                        j
                                                                                                ')
                                                                                                     d
                                                                                                             （丸－
                                                                                                                                k
                                                                                                                                    ')
                                                                                                                                         (7.45)

if and only if

                                            ／中
                                                 （:     ）如－
                                                                           ,)dx
                                                                                            =            d
                                                                                                                   (
                                                                                                                       (）
                                                                                                                            ·
                                                                                                                                         (7.46)

   This theorem tells us that under some technical conditions, we can expand functions using
the wavelets and reconstruct using their duals. The multiresolution formu'ations in Chapter 2
can be revised as
                                 · · · C l乙2 （二 v-i （二 V0 （二 )"1 C V2 c · · ·                                                            (7.47)

                                 · · ·cV_ 2cV_1cV0cV1cV2c · · .                                                                          (7.48)
where
                                Vi = Span｛中3．丸｝,                                  Vi = Span｛砂j.k}.                                       (7.49)
                                       k                                                 k
If (7.46) holds, we have
                                                 V l- W3,                         V3 1W3,                                                (7.50)
where
                               ）川3 = Span{！口j.k},                                 ）시3 = Spa머好k}.                                         (7.51)
                                      k                                                  k
Although W3 is not the orthogonal complement to V3 in V3+1 as before, the dual space W3 plays
the much needed role. Thus we have four sets of spaces that form two hierarchies to span L2(R).
    In Section 5.8, we have a list of properties of the scaling function and wavelet that do not
require orthogonality. The results for regularity and moments in Chapter 6 can also be generalized
to the biorthogonal systems.

Comparisons of Orthogonal and Biorthogonal Wavelets
The biorthogonal wavelet systems generalize the classical orthogonal wavelet systems. They
are more flexible and generally easy to design. The differences between the orthogonal and
biorthogonal wavelet systems can be summarized as follows.

   eThe orthogonal wavelets filter and scaling filter must be of the same length, and the length
    must be even. This restriction has been greatly relaxed for biorthogonal systems.

   eSymmetric wavelets and scaling functions are possible in the framework of biorthogonal
     wavelets. Actually, this is one of the main reasons to choose biorthogonal wavelets over the
    orthogonal ones.

   0Parseval's theorem no longer holds in biorthogonal wavelet systems; i.e., the norm of the
     coefficients is not the same as the norm of the functions being spanned. This is one of
     the main disadvantages of using the biorthogonal systems. Many design efforts have been
     devoted to making the systems near orthogonal, so that the norms are close.
                                         Generalizations of the Basic Multiresolution Wavelet System   Ch. 7
118


   . In a biorthogonal system, if we switch the roles of the primary and the dual, the overall
     system is still sound. Thus we can choose the best arrangement for our application. For
     example, in image compression, we would like to use the smoother one of the pair to
     reconstruct the coded image to get better visual appearance.

   . In statistical signal processing, white Gaussian noise remains white after orthogonal trans-
     forms. If the transforms are nonorthogonal, the noise becomes correlated or colored. Thus,
     when biorthogonal wavelets are used in estimation and detection, we might need to adjust
     the algorithm to better address the colored noise.

Example Families of Bi甘thogonal Systems
Because biorthogonal wavelet systems are very flexible, there are a wide variety of approaches to
design different biorthogonal systems. The key is to design a pair of filters h and /i that satisfy
(7.36) and (7.40) and have other desirable characteristics. Here we review several families of
biorthogonal wavelets and discuss their properties and design methods.

Cohen-Daubechies-Feauveau Family of Biorthogonal Spline Wavelets
Splines have been widely used in approximation theory and numerical algorithms. Therefore,
they may be desirable scaling functions, since they are symmetric, smooth, and have dyadic filter
coefficients (see Section 5.7). However, if we use them as scaling functions in orthogonal wavelet
systems, the wavelets have to have infinite support [Chu92a]. On the other hand, it is very easy
to use splines in biorthogonal wavelet systems. Choose h to be a filter that can generate splines,
then (7.36) and (7.40) are linear in the coefficients of h . Thus we only have to solve a set of
                                                                                            better
linear equations to get h , and the resulting h also have dyadic coefficients. In [CDF92],
methods are used to solve these equations indirectly.
    The filter coefficients for some members of the Cohen-Daubechies-Feauveau family of biorthog-
onal spline wavelets are listed in Table 7.1. Note that they are symmetric. It has been shown
that as the length increases, the regularity of 砂 and 砂 of this family also increases [CDF92].

                 /1/ V죵                                    万／V5
                1/2, 1/2                    -1/16, 1/16, 1/2, 1/16, -1/ 16
             1/4, 1/2,1/4                     -1/ 8, 1/4, 3/4, 1/4, -1/ 8
           1/8, 3/8, 3/8, 1/8    5/512, 15/512, 19/512, -97/512, -13/256, 175/ 256, . . .


Table 7.1. Coefficients for Some Members of Cohen-Daubechies-Feauveau Family of Biorthog-
onal Spline Wavelets (For longer filters, we only list half of the coefficients)


Cohen- Daubechies-Feauveau Family of Biorthogonal Wavelets with Less Dissimilar Filter
Length
The Cohen-Daubechies-Feauveau family of biorthogonal wavelets are perhaps the most widely
used biorthogonal wavelets, since the scaling function and wavelet are symmetric and have similar
lengths. A member of the family is used in the FBI fingerprint compression standard [BBH93,
BBOH96I. The design method for this family is remarkably simple and elegant.
Sec. 7.4. Biorthogonal Wavelet Systems                                                          119


        In the frequency domain, (7.36) can be written as

                               H （回）H ' 佃）+ 丑佃 + ir）尸' 佃 + 미 = 2.                             (7.52)

Recall from Chapter 6 that we have an explicit solution for IH(w)尸 = M (w) such that
                                         凡1(w) + 凡1(w + 미 = 2,                                (7.53)

and the resulting compactly supported orthogonal wavelet has the maximum number of zero
moments possible for its length. In the orthogonal case, we get a scaling filter by factoring M (w)
as 且(w)H* 佃). Here in the biorthogonal case, we can factor the same M (w) to get H (w) and
H (w)     .




    Factorizations that lead to symmetric h and h with similar lengths have been found in
[CDF92], and their coefficients are listed in Table 7.2. Plots of the scaling and wavelet func-
tions, which are members of the family used in the FBI fingerprint compression standard, are in
Figure 7.17.

                                          ；
                                          九
                                                            h
                                0.85269867900889     0.78848561640637
                                0.37740285561283     0.41809227322204
                                -0.11062440441844    -0.04068941760920
                                -0.02384946501956    -0.06453888262876
                                 0.03782845550726


Table 7.2. Coefficients for One of the Cohen-Daubechies-Feauveau Family of Biorthogonal
Wavelets that is Used in the FBI Fingerprint Compression Standard (We only list half of the
coefficients)


Tian-Wells Family of Biorthogonal Coiflets
The coifiet system is a family of compactly supported orthogonal wavelets with zero moments
of 1)0th the scaling functions and wavelets described in Section 6.9. Compared with Daubechies'
wavelets with only zero wavelet moments, the coifiets are more symmetrical and may have better
approximation properties when sampled data are used. However, finding the orthogonal coifiets
involves solving a set of nonlinear equations. No closed form solutions have been found, and
when the length increases, numerically solving these equations becomes less stable.
    Tian and Wells [TW95, TWBOar] have constructed biorthogonal wavelet systems with both
zero scaling function and wavelet moments. Closed form solutions for these biorthogonal coifiets
have been found. They have approximation properties similar to the coiflets, and the filter
coefficients are dyadic rationals as are the splines. The filter coefficients for these biorthogonal
Coiflets are listed in Table 7.3. Some members of this family are also in the spline family described
earlier.

Lifting Construction of Biorthogonal Systems
We have introduced several families of biorthogonal systems and their design methods. There is
another method called a lifting scheme, which is very simple and general. It has a long history
 120                                          Generalizations of the Basic Multiresolution Wavelet System   Ch. 7

          1.5




          0.5




                                      1       2     3                 -2
                          (a) 灰7DF                                               (b) 或DF




         0.5-




        -0.5


                -2
                      -
                                          2   3     4                                           3
                          （이 玖 'DF                                               (d) 攻DF

Figure 7.17. Plots of Scaling Function and Wavelet and their Duals for one of the Cohen-
Daubechies-Feauveau Family of Biorthogonal Wavelets that is Used in the FBI Fingerprint Corn-
pression Standard




 [Mar92, Mar93, DM93, KS92, VH92, Donar], and has been systematically developed
                                                                                           recently
[Swe96a, Swe95]. The key idea is to build complicated biorthogonal systems using
                                                                                       simple and
invertible stages. The first stage does nothing but to separate even and odd samples, and it is
easily invertible. The structure is shown in Figure 7.18, and is called the lazy wavelet transform
in [Swe96a].




                                                                           \／玩
                      1, 1                                             1,1
                   1/2工 1/2                                -1/ 4, 1/2, 3/2, 1/2, -1/ 4
             3/8, 1, 3/4, 0, -1/8             3/64, 0, -3/16, 3/8, 41/32, 3/4, -3/ 16, -1/ 8, 3/64
       -1/ 16, 0, 9/16, 1, 9/16, 0, -1/ 16    -1/ 256, 0, 9/128, -1/16, -63/ 256, 9/16, 87/64, . . ·


Table 7.3. Coefficients for some Members of the Biorthogonal Coiflets. For Longer Filters, We
only List Half of the Coefficients.
Sec. 7.4. Biorthogonal Wavelet Systems                                                                121




                                               12   F_   _.   even니       丁


                              니     z
                                         니12
                                                    HH+ odd               12         汁




                               Figure 7.18. The Lazy Wavelet Transform


     After splitting the data into two parts, we can predict one part from the other, and keep
only the prediction error, as in Figure 7.19. We can reconstruct the data by recomputing the
prediction and then add back the prediction. In Figure 7.19, s and t are prediction filters.
    By concatenating simple stages, we can implement the forward and inverse wavelet transforms
as in Figure 7.20. It is also called the ladder structure, and the reason for the name is clear from
the figure. Clearly, the system is invertible, and thus biorthogonal. Moreover, it has been shown
the orthogonal wavelet systems can also be implemented using lifting [DS96a]. The advantages
of lifting are numerous:

   1Lifting steps can be calculated inplace. As seen in Figure 7.20, the prediction outputs based
     on one channel of the data can be added to or subtracted from the data in other channels,
     and the results can be saved in the same place in the second channel. No a山iliary memory
    is needed.

   1The predictors s and t do not have to be linear. Nonlinear operations like the medium
     filter or rounding can be used, and the system remains invertible. This allows a very simple
     generalization to nonlinear wavelet transform or nonlinear multiresolution analysis.

   0The design of biorthogonal systems boils down to the design of the predictors. This may
    lead to simple approaches that do not relay on the Fourier transform [Swe96a], and can be
    generalized to irregular samples or manifolds.

   . For biorthogonal systems, the lifting implementations require less numerical operations
     than direct implementations IDS96a1. For orthogonal cases, the lifting schemes have the
     computational complexity similar to the lattice factorizations, which is almost half of the
     direct implementation.



                           highpass                                              highpass

               -   s                                                  -   t

                            lowpass                                               lowpass

                       (a) The Lifting Step                               (b) The Dual Lifting Step

                            Figure 7.19. The Lifting and Dual Lifting Step
122                                             Generalizations of the Basic Multiresolution Wavelet System    Ch. 7



                    卜    2
                                                =1 '                  그1             그H
                                   寸 Si           -tl                   H 8m           m tm



            니   니       L2
                                                11 .      r           11H            7H小           卜l



                                 (a) The Forward Wavelet Transform using Lifting

                                                                                         12
                    그－U             口L- '                     그1           그1
                         tm               8m                  t1               Si                       나


                    벼1              그＋                                                     2
        니   K

                                 (b) The Inverse Wavelet Transform using Lifting

                               Figure 7.20. Wavelet Transform using Lifting




7.5 卜Au出wavelets
In Chapter 2, we introduced the multiresolution analysis for the space of L2 functions, where we
have a set of nesting subspaces

                              {O} c. ..cV_2cV_1cV0cV1cV2c...cL2,                                              (7.54)

where each subspace is spanned by translations of scaled versions of a single scaling function 99;
e.g.,
                                           vi = Span{2j'2Y7(2jt 中 k)}.                                        (7.55)
                                                  k

The direct difference between nesting subspaces are spanned by translations of a single wavelet
at the corresponding scale; e.g.,

                                 W3 = V3+1 e V, = Span{2j'2砂(23t - k)}.                                       (7.56)
                                                          k

There are several limitations of this construction. For example, nontrivial orthogonal wavelets can
not be symmetric. To avoid this problem, we generalized the basic construction, and introduced
multiplicity-M (M-band) scaling functions and wavelets in Section 7.2, where the difference
spaces are spanned by translations of M- 1 wavelets. The scaling is in terms of the power of M;
i.e.,
                                           'P3,k (t) = 凡rj/2y9（凡Pt - 丸）.                                      (7.57)

In general, there are more degrees of freedom to design the M-band wavelets. However, the nested
V spaces are still spanned by translations of a single scaling function. It is the multiwavelets that
Sec. 7.5. Multiwavelets                                                                          123


removes the above restriction, thus allowing multiple scaling functions to span the nested V spaces
tGLT93, GL94, Str96b]. Although it is possible to construct M-band multiwavelets, here we only
present results on the two-band case, as most of the researches in the literature do.

Construction of Two-Band Multiwavelets
Assume that V0 is spanned by translations of R different scaling functions 咤 (t), i = 1, . . . , R.
For a two-band system, we define the scaling and translation of these functions by

                                    (P,3,k (t) = 2j/2甲1(2jt - k).                               (7.58)

The multiresolution formulation implies

                                V3 = Span{ oi,3,k(t) : i = 1, . . . , R}.                       (7.59)
                                         k

We next construct a vector scaling function by

                                    令 (t) = [,l (t), . . . , R(t)]T.                            (7.60)

Since V0 C V1, we have

                                   吼）= 扼 >）回히갸 叫 n)                                             (7.61)


where H (k) is a R x R matrix for each k E Z. This is a matrix version of the scalar recursive
equation (2.13). The first and simplest multiscaling functions probably appear in [Alp93], and
they are shown in Figure 7.21.



                                     1


                                                 1卜
                                                      V／죵
                                         伽（t)               1 加（t)

                     Figure 7.21. The Simplest Alpert Multiscaling Functions


    The first scaling function 1(t) is nothing but the Haar scaling function, and it is the sum
of two time-compressed and shifted versions of itself, as shown in Figure 2.2(a). The second
scaling function can be easily decomposed into linear combinations of time-compressed and shifted
versions of the Haar scaling function and itself, as

                    加 = 똬 ,位）+ 如, (2t) 三，뇨小 1) +                            l mO
                                                                            m  二
                                                                                   甲
                                                                                   2
                                                                                       t    l
                                                                                       O二
                                                                                                (7.62)
                            二                二         {


This is shown in Figure 7.22
  124                                                         Generalizations of the Basic Multires히ution Wavelet System
                                                                                                                                   Ch. 7




                                      孕                                                          爭                          孕

                                                                                                      Li
                                                          1                                                             +

                                      孕                                                  1
                                                                                             李                              孕

                        Figure 7.22. Multiwavelet Refinement Equation (7.62)


     Putting the two scaling functions together we have

          1r 四l (t) 1   1 1            0 1I 1I 四l (2t) 1 , 1     1                            0 1I Ir 四1(2t - 1) 1
                ; ( 1 = 1 /=
            '   1


                                                     (
                                      1/ 2 ] . 甲2(2t) j1 + [1 -v '3/
                                          ,   八       '   1



          L p2(t) J     [ v'3/ 2                                                             1/ 2 i L 甲2(2t - 1)( ]!            (7.63)
                                                                                                       '   4
                              .
                                                                 /=
                                  八   m
                    .
                                                                    .


                                                                     2
                                                                                 .   八       .   ／八
                                                              ),1
                                                                                                               ）八
                                                                                                                    .       .




    Further assume R wavelets span the difference spaces
                                                                                 ; i.e.,
                            W3 = V3+1 e V3 = Span{吻,3,k (t) : i = 1, . . . , R}.
                                                                                                                                (7.64)
                                                                        k
 Since W0 C V1 for the stacked wavelets W(t) there must
                                                        exist a sequence of R x R matrices C(k),
 such that
                                                  W(t) = \／百 >二C(k) m(2t -k)                                                    (7.65)
                                                                        k
 These are vector versions of the two scale recursive
                                                      equations (2.13) and (2.24).
    We can also define the discrete-time Fourier transform
                                                             of H (k) and G(k) as

                           H(U) =＞二H（丸）e"k,                                 G(四) =＞二C（凡）e" 「·
                                                                                           工                                    (7.66)
                                              k                                          k

Properties of Multiwavelets
Approximation, Regularity and Smoothness
Recall from Chapter 6 that the key to regularity and
                                                         smoothness is having enough number
of zeros at ir for H (w). For multiwavelets, it
                                                 has been shown that polynomials can be ex-
actly reproduced by translates of 令 (t) if and only if
                                                        H (w) can be factored in special form
[Plo95c, Plo95a, P1o95b]. The factorization is
                                                 used to study the regularity and convergence
of refinable function vectors [CDP9S], and to
                                              construct multi-scaling functions with approxima-
tion and symmetry [PS95] . Approximation and smoothness
                                                             of multiple refinable functions are
also studied in [HSS96, JRZ96a, JRZ97J.

Support
In general, the finite length of H (k) and C(k) ensure the finite
                                                                  support of m(t) and 山(t). However,
there are no straightforward relations between the suppo
                                                              rt length and the number of nonzero
Sec. 75. Mu比iwavelets                                                                           125


coefficients in H (k) and G(k). An explanation is the existence of nilpotent matrices [SW97]. A
method to estimate the support is developed in [SW97].

Orthogonality
For these scaling functions and wavelets to be orthogonal to each other and orthogonal to their
translations, we need [SS95]

                             H（미甘回 + H佃 + ir)Ht (w + ir) = IR,                                 (7.67)

                             G(w)G十（w) + G(w + ir)G卞（(4) + 미 = JR,                             (7.68)

                            H (U)Gt (w) + H (w + ir)Gt (w + 미 = 0R,                            (7.69)

where f denotes the complex conjugate transpose, JR and 0R are the R x R identity and zero
matrix respectively. These are the matrix versions of (5.22) and (5.30). In the scalar case, (5.30)
can be easily satisfied if we choose the wavelet filter by time-reversing the scaling filter and
changing the signs of every other coefficients. However, for the matrix case here, since matrices
do not commute in general, we cannot derive the G(k)'s from H (k)'s so straightforwardly. This
presents some difficulty in finding the wavelets from the scaling functions; however, this also gives
us flexibility to design different wavelets even if the scaling functions are fixed [SS95].
    The conditions in (7.67-7.69) are necessary but not sufficient. Generalization of Lawton's
sufficient condition (Theorem 14 in Chapter 5) has been developed in [Plo97b, Plo97a, JRZ96b].

Im미帥犯ntat油n of M비山／avelet Transform
Let the expansion coefficients of multiscaling functions and multiwavelets be

                                       c2,3 (k) = (f (t),coi,3,k (t)),                         (7.70)

                                       di,j (k) = (f (t),砂i,j,k (t)) .                         (7.71)

We create vectors by
                                    C3(k) = [ci,j (k),. . . ,CR,J (k)IT,                       (7.72)

                                    D3(k) = [d1,3 (k),. . . ,dR.J(k)]T.                        (7.73)

For f (t) in Vo, it can be written as linear combinations of scaling functions and wavelets,
                                                           X)


                        f(t) = Z C3。(k)也小）4二 Z긔硏'I',,嗣·                                        (7.74)
                                丸                         j= jo   k

Using (7.61) and (7.65), we have

                               （午嗣 = 扼Zm加冊 + n)                                                化75)


and
                                까고劤 = 'I吟그枷）ci마＋ri).                                           (7.76)
126                                      Generalizations of the Basic Multiresolution Wavelet System   Ch. 7


                                                               =14H=   +
                                              H     (-    n)
                                                               HHH＝    나
                                                                           12   r11+   口   '   (k)
                 q休）
                                                               H
                                               G   (-    n)
                                                                                       D3_1(k)

                                       (a) Forward Transform



               C3_i (k)


                                                                                       ci（丸）


              D741（丸）


                                        (b) Inverse Transform

                          Figure 7.23. Discrete Multiwavelet Transform



Moreover,
                  ci써 키厄Z 回劤k孕巾硏 미 + G恂切尸但k +네 ·                                                       化77)
                                k

These are the vector forms of (3.9), (3.10), and (3.20). Thus the synthesis and analysis filter
banks for multiwavelet transforms have similar structures as the scalar case. The difference is
that the filter banks operate on blocks of R inputs and the filtering and rate-changing are all
done in terms of blocks of inputs.
    To start the multiwavelet transform, we need to get the scaling coefficients at high resolution.
Recall that in the scalar case, the scaling functions are close to delta functions at very high
resolution, so the samples of the function are used as the scaling coefficients. However, for multi-
wavelets we need the expansion coefficients for R scaling functions. Simply using nearby samples
as the scaling coefficients is a bad choice. Data samples need to be preprocessed (prefiltered) to
produce reasonable values of the expansion coefficients for multi-scaling function at the highest
scale. Prefilters have been designed based on interpolation [XGHS9G], approximation [HR96],
and orthogonal projection [VA961.

Examples
Because of the larger degree of freedom, many methods for constructing multiwavelets have been
developed.

Geronimo-Hardin-Massopust Multiwavelets
A set of multiscaling filters based on fractal interpolation functions were developed in [GHM94],
and the corresponding multiwavelets were constructed in [5S95]. As shown in Figure 7.24, they
Sec. 7.5. Multiwavelets
                                                                                             127


         3                                           3

        2.5                                         2.5-

          2   ,
                                                      2

        1.5                                         1.5

          1-                                          1

        0.5 ,                                       0.5r

          0                                           0

       -0.5-                                       -0.5


         _10        0.5       1     1.5       2                0.5               1.5

                          (a) pi




                          （이 砂l                                      (d) 砂2


 Figure 7.24.       Geronimo-Hardin-Massopust Multi-scaling Function and Strang-Strela Multi-
 砥／avelets


 are both symmetrical and orthogonal-a combination which is impossible for tw아band orthogonal
 scalar wavelets. They also have short support, and can exactly reproduce the hat function. These
 interesting properties make multiwavelet a promising expansion system.


 Spline Multiwavelets
 Spline bases have a maximal approximation order with respect to their length, however spline
 uniwavelets are only semiorthogonal [SS94J. A family of spline multiwavelets that are symmetric
 and orthogonal is developed in [RN961.


 Other Constructions
 Other types of multiwavelets are constructed using Hermite interpolating conditions [CL96],
 matrix spectral factorization [CNKS96], finite elements [SS94], and oblique projections [Ald96].
 Similar to multiwavelets, vector-valued wavelets and vector filter banks are also developed [XS96].
 128                                       Generalizations of the Bas七 Mu出resolution Wavelet System   Ch. 7


 Applications
Multiwavelets have been used in data compression [HSS*95, LLK96, SHS*96], noise reduction
 [DS96b, SHS*96}, and solution of integral equations [CMX96I. Because multiwavelets are able to
offer a combination of orthogonality, symmetry, higher order of approximation and short support,
methods using multiwavelets frequently outperform those using the comparable scale wavelets.
However, it is found that prefiltering is very important, and should be chosen carefully for the
applications [DS96b, SHS*96, XGHS96J. Also, since discrete multiwavelet transforms operate
on size-R blocks of data and generate blocks of wavelet coefficients, the correlation within each
block of coefficients needs to be exploited. For image compression, predictions rules are proposed
to exploit the correlation in order to reduce the bit rate [LLK96]. For noise reduction, joint
thresholding coefficients within each block improve the performance [DS96b}.


7.6    Overcomplete Representations, Frames, Redundant Transforms, and
       Adaptive Bases

In this chapter, we apply the ideas of frames and tight frames introduced in Chapter 4 as well
 as bases to obtain a more efficient representation of many interesting signal classes. It might be
helpful to review the material on bases and frames in that chapter while reading this section.
     Traditional basis systems such as Fourier, Gabor, wavelet, and wave packets are efficient
representations for certain classes of signals, but there are many cases where a single system is
not effective. For example, the Fourier basis is an efficient system for sinusoidal or smooth periodic
signals, but poor for transient or chirp-like signals. Each system seems to be best for a rather
well-defined but narrow class of signals. Recent research indicates that significant improvements
in efficiency can be achieved by combining several basis systems. One can intuitively imagine
removing Fourier components until the expansion coefficients quit dropping off rapidly, then
switching to a different basis system to expand the residual and, after that expansion quits
dropping off rapidly, switching to still another. Clearly, this is not a unique expansion because the
order of expansion system used would give different results. This is because the total expansion
system is a linear combination of the individual basis systems and is, therefore, not a basis itself
but a frame. It is an overcomplete expansion system and a variety of criteria have been developed
to use the freedom of the nonuniqueness of the expansion to 缸lvantage. The collection of basis
systems from which a subset of expansion vectors is chosen is sometimes called a dictionary.
    There are at least two descriptions of the problem. We may want a single expansion system
to handle several different classes of signals, each of which are well-represented by a particular
basis system or we may have a single class of signals, but the elements of that class are linear
combinations of members of the well-represented classes. In either case, there are several criteria
that have been identified as important [CD94, CD95a]:

   . Sparsity: The expansion should have most of the important information in the smallest
     number of coefficients so that the others are small enough to be neglected or set equal to
     zero. This is important for compression and denoising.

   1 Separation: If the measurement consists of a linear combination of signals with different
     characteristics, the expansion coefficients should clearly separate those signals. If a single
     signal has several features of interest, the expansion should clearly separate those features.
     This is important for filtering and detection.
 Sec. 7.6. Overcomplete Representations, Frames, Redundant Transforms, and Adaptive Bases             129

    1Superresolution: The resolution of signals or characteristics of a signal should be much
      better than with a traditional basis system. This is likewise important for linear filtering,
      detection, and estimation.

    eStability: The expansions in terms of our new overcomplete systems should not be signif-
     icantly changed by perturbations or noise. This is important in implementation and data
     measurement.

    1Speed: The numerical calculation of the expansion coefficients in the new overcomplete
      system should be of order O(N) or O(Nlog(N) ).

   These criteria are often in conflict with each other, and various compromises will be made in
the algorithms and problem formulations for an acceptable balance.


Overcomplete Representations
This section uses the material in Chapter 4 on bases and frames. One goal is to represent
                                                                                          a signal
using a "dictionary" of expansion functions that could include the Fourier basis, wavelet basis,
Gabor basis, etc. We formulate a finite dimensional version of this problem as


                                     y(n) =＞二akxk (n)                        n小EZ                   (7.78)
                                                 丸

for n = 0, 1, 2, · · · ,N -1 and k = 0, L 2, · · · , 7( -1. This can be written in matrix form as

                                                      y= Xa                                     (7.79)

where y is a N x 1 vector with elements being the signal values y(n), the matrix X is N
                                                                                                xK
the columns of which are made up of all the functions in the dictionary and a is a K x 1 vector
of the expansion coefficients ak. The matrix operator has the basis signals xk as its columns so
that the matrix multiplication (7.79) is sim1lply the signal expansion (7.78).
    For a given signal representation problem, one has two decisions: what dictionary to use (i.e.,
choice of the X) and how to represent the signal in terms of this dictionary (i.e., choice
                                                                                              of a).
Since the dictionary is overcomplete, there are several possible choices of a and typically
                                                                                            one uses
prior knowledge or one or more of the desired properties we saw earlier to calculate the a.


A Matrix Example
Consider a simple two-dimensional system with orthogonal basis vectors

                                    !1=
                                    xi=
                                            [1
                                           [。]
                                                          and 12:            [?
                                                                                  ]             (7.80)

which gives the matrix operator with x1 and x2 as columns

                                                          I i    01
                                                 入   ＝二   1                                     (7.81)
                                                          L U    l J
                                                            ,\   4   1
                                                                         .
                                                                      Generalizations of the Basic Multiresolut向n Wavelet System                                                                   Ch. 7
130


                                                                                                first
Decomposition with this rather trivial operator gives a time-domain description in that the
                                                                                second coefficient is
expansion coefficient a0 is simply the first value of the signal, x(0), and the
the second value of the signal. Using a different set of basis vectors might give the  operator


                                                                                                                 0.7071 1
                                                                                                                                          ]
                                                                           r 0.7071
                                                             入
                                                                 =         L 70710.
                                                                                                             -
                                                                                                                 0.
                                                                                                                   7071
                                                                                                                                                                                                  (7.82)



which has the normalized basis vectors still orthogonal but now at a 45O angle from the basis
vectors in (7.81). This decomposition is a sort of frequency domain expansion. The first column
vector will simply be the constant signal, and its expansion coefficient a(0) will be the average
of the signal. The coefficient of the second vector will calculate the difference in y(O) and y(l)
and, therefore, be a measure of the change.
             that y
       ，야1.6 (5毗  7 =
                                   =
                                        [ j       can   be
                                                              represented exactly with only one nonzero coefficient using



                                                                                                                      [ 小如posite
                                        Ii]
        Notice
(7.
        81小蜘蜘如叫7.
signals y =
                                                             82) , while
                                                              can          be
                                                                                           for
                                                                                      represented
                                                                                                            y=
                                                                                                                       sparsely
                                                                                                                                                 by   (7.
                                                                                                                                                               is
                                                                                                                                                             81)            while
                                                                                                                                                                                         y =   [ ]
                                                                                                                                                                                    true. This means the

                                                                                                                                                                                                     and

                 F
         1 I can be represented sparsely by (7.82).
                          ii
y=               I
     I -' J
   If we create an overcomplete expansion by a linear combination of the previous orthogonal
basis systems, then it should be possible to have a sparse representation for all four of the previous
signals. This is done by simply adding the columns of (7.82) to those of (7.81) to give

                                                                 Ii                   0          0.7071                           0.7071 1
                                                       入=        I                                                                                1                                               (7.83)
                                                                                                                      -U. (U (I                  j
                                                                      -.                         ,\   느八md                        ,\   .m』＼.m1


                                                                 L U                  I          U. (U(I


      This is clearly overcomplete, having four expansion vectors in a tw아dimensional system. Finding
      ak requires solving a set of underdetermined equations, and the solution is not unique.
         For example, if the signal is given by


                                                                                          y=
                                                                                                      Iii
                                                                                                      I r) 1
                                                                                                                                                                                                  (7.84)
                                                                                                      LUJ


      there are an infinity of solutions, several of which are listed in the following table.


                                                   2         3                       4                            5                           6
                                                                                                                                                                    m
                     Case           1
                                                                                                                                                                    00
                                                                                                                                                                        /
                     a0        0.5000         1.0000    1.0000                  1.0000                            0                           0
                 （보1           0.0000         0.0000         0                       0                      -1.0000                      1.0000
                               0.3536              0    0.0000                       0                       1.4142                           0             0.7071
                     a2
                     a3        0.3536              0         0                  0.0000                            0                      1.4142             0.7071


                     小네2       0.5000         1.0000    1.0000                  1.0000                       3.0000                       3.0000            1.0000
Sec. 7.6. Overcomplete Representations, Frames, Redundant Transforms, and Adaptive Bases     131


   Case 1 is the minimum norm solution of y = X上 for ak. It is calculated by a pseudo inverse
with the MATLAB command a = pinv (X) *y . It is also the redundant DWT discussed in the
next section and calculated by a = X ' *y/2. Case 2 is the minimum norm solution, but for no
more than two nonzero values of ak. Case 2 can also be calculated by inverting the matrix (7.83)
with columns 3 and 4 deleted. Case 3 is calculated the same way with columns 2 and 4 deleted,
case 4 has columns 2 and 3 deleted, case 5 has 1 and 4 deleted, case 6 has 1 and 3 deleted, and
case 7 has 1 and 2 deleted. Cases 3 through 7 are unique since the reduced matrix is square and
nonsingular. The second term of a for case 1 is zero because the signal is orthogonal to that
expansion vector. Notice that the norm of a is minimum for case 1 and is equal to the norm of
y divided by the redundancy, here two. Also notice that the coefficients in cases 2, 3, and 4 are
the same even though calculated by different methods.
   Because X is not only a frame, but a tight frame with a redundancy of two, the energy (norm
squared) of a is one-half the norm squared of y. The other decompositions (not tight frame or
basis) do not preserve the energy.
   Next consider a two-dimensional signal that cannot be exactly represented by only one ex-
pansion vector. If the unity norm signal is given by

                                                    1 0.9806 1
                                             y=     L 1961
                                                       0.        .1
                                                                                            (7.85)

the expansion coefficients are listed next for the same cases described previously.


                                                                                     口
                                                                                     r
     Case          1         2          3          4              5        6
                                                                                     0
     a0       0.4903    0.9806     0.7845     1.1767              0        0
     a1       0.0981    0.1961          0          0        -0.7845   1.1767        0
     a2       0.4160         0     0.2774          0         1.3868        0   0.8321
     a3       0.2774         0          0    -0.2774              0   1.3868   0.5547

     II에2     0.5000     1.0000    0.6923     1.4615        2.5385    3.3077   1.0000


    Again, case 1 is the minimum norm solution; however, it has no zero components this time
because there are no expansion vectors orthogonal to the signal. Since the signal lies between the
900 and 450 expansion vectors, it is case 3 which has the least two-vector energy representation.
    There are an infinite variety of ways to construct the overcomplete frame matrix X. The
one in this example is a four-vector tight frame. Each vector is 450 degrees apart from nearby
vectors. Thus they are evenly distributed in the 180t) upper plane of the two dimensional space.
The lower plane is covered by the negative of these frame vectors. A three-vector tight frame
would have three columns, each 600 from each other in the tw아dime瑁ion plane. A 36-vector
tight frame would have 36 columns spaced 50 from each other. In that system, any signal vector
would be very close to an expansion vector.
    Still another alternative would be to construct a frame (not tight) with nonorthogonal rows.
This would result in columns that are not evenly spaced but might better describe some particular
class of signals. Indeed, one can imagine constructing a frame operator with closely spaced
expansion vectors in the regions where signals are most likely to occur or where they have the
most energy.
132                                         Generalizations of the Basic Multiresolution Wavelet System    Ch. 7


  We next consider a particular modified tight frame constructed so as to give a shift-invariant
DWT.



Shift-Invariant Redundant Wavelet Transforms and Nondecimated Filter Banks
One of the few flaws in the various wavelet basis decompositions and wavelet transforms is the fact
the DWT is not translation-invariant. If you shift a signal, you would like the DWT coefficients
to simply shift, but it does more than that. It significantly changes character.
   Imagine a DWT of a signal that is a wavelet itself. For example, if the signal were


                                           y（미 = 甲(24n中 10)                                               (7.86)


then the DWT would be


                             d4(10) = 1      all other d3 (k) = c(k) = 0.


In other words, the series expansion in the orthogonal wavelet basis would have only one nonzero
coefficient.
    If we shifted the signal to the right so that y(n) = p(24(n - 1) - 10), there would be many
nonzero coefficients because at this shift or translation, the signal is no longer orthogonal to
most of the basis functions. The signal energy would be partitioned over many more coefficients
and, therefore, because of Parseval's theorem, be smaller. This would degrade any denoising or
compressions using thresholding schemes. The DWT described in Chapter 9 is periodic in that
at each scale j the periodized DWT repeats itself after a shift of n = 27, but the period depends
on the scale. This can also be seen from the filter bank calculation of the DWT where each scale
goes through a different number of decimators and therefore has a different aliasing.
    A method to create a linear, shift-invariant DWT is to construct a frame from the orthogonal
DWT supplemented by shifted orthogonal DWTs using the ideas from1l the previous section. If
you do this, the result is a frame and, because of the redundancy, is called the redundant DWT
or RDWT.
    The typical wavelet based signal processing framework consists of the following three simple
steps, 1) wavelet transform; 2) point-by-point processing of the wavelet coefficients (e.g. thresh-
olding for denoising, quantization for compression); 3) inverse wavelet transform. The diagram
of the framework is shown in Figure 7.25. As mentioned before, the wavelet transform is not
translation-invariant, so if we shift the signal, perform the above processing, and shift the output
back, then the results are different for different shifts. Since the frame vectors of the RDWT
 consist of the shifted orthogonal DWT basis, if we replace the forward/inverse wavelet transform



                             D砥／T     1H
                                                    스        H        II）砥丁       H




Figure 7.25. The Typical Wavelet Transform Based Signal Processing 까amework (스 denotes
the pointwise processing)
                                                                                  Bases   ,   133
Sec 7.6. Overcomplete Representations, Frames, Redundant Transforms, and Adaptive



                      H       RDWT        H日＝   卄
                                                      스      H       IRDWT


Figure 7.26. The Typical Redundant Wavelet Transform Based Signal Processing Framework
(스 denotes the pointwise processing)


in the above framework by the forward/inverse RDWT, then the result of the scheme in Fig-
ure 7.26 is the same as the average of all the processing results using DWTs with different shifts
of the input data. This is one of the main reasons that RDWT-based signal processing tends to
be more robust.
   Still another view of this new transform can be had by looking at the Mallat-derived filter
bank described in Chapters 5 and 8. The DWT filter banks illustrated in Figures 3.3 and 3.6
                                                                                              the
can be modified by removing the decimators between each stage to give the coefficients of
                                                                          the undecimate d filter
tight frame expansion (the RDWT) of the signal. We call this structure
bank. Notice that, without the decimation, the number of terms in the DWT is larger than
                                                                                                 is
N. However, since these are the expansion coefficients in our new overcomplete frame, that
consistent. Also, notice that this idea can be applied to M-band wavelets and wavelet packets   in
the same way.
     These RDWTs are not precisely a tight frame because each scale has a different redundancy.
However, except for this factor, the RDWT and undecimated filter have the same characteristics
of a tight frame and, they support a form of Parseval's theorem or energy partitioning.
     If we use this modified tight frame as a dictionary to choose a particular subset of expansion
vectors as a new frame or basis, we can tailor the system to the signal or signal class. This is
discussed in the next section on adaptive systems.
     This idea of RDWT was suggested by Mallat [Ma191], Beylkin [Bey92], Shensa [She92}, Du-
tilleux [Dut891, Nason [NS95}, Guo [Guo94, Guo951, Coifman, and others. This redundancy
comes at a price of the new RDWT having O(N log(N)) arithmetic complexity rather than
                                                                                              Weiss
O(N). Liang and Parks [LP94b, LP94a], Bao and Erdol 1BE94, BE93}, Marco and
 [MW.T94. MW94h. MW94a], Dauhechies [Dau921. and others 1PKC961              have  used  someform
 of averaging or "best basis" transform to obtain shift invariance.
      Recent results indicate this nondecimated DWT, together with thresholding, may be the best
 denoising strategy [DJKP95b, DJKP95a, LGO*95, CD95b, LGOB9S, GLOB9S, LGO*96, Guo95].
 The nondecimated DWT is shift invariant, is less affected by noise, quantization, and error, and
 has order Nlog(N) storage and arithmetic complexity. It combines with thresholding to give
 denoising and compression superior to the classical Donoho method for many examples. Further
 discussion of use of the RDWT can be found in Section 10.3.

 Adaptive Construction of Frames and Bases
 In the case of the redundant discrete wavelet transform just described, an overcomplete expansion
 system was constructed in such a way as to be a tight frame. This allowed a single linear shift-
 invariant system to describe a very wide set of signals, however, the description was adapted
 to the characteristics of the signal. Recent research has been quite successful in constructing
 expansion systems adaptively so as to give high sparsity and superresolution but at a cost of
 added computation and being nonlinear. This section will look at some of the recent results in
  this area [MZ93, DJ94a, CD94, CD95a].
 134                                       Generalizations of the Basic Multiresolution Wavelet System   Ch. 7


    While use of an adaptive paradigm results in a shift-invariant orthogonal transform, it is
nonlinear. It has the property of DWT{a f (x)} = a DWT{f (x)}, but it does not satisfy su-
perposition, i.e. DWT{ 1 (x) + g(x)} 7E DWT{f (x)} + DWT{g(x) }. That can sometimes be a
problem.
   Since these finite dimensional overcomplete systems are a frame, a subset of the expansion
vectors can be chosen to be a basis while keeping most of the desirable properties of the frame.
This is described well by Chen and Donoho in [CD94, CD95a}. Several of these methods are
outlined as follows:

      . The method of fr缸1les (MOF) was first described by Daubechies [Dau88b, Dau90, Dau921
        and uses the rather straightforward idea of solving the overcomplete frame (underdeter-
        mined set of equations) in (7.83) by minimizing the L2 norm of a. Indeed, this is one of
        the classical definitions of solving the normal equations or use of a pseud아inverse. That
        can easily be done in MATLAB by a = play (X) *y. This gives a frame solution, but it is
        usually not sparse.

    . The best orthogonal basis method (BOB) was proposed by Coifman and Wickerhauser
      [CW92, DJ94a] to adaptively choose a best basis from a large collection. The method is
      fast (order N log N) but not necessarily sparse.

   1Mallat and Zhang [MZ93] proposed a sequential selection scheme called matching pursuit
    (MP) which builds a basis, vector by vector. The efficiency of the algorithm depends on
    the order in which vectors are added. If poor choices are made early, it takes many terms
    to correct them. Typically this method also does not give sparse representations.

    . A method called basis pursuit (BP) was proposed by Chen and Donoho [CD94, CD95a]
      which solves (7.83) while minimizing the L' norm of a. This is done by linear programmin
                                                                                                    g
      and results in a globally optimal solution. It is similar in philosophy to the MOFs but uses an
      L1 norm rather than an L2 norm and uses linear programming to obtain the optimization.
      Using interior point methods, it is reasonably efficient and usually gives a fairly sparse
      solution.

   . Krim et al. describe a best basis method in [KMDW95]. Tewfik et al. propose a method
     called optimal subset selection in [NAT96] and others are [BM95, Cro96].

  All of these methods are very signal and problem dependent and, in some cases, can give
much better results than the standard M-band or wavelet packet based methods.


7.7     Local Trigonometric Bases

In the material up to this point, all of the expansion systems have required the tra嶝lation and
scaling properties of (1.5) and the satisfaction of the multiresolution analysis assu叩tion of (2.13).
까om this we have been able to generate orthogonal basis systems with the basis functions having
compact support and, through generalization to M-band wavelets and wavelet packets, we have
been able to allow a rather general tiling of the time-frequency or time-scale plane with flexible
丘equency res아uti이1.
   By giving up the multiresolution analysis (MRA) requirement, we will be able to create
another basis system with a time-frequency tiling somewhat the dual of the wavelet or wavelet
Sec. 7.7.   Local Trigonometric Bases                                                          135


packet system. Much as we saw the multiresolution system dividing the frequency bands in a
logarithmic spacing for the M = 2 systems and a linear spacing for the higher M case, and
a rather general form for the wavelet packets, we will now develop the loc工l cosine and loc口l
sine basis systems for a more flexible time se앉llenting of the time-frequency plane. Rather than
modifying the MRA systems by creating the time-varying wavelet systems, we will abandon the
入4RA and build a ba駁S 小rectly.
   What we are looking for is an expansion of a signal or f끄lction in the form

                                                1(t) = 二 a,,(n) xk,.(t),                     (7.88)
                                                               k,n

where the functions xj,k (t) are of the form (for example)

                                       xk.n(t) = Wk(t) cos(air(n + fl)t + y).                (7.89)

Here wk (t) is a window function giving localization to the basis function and c, 3 and y are
constants the choice of which we will get to shortly. k is a time index while n is a frequency
index. By requiring orthogonality of these basis functions, the coefficients (the transform) are
found by an inner product

                                                                                             (7.90)
                                 ak   (n)   =   (f(t)   ,xk,    小))   =   ff   (t) 小) dt.
                                                                                 xk，
We will now examine how this can be achieved and what the properties of the expansion are.
    Fundamentally, the wavelet packet system decomposes L2(正t) into a direct sum of orthogonal
spaces, each typically covering a certain frequency band and spanned by the translates of a
particular element of the wavelet packet system. With wavelet packets time-frequency tiling with
flexible frequency resolution is possible. However, the temporal resolution is determined by the
frequency band associated with a particular element in the packet.
    Local trigonometric bases [Wic95, AWW92] are duals of wavelet packets in the sense that
these bases give flexible temporal resolution. In this case, L2 (正t) is decomposed into a direct sum
of spaces each typically covering a particular time interval. The basis functions are all modulates
of a 且Xed window function.
    One could argue that an obvious approach is to partition the time axis into di如int bins
and use a Fourier series expansion in each temporal bin. However, since the basis functions are
 "rectangular-windowed" exponentials they are discontinuous at the bin boundaries and hence
undesirable in the analysis of smooth signals. If one replaces the rectangular window with a
"smooth" window, then, since products of smooth functions are smooth, one can generate smooth
windowed exponential basis functions. For example, if the time axis is split uniformly, one is
looki叩 at basis functions of the form 如巾 나）et2元nt } 小，n E Z for some smooth window 如iction
w(t). Unfortunately, orthonormality disallows the function w(t) from being well-concentrated in
time or in frequency - which is undesirable for time frequency analysis. More precisely, the
Balian-Low theorem (see p.108 in [Dau92]) states that the Heisenberg product of g (the product
of the tim1le-spread and frequency-spread which is lower bounded by the Heisenberg uncertainty
principle) is infinite. However, it turns out that windowed trigonometric bases (that use cosines
and sines but not exponentials) can be orthonormal, and the window can have a finite Heisenberg
product [DJJ]. That is the reason why we are looking for local trigonometric bases of the form
given in (7.89).
136                                                           Generalizations of the Basic Multires이ution Wavelet System            Ch. 7


Nonsmooth Local Trigonometric Bases
To construct local trigonometric bases we have to choose: (a) the window functions wk (t); and
(b) the trigonometric functions (i.e., a, fi and -y in Eq. 7.89). If we use the rectangular window
(which we know is a bad choice), then it suffices to find a trigonometric basis for the interval
that the window spans. Without loss of generality, we could consider the unit interval (0, 1) and
hence we are interested in trigonometric bases for L2((0, 1)). It is easy to see that the following
four sets of functions satisfy this requirement.

          1· 如小）} = {\／牙cos（冗（n + 枷）}, nE {0, 1. 2, . . .};

          2· 如小）} = {V吼i小(n + 枷小 n e {0, 1, 2. . . .};

          3. 如小）} = {i, \／프cos（兀7it) },n E {1, 2, . . .}:

          4. {九(t)} = {.../易sin(irnt)}, n E {0. 1. 2, . . .}.

   Indeed, these orthonormal bases are obtained from the Fourier series on (- 2, 2) (the first
two) and on (- 1, 1) (the last two) by appropriately imposing symmetries and hence are readily
verified to be complete and orthonormal on (0, 1). If we choose a set of nonoverlapping rectangular
window functions Wk (t) such that >k Wk(t) = 1 for all t e 正. and define Xk.n(t) = 2iJk（加，     ,(t),
then, {xk,fl(t)} is a local trigonometric basis for L2(丑), for each of the four choices of phi,,(t)
above.

Construction of Smooth Windows
We know how to construct orthonormal trigonometric bases for disjoint temporal bins or intervals.
Now we need to construct smooth windows Wk (t) that when applied to cosines and sines retain
orthonormality. An outline of the process is as follows: A unitary operation is applied that
"unfolds" the discontinuities of all the local basis functions at the boundaries of each temporal bin.
Unfolding leads to overlapping (unfolded) basis functions. However, since unfolding is unitary,
the resulting functions still form an orthonormal basis. The unfolding operator is parameterized
by a function r (t) that satisfies an algebraic constraint (which makes the operator unitary). The
smoothness of the resulting basis functions depends on the smoothness of this underlying function
r   (t)    .




   The function r (t), referred to as a rising cutoff function. satisfies the following conditions (see
Fig. 7.27) :

                                                                                                               JL +L
                                                                                                                               l
                                                                                          .. .
                                                                                                                           中




                       Ir(t)I2 +1r (- t)12 = 1,              for all t E IR:                                               l       (7.91)
                                                                                         Utt) = l 1.
                                                                                                               rl n
                                                                                                                  f1
                                                                                                     10,
r (t) is called a rising cutoff function because it rises from 0 to 1 in the interval [-1, 1] (note: it does
not necessarily have to be monotone increasing). Multiplying a function by r(t) would localize it
to [-1, 的j. Every real-valued function r (t) satisfying (7.91) is of the form r (t) = sin(8(t)) where


                         9   (t)   +9   (1   t)   =   즐   for all t E IR;      r   (t)    =      {   O 즈
                                                                                                       2
                                                                                                           f
                                                                                                           r
                                                                                                           1
                                                                                                               U
                                                                                                               +

                                                                                                               L
                                                                                                               +
                                                                                                                       H




                                                                                                                       L
                                                                                                                           L
                                                                                                                                   (7.92)
Sec. 7.7. Local Trigonometric Bases                                                                                   137

This ensures that r (- t) = sin(9(- t)) = sin(즐 -9(t)) = cos(9(t)) and therefore r2(t) +r2(- t) = 1.
One can easily construct arbitrarily smooth rising cutoff functions. We give one such recipe from
[Wic95] (p.105) . Start with a function

                                      .   r        0)          .   .           .         .          if t < 1
                              r［이（t) = 1 sin（즐（1 +t) )                                              if 卄1 ＜二 t < 1   (7.93)
                                          (        1,                                               if t> 1

It is readily verified to be a rising cutoff function. Now recursively define r[11(t), r[21(t), . . . as
白ilows:
白nOWS:
                                                                                                (7.94)
                                          「   ［.   ［미
                                                    +n   (t)  ).       ＝   『       （8m       （즐t)
Notice that r1n1(t) is a rising cutoff function for every n. Moreover, by induction on n it is easy
to show that r[,;](t) E C2" H1 (it suffices to show that derivatives at t = -1 and t = 1 exist and
are zero up to order 27l - 1).

Folding and Unfolding
Using a rising cutoff function r (t) one can define the folding operator, U, and its inverse, the
unfolding operator U士 as follows:


                            U(r)f小｛窄섟社珊二t),t), !｛亡0。
                        「'（「）/(!)={ 窄섟，;:（崙｝(-t), !::>0<。
Notice that U*(r)U(r)f (t) = (Ir(t)I2 + jr(- t)I2)f (t) = U(r)U*(r)f (t) and that IIU(r)f II = I1f II =
  U*(r)f II showing that U(r) is a unitary operator on L2(표t). Also these operators change 1 (t)
only in [-1, 11 since U(r)f (t) = f (t) = U*(r)f (t) for t 5 -1 and t 之 1. The interval [-1, 11 is the
action region of the folding/unfolding operator. U(r) is called a folding operator acting at zero
because for smooth f, U(r)f has a discontinuity at zero. By translation and dilation of r (t) one
can define U(r, t0, e) and U*(r, to, e) that folds and unfolds respectively about t = to with action
reg幻n [t0 - E, to +日 and act切nr口dil工S C.
    Notice (7.95) and (7.96) do not define the value U(r)f (0) and U*(r)f (0) because of the dis-
continuity that is potentially introduced. An elementary exercise in calculus divulges the nature
of this discontinuity. 1ff E Cd(IR), then U(r)f E Cd(正｛\ {0}). At t = 0, left and right derivatives
exist with all even-order left-derivatives and all odd order right-derivatives (upto and including
d) being zero. Conversely, given any function f e Cd(皿\ {0}) which has a discontinuity of the
above type, U*(r)f has a unique extension across t = 0 (i.e., a choice of value for (U*(r)f)(0))
that is in Cd(正t). One can switch the signs in (7.95) and (7.96) to obtain another set of folding
and unfolding operators. In this case, for f E Cd (IR). U(r)f will have its even-order right deriva-
tives and odd-order left derivatives equal to zero. We will use U. 나 and U_ , U, respectively
to distinguish between the two types of folding/unfolding operators and call them positive and
negative polarity folding/unfolding operators respectively.
    So far we have seen that the folding operator is associated with a rising cutoff function, acts
at a certain point, has a certain action region and radius and has a certain polarity. To get a
qualitative idea of what these operators do, let us look at some examples.
138                                       Generalizations of the Basic Multiresolution Wavelet System    Ch. 7


   First, consider a case where f (t) is even- or-odd symmetric about the folding point on the
action interval. Then, Uf corresponds to simply windowing f by an appropriate window function.
Indeed, if f (t) = f (- t) on [-1, 1],



                        U+(r,0,1)1(t):{ 압玄上3}{3:                      if t > 0,
                                                                       if t <0,
                                                                                                        (7.97)


and if f (t) = -f (- t) on [-1, 1]



                        U+(r,0,1)1(t)={ 압勻上杉：}
                                                                      if t >0,
                                                                                                        (7.98)
                                                                      if t <0.


Figure 7.27 shows a rising cutoff function and the action of the folding operators of both polarities
on the constant function. Observe the nature of the discontinuity at t = 0 and the effect of polarity
reversal.


                                                         1.5


                                                           1


                                                         0.5 -



                                                           으2       너           0        1         2
                                                                               (b)

                                                         1.5




                           (c)                                                 (d)

Figure 7.27. (a) The Rising Cutoff Function r (t) = r[3] (t); (b) f (t) 三 1; (c) U+(r[3] 刃, 1)1 (t);
(d) U_ (r[3],0, 1)1 (t)
Sec. 7.7. Local Trigonometric Bases                                                                                                                                  139

   We saw that for signals with symmetry in the action region folding, corresponds to windowing.
Next we look at signals that are supported to the right (or left) of the folding point and see what
unfolding does to them. In this case, UL(r)(f) is obtained by windowing the even (or odd)
extension of 1 (t) about the folding point. Indeed if 1 (t) = 0, t < 0


                               까（
                               U
                                          (r,
                                                「，
                                                          q1)
                                                          0,
                                                                 1)
                                                                      /(!
                                                                      f (t)
                                                                           )=
                                                                                        { ff(-(t)
                                                                                        {r
                                                                                                       r
                                                                                                                (t)
                                                                                                                (t)
                                                                                                                                    ,),
                                                                                                                                    t)
                                                                                                                                          ,
                                                                                                                                                   if t >
                                                                                                                                                          0,
                                                                                                                                                   if t <。,
                                                                                                                                                                   (7.99)

and if f (t) =0, t >0,


                           U
                               (r,
                                     0,
                                                     1)
                                                                1
                                                                 (t)   =        {   -




                                                                                    r
                                                                                             (-
                                                                                                  -.




                                                                                                           t)
                                                                                                                  r
                                                                                                                      f (t)
                                                                                                                      (-
                                                                                                                           t)
                                                                                                                                ,
                                                                                                                                    f (-
                                                                                                                                              t)
                                                                                                                                                   ,
                                                                                                                                                       if t > 0,
                                                                                                                                                       if t < 0,
                                                                                                                                                                   (7.100)

Figure 7.28 shows the effect of the positive unfolding operator acting on cosine and sine func-
tions supported on the right and left half-lines respectively. Observe that unfolding removes the
discontinuities at t = 0. If the polarity is reversed, the effects on signals on the half-line are
switched; the right half-line is associated with windowed odd extensions and left half-line with
windowed even extensions.

Local Cosine and Sine Bases
Recall the four orthonormal trigonometric bases for L2((0, 1)) we described earlier.

   1. 佃小月 = {v色co帥如 + 枷）}, fl E {0, 1, 2, . . .};

   2. ｛仇떠｝ = { 2si미冗(n+ 枷）}, n E {0, 1, 2, . . .};

   3. {t   (t)} = {1, v'亘cos(冗nt) }, nE {1, 2, . . .};

   4. {    (t)} = {v亘sin(7rnt) }, ii E {0, 1, 2, . . .}.

The bases functions have discontinuities at t = 0 and t = 1 because they are restrictions of
the cosines and sines to the unit interval by rectangular windowing, The natural extensions of
these basis functions to t E 正t (i.e., unwindowed cosines and sines) are either even
                                                                                          (say "+")
or odd (say "-") symmetric (locally) about the endpoints t = 0 and t = 1. Indeed the basis
f끄lctions for the four cases are (+, -), (- . +). (+. + ) and (- , -) symmetric,
                                                                                    respectively, at
(0, 1). From the preceding analysis, this means that unfolding these basis functions corresponds
to windowing if the unfolding operator has the right polarity. Also observe that the basis functions
are discontinuous at the endpoints. Moreover, depending on the symmetry at each endpoint all
odd derivatives (for "+" symmetry) or even derivatives (for "- " symmetry) are zero. By
                                                                                            choosing
unfolding operators of appropriate polarity at the endpoints (with non overlapping action regions)
for the four bases, we get smooth basis functions of compact support. For example. for
                                                                                              (+,-)
symmetry, the basis function U+(ro, 0, fo)U+(ri. 1. 1)仇(t) is supported in (- to. 1 + El) and is
as many times continuously differentiable as r0 and r1 are.
     Let {t3 } be an ordered set of points in 正t defining a partition into disjoint intervals I)
                                                                                                  =
[t3, tJ +ii. Now choose one of the four bases above for each interval such that at tj the basis
functions for I中1 and that for I have opposite symlmetries. We say the polarity at t3 is positive
if the symmetry is -)(+ and negative if it is +)(-. At each t3 choose a smooth cutoff function
140                                          Generalizat向as of the Ba引c r너U出res이Ut山n Wavelet System     Ch. 7



                                    1   1



        0.5                                                0.5




       -0.5                                               -0.5


                -2          0            2                         -2           0           2
                           (a)                                                 (b)




        0.5 ,                                              0.5




       -0.5                                               -0.5

                     1 1

                -2          0            2                         -2           0           2
                           (C)                                                 (d)

Figure 7.28. Folding Functions Supported on Half-Lines. (a) f (t) = cos(즐11t)u(t) ((u(t) is
the Unit Step or Heaviside Function) ; (b) U+(r3j.0, 1)1 (t); (c) f (t) = sin(플11t)u(- t); (d)
U+(r[31, 0, 1)1 (t)


rj (t) and action radius f7 so that the action intervals do not overlap. Let p(j) be the polarity of
t3 and define the unitary operator


                                        U' = fJU
                                              3
                                                 (j)(rj,tj,ej).                                       (7.101)


Let {吻 (t)} denote all the basis functions for all the intervals put together. Then {仇(t)} forms
a nonsmooth orthonormal basis for L2 (正t). Simultaneously {U' 仇 (t) } also forms a smooth
    orthonormal basis for L2(正t). To find the expansion coefficients of a function f (t) in this ba駁s
꺾任｝ use
                                      (1, UJ,l) = (UI, 吻2) .                                  (7.102)
In other words, to compute the expansion coefficients of 1 in the new (smooth) basis, one merely
folds f to Uf and finds its expansion coefficients with respect to the original basis. This allows
one to exploit f戚 algorithms available for coefficient computation in the original basis.
    So for an arbitrary choice of polarities at the end points t3 we have smooth local trigonometric
bases. In particular by choosing the polarity to be positive for all t3 (consistent with the choice
Sec 7.8. Discrete Multiresolution Analysis, the Discrete-Time Wavelet
Transform, and the Continuous Wavelet Transform
                                                                                              141


of the first basis in all intervals) we get local cosine bases. If the polarity is negative for all
ta (consistent with the choice of the second basis for all intervals), we get local sine bases.
Alternating choice of polarity (consistent with the alternating choice of the third and fourth
bases in the intervals) thus leads to alternating cosine/sine bases.
     All these bases can be constructed in discrete time by sampling the cosines/sines basis func-
tions [Wic951. Local cosine bases in discrete time were constructed originally by Malvar and are
                                                                                                im-
sometimes called lapped orthogonal transforms [Mal92]. In the discrete case, the efficient
                                 transforms  (using DCT  I-TV and  DST  I-IV) can  be utilized after
plementation of trigonometric
 folding. In this case, expanding in local trigonometric bases corresponds to computing a DCT
after preprocesing (or folding) the signal.
     For a sample basis function in each of the four bases, Figure 7.7 shows the corresponding
 smooth basis function after unfolding. Observe that for local cosine and sine bases, the basis
 functions are not linear phase; while the window is symmetric, the windowed functions are not.
 However, for alternating sine/cosine bases the (unfolded) basis functions are linear phase. There
 is a link between local sine (or cosine) bases and modulated filter banks that cannot have linear
 phase filters (discussed in Chapter 8). So there is also a link between alternating cosine/sine
 bases and linear-phase modulated filter banks (again see Chapter 8). This connection is further
 explored in [Gop96a].
     Local trigonometric bases have been applied to several signal processing problems. For ex-
 ample, they have been used in adaptive spectral analysis and in the segmentation of speech into
  voiced and unvoiced regions [Wic95]. They are also used for image compression and are known
 in the literature as lapped-orthogonal transforms [Mal92].



Signal Adaptive Local Trigonometric Bases
In the adaptive wavelet packet analysis described in Section 7.3, we considered a full filter bank
tree of decompositions and used some algorithm (best-basis algorithm, for instance) to prune the
tree to get the best tree topology (equivalently frequency partition) for a given signal. The idea
here is similar. We partition the time axis (or interval) into bins and successively refine each
                                                                                                 use
partition into further bins, giving a tree of partitions for the time axis (or interval). If we'
smooth local trigonometric    bases at each of the leaves of a full or pruned tree, we get a smooth
basis for all signals on the time axis (or interval). In adaptive local bases one grows a full tree
 and prunes it based on some criterion to get the optimal set of temporal bins.
    Figure 7.30 schematically shows a sample time-frequency tiling associated with a particular
 local trigonometric basis. Observe that this is the dual of a wavelet packet tiling (see Fig-
 ure 7.15)-in the sense that one can switch the time and frequency axes to go between the
 two.



 7.8     Discrete Multiresolution Analysis, the Discrete- Time Wavelet
         Transform, and the Continuous Wavelet Transform

 Up to this point, we have developed wavelet methods using the series wavelet expansion of
 continuous- time signals called the discrete wavelet transform (DWT), even though it probably
 should be called the continuous-time wavelet series. This wavelet expansion is analogous to the
 142                                                            Generalizations of the Basic Multiresolution Wavelet System                       Ch. 7




                        0                                                                 0
        너                                                                     너                                            \ \
                        -2
                                          2                 4    6             -2             0                     2                4        6
                                         (a)                                                                       (b)




        -1
                   0
                                              \        ＼』
                                                                              너
                                                                                     0
                                                                                              寸 I1                                       \)
                   -2
                             0                2             4    6                   -2
                                                                                              0                        2             4        6
                                        (c)
                                                                                                                 (d)
                               i
                                                                                                  ／尸
                                                                                                       1


                  0          1n
                                                                                    0
        너                                         \'
                                                                              너
              -2
                             0                2             4   6               -2
                                                                                              0                        2             4        6
                                  (e)
                                                                                                                 (f)
                             1\                                                               了
                                                                                                                                 \


             0                                                                 0
        너                                                                    너
             -2
                             0          2                   4   6                             0                  2               4            6
                                  （이
                                                                               -2
                                                                                                           (h)
Figure 7.29. Trigonometric basis functions - before and after unfolding. (a) f
                                                                                                       (t)
cos(즐(n + .5)t)u(t)u(4 - t) where n = 10; (b) U+(r[3],0, 1)U+(r[3],4, 1)1 (t); (c) f (t)
                                                                                                 = sin(퓽(n +
.5)t)u(t)u(4 - t) where n = 10; (d) U_ (r[a} , 0, l)U_ (r[3] , 4, 1)1 (t); (e) 1 (t) = cos(퓽 (n)t)u(t)u(4
                                                                                                           - t ')
where n = 10. (f) U+(r[31, 0. 1)U..(r(3] ,4, 1)f (t); (g) f (t) = sin(和1) t)zi(t)u(4 - t) where n = 10.
(h) ［乙師卜 0, 1刃d佃, 4, 1) f（外
Sec 7.8.   Discrete Multiresolution Analysis, the Discrete- Time Wavelet
Transform, and the Continuous Wavelet Transform                                                 143




                                f




                                                            t

                                           Figure 7.30. Local Basis

Fourier series in that both are series expansions that transform continuous-time signals into a
discrete sequence of coefficients. However, unlike the Fourier series, the DWT can be made
periodic or nonperiodic and, therefore, is more versatile and practically useful.
    In this chapter we will develop a wavelet method for expanding discrete-time signals in a
series expansion since, in most practical situations, the signals are already in the form of discrete
samples. Indeed, we have already discussed when it is possible to use samples of the signal as
scaling function expansion coefficients in order to use the filter bank implementation of Mallat's
algorithm. We find there is an intimate connection between the DWT and DTWT, much as
there is between the Fourier series and the DFT. One expands signals with the FS but often
implements that with the DFT.
    To further generalize the DWT, we will also briefly present the continuous wavelet transform
which, similar to the Fourier transform, transforms a function of continuous time to a repre-
sentation with continuous scale and translation. In order to develop the characteristics of these
various wavelet representations, we will often call on analogies with corresponding Fourier repre-
sentations. However, it is important to understand the differences between Fourier and wavelet
methods. Much of that difference is connected to the wavelet being concentrated in both time
and scale or frequency. to the periodic nature of the Fourier basis, and to the choice of wavelet
bases.

Discrete Multiresolution Analysis and the Discrete-Time Wavelet Transform
Parallel to the developments in early chapters on multiresolution analysis, we can define a discrete
multiresolution analysis (DMRA) for 12, where the basis functions are discrete sequences [Rio93b,
Rio93a, VK95]. The expansion of a discrete-time signal in terms of discrete-time basis function
is expressed in a form parallel to (1.8) as

                                          /（미 = Z缸枷（2                      H 丸）              (7.103)
                                                     3小
 144                                      Generalizations of the Basic Multiresolution Wavelet System   Ch. 7


 where 砂(m) is the basic expansion function of an integer variable m. If these expansion functions
 are an orthogonal basis (or form a tight frame), the expansion coefficients (discrete-time wavelet
 transform) are found from an inner product by

                        따（川 = (1(n)，砂（23n - k)) = 二／佃) ,(2琉 出                                       (7.104)

    If the expansion functions are not orthogonal or even independent but do span Z2, a biorthog-
onal system or a frame can be formed such that a transform and inverse can be defined.
    Because there is no underlying continuous- time scaling function or wavelet, many of the
questions, properties, and characteristics of the analysis using the DWT in Chapters 1, 2, 6,
etc. do not arise. In fact, because of the filter bank structure for calculating the DTWT, the
design is often done using multirate frequency domain techniques, e.g., the work by Smith and
Barnwell and associates [AS96}. The questions of zero wavelet moments posed by Daubechies,
which are related to ideas of convergence for iterations of filter banks, and Coifman's zero scaling
function moments that were shown to help approximate inner products by samples, seem to have
no DTWT interpretation.
    The connections between the DTWT and DWT are:

   . If the starting sequences are the scaling coefficients for the continuous multiresolution anal-
     ysis at very fine scale, then the discrete multiresolution analysis generates the same coeffi-
     cients as does the continuous multiresolution analysis on dyadic rationals.

   1 When the number of scales is large, the basis sequences of the discrete multiresolution
     analysis converge in shape to the basis functions of the continuous multiresolution analysis.

    The DTWT or DMRA is often described by a matrix operator. This is especially easy if the
transform is made periodic, much as the Fourier series or DFT are. For the discrete time wavelet
transform (DTWT), a matrix operator can give the relationship between a vector of inputs to
give a vector of outputs. Several references on this approach are in ERW97, HRW92, KT94a,
KT93, RGN94, RG95. KT94b. Kwo941.

Continuous Wavelet Transforms
The natural extension of the redundant DWT in Section 7.6 is to the continuous wavelet transform
(CWT), which transforms a continuous-time signal into a wavelet transform that is a function
of continuous shift or translation and a continuous scale. This transform is analogous to the
Fourier transform, which is redundant, and results in a transform that is easier to interpret, is
shift invariant, and is valuable for time-frequency/scale analysis. [HW89, GKM89, You80. RD92.
Dau92, VK95, Rio91]
    The definition of the CWT in terms of the wavelet w(t) is given by


                                                                                                   (7.105)
                              끼S，
                                    小．
                                           ' /'   11
                                                       (t)   『
                                                                 （느）
                                                                       dt
where the inverse transform is


                           /（）= Kff如(s,r)w(느，
                           『                D 帥T                                                   (7.106)
 Sec. 7.8   ［기screte F너미t res이Ut山n Anam늬s, the 미screte-Time ＼八／avelet
 Transform, and the Continuous Wavelet Transform
                                                                                                 145

 with the normalizing constant given by


                                             K=／싸민"匈                                          (7.107)

 with W(w) being the Fourier transform of the wavelet w(t). In order for the wavelet to be
 admissible (for (7.106) to hold), K < o工 In most cases, this simply requires that W(0)
                                                                                          = 0 and
that W(w) go to zero (W(回 = 0) f航 enough that K < 以）.
     These admissibility conditions are satisfied by a very large set of functions and give very
little insight into what basic wavelet functions should be used. In most cases, the wavelet w(t)
is chosen to give as good localization of the energy in both time and scale as possible for the
class of signals of interest. It is also important to be able to calculate samples of the CWT as
efficiently as possible, usually through the DWT and Mallat 's filter banks or FFTs. This, and
the interpretation of the CWT, is discussed in [Dau92, VK95, Gop90. GB90, P P89, GKM89,
JB82, RD92, VLU97].
     The use of the CWT is part of a more general time-frequency analysis that may or may not
use wavelets [Coh89, Coh95, HB92, Boa92, LP89].

Analogies between Fourier Systems and Wavelet Systems
In order to better understand the wavelet transforms and expansions, we will look at the various
forms of Fourier transforms and expansion. If we denote continuous time by CT, discrete time
by DT, continuous frequency by CF, and discrete frequency by DF, the following table will show
what the discrete Fourier transform (DFT), Fourier series (FS), discrete-time Fourier transform
(DTFT), and Fourier transform take as time domain signals and produce
                                                                           as frequency domain
transforms or series. For example, the Fourier series takes a continuous-time input signal
                                                                                            and
produces a sequence of discrete-frequency coefficients while the DTFT takes a discrete-time se-
quence of numbers as an input signal and produces a transform that is a function of continuous
frequency.

                                                      DT       CT
                                             DF      DFT       FS
                                             CF     DTFT       FT


      Table 7.4. Continuous and Discrete Input and Output for Four Fourier Transforms

    Because the basis functions of all four Fourier transforms are periodic, the transform of a
periodic signal (CT or DT) is a function of discrete frequency. In other words, it is a sequence
of series expansion coefficients. If the signal is infinitely long and not periodic, the transform is
a function of continuous frequency and the inverse is an integral, not a sum.

                                Periodic in time 4수 Discrete in frequency

                                Periodic in frequency ＜수 Discrete in time
A bit of thought and, perhaps, referring to appropriate materials on signal processing and Fourier
methods will make this clear and show why so many properties of Fourier analysis are created
by the periodic basis functions.
146                                       Generalizations of the Basic Multiresolution Wavelet System   Ch. 7


     Also recall that in most cases, it is the Fourier transform, discrete-time Fourier transform,
or Fourier series that is needed but it is the DFT that can be calculated by a digital computer
and that is probably using the FFT algorithm. If the coefficients of a Fourier series drop off fast
enough or, even better, are zero after some harmonic, the DFT of samples of the signal will give
the Fourier series coefficients. If a discrete-time signal has a finite nonzero duration, the DFT of
its values will be samples of its DTFT. From this, one sees the relation of samples of a signal to
the signal and the relation of the various Fourier transforms.
     Now, what is the case for the various wavelet transforms? Well, it is both similar and different.
The table that relates the continuous and discrete variables is given by where DW indicates
discrete values for scale and translation given by j and k, with CW denoting continuous values
 for scale and translation.
                                                DT           CT
                                      DW      DTWT         DWT
                                      CW     DTCWT         C砥／T


      Table 7.5. Continuous and Discrete Input and Output for Four Wavelet Transforms

   We have spent most this book developing the DWT, which is a series expansion of a continuous
time signal. Because the wavelet basis functions are concentrated in time and not periodic, both
the DTWT and DWT will represent infinitely long signals. In most practical cases, they are made
periodic to facilitate efficient computation. Chapter 9 gives the details of how the transform is
                                                                                             and
made periodic. The discrete-time, continuous wavelet transform (DTCWT) is seldom used
not discussed here.
    The naming of the various transforms has not been consistent in the literature and this is
complicated by the wavelet transformls having two transform variables, scale and translation. If
we could rename all the transforms, it would be more consistent to use Fourier series (FS) or
wavelet series (WS) for a series expansion that produced discrete expansion coefficients, Fourier
transforms (FT) or wavelet transforms (WT) for integral expansions that produce functions of
                                                                                           or CT
continuous frequency or scale or translation variable together with DT (discrete time)
(continuous time) to describe the input signal. However, in common usage, only        the  DTFT
 follows this format!

                Common （兀ns始扼nt            Time,      Transform        Input       Output
                  name   name              C or D      C or D         per幻小C       periodic
                   FS    CTFS                C            D             Yes          No
                  DFT   DTFS                 D            D             Yes          Yes
                 Dl下T   DTFT                 D            C              No          Yes
                   FT   CTFT                 C            C              No          No
                  I叭VT  CTWS                 C            D            YorN         Y or N
                 DT砥／T  DT砥／S                D            D            YorN         Y or N
                        DT砥／T                D            C              N            N
                  CWT   CTWT                 C            C              N            N


 Table 7.6. Continuous and Discrete, Periodic and Nonperiodic Input and Output for Transforms
Sec. 7.8. Discrete Multiresolution Analysis, the Discrete-Time Wavelet
Transform, and the Continuous Wavelet Transform                                                147


    Recall that the difference between the DWT and DTWT is that the input to the DWT is a
sequence of expansion coefficients or a sequence of inner products while the input to the DTWT
is the signal itself, probably samples of a continuous-time signal. The Mallat algorithm or filter
bank structure is exactly the same. The approximation is made better by zero moments of the
scaling function (see Section 6.8) or by some sort of prefiltering of the samples to make them
closer to the inner products [SN96].
    As mentioned before, both the DWT and DTWT can be formulated as nonperiodic, on-going
transforms for an exact expansion of infinite duration signals or they may be made periodic to
handle finite-length or periodic signals. If they are made periodic (as in Chapter 9), then there
is an aliasing that takes place in the transform. Indeed, the aliasing has a different period at the
different scales which may make interpretation difficult. This does not harm the inverse transform
which uses the wavelet information to "unalias" the scaling function coefficients. Most (but not
all) DWT, DTWT, and matrix operators use a periodized form [5V93].
Chapter 8


      Filter Banks and Transmultiplexers


8.1    Introduction
In this chapter, we develop the properties of wavelet systems in terms of the underlying filter
banks associated with them. This is an expansion and elaboration of the material in Chapter 3,
where many of the conditions and properties developed from a signal expansion point of view in
Chapter 5 are now derived from the associated filter bank. The Mallat algorithm uses a special
structure of filters and downsamplers/upsamplers to calculate and invert the discrete wavelet
transform. Such filter structures have been studied for over three decades in digital signal pro-
cessing in the context of the filter bank and transmultiplexer problems [SB86b, Vai87a, VNDS89,
VD89, Vet87, VL89, Mal92, Vai92, RC83]. Filter bank theory, besides providing efficient compu-
tational schemes for wavelet analysis, also gives valuable insights into the construction of wavelet
bases. Indeed, some of the finer aspects of wavelet theory emanates from filter bank theory.

The Filter Bank
A filter bank is a structure that decomposes a signal into a collection of subsignals. Depending
on the application, these subsignals help emphasize specific aspects of the original signal or
may be easier to work with than the original signal. We have linear or non-linear filter banks
depending on whether or not the subsignals depend linearly on the original signal. Filter banks
were originally studied in the context of signal compression where the subsignals were used to
"represent" the original signal. The subsignals (called subband signals) are downsampled so that
the data rates are the same in the subbands as in the original signal-though this is not essential.
Key points to remember are that the subsignals convey salient features of the original signal and
are sufficient to reconstruct the original signal.
     Figure 8.1 shows a linear filter bank that is used in signal compression (subband coding). The
analysis filters {h } are used to filter the input signal x(n). The filtered signals are downsampled
to give the subband signals. Reconstruction of the original signal is achieved by upsampling,
filtering and adding up the subband signals as shown in the right-hand part of Figure 8.1. The
desire for perfect reconstruction (i.e., y(n) = x(n)) imposes a set of bilinear constraints (since all
operations in Figure 8.1 are linear) on the analysis and synthesis filters. This also constrains the
downsampling factor, M, to be at most the number of subband signals, say L. Filter bank design
involves choosing filters {h1} and {gj } that satisfy perfect reconstruction and simultaneously give
informative and useful subband signals. In subband speech coding, for example, a natural choice
of desired frequency responses-motivated by the nonuniform sensitivity of the human ear to
various frequency bands-for the analysis and synthesis filters is shown in Figure 8.2.

148
                                                                                                                    149
Sec. 8.1. Introduction




                                                               南（미
                         /d미                                                       } 凡／    go（미



                                                               d1（미
                         hi(n)         1m나
                                             TM                                            gl(n)


        可미                                                                                                 아
                                                                                                               n)
                                  （미         TM                                    TM      9L-1(미
                                                                    (rt)
                                                                l
                                                         dL_
                                                     -                     H
                              1
                         L-
                  Figure 8.1. L-Band Filter Bank with Rate-Change Factor of M

   In summary, the filter bank problem involves the design of the filters h (미 and 吼(n), with
the following goals:


   1. Perfect Reconstruction (i.e., y(n) = x(n)).


   2. Usefulness. Clearly this depends on the application. For the subband coding application,
      the filter frequency responses might approximate the ideal responses in Figure 8.2. In other
      applications the filters may have to satisfy other constraints or approximate other frequency
      reSl)OnSeS.


If the signals and filters are multidimensional in Figure 8.1, we have the multidimensional filter
bank design problem.




                  rm1                        U           0                     0       1            L- 1



                                                  즈L
              中7r                                주             0                   三
                                                               L)
                 Figure 8.2. Ideal Frequency Responses in an L-band Filter Bank
150                                                                 Filter Banks and Transmultiplexers    Ch. 8


 Transmultiplexer
 A transmultiplexer is a structure that combines a collection of signals into a single signal
                                                                                               at a
higher rate; i.e., it is the dual of a filter bank. If the combined signal depends linearly on the
constituent signal, we have a linear transmultiplexer. Transmultiplexers were originally studied
in the context of converting time-domain-multiplexed (TDM) signals into frequency domain mul-
tiplexed (FDM) signals with the goal of converting back to time-domain-multiplexed signals at
some later point. A key point to remember is that the constituent signals should be recoverable
from the combined signal. Figure 8.3 shows the structure of a transmultiplexer. The input signals
y (n) were upsampled, filtered, and combined (by a synthesis bank of filters) to give a composite
signal d(n). The signal d(n) can be filtered (by an analysis bank of filters) and downsampled
to give a set of signals x (n). The goal in transmultiplexer design is a choice of filters that
ensures perfect reconstruction (i.e., for all i, x2(n) = yj(fl)). This imposes bilinear constraints
on the synthesis and analysis filters. Also, the upsarnpling factor must be at least the number
of constituent input signals, say L. Moreover, in classical TDM-FDM conversion the analysis
and synthesis filters must approximate the ideal frequency responses in Figure 8.2. If the input
signals, analysis filters and synthesis filters are multidimensional, we have a multidimensional
transmultiplexer.

Perfect Reconstruction-A Closer Look
We now take a closer look at the set of bilinear constraints on the analysis and synthesis filters of a
filter bank and/or trausmultiplexer that ensures perfect reconstruction (PR). Assume that there
are L analysis filters and L synthesis filters and that downsampling/upsampling is by some
                                                                                               integer
M. These constraints, broadly speaking, can be viewed in three useful ways, each applicable in
specific situations.

   1. Direct characterization - which is useful in wavelet theory (to characterize orthonormality
      and frame properties), in the study of a powerful class of filter banks (modulated filter
      banks), etc.

   2. Matrix characterization - which is useful in the study of time-varying filter banks.

   3. z-transform-domain (or polyphase-representation) characterization - which is useful in the
      design arid implementation of (unitary) filter banks and wavelets.

Direct Characterization of PR
We will first consider the direct characterization of PR, which, for both filter banks and trans-
multiplexers, follows from an elementary superposition argument.

Theorem 38 A filter bank is PR if and only if, for all integers ii1 and n2,

                         L- 1

                         乞 二M蜘＋ni)g十枷 H向 = 伽 卞 向1                                                        (8.1)
                          i=O   n

A transmultiplexer is PR if and only if, for all i, j E {0, 1,. . . ,L - l} ,

                                ＞二九i(n)9j(m入17- n) = (5（加（i- j).                                         (8.2)
Sec. 8.1. Introduction                                                                          151




    yo(n)                                                                                 xo（미
                 I M              90(n)                                  h0（미    TM



    y1(미                                                                                  幻（미
                                  gi   (n)
                                                                         h1（미    凡I

                                                      (n)
                                                 d
  YL-1(미
                 TM                                                              TM
                                                                                          XL_       (미
                                  L-1（미                          뇨
                                                                         L-1（미
                                                                                                1
          H




               Figure 8.3. L-Band Tansmultiplexer with Rate Change Factor of Al

Moreover, if the number of channels is equal to the downsampling factor (i.e., L = IMl),(8.1)
and (8.2) are equivalent.

Consider a PR filter bank. Since an arbitrary signal is a linear superposition of impulses, it
suffices to consider the input signal, x(n) = 8(n - n1), for arbitrary integer n1. Then (see
Figure 8.1) di(n) = hi(Mn - ni) and therefore, y(n2) = ＞二 >二gj(ri2 小 Mn)di(n). But by PR,
                                                             i       n

y(n2) = 8(n2 - n1). The filter bank PR property is precisely a statement of this fact:

       9(m) = Z三川m- A刎町미 = Z＞그(n2 - Mn)h2(A／小메日他 H 메·
                   ?     fl                  z          fl



Consider a PR transmultiplexer. Once again because of linear superposition, it suffices to consider
only the input signals xi(n) = 5(n)8(i- j) for all i and j. Then, d(미 = gj(n) (see Figure 8.3), and
y (l) = > hj(加(Ml - n). But by PR yi(l) = 8(l)d(i - j). The transmultiplexer PR property

is precisely a statement of this fact:

                   肌(1) = ＞二屈(n)d（凡Ii 中 n) = ＞二九j(n)gj（入Ii 中 n) = S（加（可 - j).
                              n                      Ti



Remark: Strictly speaking, in the superposition argument proving (8.2), one has to consider
the input signals x1(n) = S(n - ni)5(i - j) for arbitrary n1. One readily verifies that for all n1
(8.2) has to be satisfied.
 152                                                                 Filter Banks and Transmultiplexers    Ch. 8


    The equivalence of (8.1) and (8.2) when L = M is not obvious from the direct characteriza-
tion. However, the transform domain characterization that we shall see shortly will make this
connection obvious. For a PR filter, bank the L channels should contain sufficient information
to reconstruct the original signal (note the summation over i in (8.1)), while for a transmulti-
plexer, the constituent channels should satisfy biorthogonality constraints so that they can be
reconstructed from the composite signal (note the biorthogonality conditions suggested by (8.2)).

Matrix characterization of PR
The second viewpoint is linear-algebraic in that it considers all signals as vectors and all filtering
operations as matrix-vector multiplications [Vet87}. In Figure 8.1 and Figure 8.3 the signals x(n),
d (n) and y(n) can be naturally associated with infinite vectors x, d1 and y respectively
                                                                                                  . For
example, x = ［· · · , x(- 1), x(O), x(1),. . .]. Then the analysis filtering operation can be expressed
as
                               d1= H2x,          foriE{ O, 1, 2, . . .,L- 1},                             (8.3)
where, for each i, H2 is a matrix with entries appropriately drawn from filter h2. H2 is a block
Toeplitz matrix (since its obtained by retaining every 兀rt九 row of the Toeplitz matrix representing
convolution by h) with every row containing h2 in an index-reversed order. Then the synthesis
filtering operation can be expressed as

                                               y= 二G?d,                                                   (8.4)

where, for each i, Gi is a matrix with entries appropriately drawn from filter g. Gi is also a
block Toeplitz matrix (since it is obtained by retaining every Mth row of the Toeplitz matrix
whose transpose represents convolution by gj) with every row containing gj in its natural order.
Define d to be the vector obtained by interlacing the entries of each of the vectors d3: d =
[. . . , d (0), d1(0),. . . , dM_ j(O), d0 (1), d1(1),. . .]. Also define the matrices H and G (in terms of
H2 and G2) so that
                                       d= Hx,      and    y= GTd.                                         (8.5)
H is obtained by interlacing the rows of H2 and G is obtained by interlacing the rows of G2. For
example, in the FIR case if the filters are all of length N,



                        ／奴N 小 1)        ...     ho(N - 凡I 中 1)              h0 (0)     0


 d = Hx 望f             hL_ l (N 中 1)    .. .   hL_ l (N - Al - 1)         hL_ 1(0)     0
                              0          0        h0(N- 1)


                             0           0       hL_ l (N- 1)



짜om this development, we have the following result:
Sec. 8 1   Intr이加Ct山n                                                                        153


Theorem 39 A filter bank is PR if
                                                          GTH = I.                           (8.7)

A transrnultiplexer is PR if
                                                          HGT = I.                           (8.8)

凡勿reo刃er, v沇en L = M, 切th 口)fld毗ons are equ切（llent.

One can also write the PR conditions for filter banks and transmultiplexers in the following form,
which explicitly shows the formal relationship between the direct and matrix characterizations.
For a PR filter bank we have
                                                      兄可耳＝I.                                 (8.9)

Correspondingly for a PR transmultiplexer we have

                                                    瓦可 = 叩 + 肛·                             (8.10)

Polyphase (Transform- Domain) Characterization of PR
We finally look at the analysis and synthesis filter banks from a polyphase representation view-
point. Here subsequences of the input and output signals and the filters are represented in the
z-transform domain. Indeed let the z-transforms of the signals and filters be expressed in terms
of the z-transforms of their subsequences as follows:
                                                               凡1-1

                                             X(z) = Z :k차（少）
                                                                k=O



                                             Y(z) = ＞二 少Yk(Z兀I)
                                                                 丸＝
                                                              凡I 小 l

                                            H (z) = ＞二 之’勺／Lk(2入I)
                                                              k=0
                                                               入1- i

                                            G2(z) = ＞二 Z'Gj,k(ZM)
                                                               k=O

Then, along each branch of the analysis bank we have

                        1가（기   =   [ 兀11｛且2(z)X(z)}
                                                   ( ／섣：-i             \   ／世二l    \   )

                                   [J lt기 { ( Z 2" "瓦，(z) ) ( 乞 : '兀（zM) ) }
                                                   L \ k=0             /   \1= O   / 1



                                   [lit기 { 乞 少勻如名吟兀（少）
                                             ｛立：
                                                    k .i==0
                                   iLl- i                                  凡1-1

                               = 三 d(／尸丸）H2,k (z）兀（z) = Z 且自k(Z)Xk（名）
                                                                    ·
                                   k.1=O                                    k
154                                                               Filter Banks and Transmultiplexers    Ch. 8


Similarly, from the synthesis bank, we have
                                       L- 1
                           Y（기    =    ＞二／가（z入J)（玉（기                                                   (8.16)
                                       i= 0
                                       L- 1               (M- 1           \

                                  = Zn（少）4
                                       i= 0
                                        ,I-1
                                       4｛二l      r느？
                                                 (느3                          )
                                       느        {i,kZM 가（少）· r
                                       乞 :: '' 位戶i
                                       k=0
                                       k==0
                                                    >1
                                                 I' t=0
                                                 \L t=U                       )

and therefore (from (8.12))
                                               L- 1
                                      Yk伺 = Z GL洞긔z).                                                  (8.17)
                                               i= 0

For i e {0, 1, . . . , L - 1} and k e {0, 1, . . . , M - 1}, define the polyphase component matrices
(H (z))i,k = 月i.k（기 and 四小小,k = Gi,k (z). Let 차（기 and %（기 denote the 小transforms of
the polyphase signals x (미 and yp(fl), and let D (z) be the vector whose components are D (z).
Equations (8.16) and (8.17) can be written compactly as

                                       I기，（기 = H伺차回，                                                   (8.18)

                                       耳（2) = G三(z)D (z),                                              (8.19)
and
                                   耳伺 = 町回H（기차떠·                                                       (8.20)
Thus, the analysis filter bank is represented by the multi-input (the polyphase components of
X(z)), multi-output (the signals D1(z)) linear-shift-invariant system H (z) that takes in X (z)
and gives out D (z). Similarly, the synthesis filter bank can be interpreted as a multi-input
(the signals D (z)), multi-output (the polyphase components of Y(z)) system C ' (z), which
maps D (z) to }' (z). Clearly we have PR if 耳(z) = X (z). This occurs precisely when
畔 (z)H （기 = I.
   For the transmultiplexer problem, let 1 (z) and X (z) be vectorized versions of the input and
output signals respectively and let D (z) be the generalized polyphase representation of the signal
D(z). Now 까（기 = 町回디기 and 차（기 = 馬（기까떠· Hence 차（기 = H (z)G三（z)1' (z),
and for PR H (z)G三(z) = I.

Theorem 40 A filter bank has the PR property if and only if

                                         畔伺피기 =／·
A 加ansmult切扼xer h（工S 坑ePR 끄ro끄日抑／!/ 口nd only if

                                         瓦回畔回 = I

U脆ere 瓦（기 and（斗（기 are 口s defined 的加e.
Sec 8.2. Unitary Fifter Banks                                                                    155


Remark: If G二(z)H (z) = I, then H (z) must have at least as many rows as columns (i.e.,
L 之 M is necessary for a filter bank to be PR). If H (z)GT(z) = I then HP(z) must have at
least as many columns as rows (i.e., M ? L is necessary for a tranmultiplexer to be PR). If
L = M, G (z)H (z) = I = H ' (z)GF(z) and hence a filter bank is PR if the corresponding
transmultiplexer is PR. This equivalence is trivial with the polyphase representation, while it is
not in the direct and matrix representations.
    Notice that the PR property of a filter bank or transmultiplexer is unchanged if all the
analysis and synthesis filters are shifted by the same amount in opposite directions. Also any
one analysis/synthesis filter pair can be shifted by multiples of M in opposite directions without
affecting the PR property. Using these two properties (and assuming all the filters are FIR), we
can assume without loss of generality that the analysis filters are supported in [0, N - 1] (for
some integer N). This also implies that H (z) is a polynomial in z 1, a fact that we will use in
the parameterization of an important class of filter banks-unitary filter banks.
    All through the discussion of the PR property of filter banks, we have deliberately not said
anything about the length of the filters. The bilinear PR constraints are completely independent
of filter lengths and hold for arbitrary sequences. However, if the sequences are infinite then
one requires that the infinite summations over n in (8.1) and (8.2) converge. Clearly, assuming
 that these filter sequences are in 2 (Z) is sufficient to ensure this since inner products are then
 w아l-d沮ned.


8.2     Unitary Filter Banks
From (8.5) it follows that a filter bank can be ensured to be PR if the analysis filters are chosen
such that H is left-unitary, i.e., HTH = I. In this case, the synthesis matrix G = H (from (8.7))
and therefore G2 = H2 for all i. Recall that the rows of G1 contain g, in natural order while the
rows of H2 contains h2 in index-reversed order. Therefore, for such a filter bank, since G2 = H,,
the synthesis filters are reflections of the analysis filters about the origin; i.e., g1(n) = h2(- n).
Filter banks where the analysis and synthesis filters satisfy this reflection relationship are called
unitary (or orthogonal) filter banks for the simple reason that H is left-unitary. In a similar
fashion, it is easy to see that if H is right-unitary (i.e.. HHT = I). then the transmultiplexer
associated with this set of analysis filters is PR with g, (n) = h1(- n). This defines unitary
transmultiplexers.
    We now examine how the three ways of viewing PR filter banks and transmultiplexers simplify
when we focus on unitary ones. Since g,(n) = h,(- n), the direct characterization becomes the
following:
Theorem 41 A filter bank is unitary if

                            乞＞二h (蜘＋메h (蜘＋n2) = 5(nj - n2).                                    (8.23)
                                2   fl


A 地nsmul帥泌xer is 2工nitary 涉

                                         ＞二／ii(n)h3(IYIl +n) = 6（加（i 寸j).                      (8.24)
                                          n


{/ 坑e number of ch（工nnels is equ毗 切 坑e dot,片zsampling fac加r, 仇en 口 /ilter ban丸 招 unitary z了 坑e
col寸es工）ondii四 tr口nsmult切lexer is unitai그／.
 156                                                           Filter Banks and Transmultiplexers     Ch. 8


 The matrix characterization of unitary filter banks/transmultiplexers should be clear from the
 above discussion:

Theorem 42 A filter bank is unitary if HTH = I, and a transrnultiplexer is unitary if
HHT = I.

The z-transform domain characterization of unitary filter banks and transmultiplexers is given
below:

Theorem 43 A filter bank is unitary if H ' (z ')HP(z) = I, and a transrnultiplexer is unitary
涉H (z)H了（z_1) = I.

    In this book (as in most of the work in the literature) one primarily considers the situation
where the number of channels equals the downsampling factor. For such a unitary filter bank
(transmultiplexer), (8.9) and (8.10) become:


                                                                                                    (8.25)


and

                                        H沮｝＝叩m力I.                                                   (8.26)

 The matrices H2 are pairwise orthogonal and form a resolution of the identity matrix. In other
 words, for each i, HTH, is an orthogonal projection matrix and the filter bank gives an orthogonal
 decomposition of a given signal. Recall that for a matrix P to be an orthogonal projection matrix,
P2 = P and P 2 0; in our case, indeed, we do have H了Hi 之 0 and HTHHTHi = HTHI.
    Unitarity is a very useful constraint since it leads to orthogonal decompositions. Besides, for
 a unitary filter bank, one does not have to design both the analysis and synthesis filters since
h2(n) = gj(- n). But perhaps the most important property of unitary filter banks and trans-
multiplexers is that they can be pararneterized. As we have already seen, filter bank design is a
nonlinear optimization (of some goodness criterion) problem subject to PR constraints. If the PR
constraints are unitary, then a parameterization of unitary filters leads to an unconstrained opti-
mization problem. Besides, for designing wavelets with high-order vanishing moments, nonlinear
equations can be formulated and solved in this parameter space. A similar parameterization of
nonunitary PR filter banks and transmultiplexers seems impossible and it is not too difficult to
intuitively see why. Consider the following analogy: a PR filter bank is akin to a left-invertible
matrix and a PR transmultiplexer to a right-invertible matrix. If L = Al, the PR filter bank
is akin to an invertible matrix. A unitary filter bank is akin to a left-unitary matrix, a unitary
transmultiplexer to a right-unitary matrix, and when L = Al, either of them to a unitary matrix.
Left-unitary, right-unitary and in particular unitary matrices can be parameterized using Givens'
rotations or Householder transformations [GL93}. However, left-invertible, right-invertible and,
in particular, invertible matrices have no general parameterization. Also, unitariness allows ex-
plicit parameterization of filter banks and transmultiplexers which just PR alone precludes. The
analogy is even more appropriate: There are two parameterizations of unitary filter banks and
transmultiplexers that correspond to Givens' rotation and Householder transformations, respec-
tively.
 Sec. 8.2. Unitary Filter Banks
                                                                                                               157

    All our discussions on filter banks and transmultiplexers carry over naturally with very small
notational changes to the multi-dimensional case where downsampling is by some integer matrix
[GB94a]. However, the parameterization result we now proceed to develop is not known in the
multi-dimensional case. In the tw아dimensional case, however, an implicit, and perhaps not too
practical (from a filter-design point of view), parameterization of unitary filter banks is described
in [BC92].
    Consider a unitary filter bank with finite-impulse response filters (i.e., for all i, hi is a finite
sequence). Recall that without loss of generality, the filters can be shifted so that H (z) is a
polynomial in z 1. In this case G,(z) = H (zH1) is a polynomial in z. Let

                                                                       K- i
                                                        .1了；(z) = ＞二M枷也                                      (8.27)
                                                                       k=O


That is, H (z) is a matrix polynomial in z 1 with coefficients h (k) and degree K - 1. Since
H '(z ')H (z) = I, from (8.27) we must have h ' (O)h (K - 1) = 0 as it is the coefficient of
zK4l in the product H ' (z ')H (z). Therefore h (0) is singular. Let 尸k1 be the unique
projection matrix onto the range of h끄(K - 1) (say of dimension dKH1). Then hp(0)TPK1 =
0 = P_ 1h끄(O). Also PKmih(K - 1) = h(K - 1) and hence (I - PK寸1)h(K - 1) = 0. Now
[I - PK_1 + ZPK_1] H (z) is a matrix polynomial of degree at most K -2. If h(0) and h(K - 1)
are nonzero (an assumption one makes without loss of generality), the degree is precisely K - 2.
Also it is unitary since I - 尸k1 + ZPK. 1 is unitary. Repeated application of this procedure
(K 中 1) times gives a degree zero (constant) unitary matrix V0. The discussion above shows that
an arbitrary unitary polynomial matrix of degree K - 1 can be expressed algorithmically uniquely
as described in the following theorem:

Theorem 44 For 口 끄可ynom可口lm口勿ix 丑刃（z), un可ta,킵 on t九e un化 circle 在．e., 町何牡M
                                                                                           기=
I) , and of polynomial degree K - 1, there exists a unique set of projection matrices Pk (each of
r口n丸 some integer dk力 suc九 坑毗


                                          耳K기
                                                        {kii，나卄'小·                                          (8.28)


Remark: Since the projection Pk is of rank 5k, it can be written as vjvT
                                                                         + . . . + V5kV},, for a
nonunique set of orthonormal vectors v2. Using the fact that

                        Tj           丁尸             l
                                                                                  i- i
                         임                      2
                                                    （叩｝＋꺄고弘月 = fiJI- 如F + z뇨呵］
               刃             U        刃
                                                                                                            (8.29)
                    ;
                                 ;
                             J
                J
                                                                                  i= 7


defining 스 = 乞k 5k and collecting all the vi's that define the Pk 'S into a single pool (and
reindexing) we get the following factorization:



                                      H
                                          (z)
                                                =       fi
                                                        k＝스
                                                              [I
                                                                   -   VkV{ + Z   iv     vT]   1   V。
                                                                                                        .
                                                                                                            (8.30)
158                                                              Filter Banks and Transmultiplexers   Ch. 8



If H (z) is the analysis bank of a filter bank, then notice that 스 (from (8.30)) is the number
of storage elements required to implement the analysis bank. The minimum number of storage
elements to implement any transfer function is called the McMillan degree and in this case i is
indeed the McMillan degree [Vai92]. Recall that PK is chosen to be the projection matrix onto
the r工nge of hP(K - 1). Instead we could have chosen 尸k to be the projection onto the nullspace
of hP(0) (which cont恤s the range of h (K 小 1)) or any space sandwiched between the two. Each
choice leads to a different sequence of factors PK and corresponding 5k (except when the range
and nulispaces in question coincide at some stage during the order reduction process). However,
스｝ the 入1Cl뇨4illan de因氾e is constant.
    Equation (8.30) can be used as a starting point for filter bank design. It parameterizes all
unitary filter banks with McMillan degree 스. If 스 = K, then all unitary filter banks with filters
of length N ( MK are parameterized using a collection of K - 1 unitary vectors, vk, and a
unitary matrix, V0. Each unitary vector has (M - 1) free parameters, while the unitary matrix
has M (M 小 1)/2 free parameters for a total of (K - 1)(M 寸1) +              free parameters for H (z).
                                                                       (M
The filter bank design problem is to choose these free parameters to optimize the "usefulness"
criterion of the filter bank.
    If L> M, and H (z) is left-unitary, a similar analysis leads to exactly the same factorization
as before except that V0 is a left unitary matrix. In this case, the number of free parameters is
given by (K- 1)(L- 1) +
                        （計（吩             For a transmultiplexer with L <M, one can use the same

factorization above for H '(z) (which is left unitary). Even for a filter bank or transmultiplexer
with L = M, factorizations of left-/right-unitary H,(z) is useful for the following reason. Let us
assume that a subset of the analysis filters has been predesigned (for example in wavelet theory
one sometimes independently designs h0 to be a K-regular scaling filter, as in Chapter 6). The
submatrix of H (z) corresponding to this subset of filters is right-unitary, hence its transpose can
be parameterized as above with a collection of vectors v! and a left-unitary V0. Each choice for
the remaining columns of Vo gives a choice for the remaining filters in the filter bank. In fact, all
possible completions of the original subset with fixed McMillan degree are given this way.
    Orthogonal filter banks are sometimes referred to as lossless filter banks because the collective
energy of the subband signals is the same as that of the original signal. If U is an orthogonal
matrix, then the signals x(미 and Ux(n) have the same energy. If P is an orthogonal projection
matrix, then

                                  IIxII2 = 1jPxII2 + 11(1 - P)x112 .


For any give X(z), X(z) and z中'X (z) have the same energy. Using the above facts, we find that
白r any projection matri兀 므


                          까떠 = [I- P+ z뾔 차떠 혤 T(z)차（기

has the same energy as X (z). This is equivalent to the fact that T(z) is unitary on the unit
circle (one can directly verify this). Therefore (from (8.28)) it follows that the subband signals
have the same energy as the original signal.
Sec. 8.2. Unitary Filter Banks                                                                                                    159


   In order to make the free parameters explicit tot filter design, we now describe V0 and {v}
using angle parameters. First consid r m, with Vj 1 = 1. Clearly, vi has (M - 1) degrees of
freedom. One way to parameterize vi '!Sing (M - 1) angle parameters 9j,k, k E {0, 1,.. . , M - 2}
would be to define the components of v, as follows:




                                   {
                                   ｛丑
                                    fJ sin(O,..1) } cos(02,3)                              for jE{ 0, 1, . . . 小f- 2}
                                             1=0
                    (v1)   7   =

                                       I TT
                                       (M-
                                                   )
                                                   1
                                       ) llS1flt口jJ) r
                                                       -   .   -   i,   .
                                                                                           for j = Al - 1.
                                       \ 1=U                                I



As for V0, it being an Al x Al orthogonal matrix, it has                                                  degrees of freedom. There are
                                                                                                (Al
                                                                                                k2
two well known parameterizations of constant orthogonal matrices, one based on Givens' rotation
(well known in QR factorization etc. {DS83]), and another based on Householder reflections. In
the Householder parameterization

                                                                                A卜-1

                                                                   v0= JJ [I- 2v1vfl,
                                                                                i= 0


where v2 are unit norm vectors with the first i components of V2 being zero. Each matrix factor
[I 小 2v2vfl when multiplied by a vector q, reflects q about the plane perpendicular to v2, hence
the name Householder reflections. Since the first i components of v, is zero, and jvi11 = 1, v2 has
M - i - 1 degrees of freedom. Each being a unit vector, they can be parameterized as before
using M - i - 1 angles. Therefore, the total degrees of freedom are

                                              M- 1                                     凡f- i

                                              二四-1- i) 4그나朴
                                               i= 0                                    i= 0           '


In summary, any orthogonal matrix can be factored into a cascade of M reflections about the
planes perpendicular to the vectors v2.
    Notice the similarity between Householder reflection factors for V0 and the factors of H (z) in
(8.30). Based on this similarity, the factorization of unitary matrices and vectors in this section is
called the Householder factorization. Analogous to the Givens' factorization for constant unitary
matrices, also one can obtain a factorization of unitary matrices H (z) and unitary vectors
 V(z) [DVN88I. However, from the points of view of filter bank theory and wavelet theory, the
Householder factorization is simpler to understand and implement except when M = 2.
    Perhaps the simplest and most popular way to represent a 2 x 2 unitary matrix is by a
rotation parameter (not by a Householder reflection parameter). Therefore, the simplest way to
represent a unitary 2 x 2 matrix H,(z) is using a lattice parameterization using Given's rotations.
Since tw아channel unitary filter banks play an important role in the theory and design of unitary
modulated filter banks (that we will shortly address). we present the lattice parameterization
 [VH88]. The lattice parameterization is also obtained by an order-reduction procedure we saw
while deriving the Householder-type factorization in (8.28).
 160                                                                                                  Filter Banks and Transmultiplexers     Ch. 8


 Theorem 45 Ever김 unitary 2 x 2 m口打初 馬 （기 (in p口I才icul口r 疏e j7O切血zse m口加ix of a two
 channel FIR unitary filter bank) is of the form

                                                               0
                   H
                           (z)
                                        =
                                                [:
                                                              士1                                                                           (8.31)

 where
                       R
                                 (9)
                                            =        [     cos9
                                                         -sine
                                                                     sin9
                                                                     COS 9
                                                                                      and
                                                                                                 /=
                                                                                                           [:
                                                                                                                二］                         (8.32)


Equation (8.31) is the unitary lattice parameterization of H (z). The filters Ho(z) and Hi(z) are
given by

                                                              田卄瓦(z'小니·
By changing the sign of the filter hi(n), if necessary, one can always write H (z) in the form

                                                珥（기 = R(OK_1)ZR(OK_기z . . .ZR(O아

Now, if Hj (z) is the reflection of Ho,3 (z) (i.e., Ho,3(z) = z '< +'Ho,j (zm1)), then (from the
algebraic form of R(9))

                                       I 尸，0,아긴 玩，11긴 ] = [ 也唄 曳中？ ] .                                                                     (8.33)
                                       In ',叭기 111,1（기 j  I -'o:                            i기        no：
                                                                                                        叭引 J
    With these parameterizations, filter banks can be designed as an unconstrained optimization
problem. The parameterizations described are important for another reason. It turns out that the
most efficient (from the number of arithmetic operations) implementation of unitary filter banks
is using the Householder parameterization. With arbitrary filter banks, one can organize the corn-
putations so as capitalize on the rate-change operations of upsampling and downsampling. For
example, one need not compute values that are thrown away by downsarnpling. The gain from us-
ing the parameterization of unitary filter banks is over and above this obvious gain (for example,
see pages 330-331 and 386-387 in [Vai92}). Besides, with small modifications these parameteriza-
tions allow for unitariness to be preserved, even under filter coefficient quantization-with this
having implications for fixed-point implementation of these filter banks in hardware digital signal
processors [Vai92].


8.3      Unitary Filter Banks- Some Illustrative Examples

 A few concrete examples of Al-band unitary filter banks and their parameterizations should
clarify our 小scussi이l.
    First consider the two-band filter bank associated with Daubechies' four-coefficient scaling
function and wavelet that we saw in Section 5.9. Recall that the lowpass filter (the scaling filter)
is given by

                                                         Ii         0          1        2              3
                                                     枷（미           1+13
                                                                    4\／万
                                                                             3十V／죵
                                                                              'lv／互    告碧 능岩·
Sec. 8.3. Unitary Filter Banks-Some Illustrative Examples
                                                                                               161

The highpass filter (wavelet filter) is given by hi(n) = (- 1)nho(3 - n), and both (8.1) and (8.2)
are satisfied with gj (n) = hi(- n). The matrix representation of the analysis bank of this filter
bank is given by



                             卜＼ ／죵
                              4Vb
                                           ： 小市
                                                      血m蠶籌： 口     0       0
                             H 1十＼
                                 ／죵
        d = Hx ＝二               4v5     芸弩                        0



                                                                          聲
                                                                                             (8.34)
                                                                          0
                                                                                 "




                                                      ：密薰和
                                0         0                     3+ v／죵和
                                0         0
                                                                      ：
                                                                      1




One readily verifies that HTH = I and HHT = I. The polyphase representation of this filter
bank is given by


              馬（기 =
                        赤［       (1 + \／죵） + zH' (3 + \／죵） (3 + \／죵） + ze' (l - \／죵） "
                                 (3 +\／죵）+ zH1(1中 \／죵） (- 3＋侮卜戶 (1＋而） .                      (8.35)

and one can show that H ' (z 1)H (z) = I and H (z)H ' (zH') = I. The Householder factoriza-
tion of H (z) is given by
                                    馬（기 = [/ - vivT + zH1vivfl乞                              (8.36)
where

                        V1＋器針 帥d %=[：月믐 !；針
Incidentally, all two-band unitary filter banks associated with wavelet tight frames have the
same value of V0. Therefore, all filter banks associated with two-band wavelet tight frames are
completely specified by a set of orthogonal vectors vi, K - 1 of them if the h0 is of length
2K. Indeed, for the six-coefficient Daubechies wavele.ts (see Section 5.9), the parameteriz
                                                                                               ation
of H (z) is associated with the following two unitary vectors (since K = 3): vf = 卜.3842.9232]
and v子 = [-.1053 - .9944].
    The Givens' rotation based factorization of H (z) for the 4-coefficient Daubechies filters
                                                                                               given
by:

                        馬（z)=[-:：誥 二：黑0 二飴 ：盟］,                                              (8.37)
where 60 = 퓽 and 9l = 中｛들 . The fact that the filter bank is associated with wavelets is precisely
because oo + 01 = 플 . More generally, for a filter bank with filters of length 2K to be associated
with wavelets, 드仁bl tk = . This is expected since for filters of length 2K to be associated with
wavelets we have seen (from the Householder factorization) that there are K 卞 1 parameters
                                                                                             Vk.
   Our second example belongs to a class of unitary filter banks called modulated filter banks,
which is described in a following section. A Type 1 modulated filter bank with filters of length
N = 2M and associated with a wavelet orthonormal basis is defined by


  瓦（「）小小(ir("" ::'" .5) (2i『i) 1) -81sinf in（甘")b (2汁1)카 (8.38)
162                                                                                               Filter Banks and Transmultiplexers    Ch. 8


where i E {0, . . . , M - 1} and n E {0, . . . , 2M - 1} [GB95b, GB95c]. Consider a three-band
example with length six filters. In this case, K = 2, and therefore one has one projection P1 and
the matrix V0. The projection is one-dimensional and given by the Householder parameter


                                                                                                                            쿄小
                                                                                                   1 1
                      口，       1                                             1                老
                                                                                                                                       (8.39)
                                                                          而
                                                                                                          ]
                      '    =

                               V/g
                 vi
                                                                                                          +
                                                       and    V0＝                                         ]
                                                                                                          l
                                          느                                                   2
     The third example is another Type 1 modulated filter bank with M = 4 and N = 8. The
filters are given in (8.38). H (z) had the following factorization

                                              H （기 = [/ -P1 + zH1Pi] V0,                                                               (8.40)

where P1 is a tw아dimensional projection P1 = vivT +v2v子 (notice the arbitrary choice of v1 and
v2) given by
                               f
                           41636433418450
                                     0.                   00000000000000
                                                                     -               F   0.                                  -




                      I -0.78450701561376           1 - 0.14088210492943
                 V1 =
                      I  0.32495344564406 1V2 = I       0.50902478635868
                      L 0.32495344564406 -          L -0.84914427477499 -
and



                                                             l扼0 l       l 0扼d
                                                                                                  l 0扼
                                                                                 l
                                                                                                                        %
                                                m
                                                l 寸n
                                                   乙
                                                                                 扼
                                                                                                              1




                                                                                                                  H 1




                                                                                 l
                                                                                                                        1


                                                                                 0
Notice that there are infinitely many choices of v1 and v2 that give rise to the same projection
P1.

8.4    M- band Wavelet Tight Frames

In Section 7.2, Theorem (7.7), while discussing the properties of M-band wavelet systems, we
saw that the lowpass filter h0 (h in the notation used there) must satisfy the linear constraint
Z岫2) = \／而.Otherwise, a scaling function with nonzero integral could not exit. It turns
out that this is precisely the only condition that an FIR unitary filter bank has to satisfy in order
for it to generate an M-band wavelet system [Law90, GB92c]. Indeed, if this linear constraint
is not satisfied the filter bank does not generate a wavelet system. This single linear constraint
(for unitary filter banks) also implies that 三 h (n) = 0 for i E {1, 2, . . . , M - 1} (because of
                                                                 h
Eqn. 8.1). We now give the precise result connecting FIR unitary filter banks and wavelet tight
frames.
Theorem 46 C初en an FIR u硫ai긔 /ilter b毗 毗坑 ZM미                                                            = \／而， 坑ere exis加 an unique,

compactly supported, scaling function 吼(t) E L2(IR) (with support in [0, 유븍], assuming h0 is
supported in [0, N - 1]) determined by the scaling recursion:

                                          蜘(t) = V而Z九M向蜘(Mt                                         川·                                 (8.41)
                                                                 丸
 Sec. 8.4. M-band Wavelet Tight Frames                                                                                               163

 Dc／沇ew口velets, 吻떠，

                      吻떠 = 而＞二m（扮枷(Mt 出                                                              i e {L 2, . . . , 凡r H l} ,   (8.42)
                                                   k

 and functions, 砂i, j, k(t),
                                                       砂2,3 , 丸（t) = 兀1j/2吻（凡f3 t 卄 丸）.                                            (8.43)
 T／工en｛吻, j,k} Jo竹ns a tight fr口me for L2（正t). Th口t 秀5, 加r 毗 / e L2（正｛)



                                              f(t) = 三 Z                          (/，仇3大）砂2,3，丸（外                                  (8.44)
                                                              2＝二1 3丙＝m以）


 Also,
                                                                              M-            1   여그    (X)

                   f(t) =＞二（/，砂O,O,k）砂O,O,k (t) + ＞二Z ＞二 (/，砂i.3.k）砂自3,k (t).                                                      (8.45)
                               丸                                                  i= 1          j= 1 丸＝＝寸아그


Remark: A similar result relates general FIR (not necessarily unitary) filter banks and M-band
 wavelet frames [CDF92, GB92c, Gop92].
    Starting with (8.41), one can calculate the scaling function using either successive
                                                                                         approxima-
 t油i or i毗eq油毗油ion the it工adic rationals-i.e., exactly as in the tw아硫nd case in Chapter
                                                                                                7그
Equation (8.42) then gives the wavelets in terms of the scaling function. As in the tw아band case,
the functions 吻떠, so constructed, invariably turn out highly irregular and sometimes fractal.
The solution, once again, is to require that several moments of the scaling function (or
                                                                                            equiva-
lently the moments of the scaling filter h0) are zero. This motivates the definition of K-re目llar
M-band scaling filters: A unitary scaling filter h0 is said to be K regular if its Z-transform can


                                                                                                             ]]
be written in the form

                                    （:                                                            (M_   1)
                                                                                                                  K
                                   玩 =
                                                                z_
                                                                                                                      Q(z)
                                                                                      +z_
                                              )=
                                                        [1+
                                                                     l+
                                                                          .   .   .




                                                                                                                                   (8.46)
                                                                              M
                                   H。
                                        (z)
                                                                                                                             ,
 for maximal possible K. By default, every unitary scaling filter h0 is one-regular (because
 Z ,ho(n) = \／元7 - see Section 7.2, Theorem 7.7 for equivalent characterizations of K-reg
                                                                                           ularity).
Each of the K-identical factors in Eqn. 8.46 adds an extra linear constraint on h0
                                                                                     (actually, it is
one linear constraint on each of the M polyphase subsequences of h0 - see Section 5.10).
     There is no simple relationship between the smoothness of the scaling function and K-
regularity. However, the smoothness of the maximally regular scaling filter, h0, with 琡ed filter
length N, tends to be an increasing function of N. Perhaps one can argue that K-regularity is
                                                                                                  an
important concept independent of the smoothness of the associated wavelet system. K-regularity
implies that the moments of the wavelets vanish up to order K - 1, and therefore, functions can
be better approximated by using just the scaling function and its translates at a given scale. For-
mulae exist for M-band maximally regular K-regular scaling filters (i.e., only the
                                                                                      sequence h0)
ISHGB93J. Using the Householder parameterization, one can then design the remaining filters
                                                                                                  in
the filter bank.
    The linear constraints on h0 that constitute K-regularity become nonexplicit nonlinear con-
straints on the Householder parameterization of the associated filter bank. However, one-regular
                                                                                                  ity
164                                                                                 Filter Banks and Transmultiplexers    Ch. 8



can be explicitly incorporated and this gives a parameterization of all M-band compactly sup-
ported wavelet tight frames. To see, this consider the following two factorizations of H (z) of a
unitary filter bank.
                                               l

                                瓦（:)= H                  [i- P+ z '尸小乞                                                   (8.47)
                                         k=K- 1

and
                                           l

                              町（이         HE'- 아卄-1Q日吼·                                                                  (8.48)
                                         k=K- 1

Since H (1) = V0 and H ' (1) = Wo, V0 = Wi'. The first column of W0 is the unit vector
[H0,0(1), IIo,i (1), . . . , Ho,M_ l (1)]T. Therefore,


                                          ＞二
                                          k=0
                                                   且0,   0,   k ') 2 =
                                                              kI         l·
But since ＞二 ho(n) = Ho(1) = v'Ai,
                                         凡i-1

                                         ＞二 Ho,k(1) = 'I而·
                                         k=0

Therefore, for all k, Ho,k (1) = 赤 . Hence, the first row of Vj is [1/ v'j7, i/ v'M,. . . , i/ ti] . In
other words, a unitary filter bank gives rise to a WTF if the first row of Vo in the Householder
parameterization is the vector with all entries 1/ v'M.
   Alternatively, consider the Given's factorization of H (z) for a two-channel unitary filter bank.



                 瓦（:)=｛立,1：喆
                                                         z_ l sin0i                      cos     sin 9o
                                                                                                                         (8.49)
                                                                          ]}[
                                                         z_ 1 cos0i                  -    Sit)   cos90
                            i=K- 1

Since for a WTF we require

                I 念 金 1= 111o.oc1)
                           Ho, (1)
                                   H1,0(1)
                                                                         =      [    cos
                                                                                                 sin   (e)
                                                                                                                         (8.50)
                [. 七三     市 ]        L                   H1.1(1)                [   -S1flU口)     cos
                                                                                           （인．
                                                                                                         (e)
we have e = Z各l 0, = . This is the condition for the lattice parameterization to be associated
with wavelets.

8.5    Modulated Filter Banks

Filter bank design typically entails optimization of the filter coefficients to maximize some
goodness measure subject to the perfect reconstruction constraint. Being a constrained (or
unconstrained for parameterized unitary filter bank design) nonlinear programming problem,
numerical optimization leads to local minima, with the problem exacerbated when there are a
large number of filter coefficients. To alleviate this problem one can try to impose structural
                                                                                                            165
Sec. 8 5. Modulated Filter Banks


                                                           the desired ideal response, one can im-
constraints on the filters. For example, if Fig. 8.2 is
                                                            are obtained by modulation of a single
pose the constraint that all analysis (synthesis) filters
                                                is the basic idea behind modulated filter banks
"prototype" analysis (synthesis) filter. This
                                                          LV95]. In what follows, we only consider
[Mal92, KV92, Vai92, NK92, GB95b, GB93, Gop96b,
                                                               ampling factor; i.e., L = M.
the case where the number of filters is equal to the downs
                                                             by shifting an the response of an ideal
    The frequency responses in Fig. 8.2 can be obtained
                                                  古）磊，i e {O, . . . ,M - 1}. This can be achieved
lowpass filter (supported in [-k, 希 ]) by (i +
                                                           frequency and arbitrary phase. However,
by modulating with a cosine (or sine) with appropriate
                                                       perfect reconstruction. A general choice of
some choices of phase may be incompatible with
                                                             filter banks of this type) is given by the
phase (and hence modulation, that covers all modulated
following definition of the analysis and synthesis filters:


                          屈的如）cos臼나小응D, 注冗（川                                                               (8.51)




                          gj(n) =g(n) cos（和『三）(n『을）), 注兄（M)
                                                                                                           (8.52)


                                                       phase. Now one can substitute these forms
Here c is an integer parameter called the modulation
                                                             the prototype filters h and g. This is
for the filters in (8.1) to explicit get PR constraints on
                                                       ation over i in (8.1) is a trigonometric sum
a straightforward algebraic exercise, since the summ
                                                           conditions depend only on the parity of
that can be easily computed. It turns out that the PR
                                                      ality, we choose c E {M - 1, M - 2}-other
the modulation phase c. Hence without loss of gener
                                                               filters h and g.
choices being incorporated as a preshift into the prototype
                                                            choice   of modulation phase:
    Thus there are two types of MFBs depending on the
                                                                              -   1 Type 1 Filter   Bank
                                                                                                           (8.53)
                                   (Y =
                                          !M
                                               ( lvi - z                             iype 二 riiter DanK

                                                         down without more notational machinery.
The PR constraints on h and g are quite messy to write
                                                            stood pictori섧ly. Let the 凡l polyphase
But the basic nature of the constraints can be easily under
                                                       into pairs as suggested in Fig. 8.4. Each
components of h and g respectively be partitioned
                                                      pair g (i.e., those four sequences) satisfy the
polyphase pair from h and an associated polyphase
                                                              , these subsequences could be used as
PR conditions for a two-channel filter bank. In other words
                                                             PR filter bank. As seen in Figure 8.4,
analysis and synthesis filters respectively in a tw아channel
                                                         aints on these sequences that PR imposes
some polyphase components are not paired. The constr
                                                       that the PR constraints on the coefficients
will be explicitly described soon. Meanwhile, notice
                                                      constraints (since there are roughly M/2 PR
are decoupled into roughly M/2 independent sets of
pairs in Fig. 8.4). To quantify this, define J:



                                                                                  2
                                                                                  皿邕卑
                                                                                      Type 1, M even
                                                  J
                                                      r
                                          J               1
                                                                                      Type 1, M odd        (8.54)
                                                                                      Type 2, M even
                                                              1
                                                                  j
                                                                                      Type 2, M odd.
                                                                      1
                                                                          \
                                                     into a set of J two-channel PR constraints
 In other words, the MFB PR constraint decomposes
                                                            components of h and g.
 and a few additional conditions on the unpaired polyphase
  166
                                                                                                                                             Filter Banks and Transmultiplexers                              Ch. 8




                                1/                                                                                                                            \              1
                                0                             2                                     M       -
                                                                                                                     2
                                                                                                                                 誓                M   -   3       八1 -   2      M   -1



                                                                       (a) Type 1 入If咀 - M even




                     0
                          (1
                                            l             2
                                                              r
                                                                                 M          -
                                                                                                (
                                                                                                3                    M   -
                                                                                                                             1
                                                                                                                                     \
                                                                                                                                     끄尹                   凡f 小 3
                                                                                                                                                                     \
                                                                                                                                                                         入！ + 2
                                                                                                                                                                                    1
                                                                       (b) Type 1 入4FB - 凡I odd




             1                  /
                                    /
                                                                        I                                                    \                                \ 1
             0                                  2
                                                                  古4
                                                                                                M       -
                                                                                                                2
                                                                                                                                 誓                            凡1- 3            九r 小 2        八   -   1



                                                                  （이 Type 2 卜VIFB - 凡I even




                 0
                     (K
                                        l             2
                                                                                     /／小＼
                                                                                                                                                      \ 1
                                                                            M戶
                                                                                                                M尹
                                                                                                                                          九1- 4       M    ＝므 3      人    -2        入    -   1



                                                                  (d) Tyr比 2 人Ir沼 - 凡／ odd


                                            Figure 8.4. Tw아Channel PR Pairs in a PR MFB


    We first define M polyphase components of the analys
                                                              is and synthesis prototype filters, viz.,
Pi(z) and Q1(z) respectively. We split these sequences furthe
                                                                r into their even and odd components
to give Pi,o(z), Pi, j(z), Q1,o(z) and Q1.1(z) respectively.
                                                             More precisely, let


                          H(z) = 乞 戶m的 = Z 尸師(z삐 + 尸吼 (z삐）,                                                                                                                                              (8.55)
                                                1=0                                             1=0

                                                凡1- i                                       M- i
                               G(z) = Z z1Q小씨 = Z /(Qi,。(z2九1) + ZMQL,i (z2凡1) ),                                                                                                                        (8.56)
                                                    1=0                                         1=0
Sec. 8.5.   Modulated Filter Banks                                                               167


and let

                                     P(z):[*押二：) 소（,(1,z1)(Z)                               (8.57)

with Q(z) defined similarly. Let 工 be the 2 x 2 identity matrix.

Theorem 47 (Modulated Filter Banks PR Theorem) An modulated filter bank (切e 1 or
Type 2) (as de／沇ed in (8.51) and (8.52刀 is PR 涉加n iE 冗（J)

                                                P (z）町 （기 =                                 (8.58)

  口nd fur疏e7刃zore !/ a is even P邑．o(z)Q클 ,0（기 = 右． In 仇e1切e 2 case, 凹e fur坑er require
                   2
PM_1(z)QM_1(z) mm j7 '

The result says that P1, Pa_i, Qi and Q.나 form analysis and synthesis filters of a tw아channel
PR filter bank ((8.1) in Z-transform domain).
   Modulated filter bank design involves choosing h and g to optimize some goodness criterion
while subject to the constraints in the theorem above.

Unitary Modulated Filter Bank
In a unitary bank, the filters satisfy gj(n) = h2(- n). From (8.13) and (8.14), it is clear that in
a modulated filter bank if g(n) = h(- n), then gj(n) = hi(- n). Imposing this restriction (that
the analysis and synthesis prototype filters are reflections of each other) gives PR conditions for
unitary modulated filter banks. That g(n) = h(- n) means that Pi(z) = Qi(ze1) and therefore
Q1(z) = Pj(Ze'). Indeed, for PR, we require
                                                             '       9
                                         P,(z)PT (z ') =i｝工
                                                         .




                                                                                            (8.59)
                                            ,   .   口기           .                           .     .




This condition is equivalent to requiring that Pj and P。  _1 are analysis filters of a two-channel
unitary filter bank. Equivalently, for 1 E 兄(M), P1.o and P1,1 are power-complementary.

Corollary 6 (Unitary MFB PR Theorem) A modulated filter bank (Type 1 or: Type 2) is
unit（工ry 涉加rlE 冗（J), Pz.d기 and P1,1（기 are power complement口丁그／.

                            m기Pd尸）4-         I카'回m戶）      ＝근- ,' iE兄（An                      (8.&fl
                             L,U\'/ .U%, / ' - &.i ,j ' /  A4 ' 1 \ /                        "

Fur仇ermore, 切九en a is e킴en 具 ,小m如何1) = 赤 (i.e., P易0（기 九as to be ；늚z" for some
inteqer k). In 坑e Type 2 case, 凹e／咐坑er require 尸뇨卜K기PM1仁-1) = 유 ／可. e., 尸M-1(기 /ias
1』1 , ,n 9 山 3. Pnm nnm七1 n ;m1 ,/,n』nm1 , '
vo oe - z " jor some inieger 凡).

   Unitary modulated filter bank design entails the choice of h, the analysis prototype filter.
There are J associated two-channel unitary filter banks each of which can be parameterized
using the lattice parameterization. Besides, depending on whether the filter is Ty氾 2 and/or
alpha is even one has to choose the locations of the delays.
   For the prototype filter of a unitary MFB to be linear phase, it is necessary that

                                        P小K기 = 名_2k+lpi(z_1),                               (8.61)
168                                                                                      Filter Banks and Transmultipiexers                 Ch. 8

for some integer k. In this case, the prototype filter (if FIR) is of length 2Mk and symmetric
about (Mk - 古 ) in the Type 1 case and of length 2Mk - 1 and symmetric about (Mk - 1)
(for both Class A and Class B MFBs). In the FIR case, one can obtain linear-phase
                                                                                        prototype
filters by using the lattice parameterization [VH88] of two-channel unitary filter banks. Filter
banks with FIR linear-phase prototype filters will be said to be canonical. In this case, P1(z) is
typically a filter of length 2k for all 1. For canonical modulated filter banks, one has to check
power complementarity only for 1 E 冗（J).


8.6    Modulated Wavelet Tight Frames
For all Al, there exist Al-band modulated WTFs. The simple linear constraint on h0 becomes
a set of J linear constraints, one each, on each of the J two-channel unitary lattices associated
with the MFB.

Theorem 48 (Modulated Wavelet Tight Frames Theorem) Every compactly
                                                                               supported mod-
ulated WTF is associated with an FIR unitary MFB and is parameterized by J unitary lattices
suc／工 坑at 坑e sum o/ 坑e ai四les in 坑e lattices satis力／ 伽r 1 e 7 (J)) Eqn. 8. 62.


                              ＞二q泮毛 극 느和和）·                                                                                               (8.62)
                                 k


If a canonical MFB has Jk parameters, the corresponding WTF has J (k - 1) parameters.
    Notice that even though the PR conditions for MFBs depended on whether it is Type 1
                                                                                          or
Type 2, the MWTF conditions are identical. Now consider a Type 1 or Type 2 MFB with one
angle parameter per lattice; i.e., N = 2M (Type 1) or N = 2M - 1 (Type 2). This angle
parameter is specified by the MWTF theorem above if we want associated wavelets. This choice
of angle parameters leads to a particularly simple form for the prototype filter.
    In the Type 1 case [GB95b, GB93J,

                                       ／万4        /       7r

                               h(n) = V j jsiI1(4ij(2n+ l)).                                                                              (8.63)

and therefore


  h2(n）小小(7r('" ':;" " ")                                                            (                                            \
                                                                                                                                  11
                                                                                                                                   /
                                                          冗 14                                                                   兀H
                                                                                                                                  4
                                                                                                                                      ]
                                                                                                        +
                                                                                 \
                                              2
                                                      m
                                                      l                              n
                                                                                                                                           R
                                                                                                                                           니
                                                                                                                                               d
                                                                                                                                               1
                                                                             \
                                              n
                                              乙
                                              1




                                                                                                                            1)
                                                                                          "i
                                                                                                   (n
                                                                         1
                                                                                     S                      .
                                                                                                                                               n
                                                                                                                                               b

                                                                                                        M
                                                                                                                     (2i+
                                                                     1
                                                                 /
                                                                 /
                                                                                                                5)
   In the Type 2 case [GB95b},

                                     .   /2           f ir .                         .\
                                 h(n) = VM5in ()ji (n+ l))                                     1                                          (8.65)

and hence


  h加＝'I퓨卜（"（「" 깝’" ') (27
                      (2i+1)
                       『1){),51
                             J_ sin0(iri M
                                        (n--i) (2汁1){)} 侶66)
 Sec. 8.7    Linear Phase Filter Banks
                                                                                                169

 8.7        Linear Phase Filter Banks
In some applications, it is desirable to have filter banks with linear-phase filters [SVN93J. The
linear-phase constraint (like the modulation constraint studied earlier) reduces the number of
 free parameters in the design of a filter bank. Unitary linear phase filter banks have been studied
recently [SVN93, GB94b}. In this section we develop algebraic characterizations of certain types
of linear filter banks that can be used as a starting point for designing such filter banks.
    In this section, we assume that the desired frequency responses are as in (8.2). For simplicity
we also assume that the number of channels, Al, is an even integer and that the filters are FIR.
It should be possible to extend the results that follow to the case when M is an odd integer in a
straightforward manner.
     Consider an M-channel FIR filter bank with filters whose passbands approximate ideal filters.
Several transformations relate the M ideal filter responses. We have already seen one example
where all the ideal filters are obtained by modulation of a prototype filter. We now look at
other types of transformations that relate the filters. Specifically, the ideal frequency response of
/1Ar'-leican be obtained by shifting the response of the h, by ir. This either corresponds to the
restriction that


       h凡ielei(7i) = (- 1少屈(n) ; HMlmi（기 = 瓦(- z) ; 丑入imlmi(W) = 珏佃＋ir),                      (8.67)

or to the restriction that


 hM寸1-i（미 = (- 1少h (N- 1- n) ; 且凡1-1-i（기 =.1／尹（-z) ; 月凡1-1小i(w) =I칵（回＋미 (8.68)


where N is the filter length and for polynomial H (z), HR(z) denotes its reflection
                                                                                       polynomial
(i.e. the polynomial with coefficients in the reversed order). The former will be called pairwise-
 shift (or PS) symmetry (it is also known as pairwise-mirror image symmetry [NV88]) , while
the latter will be called p口勿낀'ise-coni四毗e小就沂 (or PCS) symmetry (also known as
                                                                                         pairwise-
symmetry [NV881). Both these symmetries relate pairs of filters in the filter bank. Another type
of symmetry occurs when the filters themselves are symmetric or linear-phase. The only type of
linear-phase symmetry we will consider is of the form


                               凡（미 = 士／z2(N- 1- n) ; 珏（기 = 士I甘떠，

where the filters are all of fixed length N, and the symmetry is about 쁘尹· For an M-channel
linear-phase filter bank (with M an even integer), M/2 filters each are even-symmetric and odd-
symmetric respectively [SVN93].
    We now look at the structural restrictions on H (z), the polyphase component matrix
                                                                                            of the
analysis bank that these three types of symmetries impose. Let J denote the exchange matrix with
ones on the antidiagonal. Postmultiplying a matrix A by J is equivalent to reversing the order of
the columns of A. and premultiplying is equivalent to reversing the order of the rows of A. Let V
denote the sign-alternating matrix, the diagonal matrix of alternating 士1's. Postmultiplying
                                                                                                by
170                                                                Filter Banks and Transmultiplexers    Ch. 8


V, alternates the signs of the columns of A, while premultiplying 缸ternates the signs of the rows
of A. The polyphase components of H (z) are related to the polyphase components of HR(z) by
reflection and reversal of the ordering of the components. Indeed, if H (z) is of length Mm, and
        入f- i
且（z) = 乞 戶局（少), then,
           1=0



                         끄R（기 = z凡1m+1 三 y局（:‘八J)
                                              1=   0


                                 = Z戶M-나- inM+ A偏(zM))
                                     1=0
                                     入f-i

                                 = ＞二zm11珤-i니          仁M)     .



                                     1=0

Therefore
                                  （且R)i（기 = (H入f-i- I) （기                                               (8.69)

and for linear-phase H (z), since HR(z) = 士且（2),

                                   H1（기 = 士 '
                                           （zjR
                                              ' )M-i나（名）.                                               (8.70)

Lemma 1 For even 凡I, ／乙（기 is o/ 坑e foi斗n

PS Symmetry

           [ w0（기             Wi（기      ] H1 /         0 ] [ w0（기               I仍（기
                                                                                                        (8.71)
           LJW0(z)V      (_1)M12JW1(z)V j - [ 0        J j L Wo(z)V         (_1)M12W1(z)V


PCS Symmetry

           I   Wo(z)          Wi(z)J   1 - I '               0 ] I Wo（기                Wi（之）J       ]
           [ J14／尹（z)V   (_l)M/2JI磅떠Jv ] 中 [ 0               J] L W1' (z)V       (_i) TM! 2 W 仁)JV ]
                                                                                                  (8.72)

Linear Phase


                     ［訊z)z) D唱器小［訊z)z) D唱多｛:; ]［二 J0                                                    (8.73)

      or

                    이趾］ 器걺H田z)z) 堺訂［二 J0                                                                (8.74)
Sec. 8.7. Linear Phase Filter Banks                                                                                                   171

Linear Phase and PCS


        [     Wo(z)
            JDWo(z) V
                               DWj (z)J    1- [ '
                           (_1)M72JW (Z)JV j - [ 0
                                                                               0 1 1 Wo(z)
                                                                               J ] [ DW0(z)V
                                                                                                                      DW (z)J
                                                                                                                  (_ 1)M/2W (z)JV j
                                                                                                                                   1

                                                                                                                                (8.75)

Linear Phase and PS

       [  Wo(z)                 DW (z)J         1 -. 1 '                        0 i f  Wo(z)                          DW (z)J       1
       L JW0(z) V        (_ 1)It"h/ 2JDWJ?(z)JV ] - L 0                        JD j [ DW0(z)V                     (_ 1)M12Wj (z)JV ]
                                                                                                                                (8.76)


    Thus in order to generate H (z) for all symmetries other than PS, we need a mechanism that
generates a pair of matrices and their reflection (i.e., Wo (z), Wi (z) W (z) and Wf (z)). In the
scalar case, there are two well-known lattice structures, that generate such pairs. The first case
is the orthogonal lattice [VH88], while the second is the linear-prediction lattice [R583]. A Kt九
order orthogonal lattice is generated by the product

                                                                욱
               位［므；
                  , 二：:]}[                   b i q12
                                                            1       匈 幻
                                             l

                          m小
                                                                        凹姓z) 凞十‘x（기·
                                                            1
                                     2                      1
                                                                                               寸




                                             l
                                                            1
                                    2
                                                            \
                                                                                               H

                                                                                                         中




This lattice is always invertible (unless ai and b1 are both zero!), and the inverse is anticausal
since

                                    ［툐 二二］" = ,/，小‘                                                ;：寸
As we have seen, this lattice plays a fundamental role in the theory of two-channel FIR unitary
modulated filter banks. The hyperbolic lattice of order K generates the product

                     K
                     nM
                                                                D
                                                                1
                          ai 2
                                                                          이：
                                                                           ｝目 凞十‘如·
                                                                                                                                 /
                                                                    0
                                                                                                                                 1
                           D
                           1
                                                                                                                                 j
                                                                n   0
                                                                                                                                 /]
                                                                                                                                 \
where Yo(z) and Yi(z) are of order K. This lattice is invertible only when a 7E b? (or equivalently
(a + b1) /2 and (a1 - b1) /2 are nonzero) in which case the inverse is noncausal since

                                                       z 1b            1       r
                                    [:
                                             :         r뇨：          口三 - by L -zb1                 ；기·
Since the matrix     [
                     ./
                   L b2  a1 i
                     (Ji (1i
                              .跏
                               b,        ]
                                      orthogonal i什
                                            -
                                                       , ,
                                                       be
                                                           -
                                                             =
                                                                     -
                                                                       , .:
                                                                          ｛口
                                                                            {a力z} = {0，士1}, the
                                                                                   b가   ｛士1,                 0}
(2 x 2) matrix generated by the lattice can never be unitary.
    Formally, it is clear that if we replace the scalars a1 and b1 with square matrices of size
M/ 2 x AI/ 2 then we would be able to generate matrix versions of these two lattices which can
then be used to generate filter banks with the symmetries we have considered. We will shortly
see that both the lattices can generate unitary matrices, and this will lead to a parameterization
of FIR unitary H (z) for PCS, linear-phase, and PCS plus linear-phase symmetries. We prefer
to call the generalization of the orthogonal lattice, the antis ymmetric lattice and to call the
 172                                                                           Filter Banks and Transmultiplexers     Ch. 8


generalization of the hyperbolic lattice, the symmetric lattice, which should be obvious from the
form of the product. The reason for this is that the antisymmetric lattice may not generate a
unitary matrix transfer function (in the scalar case, the 2 x 2 transfer function generated is always
unitary). The antisymmetric lattice is defined by the product

                                             K
                                             nm
                                     r
                                     11<1L                                                    ］
                                 呵
                          x（기                      A丑                                                               (8.77)
                                                        z 1A]
                                                        z:
                                                              1B
                                                                         }［쏘
                                                                                  ,   B0A。
where Ai and B are constant square matrices of size M/2 x M/2. It is readily verified that X(z)
is of the form

                                     x（기＝［難：) 韋目］                                                                   (8.78)

Given X(z), its invertibility is equivalent to the invertibility of the constant matrices,


            ［名 三：] since［소‘ 二：'B小나‘ 三：]                                                        '
                                                                                              LO
                                                                                              1
                                                                                                    zH'Ij
                                                                                                      L]
                                                                                                            '
                                                                                                                    (8.79)

which, in turn is related to the invertibility of the complex matrices C7 = (A: + zB1) and D7 =
(Ai 寸 2夙）1since,

                                                  0D    J
                                                        r J
                                                          !
                    出 三，][ci
                         1。                                        -21 ] = [ A7
                                                                    ii ]
                                                                                 且 ]
                                                                           1- Bi 凡 .1 "
Moreover, the orthogonality of the matrix is equivalent to the unitariness of the complex matrix C1
(since D, is just its Hermitian conjugate). Since an arbitrary complex matrix of size M/2 x M/2
is determined by precisely 2
                               們'小岫「s,ea的the matrices
                                                   ［名 三：]5朗！hat
many degrees of freedom. Clearly when these matrices are orthogonal X(z) is unitary (on the
unit circle) and XT(zel)X(z) = I. For unitary X(z) the converse is also true as will be shortly
proved.
   The symmetric lattice is defined by the product          .
                                     呵
                           x（기
                                     位［盒 :::g: ]}［盒 三：]                                                             (8.80)

Once again A7 and B7 are constant square matrices, and it is readily verified that X(z) written
as a product above is of the form


                                     如＝［凞） 凞）I       Y0（기          }7.（기
                                                                                                                    (8.81)

The invertibility of X(z) is equivalent to the invertibility of


               ［各 三：] 師ce ［各 煮小［盒 三：][: z 0'I                                                                   (8.82)

which in turn is equivalent to the invertibility of G'i 4 (凡 + B7) and D7 = (A2 - B2) since

                      n. J / ] [ (7i 0 ] r J I 1= H                                          Bj 1
                      2[ I     -Ij    [ 0         D1 ] [I          -Ij         [B,           A1 ]
       Sec. 8.7. Linear Phase Filter Banks
                                                                                                                                                                                           173


      The orthogonality of the constant matrix is equivalent to the orthogonality of the real matrices

                and D, , and
                                                                                                                                                                                           2)
     C,
                               since
                                         each real orthogonal matrix of                                                        2 x                2 is                    by
                                                                                                                               )
                                                                                                        size
                                                                                                                     M/
                                                                                                                                             M/
                                                                                                                                                         determined
                                                                                                                                                                               (찡
               「3   「8, the
                『0 (0   (500. 0513m.
                            constant          『3m006537022
                                     orthogonal matrices
                                     「15.                           of freedom. Clearly
                                                                                                               (M/
                                                        2
 parameters,
                                                      8m31
 m
                                                                                                 have
                                                                                                                                   degrees
                                                                                                                                                                                    when
                                                                                                                          2\
 the matrices are orthogonal XT(z_ i)X (z) = I. For the hyperbolic lattice too, the converse is
 true.
    We now give a theorem that leads to a parameterization of unitary filter banks with the
 symmetries we have considered (for a proof, see [GB94b}).

Theorem 49 Let X (z) be a unitary M x M polynomial matrix of degree K. Depending
                                                                                              on
whether X(z) is of the form in (8.78), or (8.81), it is generated by an order K antisymmetric or
symmetric lattice.



Characterization of Unitary H (z) -                                              PS Symmetry
The form of H (z) for PS symmetry in (8.71) can be simplified by a permutation. Let P be the
permutation matrix that exchanges the first column with the last column, the third column with
the last but third, etc. That is,


                                                                                                             00 1
                                                                                                                110 0 0
                                                                            0l0 1




                                                                                          000 1
                                                                                110 0 0




                                                                                              11l 0 0
                                                                                                           上
                                                                                                           1
                                                                                                           1

                                                                                                           000  1
                                                                                                                110   0
                                                                                                                   l4
                                                                            000 1
                                                                                110 0 l
                                                 P=
                                                                                                           00l 1110 0 0




The
 【奴毗미出(z)
      z)V 回統없印卜小川can b毗恤帥朗시 羽目 訊z)z) 므
and therefore




                                                         口k三扼三扼三而
                                                                        0J / 0
                                                                               ] [ wo（기                     Wi（기
                                       끄d기
                                                                               .1 L Wo(z)V              (_1)M12lVi(z) V

                                             = 士［: 川瑥；?) 趾小
                                                                    m

                                                                    1

                                                                    1

                                                                1

                                                                L




                                                                        r/ 0
                                             : 士［二 J0 ［二 }]［텍') W0(z)
                                                                1




                                                                                                                                                                      P
                                                                1




                                             = 士［二 川텍') W (z)
                                                                戶




                                                            O:)]P
                                                                1

                                                                1

                                                                L




For PS symmetry, one has the following parameterization of unitary filter banks.
174                                                                                                              FiIter Banks and Transmultip1exers        Ch. 8


Theorem 50 (Unitary PS Symmetry) H (z) of order K forms a unitary PR filter bank with
PS symmeti김 涉 坑ere e娩就 unit口ry, order K, 凡1/ 2 )< 凡i/'2 matrices W （기 (m72d 功'{ (z), si工ch th毗


                                                   H (z)=1小， JI 凹') W0(小·
                                                                                                                                                                 8
                                             /1\                                                                                                           八乂니
                                                                                                                                                                     nd




                                                         .       ..-    - .   .. (M12'\
A  “可   '扼H 凹1坑 尸S
             『y    「，        is           by 끄『ecisety 2
                                                   symm랴四    2    (Lo + Li) + 2       de    比竹nined                 (M/        -   i)                    \d)
p口rameters n加re q 之 K andL1 > K are 琉e 凡Ic凡lilian degrees of W （기 and W （기 res끄ectively.



Characterization of Unitary H (z) -                                                         PCS Symmetry
In this case


                                   月p（기                     =
                                                                            [
                                                                            /
                                                                            r
                                                                            rt1

                                                                                  0
                                                                                           0 ] [ Wo（기              WI（까J        ]
                                                                                           J] I W11 (z)V    (- 1) TM72WJ' (z)JV j
                                                            def
                                                                       ［二 J0 -（믐三）
                                                                                R 冊，]
                                                                       [: J0 -楹）R 儡R] [: g] 7·
Hence from Lemma 1 H (z) of unitary filter banks with PCS symmetry can be parameterized as
follows:

Theorem 51 HP(z) forms an order K, unitary filter bank with PCS symmetry if


                                                                                  K
                                                                                  nm
                                                                                   ［立， z:1B1}［名 三：][: 小
                                                                            /
                                                                                                                                                          (8.84)
                                                                            J
                            (z)         ［二
                                    =
                                                                            11
                                                            J0              (
                        H                                                   \
 where
『』6dA1-B, BA小「ec毗stant如小而ces.
parameters.
                                                                                                                   characterized by 2K
                                                                                                               （기 7m. m0!
                                                                                                              耳，          is
                                                                                                                                          6m646m
                                                                                                                                                         (M/
                                                                                                                                                           2
                                                                                                                                                                 2
                                                                                                                                                                     '\
Characterization of Unitary H,(z) -                                                         Linear-Phase Symmetry
For the linear-phase case,


                  m（기 = 이Wo(z)
                          Wi 器二［二 J0
                                  -     1, [ J                               ' 1 1 Wo(z) +Wi(z)               W (z) -W/ ?(z) ] [ /                 0 1
                                  H     巨낳 [ /                   甘1上
                                                                            -I ] [ 1'Vo(z) - W1（기             W寸（z) + 14'껀（기 ] [ 0                 J ]
                                                                       1/
                                                                 m



                                  def         1 ,) [ /                            I ] 1 叫 （기                W{（기 ] [ /                  0 ]
                                                                       rJ
                                                                                                                               0
                                             7닉[ I               1
                                                                                  _Ij L (WflR(z)           (W)h?(z) ] [0                Jj .

Therefore, we have the following Theorem:
Sec. 8.7. Linear Phase Filter Banks                                                                                                                                                                                                                       175


Theorem 52 HP(z) of order K. forms a unitary filter bank with linear-phase filters if



                                                                                                                         [    AB                        BA
                                                                                                                                                                                                                       ]［二
                                                                                                                                                                          \
                                                                                          !      기   (         K

                                                                                          '1 Un                                           2 2
                                                      4
                                                                                                                                                                          1(
                                                                                                                                                                                                                                                         (8.85)
                       H    (z)       ＝     늉
                                                      1




                                                                       ［;
                                                                                      -      j L. 1  lii       1=
                                                                                                                                                                          r
                                                                                                                                                                          J
                                                                                                                                                                                    ［守
                                                                                                                                                                                               三：                          J0        ,




where［玄 骨 are consta毗毗hogonalma！砒es. H (z) is characterizedby 2K（찡'）「
rameters.
                                                                    『
Characterization of Unitary H (z) 中 Linear Phase and PCS Symmetry
In this case, H (z) is given by

                                                                                          0J
                                                                            r11
                           /7P（기
                                                =                      r J  [     0
                                                                                      0 ] [  Wo（기                                             .1까g2（三）J   ]
                                                                                        ] L DW0(z) V                                      (- 1)' 'W (z)JV J
                                                def

                                                                                  [ J0 나砥기 瑥澔n/
                                                                                          rJ 0




                                                                                          ]［텍 （叫？ ]［二 ]
                                                                                  戶

                                                                                  1

                                                                                  1
                                                                                          I      0 ] [ I                             D
                                                                                  1
                                                                                          0      Jj L- D                             I                                                                                          J0
                                                                                                                                                                                                                                         P.
                                                                                  L                                                                                            ')                   R   (z)
Therefore we have proved the following Theorem:
Theorem 53 H (z) of order K forms a unitary filter bank with linear-phase and PCS filters if
仇ere exis拓 a unitary, order ／乙 凡1/ 2 )< 凡1/2 matrix W （기 such 坑口t


                                            H (z）伉口. DJ［텍') （叫？2R(z)
                                                                 (:) lj rj
                                                                        t。01
                                                                           jjP.                                                                                                                                                                          (8.86)

                                                                                                                                                                                    +
     this case                                                                                   by precisely                                   2                         L                                                          where L2             K is
                                                                                                                                                                                         (M/
In
                                  H
                                      (z)        is
                                                          determined
                                                                                                                                   (M/              -    1)
                                                                                                                                                                                                              parameters
                                                                                                                                                                                               2)
坑eMc凡fill（工n degree o/ 叫 （z) .

Characterization of Unitary H (z) -                                                                                      Linear Phase and PS Symmetry
From the previous result we have the following result:
Theorem 54 H (z) of order K forms a unitary filter bank with linear-phase and PS filters if
there exists a unitary, order K, M/ 2 x M/ 2 matrix W (z) such that


                                            H (z）伉［ 1, 品］[W。(z) (TV和(z)出 小·                                                                                                                                                                              (8.87)
                                                                                                                              +
H    is                                         by precisely                                         2                    L               112)                                                      where L2               K is the
                                                                                                                                     ('
          determined                                                                      (M/
                                                                                                           -        1)
                                                                                                                                                             parameters                                                                       McMillan
degree of W (z).
     Notice that Theorems 50 through Theorem 54 give a completeness characterization for unitary
filter banks with the symmetries in question (and the appropriate length restrictions on the
filters). However, if one requires only the matrices W (z) and W{ (z) in the above theorems
to be invertible on the unit circle (and not unitary), then the above results gives a method to
<eiierate nonunitary PR filter banks with the symmetries considered. Notice however, that in
1lie nonunitary case this is not a complete parameterization of all such filter banks.
176                                                                       Filter Banks and Transmultiplexers    Ch. B


8.8       Linear-Phase Wavelet Tight Frames

A necessary and sufficient condition for a unitary (FIR) filter bank to give rise to a compactly
supported wavelet tight frame (WTF) is that the lowpass filter h0 in the filter bank satisfies the
linear constraint [GB92c]
                                              ＞二九。(n) = Vi i.                                                  (8.88)
                                               n


   We now examine and characterize how H,(z) for unitary filter banks with symmetries can be
constrained to give rise to wavelet tight frames (WTFs). First consider the case of PS symmetry
in which case H,(z) is parameterized in (8.83). We have a WTF if

                         first row of H (z)I,_1 = [ 1/ v'i              . . . 1/ V's?                          (8.89)

In (8.83), since P permutes the columns, the first row is unaffected. Hence (8.89) is equivalent
to the first rows of both W (z) and W1'(z) when z = 1 is given by

                                        [ \／百/M ... \／刃M ] ·

This is precisely the condition to be satisfied by a WTF of multiplicity M/2. Therefore both
W (z) and Wf (z) give rise to multiplicity M/2 compactly supported WTFs. If the McMillan
degree of W (z) and Wf (z) are L0 and L1 respectively, then they are parameterized respectively
      / A
        "J'/ 1) H ]' \                    / 入
                                            "/"/ 9 H ]' \
by ( '' /5 ' J + (M/2 - 1)L0 and ( " ' 5 ' J + (M/2 - 1)Li parameters. In summary, a
                                                                               /1 ",rln     i\

WTF with PS symmetry can be explicitly parameterized by 2 ( ""' ': 1 ') + (M/2 - 1) (L。+ Li)
                                                                \    口   /
parameters. Both L0 and L1 are greater than or equal to K.
    PS symmetry does not reflect itself as any simple property of the scaling function 伽(t) and
wavelets 吻(t), i E {1, . . . , M - 1) of the WTF. However, from design and implementation points
of view, PS symmetry is useful (because of the reduction in the number of parameters).
    Next consider PCS symmetry. From (8.84) one sees that (8.89) is equivalent to the first rows
of the matrices A and B defined by


                                                                                    \
                                                                                    11t
                                                                                      r1J
                                                       (   0                   弓
                                [A-B 朴LK냐，liiA,
                                    .     _        ,           r    .     11




are of the form [ 1/ v'M . . . 1/ VTA1 ] . Here we only have an implicit parameterization of
WTFs, unlike the case of PS symmetry. As in the case of PS symmetry, there is no simple
symmetry relationships between the wavelets.
   Now consider the case of linear phase. In this case, it can be seen [SVN93I that the wavelets
are also linear phase. If we define


                                                                                J
                                                           0

                                                                   AB   BA
                                    AB사｛如 B
                                                                                \
                                                                                1
                                                                                \
then it can be verified that one of the rows of the matrix A + B has to be of the form
 [ \/57i7 ... \/7M ]. This is an implicit parameterization of the WTF.
Sec. 8.9.   Linear-Phase Modulated Filter Banks                                                              177

     Finally consider the case of linear phase with PCS symmetry. In this case, also the wavelets are

然烈業스쑈騈弓耕"叫弔搬窟品瑥瑥恣器烈烈喆，誌
 2 W:E
M/
M/ WTF. 12 1岫
           this 呼 the W1
                  毗
                 In   WTF
                       「 18
                          is by
                             67 9
                            case,
                                precisely
                                          (M/ 2
                                              2
                                                )+ 2 L
                                                  mm0
                                                  parameterized
                                                                       《0
                                                                        「1204    「岫017
                                                                                         -
                                                                                                  (M/   -     1)
parameters where L 2 K is the McMillan degree of W (z).



8.9      Linear-Phase Modulated Filter Banks

The modulated filter banks we described

     1. have filters with nonoverlapping ideal frequency responses as shown in Figure 8.2.


     2. are associated with DCT III/ IV (or equivalently DST III/ IV) in their implementation


     3. and do not allow for linear phase filters (even though the prototypes could be linear phase).

In trying to overcome 3, Lin and Vaidyanathan introduced a new class of linear-phase modulated
filter banks by giving up 1 and 2 [LV951. We now introduce a generalization of their results from
a viewpoint that unifies the theory of modulated filter banks as seen earlier with the new class of
modulated filter banks we introduce here. For a more detailed exposition of this viewpoint see
[Gop96b].
     The new class of modulated filter banks have 2M analysis filters, but M bands-each band
being shared by two overlapping filters. The M bands are the M-point Discrete Fourier Transform
bands as shown in Figure 8.5.


                                          梳＝{ 亨 툐｛
                                                 ，「，
                                                   껜                                                        (8.90)


Two broad classes of MFBs (that together are associated with all four DCT/DSTs [RY90]) can
be defined.




                      -ir                H끄L
                                          2凡1
                                                                  小_!E (1
                                                                   2八t '
                                                                            그二
                                                                            2M   搗           7r

                                                                       w

            Figure 8.5. Ideal Frequency Responses in an M-band DFT-type Filter Bank
178                                                                                                Filter Banks and Transmultiplexers     Ch. 8


DCT/DST I/ Il based 2M Channel Filter Bank

                                                                                       Q尸
                                                                                        2
                                                                                                              曷
                           h   (n)           =     k小       （n) cos （쥬秀       n-
                                                                              （
                                                                                            \1J/     iE                                 (8.91a)

                                                                                                                  品
                      九M卄回 小枷- M) sin（유土（n을）) , 可E                                                                                  (8.91b)

                                                                                                              S
                           吼(n) ＝丸zg(Ti)cos（命（n+ 을）),                                                         l
                                                                                                              E
                                                                                                      2                                 (8.91c)

                                                                                   i
                                                                                                                  e   品
                     9M+   佃）=－自g(n+M)sin（유i(.十 을）) , 2                                                                                 (8.91d)

The sets S1 and S2 are defined depending on the parity of a as shown in Table 8.1. When a is
even (i.e., Type 1 with odd M or Type 2 with even M), the MFB is associated with DCT I and
DST I. When a is odd (i.e., Type 1 with even M or Type 2 with odd M), the MFB is associated
with DCT II and DST II. The linear-phase MFBs introduced in [LV95] correspond to the special
case where h(n) = g(미 and a is even. The other cases above and their corresponding PR results
are new.

                                                                         S                        S2
                  a even, DCT/DST I                               冗（M) u{ M}                  兄（M)\{O}
                  a odd, DCT/DST II                                 兄(M)                    冗(M)\ {O} u {M}


                  Table 8.1. Class A MFB: The Filter Index Sets S1 and S2

     The PR constraints on the prototype filters h and g (for both versions of the filter banks
above) are ex口et匈 坑es口me as th口t for 坑e modulated filter ban丸 就1｛硫ed earlier {Gop96b]. When
the prototype filters are linear phase, these filter banks are also linear phase. An interesting
consequence is that if one designs an M-channel Class B modulated filter bank, the prototype
filter can also be used for a Class A 2M channel filter bank.


8.10    Linear Phase Modulated Wavelet Tight Frames

Under what conditions do linear phase modulated filter banks give rise to wavelet tight frames
(WTFs)? To answer this question, it is convenient to use a slightly different lattice parameteri-
zation than that used for Class B modulated filter banks. A seemingly surprising result is that
some Class A unitary MFBs cannot be associated with WTFs. More precisely, a Class A MFB
is associated with a WTF only if it is Type 1.



                   ［出，（
                     目 寐小川，小寸蜘）                                                                                                          (8.92)


where
                                     T
                                         '
                                             (O)        =    [    cosOlk
                                                                 - Sin 91,k
                                                                                   Z 'SiflOj,k
                                                                                   z 'c0591,k .
                                                                                                          '
 Sec. 8.11. Time-Varying Filter Bank Trees
                                                                                                  179

    With this parameterization we define 0i as follows:



                            너｛,(::) 豁小口鼎)                         sin(01)
                                                                  cos   )
                                                                      (0,
                                                                                                (8.93)


                                   k1-1
 where in the FIR case 0i = 乞 9i,k as before. Type 1 Class A MFBs give rise to a WTF if
                                   k=O
 ei = 퓽 for all 1 E I之（J).

Theorem 55 (Modulated Wavelet Tight Frames Theorem) A class A MFB of Type 1
gives rise to a WTF if 01 = 퓽 . A class B MFB (Type 1 or Type 2) gives 仇se to a WTF
涉 ei = 퓽 + 곬7（을 - 1).


8.11      Time-Varying Filter Bank Trees

Filter banks can be applied in cascade to give a rich variety of decompositions. By appropriately
 designing the filters one can obtain an arbitrary resolution in frequency. This makes them partic-
ularly usef따 in the analysis of stationary signals with phenomena residing in various frequency
bands or scales. However, for the analysis of nonstationary or piecewise stationary signals such
 filter bank trees do not suffice. With this in mind we turn to filter banks for finite-length signals.
      If we had filter bank theory for finite-length signals, then, piecewise stationary signals can
be handled by considering each homogeneous segment separately. Several approaches to filter
banks for finite-length signals exist and we follow the one in [GB95a]. If we consider the filter
bank tree as a machine that takes an input sample(s) and produces an output
                                                                                      sample(s) every
instant then one can consider changing machine every instant (i.e., changing the filter coefficients
every instant). Alternatively, we could use a fixed machine for several instants and then switch
to another filter bank tree. The former approach is investigated in [PV96]. We follow the latter
approach, which, besides leveraging upon powerful methods to design the constituent filter bank
trees switched between, also leads to a theory of wavelet bases on an interval [HKRV93, GB95a].
     Let H (z), the polyphase component matrix of the analysis filter bank of a unitary filter bank
be of the form (see (8.27))
                                                 K- i
                                             馬回＝ 三b （枷止                                         (8.94)
                                                 k=O

It is convenient to introduce the sequence x = ［· · · , T (0), x(_1), . . . , x(- M + 1), x(M), x(M -
1), . · ·} obtained from x by a permutation. Then.




             d = 甘爻 d竺         '    怖佯- 1)      怖佯小2)      ·11 怖(0)           0     "   jt,    (8.95)
                                     0          h低- 1)     . . . h9(1)      h (0)
180                                                                                                                        Fflter Banks and Transmultiplexers                 Ch. 8


and H is unitary if H is unitary. (8.28) induces a factorization of H (and hence H). If V0 =
diag(Vo) and




                   vZ   =
                                         /Ji           /             尸；            0                                      for i E {1. . . . .K- 1}.                     (8.96)
                                          0                        P,          /       尸？



                                                                                                0
                                                                               ci= fl v1.                                                                               (8.97)
                                                                                         i=K- 1

The factors Vi, with appropriate modifications, will be used as fundamental building blocks for
filter banks for finite-length signals.
     Now consider a finite input signal x = [x(O). x(1), ' . ,x(L - 1)1, where L is a multiple of Al
and let 文 = [x(M - 1),. . . ,x(O),x (M). . . . . x(L 中 1). . . · ,x(L- M)]. Then, the finite vector d
(the output signal) is given by

                  =h (K - 1)                      ...                     h,(O)                 0                                                                  1)

                            0           h (K - 1)                              ...          h (0)
d = 甘文 望

                                                                                                0          h (K - 1)                        ...          hP(0)     0
                            0                                                                                  0                         h (K - 1)        .. .   h (O) -

H［iis, ,an
戶        , (L N+
         比－   -  A/) ,x L matrix,
               + M)             , 工m,, , , N = MK
                                         t,    凡iKiis, , h
                                                   .   the, l , , , .h , nh
                                                           where
                                                           Wh             the
                                                                          N＝  filters.
                                                                            , 6h,  ,,  w , i,
                                                                                       W since         98)
                                                                                              , , the r。ws   length           。f                .   N。
                                                                                                                                                    N,                  (8.
O1 H are mutuanv ortnonormai (i.e.. nas ranx LI. one nas to aDnena IV - M = IVI (it - 1) rows
irom tne ortnogonai complement O1 11 to maKe tne map trom x to an augmentea a unitary. io
get a complete description of these rows, we turn to the factorization of H,(z). Define the L x L
matrix V0 = diag(Vo) and for i E {1,. . . , K - 1} the (L - Mi) x (L - Mi + M) matrices

                                         P             I- P                          0              ...                              0
                                              0                    P,          I-        P2         .
                                Vi =                                                                                  0              .
                                                                                                                                                                    (8.99)

                                                                                       0            只       / 小只                     0
                                              0                                      . ..           0         P                    / H 尸i

                                                                                            0
then甘 is readily verified by induction to be [J                                                         Vt. Since each of the factors (except V0) has
                                                                                       i=K- 1
M more columns than rows, they can be made unitary by appending appropriate rows. Indeed,
IB, 1
I Vi i isunitarywhere, B7= {Tf (I- P1) 0 . . . 01, andC7= [0 . . . 0 므？e . ] .
' ci '
Sec. 8.11   Time-Varying Filter Bank Trees                                                               179


    With this parameterization we define e1 as follows:

                            너｛(1)) 豁小［                      cos   (Oi)
                                                            寸 sin(e1)
                                                                                 sin
                                                                                cos
                                                                                       (ei)
                                                                                        (e1)
                                                                                                        (8.93)


                                    k,-i
where in the FIR case Ei = >               9Lk as before. Type 1 Class A MFBs give rise to a WTF if
                                    k=O
e1 = 즐 幻r all 1 E I之（J).

Theorem 55 (Modulated Wavelet Tight Frames Theorem) A class A MFB of Type 1
g切es 仇se to 口 WTF 涉 e1 = 퓽· A class B MFB (7切死 1 or 7切e 2) g切es 仇se to 口 WTF
涉ei = 퓽 + 希（을 - 1)·


8.11        Time-Varying Filter Bank Trees
Filter banks can be applied in cascade to give a rich variety of decompositions. By appropriately
designing the filters one can obtain an arbitrary resolution in frequency. This makes them partic-
ularly useful in the analysis of stationary signals with phenomena residing in various frequency
bands or scales. However, for the analysis of nonstationary or piecewise stationary signals such
filter bank trees do not suffice. With this in mind we turn to filter banks for finite-length sig追ls.
     If we had filter bank theory for finite-length signals, then, piecewise stationary sign섦s can
be handled by considering each homogeneous segment separately. Several approaches to filter
banks for finite-length signals exist and we follow the one in [GB95aJ. If we consider the filter
bank tree as a machine that takes an input sample(s) and produces an output s跏ple(s) every
instant then one can consider changing machine every instant (i.e., changing the ifiter coefficients
every instant). Alternatively, we could use a fixed machine for several instants and then switch
to another filter bank tree. The former approach is investigated in [PV96]. We follow the latter
approach, which, besides leveraging upon powerful methods to design the constituent filter bank
trees switched between, also leads to a theory of wavelet bases on an interval [HKRV93, GB95a].
     Let H (z), the polyphase component matrix of the analysis filter bank of a unitary filter bank
be of the form (see (8.27))
                                                     K- i
                                             馬（기 = Z b（枷“k·                                             (8.94)
                                                     知＝0

It is convenient to introduce the sequence 文 = [. . . , x(0), x(- 1),. . . , x(- M + 1), x(M), x(M -
1),. . . obtained from x by a permutation. Then.




              d = 甘文 呵         ""    hP(K - 1)     h (K - 2)             .. .   h (0)            0      侶95)
                                         0         h (K - 1)             . ..   h (1)          hj)(0)
180                                                                                    Fflter Banks and Transmu出plexers        Ch. 8


and H is unitary if l L is unitary. (8.28) induces a factorization of ii (and hence H). If V。=
diag(Vo) and




               vi             尸i      / 中 Pi        0                                 foriE{ 1. . . . .K- 1}.             (8.96)
                              0         只         / H ／가



                                                               0
                                                  H= H v1.                                                                (8.97)
                                                          i=K 十 l

The factors V1, with appropriate modifications, will be used as fundamental building blocks for
filter banks for finite-length signals.
     Now consider a finite input signal x = [x(0). x(1), . . · , T([- 1)], where L is a multiple of Al
and let k = [x(M -1) ,. . . ,x(O),x(M), . · · .x(L -1) . . . · ,x(L- M)1. Then, the finite vector d
(the output signal) is given by

             =h,(K - 1)             . ..        h,(O)              0                                                      0

                    0        /2P(7( 寸 1)          ...         h刃（0)
d = 甘爻 匹f

                                                                   0         h,(K - 1)            ...
                                                                                                  0         hP(O)
                                                                                 0            hr,(K - 1)
                                                                                               h (0) -       ...
                                                                                                   (8.98)
H is an (L - N + M) x L matrix, where N       = MK    is the length of the filters. Now  since  the rows
of H are mutually orthonormal (i.e..  has   rank L'}. one  has  to aDDend  N   - M   = M  (K  -  1) rows
trom tne ortflogonal complement ot ii to make tne map irom x to an augmentea a unitary. 土O
get a complete description of these rows, we turn to the factorization of H)(z). Define tile L x L
matrix Vo = diag(Vo) and for i E {1, . . . , K - 1} the (L - Mi) x (L - Mi + M) matrices

                               .1:二        I 小只         0              ...                    0

                                0           只      / H 只 ．.
                        Vt
                                                                                  0                                           (8.99)

                                                         0             P     I-       P       0
                                0                       ...            0          P       /       Pi


then且 is readily verified by induction to be                  fl        Vi. Since each of the factors (except V0) has
                                                         i=K 尸1




[
M more columns than rows, they can be made unitary by appending appropriate rows. Indeed,
    Bi 1
    Vi 1 is unitary where, B3 = [ TT(I小P3)                         0       ...    0] , and C3 = [0         ...   0   可P3. ] ·
    ci '
Sec. 8.11. Time-Varying Filter Bank Trees                                                                                                                                     181


Here 三 is the c5i x M left unitary matrix that spans the range of the P; i.e., P, = 三三T, and T
is the (M - 하) x M left unitary matrix that spans the range of the卜 P2; i.e., I - J} = TTT.
Clearly [T1E} is unitary. Moreover, if we define T0 = Vo and for i E {1, . . . , K - l} ,




                                                                                                            0夙Mq0                 0000
                                                                   J(aim하）(i小1)
                                                                         0


                                                                                        000
                                          l\      =


                                                                                                                                  n
                                                           +
                                                               4




then each of the factors T2 is a square unitary matrix of size L - N + M and

                                                                                              1 弓vo -
                                                                       0

                                                               fi
                                                           t= K + I
                                                                                   T,     =
                                                                                                           H


                                                                                                           l1vo
                                                                                                             _   r
                                                                                                                              -
                                                                                              勺
                                                                                                  (-   -
is the unitary matrix that acts on the data. The corresponding unitary matrix that acts on x

(rather   than   )   is   of the   form
                                          IU      H]               '   where              U h朗 MK                         -       M小        rows of entry filters   in   (K   -




                                           [wj                                                                                                                                    1)
sets given by (8.101), while W has <\ rows of exit filters in (K - 1) given by (8.102):

                             T3(I -月）[ 岬（j- l) J                                              蚌（j寸2)J                             ···       坪（0)J, ]                     (8.101)

                                   曷月 [ 畔（j- 1)J                                        坪（j小2)J                           · · · 岬（0)J ] ,                                (8.102)
where J is the exchange matrix (i.e., permutation matrix of ones along the anti-diagonal) and
                                                       1                                                                              j牛1

                              까（z) = fi [I- P1+ z뇌％혤Z啄涉"1                                                                                                                (8.103)
                                                 i=7el                                                                                i=O
                                                                                                                                      i=0

The rows of U and W form the entry and exit filters respectively. Clearly they are nonunique.
The input/output behavior is captured in




                                                           日                   w

     For example, in the four-coefficient Daubechies' filters in [Dau88a] case, there is one entry
                                                                                                           UHW       x.                                                  (8.104)



filter and exit filter.
                           [   0.8660 0.5000             0          01
                           I -0.1294 0.2241       0.8365       0.4830 I
                                                                                           (8.105)
                           1 - 0.4830 0.8365 -0.2241 -0.1294 1 '
                           L         0       0 -0.5000         0.8660 j
   If the input signal is right-sided (i.e., supported in {0, 1, . . . }), then the corresponding filter
bank would only have entry filters. If the filter bank is for left-sided signals one would only have
182                                                                                                Filter Banks and Transmultiplexers            Ch. 8


exit filters. Based on the above, we can consider switching between filter banks (that operate
on infinite extent input signals). Consider switching from a one-channel to an M channel filter




                                            [
bank. Until instant n = -1, the input is the same as the output. At n = 0, one switches into an
M-channel filter bank as quickly as possible. The transition is accomplished by the entry filters
(hence the name entry) of the M-channel filter bank. The input/output of this time-varying filter
bank is
                                                                                     ]
                                                          100
                                                   0
                                        =
                                                 d
                                                  U                                  Ix. (8.106)
                                                                  H]
Next consider switching from an M-channel filter bank to a one-channel filter bank. Until n = -1,
the M-channel filter bank is operational. From n = 0 onwards the inputs leaks to the output.
In this case, there are exit filters corresponding to flushing the states in the first filter bank
implementation at n = 0.


                                                           HW0
                                                                                00
                                            d=
                                                                            I
Finally, switching from an M1-band filter bank to an M2-band filter bank can be accomplished
as follows:
                                                                                           1
                                                         1lVJ00
                                                     戶
                                                            d
                                                     1
                                                                                           1
                                                     1
                                                                                0
                                                            1
                                            d
                                                     1
                                                     [
                                                                                               Y
                                                     1
                                                                                           1                                            (8.108)
                                                                                                                1
                                                                                                                1
                                                                                0-
                                                     1
                                                     1
                                                     1
                                                                                               "




                                                                                           ]
                                                                       U2
                                                     1
                                                                       H2
The transition region is given by the exit filters of the first filter bank and the entry filters of
the second. Clearly the transition filters are abrupt (they do not overlap). One can obtain
overlapping transition filters as follows: replace them by any orthogonal basis for the row space
。f   the matrix   FL U
                   쁘l
                      LJ2 J
                         .?    r examDle. c。
                              1.   F。          nsider switching                          filter       between       tw。   -channel       banks
with length-4 and length-6 Daubechies' filters. In this case, there is one exit filter (W1) and two
entry filters (U2).

Growing a Filter Bank Tree
Consider growing a filter bank tree at n = 0 by replacing a certain output channel in the tree
(point of tree growth) by an M channel filter bank. This is equivalent to switching from a
one-channel to an M-channel filter bank at the point of tree growth. The transition filters
associated with this change are related to the entry filters of the M-channel filter bank. In fact,
every transition filter is the net effect of an entry filter at the point of tree growth seen from the
perspective of the input rather than the output point at which the tree is grown. Let the mapping
from the input to the output "growth" channel be as shown in Figure 8.6. The transition filters
are given by the system in Figure 8.7, which is driven by the entry filters of the newly added
filter bank. Every transition filter is obtained by running the corresponding time-reversed entry
filter through the synthesis bank of the corresponding branch of the extant tree.

Pruning a Filter Bank Tree
In the more general case of tree pruning, if the map from the input to the point of pruning is
given as in Figure 8.6, then the transition filters are given by Figure 8.8.
Sec. 8.11. Time-Varying Hiter Bank Trees                                                                183




                           由（기             jM1 1+                    ALml (   )         .IML_ 1


                                 Figure 8.6. A Branch of an Existing Tree



Wavelet Bases for the Interval
By taking the effective input/output map of an arbitrary unitary time-varying filter bank tree, one
readily obtains time-varying discrete-time wavelet packet bases. Clearly we have such bases for
one-sided and finite signals also. These bases are orthonormal because they are built from unitary
building blocks. We now describe the construction of continuous-time time-varying wavelet bases.
What follows is the most economical (in terms of number of entry/exit functions) continuous-time
time-varying wavelet bases.



        UI코   （z）   小＋
                         IML_ 1 H      畔-1（기        尸＋ 小＋       -.
                                                                      TM1         -.
                                                                                        畔（기

                               Figure 8.7. Transition Filter For Tree Growth



Wavelet Bases for L2([0, 以）))
Recall that an M channel unitary filter bank (with synthesis filters {hi }) such that >             ho (n) =
 /M gives rise to an M-band wavelet tight frame for L2 (正t). If

                           wi,j= S加n｛仇3丙｝望
                                         『{ Ms"'吻（凡／jt- 丸）}                            for k eZ,      (8.109)


then Wo, j forms a multiresolution analysis of L2 (正L) with

                            W0,i = W0,3_1 田 W1,3_1 . . . 田 WM_l,3_l                    Vj E Z.        (8.110)

In [Dau92], Daubechies outlines an approach due to Meyer to construct a wavelet basis for
 r2／口＼ m小＼\
L2([0. ooI). r뇨M\
              One 1\..,\ ．· 八，,+n 11/
                  projects                    W竹'J which is the space spanned by the restrictions of
                                       八11f,\ 11/ /t口i/ . , . 1,Ln1, ;', +kmmM뇨mLnnMnU뇨4 1\t, +1M노 m口f1山寸mnm八f
                                  Wn 4 onto
砂o.j.k(t) to t > 0. We give a different construction based on the following idea. For k E IN,
support of 砂i.3.k(t) is in [0,的). With this restriction (in (8.109)) define the spaces W. As
j -* 아그 (since W0,3 -, L2(正｛)) W - L2([0,的)). Hence it suffices to have a multiresolution



       w（기 -.            IML_ 2 H      ALH2（기   -           -
                                                                     IMi      H         小（기


                                    Figure 8.8. Transition Filter For Pruning
184                                                                                         Filter Banks and Transmultiplexers   Ch. B


analysis for W   to get a wavelet basis for L2([0, oc)). (8.110) does not hold with W2,3 replaced
by W二 because WT is bigger than the direct sum of the constituents at the next coarser scale.
Let Ui_i be this difference space:

                              V喘＝吼누1由wmr··0W在"i-i飼i-i                                                                        (8.111)
If we can find an orthonormal basis for 113, then we have a multiresolution analysis for L2([0, 的)).
    We proceed as follows. Construct entry filters (for the analysis filters) of the filter bank with
synthesis filters {h2 }. Time-reverse them to obtain entry filters (for the synthesis filters). If 스
is the McMillan degree of the synthe前s bank, there are 스 entry filters. Let u (n) denote the i th
synthesis entry filters. Define the entry functions

                                       L1-1
                    p1(t) =\／可ZM川蜘（Mt- 川，                                       I E {0,· ··，스- 1} ·                          (8.112)
                                        k=0


m떠 is corn刃口C啣 su卯orted 미畔伊 + 据］                  . Let U) = S끄an {Uj,3} 呵 Span {M3'2u2（兀13t) }.
By considering one stage of the analysis and synthesis stages of this PR filter bank on right sided
signals), it readily follows that (8.111) holds. Therefore

          {吻,j,k I i E {1, . . . ,M- 1} ,j EZ,kE1나} u{ /工i,j I iE{ 0, . . . ,스- 1} ,j EZ}

forms a wavelet tight frame for L2([o, 的)). If one started with an ON basis for L2(]R), the newly
constructed basis is an ON basis for L2([0, oo)). Indeed if {伽(t - k)} is an orthonormal system


                                仰（t）吻（t 中 n) dt = ＞二UI（丸）九i（凡Ii + 丸） = 0,
                               。
                                                                     k
                         1>
and

                               Jt之0
                                   /    pj
                                             (t)
                                                   pm
                                                        (t)
                                                              dt=    ＞二111
                                                                      k
                                                                          （丸）
                                                                                :.'   （丸）
                                                                                               =
                                                                                                   0.
The dimension of lI is precisely the McMillan degree of the polyphase component matrix of the
scaling and wavelet filters considered as the filters of the synthesis bank. There are precisely as
many entry functions as there are entry filters, and supports of these functions are explicitly given
in terms of the lengths of the corresponding entry filters. Figure 8.9 shows the scaling function,
wavelet, their integer translates and the single entry function corresponding to Daubechies four
coefficient wavelets. In this case, uo = {-J/ 2, 1/2}.

Wavelet Bases for L2((- 的刈)
One could start with a wavelet basis for L2([0, 以）)) and reflect all the functions about t = 0.
This is equivalent to swapping the analysis and synthesis filters of the filter bank. We give an
independent development. We start with a WTF for L2 (皿) with functions

                                                              N- i
                                       仇（t) = \／可 ＞二 九i（丸）伽（Mt + 砒                                                           (8.115)
                                                              k=O
Sec. 8.11. Time-Varying Filter Bank Trees                                                      185


supported in卜퓨글刈. Scaling and wavelet filters constitute the analysis bank in this case. Let
스 be the McMillan degree of the analysis bank and let {w2} be the (analysis) exit filters. Define
the exit functions
                                    L1-1
                      m(t) =Vi7＞二 凹i（丸）吼（Mt+ k),             IE{0, . . .，스- 1} .            (8.116)
                                      k=O


)m) = SP.n {AJj/2
VV    Span{M3/2z'1(Mit)
                「，（凡fjt) }, and 1V:
                                W.; = Span{
                                      SPOn｛吻，  j,k} =
                                            ,b,3k}  def {MiI2吻(凡it+ k) } fork E IN. Then
as j- 苡기 w西HL2((H的，     0]) and

          ｛仇j.k 1 i E {1, . . . 小4- 1} 口 EZ丙 E 八｝u {z在．j 1 i e {0, . . . , 스 -1} ,j EZ}

forms a WTF for L가(- m, 0]). Orthonormality of this basis is equivalent to the orthonormality
of its parent basis on the line. An example with one exit function (corresponding to M = 3,
N = 6) Type 1 modulated WTF obtained earlier is given in Figure 8.10.




                                                                            /
                                                      I .5




                                                      0.5



                             ／人
                                                                                ／人



                                  自         3   4                      2
                                                                      (b,
                                                                                3    4




  Figure 8.9. (a) Entry function 尸o(t), 吼(t) and 吼(t - 1) (b) Wavelet 吻(t) and 吻(t - 1)


Segmented Time-Varying Wavelet Packet Bases
Using the ideas above, one can construct wavelet bases for the interval and consequently seg-
mented wavelet bases for L2(正t). One can write 正t as a disjoint union of intervals and use a
different wavelet basis in each interval. Each interval is will be spanned by a combination of
scaling functions, wavelets, and corresponding entry and exit functions. For instance Fi엣re 8.10
and Figure 8.9 together correspond to a wavelet basis for L2 (正t), where a 3-band wavelet basis
with length-6 filters is used for t < 0 and a 2-band wavelet basis with length-4 filters is used for
t > 0. Certainly a degree of overlap between the exit functions on the left of a transition and
entry functions on the right of the transition can be obtained by merely changing coordinates in
the finite dimensional space corresponding to these functions. Extension of these ideas to obtain
segmented wavelet packet bases is also immediate.
                                                                 Filter Banks and Transmultiplexers   Ch. 8
186


               2.5




               1.5




               0.5




               0.5




                                     0       -3   -2    -I   0           -3   -2    -l   0
                     -3   -2    -l
                                                    (1力                         (c)
                            (a)



                                                                                                        (c)
Figure 8.10. (a) Exit function vo(t), 吼(t) and 'bo(t + 1) (b) Wavelet 吻(t) and 吻(t + 1)
Wavelet 仇(t) and 仇(t + 1)



8.12    Filter Banks and Wavelets-Summary
Filter banks are structures that allow a signal to be decomposed into subsignals나ypically at
                                                                                            the filter
a lower sampling rate. If the original signal can be reconstituted from the subsignals,
bank is said to be a perfect reconstruction (PR) filter bank. For PR, the analysis and synthesis
                                                                                                three
filters have to satisfy a set of bilinear constraints. These constraints can be viewed from
                                                                                                  one
perspectives, viz., the direct, matrix, and polyphase formulations. In PR filter bank design
chooses filters that maximize a "goodness" criterion and satisfy the PR constraints.
     Unitary filter banks are an important class of PR filter banks-they give orthogonal decom-
positions of signals. For unitary filter banks, the PR constraints are quadratic in the analysis
filters since the synthesis filters are index-reverses of the analysis filters. All FIR unitary filter
                                                                                                     )
banks can be explicitly par缸1leterized. This leads to easy design (unconstrained optimization
and efficient  implementa   tion.  Sometimes   one  can impose structural constraints compatible with
the goodness criterion. For example, modulated filter banks require that the analysis and syn-
thesis filters are modulates of single analysis and synthesis prototype filter respectively. Unitary
modulated filter banks exist and can be explicitly parameterized. This allows one to design and
implement filter banks with hundreds of channels easily and efficiently. Other structural con-
 straints on the filters (e.g., linear phase filters) can be imposed and lead to parameterizations of
 associated unitary filter banks. Cascades of filter banks (used in a tree structure) can be used to
 recursively decompose signals.
    Every unitary FIR filter bank with an additional linear constraint on the lowpass filter is
 associated with a wavelet tight frame. The lowpass filter is associated with the scaling function,
 and the remaining filters are each associated with wavelets. The coefficients of the wavelet
 expansion of a signal can be computed using a tree-structure where the filter bank is applied
                                                                                               with
 recursively along the lowpass filter channel. The parameterization of unitary filter banks,
 a minor modification, gives a parameterization of all compactly supported   wavelet  tight frames.
Sec. 8.12. Filter Banks and Wavelets-Summary
                                                                                               187


In general, wavelets associated with a unitary filter bank are irregular (i.e., not smooth)
                                                                                              . By
imposing further linear constraints (regularity constraints) on the lowpass filter, one obtains
smooth wavelet bases. Structured filter banks give rise to associated structured wavelet bases;
modulated filter banks are associated with modulated wavelet bases and linear phase filter banks
are associated with linear-phase wavelet bases. Filter banks cascade-where all the channels are
recursively decomposed, they are associated with wavelet packet bases.
    From a time-frequency analysis point of view filter banks trees can be used to give arbitrary
resolutions of the frequency. In order to obtain arbitrary temporal resolutions one has to use local
bases or switch between filter bank trees at points in time. Techniques for time-varying filter
banks can be used to generate segmented wavelet bases (i.e., a different wavelet bases for disjoint
segments of the time axis). Finally, just as unitary filter banks are associated with wavelet tight
frames, general PR filter banks, with a few additional constraints, are associated with wavelet
frames (or biorthogonal bases).
Chapter 9


  Calculation of the Discrete Wavelet
                            Transform


Although when using the wavelet expansion as a tool in an abstract mathematical analysis,
the infinite sum and the continuous description of t e R are appropriate, as a practical signal
processing or numerical analysis tool, the function or signal 1 (t) in (9.1) is available only in
terms of its samples, perhaps with additional information such as its being band-limited. In
this chapter, we examine the practical problem of numerically calculating the discrete wavelet
transform.


9.1    Finite Wavelet Expansions and Transforms

The wavelet expansion of a signal 1 (t) as first formulated in (1.9) is repeated here by


                                 f (t) = ＞二 乞 (/，砂j,k）砂j.k(t)                                    (9.1)
                                         k= -ooj＝ 寸아그


                                                                                                 first
where the {'j, k(t)} form a basis or tight frame for the signal space of interest (e.g., L2). At
glance, this infinite series expansion seems  to have  the  same  practical problems   in calculation
that an infinite Fourier series or the Shannon sampling formula has. In a practical situation,
this wavelet expansion, where the coefficients are called the discrete wavelet transform (DWT), is
often more easily calculated. Both the time summation over the index k and the scale summation
over the index j can be made finite with little or no error.
    The Shannon sampling expansion [Pap77, Mar9ll of a signal with infinite support in terms of
sinc(t) = 욘뿌2expansion functions

                                           的


                                 f(t) = ＞二 /(Tn) sinc（和irn)
                                         7l=-_
                                                                                                 (9.2)



 requires an infinite sum to evaluate 1 (t) at one point because the sinc basis functions have infinite
 support. This is not necessarily true for a wavelet expansion where it is possible for the wavelet
 basis functions to have finite support and, therefore, only require a finite summation over k in
 (9.1) to evaluate 1 (t) at any point.

 188
                                                                                                    189
Sec. 9.1. Finite Wavelet Expansions and Transforms


   The lower limit on scale j in (9.1) can be made finite by adding the scaling function to the
basis set as was done in (2.28). By using the scaling function, the expansion in (9.1) becomes
                                OO                         OO    的


                      f(t) = ＞二 (f, oJ。,k)pJ。,k(t) + E          >i (f,砂3,k) 砂j,k(t).               (9.3)
                              k= m아）                     k==H乂 3 = Jo


where j = J0 is the coarsest scale that is separately represented. The level of resolution or
coarseness to start the expansion with is arbitrary, as was shown in Chapter 2 in (2.19), (2.20),
and (2.21). The space spanned by the scaling function contains all the spaces spanned by the
lower resolution wavelets from j = -的 up to the arbitrary starting point j = J0. This means
Vj。= W_的 4) · · . 4) Wj。     _l. In a practical case, this would be the scale where separating detail
becomes important. For a signal with finite support (or one with very concentrated energy), the
scaling function might be chosen so that the support of the scaling function and the size of the
 features of interest in the signal being analyzed were approximately the same.
     This choice is similar to the choice of period for the basis sinusoids in a Fourier series expansion.
If the period of the basis functions is chosen much larger than the signal, much of the transform
is used to describe the zero extensions of the signal or the edge effects.
     The choice of a finite upper limit for the scale j in (9.1) is more complicated and usually
 involves some approximation. Indeed, for samples of f (t) to be an accurate description of the
 signal, the signal should be essentially bandlimited and the samples taken at least at the Nyquist
 rate (two times the highest frequency in the signal's Fourier transform).
     The question of how one can calculate the Fourier series coefficients of a continuous signal
  from the discrete Fourier transform of samples of the signal is similar to asking how one calculates
 the discrete wavelet transform from samples of the signal. And the answer is similar. The samples
 must be "dense" enough. For the Fourier series, if a frequency can be found above which there
                                                                                                      that
 is very little energy in the signal (above which the Fourier coefficients are very small),
  determines the Nyquist frequency and the necessary sampling rate. For           the  wavelet  expansion,
  a scale must be found above which there is negligible detail or energy. If this scale is j = J1, the
 signal can be written
                                                     的
                                                                                                     (9.4)
                                       f(t) 勺 乞 (f,甲J1,k)甲J1,k(t)
                                               k==H＜均


 or, in terms of wavelets, (9.3) becomes
                                 （均                         凹    J1- 1


                       f(t)尸 乞 (/,CpJ。,k) 'J0,k (t) + 乞 ＞二（/，砂j,k）砂j,k（外
                                                                                                     (9.5)
                               k＝尸아＞                      k= -乂 3 = Jo



 This assumes that approximately f E Vj, or equivalently, jjf - Pj1f1 穴二 0, where Pj1 denotes
 the orthogonal projection of f onto Vj1.
     Given 1 (t) E Vj, so that the expansion in (9.5) is exact, one computes the DWT coefficients
 in two steps.

    1. Projection onto finest scale: Compute (1' cpJ1,k)

     2. Analysis: Compute (f, V'j,k), j E {Jo,. . . ,J1- 1} and (f, Y7j。,丸).
     190                                                                                                        Calculation of the DWT     Ch. 9


  For J1 large enough, c'J1,k(t) can be approximated by a Dirac impulse at its center of mass since

     f     (t)
                   dt =   1.
                                For
                                              large
                                                      j this gives

                                        2" f f(t)7(2九)dt,11(t)d(t- 23mo)dt= f(t - 2-3m이                                                    (9.6)
         m0 =      p dt is the fi                                 moment                      Therefore the scaling function coefficients at
  the j = J1 scale are
                                                                                          .
 where
                           ft
                                        (t)
                                                            rst
                                                                           of
                                                                                a
                                                                                    (t)
                 cj1(k)= (1,7J1,k)= 2J1/2f f(t)『(2"'t - k)dt= 2J1/2f f(t+ 2-ilk)『(2u1t)dt (9.7)
which are approximately

                                                      Cj1（劤 = (/，甲J1,k) 솨 2小Ji/2/(2中'1(mo + 丸）).                                           (9.8)
For all 2-regular wavelets (i.e., wavelets with two vanishing moments, regular wavelets other
than the Haar wavelets中1even in the M-band case where one replaces 2 by M in the above
equations, m0 = 0), one can show that the samples of the functions themselves form a third-
order approximation to the scaling function coefficients of the signal [GB92b}. That is, if f (t) is
a quadratic polynomial, then

                                      cJl（川 = (/，甲Jl ,丸） = 2_ hh/2f(2e11(mo + 丸）) 勺 2寸Ji/2/(2_ Ji丸）.                                      (9.9)
Thus, in practice, the finest scale J1 is determined by the sampling rate. By rescaling the
function and amplifying it appropriately, one can assume the samples of 1 (t) are equal to the
scaling function coefficients. These approximations are made better by setting some of the scaling
function moments to zero as in the coifiets. These are discussed in Section 6.8.
     Finally there is one other aspect to consider. If the signal has finite support and L samples
are given, then we have L nonzero coefficients (f, Y)Jl ,k). However, the DWT will typically have
more than L coefficients since the wavelet and scaling functions are obtained by convolution and
downsampling. In other words, the DWT of a L-point signal will have more than L points.
Considered as a finite discrete transform of one vector into another, this situation is undesirable.
The reason this "expansion" in dimension occurs is that one is using a basis for L2 to represent
a signal that is of finite duration, say in L2[0, p1.
     When calculating the DWT of a long signal, .10 is usually chosen to give the wavelet description
of the slowly changing or longer duration features of the signal. When the signal has finite support
or is periodic, Jo is generally chosen so there is a single scaling coefficient for the entire signal
or for one period of the signal. To reconcile the difference in length of the samples of a finite
support signal and the number of DWT coefficients, zeros can be appended to the samples of
1 (t) or the signal can be made periodic as is done for the DFT.


9.2               Periodic or Cyclic Discrete Wavelet Transform

If 1 (t) has finite support, create a periodic version of it by

                                                                     1(t) =＞二 f (t+ Pn)                                                  (9.10)
Sec. 9 3. Filter Bank Structures for Calculation of the DWT and Complexity
                                                                                                  191


where the period P is an integer. In this case, (f, o7,k) and (f, 砂 j,k) are periodic sequences in k
with period P2J (if j 之 0 and 1 if j <0) and

                                     d
                                         (j小）   =
                                                    2「 '   /f
                                                                (t）砂（2'
                                                                      "
                                                                          (
                                                                              ‘
                                                                                  丸）
                                                                                       毗        (9.11)




                 d(j,k) = 23/2 j f(t + 2'3k)i,L(」23t)dt = 23/2J f(t + 2"t)砂(2'"t) dt            (9.12)
                                                                                                   J0 is
where f =< k >P2j (k modulo P23) and 1 E {O, 1, ... ,P2j - 1}. An obvious choice for
1. Notice that in this case given L = 2J' samples    of the signal, (f, 甲J, ,k), the wavelet transform
has exactly 1 + 1 + 2 + 22 + · · · + 2JlHl = 2J1 = L terms. Indeed, this gives a linear, invertible
discrete transform which can be considered apart from any underlying continuous process similar
the discrete Fourier transform existing apart from the Fourier transform or series.
    There are at least three ways to calculate this cyclic DWT and they are based on the equations
(9.25), (9.26), and (9.27) later in this chapter. The first method simply convolves the scaling
coefficients at one scale with the time-reversed coefficients h(- n) to give an L + N - 1 length
sequence. This is aliased or wrapped as indicated in (9.27) and programmed in dwt5 . m in Ap-
pendix 3. The second method creates a periodic 乙 (k) by concatenating an appropriate number
of c3 (k) sections together then convolving h(n) with it. That is illustrated in (9.25) and in dwt .m
                                                                                                c3(k) to
in Appendix 3. The third approach constructs a periodic h(n) and convolves it with
                                                                                        these  ideas are
implement (9.26). The MATLAB programs should be studied to understand how
 actually implemented.
     Because the DWT is not shift-invariant, different implementations of the DWT may appear
 to give different results because of shifts of the signal and/or basis functions. It is interesting to
 take a test signal and compare the DWT of it with different circular shifts of the signal.
                                                                                                several
     Making f (t) periodic can introduce discontinuities at 0 and P. To avoid this, there are
 alternative constructions of orthonormal bases for L2[O. pj ICDV93. HKRV92, HKRV93,           GB95a1.
 All of these constructions use (directly or indirectly) the concept of time-varying filter banks. The
 basic idea in all t.hese constructions is to retain basis functions with support in JO, J기, remove
 ones with support outside [0. P1 and replace the basis functions that overlap across' the endpoints
 with special entry/exit functions that ensure completeness. These boundary functions are chosen
 so that the constructed basis is orthonormal. This is discussed in Section 8.11. Another way to
 deal with edges or boundaries uses "lifting" as mentioned in Section 3.4.


 9.3     디！ter Bank Structi卄es 向rC키C네ation of the DWT and Comp陀x作y

 Given that the wavelet analysis of a signal has been posed in terms of the finite expansion of (9.5),
 the discrete wavelet transform (expansion coefficients) can be calculated using Mallat's algorithm
 implemented by a filter bank as described in Chapter 3 and expanded upon in Chapter 8. Using
 the direct calculations described by the one-sided tree structure of filters and down-samplers in
 Figure 3.4 allows a simple determination of the computational complexity.
     If we assume t.he length of the sequence of the signal is L and the length of the sequence of
 scaling filter coefficients h(n) is N. then the number of multiplications necessary to calculate each
                                                                                                 1, k),
 scaling function and wavelet expansion coefficient at the next scale, c(Jj - 1, k) and d(J1 -
  from the samples of the signal. f (Tk) 志 c(Ji, k), is LN. Because of the downsampling, only half
 192                                                                                      Caic미計泊n of the DWT     Ch. 9


 are needed to calculate the coefficients at the next lower scale, c(J2 - 1, k) and d(J2 - 1, k), and
 repeats until there is only one coefficient at a scale of j = J0. The total number of multiplications
 is, therefore,

                               Mult =LN+ LN/2+ LN/4+ . ..+N                                                     (9.13)

                             =LN(l+ l/ 2+ l/ 4+ . ·.+l/ L) =2NL- N                                              (9.14)

which is linear in L and in N. The number of required additions is essentially the same.
   If the length of the signal is very long, essentially infinity, the coarsest scale J0 must be
determined from the goals of the particular signal processing problem being addressed. For this
case, the number of multiplications required per DWT coefficient or per input signal sample
                                                                                             is

                                    Mult/sample = N (2 - 2小.'0)                                                 (9.15)

    Because of the relationship of the scaling function filter h(n) and the wavelet filter h1(n) at
each scale (they are quadrature mirror filters), operations can be shared between them through
the use of a lattice filter structure, which will almost halve the computational complexity. That
is developed in Chapter 8 and [Vai92].


9.4    The Periodic Case

In many practical applications, the signal is finite in length (finite support) and can be processed
as single "block," much as the Fourier Series or discrete Fourier transform (DFT) does. If the
signal to be analyzed is finite in length such that


                                                                       00
                                                                            t ＜二 0
                                                                   r
                                                               1
                                    f (t)     J
                                              1
                                              r
                                                          /\
                                                                            t> P                                (9.16)
                                                                                                                    =

                                                                        1
                                                                        r
                                                                            0 < / ＜二 /)
                                                      1
                                                                                                                              r
                                                  1
                                              \
                                                                                                                          \
we can construct a periodic signal f (t) by


                                       f (t) =Z f (t+Pn)                                                        (9.17)


and then consider its wavelet expansion or DWT. This creation of a meaningful periodic function
can still be done, even if f (t) does not have finite support, if its energy is concentrated and some
overlap is allowed in (9.17).

Periodic Property 1: 111(t) is periodic with integer period P such that f (t) = f (t+ Pn), then
仇e scaling function （工nd wa！胤et e町）口ns切n coe月icients 仕)l4四 te竹ns) 口t scale J are 끄er寸odic with
period 2 Jp

                        If    f (t) = f (t+ P) 坑en                           따（히 =d7（丸＋2J1기                 (9.18)
Sec. 9.4. The Periodic Case                                                                                                        193


     This is easily seen from

                     丙   （   ()       =   /:f (t）砂（2' "!   -            ,）毗：
                                                                                        //(！       『Pn）砂（23t,    (）   毗           (9.19)

which, with a change of variables, becomes


      =fJ(x)砂(2i(x_ Pn)_k)dx= ff(x)砂(22x_(23Pn+k))dx= dj(k+23P                                                                )   (9.20)

and the same is true for 3 (k).

Periodic Property 2: The sc（工ling 加mc蜘n （刃2(i 凹avelet ex刃（工nsion coe刃icients (D WT tei刃is)
cam be calculated from the inner product of f (t) with 甲(t) and 砂(t) or, equivalently, from the
inner product of 1 (t) with the periodized 7(t) and 砂(t).

                                             a}(k) = (1(t),甲(t)) = (f(t), (t))                                                    (9.21)

and
                                             d3（丸）= （了（t)肋(t) ) = (1(t)，可（t) )                                                    (9.22)

where 7(t) = Z cp(t + Pn) and 砂(t) = Za (t + Pn).
     This is seen from
싸          f的 사                   .           1小 /P                            :                     '      I尸   』 . C小   .
d3（丸）=/．的／(t）砂（22t毗）dt= 2日／. f (t）砂（2"(t+P" 나）毗＝工 /(t) 2／砂（2' (t＋尸" )-k) cit
                                                                                                                                  (9.23)

                                               따（丸）=/, f (t）砂（23t中丸）dt                                                            (9.24)
                                                사              I   '>              八，          .




where 砂(2it - k) = >二, 砂(2j (t + Pn) - k) is the periodized scaled wavelet.


Periodic Property 3: If f (t) is 끄eriodic 'a庇幻卿切dl가 坑er工 凡c口11毗 's algor吼九m for c口lci工lating
the D WT coefficients in (3.9) becomes

                                               8j(k) = 54 (                             2k)        +i (m)                         (9.25)
                                                           1,


or
                                               乙（丸） = ＞二万（m 中 2k) c3+1(m)                                                         (9.26)

or
                                                    三｝（丸）= ＞二 c3 (k + P미                                                          (9.27)

乞U九ere for (9.27)
                                               ci徇 = Z枷小 胱k什1（川                                                                   但28)
194                                                                       C키cul計ion of the DWT    Ch. 9


      T九e corresponding re／毗切nsh切S for 坑e wavelet （刃e疥cients are


                    蜘) = ＞二九l(rn- 2引乙+1的 = Zmm 毗厄可川                                              (9.29)
                              rn                          m

or
                                     可姑）= ＞二 d3（丸 + 23Pn)                                        (9.30)


n脆ere
                                   山（丸）= ＞二九l(7n- 2丸）c3+i (m)                                    (9.31)


   These are very important properties of the DWT of a periodic signal, especially one artificially
constructed from a nonperiodic signal in order to use a block algorithm. They explain not only
the aliasing effects of having a periodic signal but how to calculate the DWT of a periodic signal.


9.5     Structure of the Periodic Discrete Wavelet Transform
If 1 (t) is essentially infinite in length, then the DWT can be calculated as an ongoing or continuous
process in time. In other words, as samples of 1 (t) come in at a high enough rate to be considered
equal to c. 1(k), scaling function and wavelet coefficients at lower resolutions continuously come
out of the filter bank. This is best seen from the simple two-stage analysis filter bank in Figure 3.4.
If samples come in at what is called scale J1 = 5, wavelet coefficients at scale j = 4 come out
the lower bank at half the input rate. Wavelet coefficients at j = 3 come out the next lower
bank at one quarter the input rate and scaling function coefficients at j = 3 come out the upper
bank also at one quarter the input rate. It is easy to imagine more stages giving lower resolution
wavelet coefficients at a lower and lower rate depending on the number of stages. The last one
will always be the scaling function coefficients at the lowest rate.
     For a continuous process, the number of stages and, therefore, the level of resolution at the
coarsest scale is arbitrary. It is chosen to be the nature of the slowest features of the signals
being processed. It is important to remember that the lower resolution scales correspond to a
slower sampling rate and a larger translation step in the expansion terms at that scale. This is
why the wavelet analysis system gives good time localization (but poor frequency localization)
at high resolution scales and good frequency localization (but poor time localization) at low or
coarse scales.
     For finite length signals or block wavelet processing, the input samples can be considered
as a finite dimensional input vector, the DWT as a square matrix, and the wavelet expansion
coefficients as an output vector. The conventional organization of the output of the DWT places
the output of the first wavelet filter bank in the lower half of the output vector. The output of
the next wavelet filter bank is put just above that block. If the length of the signal is two to a
power, the wavelet decomposition can be carried until there is just one wavelet coefficient and
one scaling function coefficient. That scale corresponds to the translation step size being the
length of the signal. Remember that the decomposition does not have to carried to that level.
It can be stopped at any scale and is still considered a DWT, and it can be inverted using the
appropriate synthesis filter bank (or a matrix inverse).
Sec 9.6    More General Structures                                                            195

9.6       More General Structures
The on心ided tree structure of Mallet's algorithm generates the basic DWT. From the filter bank
in Figure 3.4, one can imagine putting a pair of filters and downsainplers at the output of the
lower wavelet bank just as is done on the output of the upper scaling function bank. This can be
continued to any level to create a balanced tree filter bank. The resulting outputs are "wavelet
packets" and are an alternative to the regular wavelet decomposition. Indeed, this "growing" of
the filter bank tree is usually done adaptively using some criterion at each node to decide whether
to add another branch or not.
    Still another generalization of the basic wavelet system can be created by using a scale factor
other than two. The multiplicity-M scaling equation is

                                     甲(t) = 乞 싸）dm- k)
                                            k

and the resulting filter bank tree structure has one scaling function branch and M - 1 wavelet
branches at each stage with each followed by a downsampler by M. The resulting structure is
called an M-band filter bank, and it too is an alternative to the regular wavelet decomposition.
This is developed in Section 7.2.
    In many applications, it is the continuous wavelet transform (CWT) that is wanted. This can
be calculated by using numerical integration to evaluate the inner products in (1.11) and (7.105)
but that is very slow. An alternative is to use the DWT to approximate samples of the CWT much
as the DFT can be used to approximate the Fourier series or integral [nRGB91, RD92, VLU97].
    As you can see from this discussion, the ideas behind wavelet analysis and synthesis are ba-
sically the same as those behind filter bank theory. Indeed, filter banks can be used calculate
discrete wavelet transforms using Mallat's algorithm, and certain modifications and generaliza-
tions can be more easily seen or interpreted in terms of filter banks than in terms of the wavelet
expansion. The topic of filter banks in developed in Chapter 3 and in more detail in Chapter 8.
Chapter 10


          Wavelet-Based Signal Processing
                         and Applications


This chapter gives a brief discussion of several areas of application. It is intended to show
what areas and what tools are being developed and to give some references to books, articles,
and conference papers where the topics can be further pursued. In other words, it is a sort of
annotated bibliography that does not pretend to be complete. Indeed, it is impossible to be
complete or up-to-date in such a rapidly developing new area and in an introductory book.
   In this chapter, we briefly consider the application of wavelet systems from two perspectives.
First, we look at wavelets as a tool for denoising and compressing a wide variety of signals.
Second, we very briefly list several problems where the application of these tools shows promise
or has already achieved significant success. References will be given to guide the reader to the
details of these applications, which are beyond the scope of this book.




10.1    Wavelet-Based Signal Processing

To accomplish frequency domain signal processing. one can take the Fourier transform (or Fourier
series or DFT) of a signal, multiply some of the Fourier coefficients by zero (or some other
constant), then take the inverse Fourier transform. It is possible to completely remove certain
components of a signal while leaving others completely unchanged. The same can be done by
using wavelet transforms to achieve wavelet-based, wavelet domain signal processing, or filtering.
Indeed, it is sometimes possible to remove or separate parts of a signal that overlap in both
time and frequency using wavelets, something impossible to do with conventional Fourier-based
techniques.
     The classical paradigm for transform-based signal processing is illustrated in Figure 10.1
where the center "box" could be either a linear or nonlinear operation. The "dynamics" of the
processing are all contained in the transform and inverse transform operation, which are linear.
 The transform-domain processing operation has no dynamics; it is an algebraic operation. By
dynamics, we mean that a process depends on the present and past, and by algebraic. we mean it
 depends only on the present. An FIR (finite impulse response) filter such as is part of a filter bank
 is dynamic. Each output depends on the current and a finite number of past inputs (see (3.11)).
 The process of operating point-wise on the DWT of a signal is static or algebraic. It does not
 depend on the past (or future) values, only the present. This structure, which separates the linear,

196
                                                                                             197
Sec. 10.2. Approximate FFT using the Discrete Wave1et Transform


                                                                    Inverse
             x               I叭VT       HH
                                                 Processor    H14


                                                                     DWT      1     X


                                                 Linear or          Linear
                             Linear              Nonlinear




                           Figure 10.1. Transform-Based Signal Processor




dynamic parts from the nonlinear static parts of the processing, allows practical and theoretical
results that are impossible or very difficult using a completely general nonlinear dynamic system.
   Linear wavelet-based signal processing consists of the processor block in Figure 10.1 multi-
plying the DWT of the signal by some set of constants (perhaps by zero). If undesired signals
or noise can be separated from the desired signal in the wavelet transform domain, they can
be removed by multiplying their coefficients by zero. This allows a more powerful and flexible
processing or filtering than can be achieved using Fourier transforms. The result of this total
process is a linear, time-varying processing that is far more versatile than linear, time-invariant
processing. The next section gives an example of using the concentrating properties of the DWT
to allow a faster calculation of the FFT.



10.2      Approximate FFT using the Discrete Wavelet Transform
In this section, we give an example of wavelet domain signal processing. Rather than computing
the DFT from the time domain signal using the FFT algorithm, we will first transform the signal
into the wavelet domain, then calculate the FFT, and finally go back to the signal domain which
iS 11OW the Fouri吐 domain,
    Most methods of approximately calculating the discrete Fourier transform (DFT) involve
calculating only a few output points (pruning), using a small number of bits to represent the
various calculations, or approximating the kernel, perhaps by using cordic methods. Here we use
 the characteristics of the signal being transformed to reduce the amount of arithmetic. Since
 the wavelet transform concentrates the energy of many classes of signals onto a small number
 of wavelet coefficients, this can be used to improve the efficiency of the DFT [GB96a, GB97c,
 Guo97, GB97a] and convolution [GB96b].


 It吐roduction
 The DFT is probably the most important computational tool in signal processing. Because of the
 characteristics of the basis functions, the DFT has enormous capacity for the improvement of its
 arithmetic efficiency [BP85]. The classical Cooley-皿lkey f戚 Fourier transform (FFT) algorithm
 has the complexity of O(N log2 N). Thus the Fourier transform and its f戚 algorithm, the FFT,
 are widely used in many areas, including signal processing and numerical analysis. Any scheme
 to speed up the FFT would be very desirable.
198                                            Wavelet-Based Signal Processing and AppIications   Ch. 10


    Although the FFT has been studied extensively, there are still some desired properties that
are not provided by the classical FFT. Here are some of the disadvantages of the FFT algorithm:

  1. Pruning is not easy.
     When the number of input points or output points are small compared to the length of the
     DWT, a special technique called pruning [SB931 is often used. However, this often requires
     that the nonzero input data are grouped together. Classical FFT pruning algorithms do
     not work well when the few nonzero inputs are randomly located. In other words, a sparse
     signal may not necessarily give rise to faster algorithm.

  2. No speed versus accuracy tradeoff.
     It is common to have a situation where some error would be allowed if there could be a
     significant increase in speed. However, this is not easy with the classical FFT algorithm.
     One of the main reasons is that the twiddle factors in the butterfly operations are unit
     magnitude complex numbers. So all parts of the FFT structure are of equal importance.
     It is hard to decide which part of the FFT structure to omit when error is allowed and the
     speed is crucial. In other words, the FFT is a single speed and single accuracy algorithm.

  3. No built-in noise reduction capacity.
     Many real world signals are noisy. What people are really interested in are the DFT of
     the signals without the noise. The classical FFT algorithm does not have built-in noise
     reduction capacity. Even if other denoising algorithms are used, the FFT requires the same
     computational complexity on the denoised signal. Due to the above mentioned shortcom-
     ings, the fact that the signal has been denoised cannot be easily used to speed up the
     FFT.


Review of the Discrete Fourier Transform and FFT
The discrete Fourier transform (DFT) is defined for a length-N complex data sequence by

                             N- i
                     X (k) = ＞二2(71) eHj2" "k/N,            k= 0, . . . ,N- 1                     (10.1)
                             n=0


where we use j = \/:::1. There are several ways to derive the different fast Fourier transform
(FFT) algorithms. It can be done by using index mapping [BP85}, by matrix factorization, or
by polynomial factorization. In this chapter, we only discuss the matrix factorization approach,
and only discuss the s아called radix-2 decimation in time (DIT) variant of the FFT.
    Instead of repeating the derivation of the FFT algorithm, we show the block diagram and
matrix factorization, in an effort to highlight the basic idea and gain some insight. The block
diagram of the last stage of a length-8 radix-2 DIT FFT is shown in Figure 10.2. First, the input
data are separated into even and odd groups. Then, each group goes through a length-4 DFT
block. Finally, butterfly operations are used to combine the shorter DFTs into longer DFTs.
    The details of the butterfly operations are shown in Figure 10.3, where Wk = e32u1N is
called the twiddle factor. All the twiddle factors are of magnitude one on the unit circle. This
is the main reason that there is no complexity versus accuracy tradeoff for the classical FFT.
Suppose some of the twiddle factors had very small magnitude, then the corresponding branches
Sec. 10.2.   Approximate FFT using the Discrete Wavelet Transform                            199




                                                              日m口 색二瓦口mH




                                        口m> m 小11 U弓O
                                    H
                                                          b




                                                              日m口색＝ 曷口으
                                                          1




                       Figure 10.2. Last Stage of a Length-8 Radix그 DIT FFT




of the butterfly operations could be dropped (pruned) to reduce comple姓ty while minimizing the
error to be introduced. Of course the error also depends on the value of the data to be multiplied
with the twiddle factors. When the value of the data is unknown, the best way is to cutoff the
branches with small twiddle f比tors.
    The computational complexity of the FFT algorithm can be easily established. If we let
CFFT(N) be the complexity for a length-N FFT. we can show


                                     CFFT(N) = O(N) + 2CFFT(N/2),                           (10.2)


where O(N) denotes linear complexity. The solution to Equation 10.2 is well known:


                                                        CFFT(N) = O(Nlog2N).                (10.3)


This is a classical case where the divide and conquer approach results in very effective solution.




                       Figure 10.3. Butterfly Operations in a Radix-2 DIT FFT
 200                                                               Way이e卜Based 듸gnal F가ocessing and Applicat山ns                           Ch. 10


  The matrix point of view gives us additional insight. Let FN be the NxN DFT matrix; i.e.,
FN(m, n) = eH32冗mn1N , where m, n E {0, 1, . . . , N- 1}. Let SN be the NxN even-odd
                                                                                     separation
matrix; e.g.,
                                                         上
                                                         1
                                                         mU


                                                                               00l0
                                                           n                          00   l
                                                                                        Un
                                                             00
                                             S4                                                                                     (10.4)
                                                                                      0l00


Clearly S.JSN = 'N, where 'N is the NxN identity matrix. Then the DIT FFT is based on the
following matrix factorization,


                   FN
                        =   FNS\
                                   TSN
                                         =    I
                                              [    'N/
                                                  IN/
                                                         2
                                                         2     -
                                                                   TN/
                                                                         TN/
                                                                                    ,2 ,
                                                                                       2
                                                                                           1
                                                                                           jL 。[FN/
                                                                                                            2    ; 0
                                                                                                                 FN/ 2
                                                                                                                         ]   SN,
                                                                                                                                   (10.
                                                                                                                                             5)
where TN/2 is a diagonal matrix with WJq, i E {0, 1, . . . , N/2 - 1} on the diagonal. We can
visualize the above factorization as

                                                                               ／二          入

                                                                                           7                                       (10.6)
                                                                                                            그＼
                                                                               \=
                                                                                                      /r"




where we image the real part of DFT matrices, and the magnitude of the matrices for butterfly
operations and even-odd separations. N is taken to be 128 here.


Review of the Discrete Wavelet Transform
In this section, we briefly review the fundamentals of the discrete wavelet transform and introduce
the necessary notation for future sections. The details of the DWT have been covered in other
chapters.
    At the heart of the discrete wavelet transform are a pair of filters h and g 小 lowpass and
highpass respectively. They have to satisfy a set of constraints (5.1) {VK95, SN96, Vai92]. The
block diagram of the DWT is shown in Figure 10.4. The input data are first filtered by h and g
then downsampled. The same building block is further iterated on the lowpass outputs.




               Figure 10.4. Building Block for the Discrete Wavelet Transform
  Sec. 10.2. Approximate FFT using the Discrete Wave1e
                                                       t Transfo                          rm
                                                                                                                                             201

     The computational complexity of the DWT algori
                                                     thm can also be easily established. Let
  CDWT (N) be the complexity for a length-N DWT. Since
                                                       after each scale, we only further operate
  on half of the output data, we can show

                                     CDWT (N) = O(N) + CDWT (N/2),
                                                                                                                                           (10.7)
  which gives rise to the solution
                                               CD印T (川 = O(N).                                                                             (10.8)
     The operation in Figure 10.4 can also be expressed in
                                                                                                  matrix form WN; e.g., for Haar wavelet,




                                                                       m 0 上
                                                                                          l
                                                                                          m           0

                                                                             0                                    0 l 0
                                                                                                  工
                                                                                                  ｝

                                                                       工
                                                                       1   ］              0 l 0
                                    wr ""r = v'/ 2
                                                                                                      0 l
                                                                                 1                                                         (10.9)
                                                                                                            l
                                                                                                            1
                                                                                          1




 The orthogonality conditions on h and g ensure W;VWN =
                                                            'N. The matrix for multiscale DWT
 is formed by WN for different N; e.g., for three scale DWT
                                                            ,


                                                   ]                      ]
                             [WN/
                                     4
                                                                                                        "
                                               4
                                                                                     ［꽈
                                                                                                  "
                                         'N/
                                                                                                            'N/
                                                                                                                          2   小·
                                                                                                                                    (10.
                                                       IN/
                                                                                                                                             1이
                                                                   2
     We could further iterate the building block on some
                                                         of the highpass outputs. This general-
 ization is called the wavelet packets [CW92].

 The Algorithm Development
The key to the fast Fourier transform is the factorization
                                                            of FN into several sparse matrices, and
one of the sparse matrices represents two DFTs of half
                                                           the length. In a manner similar to the
DIT FFT, the following matrix factorization can be made:


                  FN小빠w尸出二 却：][FN。/2 ;FN/0 2］也？,
where AN/2, BN/2, CN/2, and DN/2 are all diagon
                                                al matrices. The values on the diagonal of
AN/ 2 and CN/2 are the length-N DFT (i.e., freque
                                                  ncy response) of h, and the values on the
diagonal of BN/2 and DN/2 are the length-N DFT of g. We
                                                         can visualize the above factorization
as



                                                             毛4,
                                                                                                                                   (10.12)



where we image the real part of DFT matrices, and
                                                     the magnitude of the matrices for butter-
fly operations and the one-scale DWT using length-16 Daube
                                                              chies' wavelets [Dau88a, Dau92}.
Clearly we can see that the new twiddle factors have
                                                     non;unit magnitudes.
                                                                        Wavelet-Based Signal Processing and Applications   Ch. 10
202




                                                         日山口 寸1뗘荀口mH
                                                    卜




                                  日旨口叩二協口mH읍口m1H
                         mH
                              H




                                                          日山口 寸겁荀口mH
                          -
                              H



                              H
                                                     p



                              H




                   Figure 10.5. Last stage of a length-8 DWT based FFT.




    The above factorization suggests a DWT-based FFT algorithm. The block diagram of the
last stage of a length-8 algorithm is shown in Figure 10.5. This scheme is iteratively applied to
shorter length DFTs to get the full DWT based FFT algorithm. The final system is equivalent to
a full binary tree wavelet packet transform [CW90] followed by classical FFT butterfly operations,
where the new twiddle factors are the frequency response of the wavelet filters.
    The detail of the butterfly operation is shown in Figure 10.6, where i e {0, 1, . . . , N/2- 1}.
Now the twiddle factors are length-N DFT of h and g. For well defined wavelet filters, they have
 well known properties; e.g., for Daubechies' family of wavelets, their frequency responses are
 monotone, and nearly half of which have magnitude close to zero. This fact can be exploited to
 achieve speed vs. accuracy tradeoff. The classical radix-2 DIT FFT is a special case of the above
 algorithm when h = [1, 01 and g = [0, 1]. Although they do not satisfy some of the conditions
 required for wavelets, they do constitute a legitimate (and trivial) orthogonal filter bank and are
 often called the lazy wavelets in the context of lifting.



                                                                       AN/2（自i)

                                                   CN/2(i, i)

                                                   BN/2(i, i)

                                                                       DN/2(t

                    Figure 10.6. Butterfly Operations in a Radix-2 DIT FFT
Sec. 10 2   Approximate FFT us나lg the Discrete Wavelet Transform                                 203


Computational Complexity
For the DWT-based FFT algorithm, the computational complexity is on the same order of the
FFT 小 O(Nlog2 N), since the recursive relation in (10.2) is again satisfied. However, the
constant appearing before N log2 N depends on the wavelet filters used.

Fast Approximate Fourier I ranstorm
The basic idea of the f戚 approximate Fourier transform (FAFT) is pruning; i.e., cutting off
                                                                                                 the
part of the diagram. Taditional1y, when only part of the inputs are nonzero, or only part of
outputs are required, the part of the FFT diagram where either the inputs are zero or    the outputs
are undesired is pruned [SB931, so that the computational complexity is reduced. However, the
                                                                                                 the
classical pruning algorithm is quite restrictive, since for a majority of the applications, both
inputs and the outputs are of full length.
     The structure of the DWT-based FFT algorithm can be exploited to generalize the classical
pruning idea for arbitrary signals, From the input data side, the signals are made sparse by旽he
 wavelet transform [Mey93, Mey87. Mey90, Dau92]; thus approximation can be made to speed
up the algorithm by dropping the insignificant data. In other words, although the input signal
 are normally not sparse, DWT creates the sparse inputs for the butterfly stages of the FFT. So
                                                                                             the
 any scheme to prune the butterfly stages for the classical FFT can be used here. Of course,
 price we have to pay here is the computational complexity of the DWT operations. In actual
 implementation, the wavelets in use have to be carefully chosen to balance the benefit of the
                                                                                             the
 pruning and the price of the transform. Clearly, the optimal choice depends on the class of
 data we would encounter.
      From the transform side, since the twiddle factors of the new algorithm have decreasing
                                                                                                    of
 magnitudes, approximation can be made to speed up the algorithm by pruning the sections
 the algorithm which correspond to the insignificant twiddle factors. The frequency response of the
 Daubechies' wavelets are shown in Fignre 10.7. We can see that they are monotone decreasing.
 As the length increases, more and more points are close to zero. It should be noted that those
 filters are not designed for frequency responses. They are designed for flatness at 0 and 7r. Various
 methods can be used to design wavelets or orthogonal filter banks [Ode96, Sel96, Vai92] to achieve
 better frequency responses. Again, there is a tradeoff between the good frequency response of
 the longer filters and the higher complexity required by the longer filters.

 Computat向nal Complex仕y
 The wavelet coefficients are mostly sparse, so the input of the shorter DFTs are sparse. If the
 implementation scales well with respect to the percentage of the significant input (e.g., it uses half
 of the time if only half of t.he inputs are significant), then we can further lower the complexity.
 Assume for N inputs, aN of them are significant (a 드 1), we have

                                   CF.4FT(N) = O(N) + 2aCFAFT(N/2).                            (10.13)

 For example, if a = 吉 , Equation (10.13) simplifies to

                                    CFAFT(N) = O(N) + CFAFT(N/2),                              (10.14)

  which leads to
                                             CFAFT (N) = O(N).                                 (10.15)
204                                                   Wavelet- Based Signal Processing and Applications   Ch. 10


                                 frequency response of Daubechies family of wavele冶
                       1.5




                                                                            冶ngth콕
                                                                          - ength七
                                                                        11 泊n아h-16
                                                                            1ength-32




                    8크5mE




                                                                                " ,.


                                                0.4     0.5     0.6    0.7     0.8      0.9
                                                  frequency (os兀)


          Figure 10.7. The Frequency Responses of Daubechies' Family of Wavelets



So under the above conditions, we have a linear complexity approximate FFT. Of course, the
complexity depends on the input data, the wavelets we use, the threshold value used to drop
insignificant data, and the threshold value used to prune the butterfly operations. It remains
to find a good tradeoff. Also the implementation would be more complicated than the classical
FFT.


N이se Reduct佃n Capacity
It has been shown that the thresholding of wavelet coefficients has near optimal noise reduction
property for many classes of signals [Don95]. The thresholding scheme used in the approximation
in the proposed FAFT algorithm is exactly the hard thresholding scheme used to denoise the data.
Soft thresholding can also be easily embedded in the FAFT. Thus the proposed algorithm also
reduces the noise while doing approximation. If we need to compute the DFT of noisy signals, the
proposed algorithm not only can reduce the numerical complexity but also can produce cleaner
results.


Summary
In the past, the FFT has been used to calculate the DWT [VK95. SN96. Vai92], which leads
to an efficient algorithm when filters are infinite impulse response (IIR). In this chapter, we did
just the opposite - using DWT to calculate FFT. \Ve have shown that when no intermediate
coefficients are dropped and no approximations are made, tile proposed algorithm computes the
exact result, and its computational complexity is on the same order of the FFT; i.e., O(N log2 N).
The advantage of our algorithm is two fold. From the input data side, the signals are made sparse
 Sec. 10.3. Nonlinear Filtering or Denoising with the DWT
                                                                                                  205

 by the wavelet transform, thus approximation can be made to speed up the algorithm by
                                                                                            dropping
 the insignificant data. 짜om the transform side, since the twiddle factors of the new algorithm
 have decreasing magnitudes, approximation can be made to speed up the algorithm by pri1ning
 the section of the algorithm which corresponds to the insignificant twiddle factors. Since wavelets
 are an unconditional basis for many classes of signals [SN96, Mey90, Dau92], the algorithm is
 very efficient and has built-in denoising capacity. An alternative approach has been developed
 by Shentov, Mitra, Heute, and Hossen [SMHH95, HHSM95] using subband filter banks.




10.3      Nonlinear Filtering or Denoising with the DWT

  Wavelets became known to most engineers and scientists with the publication of Daubechies'
 important paper [Dau88a1 in 1988. Indeed, the work of Daubechies [Dau92], Mallat 小4al89b,
  Mal89c, MZ93], Meyer [Mey92b, Mey93], and others produced beautiful and interesting struc-
  tures, but many engineers and applied scientist felt they had a "solution looking for a problem."
 With the recent work of Donoho and Johnstone together with ideas from Coifman, Beylkin and
 others, the field is moving into a second phase with a better understanding of why wavelets work.
 This new understanding combined with nonlinear processing not only solves currently important
 problems, but gives the potential of formulating and solving completely new problems. We now
 have a coherence of approach and a theoretical basis for the success of our methods that should
 be extraordinarily productive over the next several years. Some of the Donoho and Johnstone
 references are [DJ94b, Don93b, Don95, Don93a, Donar, DJKP95b, DJ95, DJ94a, CD94, Don93c,
 Don94, CD95a] and related ones are [Sai94b, Mou93, TM94b, TM94a, BDGM94]. Ideas from
 Coifman are in [CW90, CW92, CM94, CMW92, CMQW92, CD95b, BCR91}.
     These methods are based on taking the discrete wavelet transform (DWT) of a signal,
                                                                                              passing
 this transform through a threshold, which removes the coefficients below a certain value, then
 taking the inverse DWT, as illustrated in Figure 10.1. They are able to remove noise and achieve
high compression ratios because of the "concentrating" ability of the wavelet transform. If a
 signal has its energy concentrated in a small number of wavelet dimensions, its coefficients will
be relatively large compared to any other signal or noise that has its energy spread over a large
number of coefficients. This means that thresholding or shrinking the wavelet transform will
remove the low amplitude noise or undesired signal in the wavelet domain, and an inverse wavelet
transform will then retrieve the desired signal with little loss of detail. In traditional Fourier-
based signal processing, we arrange our signals such that the signals and any noise overlap as
little as possible in the frequency domain and linear time-invariant filtering will approximately
separate them. Where their Fourier spectra overlap, they cannot be separated. Using linear
wavelet or other time-frequency or time-scale methods, one can try to choose basis systems such
that in that coordinate system. the signals overlap as little as possible, and separation is possible.
     The new nonlinear method is entirely different. The spectra can overlap as much as they
want. The idea is to have the amplitude, rather than the location of the spectra be as different
as possible. This allows clipping, thresholding, and shrinking of the amplitude of the transform
to separate signals or remove noise. It is the localizing or concentrating properties of the wavelet
transform that makes it particularly effective when used with these nonlinear methods. Usually
the same properties that make a system good for denoising or separation by nonlinear methods,
makes it good for compression. which is also a nonlinear process.
                                                         Wavelet-Based Signal Processing and Applications       Cli. 10
206


Denoising by Thresholding
We develop the basic ideas of thresholding the wavelet transform using Donoho's formulations
[Don95, DJ94b, LGO*95]. Assume a finite length signal with additive noise of the form

                                          Yi= Xj+ Eflz,       i= 1, . . . ,N                                   (10.16)

as a finite length signal of observations of the signal x, that is corrupted by i.i.d. zero mean, white
Gaussian noise ni with standard deviation e, i.e., n2 好玎(0, 1). The goal is to recover the signal
x from the noisy observations y. Here and in the following, v denotes a vector with the ordered
elements vi if the index i is omitted. Let W be a left invertible wavelet transformation matrix
of the discrete wavelet transform (DWT). Then Eq. (10.16) can be written in the transformation
domain
                                      Y = x + N,        or,     y; = 兀 + N,                                    (10.17)

where capital letters denote variables in the transform domain, i.e., V = Wy. Then the inverse
transform matrix WU' e虹sts, and we have

                                                    w-1w = I.                                                  (10.18)


   The following presentation follows Donoho's approach [DJ94b, Don93b, Don95, Don93a,
LGO*95J that assumes an orthogonal wavelet transform with a square W; i.e., W1' = WT.
We will use the same assumption throughout this section.
   Let X denote an estimate of X, based on the observations V. We consider diagonal linear
projections
                      스 = diag(81, . . . ,dp,r), 8i E {0, 1}, i = 1, .JV1         (10.19)

which give rise to the estimate

                                     x = w- 1文 = w- 1스V = w- 1스W勺．                                              (10.20)


 The estimate X is obtained by simply keeping or zeroing the individual wavelet coefficients. Since
 we are interested in the 12 error we define the risk measure

                   冗（兄X) = E［恤尸端］＝아阿' 佯 -x川十이以H치司 ·                                                             (10.21)


 Notice that the last equality in Eq. (10.21) is a consequence of the orthogonality of W. The
 optimal coefficients in the diagonal projection scheme are 5i = l兀 >.;1 i.e., only those values of
 V where the corresponding elements of X are larger than c are kept, all others are set to zero.
 T址s leads to the ideal risk
                                                            N
                                          冗id（兀 X) = >二 min(X2,E2)·                                             (10.22)
                                                           n=1

 The ideal risk cannot be attained in practice, since it requires knowledge of X, the wavelet
 transform of the unknown vector x. However, it does give us a lower limit for the l2 error.
                                                                                                     a factor of 2[DJ94a]
      11t is interesting to note that allowing arbitrary & e 正t improves the ideal risk by at most
Sec. 10.3. Non'inear Filtering or Denoising with the DWT                                         207

   Donoho proposes the following scheme for denoising:
   1. compute the DWT Y = Wy
   2. perform thresholding in the wavelet domain, according to s아called hard thresholdirig

                                          文＝
                                                T뇨
                                                     （1
                                                      ',   :)=   {   Y,
                                                                     0,
                                                                          iYl 2t
                                                                           Yl< t
                                                                                              (10.23)

      or according to so-called soft thresholding


                                 火＝T늉（Y,t) = { ""("찡少 '), 1求二                                 (10.24)


   3. compute the inverse DWT t = WelX
This simple scheme has several interesting properties. It 's risk is within a logarithmic factor
(log N) of the ideal risk for both thresholding schemes and properly chosen thresholds t(N, e). If
one employs soft thresholding, then the estimate is with high probability at least as smooth as the
original function. The proof of this proposition relies on the fact that wavelets are unconditional
bases for a variety of smoothness classes and that soft thresholding guarantees (with high prob-
ability) that the shrinkage condition lxii < lxii holds. The shrinkage condition guarantees that
tis in the same smoothness class as is x. Moreover, the soft threshold estimate is the optimal
estimate that satisfies the shrinkage condition. The smoothness property guarantees an estimate
free from spurious oscillations which may result from hard thresholding or Fourier methods. Also,
it can be shown that it is not possible to come closer to the ideal risk than within a factor log N.
Not only does Donoho's method have nice theoretical properties, but it also works very well in
practice.
    Some comments have to be made at this point. Similar to traditional approaches (e.g., low
pass filtering), there is a trade-off between suppression of noise and oversmoothing of image
details, although to a smaller extent. Also, hard thresholding yields better results in terms of the
12 error. That is not surprising since the observation value y1 itself is clearly a better estimate
for the real value x1 than a shrunk value in a zero mean noise scenario. However, -the estimated
function obtained from hard thresholding typically exhibits undesired, spurious oscillations and
does not have the desired smoothness properties.

Shift-Invariant or Nondecimated Discrete Wavelet Transform
As is well known, the discrete wavelet transform is not shift invariant; i.e., there is no "simple"
relationship between the wavelet coefficients of the original and the shifted signal2. In this section
we will develop a shift-invariant DWT using ideas of a nondecimated filter bank or a redundant
DWT [LGO*95, LGO*96. LGOB95]. Because this system is redundant, it is not a basis but will
be a frame or tight frame (see Section 7.6). Let X = Wi be the (orthogonal) DWT of x and SR
be a m1latrix performing a circular right shift by R with R e Z. Then
                                   X, = Wi5 = WS肛 = WSRW 'X,                                  (10.25)
which establishes the connection between the wavelet transforms of two shifted versions of a
signal. r and x5-. by the orthogonal matrix WSRW 寸1. As an illustrative example, consider
Fig. 10.8.
  2Since we deal with finite length signals. we really mean circular shift.
208                                                     Wavelet- Based Signal Processing and Applications                      Ch. 10


       0.5                        '                               0.5                                                      긔




                                                                             I,   !   '1   .   .   ,




                                                                        rr        " "1




      -0.5                                                 -。.j
         0      200     400     600        800    10刃               0                  200             400   600   800   1000
                   (a) DWT of skyline                               (b) DWT of skyline circular shifted by 1

                      Figure 10.8. Shift Variance of the Wavelet Transform


    The first and most obvious way of computing a shift invariant discrete wavelet transform
(SIDWT) is simply computing the wavelet transform of all shifts. Usually the two band wavelet
transform is computed as follows: 1) filter the input signal by a low-pass and a high-pass filter,
respectively, 2) downsample each filter output, and 3) iterate the low-pass output. Because of
the downsampling, the number of output values at each stage of the filter bank (corresponding
to coarser and coarser scales of the DWT) is equal to the number of the input values. Precisely
N values have to be stored. The computational complexity is O(N). Directly computing the
wavelet transform of all shifts therefore requires the storage of N2 elements and has computational
complexity O(N2).
    Beylkin [Bey92j, Shensa [She92], and the Rice group3 independently realized that 1) there
are only N log N different coefficient values among those corresponding to all shifts of the input
signal and 2) those can be computed with computational complexity N log N. This can be easily
seen by considering one stage of the filter bank. Let

                                         y = [yo Yi. 1/2 . . . YNIT = hx                                                  (10.26)

where 1/ is the output of either the high-pass or the low-pass filter in the analysis filter bank, x
the input and the matrix h describes the filtering operation. Downsampling of y by a factor of
two means keeping the even indexed elements and discarding the odd ones. Consider the case of
an input signal shifted by one. Then the output signal is shifted by one as well, and sampling
with the same operator as before corresponds to keeping the odd-indexed coefficients as opposed
to the even ones. Thus, the set of data points to be further processed is completely different.
However, for a shift of the input signal by two, the downsampled output signal differs from the
output of the nonshifted input only by a shift of one. This is easily generalized for any odd and
even shift and we see that the set of wavelet coefficients of the first stage of the filter bank for
arbitrary shifts consists of only 2N different values. Considering the fact that only the low-pass
component (N values) is iterated, one recognizes that after L stages exactly LN values result.
Using the same arguments as in the shift variant case, one can prove that the computational
complexity is O(N log N). The derivation for the synthesis is analogous.
  3Those are the ones we are aware of.
 Sec. 10.3. Nonlinear Filtering or Denoising with the DWT
                                                                                                 209

    Mallat proposes a scheme for computing an approximation of the continuous wavelet transform
 [Mal911 that turns out to be equivalent to the method described above. This has been realized
and proved by Shensa[She92]. Moreover, Shensa shows that Mallat's algorithm exhibits the same
structure as the s아called algorithm a trous. Interestingly, Mallat's intention in [Mal91] was not
in particular to overcome the shift variance of the DWT but to get an approximation of the
continuous wavelet transform.
    In the following, we shall refer to the algorithm for computing the SIDWT as the Beylkin
algorithm4 since this is the one we have implemented. Alternative algorithms for computing
a shift-invariant wavelet transform[LP94b] are based on the scheme presented in
                                                                                        [Bey92]. They
explicitly or implicitly try to find an optimal, signal-dependent shift of the input signal. Thus, the
transform becomes shift-invariant and orthogonal but signal dependent and, therefore, nonlinear.
We mention that the generalization of the Beylkin algorithm to the multidimensional case, to an
M-band multiresolution analysis, and to wavelet packets is straightforward.


Combining the Shensa-Beylkin-Mallat- b trous Algorithms and Wavelet Denoising
It was Coifinan who suggested that the application of Donoho's method to several shifts of the
 observation combined with averaging yields a considerable improvement.5 This statement first
lead us to the following algorithm: 1) apply Donoho's method not only to "some" but to all
circular shifts of the input signal 2) average the adjusted output signals. As has been shown in
the previous section. the computation of all possible shifts can be effectively done using
                                                                                           Beylkin's
algorithm. Thus, instead of using the algorithm just described, one simply applies
                                                                                        thresholding
to the SIDWT of the observation and computes the inverse transform. .
    Before going into details, we want to briefly discuss the differences between using the tradi-
tional orthogonal and the shift-invariant wavelet transform. Obviously, by using more than
                                                                                                  N
wavelet coefficients, we introduce redundancy. Several authors stated that redundant wavelet
transforms, or frames, add to the numerical robustness [Dau92] in case of adding white noise
in the transform domain; e.g., by quantization. This is, however, different from the scenario
we are interested in, since 1) we have correlated noise due to the redundancy, and 2)
                                                                                           we try to
remove noise in the transform domain rather than considering the effect of adding some
                                                                                               noise
[LGO木95, LGO木96].


Performance Analysis
The analysis of the ideal risk for the SIDWT is similar to that by Guo[Guo95]. Define the sets
A and B according to

                                             A         =       ｛히 匹d 之 e}                    (10.27)
                                             B         =       ｛히 1兀1 < E}                   (10.28)

and an ideal diagonal projection estimator, or oracle.

                                     x   =   !    Yi
                                                           =   兀 + N,   1
                                                                        2

                                                                        1
                                                                        二1
                                                                         2
                                                                            E
                                                                                AB           (10.29)
                                             (,
                                                  U

  4However, it should be noted that Mallat published his algorithm earlier.
  5A similar remark can be found in [Sai94aj, p. 53.
                                                             Wavelet-Based Signal Processing and Applications    Ch. 10
210


The pointwise estimation error is then
                                                                        AB
                                                                        EE                                      (10.30)


In the following, a vector or matrix indexed by A (or B) indicates that only those rows are kept
that have indices out of A (or B). All others are set to zero. With these definitions and (10.21),
the ideal risk for the SIDWT can be derived

           兀d（兀치        =   E   [uw_
                                       1
                                           (.
                                                -   X)
                                                         I   ]                                                  (10.31)

                                                  21
                            E [MWm ' (NA - XB) II 2j                                                            (10.32)

                             I
                                          孕二（斗枷）
                            이L（NA中XB)' 므：(711/1l
                                                                                                                (10.33)
                                         cw_1    J
                            E［心w中lTw_1NA] - 2X加w-I月［NA]＋畔山－1XB                                                  (10.34)
                            tr [E {W小1NANXWH'T]] + XBCW-1XB                                                     (10.35)
                            tr [WH1E [WAenfflTv4'] W_1T] + XBCW-1XB                                             (10.36)
                            e2tr [WH'WAW3WU1T] + XBCW-1XB.                                                      (10.37)

where tr(X) denotes the trace of X. For the derivation we have used, the fact that NA =
fWAfl and consequently the NAi have zero mean. Notice that for orthogonal W the Eq. (10.37)
immediately specializes to Eq. (10.22). Eq. (10.37) depends on the particular signal XB, the
transform, We1, and the noise level E.
    It can be shown that when using the SIDWT introduced above and the thresholding scheme
                                                                                             upper
proposed by Donoho (including his choice of the threshold) then there exists the same
bound for the actual risk as for case of the orthogonal DWT. That is the ideal risk times loga-
                                                                                            a
rithinic (in N) factor. We give only an outline of the proof. Johnstone and Silverman state[JS94b]
                                                                                                ith
that for colored noise an oracle chooses 하 = 1x,之m where E, is the standard deviation of the
                                                                                        one has  to
component. Since Donoho's method applies uniform thresholding to all components,
show that the diagonal elements of C11／나i (the variances of the components of N) are     identical.
                                                                                             state-
This can be shown by considering the reconstruction scheme of the SIDWT. With these
ments, the rest of the proof can be carried out in the same way as the one given   by Donoho   and
加h幟one [DJ94b].


Examples of Denoising
The two examples illustrated in Figure 10.9 show how wavelet based denoising works. The first
shows a chirp or doppler signal which has a changing frequency and amplitude. Noise is added
to this chirp in (b) and the result of basic Donoho denoising is shown in (c) and of redundant
DWT denoising in (d). First, notice how well the noise is removed and at almost no sacrifice in
the signal. This would be impossible with traditional linear filters.
                                                                                         DWT
    The second example is the Houston skyline where the improvement of the redundant
is more obvious.
Sec 10.4. Statistical Estimation                                                                                                   211


                      。.。4k
                      0 02


                                   0


                -0 02


                      0.04


                -0.           06-
                                。
                                                200           400   600   800   1000

                                               (a) Original Doppler                                      (b) Noisy Doppler

                      O.04                                                                   0 041

                                                                                             0.02k
                      o.      o4
                                   0卄
                      0.02-                                                                  0.02k


                也m


                -o            06。
                                                                                       :：『 ’니 V \/ 느1
                                                200           400   600   800   1000

                                            (c) DWT Denoised Doppler                                 (d) RDWT Denoised Doppler


                      004


                      的，r




                山O2-




                                        0       200           400   600   800   1000             0       200   400   600     800

                                            (e) Original Houston Skyline                              (f) Noisy Houston Skyline
                      0.06 "                          hr-,\




                                                                                       -0.    02


                                                                                       -     。 。4


                                                200           400   600   800   1000             0       200   400   600     800

                                            (g) DWT Denoised Skyline                                 (h) RDWT Denoised Skyline

                                               Figure 10.9. Example of Noise Reduction using 砂D8'




10.4      Statistical Estimation
Tlii problem is very siniilar to the signal recovery problem; a signal has to be estimated from
additive white Gaussian noise. By linearity, additive noise is additive in the transform domain
where the problem becomes: estimate 0 from y = 9 + EZ, where z is a noise vector (with each
212                                               Wavelet-Based Signal Processing and Applications   Ch. 10


component being a zero mean variance one Gaussian random variable) and c > 0 is a scalar noise
level. The performance measured by the mean squared error (by Parseval) is given by

                                                              112
                                     尾（日 0) = E 0(y) -0IL.
                                                              112



It depends on the signal (0), the estimator 0, the noise level E, and the basis.
    For a 丘Xed E, the optimal minmax procedure is the one that minimizes the error for the worst
possible signal from the coefficient body a


                                     까(e) = inf sup 尾他 비．
                                             a ace

Consider the particular nonlinear procedure 0 that corresponds to soft-thresholding of every noisy
coefficient yi:

                                    Tr (xz) = sgn(y2)(IyiI - e)+.


Let r5(9) be the corresponding error for signal 9 and let r: (e) be the worst-case error for the
coefficient body e.
   If the coefficient body is solid, orthosyinmetric in a particular basis, then asymptotically (e- 0)
the error decays at least as fast in this basis as in any other basis. That is r (e) approaches
zero at least as fast as r (Ue) for any orthogonal matrix U. Therefore, unconditional bases are
nearly optimal asymptotically. Moreover, for small E we can relate this procedure to any other
procedure as follows [Don93b1:


                      R*(e. e) < r ' ( ,e) 드 O(log(1/E)) · R ' (i. e),      E- 0.




10.5     Signal and Image Compression

Fundamentals of Data Compression
From basic information theory, we know the minimum average number of bits needed to represent
realizations of a independent and identically distributed discrete random variable X is its entropy
H (X) [CT91]. If the distribution p(X) is known, we can design Huffman codes or use the
arithmetic coding method to achieve this minimum [BCW90I. Otherwise we need to use adaptive
method [WNC87J.
    Continuous random variables require an infinite number of bits to represent, so quantization is
always necessary for practical finite representation. However, quantization introduces error. Thus
the goal is to achieve the best rate-distortion tradeoff [JN84, CT91, BW94]. Text compression
[BCW90J, waveform coding [JN841 and subband coding [VK95] have been studied extensively
over the years. Here we concentrate on wavelet compression, or more general, transform coding.
Also we concentrate on low bitrate.
 Sec. 10.5. Signal and Image Compression                                                            213



                -
                          Transform        m4H
                                                      Quantize          -.
                                                                             Entropy Code   中＋
                              Figure 10.10. Prototype Transform Coder




Prototype Transform Coder
The simple three-step structure of a prototype transform coder is shown in Figure 10.10. The
first step is the transform of the signal. For a length-N discrete signal f (ri), we expand it using
a set of orthonormal basis functions as

                                                           N

                                                 f (n) = ＞二ci吻（n),                               (10.38)
                                                            1


where

                                                 c = (f (n) 肋如力．                                 (10.39)

   We then use the uniform scalar quantizer Q as in Figure 10.11, which is widely used for
wavelet based image compression {Sha93, SP96aJ,


                                                      =    Q(ci)    .                            (10.40)

Denote the quantization step size as T. Notice in the figure that the quantizer has a dead
zone, so if 1ci1 < T, then Q(ci) = 0. We define an index set for those insignificant coefficients


                                                          CL?




                                                                T




                              Figure 10.11. Uniform Scalar Quantizer
214                                                              Wavelet-Based Signal Processing and Applications          Ch. 10


工 = {i: 1ci1 <T} . Let M be the number of coefficients with magnitudes greater than T (signif-
icant coefficients) . Thus the size of I is N - M. The squared error caused by the quantization
is
                                   N
                                   乞佃 m尸 스X +＞二佃 - e)2.                                                             (10.41)
                                   亡＝1                      iE工          河工

Since the transform is orthonormal, it is the same as the reconstruction error. Assume T is small
enough, so that the significant coefficients are uniformly distributed within each quantization
bins. Then the second term in the error expression is

                                                                                                                    (10.42)
                                           느(c -j ' = M- .
                                           -1m                     八      丁2
                                           i로工


For the first term, we need the following standard approximation theorem [DL931 that relates it
to the l, norm of the coefficients,

                                           n76
                                           iiiii
                                                   「＝
                                                        =
                                                            (N
                                                            (
                                                                 2＝二l
                                                                         )
                                                                        「 ""   .
                                                                                                                    (10.
                                                                                                                              43)


Theorem 56 Let A =       le P   > 곶{ 仇en


                                           二c드 ,받,M1-2》
                                           iE工
                                                                                                                     (10.44)


 This theorem can be generalized to infinite dimensional space if 1If II2, < +的. It has been shown
 that for functions in a Besov space, 1If喘 < +的 does not depend on the particular choice of the
 wavelet as long as each wavelet in the basis has q > A - 古 vanishing moments and is 'q times
 continuously differentiable 小ley92b]. The Besov space includes piece-wise regular functions that
 may include discontinuities. This theorem indicates that the first term of the error expression
 decreases very fast when the number of significant coefficient increases.
      The bit rate of the prototype compression algorithm can also be separated in two parts.
 For the first part, we need to indicate whether the coefficient is significant, also known as the
 significant map. For example, we could use 1 for significant, and 0 for insignificant. We need a
  total of N these indicators. For the second part, we need to represent the values of the significant
  coefficients. We only need M values. Because the distribution of the values and the indicators
  are not known in general, adaptive entropy coding is often used {WNC87I.
      Energy concentration is one of the most important properties for low bitrate transform coding.
  Suppose for the sample quantization step size T, we have a second set of basis that generate
  less significant coefficients. The distribution of the significant map indicators is more skewed.
  thus require less bits to code. Also, we need to code less number of significant values, thus
                                                                                                    as
  it may require less bits. In the mean time, a smaller Al reduces the second error term
  in Equation 10.42. Overall, it is very likely that the new basis improves the rate-distorti       on
  performance. Wavelets have better energy concentration property than the Fourier transform
   for signals with discontinuities. This is one of the main reasons that wavelet based compression
   methods usually out perform DCT based JPEG, especially at low. bitrate.
Sec. 10.5. Signal and Image Compression
                                                                                              215

Improved Wavelet Based Compression Algorithms
The above prototype algorithm works well 小lF97, Guo97], but can be further improved for its
various building blocks [GB97b]. As we can see from Figure 10.12, the significant map
                                                                                        still
has considerable structure, which could be exploited. Modifications and improvements use the
following ideas:

   . Insignificant coefficients are often clustered together. Especially, they often cluster around
     the same location across several scales. Since the distance between nearby coefficients
     doubles for every scale, the insignificant coefficients often form a tree shape, as we can
     see from Figure 2.5. These so called zero-trees can be exploited [Sha93, SP96a] to achieve
     excellent results.

   . The choice of basis is very important. Methods have been developed to adaptively choose
     the basis for the signal [RV93, XHRO95]. Although they could be computationally
                                                                                        very
     intensive, substantial improvement can be realized.

   1Special run-length codes could be used to code significant map and values [TW96, TVC96].




                            100           200      300          400          500

                   Figure 10.12. The Significant Map for the Lenna image.
216                                             Wavelet-Based Signal Processing and Applications   Ch. 10


   . Advanced quantization methods could be used to replace the simple scalar quantizer [JCF95].

   . Method based on statistical analysis like classification, modeling, estimation, and prediction
     also produces impressive result [LRO97].

   . Instead of using one fixed quantization step size, we can successively refine the quantization
     by using smaller and smaller step sizes. These embedded schemes allow both the encoder
     and the decoder to stop at any bit rate [Sha93, SP96a].

   . The wavelet transform could be replaced by an integer-to-integer wavelet transform, no
     quantization is necessary, and the compression is lossless [SP96a].
  Other references are:[Don95, DJ94b, Don93b, Sai94b, GOL*94b, Sha93, SC95, SC96, Sha93,
VBL95, SP96a, SP96b, BW94, Guo97J.


10.6    Why are Wavelets so Useful?
The basic wavelet in wavelet analysis can be chosen so that it is smooth, where smoothness is
measured in a variety of ways [Mey87]. To represent 1 (t) with K derivatives, one can choose
a wavelet 砂(t) that is K (or more) times continuously differentiable; the penalty for imposing
greater smoothness in this sense is that the supports of the basis functions, the filter lengths
and hence the computational complexity all increase. Besides, smooth wavelet bases are also the
"best bases" for representing signals with arbitrarily many singularities [Don93bJ, a remarkable
property.
    The usefulness of wavelets in representing functions in these and several other classes stems
from the fact that for most of these spaces the wavelet basis is an unconditional basis, which is
a near-optimal property.
    To complete this discussion, we have to motivate the property of an unconditional basis being
asymptotically optimal for a particular problem, say data compression {Don93b]. Figure 10.13
suggests why a basis in which the coefficients are solid and orthosymmetric may be desired. The
signal class is defined to be the interior of the rectangle bounded by the lines x = 土a and y = 士b.
The signal corresponding to point A is the worst-case signal for the two bases shown in the figure;
the residual error (with n = 1) is given by asin(O) + bcos(O) for 0 E {0,이 and is minimized by
0 = 0, showing that the orthosymmetric basis is preferred. This result is really a consequence of
the fact that a ;E b (which is typically the case why one uses transform coding-if a = b, it turns
out that the "diagonal" basis with 0 = 플 is optimal for n = 1). The closer the coefficient body
is to a solid, orthosymmetric body with varying side lengths, the less the individual coefficients
are correlated with each other and the greater the compression in this basis.
    In summary, the wavelet bases have a number of useful properties:
   1. They can represent smooth functions.

   2. They can represent singularities

   3. The basis functions are local. This makes most coefficient-based algorithms naturally adap-
      tive to inhomogeneities in the function.

   4. They have the unconditional basis (or near optimal in a minimax sense) property for a
      variety of function classes implying that if one knows very little about a signal, the wavelet
      basis is usually a reasonable choice.
Sec. 10.7. Applications                                                                        217




                          Figure 10.13. Optimal Basis for Data Compression


   5. They are computationally inexpensive-perhaps one of the few really useful linear transform
      with a complexity that is O(N)-as compared to a Fourier transform, which is N log(N)
      or an arbitrary linear transform which is O(N2).

   6. Nonlinear soft-thresholding is near optimal for statistical estimation.

   7. Nonlinear soft-thresholding is near optimal for signal recovery.

   8. Coefficient vector truncation is near optimal for data compression.


10.7      Applications

Listed below are several application areas in which wavelet methods have had some success.

Numerical Solutions to Partial Differential Equations
The use of wavelets as basis functions for the discretization of PDEs has had excellent success.
They seem to give a generalization of finite element methods with some characteristics of multigrid
methods. It seems to be the localizing ability of wavelet expansions that give rise to sparse
operators and good numerical stability of the methods [GLRT90, RBSB94, RW97, BCR91, Bey94,
HPW94, BCR92, LPT92, BK97, BKV93I.

Seismic and Geophysical Signal Processing
One of the exciting applications areas of wavelet-based signal processing is in seismic and geophys-
ical signal processing. Applications of denoising, compression, and detection are all important
here, especially with higher-dimensional signals and images. Some of the references can be found
in [RD86, OY87, Sca94, FK94, Sai94b, LM89, GGT89, GB96c] [GGM84b, GGM84a, DDO97,
Bey97].
218                                             Wavelet-Based Signal Processing and Applications   Ch. 10


Medical and Biomedical Signal and Image Processing
Another exciting application of wavelet-based signal processing is in medical and biomedical
signal and image processing. Again, applications of denoising, compression, and detection are all
important here, especially with higher dimensional sign싫s and images. Some of the references
can be found in [AU96, Tur86, IRP*961.

Application in Communications
Some applications of wavelet methods to communications problems are in [TM94b, LKC*94,
Lin95, WWJ95, SL96].

Fractals
Wavelet-based signal processing has been combined with fractals and to systems that are chaotic
[FHV93, Mas94, Wor96, DL92, AAEG89, Aus89, WO92a, WO92b]. The multiresolution formu-
lation of the wavelet and the self-similar characteristic of certain fractals make the wavelet a
natural tool for this analysis. An application to noise removal from music is in [BCG94].
    Other applications are to the automatic target recognition (ATR) problem, and many other
questions.


10.8       Wavelet Software
There are several software packages available to study, experiment with, and apply wavelet signal
analysis. There are several MATLAB programs at the end of this book. MathWorks, Inc. has
a Wavelet Toolbox [MMOP96]; Donoho's group at Stanford has WaveTool; the Yale group
                                                                                              has
XWPL and WPLab [Wic951; Taswell at Stanford has WavBox [Tas961, a group in Spain
                                                                                              has
Uvi-Wave; MathSoft, Inc. has S+WAVELETS; Aware, Inc. has WaveTool; and the DSP group
at Rice has a MATLAB wavelet toolbox available over the internet at http://www-dsp.rice.edu.
There is a good description and list of several wavelet software packages in [BDG96}. There are
several MATLAB programs in Appendix C of this book. They were used to create the various
examples and figures in this book and should be studied when studying the theory of a particular
加pic.
Chapter 11


                                                           Summary Overview
This chapter presents a brief summary of the results of this book to show how the basic ideas
developed around the multiplier-2 (2-band) wavelet analysis and the DWT generalize into a very
rich set of systems and choices that can become bewildering.


11.1     Properties of the Basic Multiresolution Scaling Function

The first summary is given in four tables of the basic relationships and equations, primarily
developed in Chapter 5, for the scaling function 甲(t), scaling coefficients h(n), and their Fourier
transforms m (w) and H (w) for the multiplier M = 2 or tw아band multiresolution system. The
various assumptions and conditions are omitted in order to see the "big picture" and to see the
effects of increasing constraints.

 Case       Condition                           甲(t)                     令   (w)
                                                                                          Signal Space
   1     Multiresolution     甲(t) = Z 枷）VM2卜 ri)                  m佃H I-I 亮H(制            distribi此ion
   9      Partition of 1           >二c0(t- n) = 1                   m (2ir丸） = 히川         distribution

   3       Orthogonal          加 （t) 99(t H 丸） dt = 8（肋                                       L2
                                                                 Z 回w + 2砒）尸 = 1
   5     SF Smoothness                쯔으f '/ N八
                                        !   1
                                                  1\   四
                                                                                           poly e V3
                                       at


   6       SF Moments              f t1'p(t) dt = 0                                         Coifiets

    Table 11.1. Properties of M = 2 Scaling Functions (SF) and their Fourier Transformls



 Case      Condition                 h（미                               H （미               Eigenval.{T}
   1       Existet乂e            Z M미 = \／牙                          H (0) = \/／牙

   2     Fundamental        Zh (2미 = ＞二 /z(2n + 1)                   丑佃） = [)                EV = 1

   3         QMF           오 h(미 h(n + 2k) = 8（히             1H(w) j2 + IH(w + 可)I2 = 2      EV < 1

   4      Orthogonal       ）그回 九(n 寸 2k) = 6（劤               四佃甲 + 四佃 + ir기2 = 2           one EV = 1
           L2 Basis                                          and 끄（미 尹 0, 叫 5 ir/3          others ＜二 1

   6        Coiflets            二 72k帥2) = 0

       Table 11.2. Properties of M = 2 Scaling Coefficients and their Fourier Transforms

                                                                                                       219
220                                                                                   Summary Overview       Ch. 11


 Case      Cond抗幻n                    砂（t)                        山       （回）
                                                                                             Signal Space

   1         MRA         砂（t) = Z M미扼미2t - n)            'P (w) = '-I 寸5m（붊）                 distribution

   3      Orthogonal                （t- 丸） dt = 0                                                 L2
                             加 （t) ！夕

   3      Orthogonal       / 砂（t) 砂（t- 丸）dt = d（川                                                 L2

   5     W Moments              / 少 砂（t) dt = 0                                             p아yn야 E W

          Table 11.3. Properties of M = 2 Wavelets (W) and their Fourier Transforms




 Case      Cond此ion                   h1佃）                            丑         (w)
                                                                                               Eigenval.{T}

   2     Fundamental              ＞二h1(n) = 0                    H1(0) = 0

   3      Orthogonal        hi(n) = (- 1)'九（1 小 n)         田d回）1 = IH(w + 冗）1
   3      Orthogonal      Z Mm沌但m日2) = 万（m) 田K四기2 + 1丑（w）尸 = 2
   5      Smoothness             Z 十M미 = 0                月佃）= （口7H 미k 月佃）                      1 '21 ' 1
                                                                                                        4'

       Table 11.4. Properties of M = 2 Wavelet Coefficients and their Fourier Transforms



    The different "cases" represent somewhat similar conditions for the stated relationships. For
example, in Case 1, Table 1, the multiresolution conditions are stated in the time and frequency
domains while in Table 2 the corresponding necessary conditions on 九(n) are given for a scaling
function in L '. However, the conditions are not sufficient unless general distributions are allowed.
In Case 1, Table 3, the definition of a wavelet is given to span the appropriate multiresolution
signal space but nothing seems appropriate for Case 1 in Table 4. Clearly the organization of
these tables are somewhat subjective.
    If we "tighten" the restrictions by adding one more linear condition, we get Case 2 which has
consequences in Tables 1, 2, and 4 but does not guarantee anything better that a distribution.
Case 3 involves orthogonality, both across scales and translations, so there are two rows for Case 3
in the tables involving wavelets. Case 4 adds to the orthogonality a condition on the frequency
response H (w) or on the eigenvalues of the transition matrix to guarantee an L2 basis rather than
a tight frame guaranteed for Case 3. Cases 5 and 6 concern zero moments and scaling function
smoothness and symmetry.
    In some cases, columns 3 and 4 are equivalent and others, they are not. In some categories,
a higher numbered case assumes a lower numbered case and in others, they do not. These tables
try to give a structure without the details. It is useful to refer to them while reading the earlier
chapters and to refer to the earlier chapters to see the assumptions and conditions behind these
 tables.
Sec. 11.2. Types of Wavelet Systems                                                        221


11.2     Types of Wavelet Systems
Here we try to present a structured list of the various classes of wavelet systems in terms of
modification and generalizations of the basic M = 2 system. There are some classes not included
here because the whole subject is still an active research area, producing new results daily.
However, this list plus the table of contents, index, and references will help guide the reader
through the maze. The relevant section or chapter is given in parenthesis for each topic.

   1Signal Expansions          (1)

         - General Expansion Systems           (7.6)
         - Multiresolution Systems       (2)

   1Multiresolution Wavelet Systems            (2)

         - M = 2 or two-band wavelet systems             (2-6)
         - M > 2 or M-band wavelet systems             (7.2)
         - wavelet packet systems      (7.3)
         尸 multiwavelet systems       (7.5

   . Length of scaling function filter        (5)

         - Compact support wavelet systems
         - Infinite support wavelet systems

   1Orthogonality        (5)

         - Orthogonal or Orthonormal wavelet bases
         - Semiorthogonal systems
         - Biorthogonal systems       (7.4)

   1Symmetry

         - Symmetric scaling functions and wavelets              (7.4,7.5)
            Approximately symmetric systems            (6.9)
         小 Minimum phase spectral factorization systems               (6)
         - General scaling functions

   1Complete and Overcomplete systems                (4,7.6)

         - Frames
         - Tight frames
         - Redundant systems and transforms             (7.6,10.3)
         - Adaptive systems and transforms, pursuit methods                  (7.6)
222                                                                     Summary Overview    Ch. 11


  1Discrete and continuous signals and transforms {analogous Fourier method}        (7.8)

      寸 Discrete Wavelet Transform {Fourier series} (1)
      - Discrete-time Wavelet Transform {Discrete Fourier transforms} (3,8)
         Continuous-time Wavelet Transform {Fourier transform or integral} (7.8)

  1Wavelet design    (6)

        Max. zero wavelet moments [Daubechies]
        Max. zero scaling function moments
        Max. mixture of SF and wavelet moments zero [Coifman]          (6.9)
        Max. smooth scaling function or wavelet [Heller, Lang, etc.]
         Mm1l. scaling variation [Gopinath. Odegard, etc.]
      - Frequency domain criteria
           * Butterworth [Daubechiesi
           永 least-squares, constrained LS, Chebyshev
         Cosine modulated for M-band systems       (8.5)

  1Descriptions   (2)

      - The signal itself
      - The discrete wavelet transform (expansion coefficients)
      - Time functions at various scales or translations
      - Tiling of the time-frequency/scale plane    (7.1)
Chapter 12


                                                                  References


We would especially recommend five other books that complement this one. An excellent reference
for the history, philosophy, and overview of wavelet analysis has been written by Barbara Burke
Hubbard [Hub961. The best source for the mathematical details of wavelet theory is by Ingrid
Daubechies 1Dau92]. Two good general books which starts with the discrete-time wavelet series
and filter bank methods are by Martin Vetterli and Jelena Kova亡evi [VK95] and by Gilbert
Strang and Truong Nguyen [SN961. P. P. Vaiyanathan has written a good book on general
multirate systems as well as filter banks [Vai92].
    Much of the recent interest in compactly supported wavelets was stimulated by Daubechies
[Dau90, Dau88a, Dau92, CDV93} and S. Mallat 小4al89b, Mal89c, Mal89a} and others [Law90,
Law9lbl. A powerful point of view has been recently presented by D. L. Donoho, I. M. John-
stone, R. R. Coifman, and others [Don93b, Don95, Don93a, Donar, DJKP95b, DJ95, DJ94a,
BDGM94, CD95a, CD95b]. The development in the DSP community using filters has come from
Smith and Barnwell [SB86a, 5B87], Vetterli [Vet86, Vet87, VG89, VK95}, and Vaidyanathan
[Vai87a, VM88, Vai92}. Some of the work at Rice is reported in [Gop90, GB95c, SHGB93,
GB95b, Gop92, Bur93, GOL*94a, GOL*94b, OGL*95, LGO*95, WOG*95a} [LGOB95, GLOB95,
LGO*96, WOG*95b, WB95] Analysis and experimental work was done using the Matlab corn-
puter software system [MLB89, MMOP96}. Overview and introductory articles can be found in
[GKM89, Mey89, Dau89, Bur93, Coi90, Str89, GB92c, Rus92, BNW94, Bur94, Str94]. {RV91,
JS94a, Ngu95b, VD95, BDG96} Two special issues of IEEE Transactions have focused on wavelet
methods [DMW92, DFN*93]. Books on wavelets, some of which are edited conference proceed-
ings include [CGT89, KR90, AKM90, Mey90, Mey92a, Chu92a, Chu92b, Dau92, Vai92, AH92,
RBC*92, Mal92, Mey92b] [You93, Mey93, BF93, 引V93, Koo93, FHV93, Fli94, CMP94, FK94,
Kai94] [Wal94, Mas94, VK95, Wic95, SN96, AU96, HW96b, Wor96, Hub96, T的6] [AH92, Mal97,
Tew97, AS96, RW97, Chu97J.
    Another way to keep up with current research and results on wavelets is to read the Wavelet
Digest on the world-wide-web at: http://www.math.scarolina.edu/"wavelet edited by Wim
Sweldens.




                                                                                          223
                                                                    B向油graphy


[AAEG89]   F. Argoul, A. Arneodo, J. Elezgaray, and G. Grasseau. Wavelet transform of fractal aggre-
           gates. Physics Letters A., 135:327-336, March 1989.
[AAU96]    Akram Aldroubi, Patrice Abry, and Michael Unser. Construction of biorthogonal wavelets
           starting from any two multiresolutions. preprint, 1996.
[A1192]    A. N. Akansu and R. A. Haddad. Multiresolution Signal Decomposition, 가ansforms, Sub-
           bands, and Wavelets. Academic Press, San Diego, CA, 1992.
[AKM90]    Louis Auslander, Tom Kailath, and Sanjoy K. Mitter, editors. Signal Processing, Part I:
           Signal Processing Theory. Springer-Verlag, New York, 1990. IMA Volume 22, lectures from
           IMA program, July 1988.
[Ald96]    A. Aidroubi. Oblique and Hierarchical Multiwajelet Bases. Technical Report, National
           Institutes of Health, December 1996.

[Alp93]    B. Alpert. A class of bases in 12 for the sparce representation of integral operators. SIAM
           J. 凡n玩九． An口lysis, 24, 1993.
[A596]     Ali N. Akansu and Mark J. T. Smith. Subband and Wavelet 가ansforms, Design and Ap-
           plications. Kluwer Academic Publishers, Boston, 1996.
[AU96J     Akrarn Aidroubi arid Michael Unser, editors. Wavelets in MedrcniC and Biology. CRC Press.
           Boca Raton, 1996.
[Aus89}    P. Auscher. Ondelettes fractales et applications. PhD thesis, 1989.
[AWW92     P. Auscher, G. Weiss, and M. V. Wickerhauser. Local sine and cosine bases of Coifman
           and Meyer and the construction of smooth wavelets. In C. K. Chui, editor, Wavelets: A
           Tuto기ll in Theory and Applications, pages 15-51, Academic Press, 1992. Volume 2 in series
           on Wavelet Analysis and its Applications.
[BBH93}    J. N. Bradley, C. M. Brislawn, and T. Hopper. The FBI wavelet/scalar quantization stan-
           dard for gray-scale fingerprint image compression. In Visual Info. Process. II, SPIE, Orlando,
           FL, April 1993.
[BBOH96]   C. M. Brislawn, J. N. Bradley, R. J. Onyshczak, and T. Hopper. The FBI compression
           standard for digitized fingerprint images. In Proceedings of the SPIE Conference 2847,
           Applications of Digital Image Processing XIX, 1996.
[BC92]     S. Basu and C. Chiang. Complete parameterization of two dimensional orthonormal
           wavelets. In Proceedings of IEEE-SP Symposium on Time-Frequency and Time-Scale Meth-
           ods '92, Victoria, BC, IEEE, 1992.

224
BIBLIOGRAPHY                                                                                    225


[BCG94]    Jonathan Berger, Ronald R. Coifman, and Maxim J. Goldberg. Removing noise from music
           using local trigonometric bases and wavelet packets. Journal of the Audio Enginee仇ng
           Society, 42(10):808-817, October 1994.
[BCR91]    G. Beylkin, R. R. Coifman, and V. Rokhlin. Fast wavelet transforms and numerical alg口
           rithms I. Communications on Pure and Applied Mathematics, 44:141-183, 1991.
[BCR92]    C. Beylkin, R. R. Coifman, and V. Rokhlin. Wavelets in numerical analysis. In M. B.
           Ruskai, G. Beylkin, I. Daubechies, Y. Meyer, R. Coifman, S. Mallat, and L Raphael, ed-
           itors, Wavelets and Their Applications, pages 181-210, Jones and Bartlett, Boston, 1992.
           Outgrowth of the NSF/CBMS Conference on Wavelets, Lowell, June 1990.
[BCW90]    T. C. Bell, J. G. Cleary, and I. H. Witten. Text Compression. Prentice Hall, N.J., 1990.
[BDG96I    Andrew Brice, David Donoho, and Hong-Ye Gao. Wavelet analysis. IEEE Spectrum,
           33(10):26-35, October 1996.
[BDGM94]   A. G. Bruce, D. L. Donoho, H.-Y. Gao, and R. D. Martin. Denoising and robust nonlinear
           wavelet analysis. In Proceedings of Conference on Wavelet Applications, pages 325-336,
           SPIE, Orlando, FL, April 1994.
[BE931     F. Bao and Nurgun Erdol. On the discrete wavelet transform and shiftability. In Proceedings
           of the Asilomar Conference on Signals, Systems and Computers, pages 1442-1445, Pacific
           Grove, CA, November 1993.
[BE94]     F. Bao and N. Erdol. The optimal wavelet transform and translation invariance. In Pro-
           ceedings o/ 疏e IEEE Internation毗 Co?寸e7毛nce on Acous挽Cs, 枷eech, 口nd S勾n口lP恤essing,
           pages 111:13-16, ICASSP-94, Adelaide, May 1994.
[Bey92}    G. Beylkin. On the representation of operators in bases of compactly supported wavelets.
           SIAM Journal on Numerical Analysis, 29(6):1716-1740, December 1992.
[Bey94]    G. Beylkin. On wavelet-based algorithms for solving differential equations. In John J.
           Benedetto and Michael W. Frazier, editors, Wavelets: Mathematics and Applications,
           pages 449-466, CRC Press, Boca Raton, 1994.
[Bey97]    Gregory Beylkin. An adaptive pseudo-wavelet approach for solving nonlinear partial differ-
           ential equations. In W. Dahmen, A. Kurdila, and P. Oswald, editors, Multiscale Wavelet
           Methods for Partial Differential Equations. Academic Press, San Diego, 1997. Volume 6 in
            the series: Wavelet Analysis and Applications.
[BF9司      加뇨i J. Benedetto and 入'Iichael W. Frazier, editors. 14／口velets: Ma坑em口tics 口nd A까）lic口－
           tions. CRC Press, Boca Raton, FL, 1993.
[BK97]     Gregory Beylkin and James M Keiser. On the adaptive nomerical solution of nonlinear
           partial differential equations in wavelet bases. Journal of Computational Physics, 132:233-
           259, 1997.
 [BKV93]   G. Beylkin, 3. M. Keiser, and L. Vozovoi. A New Class of Stabel Time Discretization
           Schemes for the Solution of Nonlinear PDE's. Technical Report, Applied Mathematics
           Program, University of Colorado, Boulder, CO, 1993.
 [BM95]    Albert P. Berg and Wasfy B. Mikhael. An efficient structure and algorithm for the mixed
           transform representation of signals. In Proceedings of the 29th Asilomar Conference on
           Signals, Systems, and Computers, Pacific Grove, CA, November 1995.
 [BNW94]    A. Benveniste, R. Nikoukhah, and A. S. Wilisky. Multiscale system theory. IEEE T口nsac-
            tions on Circuits and Systems, I, 41(1):2-15. January 1994.
 [BO96]     C. S. Burrus and J. E. Odegard. Wavelet systems and zero moments. IEEE Transactions
            on Signal Processing, submitted, November 11996. Also CML Technical Report, Oct. 1996.
226                                                                                        Bibliography


[BO971     C. Sidney Burrus and Jan E. Odegard. Generalized coifiet systems. In Proceedings of the
           International Conference on Digital Signal Processing, Santorini, Greece, July 1997.
[Boa92]    Boualem Boashash, editor. Time-Frequency Signal Analysis. Wiley, Halsted Press, New
           York, 1992. Result of 1990 Special Converence on Time-Frequency Analysis, Gold Coast,
           Australia.
[BP85}     C. S. Burrus and T. W. Parks. DFT/FFT and Convolution Algorithms. John Wiley &
           Sons, New York, 1985.
[Bur93]    C. S. Burrus. Scaling Functions and Wavelets. first version written in 1989, The Computa-
           tional Mathematics Lab. and ECE Dept., Rice University, Houston, Tx, 1993.
{Bur94]    Barbara Burke. The mathematical microscope: waves, wavelets, and beyond. In M. Bartu-
           帥ak, et al, editor, A Positron N口med P仇scilla, Sci日i此加 1九sco刃e7궁／ 口t 坑e 肝ont才er, chap-
           ter 7, pages 196-235, National Academy Press, Washington, DC, 1994.
[B＼人／9긔    入4ichae1 Burrows and David J. ＼入／heeler. A 夙ock-Sor枷g Lossless D口t口 (7om끄7毛ssion A伽‘
           鹿thm. Technical Report 124, Digital Systems Research Center, Palo Alto, 1994.
[CD941     Shaobing Chen and David L. Donoho. Basis pursuit. In Proceedings of the 28th Asilomar
           Conference on Signals, Systems, and Computers, pages 41-44, Pacific Grove, CA, November
           1994. Also Stanford Statistics Dept. Report, 1994.
[CD95a}    Shaobing Chen and David L. Donoho. Atomic Decomposition by Basis Pursuit. Technical
           Report 479, Statistics Department, Stanford, May 1995. preprint.
[CD95b]    R. R. Coifman and D. L. Donoho. Translation-invariant de-noising. In Anestis Antoniadis,
           editor, Wavelets and Statistics, Springer-Verlag, to appear 1995. Springer Lecture Notes.
[CDF92]    A. Cohen, I. Daubechies, and J. C. Feauveau. Biorthogonal bases of compactly supported
           wavelets. Communications on Pure and Applied Mathematics, 45:485-560, 1992.
{CDM91]    S. Cavaretta, W. Dahmen, and C. A. Micchelli. Stationary Subdivision. Volume 93, Amer-
           ican Mathematical Society, 1991.
[CDP95]    A. Cohen, I. Daubechies, and G. Plonka. Regularity of refinable function vectors. Technical
           Report 95/16, Universitt Rostock, 1995. To appear in: J. Fourier Anal. Appl.
[CDV93]    Albert Cohen, Ingrid Daubechies, and Pierre Vial. Wavelets on the interval and fast wavelet
           transforms. Applied and Computational Harmonic Analysis, 1(1):54-81, December 1993.
[CGT89]    J. M. Combes, A. Grossmann, and P. Tchamitchian, editors. Wavelets, Time-Frequency
           Methods and Phase Space. Springer-Verlag, Berlin, 1989. Proceedings of the International
           Conference, Marseille, France, December 1987.
[Chu92a]   Charles K. Chui. An Introduction to Wavelets. Academic Press, San Diego, CA, 1992.
           Volume 1 in the series: W口t肥let An口蜘招 and its A까兄ic毗加ns.
[Chu92b]   Charles K. Chui. Wavelets: A Tutorial in Theory and Applications. Academic Press, San
           Diego, CA, 1992. Volume 2 in the series: Wavelet Analysis and its Applications.
[Chu9끼     Charles K. Chui, 14／口velets: A M毗帥口tic口I To아for Signal An口lysis. SIA入4, Ph沌dilph屯
           1997.
[CL96]     C. K. Chui and J. Lian. A study of orthonormal multi-wavelets. Applied Numerical Math-
           ematics, 20(3):273-298, March 1996.
[CM94]     Ronald R. Coifman and Fazal Majid. Adapted Waveform Analysis and Denoising. Technical
           Report, Yale University, New Haven, 1994.
[CMP94I    Charles K. Chui, Laura Montefusco, and Luigia Puccio, editors. Wavelets: Theory, Algo-
           rithms, and Applications. Academic Press, San Diego, 1994. Volume 5 in the series: Wavelet
           Analysis and its Avvlications.
미BL山GRAPHY                                                                                         227


[CMQW92J R. R. Coifman, Y. Meyer, S. Quake, and M. V. Wickerhauser. Signal processing and corn-
         pression with wave packets. In Y. Meyer, editor, Proceedings of the Internatiouul Conference
         on Wavelets, 1989 Mars eille. Masson, Paris, 1992.
[CMW92J     R. R. Coifman, Y. Meyer, and M. V. Wickerhauser. Wavelet analysis and signal processing.
            In 入'I. B. Ruskai et al., editor, W口叱扼ts and T九eir Apj兄比口挽ons, 加nes and Bart노tt, Boston,
            1992.
[CMX96J     Z. Chen, C. A. Micchelli, and Y. Xu. The Petrov-Galerkin Method for Second Kind Integral
            Equations II: Multiwavelet Schemes. Technical Report, Math. Dept. North Dakota State
            University, November 1996.
[CNKS96]    T. Cooklev, A. Nishihara, M. Kato, and M. Sablatash. Two-channel multifilter banks and
            multiwavelets. In IEEE Proc. m1t. Conf. Acoust., Speech, Signal Processing, pages 2769寸
            2772, 1996.
[Coh89]     L. Cohen. Time-frequency distributions - a review. Proceedings of the IEEE, 77(7):941-981,
            1989.
[Coh92]     A. Cohen. Biorthogonal wavelets. In Charles K. Chui, editor, Wavelets: A T比o仇al in
            Theory and Applications, Academic Press, Boca Raton, 1992. Volume 2 in the series:
            Wavelet Analysis and its Applications.
[Coh95]     Leon Cohen. Time-Frequency Analysis. Prentice Hall, Englewood Cliffs, NJ, 1995.
[Coi90]     R. R. Coifman. Wavelet analysis and signal processing. In Louis Auslander, Tom Kailath,
            and Sanjoy K. Mitter, editors, Signal Processing, Pa忖 I: Signal Processing Theory, pages 59-
            68, Springer-Verlag, New York, 1990. IMA vol. 22, lectures from IMA Program, summer
            1988.
[Cr096]     Matthew Crouse. Frame Robustness for De-Noising. Technica1 Report, EE 696 Course
            Report, Rice University, Houston, Tx, May 1996.
[CS93]      A. Cohen and Q. Sun. An arthmetic characterization of the conjugate quadrature fil-
            ters associated to orthonormal wavelet bases. SIAM Journal of Mathematical Analysis,
            24(5):1355-1360, 1993.
[CT91]      T. M. Cover and J. A. Thomas. Elements of Information Theory. John Wiley $ Sons, N.Y.,
            1991.
[CW90]      Ronald R. Coifman and M. V. Wickerhauser. Best-Adapted Wave Packet Bases. Technical
            Report, Math Dept., Yale University, New Haven, 1990.
[CW92]      R. R. Coifman and M. V. Wickerhauser. Entropy-based algorithms for best basis selection.
            IEEE Transaction on Information Theo八, 38(2):713-718, March 1992.
[Dau88a]    Ingrid Daubechies. Orthonormal bases of compactly supported wavelets. Communications
            on Pure 口nd A끄7교扼d 凡；ra坑em口挽Cs, 41:909-996, No＼肥mber 1988.
[Dau88b]    Ingrid Daubechies. Time-frequency localization operators: a geometric phase space ap-
            proach. IEEE Transactions on Information Theory, 34(4):605-612, July 1988.
[Dau89]     Ingrid Daubechies. Orthonormal bases of wavelets with finite support - connection with
            discrete filters. In J. M. Combes, A. Grossman, and Ph. Tchamitchian, editors, Wavele幻,
             Time-Frequency Methods and Phase Space, pages 38-66. Springer-Verlag, Berlin, 1989. Pr아
            ceedings of International Colloquium on Wavelets and Applications, Marseille, France, Dec.
            1987.
[Dau90]     Ingrid Daubechies. The wavelet transform, time-frequency localization and signal analysis.
            IEEE Transaction on Information Theo겡, 36(5):961-1005, September 1990. Also a Bell
            Labs Technical Report.
228                                                                                          Bibliography


]Dau92J     Ingrid Daubechies. Ten Lectures on Wavelets. SIAM, Philadelphia, PA, 1992. Notes from
            the 1990 CBMS-NSF Conference on Wavelets and Applications at Lowell, MA.
[Dau93]     Ingrid Daubechies. Orthonormal bases of compactly supported wavelets II, variations on a
            theme. SIAM Journal of Mathematical Analysis. 24(2):499-519, March 1993.
[Dau96}     Ingrid Daubechies. Where do wavelets comre from? - a personal point of view. Proceedings
            of the IEEE, 84(4):510-513, April 1996.
[DD87]      G. Deslauriers and S. Dubuc. Interpolation dyadique. In G. Cherbit, editor, Fractals,
            D初nensions Non E毗扼rs et A까疵C毗이四， pages 44-45, 入lasson. Paris, 1987.
[DDO97]     Wolfgang Dahmen, Andrew Durdila, and Peter Oswald, editors. Multiscale Wavelet Methods
            for Partial Differential Equations. Academic Press, San Diego, 1997.
[DFN*93]    Special issue on wavelets and signal processing. IEEE T口nsactions on Signal Processing,
            41(12):3213-3600, December 1993.
[DJ94a]     David L. Donoho and lain M. Johnstone. Ideal denoising in an orthonormal basis chosen
            from a library of bases. C. R. Acad. Sci. Paris, Ser. I, 319, to appear 1994. Also Stanford
            Statistics Dept. Report 461, Sept. 1994.
[DJ94b]     David L. Donoho and lain M. Johnstone. Ideal spatial adaptation via wavelet shrinkage.
            Biornet吼a, 81:425-455, 1994. Also Stanford Statistics Dept. Report TR-400, July 1992.
[DJ95]      David L. Donoho and lain M. Johnstone. Adapting to unknown smoothness via wavelet
            shrinkage. Journal of American Statist. Assn., to appear 1995. Also Stanford Statistics
            Dept. Report TR-425, June 1993.
{DJJJ       Ingrid Daubechies, St6phane Jaffard, and Jean-Lin Journ. A simple Wilson orthonormal
            basis with exponential decay. preprint.
[DJKP95a] David L. Donoho, lain M. Johnstone, Gerard Kerkyacharian, and Dominique Picard. Discus-
          sion of "Wavelet Shrinkage: Asymptopia?". Journal Royal Statist. Soc. Ser B., 57(2):337-
          369, 1995. Discussion of paper by panel and response by authors.
[DJKP95b] David L. Donoho, lain M. Johnstone, Gerard Kerkyacharian, and Dominique Picard.
          Wavelet shrinkage: asymptopia? Journal Royal Statistical Society B., 57(2):301-337, 1995.
          Stiso Stanford Statistics Dept. Report TR-419, March 1993.
[DL91]      Ingrid Daubechies and Jeffrey C. Lagarias. Tw아scale difference equations, part I. existence
            and global regularity of solutions. SIAM Journal of Mathematical Analysis, 22:1388-1410.
            1991. From an internal report, AT&T Bell Labs, Sept. 1988.
[DL92]      Ingrid Daubechies and Jeffrey C. Lagarias. Tw아scale difference equations, part II. local reg-
            ularity, infinite products of matrices and fractals. SIAM Journal of Mathematical Analysis,
            23:1031-1079, July 1992. From an internal report, AT&T Bell Labs, Sept. 1988.
[DL93]      R. DeVire and G. Lorentz. Constructive Approximation. Springer-Verlag, 1993.
[DM93]      R. E. Van Dyck and T. G. Marshall, Jr. Ladder realizations of fast subband/vq coders
            with diamond structures. In Proceedings of IEEE International Symposium on Circuits and
            Systems, pages 111:177-180, ISCAS, 1993.
[DMW92]     Special issue on wavelet transforms and multiresolution signal analysis. IEEE Transactions
            on Information Theory, 38(2, part II):529-924, March, part 111992.
1Don93a]    David L. Donoho. Nonlinear wavelet methods for recovery of signals. densities, and spec-
            tra from indirect and noisy data. In Ingrid Daubechies, editor. Different Perspectives on
             Wavelets, I, pages 173-205, American lvlathematical Society, Providence, 1993. Proceedings
            of Symposia in Applied Mathematics and Stanford Report 437, July 1993.
미B니OGRAP- Y                                                                                           229


[Don93b}   David L. Donoho. Unconditional bases are optimal bases for data compression and for sta-
           tistical estimation. A끄plied 口nd Corn까tat啣川 丑ar刃20fl化 An毗／毓s, 1(1):100-115, December
           1993. Also Stanford Statistics Dept. Report TR-410, Nov. 1992.
[Dcn93c]   David L. Donoho. Wavelet Skrinkage and W. V. D. - A Ten Minute Tour. Technical
           Report TR-416, Statistics Department, Stanford University, Stanford, CA, January 1993.
           Preprint.
[Don94J    David L. Donoho. On minimum entropy segmentation. In C. K. Chui, L. Montefusco, and
           L. Puccio, ed代ors, W口ye扼加．‘ T九eor킵， A勺on疏ms, （工nd A끄7疵ca挽ons, Academic Press, San
           Diego, 1994. Also Stanford Tech Report TR-450, 1994; Volume 5 in the series: Wavelet
           Analysis and its Applications.
{Don95J    David L. Donoho. De-noising by soft-thresholding. IEEE 升ansactions on Information
           Theory, 41(3):613-627, May 1995. also Stanford Statistics Dept. report TR-409, Nov. 1992.
[D（끄ia日    David L. Don아io. Interj）아ating wavelet transforms. A까疵ed 口nd Comput口tior工口i 丑口I了nonic
           Analysis, to appear. Also Stanford Statistics Dept. report TR-408, Nov. 1992.
[DS52]     R. J. Duffin and R. C. Schaeffer. A class of nonharmonic fourier series. Transactions of the
           Ame月can 人／口坑em口t記毗 Socie却／} 72:341-366, 1952.
[DS83]     J. E. Dennis and R. B. Schnabel. Numerical Methods for Unconstrained Optimization and
           Nonlinear Equations. Prentice-Hall, Inc., Englewood Cliffs, New Jersey, 1st edition, 1983.
[DS96a}    Ingrid Daubechies and Wim Sweldens. Factoring Wavelet Transforms into Lifting Steps.
           Technical Report, Princeton and Lucent Technologies, NJ, September 1996. Preprint.
[DS96b]    T. R. Downie and B. W. Silverman. The Discrete Multiple Wavelet T口nsform and Thresh-
           olding Methods. Technical Report, University of Bristol, November 1996. Submitted to
           IE万 Tr口n. 航gn口1 Process可rig.
[Dut89J    P. Dutilleux. An implementation of the "algorithme a trou" to compute the wavelet trans-
           form. In J. M. Combes, A. Grossmann, and Ph. Tchamitchian, editors, Wavelets, Time-
           Frequency Methods and Phase Space, pages 2-20, Springer-Verlag, Berlin, 1989. Proceedings
           of International Colloquium on Wavelets and Applications, Marseille, France, Dec. 1987.
iDvN88}    Z. Doanata, P. P. Vaidyanathan, and T. Q. Nguyen. General synthesis procedures for FIR
           lossless transfer mlatrices, for perfect-reconstruction muitirate fliter bank applications. IEEE
            Tn刃is口c挽ons on Acou就扼5, 枷eech, 口nd S四n毗 Process勿四， 36(10):1561小1574, October 1988.
[Eir92]    T. Eirola. Sobolev characterization of solutions of dilation equations. SIAM Journal of
           Mathematical Analysis, 23(4):1015-1030, July 1992.
[FHV93}    M. Farge, J. C. R. Hunt, and J. C. Vassilicos, editors. Wavelets, Fractals, and Fourier
           Tranforms. Clarendon Press, Oxford, 1993. Proceedings of a conference on Wavelets at
           Newnham College, Cambridge, Dec. 1990.
[FK94J     Efi Foufoula-Georgiou and Praveen Kumar, editors. Wavelets in Geophyics. Academic
           Press, San Diego, 1994. Volume in the series: Wavelet Analysis and its Applications.
[Fli9식     F. J. Fliege. M毗竹口te 1万gital Sign口I Processing: IvIul打-ir口te Systems, Filter B口n无5, 口nd
           Wavelets. Wiley & Sons, New York, 1994.
[Gab46]    D. Gabor. Theory of communication. Journal of the Institute for Electrical Engineers,
           93:429-439, 1946.
[GB90]     R. A. Gopinath and C. S. Burrus. Efficient computation of the wavelet transforms. In Pro-
           ceedings 0/ 坑e IEEE Intern口tion口1 Conference on Acous挽cs, 枷eech, 口nd S四n毗 尸rocess初四，
           pages 1599-1602, Albuquerque, NM, April 1990.
230                                                                                       Bibliography


[GB92a]    R. A. Gopinath and C. S. Burrus. Cosine中modulated orthonormal wavelet bases. In Paper
           Summar그es 加r 坑e IE月E 毓gn口I Processing Soc扼切 'S 夙／th DSP Wor丸毗O1기 page 1.10.1,
           Starved Rock Lodge, Utica, IL, September 13-16, 1992.
[GB92b]    R. A. Gopinath and C. S. Burrus. On the moments of the scaling function 砂o. In Proceedings
           of the IEEE International Symposium on Circuits and Systems, pages 963-966, ISCAS-92,
           San Diego, CA, May 1992.
[GB92c}    R. A. Gopinath and C. S. Burrus. Wavelet transforms and filter banks. In Charles K. Chui,
           editor, Wavelets: A Tutorial in Theory and Applications, pages 603-655, Academic Press,
           San Diego, CA, 1992. Volume 2 in the series: Wavelet Analysis and its Applications.
[GB93]     R. A. Gopinath and C. S. Burrus. Theory of modulated filter banks and modulated wavelet
           tight frames. In Proceedings of the IEEE International Conference on Signal Processing,
           pages III-169--172, IEEE ICASSP-93, Minneapolis, April 1993.
[GB94a]    R. A. Gopinath and C. S. Burrus. On upsampling, downsampling and rational sampling
           rate filter banks. IEEE Transactions on Signal Processing, April 1994. Also Tech. Report
           No. CML TR91-25, 1991.
[GB94b]    R. A. Gopinath and C. S. Burrus. Unitary FIR filter banks and symmetry. IEEE Transaction
           on Circuits and Systems II, 41:695-700, October 1994. Also Tech. Report No. CML TR92-
           17, August 1992.
[GB95a]    R. A. Gopinath and C. S. Burrus. Factorization approach to unitary time-varying filter
           banks. IEEE Transactions on Signal Processing, 43(3):666-680, March 1995. Also a Tech
           Report No. CML TR-92-23, Nov. 1992.
[GB95b]    R. A. Gopinath and C. S. Burrus. Theory of modulated filter banks and modulated wavelet
           tight frames. A刃j兄可ed 口nd Coi九끄utational 丑ai刃zonic An毗彫5: 仍／口velets and S四n｛工1 Process-
           ing, 2:303-326, October 1995. Also a Tech. Report No. CML TR-92-10, 1992.
[GB95c]    Ramesh A. Gopinath and C. Sidney Burrus. On cosine-modulated wavelet orthonormal
           bases. IEEE Transactions on Image Processing, 4(2):162-176, February 1995. Also a Tech.
           Report No. CML TR-91-27, March 1992.
[GB96a]    Haitao Guo and C. Sidney Burrus. Approximate FFT via the discrete wavelet transform.
           In Proceedings of SPIE Conference 282,5, Denver, August 6-9 1996.
[GB96b]    Haitao Guo and C. Sidney Burrus. Convolution using the discrete wavelet transform. In Pro-
           ceedings a/ 坑e IEEE Intei斗2（比ion口I Conference on Acous挽cS, 枷eec九， 口nd 航gnal Processing,
           pages 111-1291-1294, IEEE ICASSP-96, Atlanta, May 7-10 1996.
[GB96c]    Haitao Guo and C. Sidney Burrus. Phase-preserving compression of seismic images using
           the self-adjusting wavelet transform. In NASA Combined Indust긔, Space and Earth Science
           Data Compression Workshop (in conjunction with the IEEE Data Compression Conference,
           DCC-96), JPL Pub. 96-11, pages 101나109, Snowbird, Utah, April 4 1996.
[GB97a]    Haitao Guo and C. Sidney Burrus. Fast approximate Fourier transform via wavelet trans-
           forms. IEEE Transactions on Signal Processing, submitted, January 1997.
[GB97b]    Haitao Guo and C. Sidney Burrus. Waveform and image compression with the Burrows
           Wheeler transform and the wavelet transform. In Proceedings of the IEEE International
           Conference on Image Processing, IEEE ICIP-97, Santa Barbara, October 26-29 1997.
[GB97cJ    Haitao Guo and C. Sidney Burrus. Wavelet transform based f就 approximate Fourier
           transform. In Proceedings of the IEEE Inte斗2ational Conference on Acoustics, Speech, and
           Signal Processing, pages III:1973-1976, IEEE ICASSP-97, Munich, April 21-24 1997.
[GGM84a]   P. Goupillaud, A. Grossman, and J. Morlet. Cyclo-octave and related transforms in seismic
           signal analysis. SIAM J. Math. Anal., 15:723-736, 1984.
 BIBLIOGRAPHY
                                                                                                     231

 [GGM84b]    P. Groupillaud, A. Grossman, and J. Monlet. Cyclo-octave and related transforms in seismic
             signal analysis. Geoexploration, (23), 1984.
 [GGT89]     S. Ginette, A. Grossmann, and Ph. Tchamitchian. Use of wavelet transforms in the study
             of propagation of transient acoustic signals across a plane interface between two homoge-
             neous media. In J. M. Combes, A. Grossmann, and Ph. Tchamitchian, editors, Wavele幻:
             Time-Frequency Methods and Phase Space, pages 139-146, Springer-Verlag, Berlin, 1989.
             Proceedings of the International Conference, Marseille, Dec. 1987.
 [GHM94}     J. S. Geronimo, D. P. Hardin, and P. R. Massopust. 까actal functions and wavelet expansions
             based on several scaling functions. Journal of Approrimation Theory, 78:373-401, 1994.
 {GKM89J     A. Grossman, R. Knonland-Martinet, and J. Monet. Reading and understanding continuous
             wavelet transforms. In J. M. Combes, A. Grossmann, and Ph. Tchamitchian, editors,
             Wavelets, Time-Frequency Methods and Phase Space, pages 2-20, Springer-Verlag, Berlin,
             1989. Proceedings of International Colloquium on Wavelets and Applications, Marseille,
             France, Dec. 1987.
[GL93]       C. H. Golub and C. F. Van Loan. Matrix Compuations. Johns Hopkins University
                                                                                          Press,
             1993.
[GL94]       T. N. T. Goodman and S. L. LEE. Wavelets of multiplicity r.          Tran. Ame仇can Mat九.
             Society, 342(1) :307-324, March 1994.
[GLOB95}     H. Guo, M. Lang, J. E. Odegard, and C. S. Burrus. Nonlinear processing of a shift-invariant
             DWT for noise reduction and compression. In Proceedings of the International Conference
             on Digital Signal Processing, pages 332-337. Limassol. Cyprus. June 26-28 1995.
[GLRT90J    R. Glowinski, W. Lawton, M. Ravachol. and E. Tenenbaum. \Vavelet solution of linear and
            nonlinear elliptic, parabolic and hyperbolic problems in one dimension. In Proceedings of
            坑e Ninth SIAM Inte?斗iation口1 Conference on Comp毗ing 人le仇（)ds in A끄끄i扼d Sciei比es 口nd
            Enginee忖ng, Philadelphia, 1990.
[GLT931     T. N. T. Goodman, S. L. Lee. and W. S. Tang. Wavelets in wandering subspaces.
                                                                                          Thin.
            American Math. Society. 338(2):639-654. August 1993.
[GOB92]     R. A. Gopinath, J. E. Odegard. and C. S. Burrus. On the correlation structure of multiplicity
            M scaling functions and wavelets. In Proceedings of the IEEE International Symposiu力1 on
            Circuits and Systems, pages 959-962. ISCAS-92. San Diego, CA, May 1992.
[OOB94]     R. A. Gopinath, J. E. Odegard, and C. S. Burrus. Optimal wavelet representation of
            signals and the wavelet sampling theorem. IEEE Transactions on Circuits and Systems II,
            41(4):262-277, April 1994. Also a Tech. Report No. CML TR-92-05, April 1992, revised
            Aug. 1993.
[GOL*94aJ   H. Guo, J. E. Odegard, M. Lang, R. A. Gopinath, I. Selesnick, and C. S. Burrus. Speckle re-
            duct ion via wavelet soft-thresholding with application to SAR based ATD/R. In Proceedings
            of SPIE Conference 2260, San Diego. July 1994.
[GOL*94b1 H. Guo, J. E. Odegard, M. Lang, R. A. Gopinath, I. W. Selesnick, and C. S. Burrus. Wavelet
          based speckle reduction with application to SAR based ATD/R. In Proceedings of the IEEE
          International Conference on Image Processing, pages 1:75中79, IEEE ICIP-94, Austin, Texas,
          November 13-16 1994.
[Gop90}     Ramesh A. Gopinath. The Wavelet 升ansforms and Time-Scale Analysis of Signals. Mas-
            ter뇽 thesis, Rice University, Houston, Tx 77251, 1990.
[Gop92j     Ram田h A. Gopin毗h. 14乞刃elets and F玎ter Bai琉s - New Resu尻s and A까流口功ion且 PhD
            thesis, Rice University, Houston, Tx, August 1992.
232                                                            .                           Bibliography


[Gop96a]   R. A. Gopinath. Modulated filter banks and local trigonometric bases - some connections,
           Oct 1996. in preparation.
[Gop96b]   R. A. Gopinath. Modulated filter banks and wavelets, a general unified theory. In Pro-
           ceedzngs of the IEEE International Conference on Acoustics, Speech, and Signal Processing,
           pages 1585-1588, IEEE ICASSP-96, Atlanta, May 7-10 1996.
[GORB96]   3. G6tze, J. E. Odegard, P. Rieder, and C. S. Burrus. Approximate moments and regularity
           of efficiently implemented orthogonal wavelet transforms. In Proceedings of the IEEE Inter-
           national Symposium on Circuits and Systems, pages 11-405-408, IEEE ISCAS-96, Atlanta,
           May 12-14 1996.
[Gri93]    Gustaf Gripenberg. Unconditional bases of wavelets for Sobelov spaces. SIAM Journal of
           Mathematical Analysis, 24(4):1030-1042. July 1993.
[Guo94}    Haitao Guo. Redundant Wavelet P口nsform and Denoising. Technical Report CML-9417,
           ECE Dept and Computational Mathematics Lab, Rice University, Houston, Tx, December
           1994.
[Guo95]    Haitao Guo. Theo그／and Applications of the Shift-Invariant, Time- Varying and Undecimated
           Wavelet Transform. Master's thesis, ECE Department, Rice University, April 1995.
[Guo9기     Haitao Guo. W口vele拓 /or Approxim口比 Fourier 升ansfoi斗n 口nd D口t（工 (Yom끄ression. PhD
           thesis, ECE Department, Rice University, Houston, Tx, May 1997.
[Haa10]    Alfred Haar. Zur Theorie der orthogonalen Funktionensysteme. Mathernatische Annalen,
           69:331-371, 1910. Also in PhD thesis.
[HB92]     F. Hlawatsch and G. F. Boudreaux-Bartels. Linear and quadratic time-frequency signal
           representations. lEE万 S四n口i 尸rocessing M四口名初le, 9(2):21-67, April 1992.
[Hei93]    Henk J. A. M. Heijmans. Descrete wavelets and multiresolution analysis. In Torn H. Koorn-
           winder, editor, l'뇨velets: An 風em아2t口7김 Tre毗ment of T九eoi낑 (m72d A끄I兄ic口挽ons, pages 49
           80, World Scientific, Singapore, 1993.
[Hel95]    Peter N. Heller. Rank m wavelet matrices with n vanishing moments. SIAM Journal on
           Matrix Analysis, 16:502-518, 1995. Also as technical report AD940123, Aware, Inc., 1994.
[Her71]    O. Herrmann. On the approximation problem in nonrecursive digital filter design. IEEE
           Tr口nsaction,9 on circuit Tbfory. 18:411-413, May 1971. Reprinted in DSP reprints. IEEE
           Press, 1972, page 202.
[HHSM95]   A. N. Hossen, U. Heute, O. V. Shentov, and S. K. Mitra. Subband DFT - Part II: accuracy,
           complexity, and applications. Signal Processing, 41:279-295, 1995.
[HKRV92]   Cormac Herley, Jelena Kov亡evh, Kannan Ramchandran, and Martin Vetterli. Time-
           varying orthonormal tilings of the time-frequency plane. In Proceedings of the IEEE Signal
           Processing Society 's International Symposium on Time-Frequency and Time-Scale Analy-
           sis, pages 11-14, Victoria, BC, Canada, October 4-6, 1992.
[HKRV93]   Cormac Herley, Jelena Kova亡evid, Kannan Ramchandran, and Martin Vetterli. Tilings of the
           time-frequency plane: consturction of arbitrary orthogonal bases and f戚 tiling algorithms.
           IEEE 升ansactions on Signal Processing, 41(12):3341小3359, December 1993. Special issue
           on wavelets.
IHPW941    Fr6d6ric Heurtaux, Fabrice Planchon, and Mladen V. Wickerhauser. Scale decomposition
           in Burgers' equation. In John J. Benedetto and Michael W. Frazier, editors, Wavelets:
           凡a卄比m比比s and A끄j兄叱ations, pages 505小524, CRC Press, Boca Raton, 1994.
[HR9이      D. P. Hardin and D. ＼사． Roach. M毗2W凹毗tPre再lters /: Or坑ogonal 끄re／氾ers preser그flng
           approximation order p < 2. Technical Report, Vanderbilt University, 1996.
 BIBLIOGRAPHY
                                                                                                   233

 {HRW92]     Peter N. Heller, Howard L. Resnikoff, and Raymond O. Wells, Jr. Wavelet matrices and
             the representation of discrete functions. In Charles K. Chui, editor, Wavelets: A T比o仇al
             in Theo八／ and Applications, pages 15-50, Academic Press, Boca Raton, 1992. Volume 2 in
             the series: Wavelet Analysis and its Applications.
 [HSS*95]    P. N. Heller, V. Strela, C. Strang, P. Topiwala, C. Heil, and L. S. Hills. Multiwavelet
             filter banks for data compression. In IEEE Proceedings of the International Symposium on
             Circuits and Systems, pages 1796-1799, 1995.
 [HSS96]     C. Heil, G. Strang, and V. Strela. Approximation by translates of refinable functions.
             Numer낱sche 兀I,口坑em（功i自 73(1):75-94, March 1996.
[Hub961      Barbara Burke Hubbard. The World According to Wavelets. A K Peters, Wellesley, MA,
             1996.
[HW89]       C. E. Heil and D. F. Walnut. Continuous and discrete wavelet transforms. SIAM Review,
             31(4):628-666, December 1989.
[HW94]      Peter N. Heller and R. O. Wells. The spectral theory of multiresolution operators and
            applications. In C. K. Chui, L. Montefusco, and L. Puccio, editors, Wavelets: Theory,
            Algorithms, and Applications, pages 13-31, Academic Press, San Diego, 1994. Also as
            technical report AD930120, Aware, Inc., 1993; Volume 5 in the series: Wavelet Analysis
            and its Aj가冗比毗切ns.
[HW96a]     Peter N. Heller and R. O. Wells. Sobolev regularity for rank M wavelets. SIAM Journal on
            Mathematical Analysis, submitted, Oct. 1996. Also a CML Technical Report TR9608, Rice
            University, 1994.
{HW96b]     Eugenio Hernandez and Guido Weiss. A First Course on Wavelets. CRC Press, Boca Raton,
            1996.
[IRP*96]    Plamen Ch. Ivanov, Michael C Rosenblum, C.-K. Peng. Joseph Mietus, Shlomo Havlin,
            H. Eugene Stanley, and Ary L. Goldberger. Scaling behaviour of heartbeat intervals obtained
            by wavelet-based time-series analysis. Nature. 383:323-327. September 26 1996.
[JB82]      H. W. Johnson and C. S. Burrus. The design of optimal DFT algorithms using
                                                                                         dynamic
            programming. In Proceedings of the IEEE International Conference on Acoustics, Speech,
            and Signal Processing. pages 20-23. Paris, May i982.
[JCF95]     R. L. Josho, V. J. Crump, and T. R. Fischer. Image subband coding using arithmetic coded
            trellis coded（쁘antiz毗油1. Th沼月 가口nsactions on C壬rcuz拓 口nd Systems, 515-523, December
            1995.
[Jia95]     R. Q. Jia. Subdivision schemes in L, spaces. Advances in Computational Mathematics,
            3:309-341, 1995.
[JMNK96]    Bruce R. Johnson, Jason P. Modisette, Peter A. Nordlander, and James L. Kinsey. Quadra-
            ture Integration for Compact Support Wavelets. Technical Report, Chemistry Dept. Rice
            University, November 1996. preprint. submitted to Journal of Computational Physics.
[JN84]      N. S. Jayant and P. Noll. Digital Coding of Waveforms. Prentice-Hall, Inc., Englewood
            Cliffs, NJ, 1st edition, 1984.
[JRZ96a]    R. Q. Jia, S. D. Riemenschneider, and D. X. Zhou. Approximation by Multiple Refinable
            Functions. Technical Report, University of Alberta, 1996. To appear in: Canadian Journal
            of Mathematics.
[JRZ96b]    R. Q. Jia, 5. D. Riemenschneider, and D. X. Zhou. Vector Subdivision Schemes and Multiple
            Wavelets. Technical Report, University of Alberta, 1996.
234                                                                                        BbIiography


[JRZ97J    R. Q. Jia, S. D. Riemenschneider, and D. X. Zhou. Smoothness of Multiple Refinable
           Functions and Multiple Wavelets. Technical Report, University of Alberta, 1997.
[JS94a]    Bj6rn Jawerth and Wim Sweldens. An overview of wavelet based multiresolution analyses.
           SIAM Review, 36:377-412, 1994. Also a University of South Carolina Math Dept. Technical
           Report, Feb. 1993.
[JS94b]    I. 入4. 而h毗one and B. ＼入／. Silverman. 仍／口velet Threshold Estim口切rs for 1）口t（工 ii凡t九 Corre-
           lated Noise. Technical Report, Statistics Dept., University of Bristol, September 1994.
[Kai941    G. Kaiser. A Friendly Guide to Wavelets. Birkh瓦user, Boston, 1994.
[KMDW95I H. Krim, S. Mallat, D. Donoho, and A. Wilisky. Best basis algorithm for signal enhance-
         ment. In Proceediv四s of the／月EE Ii功이斗I口tional Conference on Acou就ics, 枷eech, and S匈n口i
         Processing, pages 1561-1564, IEEE ICASSP-95 Detroit, May 1995.
[Koo93}    Tom H. Koornwinder, editor. Wavelets: An Elementary Treatment of Theory and Applica-
           tions. World Scientific, Singapore, 1993.
[KR9이      G. Kaiser and M. B. Ruskai, editors. NSF/CMBS Regional Conference on Wavelets. Uni-
           versity of Lowell, MA, June 11 - 15, 1990. Speakers: I.Daubechies, G.Beylkin, R.Coifman,
           S.Mallat, M.Vetterli, Aware, Inc.
[KS92[      A. A. A. C. Kalker and Imran Shah. La妃er structures for multidimensional linear phase
            perfect reconstruction filter banks and wavelets. In Proceedings of SPIE Conference 1818
            on Visual Communications and Image Processing, 1992.
[KT93J      Jaroslav Kautsky and Radko Turcajov丘. Discrete biorthogonal wavelet transforms as block
            circulant matrices. Linear Algegra and its Applications, submitted 1993.
[KT94a]     Jaroslav Kautsky and Radko Turcajov瓦. A matrix approach to discrete wavelets. In
            Charles K. Chui, Laura Montefusco, and Luigia Puccio, editors, Wavelets: Theory, Al-
            gorithms, and Applications, pages 117-136, Academic Press, Boca Raton, 1994. Volume 5
            in the series: Wavelet Analysis and its Applications.
[KT94b]    Man Kam Kwong and P. T. Peter Tang. W-matrices, nonorthogonal multiresolution anal-
           ysis, and finite signals of arbitrary length. preprint, 1994.
]KV921      R. D. Koilpillai and P. P. Vaidyanathan. Cosine modulated FIR filter banks satisfying
            perfect reconstruction. IEEE Transactions on Signal Processing, 40(4):770-783, April 1992.
[Kwo94]     Man Kam Kwong. MATLAB implementation of W-matrix multiresolution analyses. preprint-
            兀fCS-I가砲刃羽. , September 1994.
[Law]       W. Lawton. Private communication.
[Law90]     Wayne M. Lawton. Tight frames of compactly supported affine wavelets. Journal of Math-
            ematical Physics, 31(8):1898-1901, August 1990. Also Aware, Inc. Tech Report AD891012.
[Law91a]    Wayne M. Lawton. Multiresolution properties of the wavelet Galerkin operator. Journal of
            兀化坑em口tic口11가zysics, 32(6):1440-1443, June 1991.
[Law91b]    Wayne M. Lawton. Necessary and sufficient conditions for constructing orthonormal wavelet
            bases. Jour孔al o/ 九I口坑e丁n毗元毗 P似眉ics, 32(1):57-61, January 1991. Also Aware, Inc. Tech.
            Report AD900402, April 1990.
[Law97]     Wayne M. Lawton. Infinite convolution products & refinable distributions on Lie groups.
            Transt工ctions 可 坑e 小ne仇can 加m坑em口仇c口I Soce侃y, submitted 1997.
[LGO*95]    M. Lang, H. Guo, J. E. Odegard, C. S. Burrus, and R. O. Wells, Jr. Nonlinear processing
            of a shift-invariant DWT for noise reduction. In Harold H. Szu, editor, Proceedings of SPIE
            Confer毛nce 芻9', 才口velet Apj元化口tions //, pages 640-651, Orlando, April 17卜211995.
BIBLIOGRAPHY                                                                                       235


[LGO半96]   M. Lang, H. Guo, J. E. Odegard, C. S. Burrus, and R. O. Wells, Jr. Noise reduction using
           an undecimated discrete wavelet transform. IEEE Signal Processing Letters, 3(1):10-12,
           January 1996.
[LGOB95]   M. Lang, H. Guo, J. E. Odegard, and C. S. Burrus. Nonlinear redundant wavelet methods
           for image enhancement. In Proceedings of IEEE Workshop on Nonlinear Signal and Image
           Processing, pages 754놔757, Halkidiki, Greece, June 20-22 1995.
[LH96]     Markus Lang and Peter N. Heller. The design of maximally smooth waviets. In Proceed-
           zags a/ 仇e IEEE Intei꾸I口t可onal Conference on Acoustics夕 枷eec／工, 口nd Sign口1 Processing,
           pages 1463-1466, IEEE ICASSP-96, Atlanta, May 1996.
[Lin9司     A. R. Lindsey. Gener毗ized Or仇ogon口i勺 Mult洌e工ed Commi工nicatioi工 刃ia Wavelet P口cket
           Bases. PhD thesis, June 1995.
[LKC*94J   R. E. Learned, H. Krim, B. Claus, A. S. Willsky, and W. C. Karl. Wavelet-packet-based
           multiple access communications. In Proceedings of SPIE Conference, Wavelet Applications
           in Signal and Image Processing, Vol. 2303, pages 246-259, San Diego, July 1994.
[LLK96}    K.-C. Lian, J. Li, and C.-C. J. Kuo. Image compression with embedded multiwavelet coding.
           In Proceedings of SPIE, Wavelet Application III, pages 165-176, Orlando, FL, April 1996.
[LLS97a]   Wayne M. Lawton, S. L. Lee, and Z. Shen. Convergence of multidimensional cascade alg小
           rithm. Numerische Mathematik, to appear 1997.
[LLS97b]   Wayne M. Lawton, S. L. Lee, and Z. Shen. Stability and orthonormality of multivariate
           refinable funct沁ns. SIAM Joz玎n毗 of M口坑ematic（工I An口lysis, to appear 1997.
[LM89]     J. L. Larsonneur and J. Morlet. Wavelet and seismic interpretation. In J. M. Combes,
           A. Grossmann, and Ph. Tchamitchian, editors, Wavelets: Time-Frequency Methods and
           Phase Space, pages 126-131, Springer-Verlag, Berlin, 1989. Proceedings of the International
           Conference, Marseille, Dec. 1987.
[LP89]     G. Longo and B. Picinbono, editors. Time and Frequency Representation of Signals and
           Systems. Springer-Verlag, Wien - New York, 1989. CISM Courses and Lectures No. 309.
[LP94a}    Jie Liang and Thomas W. Parks. A translation invariant wavelet representation algorithm
           with applications. IEEE 升ansactions on Signal Processing, submitted April 1994.
[LP94b]    Jie Liang and Thomas W. Parks. A two-dimensional translation invariant wavelet represen-
           tation and its applications. In Proceedings of the IEEE International Conference on Image
           Processing, pages 1:66-70, Austin, November 1994.
[LPT92]    J. Liandrat, V. Perrier, and Ph. Tchamitchian. Numerical resolution of nonlinear parital dif-
           ferential equations using the wavelet approach. In M. B. Ruskai, G. Beylkin, I. Daubechies,
           Y. Meyer, R. Coifman, S. Mallat, and L Raphael, editors, Wavelets and Their Applications,
           pages 181-210, Jones and Bartlett, Boston, 1992. Outgrowth of the NSF/CBMS Conference
           on Wavelets. Lowell, June 1990.
[LR91}     Wayne M. Lawton and Howard L. Resnikoff. Multidimensional Wavelet Bases.              Aware
           Report AD910130. Aware, Inc., February 1991.
[LRO97J    S. M. LoPresto, K. Ramchandran, and M. T. Orchard. Image coding based on mixture
           modeling of wavelet coefficients and a fast estimation-quantization framework. Proc. DCC,
           March 1997.
[LSOB94]   M. Lang, I. Selesnick, J. E. Odegard, and C. S. Burrus. Constrained FIR filter design for
           2-band filter banks and orthonormal wavelets. In Proceedings of the IEEE Digital Signal
           Processing Workshop, pages 211-214, Yosemite, October 1994.
236
                                                                                             Bibliography

{LV95J      Yuan-Pei Lin and P. P. Vaidyanathan. Linear phase cosine-modulated filter banks. IEEE
            Transactions on Signal Processing, 43, 1995.
[Ma189a]    S. G. Mallat. Multifrequency channel decomposition of images and wavelet models. IEEE
            Transactions on Acoustics, Speech and Signal Processing, 37:2091-2110, December 1989.
小ial89bJ    S. G. Mallat. Multiresolution approximation and wavelet orthonormal bases of L2. T口ns-
            口ctions of t九e An比汽c口nA／   口坑ematic毗 Soc可e却／, 315:69寸87, 1989.
小1a189c]    S. G. Mallat. A theory for multiresolution signal decomposition: the wavelet representation.
            ／月E万 가口nsac挽ons on Pattei了lRecognition 口nd 兀化c九土ne mt日瓦gence, 11(7):674-693, July
            1989.
小4a19치      S. G. 入tallat. Zer口crossings of a wavelet transform. IEEE 升口ns口毗ons on Info竹n口tion
            Theory, 37(4):1019-1033, July 1991.
小4a192]     Henrique S. Malvar. Signal Processing with Lapped Transforms. Artech House, Boston, MA,
            1992.
小4a197]     St6phane Mallat. Wavelet Signal Processing. Academic Press, 1997. to appear.
[Mar91]     R. J. Marks II. Introduction to Shannon Sampling and Interpolation Theory.
                                                                                       Springer-
            Verlag, New York, 1991.
[Mar92]     T. G. Marshall, Jr. Predictive and ladder realizations of subband coders. In Proceedings of
            IEEE Workshop on Visual Signal Processing and Communication, Raleigh, NC, 1992.
[Mar93]     T. C. Marshall, Jr. A fast wavelet transform based on the eucledean algorithm. In Pro-
            ceedings of Conference on Information Sciences and Systems, Johns Hopkins University,
            1993.
[Mas94]     Peter R. Massopust. Fractal 只1nctions, Fractal Surfaces, and Wavelets. Academic Press,
            San Diego, 1994.
[Mau92]     J. Mau. Perfect reconstruction modulated filter banks. In Proc. mtt. Conf. Acoust., Speech,
            Signal Processing, pages IV-273, IEEE, San Francisco, CA, 1992.
小Iey87]    Y. Meyer. L'analyses par ondelettes. Pour la Science, September 1987.
[Mey89]    Y. Meyer. Orthonormal wavelets. In J. M. Combes, A. Grossmann, and Ph. Tchamitchian,
           editors. Wavelets. Time-Frequency Methods and Phase Space. pages 21-37. Springer-Ver
                                                                                                lag,
           Berlin, 1989. Proceedings of International Colloquium on Wavelets and Applications, Mar-
           seille, France, Dec. 1987.
[Mey90]    Y. Meyer. Ondelettes et oprateurs. Hermann, Paris, 1990.
[Mey92a]   Y. Meyer, editor. Wavelets and Applications. Springer-Verlag, Berlin, 1992. Proceedings
           of the Marseille Workshop on Wavelets, France, May, 1989; Research Notes in Applied
           Mathematics, RMA그0.
[Mey92b]   Yves Meyer. Wavelets and Operators. Cambridge, Cambridge, 1992. Translated by D. H.
           Salinger from the 1990 French edition.
[Mey93]    Yves Meyer. Wavelets, Algorithms and Applications. SIAM, Philadelphia, 1993. Translated
           by R. D. Ryan based on lectures given for the Spanish Institute in Madrid in Feb. 1991.
[MF97]     St6phane Mallat and Fr6d6ric F섧zon. Understanding image transform codes. In Proceedings
           of SPIE Conference, Aerosense, Orlando, April 1997.
[MLB89]    Cleve Moler, John Little, and Steve Bangert. NIATLAB User 's Guide. The MathWorks, Inc.,
           South Natick, MA, 1989.
[MMOP96} Michel Misiti, Yves Misiti, Georges Oppenheim, and Jean-Michel Poggi. Wavelet Toolbox
         User 's Guide. The MathWorks, Inc., Natick, MA, 1996.
미BL山GRAPHY                                                                                         237


小4ou93]     Pierre Moulin. A wavelet regulariz毗油method for d浚出e radar-target im晦旽 and s附:kle-
            noise reduction. Jou了tal of Mathematical Imaging and Vision, 3:123-134, 1993.
[MP89]      C. A. Micchelli and Prautzsch. Uniform refinement of curves. Linear Algebra, Applications,
            114/115:841-870, 1989.
[MW94a]     Stephen Del Marco and John Weiss. Improved transient signal detection using a wavepacket-
            based detector with an extended translation-invariant wavelet transform. IEEE Transactions
            on Signal Processing, 43, submitted 1994.
[MW94b]     Stephen Del Marco and John Weiss. M-band wavepacket-based transient signal detector
            using a translation-invariant wavelet transform. Optical Enginee仇ng, 33(7):2175-2182, July
            1994.
小4＼人／J94]   Stephen Del Marco, John Weiss, and Karl Jagler. Wavepacket-based transient signal detec-
            tor using a translation invariant wavelet transform. In Proceedings of Conference on Wavelet
            Applications, pages 792-802, SPIE, Orlando, FL, April 1994.
小4Z93]      S. G. Mallat and Z. Zhang. Matching pursuits with time-frequency dictionaries. IEEE
            Transactions on Signal Processing, 41(12):3397-3415, December 1993.
[NAT96]     Mohammed Nafie, Murtaza Ali, and Ahmed Tewfik. Optimal subset selection for adaptive
            signal representation. In Proceedings of the IEEE International Conference on Acoustics,
            Speech, and Signal Processing, pages 2511-2514, IEEE ICASSP-96, Atlanta, May 1996.
[Ngu92]     T. Q. Nguyen. A class of generalized cosine-modulated filter banks. In Proceedings of
            ISCAS, San Diego, CA, pages 943-946, IEEE, 1992.
[Ngu94]     Trong Q. Nguyen. Near perfect reconstruction pseudo QMF banks. IEEE 升ansactions on
            Signal Processing, 42(1):65-76, January 1994.
[Ngu95a]    Trong Q. Nguyen. Digital filter banks design quadratic constrained formulation. IEEE
            Transactions on Signal Processing, 43(9):2103-2108, September 1995.
{Ngu95b]    Truong Q. Nguyen. Aliasing-free reconstruction filter banks. In Wai-Kai Chen, editor, The
            Circuits and Filters Handbook, chapter 85, pages 2682-2717, CRC Press and IEEE Press,
            Roca Raton, 1995.
[NH96]      'fl나oiig Q. Nguyen and Peter N. Heller. Biorthogo1ial cosine-modulated filter band. In Pro-
            ceedings of the IEEE International Conference on Acoustics, Speech, and Signal Processing,
            pages 1471-1474, IEEE ICASSP-96, Atlanta, May 1996.
[NK92]      T. Q. Nguyen and R. D. Koilpillai. The design of arbitrary length cosine-modulated filter
            banks and wavelets satisfying perfect reconstruction. In Proceedings of IEEE-SP Symposium
            on Time-F卜equency 口nd Time-S口妃e 凡lethods '92夕 Vic切9.吼L 夙Y, pages 299-302, IEEE, 1992.
[nRGB91j    D. L. Jones nd R. G. Barniuk. Efficient approximation of continuous wavelet transforms.
            Electronics Letters, 27(9):748-750, 1991.
$595]       C. P. Nason and B. W. Silverman. The Stationary Wavelet Transfo斗7i and some Statistical
            Applications. Technical Report, Department of Mathematics, University of Bristol, Bristol,
            UK, February 1995. preprint obtained via the internet.
[NV881      T. Q. Nguyen and P. P. Vaidyanathan. Maximally decimated perfect-reconstruction FIR
            filter banks with pairwise mirror-image analysis and synthesis frequency responses. IEEE
            Transactions on Acoustics, Speech, and Signal Processing, 36(5):693-706, 1988.
[OB95]      J. E. Odegard and C. S. Burrus. Design of near-orthogonal filter banks and wavelets by
            Lagrange multipliers. 1995.
238                                                                                        BbIiography


四B96a]     Jan E. Odegard and C. Sidney Burrus. New class of wavelets for signal approximation. In
           Proceedings of the IEEE Interiiational Symposium on Circuits and Systems, pages 11-189
           192, IEEE ISCAS-96, Atlanta, May 12-15 1996.
[OB96b]    Jan E. Odegard and C. Sidney Burrus. Toward a new measure of smoothness for the design
           of wavelet basis. In Proceedings of the IEEE International Conference on Acoustics, Speech,
           and Signal Processing, pages 111-1467-1470, IEEE ICASSP-96, Atlanta, May 7-10 1996.
回B97]      J. E. Odegard and C. S. Burrus. Wavelets with new moment approximation properties.
           I月E万 T'ran敬比抗ons on S四nal Process勿四） submitted, January 1997.
[Ode96]    J. E. Odegard. Moments, smoothness and optimization of wavelet systems. PhD thesis, Rice
           University, Houston, TX 77251, USA, May 1996.
[OGB92]    J. E. Odegard, R. A. Gopinath, and C. S. Burrus. Optimal wavelets for signal decomp口
           sition and the existence of scale limited signals. In Proceedings of the IEEE International
           Conference on Signal Processing, pages IV 597-600, ICASSP-92, San Francisco, CA, March
           1992.
[OGB94}    J. E. Odegard, R. A. Gopinath, and C. S. Burrus. Design of Linear Ph口se Cosine Modulated
           Filter Banks for Subband Image Compression. Technical Report CML TR94-06, Computa-
           tional Mathematics Laboratory, Rice University, Houston, TX, February 1994.
[OGL*95]   J. E. Odegard, H. Guo, M. Lang, C. S. Burrus, R. O. Wells, Jr., L. M. Novak, and M.
           Hiett. Waelet based SAR speckle reduction and image compression. In Proceedings of
           SPIE Conference 287, Algorithms for SAR Imagery II, Orlando, April 17-21 1995.
[OS89]     A. V. Oppenheim and R. W. Schafer. Discrete- Time Signal Processing. Prentice-Hall,
           Englewood Cliffs, NJ, 1989.
[OY873     Ozdoan Yilmaz. Seismic Data Processing. Society of Exploration Geophysicists, Tulsa,
           1987. Stephen M. Doherty editor.
[P P89[    P. P. Vaidyanathan and Z. Doanata. The role of lossless systems in modern digital signal
           processing: a tutorial. IEEE 가ansactions on Education, August 1989.
[Pap77]    Athanasios Papoulis. Signal Analysis. McGraw-Hill, New York, 1977.
[PB87]     T. W. Parks and C. S. Burrus. Digital Filter Design. John Wiley & Sons, New York, 1987.
[PKC96]    J. C. Pesquet, H. Krim, and H. Carfantan. Time-invariant orthonormal wavelet represen-
           tations. IEEE 升ansactions on Signal Processing, 44(8):1964-1970, August 1996.
[Plo95aJ   C. Plonka. Approximation order provided by refinable function vectors. Technical Re-
           port 95/1, Universitt Rostock, 1995. To appear in: Constructive Approximation.
[Plo95b]   G. Plonka. Approximation properties of multi-scaling functions: a fourier approach. 1995.
           Rostock. Math. Kolloq. 49, 115-126.
[Plo95c}   G. Plonka. Factorization of refinement masks of function vectors. In C. K. Chui and L. L.
           Schumaker, editors, W口velets and 兀ful玭印el 枷刃rox2ma蜘n, pages 31卜說속 w아닢 Scient小c
           Publishing Co., Singapore, 1995.
[1기o97aJ   G. I기onka. Necess（工7꼬／and sn毋icient conditions for or坑onormali匈 of sc毗丘my 刃ectors. Tech-
           nical Report, Un如아5抗毗 Rostock, 1997.
[Plo97b]   C. Plonka. On stability of scaling vectors. In A. Le Mehaute, C. Rabut, and L. L. Schumaker,
           editors, Sur／口ce F仇仇ng 口nd 丸包尻却esolution 兀fe坑ods, Vanderbilt Un如町荀ty Pre弱，Nash너Ile,
           1997. Also Technical Report 1996/15, Universit苞t Rostock.
[Polarl    D. Pollen. Daubechies' scaling function on [0,3]. J. American Math. Soc., to appear. Also
           Aware, Inc. tech. report AD891020, 1989.
 BIBLIOGRAPHY
                                                                                                    239

 [PS95]     G. Plonka and V. Strela. Const크iction of multi-scaling functions with approximatio
                                                                                               n and
            symmetry. Technical Report 95/22, Universitt Rostock, 1995. To appear in: SIAM J.
            Math. Anal.
 [PV96]     See-May Phoong and P. P. Vaidyanathari. A polyphase approach to time-varying
                                                                                              filter
            banks. In Proc. mlt. Conf. Acoust., Speech, Signal Processing, pages 1554-1557. IEEE,
            Atlanta, GA, 1996.
[RBC*92]    M. B. Ruskai, G. Beylkin, R. Coifman, I. Daubechies, S. Mallat, Y. Meyer, and L. Raphael,
            editors. H뇨刃elets 口nd 坑eir A刃I疵cations. 而nes and Bartlett, Bost이i, MA, 1992. Outgrowth
            of NSF/CBMS conference on Wavelets held at the University of Lowell, June 1990.
[RBSB94]   J. O. A. Robertsson, J. O. Blanch, W. W. Symes, and C. S. Burrus. Galerkin-wavelet
           modeling of wave propagation: optimal finite-difference stencil design. Mathematical and
           Computer Modelling, 19(1):31-38, January 1994.
[RC831     L. Rabiner and D. Crochiere. Mu仇rate Digital Signal Processing. Prentice-Hall, 1983.
{RD86]     E. A. Robinson and T. S. Durrani. Geophysical Signal Processing. Prentice Hall, Englewood
           Cliffs, NJ, 1986.
[RD92J     Olivier Rioul and P. Duhamel. Fast algorithms for discrete and continuous wavelet trans-
           forms. IEEE 升ansactions on Information Theory, 38(2) :569-586, March 1992. Special issue
           on wavelets and multiresolution analysis.
[RD94]     Olivier Rioul and Pierre Duhamel. A Remez exchange algorithm for orthonormal wavelets.
           IE万 升口n抛毗叩5 on C茗rcuits 口nd Systems II, 41(8):550-560, August 1994.
[RG95]     Peter Rieder and Jiirgen G6tze. Algebraic optimizaion of biorthogonal wavelet transforms.
           preprint, 1995.
{RGN94J    Peter Rieder, Jiirgen G6tze, and Josef A. Nossek. Algebraic Design of Discrete Wavelet
           升ansforrns. Technical Report TUM-LNS-TR-94-2, Technical University of Munich, April
           1994. Also submitted to IEEE Trans on Circuits and Systems.
[Rio9l]    O. Rioul. Fast computation of the continuous wavelet transform. In Proc. m72t. Conf. Acoust.,
           枷eech, S四n口1 Pn冗ess玎四，IEEE, Toroi此o, Canada, 入larch 1991.
[Rio92]    Olivier Rioul. Simple regularity criteria for subdivision schemes. SIAM J. Math. Anal.,
           23(6):1544-1576, November 1992.
[Rio93a]   Olivier Rioul. A discrete-time multiresolution theory. IEEE T口nsactions on Signal Pro-
           cessing, 41(8):2591-2606, August 1993.
[Rio93b}   Olivier Rioul. Regular wavelets: a discrete-time approach. IEEE Transactions on Signal
           Processing, 41(12):3572-3579, December 1993.
[RN96J     P. Rieder and J. A. Nossek. Smooth multiwavelets based on two scaling functions. In Proc.
           IEEE Conf. on Time-下requency and Time-Scale Analysis, pages 309-312, 1996.
[Ron92]    Amos Ron. Characterization of Linear Independence and Stability of the Sfifts of a
                                                                                              Univari-
           ate Refinable Function in Terms of its Refinement Mask. Technical Report CMS TR 93육
           Computer Science Dept., University of Wisconsin, Madison, September 1992.
{RS83J     L. Rabiner and R. W. Schaefer. Speech Signal Processing. Prentice-Hall. Englewood Cliffs,
           NJ, 1983.
[RT911     T. A. Ramstad and J. P. Tanem. Cosine modulated analysis synthesis filter bank with critical
           sampling and perfect reconstruction. In Proceedings of the IEEE Inte牛lational Conference
           on Acoustics, Speech. and Signal Processing, pages 1789-1792, IEEE ICASSP-91, 1991.
240                                                                                       Bibliography


[Rus92]    Mary Beth Ruskai. Introduction. In M. B. Ruskai, G. Beylkin, R. Coifman, I. Daubechies,
           S. 入4a11at, Y. 入4eyer, and L Raphael, editors, 14뇨낀elet.s and 仇e加 A7叩i扼口t切ns, 加nes and
           Bartlett, Boston, MA, 1992.
[RV91]     Olivier Rioul and Martin Vetterli. Wavelet and signal processing. IEEE Signal Processing
           Magazine, 8(4):14-38, October 1991.
[RV93}     K. Ramchandran and M. Veterli. Best wavelet packet bases in a rate-distortion sense. IEEE
           Transactions on Image Processing, 2(2):160-175, 1993.
[RW97]     H. L. Resnikoff and R. O. Wells, Jr. Wavelet Analysis and the Scalable Structure of Infor-
           mation. Springer-Verlag, New York, 1997. to appear.
[RY90]     K. R. Rao and P. Yip. Discrete Cosine 升ansform - Algorithms, Advantages and Applica-
           tions. Academic Press, 1990.
[SA92]     E. P. Simoncelli and E. H. Adelson. Subband transforms. In John W. Woods, editor, Subband
                                                                                                Tech.
           Image Coding, Kluwer, Norwell, MA, to appear 1992. Also, MIT Vision and Modeling
           Report  No.  137, Sept. 1989.
[Sai94aI   Naoki Saito. Local Feature Extraction and Its Applications Using a Library of Bases. PhD
           thesis, Yale University, New Haven, CN, 1994.
[Sai94b]   Naoki Saito. Simultaneous noise suppression and signal compression using a library of
           orthonormal bases and the minimum discription length criterion. In E. Foufoula-Georgiou
           and P. kumar, editors, Wavelets in Geophysics, Academic Press, San Diego, 1994.
[SB86a]    M. J. Smith and T. P. Barnwell. Exact reconstruction techniques for tree-structured subband
           coders. IEEE T口nsactions on Acoustics, Speech, and Signal Processing, 34:434-441, June
           1986.
[SB86b}    M. J. Smith and T. P. Barnwell III. Exact reconstruction techniques for tree-structured
           引ibband coders. IEEE T卜口n飢比tions on Acous挽cs, 枷eech, 口nd S四n毗 Processii四134:434-
           441, 1986.
[SB871     M. J. Smith and T. P. Barnwell. A new filter bank theory for time-frequency representation.
           IEEE Transactions on Acoustics, Speech, and Signal Processing, 35:314-327, March 1987.
[SB931     H. V. Sorensen and C. S. Burrus. Efficient computation of the DFT with only a subset of
                                                                                                 March
           input or output points. IEEE Transactions on Signal Processing, 41(3):1184-1200,
           1993.
[SC95]     J. A. Storer and M. Cohn, editors. Proceedings of Data Compression Conference. IEEE
           Computer Society Press, Snowbird, Utah, March 1995.
{5C96]     J. A. Storer and M. Cohn, editors. Proceedings of Data Compression Conference. IEEE
           Computer Society Press, Snowbird, Utah, April 1996.
[Sca94]    John A. Scales. Theory of Seismic Imaging. Samizat Press, Golden, CO, 1994.
[Sel96]    I. W. Selesnick. New Techniques for Digital Filter Design. PhD thesis, Rice University,
           1996.
{Sel97]    Ivan W. Selesnick. Parameter初ation of Or坑ogonal Wavelet Systems. Technical Report,
           ECE Dept. and Computational Mathematics Laboratory, Rice University, Houston, Tx.,
           May 1997.
[Sha93]    J. M. Shapiro. Embedded image coding using zerotrees of wavelet coefficients. IEEE 가ans-
            actions on Signal Processing, 41(12):3445-3462, December 1993.
[She92]    M. J. Shensa. The discrete wavelet transform: wedding the a trous and Mallat algorithms.
           ／月EE Tr口ns口ctions on Info竹n毗切nT九eoi가 40:2464-2482, 1992.
텨BL山GRAPHY                                                                                         241


[SHGB93]   P. Steffen, P. N. Heller, R. A. Gopinath, and C. S. Burrus. Theory of regular M-band
           wavelet bases. IEEE Transactions on Signal Processing, 41(12) :3497-3511, December 1993.
           Special Transaction issue on wavelets; Rice contribution also in Tech. Report No. CML
           TR-91-22. Nov. 1991.
[SHS*96]   V. Strela, P. N. Heller, G. Strang, P. Topiwala, and C. Heil. The application of multiwavelet
           filter banks to image processing. Technical Report, MIT, January 1996. Submitted to IEEE
           Tran. Image Processing.
[Sie86]    William M. Siebert. Circuits, Signals, and Systems. MIT Press and McGraw-Hill, Cam-
           bridge and New York, 1986.
[5L96]     M. Sablatash and J. H. Lodge. The design of filter banks with specified minimum stopband
           attenuation for wavelet packet-based multiple access communications. In Proceedings of
           18th Biennial Symposium on Communications, Queen's University, Kingston, ON, Canada,
           June 1996.
[SLB97]    Ivan W. Selesnick, Markus Lang, and C. Sidney Burrus. Magnitude squared design of
           recursive filters with the Chebyshev norm using a constrained rational Remez algorithm.
           IEEE Transactions on Signal Processing, to appear 1997.
[SMHH9司    O. V. Shentov, S. K. Mitra, U. Heute, and A. N. Hossen. Subband DFT - Part I: definition,
           interpretation and extensions. Signal Processing, 41:261-278, 1995.
[5N96[     Gilbert Strang and T. Nguyen. Wavelets and Filter Banks. Wellesley-Cambridge Press,
           Wellesley, MA, 1996.
[SOB96]    Ivan W. Selesnick, Jan E. Odegard, and C. Sidney Burrus. Nearly symmetric orthogo-
           nal wavelets with non-integer DC group delay. In Proceedings of the IEEE Digital Signal
           Processing Workshop, pages 431-434, Loen, Norway, September 2-4 1996.
[SP93]     Wim Sweldens and Robert Piessens. Calculation of the wavelet decomposition using quadra-
           ture 恥rmulae. In T끄n H. Koornwinder, editor, 仍／口velets: An 風eme肋27캄 T卜e口tment of
            Theory and Applications, pages 139-160, World Scientific, Singapore, 1993.
[SP96a]    A. Said and W. A. Pearlman. A new. fast, and efficient image codec based on set partitioning
           in hierarchical trees. IEEE Transactions Cir. Syst. Video Tech., 6(3):243-250, June 1996.
[SP96bj    A. Said and W. A. Penlman. An image muitii"esolut幻ii xepreseutation for lossless and lossy
           image compression. IEEE Transactions on Image Processing, 5:1303-1310, September 1996.
[SS94]     V. Strela and G. Strang. Finite element multiwavelets. In Proceedings of SPIE, Wavelet
           Applications in Signal and Image processing II, pages 202-213, San Diego, CA, July 1994.
[SS95]     G. Strang and V. Strela. Short wavelets and matrix dilation equations. IEEE Trans. SP,
           43(1):108-115, January 1995.
[Str86]    Gilbert Strang. Introduction to Applied Mathematics. Wellesley-Cambridge Press, Wellesley,
           MA, 1986.
[Str89]    Gilbert Strang. Wavelets and dilation equations: a brief introduction. SIAM Review,
           31(4):614-627, 1989. also, MIT Numerical Analysis Report 89-9, Aug. 1989.
[Str94]    Gilbert Strang. Wavelets. American Scientist, 82(3):250-255, May 1994.
[Str96a[   G. Strang. Eigenvalues of (1 2)H and convergence of the cascade algorithm. IEEE 升ans-
           actions on Signal Processing, 44, 1996.
[Str96b]   V. Strela. Multiwavelets: Theory and Applications. PhD thesis, Dept. of Mathematics, MIT,
           June 1996.
 242
                                                                                           Bibliography

 fSV93]     A. K. Soman and P. P. Vaidyanathan. On orthonormal wavelets and paraunitary filter
            banks. 招月E2午口nsact切ns on Sign毗 尸rocessing, 끄（3):117아1183, March 1993.
[SVN93I     A. K. Soman, P. P. Vaidyanathan, and T. Q. Nguyen. Linear phase paraunitary filter banks:
            theory, factorizations and designs. IEEE 升ansactions on Signal Processing, 41(12):3480-
            3496, December 1993.
[SW93]     Larry L. Schumaker and Glenn Webb, editors. Recent Advances in Wavelet Analysis. Aca-
           demic Press, San Diego, 193. Volume in the series: Wavelet Analysis and its Applications.
[SW97J     W. So and J. Wang. Estimating the support of a scaling vector. SIAM J. Matrix Anal.
           Appl., 18(1):66小73, January 1997.
[Swe95]    Wim Sweldens. The Lifting Scheme: A Construction of Second Generation Wavelets. Tech-
           nical Report TR-1995-6, Math Dept. University of South Carolina, May 1995.
[Swe96a1   Wim Sweldens. The lifting scheme: a custom-design construction of biorthogonal wavelets.
           A끄7冗扼d and Corr叩utation끄 且口7斗nonic An毗ysis, 3(2):186-200, 1996. Also a technical report,
           math dept. Univ. SC, April 1995.
[Swe96b1   Wim Sweldens. Wavelets: what next? Proceedings of the IEEE, 84(4):68아685, April 1996.
[Tas96]    Carl Taswe比 I／
                        口nd切毗 of Wavelet Tr口nsfor了ii Algor洸枷is. Birkh苞user, Boston, 1996.
[Tew97j    Ahmed H. Tewfik. Wavelets and Multiscale Signal Processing Techniques: Theo겡
                                                                                        and
           A까航c毗ions, to appear, 1997.
[The89]    The Ultra Wave Explorer User 's Manual. Aware, Inc., Cambridge, MA, July 1989.
［끄a96]     Jun 끄an. The 凡r口坑em（工tic口1T九eo겡 口nd A끄p1土c口tions of Bior坑ogon口1C叫加in W口velet
           Systems. PhD thesis, Rice University, February 1996.
[TM94a]    Hai Tao and R. .J. Moorhead. Lossless progressive transmission of scientific data using
           biorthogonal wavelet transform. In Proceedings of the IEEE Conference on Image Process-
           ing, Austin, ICIP-94, November 1994.
[TM94b]    Hai Tao and R. J. Moorhead. Progressive transmission of scientific data using biorthogonal
           wavelet transform. In Proceedings of the IEEE Conference on Visualization, Washington,
           October 1994.
[Tur86]    M. Turner. Texture discrimination by Gabor functions. Biological Cybernetics, 55:71-82,
           1986.
[TVC96]    M. J. Tsai, J. D. Villasenor, and F. Chen. Stack-run image coding. IEEE 升ans. Circ. and
           Syst. Video Tech., 519-521, October 1996.
[TW95}     Jun Tian and Raymond O. Wells, Jr. Vanishing Moments and Wavelet Approximation.
           Technical Report CML TR-9501, Computational Mathematics Lab, Rice University, Jan-
           uary 1995.
[TW96]     J. Tian and R. O. Wells. Image compression by reduction of indices of wavelet transform
           coefficients. Proc. DCC, April 1996.
[TWBOarJ   J. Tian, R. O. Wells, C. S. Burrus, and J. E. Odegard. Coifman wavelet systems:
                                                                                           approxima-
           tion, smoothness, and computational algorithms. In Jacques Periaux, editor, Computational
           Science for the 21st Centu八／, John Wiley and Sons, New York, 1997 to appear. in honor of
           Roland Glowinski's 60th birhtday.
[Uns96]    Michael Unser. Approximation power of biorthogonal wavelet expansions. IEEE Transac-
           tions on Signal Processing, 44(3):519-527, March 1996.
[VA96]     入4. J. Vrhel and A. Aldroubi. Pr芭寸iltering for 坑e 17硫挽毗切毗切n of 兀17工it卜凹a刃elet tr口n욕／orms.
           Technical Report, National Institutes of Health, 1996.
미B니OGRAPHY                                                                                         243


[Vai87a]    P. P. Vaidyanathan. Quadrature mirror filter banks, M-band extensions and perfect-
            reconstruction techniques. IEEE Acoustics, Speech, and Signal Processing Magazine, 4(3):4-
            20, July 1987.
{Vai87b]    P. P. Vaidyanathan. Theory and design of M-channel maximally decimated quadrature
            morror filters with arbitrary M, having perfect reconstruction properties. IEEE Transactions
             on Acoustics, Speech, and Signal Processing, 35(4):476-492, April 1987.
[Vai92]     P. P. Vaidyanathan. Mu娩rate Systems and Filter Banks. Prentice-Hall, Englewood Cliffs,
            NJ, 1992.
[VBL95I     J. D. Villasenor, B. Belzer, and J. Liao. Wavelet filter evaluation for image compression.
            IEEE T口nsactions on Image Processing, 4, August 1995.
{VD891      P. P. Vaidyanathan and Z. Doganata. The role of lossless systems in modern digital signal
            processing: A tutorial. IEEE Trans. on Education, 32(3):181-197, August 1989.
[VD951      P. P. Vaidyanathan and Igor Djokovic. Wavelet transforms. In Wai-Kai Chen, editor, The
            Circuits and Filters Handbook, chapter 6, pages 134-219, CRC Press and IEEE Press, Roca
            R砒on, 1995.
[Vet86]     Martin Vetterli. Filter banks allowing perfect reconstruction. Signal Processing, 10(3):219-
            244, April 1986.
[Vet87]     Martin Vetterli. A theory of multirate filter banks. IEEE 升ansactions on Acoustics, Speech,
            and Signal Processing, 35(3):356-372, March 1987.
[VG89]      Martin Vetterli and Didier Le Gall. Perfect reconstruction FIR filter banks: some prop-
            erties and factorizations. IEEE Transactions on Acoustics, Speech, and Signal Processing,
            37(7):1057-1071, July 1989.
[VH88]      P. P. Vaidyanathan and Phuong-Quan Hoang. Lattice structures for optimal design and r口
            bust implementation of tw아channel perfect reconstruction QMF banks. IEEE Transactions
            on Acoustics, Speech, and Signal Processing, 36(1):81-93, January 1988.
[VH92]      M. Vetterli and C. Herley. Wavelets and filter banks: theory and design. IEEE Transactions
            on Acou就ics, Speech, and Signal Processing, 2207-2232, September 1992.
 [VK95]     Martin Vetterli and Jelena Kovaevi6. Wavelets and Subband Coding. Prentic于HalF,出n-
            glewood Cliffs, 1995.                                                                "

 [VL89]      M. Vetterli and D. Le Gall. Perfect reconstruction FIR filter banks: some properties and
             factorizations. IEEE 7十口ns口ctions on Acotzs挽cs, 卵eech, and S四化口1 Pn兀essi?四， 37(7):1057小
             1071, July 1989.
 [VLU97]     M. J. Vrhel, C. Lee, and M. Unser. F戚 continuous wavelet transform: a least-squares
             formulation. Signal Processing, 57(2):103-120. March 1997.
 [VM88]      P. P. Vaidyanathan and S. K. Mitra. Polyphase networks, block digital filtering, LPTV
             systems, and alias-free QMF banks: a unified approach based on pseudocirculants. IEEE
             Transactions on Acoustics, Speech, and Signal Processing, 36:381-391, March 1988.
 {VNDS89]    p. p. Vaidyanathan, T. Q. Nguyen, Z. Doganata, and T. Saramki. Improved technique for
             design of perfect reconstruction FIR QMF banks with lossless polyphase matrices. IEEE
             끄끄nsactions on Acoustics, Speech, and Signal Processing, 37(7):1042-1056, July 1989.
 [Vol92]     Hans Volkmer. On the regularity of wavelets. IEEE Transactions on Information Theory,
             38(2):872-876, March 1992.
 [Wal9긔      Gilbert G. Walter, editor. W口velets 口nd O坑er Or坑ogon毗 帥／stems tt片th Applic口tion且 CRC
             Press, Boca Raton, FL, 1994.
244
                                                                                              텨비iography

[＼人／B95]    D. Wei and C. S. Burrus. Optimal soft-thresholding for wavelet transform coding. In Proceed-
            ings of IEEE International Conference on Image Processing, pages 1:610-613, Washington,
            DC, October 1995.
{WB96]      Dong Wei and Alan C. Bovik. On generalized coiflets: construction, near-symmetry, and
            optimization. IEEE 가ansactions on Circuits and Systems:II, submitted October 1996.
[WB97}      Dong Wei and Alan C. Bovik. Sampling approximation by generalized coiflets.             IEEE
            升ansactions on Signal Processing, submitted January 1997.
[Wei95]     Dong Wei. Investigation of Biorthogonal Wavelets. Technical Report ECE-696, Rice Uni-
            versity, April 1995.
[Wel93]     R. O. Wells, Jr. Parameterizing smooth compactly supported wavelets. Transactions of the
            American Mathematical Society, 338(2):919-931, 1993. Also Aware tech report AD891231,
            Dec. 1989.
[Wic92]     M. V. Wickerhauser. Acoustic signal compression with wavelet packets. In Charles K. Chui,
            editor, 14／口velets: A 끄itoi크口1 in T九eo四 口nd A7叩i끄ations, pages 679-700, Academic Press,
            Boca Raton, 1992. Volume 2 in the series: Wavelet Analysis and its Applications.
1＼人／ic9히    入41aden Victor ＼人／ickerhauser. Ad口까ed W凹elet An毗／sis from Theory to Softw口re. A K Pe-
            ters, Wellesley, MA, 1995.
[WNC87]     1. Witten, R. Neal, and J. Cleary. Arithmetic coding for data compression. Communications
            of the ACM, 30:520-540, June 1987.
[WO92a]     G. Wornell and A. V. Oppenheim. Estimation of fractal signals from noisy measurements
            using wavelets. IEEE Transactions on Acoustics, Speech, and Signal Processing, 40(3):611尸
            623, March 1992.
[WO92b]     G. W. Wornell and A. V. Oppenheim. Wavelet-based representations for a class of self-
            similar signals with application to fractal modulation. IEEE Transactions on Information
            Theory, 38(2):785-800, March 1992.
[WOG*95a} D. Wei, J. E. Odegard, H. Guo, M. Lang, and C. S. Burrus. SAR data compression
                                                                                            using
          best-adapted wavelet packet basis and hybrid subband coding. In Harold H. Szu, editor,
          Proceedings of SPIE Conference 2491. Wavelet Applications II, pages 1131-1141. Orlando.
          April 17卞21 1995.
[WOG*95b] D. Wei, J. E. Odegard, H. Guo, M. Lang, and C. S. Burrus. Simultaneous noise reduction
          and SAR image data compression using best wavelet packet basis. In Proceedings of IEEE
          International Conference on Image Processing, pages 111:200-203, Washington, DC, October
          1995.
[Wor96]     Gregory W. Wornell. Signal Processing with Fractals, A Wavelet- Based Approach. Prentice
            Hall, Upper Saddle River, NJ, 1996.
[WTWB97] Dong Wei, Jun Tian, Raymond O. Wells, Jr., and C. Sidney Burrus. A new class of
         biorthogonal wavelet systems for image transform coding. IEEE Transactions on Image
         Processing, to appear 1997.
[WWJ95]     J. Wu, K. M. Wong, and Q. Jin. Multiplexing based on wavelet packets. In Proceedings
                                                                                                 of
            SPIE Conference, Aerosense, Orlando, April 1995.
[WZ94]     Raymond O. Wells, Jr and Xiaodong Zhou. Wavelet interpolation and approximate solutions
           of elliptic partial differential equations. In R. Wilson and E. A. Tanner, editors, Noncompact
           Lie Groups, Kluwer, 1994. Also in Proceedings of NATO Advanced Research Workshop,
           1992, and CML Technical Report TR-9203, Rice University, 1992.
BIBLIOGRAPHY                                                                                     245

[XGHS96]   X.-G. Xia, J. S. Geronimo, D. P. Hardin, and B. W. Suter. Design of prefilters for discrete
           multiwavelet transforms. IEEE Trans. SP, 44(1):25-35, January 1996.
[XHRO95]   Z. Xiong, C. Herley, K. Ramchandran, and M. T. Orcgard. Space-frequency quantization for
           a space-varying wavelet packet image coder. Proc. m2t. Conf. Image Processing, 1:614卞617,
           October 1995.
[XS96]     X.-G. Xia and B. W. Suter. Vector-valued wavelets and vector filter banks. IEEE 升ans.
           SP, 44(3):508-518, March 1996.
[You80]    R. M. Young. An Introduction to Nonharinonic Fourier Series. Academic Press, New York,
           1980.
[You93}    R. K. Young. Wavelet Theory and Its Applications. Kluwer Academic Publishers, Boston,
           MA, 1993.
[ZT92a]    H. Zou and A. H. Tewfik. Design and parameterization ofm-band orthonormal wavelets. In
           Proceedings of the IEEE International Symposium on Circuits and Systems, pages 983-986,
           ISCAS-92, San Diego, 1992.
[ZT92bJ    H. Zou and A. H. Tewfik. Discrete orthogonal M-band wavelet decompositions. In Pro-
           ceedings of the IEEE International Conference on Acoustics, Speech, and Signal Processing,
           pages IV-605-608, San Francisco, CA, 1992.
                                Appendix A.
                             Derivations for
              Chapter 5 on Scaling Functions


                                                                                               in
This appendix contains outline proofs and derivations for the theorems and formulas given
                                                     be complete    or formal, but they should be
early part of Chapter 5. They are not intended to
sufficient to understand the ideas behind why a result is true and to give some insight into its
interpretation as well as to indicate assumptions and restrictions.

Proof 1 The conditions given by (5.10) and (7.7) can be derived by integrating both sides of

                                甲（끼 =＞그回 V而p(M x - n)                                       (12.1)


口nd m口king the change o/ 刃（11끄功les !/ == 人JT


                           fo(x)dx=二h(n)f1K『(Mx_n)dx                                        (12.2)


and noting the integral is independent of translation which gives


                                  =乞 h(n)而 J o(y)古 dy.                                      (12.3)
 With no further requirements other than p E L1 to allow the sum and integral interchange and
f (x) dx / 0, this gives (7. 7) as
                                                                                        (12.4)


 and for M = 2 gives (5.10). Note this does not assume orthogonality nor any specific normaliza-
 tion of p(t) and does not even assume M is an integer.


 This is the most basic necessary condition for the existence of 甲(t) and it has the fewest assump-
 tions or restrictions.

 246
Appendix A.                                                                                                247


Proof 2 The conditioi工s in (5.14) and (7.8) are （工 down-sam까ed or坑0卯n口胱！/ of ti끄nsh工tes by
M of the coefficients which results from the or仇ogonality of translates of the scaling function
g切en by


                                       J    o   (x)       o   (x   -    m)     dx   =   「5   (m)
                                                                                                          (12.5)

in (5.13). The basic sc口ling equ口tioi工 (12.1) is substitl虎ed for 切仇 加m渤ns in (12.5) gil冗ng



       / [Zh(n) Vi7,(Mx - )1 1二h(k) V而，(Mx - Mm - k)1 dx = ES(m)
          L n                              J L k                                                   J
                                                                                                          (12.6)


which, after reordering and a change of variable y = M x, gives


                   Z工坰九（k小(y -岫- Mm - k）小明m).
                    fl       I              -
                                                                                                          (12.7)


Us可ng 坑e or仇0卯n口旒！/ in (12.5) g切es our i毛Si工lt

                                       乞坰M小Mm) = d(m)                                                     (12.8)


in (5.14) and (7.8). This result requires the or仇ogonality condition (12.5), M must be an integer,
and any non-zero normalization E may be used.



Proof 3 (Corollary 2) The result that


                                  Zh(2미스그（2n + 1) = 1/ 亘                                                  (1且9)
                                   n                               fl



in (5.17) or, more generally


                                 ＞二小In) = Z小In砒尸 UV而                                                     (12.10)


is obtained by breaking (12.기 for M = 2 into the sum of the even and odd coefficients.


                     Z枷) =＞그(2k) +                                           h(2k + 1) = K。+ K1 = \／百.   (12.11)
                         n             k


Next we use (12.8) and sum over n to give


                                           三＞二h(k + 2미싸戶 1                                               (12.12)
                                            n         k
 248                                                                                                                         Derivations for Chapter on Scaling Functions

 which we then split into even and odd sums and reorder to give:


                       늬小回뼈『小k + 1+ 2n)h(2k + 1)1
                              71
                              n           L k                                                 大
                                                                                              k                                                J




               工目2k +可咽吃目2k + 1+ 2小k + 1)
                   k
                   丸           L n
                                 r1                             -J                            k        -L n
                                                                                                          7i                             J


                                   스二K洲刈 41m2k + 1) = 瑞 + 짜 = 1.                                                                                                      (12.13)
                                            丸                                 k

Solving (12.11) and (12.13) simultaneously gives K。= K1 = 1/ v互 and our result (5.17) or
(12.9) for M = 2.
   If the same approach is taken with (7. 7) and (7.8) for M = 3, we have

                   >＞미＝ZT帥나Z可鈿＋l) +Z蜘나2) =\／죵                                                                                                                         (12.14)
                          n                     n                                  fl                                    n

凹／zich, in tei吼1S of the partial sums K1, is

                                                ＞二x(n) = K0 + K1 + K2 = \／豆                                                                                           (12.15)

Using the or仇ogonality condition (12.8) as was done in (12.12) and (12.13) gives

                                                                    晞 + 耐 + 璲 = 1.                                                                                    (12.16)
Equation (12.15) and (12.16) are simultaneously true if and only if K0 = K1 = K2 = 1/ V죵.
This 끄rocess is 2兀zlid for any integer 凡J 口nd 口fly non-zero n（刃刃iali名口tion.

Proof 3 If the support of o(x) is [0, N - 1], from the basic recursion equation with support of
h(n) assumed as [N1, N2] we have

                                                                              N2

                                                    p(x) = ＞二 枷) '/ .'p伽. n)                                                                                     (12.17)
                                                                     n= /Vl


v脆ere 坑e su卯ort 0/ 坑e rig砒 /iand 毓de of (12.17) is 四厚, (N- 1 + N2)/2). Since 坑e su끄port
of both sides of (12.17) must be the same, the limits on the sum, or, the limits on the indices of
the non zero h(n) are such that N1 = 0 and N2 = N, therefore, the support of h(n) is [0, N
                                                                                             - 1J.
Proof 4 First define the autocorrelatiori function


                                                      a
                                                          (t)
                                                                     =        f
                                                                                  『     (x)
                                                                                              『   (x
                                                                                                          -    t)
                                                                                                                    dx
                                                                                                                                                               (12.
                                                                                                                                                                         18)
and the power spectrum


                    」（』
                                   ）小帥－
                                                                ""
                                                                '        心／
                                                                                              ／蛔小岫可                                     ""   』！
                                                                                                                                                              (12.19)
 Appendix A.                                                                                                                                  249

 which a乷er changing variables, y = x - t, and reordering operations gives


                             A(.) = f『(x)e '寸3dxfo(Y)e31dy                                                                                 (12.20)
                                                = 令 (w) 호(- w) = 陣（W）尸                                                                     (12.21)
If we look at (12.18) as being the inverse Fourier transform of (12.21) and sample a(t) at t = k,
we have
                                                                     1         f苡）

                                 "休）=2江少(w)I2 """ 面                                                                                        (12.22)



        굻쭈／
          ,'" 陣（w+21ri)J2&"如寸／
                             ,'"［旱蜘『2ir）小" 如                                                                                               (12.23)

but this integral is the form of an inverse discrete- time Fourier transform (DTFT) which means

                                Z毗）e" k= ＞二 陣（回+ 2兀Z）已                                                                                     (12.24)
                                                                                              f


1/ 坑e integer tr口ns／口tes of t巾） are or坑ogon口／,a（히 = d（시 口nd we have our resu虎

                                                ＞二陣（w+ 2而j)12 = 1.                                                                        (12.25)
                                                     f


i/ 坑e scaling funct切n is not nor刃1（工／
                                    初ed


                                쭈陣(w+ 27r
                                      『)f2= f1『(t)1' dt                                                                                   (12.26)

which is similar to Parseval's theorem relating the energy in the frequency domain to the energy
in the time domain.

Proof 6 Equation (5.20) states a very interesting property of the frequency response
                                                                                     of an FIR
filter w可th 坑e sc（工／
                   ing coe肛cien加 (Is／沇er coe刃iC可ents. This resu尻 口zn be der衣)ed in 坑e frequency
or time domain. We 凹ii/ 就ow 仇e frequency （加m口in 口rgument. T九e sc口／ing equ毗ion (12.1)
becomes (5.51) in the frequency domain. Taking the squared magnitude of both sides of a scaled
version of

                                                                                                                                          (12.27)
                                   .（
                                                『）
                                                             ＝
                                                                         弓2且
                                                                                        （w/
                                                                                                      2)
                                                                                                                   .       (w/
                                                                                                                                     2)
gives

                                  呻(2回）1' 亡 힛／1(w)i' 呻（口7)1'
                                            .            .       ,                  _         _   .        .   .       .   -     .    .




                                                                                                                                          (12.28)
                                                                               1.
Add kir to w and sum over k to give for the left side of (12.28)


                                 ＞二 陣（2w +2冗丸）12 = K =1                                                                                   (12.29)
                                        k
250                                                                                                                                                                           Derivations for Chapter on Scaling Functions



which is unity from (5.57). Summing the right side of (12.28) gives

                                                 r斗 l                                    .                       -            - .n - -                                    -        . .n
                                                乙2/ i佃＋k兀） ' 呻(w＋凡兀기 '                                                                                                                                             (12.30)
                                                     k

Break this sum into a sum of the even and odd indexed terms.

  （小 l 』甘＝.      - . , .., .-.                  - . . .4                           r1 l =1 .                                                           .4.                    』. . D 中 .           . 八.   ', . )   .       .
   乙押 (w＋打凡)(' 凹(w+ 2兀凡）i ' +2d L" （回＋ (2虎＋1）兀） ' 凹(w+ (2k+ I）兀） '                                                                                                                                                 (12.31)
      k                                                                                      k

               l e
                 1丑（w)I2＞二陣（w+ 2砒）1'出蜘珣 ' 二陣（w+ (2k + 1)ir)I2
                 乙
                 n
                                 k
                                                                                                 =



                                                                                                                                                                               k

which after using (12.29) gives

                                                                                                                                                                                                                   (12.32)
                                                 =                IH         (w)              I'     出如+                                                        ir) "          =     1

which gives (5.20). This requires both the scaling and or仇ogonal relations but no specific nor-
malization of 미t) . If viewed as an FIR filter, h(n) is called a quadrature mirror filter (QMF)
because of the symmetry of its frequency response about ir.

Proof 10 The multiresolution assumptions in Section 2 require the scaling function and wavelet
satisfy (5.1) and (2.24)

                甲(t) =Z小m呵가- n),                                                                                                            砂떠스그如V' (2t- n)                                                        (12.33)


and or坑0伽r刃iali却／ requires



and
                                                                  f                (t)        『            (t             -       k)             dt         =   d   (k)                                            (12.34)

                                                                       f砂                     (t)『                   (t       -             k)       dt = 0                                                        (12.   35)
for all k e Z. Substituting (12.33) into (12.35) gives


                     f三hi(n) ./2『(2t - n) 쭈h(『) /蜘(2t - 2k -『)dt = 0                                                                                                                                               (12.36)
Rearranging and making a change of variables gives


                                                                            !,乙 J                                                                                         2k-              dy= O                   (12.37)
                           :；二
                                                      h
                                     hi
                           y.             (n)               (t)                          [甲                (y尸                         n)        甲    (y-                             Z)
Using (12.34) gives
                                                 ＞二九：(ii) 九（Z) d(n H 2丸 - Z ) = 0                                                                                                                                  (12.38)
                                                     7l,f
Appendix A.                                                                                  251


加V 毗／ k E Z. S'工mi了iing over Z gives

                                            乞h1（小(n口劤＝0                                   (12.39)

Se工）（工r口ting (12.39) into even 口nd odd 可ndices 9切es

                  乞可刎川帥4向＋Zhi(2Z+ 1) 婢Z＋卜胱) = 0                                           (12.40)
                   m                                        Z

which must be true for 毗1 integer 瓦 Definir四／니미 = 九（2n), 尻（미 = h(2n+1) （工nd可미 = g(- n)
for any sequence g, this becomes

                                            he * hie + h。* h1。= 0.                        (12.41)

From 坑e or坑0肋까n琉ty of the tr口nslates of 甲 and , one c口n 毓milar匈 아,tain 仇e following:

                                             he 女 /1e + h。女 /1O == S.                     (12.42)

                                      hie * hie + h1。* h1。= S.                            (12.43)
This can be compactly represented as

                                                        [   싸
                                                            九 사
                                                              九
                                                                     l l       =1 d 91
                                                        尸                  m
                                                                e     e

                                                                    m
                                                                    九 싸
                                                                      九
                                                        1
                                                                                          (12.44)
                                                                                to oj "
                            fh.       /1.       ],
                           [hie       hiO]
                                                        1                  1
                                                                0     O
                                                                           ]
Assuming 仇e sequences 口1毛 /mnite leng坑 (12．杯) can be used to show that

                                      h 六 /11O - 凡 士 /11e = 士S七，                          (12.45)

where Sk（미 = 8(n 小 丸）. Indeed, t琉ing 仇e 二加71S如-in of (12.4.4) we get using 坑e not毗切n
of Ch口I冗er 8 H (z)H三（ze') = I. Bec口use, 坑e filters 口re FIR 瓦 （기 is a (工口urent) polynomi口1
m的-ix i脆坑 이岫脚mi毗 matri跏I刃erse. Ther毛／ore 坑e determlinant of H （기 is o/ 坑e for刃1‘士名k
for some integer k. This is equivalent to (12.45). Now, convolving both sides of (12.45) by h we
get

                          士／1e 士 S丸         =        [he女／11O寸凡女／11e］女／ie                 (12.46)

                                            = ［征*瓦* h1。－九ie *瓦* 뇨］
                                            = ［凡*瓦* 九l。+ h1。*瓦* 凡］
                                                     ［凡*瓦＋凡*瓦］士 /11o
                                            =        h1。
                                                       .

Similarly by convolving both sides of (12.45) by h。we get

                                                     干／1O士Sk = h1e.                       (12.47)

Combining (12.47) and (12.47) gives the result

                                  hi(n) = 士(- 1)nh(- n + 1 - 2k).                         (12.48)
252                                                           Derivations for Chapter on Scaling Functions


Proof 11 14노 就ow 坑e integr口lo/ 坑e i夙ivelet is zero by 可ntegr口ting 切坑 毓des of (12.33이 gives


                             f砂(t)dt= Zhi(n) f ../o(2t-n)dt                                      (12.49)


But 仇e integr口1 on 坑e rig砒 /1（工nd side is A0, usu끄包 no竹7끄工lized to one and from (5.17) or (12.9)
口nd (1名48) we 丸now 坑毗
                                          乞h1（미 = 0                                      (12.50)

and, 坑erefore, from (1乞49力 坑e integral of the 七口avelet is zero.
   The fact that multiplying in the time domain by (- 1)'l is equivalent to shifting in the frequency
domain by ir gives Hi佃) = H (w + ir).
                                                                                             Appendix B.
                                                                                           Derivat向ns 化r
                                                                                    Section on Properties


In this appendix we develop most of the results on scaling functions, wavelets and scaling and
wavelet coefficients presented in Section 5.8 and elsewhere. For convenience, we repeat (5.1),
(5.10), (5.13), and (5.15) here

                                                    甲(t) =2J h(n) \/2 ' (2t中 n)                                                                                              (12.51)
                                                                                         n




                                                                                         5노（미 =\／易                                                                           (12.52)
                                                                                          nd




                         J／甲        （t）
                                    (t)         甲    (t  （t－         -         丸）
                                                                               k)        dt
                                                                                         dt= E5                    (k)
                                                                                                                   （丸）            =
                                                                                                                                  =       {。
                                                                                                                                           ,                     it 'C = U
                                                                                                                                                                 。therwise   (12.   53)
If normalized
1f 1l0r1llahZed


                          j    ／甲   p     （t）
                                          (t)       甲
                                                    'p         (t-
                                                               （t.                  k)
                                                                                    k)   dt=             6
                                                                                                         d   (k)
                                                                                                             （丸）              =       {｛古            it /C = U
                                                                                                                                                     。therwise               (12.   54)
The results in this appendix refer to equations in the text written in bold face fonts.

Equation (5.45) is the normalization of (5.15) and part of the orthonormal conditions required
by (12.53) for k= 0 and E= 1.

Equation (5.53) If the 甲(x - k) are orthogonal, (12.53) states


                                                I                        (x+              m)   『   (x)                   dx           =   「d   (m)
                                                                                                                                                                             (12.55)

Summing both sides over m gives


                                                         Z, f『(x + m)o(x)dx = E                                                                                              (12.56)
                                                                                                                                                                                    253
254                                                                                               Derivations for Section on Properties


which after reordering is

                                        f (x)가아小＝丑                                                                            (12.57)

Using (5.50), (12.70), and (12.73) gives


                                            f   (x)       dxAo       =         !
but f o(x) dx = A0 from (12.68), therefore

                                                      Ag= E


   If the scaling function is not normalized to unity, one can show the more
(5.53). This is done by noting that a more general form of (5.50) is




if one does not normalize A0 = 1 in (12.69) through (12.73).

Equation (5.53) follows from summing (12.53) over m as


                                   二J『(x+ m)7(x)dx= f『(x)2dx
                                   In
                                                                                                                              (12.61)


which after reordering gives


                                           『『）dx小山：
                                   f (x）쭈『（：                                                                                  (12.62)


and using (12.60) gives (5.53).

Equation (5.46) is derived by applying the basic recursion equation to its own right hand side
to give
                        (0떠＝＞그(ri)＼厄> h(k) V' o(2（小미- k)                                                                      (12.63)
                                        n             k
which, with a change of variables of Z = 2n + k and reordering of operation, becomes



                            小斗加&                                 _   2n)           ]   2   (4t-
Applying this j times gives the result in (5.46). A similar result can be derived for the wavelet.
                                                                                                    e)   .
                                                                                                                              (12.64)




Equation (5.48) is derived by defining the sum
                                                                           Z
                                            AJ =) 中（솎 )                                                                       (12.65)
                                                                           刃
Appendix B.                                                                                   255


and using the basic recursive equation (12.51) to give
                                                                            미
                               小m＞小가(2多－  t        n
                                                                                           (12.66)


Interchanging the order of summation gives



                             A』＝而＞二』(n)｛쭈『（赤 n)}
but the summation over Z is independent of an integer shift so that using (12.52) and (12.65)
giv明


                       ／』＝扼扼＞二h(n)｛二7（赤）} =247-1·                                          (12.67)

This is the linear difference equation

                                               Aj 寸 2AJ_ 1 = 0                             (12.68)

which has as a solution the geometric sequence

                                                   AJ = A。2J.                              (12.69)

If the limit e虹sts, equation (12.65) divided by 2J is the Riemann sum whose limit is the definition
of the Riemann integral of w(x)

                                         I '       1)       /       . . -   .              . . m 나八．
                                無卄히＝尸回由＝A0.                                                (12.70)
It is stated in (5.57) and shown in (12.56) that if 97(x) is normalized, then A0 = 1 and (12.69)
becomes
                                            AJ = 2 '.                                    (12,.71)
which gives (5.48).

   Equation (12.70) shows another remarkable property of w(x) in that the bracketed term is
exactly equal to the integral, independent of J. No limit need be taken!

Equation(5.49) is the "partitioning of unity" by 9' (x). It follows from (5.48) by setting J = 0.

Equation (5.50) is generalization of (5.49) by noting that the sum in (5.48) is independent of
a shift of the form

                                         二甲（多－缶）=2"
                                           t
                                                                                           (12.72)
for any integers M 2 J and L. In the limit as M -羽，赤r can be made arbitrarily close to any
x, therefore, if (x) is continuous,

                                                   甲
                                                        Z
                                                                T
                                                                                           (12.73)
                                               Z
                                                        刃
                                               Z
256                                                                                                                                                     Derivations for Section on Properties


This gives (5.50) and becomes (5.49) for J = 0. Equation (5.50) is called a "partitioning of unity"
for obvious reasons.

   The first four relationships for the scaling function hold in a generalized form for the more
general defining equation (7.4). Only (5.48) is different. It becomes

                                                                t小
                                                                                                                                                                                    (12.74)
                                                                                   .                          ．




                                                                乙 叭而7) = A7 "
                                                                                           丸
                                                                  k

for M an integer. It may be possible to show that certain rational M are allowed.

Equations (5.51), (5.72), and (5.52) are the recursive relationship for the Fourier transform
of the scaling function and are obtained by simply taking the transform (5.2) of both sides of
(12.51) giving

                              .回工伽／V가似가3wt dt                                                                                                                                       (12.75)

which after the change of variables y = 2t - n becomes


                              令(w) 그，
                                    二
                                     b노（미 n (y）可jw(y+n)/2 dy
                                                                느；r                                  /
and using (5.3) gives

              . . i r小 . . ; .m /n r . . 二... /n -  1 __. . -
             中回＝而2少" ) """" " ' / 甲（9)" " " "" dy = 而川w尼）中（畔）

which is (5.51) and (5.72). Applying this recursively gives the infinite product (5.52) which holds
for any normalization.

Equation (5.57) states that the sum of the squares of samples of the Fourier transform of the
scaling function is one if the samples are uniform every 2ir. An alternative derivation to that in
Appendix A is shown here by taking the definition of the Fourier transform of 甲(x), sampling it
every 2irk points and multiplying it times its complex conjugate.


            (w+ 2k).(w+ 2k): f『（:)6-""'"'"' dxf (y)e""2")" dy                                                                                                                       (12.76)

Summing over k gives


               ＞二陣
                 （w+2砒）
                 k
                       12=n的耐-jw("바－j2irk(x-y)dxdy    k         V              M
                                                                                                                                                                                    (12.77)



                     / /甲 = ＞二6"
                              V       5-
                                                (x)         甲   (y)            e '     「        '.        '
                                                                                                                      k
                                                                                                                                  ' " '   小   ')        dx dy


                      / /『    =
                                  V        .5
                                                      (x)             『   (x       +       z)            e3       "       착
                                                                                                                              k
                                                                                                                                    " ""           dx    dz
Append汶 B.
                                                                                           257

but
                                    ＞二ej2"k' 스그仁그）                                      (12.78)
                                        k                           f
therefore

                        ＞二陣（w+ 2砒）12=/<(:)＞二甲(x +Z) e-" dx
                         k                            V                 f

which becomes

                                  쭈／        『
                                                （7）
                                                          『
                                                              （！
                                                                   『 『）     4:
                                                                                 e" "
                                                                                   '
                                                                                        (12.79)

Because of the orthogonality of integer translates of 99(x), this is not a function of w but is
5甲(x)12 dx which, if normalized, is unity as stated in (5.57). This is the frequency domain
equivalent of (5.13).

Equations (5.58) and (5.59) show how the scaling function determines the equation coeffi-
cients. This is derived by multiplying both sides of (12.51) by 甲(2x - m) and integrating to
give

                   f (x)『(2x- m)dx= f＞二h(n)7(2x- n)7(2x- m) dx
                             伉口可小如卜如·
Using the orthogonality condition (12.53) gives

                    r   . . .       .                 . . i
                   / 甲（.' 加(2‘小m) dx ＝九（.rn)＝흐／f ko(y)I2
                                                 . . .'       i . .
                                                         dy= 寸흐九（．
                                                                 叫
which gives (5.58). A similar argument gives (5.59).
                                                       Appendix C.
                                                   Matlab Programs


                                                     of them for any scientific purpose but please
You are free to use these programs or any derivative
                                                 programs and others can be found on our web
reference this book. Up-dated versions of these
page at: ht巾刀www-dsp.rice.ed바


function p = psa(h,kk)
                                                              tion
                   calculates samples of the scaling fu工lc




하凡 하凡 이凡 U凡 h凡
  p = psa (h,kk)
                                          ximat ions from the
   phi (t) = p by kk successive appro
                                             tion is a constant.
   scaling coefficients h. Initial itera
                                      tion.       csb 5/19/ 93
   phi_k (t) is plotted at each itera

if nargin==1, kk=11; end;                 % Default number of iterations
h2= h*2/ sum(h) ;                         'I. normalize h(n)
K = length(h2) 中1; S = 128;               h Sets sample density
                               );         7. Sets initial iteration
p = [ones (1, 3半S水K) ,O] /(3牢K
P = p  (1:K* S) ;                          'h Store for later plotting
axis ([ O K*S+2 -.5 1. 4] );
hu = upsam (h2,S) ;                       h upsample h(n) by S
 for iter = O:kk                          XSuccessive approx.
    p = d끄sa皿F江e (conv (hu , p力 ;         % convolve a끄d do日n- sa皿ple
       plot (p) ; pause;                  0/, plot each iteration
    h   P = [P;p(1:K*S) ];                   7. store each iter. for plotting
    end
                                          % only the supported part
    p = p (1: K*S) ;
    L = length(p) ;
    x = ( [l :L] )/(S) ;
    axis ([ 0 3 寸. 5 1. 4] );
       plot (x,p) ;                      % Final plot
       title ( 'Scaling Function by Successive Approx. ') ;
       ylabel( 'Scaling Function') ;
       xlabel ( 'x ') ;


            258
Appendix C.                                                                       259


function p = pdyad(h,kk)




U凡 하凡 町凡 하凡 하凡
  p = pdyad(h,kk) calculates approx. (L-1) *2' (kk+2) samples of the
   scaling function phi (t) = p by kk+3 dyadic expansions
   from the scaling coefficient vector h where L=length(h) .
   Also plots phi_k (t)  at each iteration.     csb 5/19/93

if nargin==1, kk = 8; end                      2; Default iterations
h2 = h*2/ sum(h) ;                             % Normalize
N = length(h2) ; hr = h2 (N: -1:1) ; hh = h2;
axis ([ O,N-1, -.5, 1. 4] ) ;
MR = [hr, zeros (1,2*N-2) ] ;                 % Generater row for MO
MT = MR; MO = 口;
for k = 1:N-1                                 艾 Generate convolution and
    MR = [0, 0, MR (1: 3*N- 4) ];             '/    do日nsample matrix from h(n)
    MT = [MT; MR] ;
end
MO = MT(: ,N: 2*N-1) ;                         % MO*p = p if p samples of phi
MI = MO - eye (N) ;
Mi = tMI(1:N-1, :);ones (1,N) ];
pp = MJ\ [zeros (N-1,1) ;1J;                   'h Samples of phi at integers
p =    pp(2:length(pp)    -1) . ' ;
     x = [O:length(p) +1] *(N-1) /(length(p) +1) ; plot (x, [O,p,OJ) ; pause
p = conv (h2,p) ;                             % value on half integers
    x = [O: length(p) +1] *(N-1) /(length(p) +1) ; plot (x, [O,p,OJ) ; pause
y = conv (h2,dnsa皿ple (p) );                  'I. convolve and downsample
p = merge (y,p) ;                             '/ interleave values on Z and Z/2
    x = [O: length(p) +1J* (N-1) /(length(p)+1) ; plot (x, [O,p,OJ) ; pause
for k = 1:kk
    hh = upsample (hh) ;                      '/ upsample coefficients
    y = conv (hh, y) ;                        % calculate intermediate terms
    p = merge (y,p) ;                         % insert new terms between old
    x = [O:length(p) +1] 水 (N-1) /(length(p) +1) ; plot (x, [O,p,OD; pause;
end
title ( 'Scaling Function by Dyadic Expa工lsion ') ;
ylabel ( 'Scaling Function') ;
xlabel( 'x ') ;
axis;
260                                                                                                    Matlab Programs



      fu工lction [hf, ht] = pf (h,kk)




      V加 町凡 町凡 町凡 아凡
         thf, ht] = pf (h,kk) computes and plots hf, the Fourier transform
          of the scaling function phi(t)         using the freq domain
          infinite product formulation with kk iterations from the scaling
          function coefficients h. Also calculates and plots ht = phi(t)
          using the inverse FFT                     csb 5/19/93
      if nargin==1, kk=8; end               'fl Default iterations
      L = 才12; P = L;                       % Sets nu皿ber of sample points
      hp = fft (h,L) ; hf = hp;             'h Initializes iteration
      plot (abs (hf) ) ;pause;              h Plots first iteration
      for k = 1:kk                          h Iterations
        hp= [hp(1: 2:L) , hp (1: 2:L) ] ;   h Sample
        hf = hf．杜叩／sqrt (2) ;               % Product
        plot (abs (hf (1:P/2) )) ;pause;    h Plot Phi (omega) each iteration
            P=P/ 2;                         'I. Scales axis for plot
      end;
      ht = real (ifft (hf) );               'h phi (t) from inverse FFT
      ht = ht (1:8木2八kk) ; plot (ht (1: 6水2八kk) ) ;    h Plot phi(t)



      function hn = daub (N2)




       하凡 U凡 Vm 町凡 하凡 아凡 h凡 叫凡 Vm 가凡 町凡
         hn = daub (N2)
         Function to compute the Daubechies scaling coefficients from
         her development in the paper, "Orthonormal bases of compactly
         supported wavelets ", CPAM, Nov. 1988 page 977, or in her book
         "Ten Lectures on Wavelets ", SIAM, 1992 pages 168, 216.
         The polynomial R in the reference is set to zero and the
         minimum phase factorization is used.
         Not accruate for N > 20. Check results for long h(n) .
           Input:     N2 = N/ 2, where N is the length of the filter.
           Output: hn = h(n) length-N mmn phase scaling fn coefficients
         by rag 10/10/88, csb 3/ 23/93
           a
         =1;     p= l;       q= 1;      % Initialization   of variables
      hn = [1 1] ;                      'h Initialize  factors of zeros at -1
      for j = 1:N2-1,



                                          m aPq
               conv (hn, [1,1] );       'I, Generate polynomial for zeros at -1
               -a*0. 25* (j+N2-1) /j;   'h Generate the binomial coeff. of L
               conv (p, [1, -2,1] );    'I, Generate variable values for L
               [0 q 0] + a*p;           % Combine terms for L
      end;


                               q뇨 m
                                            sort (roots (q) );                    % Factor L
                                            conv (hn,real (poly (q(1:N2-1) )));   'h Combine zeros at -1 and L
                                            hn*sqrt (2) /(sum(hn) );              'I, Normalize
Append汶 C.                                                                                  261


function h = h246 (a,b)
Y h = h246 (a,b) generates orthogonal scaling fu끄ction


U凡 하凡 n凡
    coefficients h(n) for lengths 2 , 4, 카ld 6 using
   R.esnikoff 's parameterization with angles a and b.
    csb. 4/4/93
if a==b, h = [1,i] /sqrt (2) ;                 'h Length-2
elseif b==0
   hO = (i - cos (a) + sin(a) )/2;             'I. Length-4
   hi = (i + cos (a) + sin(a) )/2;
   h2 = (i + cos (a) - sin(a) )/2;
   h3 = (i - cos (a) - sin(a) )/2;
   h = [ho hi h2 h3J/sqrt (2) ;
else                                           'h Length-6
   hO = ( (1+cos (a)+sin(a) )*(i- cos (b) -sin (b) )+2*sin(b) *cos (a) )/4;
   hi = ( (i- cos (a)+sin(a) )*(i+ cos (b) -sin (b) )-2*sin(b) *cos (a) )/4;
   h2 = (1+cos (a牛b) +sin(a-b) )/2;
   h3 = (1+cos (a-b) -sin(a-b) )/2;
   h4 = (1-hO-h2) ;
   h5 = (1-hi- h3) ;
   h = [ho hi h2 h3 h4 h5] /sqrt (2) ;
end



fu乂tion [a,b] = ab(h)




아九 아凡 打凡 h凡
  [a,b] = ab (h) calculates the parameters a 카ld b from the
   scaling function coefficient vector h for orthogonal
   systems of length 2, 4, or 6 only.      csb. 5/i9/ 93.

h
  = h*2/ sum(h) ; x=O;                                % normalization
if length(h) ==2, h = [0 0 h 0 0] ; x=2; end;
if length(h) ==4, h = [0 h 0] ; x=4; end;
a = atan2 ( (2* (h(i) 八2+h(2Y2-i) +h(3) +h(4) ),(2*h(2) *(h(3) -1) -2*h(1) *(h(4) -1) ));
b = a - atan2 ( (h(3) -h(4) ),(h (3) +h(4) -i) );
if x==2, a = i; b = 1; end;
if x==4, b = 0; end;



function y = ups리nple (x)
0/, y = upsample (x) inserts zeros between each term in the row vector x.
'I. for example:       [1 0 2 0 3 0] = upsa皿ple ([ 1 2 3] ). csb 3/1/93.
L = length(x) ;
y (: ) = [x; zeros (i, L) ]; y = y. ';
y = y (i: 2*L-i) ;
262                                                                      Matlab Programs


      function y = upsa皿住眉）
      0/, y = upsam(x,S) inserts S-i zeros between each term in the row vector x.
      'h for example:       [1 0 2 0 3 0] = upsample ([ 1 2 3] ). csb 3/1/93.
      L = length(x) ;
      y (: ) = [x; zeros (S-1,L) ]; y = y. ' ;
      y = y (i: S*L-1) ;




      function y = dnsainple (x)

      가凡 h凡
        y = 由sample (x) samples x by removing the even terms in x.
         for example:    [1 3] = dnsample ([ 1 2 3 4] ). csb 3/1/93.
      =
      L
        = length（幼 ;
      V
      V
        = x (1: 2:L) ;




      function z = merge (x,y)
       /。 z = merge (x, y) interleaves the two vectors x and y.
      'h Example [1 2 3 4 5] = merge ([ 1 3 5] ,[2 4] ).
      h csb 3/1/93.
      X
      z = Ix; y,0] ;
      z 口 z (: ) ;
      z = z (1:length(z) -1) . ' ;




      function w = wave (p,h)




      이凡 하凡 h凡 이凡 이凡
        w = wave (p,h)   calculates and plots the wavelet psi(t)
         from the scaling function p and the scaling function
         coefficient vector h.
         It uses the definition of the wavelet. csb. 5/19/93.

      h2 = h*2/ sum(h) ;
      NN = length(h2) ; LL = length(p) ; K}( = rou工ld( (LL) /(NN-1) );
      hlu = upsam(h2 (NN: -1:1) .牛cos (pi* [0:NN小1] ) ,KK) ;
      w = 由lsample (conv (hlu,p) ); w = 日（1 : LL) ;
      xx = [O:LL-1] *(NN-1) /(LL-1) ;
      axis ([ 1 2 3 4] ); axis;
      plot (xx,w) ;
Appen비x C.
                                                                                          263


function g = dwt (f, h,NJ)
% function g = dwt (f, h,NJ) ; Calculates the DWT of periodic g
h with scaling filter      h and NJ scales.      rag & csb 3/17/94.
oh
N = length (h) ; L = length(f) ;
c
   =   f;   t = [];
if nargin==2, NJ = round(logiO (L) /loglO (2) ); end; % Number of scales
hO = fliplr (h) ;                             % Scaling filter
hi   =  h;   hi (1: 2:N) = -hi (1: 2:N) ;     h Wavelet filter
for j     = 1:NJ                              'I. Mallat 's algorithm
             L = length(c) ;
             c = [c (mod( (- (N-1) :-1) ,L)+i) c] ;          7. Make periodic
             d = conv (c,hl) ;    d = d(N: 2: (N+L-2) );     h Convolve 也 于sa叩le
             c = conv (c,hO) ;     C = c (N: 2: (N+L-2) );   7. Convolve 也 于sample
             t
                 =   [d,t] ;                                 % Concatenate wiet coeffs.
     end;
                                                             % The DWT
     g = [c, t] ;


     function f = idwt (g,h,NJ)
     I. function f = idwt (g,h,NJ) ; Calculates the IDWT of periodic g


       凡 L
     凡 기
                                                      rag & csb 3/17/94.

     n
         with scaling filter   h and NJ scales.


        = length(g) ;       N = length(h) ;
     if nargin==2   ,   NJ  = rou끄d(logiO (L) /loglO (2) ); end; h Number of scales
     hO = h;                                                  弦 Scaling filter
     hi = fliplr   (h)  ;   hl (2:   2:N)    =  -hi(2: 2:N) ; on Wavelet filter
     UJ = L/ (2八NJ)   ;                                       %  Number of SF coeffs.
     c = g (1:  LJ) ;                                         艾  Scaling coeffs.
     for j = 1:NJ                                             h  Mallat 's algorithm
         w = mod(O:N/      2-1,LJ)+i;                         %  Make  periodic
         d = g(LJ+1: 2*LJ) ;                                  oh
                                                                 Wavelet coeffs.
         cu(1: 2: 2*LJ+N)    =   [c   c (i,  w) ];            玄  Up- s키nple 也 periodic
         du(i: 2: 2*LJ+N)    =   [d   d(i,   w) ];            oh
                                                                 Up- sample & periodic
         c   = conv (cu,hO)      +   conv   (du,hi) ;          on
                                                                 Convolve  & combine
         c   = c (N:N+2*UJ-    i)  ;                          oh
                                                                 Periodic  part
         UJ = 2*LJ ;
      end;
      f = C;                                                  % The inverse DWT



     function r = mod(m,n)
     %r = mod(m,n) calculates r = in modulo n
       加
       i
       h

       r
             = in - n*floor (m/n) ;                                h Matrix modulo n
264                                                                        Matlab Programs


      function g = dwt5 (f, h,NJ)
      兀 function g = dwt5 (f, h,NJ)
      V. Program to calculate the DWT from the L samples of f (t) in
      'I. the vector f using the scaling filter h(n) .


       凡 하
       H 凡 N
           csb 3/ 20/94

        = length(h) ;
      C = f;    t = 口;
      if nargin==2
          NJ = rou끄d(loglo (L) /logio (2) );            h N山nber of scales
      end;
      hi = h; hl (1: 2:N) = -hl (i: 2:N) ;              X Wavelet filter
      hO = fliplr (h) ;                                h Scaling filter
      for j = i: NJ                                    'I. Mallat 's algorithm
          L = length(c) ;
          d = conv (c,hi) ;                            % Convolve
          c = conv (c,ho) ;                            % Convolve
         Lc = length(c) ;
          while Lc > 2*L                              工 卜｛ulti- wrap?
            d = [(d(1:L) + d(L+1: 2*L) ), d(2*L+1:Lc) ]; V. Wrap output
            c = [(c (1:L) + c (L+1: 2*L) ), c (2*L+1: Lc) ]; % Wrap output
            Lc = length(c) ;
         end
         d = [(d(1:N-i) + d(L+1:Lc) ), d(N:L) ];      % Wrap output
         d = d(1: 2:L) ;                              'I. Down-sample wiets coeffs.
            = [(c (1:N-1) + c (L+1:Lc) ), c (N:L) ];
               C
                                                      'I. Wrap output
                   C t
              c (i: 2:L) ;                            h Do日n-sample scaling fn c.
              [d,t] ;                                 X Concatenate wiet coeffs.
      end                                            % Finish wavelet part
      g = [c,t) ;                                    % Add scaling fn coeff.
Appendix C.                                                                 265


function a = choose (n,k)
Xa = choose (n,k)
'h BINOMIAL COEFFICIENTS
工 allowable inputs:




U凡 V加 U九 V
         m
   n : integer, k : integer
   n : integer vector, k : integer
   n : integer, k : integer vector
   n : integer vector, k : integer vector (of equal dimension)
nv = 1l ;
kv 누 k;
if (length(nv) == 1) & (length(kv) > 1)
nv = nv 水 ones (size (kv) );
elseif (length(nv) > 1) & (length(kv) == 1)
kv = kv * ones (size (nv) );
end
a = fly;
for i = 1:length(nv)
    n = nv (i) ;
    k = kv(i) ;
    if n >= 0
       if k >= 0
           if n>=   k
               c = prod(1. :n) /(prod(1:k) *prod(1:n-k) );
           else
               c = 0;
           end
      else
          c = 0;
      end
    e上se
       if k >= 0
           c = (-1) Ak * prod(1:k-n-1) /(prod(1:k)字prod(1: -n-1) );

          if n >= k
             c = (-1Y (n-k) 却rod(1: -k-1) /(prod(1:n-k) 卞prod(1: -n-1) );
          else
             C = U;
          end
       end
   end
   a(i) = C;
end
                                                                    Index


adaptive basis, 133, 138                DWT, 7, 16, 207
approximate FFT, 204                       calculation of, 195-202
                                           definition, 7
bas通 42                                     discrete-time, 8, 41
     adaptive, 133, 138                     filter bank, implementation of, 34
     biorthogonal, 43                       filterbank implementation of, 198
     orthogonal, 42                         Mailat's algorithm, 34
     unconditional, 49                      nondecimated, 136, 214
biomedical signal processing, 225           numerical complexity of, 41, 198
biorthogonal wavelets, 119                  periodic, 40
     Cohen-Daubechies-Feauveau family       redundant, 136, 214
           of, 122                          shift-invariant, 136, 214
    （兀沮ets, 124                         dyadic expansion, 71
     lifting, 124
                                        entropy coding, 222
cascade algorithm, 69
                                        filter bank, 4, 32, 154
Coifiets, 91, 99
                                              analysis, 34
     biorthogonal, 124
                                              nondecimated, 136
     generalized, 96
                                              synthesis, 37
     orthogon叫 99
                                        First generation wavelets, 3
communications, 225
                                        Fourier transforms, 52
compression, 220
                                        fractals, 225
continuous wavelet transform, 8, 150
                                        frame, 46, 133
cover of book, 6
                                              adaptive construction of, 138
                                              tight, 46
Daubechies' wavelets, 83
     coe珏Ic油比s, 81                       geophysical signal processing, 225
     design 砥 79
decimate, 33                             Haar wavelets, 5, 26, 60
denoising, 212                           hard thresholding, 213
digital filter, 33                       Holder regularity, 86
dilation equation, 13
discrete wavelet tr帥sform, see DWT       image processing, 225
Donoho's methods, 212                    inner product, 10
down-sample, 33                          iterating the filter bank, 71

 266
 INDEX                                                                                  267

 lattice, 39                             samples of signal, 90
 lifting, 39                             scaling, 3
       biorthogonal wavelets, 124        scaling coefficients, 51
 localization, 3                              necessary conditions of, 54-56
                                              parameterization of, 66-68
M-band wavelets, 106                          sufficient conditions of, 57-60
     design of, 112-113                  scaling filter, 13, see scaling coefficients
     MRA for, 106                             discrete moments of, 77
     properties of, 106-112                   regularity of, 77
Mallat's algorithm, 34                   scaling function, 10, 11, 51
medical signal processing, 225
                                              calculation of, 69-75
Modulated Filter Banks, 171
                                              coe표ic扼nts, 13
moments, 76
                                              moments of, 77, 112
     scaling function, 89
                                              properties of, 64-66
     vanishing, 78                      scaling vector, 13
MRA, 3, 10, 12, 39
                                        seismic signal processing, 225
     continuous, 10
                                        shift-invari쾨at wavelet transform, 136
     discrete, 149
                                        signal recovery, 212
     equation, 13
                                        signal spaces, 10, 51
     for M-band wavelets, 106
                                        sinc, 45, 48, 61
     properties, 227
                                        smoothness, 86
multiresolution analysis, see MRA
                                        Sobolev regularity, 87
multiwavelets, 127
                                        soft thresholding, 213
necessary conditions, 54                software, wavelet, 225
                                        spectral factorization, 80
     frequency domain, 55
nonlinear processing, 212               spline, 13, 62
norm, 10                                statistical estimation, 217
normalization, 60                       successive approximation, 69
                                             frequency domain, 71
orthogonal, 65                          su服c扼nt conditions, 57
overcomplete representation, 133, 134   summary, 227
overview, 227
                                        thresholding, 212
packets, 114                            tiling the time-frequency plane, 101
     adaptive wavelets, 115             time-frequency, 39
Parseval's theorem, 17, 46              transition matrix, 53
partial differential equations, 225     translation, 3
perfect reconstruction, 157             transmultiplexer, 156
polyphase, 159
                                        variation, 87
redundant transforms, 133, 134
refinement equation, 13                 Waish-Haddamar decomposition, 115
refinement matrix, 53                   wave, 1
regularity, 76                          wavelet, 1, 13, 59
                                            adaptive, 115
sampled signal as input, 38                 calculation 砥 69中75
268                                    Index



         design, 76
         expansion, 2
         First generation, 3
          function, 13
          moments of, 77
         mother, 3
         multiwavelets, 127, 131
         packets, 114
         properties of, 64-66
          signal processing, 203
          software, 225
          system, 2
          vector valued, 131
          what is a, 2
      wavelet systems, types of, 229
