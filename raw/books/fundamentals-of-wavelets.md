---
source_url: /run/media/yutae/Data/Fundamentals_of_Wavelets.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 176eb482f1e937b4afefac339fae16d43ef74f3f35afdf9214706b0616967acb
---
# Fundamentals of Wavelets: Theory, Algorithms, and Applications (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출 (~902,200 chars). 일부 토큰은 인식 오류로 깨짐 (한/영 혼용 OCR 산출). 원문 PDF(`books/Fundamentals_of_Wavelets.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Fundamentals of Wavelets: Theory, Algorithms, and Applications
- authors: Jaideva C. Goswami, Andrew K. Chan (Texas A&M University)
- edition: 1st
- year: 1999
- publisher: John Wiley & Sons, Inc. (A Wiley-Interscience Publication)
- pages: 324 (pdfinfo)
- isbn: 0-471-19748-3 (cloth)
- series: Wiley series in microwave and optical engineering
+ source file: `Fundamentals_of_Wavelets.pdf` (sha256: `176eb482f1e937b4…`)
+ extract: `pdftotext -layout` @ 2026-10-25, 902,200 chars

## Chapter structure (from TOC)
| # | topic | page |
|---|-------|------|
| 1 | What This Book Is About | 1 |
| 2 | Mathematical Preliminaries — linear spaces, bases, z-transform | 5 |
| 3 | Fourier Analysis — series/transform, DFT, Gibbs | 31 |
| 4 | Time-Frequency Analysis — STFT/Gabor, CWT, DWT, Wigner-Ville, ambiguity | 57 |
| 5 | Multiresolution Analysis — MRA, two-scale relations, splines | 89 |
| 6 | Construction of Wavelets — Shannon/Meyer/Battle-Lemarie/Daubechies, biorthogonal | 108 |
| 7 | DWT & Filter Bank Algorithms — decimation, PR bank, polyphase | 141 |
| 8 | Fast Integral Transform & Applications (crack detection etc.) | 187 |
| 9 | Digital Signal Processing Applications — wavelet packets, thresholding | 210 |
| 10+ | Remaining DSP/image applications through boundary-value problems | ~225-324 |

## Original text (all 325 pages)

Fundamentals
of Wavelets
Fundamentals
of Wavelets
Theory, Algorithms, and Applications



JAIDEVA C. GOSWAMI
ANDREW K. CHAN
了exas A&M Un加ersity




因
A ＼八기LE＼니NTERSC炬NCE PUBLICATI(：가시
JOHN W仕EY & SONS, It니C.
New York / Chichester / Weiriheim / Brisbane / Singapore / Toronto
 This book is printed on acid-free paper. @

Copyright （르） 1999 by John Wiley & Sons, Inc. All rights reserved.

Published simultaneously in Canada.

No part of this publication may be repr에uced, stored in a retrieval system or
transmitted in 打ly form or by any means, elec打onic, mechanical,
ph아oc아）ying, recor小ng, sc띠lning or 야herwi配，except as perm血ed under
Sections 107 or 108 of the 1976 United States Copyright Act, without either
the pr奴 written 꺄naission of the Publisher, or a毗1O1初ation through pay毗nt
of the appropriate per-copy fee to the Copyright Clearance Center, 222
Rosewood Drive, Danvers, 入A 01923, (978) 750-8400, fax (978) 750-4744.
Requests to the Publisher for permission should be ad血essed to the
Pennissions Dep可tment, John Wiley & Sons, Inc., 605 Third Avenue, New
York, NY 10158-0012, (212) 850-6011, fax (212) 850-6008. E-Mail:
PERM之EQ@WILEY.COM.

L功rary of Congress Cata切g加乎如枷bikat加n Data:
Goswami, Jaideva C.
    Fund게mentals of wavelets : theory, algorithms, and applications /
 Jaideva C. Goswasni, Andrew K. Chan.
       p. cm. - (Wiley series in microwave and optical engineering)
    Includes index.
    ISBN 0-471-19748-3 (cloth)
    1. Signal processing-Mathematics. 2. Wavelets (Mathematics)
 3. Image processing-Mathematics. 4. Electromagnetic waves-
 Scattering-Mathematical models. 5. Boundary value problems.
 I. Chan, Andrew K. II. Title. LII. Series.
 TK5102.9.G67 1999
 6213'01'5 152433-dc21                                      98-26348
Printed in the United States of America

10 9 8 7 6 5 4 3 2
                              To

         Shrimati Sati and Shri Chandra Nath Goswami
                                 -Jaideva C. Goswami

My Lord Jesus Christ from whom / received wisdom and knowledge
                              and
      my wife Sophia, for her support and encouragement
                                -Andrew K. Chan
Contents


Preface                                                            xv

 1   What This Book Is About                                         1

2    Mathematical Preliminaries                                     5
     2.1 Linear Spaces                                              5
      2.2 Vectors and Vector Spaces                                 7
     2.3 Basis Functions                                            9
           2.3.1 Orthogonality and Biorthogonality                 10
     2.4 Local Basis and Riesz Basis                               13
     2.5 Discrete Linear Normed Space                              15
     2.6 Approximation by Orthogonal Projection                    16
     2.7 Matrix Algebra and Linear Transformation                  18
           2.7.1 Elements of Matrix Algebra                        18
           2.7.2 Eigenmatrix                                       19
           2.7.3 Linear Transformation                             20
          2.7.4 Change of Basis                                    21
          2.7.5 Hermitian Matrix, Unitary Matrix, and Orthogonal
                Transformation                                     22
     2.8 Digital Signals                                           23
          2.8.1 Sampling of Signal                                 23
          2.8.2 Linear Shift-Invariant Systems                     24
          2.8.3 Convolution                                        24

                                                                   vi'
viii     CONTENTS

              2.8.4 于Transform                                           25
              2.8.5 Region of Convergence                                26
              2.8.6 Inverse z-Transform                                  28
        2.9 Exercises                                                    29
            References                                                   30

 3     Fourier Analysis                                                  31

        3.1 Fourier Series                                               31
        3.2 Examples                                                     32
              3.2.1 Rectified Sine Wave                                  32
              3.2.2 Comb Function and the Fourier Series Kernel KN (t)   33
        3.3 Fourier Transform                                            35
        3.4 Properties of the Fourier Transform                          37
              3.4.1 Linearity                                            37
              3.4.2 Time Shifting and Time Scaling                       38
              3.4.3 Frequency Shifting and Frequency Scaling             38
             3.4.4 Moments                                               38
              3.4.5 Convolution                                          39
             3.4.6 Parseval's Theorem                                    40
        3.5 Examples of the Fourier Transform                            40
             3.5.1 Rectangular Pulse                                     41
             3.5.2 Triangular Pulse                                      41
             3.5.3 Gaussian Function                                     42
        3.6 Poisson's Sum                                                43
             3.6.1 Partition of Unity                                    45
        3.7 Sampling Theorem                                             46
        3.8 P缸tial Sum and the Gibbs Phenomenon                          49
        3.9 Fourier Analysis of Discrete-Time Signals                    50
             3.9.1 Discrete Fourier Basis and Discrete Fourier Series    50
             3.9.2 Discrete-Time Fourier Transform                       52
       3.10 Discrete Fourier Transform                                   54
       3.11 Exercises                                                    55
           References                                                    56
                                                             CONTENTS    ix

4   기me-Frequency Analysis                                              57
      4.1 Window Function                                               58
      4.2 Short-Time Fourier Transform                                  60
           4.2.1 Inversion Formula                                      61
           4.2.2 Gabor Transform                                        61
           4.2.3 Time-Frequency Window                                  62
           4.2.4 Properties of ST丁                                      62
     4.3 Discrete Short-Time Fourier Transform                          64
           4.3.1 Examples of ST丁                                        64
     4.4 Discrete Gabor Representation                                  65
     4.5 Continuous Wavelet Transform                                   67
           4.5.1 Inverse Wavelet Transform                              69
           4.5.2 Time-Frequency Window                                  70
     4.6 Discrete Wavelet Transform                                     72
     4.7 Wavelet Series                                                 73
     4.8 Interpretations of the Time-Frequency Plot                     74
     4.9 Wigner-Ville Distribution                                      76
    4.10 Properties of the Wigner-Ville Distribution                    80
         4.10.1 A Real Quantity                                         80
         4.10.2 Marginal Properties                                     80
         4.10.3 Correlation Function                                    81
    4.11 Quadratic Superposition Principle                              81
    4.12 Ambiguity Function                                             83
    4.13 Exercises                                                      84
    4.14 Computer Programs                                              85
         4.14.1 Short-Time Fourier Transform                            85
         4.14.2 Wigner-Ville Distribution                               86
         References                                                     88

5   Mu川resolution Analysis                                              89
     5.1 Multiresolution Spaces                                         89
     5.2 Orthogonal, Biorthogonal, and Semiorthogonal Decomposition     92
     5.3 Two-Scale Relations                                            96
     5.4 Decomposition Relation                                         97
x       CONTENTS

         5.5 Spline Functions                                   98
              5.5.1 Properties of Splines                       102

         5.6 Mapping a Function into MRA Space                  103

         5.7 Exercises                                          104

         5.8 Con叩U妃샤如酊anis                                      106
              5.8.1 B-Splines                                   106

             References                                         107


    6   Construction of Wavelets                                108

         6.1 Necessary Ingredients for Wavelet Construction     109
              6.1.1 Relationship Between Two-Scale Sequences    109
              6.1.2 Relationship Between Reconstruction and
                    Decomposition Sequences                     110

         6.2 Cons甘uction of Semiorthogonal Spline Wavelets      112
              6.2.1 Expression for {go[k]}                      113

         6.3 Construction of Orthonormal Wavelets               114

         6.4 Orthonormal Scaling Functions                      118
              6.4.1 Shannon Scaling Function                    118
               6.4.2 Meyer Scaling Function                     119
               6.4.3 Battle-Lemari6 Scaling Function            123
               6.4.4 Dauhechies Scaling Function                125

         6.5 Construction of Biorthogonal Wavelets              129

         6.6 Graphical Display of Wavelets                      132
              6.6.1 Iteration Method                            132
               6.6.2 Spectral Method                            132
               6.6.3 Eigenvalue Method                          134

         6.7 Exercises                                          134

         6.8 Computer Programs                                  138
              6.8.1 Daubechies Wavelet                           138
               6.8.2 Iteration Method                           139

              References                                         139


    7   Discrete Wavelet Transform and Filter Bank Algorithms   141

          7.1 Decimation and Interpolation                       141
               7.1.1 Decimation                                  142
                                                                CONTENTS      xi

           7.1.2 Interpolation                                              144
           7.1.3 Convolution Followed by Decimation                         147
           7.1.4 Inte叩olation Followed by Convolution                       147
      7.2 Signal Representation in the Approximation Subspace               148
      7.3 Wavelet Decomposition Algorithm                                   149
     7.4 Reconstruction Algorithm                                           153
     7.5 Change of Bases                                                    154
     7.6 Signal Reconstruction in Semiorthogonal Subspaces                  156
           7.6.1 Change of Basis for Spline Functions                       157
           7.6.2 Change of Basis for Spline Wavelets                       160
     7.7 Examples                                                          163
     7.8 Two-Channel Perfect Reconstruction Filter Bank                    165
          7.8.1 Spectral-Domain Analysis of a Two-Channel
                PR Filter Bank                                             168
          7.8.2 Time-Domain Analysis                                       176
     7.9 Polyphase Representation for Filter Banks                         180
          7.9.1 Signal Representation in the Polyphase Domain              180
          7.9.2 Filter Bank in the Polyphase Domain                        181
    7.10 Comments on DWT and PR Filter Ba마s                                182
    7.11 Exercises                                                         183
    7.12 Computer Programs                                                 184
         7.12.1 Algorithms                                                 184
         References                                                        186

8   Fast Integral Transform and Applications                               187
     8.1 Finer Time Resolution                                             188
     8.2 Finer Scale Resolution                                            190
     8.3 Function Mapping into the Interoctave Approximation Subspaces     194
     8.4 Examples                                                          196
          8.4.1 IWT of a Line町 Function                                    197
          8.4.2 Crack Detection                                            202
          8.4.3 Decomposition of Signals with Nonoctave Frequency
                Components                                                 203
          8.4.4 Perturbed Sinusoidal Signal                                203
          8.4.5 Chirp Signal                                               204
xii    CONTENTS

            8.4.6 入4usic Signal with l寸아se                      204
            8.4.7 Dispersive Nature of the Waveguide Mode       205

           References                                           209

 9    Digital Signal Processing Applications                    210

       9.1 Wavelet Packets                                      211

       9.2 Wavelet Packet Algorithms                            212

       9.3 Thresholding                                         214
            9.3.1 Hard Thresholding                             216
            9.3.2 Soft Thresholding                             217
            9.3.3 Percentage Thresholding                       218
            9.3.4 Implementation                                218

       9.4 Interference Suppression                             219

       9.5 Faulty Bearing Signature Identification              221
            9.5.1 Pattern Recognition of Acoustic Signals       221
            9.5.2 Wavelets, Wavelet Packets, and FFF Features   226

       9.6 Two-Dimensional Wavelets and Wavelet Packets         228
            9.6.1 Two-Dimensional Wavelets                      228
            9.6.2 Two-Dimensional Wavelet Packets               231

       9.7 Wavelet and W鉀elet Packet A培ori血ms 的r
           Two-Dimensional Signals                              233
            9.7.1 Two-Dimensional Wavelet Algorithm             233
            9.7.2 Wavelet Packet Algorithm                      234

       9.8 Image Compression                                    235
            9.8.1 Image Coding                                  235
            9.8.2 Wavelet Tree Coder                            236
            9.8.3 EZW Code                                      238
            9요4 EZW Exan叩le                                     239
            9요5 Spatial-Oriented Tree                           242
            9요6 Generalized Self-Similarity Tree                244

       9.9 Microcalcification Cluster Detection                 244
            9.9.1 CAD Algorit노n Structure                       244
             9.9.2 Partitioning of Image and Nonlinear
                   Contrast Enhancement                         245
             9.9.3 Wavelet Decomposition of the Subimages       245
             9.9.4 Wavelet Coef岫ent Dom鈿 Processing             246
                                                                CONTENTS    xiii

              9.9.5 Histogram Thresholding and Dark Pixel Removal          248
              9.9.6 Parametric ART2 Clustering                             248
              9.9.7 Results                                                249
        9.10 Multicarrier Communication Systems                            249
             9.10.1 OFDM Multicarrier Communication Systems                250
             9.10.2 Wavelet Packet-Based MCCS                              252
        9.11 Three-Dimensional Medical Image Visualization                 252
             9.11.1 Three-Dimensional Wavelets and Algorithms              255
             9.11.2 Rendering Techniques                                   256
             9.11.3 Region of Interest                                     258
             9.11.4 Summary                                                258
     9.12 Computer Programs                                                258
             9.12.1 Two-Dimensional Wavelet Algorithms                     258
             9.12.2 Wavelet Packets Algorithms                             263
             References                                                    265

10   Wavelets in Boundary Value Problems                                   267
        10.1 Integral Equations                                            268
        10.2 Method of Moments                                             272
     10.3 Wavelet Techniques                                               273
             10.3.1 Use of Fast Wavelet Algorithm                          273
             10.3.2 Direct Application of Wavelets                         274
             10.3.3 Wavelets in Spectral Domain                            275
             10.3.4 Wavelet Packets                                        280
     10.4 Wavelets on the Bounded Interval                                 280
     10.5 Sparsity and Error Considerations                                282
     10.6 Numerical Examples                                               285
     10.7 Semiorthogonal Versus Orthogonal Wavelets                        291
     10.8 Differential Equations                                           294
     10.9 Expressions for Splines and Wavelets                             295
            References                                                     297

Index                                                                      301
 Preface


  This textbook on wavelets evolves from teaching undergraduate and postgraduate
  courses in the Department of Electrical Engine이ing at Texas A&M U加ersity, and
  teaching' several short courses at Texas A&M University as well as in conferences
  such as the Progress in Electromagnetic Research Symposium (PIERS), IEEE An-
 tenna and Propagation (IEEE-AP) Symposium, IEEE Microwave Theory and Tech-
 nique (IEEE-MTT) Conference, and those of the Association for Computational
 Elec甘omagnetic Society (ACES). The participants at the short courses came from
 industries as well as universities and had backgrounds mainly in electrical engineer-
 ing, physics, and mathematics with little or no prior understanding of wavelets. In
 preparing material for the lectures, we referred to many books on this subject, some
 catering to the needs of mathematicians and physicists, others to engineers with a
 signal processing background. We felt the need for a book that would combine the
 theory, algorithms, and applications of wavelets and present them in such a way that
 the reader can easily le띠n the subject and be able to apply them to solve practi-
 cal problems. That being our motivation, we have tried to keep a balance between
 mathematical rigor and practical applications of wavelet theory. Many mathematical
 concepts have been elucidated through figures.
     The book is organized as follows. The first chapter gives an overview of the book.
The rest of the book is divided into four parts. In Chapters 2 and 3 we review some
basic concepts of linear algebra, Fourier analysis, and discrete signal analysis. The
next three chapters 게e devoted to discussing theoretical aspects of time-frequency
analysis, multiresolution analysis, and construction of various types of wavelets, and
in Chapters 7 and 8 we give several algorithms to compute wavelet transforms and
implement them through filter bank approach. In Chapter 8 and in Chapters 9 and
10 we present many interesting applications of wavelets to signal processing and
bound띠y value problems.
    In preparing this book we have benefited from the assistance of a number of
people. We learned a lot about wavelets through our association with Professor
Charles Chui, to whom we are very grateful. We would like to thank Professors Raj

                                                                                   xv
xvi    PREFACE

入恤tra, Linda Kate址，and Hao Ling 如r inviting us to spe出  （at short的urses at iEEE-
AP and MTF conferences. Thanks are also due to Professor L. 啼ang for inviting
us to organize the short course at PIERS. Parts of Chapters 4 and 9 come from our
collaboration with graduate students at Texas A&M University, nonible among them
being Minsen Wang, How町d Choe, Nai-wen Lin, Tsai-fa Yu, and Zhiwha Xu. We
thank all of them for their contributions. We wish to express our deep sense of ap-
preciation to Michelle R奴n, 毗io typed and pro可read most 可 小is book. We 如nk
Professor Kai Chang for his encouragement to write this book. Thanks 게re also due
to 玉血. George J. Telecki, Executive Editor, and Ms. Angioline Loredo, Associate
Managing Editor, for their efficient management and supervision diring the produc-
tion of this book. Last but not the least, we thank Mousumi Gos\k'anii and Sophia
Chan for their encouragement and support during the preparation of this book.

                                                           JAIDEVA C. GoswAM1
                                                           ANDREW K. CHAN
Fundamentals
of Wavelets
CHAPTER ONE




What This Book Is About


The concept of wavelet analysis has been in place in one form or another since the
beginning of the twentieth century. The Littlewood-Paley technique and Caldern-
Zygmund theory in harmonic analysis and digital filter bank theory in signal pro-
cessing can be considered as forerunners of wavelet analysis. However, in its present
form, wavelet theory attracted attention in the 1980s through the work of several
researchers from various disciplines-Stromberg, Monlet, Grossmann, Meyer, Bat-
tie, Lemari , Coifman, Daubechies, Mallat, Chui-to name a few. Many other re-
searchers have also made significant contributions.
    In applications to discrete data sets, wavelets may be considered as basis functions
generated by dilations and translations of a single function. Analogous to Fourier
analysis, there are wavelet series (WS) and integral wavelet transforms (IWTs). In
wavelet analysis, WS and IWTs are intimately related. The I刃T of a finite-energy
function on the real line evaluated at certain points in the time-scale domain gives
the coefficients for its wavelet series representation. No such relation exists between
Fourier series and Fourier transform, which are applied to different classes of 佃lc-
tions; the former is applied to finite-energy periodic functions, whereas the latter is
applied to functions that have finite energy over the real line. Furthermore, Fourier
analysis is global in the sense that each frequency (time) component of the function
is influenced by all the time (frequency) components of the function. On the other
hand, wavelet analysis is a local analysis. This local nature of wavelet analysis makes
it suitable for time-frequency analysis of signals.
     Wavelet techniques enable us to divide a complicated function into several sim-
pler ones and study them separately. This property, along with fast wavelet algo-
rithms, which are comparable in efficiency to fast Fourier transform algorithms,
makes these techniques very attractive in analysis and synthesis problems. Differ-
ent types of wavelets have been used as tools to solve problems in signal analysis,
image analysis, medical diagnostics, boundary value problems, geophysical signal
processing, statistical analysis, pattern recognition, and many others. 꿔hile wavelets
have gained popularity in these areas, new applications are continually being inves-
 tigated.

                                                                                      1
 2     WHAT THIS BOOK IS ABOUT

       A reason for the popularity of wavelet is its effectiveness in representation of
   nonstationary (transient) signals. Since most of natural and hu車an-made signals are
   transient in nature, different wavelets have been used to repre닉ent this much larger
   class of signals than Fourier representation of stationary sigrals. Unlike Fourier-
   based analyses that use global (nonlocal) sine and cosine functiOns as bases, wavelet
   analysis uses bases that are localized in time and frequency to represent nonstationary
   signals more effectively. As a result, a wavelet representation is much more compact
   and easier to implement. Using the powerful multiresolution analysis, one can repre-
   sent a signal by a finite sum of components at different reso1ut아ls so that each com-
  ponent can be processed adaptively based on the objectives ofthe application. This
  capability to represent signals compactly and in several levels of노esolution is the ma-
  jor strength of wavelet analysis. In the case of solving partial differential equations
  by numerical methods, the unknown solution can be represented by wavelets of dif-
  ferent resolution, resulting in a multigrid representation. The dense matrix resulting
  from an integral operator can be made less dense using wavele-based thresholding
  techniques to attain an arbitrary degree of solution accuracy.
      There have been many research monographs on wavelet ana1ysis as well as text-
 books for specific application areas. However, there seems to be no textbook that
 provides a systematic introduction to the subject of wavelets and1its wide areas of ap-
 plications. This was the motivating factor for us to write this introductory text. Our
 aim is (1) to present this mathematically elegant analysis in a formal yet readable
 fashion, (2) to introduce to readers many possible areas of applic目tions in both signal
 processing and boundary value problems, and (3) to provide se斗eral algorithms and
 computer codes for basic hands-on practices. The level of writing will be suitable for
 college seniors and first-year graduate students. However, suffi仁ient details will be
 given so that practicing engineers without a background in signal analysis will find
 it useful.
     The book is org出lized logically to develop the concept of wavelets. It is divided
into four major parts. Rather than vigorously proving theorems and developing algo-
rithms, the subject matter is developed systematically from the very basics of signal
representation using basis functions. Wavelet analysis is explained via a parallel with
Fourier analysis and the short-time Fourier甘ansform. Multireso1ition analysis is de-
veloped to demonstrate the decomposition and reconstruction algorithms. Filter bank
theory is incorporated so that readers may draw a parallel between the filter bank
algorithm and the wavelet algorithm. Specific applications in signal processing, im-
age processing, electromagnetic wave scattering, boundary value problems, wavelet
imaging systems, and interference suppression are included. A detailed chapter-by-
chapter outline of the book follows.
     Chapters 2 and 3 are devoted to reviewing some basic mathen1atical concepts and
techniques and to setting the tone for time-frequency and time-scale analysis. To
have a better understanding of wavelet theory, it is necessary to review the basics
of linear functional space. Concepts in Euclidean vectors are extended to spaces in
higher dimensions. Vector projection, basis functions, local and Reisz bases, orthog-
onality, and biorthogonality are discussed in Chapter 2. In addition, least-squares
approximation of functions as well as such mathematical tools as matrix algebra
                                                      WHAT THIS BOOK IS ABOUT         3

and z-transform are discussed. Chapter 3 provides a brief review of Fourier analysis
to set the foundation for the development of continuous wavelet transform and dis-
crete wavelet series. The main objective of this chapter is not to redevelop Fourier
theory but to remind readers of some important issues and relations in Fourier anal-
ysis that are relevant to later development. The principal properties of Fourier Se-
ties and Fourier transform are discussed. Lesser known theorems, including Pois-
son's sum formulas, partition of unity, sampling theorem, and the Dirichlet kernel
for partial sum are developed in this chapter. Discrete-time Fourier transform and
discrete Fourier transform a七 also mentioned briefly for the pu叩ose of comparing
them with continuous and discrete wavelet transforms. Some advantages and draw-
backs of Fourier analysis in terms of signal representation are presented.
    Development of time-frequency and time-scale analysis forms the core of the
second major section of this book. Chapter 4 is devoted to a discussion of the short-
time Fourier transform (time-frequency analysis) and the continuous wavelet trans-
白nn（山ne-scale analy計旬．TI比 similarities and 小付eret兀es between these two 甘ai哈．
forms are pointed out. In addition, window widths as measures of localization of a
time function and its spectrum are intr에uced. This chapter also contains the ma-
jor properties of the transform, such as perfect reconstruction and uniqueness of in-
verse. Discussions of the Gabor transform and Wigner-Ville distribution complete
this chapter on time-frequency analysis. Chapter 5 contains an introduction to and
discussion of multiresolution analysis. The relationships between nested approxima-
tion spaces and wavelet spaces are developed via a derivation of two-scale relations
and decomposition relations. Orthogonality and biorthogonality between spaces and
between basis functions and their integer translates are also discussed. This chapter
also contains a discussion of the semiorthogonal B-spline function as well as tech-
niques for mapping the function onto multiresolution spaces. In Chapter 6, meth-
ods and requirements for wavelet construction are developed in detail. Orthogonal,
semiorthogonal, and biorthogonal wavelets are constructed via examples to eluci-
date the procedure. Biorthogonal wavelet subspaces and their orthogonal properties
are also discussed in this chapter. A derivation of the formulas used in methods to
compute and display the wavelet is presented at the end of this chapter.
    The algorithm development for wavelet analysis is contained in Chapters 7 and
8. Chapter 7 provides the construction and implementation of decomposition and
reconstruction algorithms. The basic building blocks for these algorithms are dis-
cussed at the beginning of the chapter. Formulas for decimation, interpolation, dis-
Crete convolution, and their interconnections are derived. Although these algorithms
are general for various types of wavelets, special attention is given to the compactly
 supported semiorthogonal B-spline wavelets. Mapping formulas between the spline
 spaces and the dual spline spaces are derived. The algorithms for a perfect recon-
 struction filter bank in digital signal processing are developed via z-transform in this
chapter. The time-domain and polyphase-domain equivalents of the algorithms are
discussed. Examples of biorthogonal wavelet construction are given at the end of
 the chapter. In Chapter 7, limitations to the discrete wavelet algorithms, including
 the time-variant property of the discrete wavelet transform and the sparsity of data
 distribution are pointed out. To circumvent the difficulties, the fast integral wavelet
 4     WHAT THIS BOOK IS ABOUT

  transform (FIWT) algorithm is developed in Chapter 8 for the semiothogonal spline
  wavelet. S恤ting with an increase in time resolution and ending 申ith an increase
 in scale resolution, a step-by-step development of the algorithm is 巾resented in this
 chapter. A number of applications using FIWT are included to illuhtrate its impor-
 tance.
     The final section of上is book is on the application of waveleti to engineering
 problems. Chapter 9 includes their applications to signal and image processing, and
 in Chapter 10 we discuss the use of wavelets in solving boundary vaue problems. In
 Chapter 9, the concept of wavelet packets is discussed first as an exte土lsion of wavelet
 analysis to improve the spectral domain performance of the wavelet. Wavelet packet
 representation of signal is seen as a refinement of the wavelet in the spectral do-
 main by further sub五viding the wavelet spectrum into subspectra. 까is is seen to be
 useful in subsequent discussions of radar interference suppression. Three types of
 amplitude 仕reshol竝ng are discussed in this chapter and are used in subsequent ap-
 plications to image compression. Signature recognition on faulty bearing completes
 the one- 五mensional wavelet signal processing. The wavelet algorithls in Chapter 7
 are extended to two dimensions for processing of images. Major vavelet image-
 processing applications included in this chapter are image compre$sion and target
 detection and recognition. Details of tree-type image coding are nt included be-
 cause of limited space. However, the detection, recognition, and c'ustering of mi-
crocalcifications in m刎almograms are discussed in moderate detail. 恤le application
of wavelet packets to multicarrier communication systems and the application of
 wavelet analysis to three-dimensional medical image visualization are also included.
Chapter 10 concerns wavelets in boundary value pr이）lems. 끄ie tradit如카 毗出od 可
moments and the wavelet-based method of moments are developed i n parallel. Dif-
ferent ways to use wavelets in the method of moments are discusse.. In particular,
wavelets on a bounded interval as applied to solving integral equatkns arising from
electromagnetic scatte血lg problems are presented in some detail. These boundary
wavelets are also suitable to avoid edge effects in image processing Finally, an ap-
plication of wavelets in the spectral domain is illustrated by applying them to solve
a transmission-line discontinuity problem.
    Most of the material is derived from lecture notes prepared for undergraduate
and graduate courses in the Department of Electrical Engineering at Texas A&M
University as well as for short courses taught at several conferences. The material in
this book can be covered in one semester. Topics can also be selec唯vely amplified
to complement other signal processing courses in an existing curric4lum. Exercises
are included in some chapters for the pur均se of practice. A number!of figures have
been included in each chapter to expound mathematical concepts. $uggestions on
computer code generation are also included at the end of some chapt中rs.
CHAPTER TWO




Mathematical Preliminaries


The purpose of this chapter is to familiarize the reader with some of the mathemat-
ical notations and tools that 町e useful in an unders切nding of wavelet theory. Since
wavelets 町e continuous functions that satisfy cer切in admissibility conditions, it is
prudent 的曲螂s some definitions and propert妃s of fun茁onal spaces. 恥r a more
detailed discussion of functional spaces, the reader is referred to stand町d texts on
real analysis. The wavelet algorithms discussed in later chapters involve digital pro-
cessing of coefficient sequences. A fundamental understanding of topics in digital
signal processing, such as sampling, the z-transform, linear shift-invariant systems,
and discrete convolution, is necess缸y for a good g邸p of wavelet theory. In addition,
a brief discussion of linear algebra and matrix manipulations is included that is very
useful in discrete-time domain analysis of filter banks. Readers already familiar with
its contents may skip this chapter.



2.1   UNEAR SPACES

In the broadest sense, a functional space is simply a collection of functions that
satisfy a certain mathematical structural pattern. For example, the finite-energy space
L2（小以）, 的小 a collec如n of func如ns that are square 奴e肛able; that is,



                               亡／     （玔'    六   （的·                             (2.1)
Some of the requirements and operational rules on linear spaces are stated as follows:


   1. The space S must not be empty.
   2. If工e S and y E 5, then工＋y= y＋工. 49f d0드小1E
   3. IfzcS, then（工＋ y)＋之＝工＋(y+ z)· 皿tymm岫）t} \/e
                                                                                     5
6      入4ATH日너A기CAL PREL小시NA뫼ES

    4. There exists in S a uniq此이.ment 0, such that x +0= ;                         泳油t'1상
    5. There exists in S another unique element -x such that x + (- x) = 0.
                                                                         ＼닉VeY도e
  Besides these simple yet important rules, we also define sa1ar multiplication
y = cx such that if x E S, then y E S, for every scalar c. We have the following

additional rules   for   the space   5:        CVe拓r9中比）
    1. C（工 + y) = C工 + cy.
    2. k + d）工 = c工 + d工 \'ith scalar C and d.
    3. (cd)x = c(dx).
    4. 1 1x = 工．

Spaces that satisfy these additional rules are calle&f'inear spaces. However, up to
now, we have not defined a measure to gauge the size of an element in a linear snace.
it we assign a number lix ii, caliec me no力7i aix, to eacn runction in D , mis space
becomes a normed linear space (i.e., a space with a measui4 associated with it). The
norm of a space must also satisfy certain mathematical propertie3:

    1. II工II 之 0 and U工11 = 0 <===> 工 == 0.
    2. II工 + 川 5 h11 + 卄yll.
    3. fla工n = 口 11工fi, where 口 is scalar.

   The norm of a function is simply a measure of the distance of the function to the
origin (i.e., 0). In other words, we can use the norm

                                                       卄工 叫 yU                                (2.2)

to measure the difference (or distance) between two functions, x                    y.
    There are a variety of norms that one may choose as a meas                      for a particular
linear space. For example, the finite-energy space L2(小以）, 以）) u                    the norm



                            似11= L        [/   -   :   If（玔'   이 " ' （的，                      (2.3)
which we shall call theL놔 . This norm has also been used to measure the overall
difference (or error) between two finite-energy functions. This measure is called the
root-mean-square error (RMSE) defined by


                 RMSE=[T-
                 m52= [：覲｝a  'T/2·f(x)-fa(玔2dx
                                                                                2

                      Lim T!J，
                        *。。  -T/2                                          ]'
                                                                                              (2.4)


where fa (x) is an approximating function to f (x). The expres:
approximation error in the L2 sense.
                                                          VECT（긔之SAND VECTC水 SPACES               7


2.2    VECTORS AND VECTOR SPACES

Based on the basic concepts of functional spaces discussed in Section 2.1, we now
present some fundamentals of vector spaces. We begin with a brief review of geo-
metric vector analysis.
    A vector V in a three-dimensional Euclidean vector space is defined by three
complex numbers {vi, v2, V3} associated with three orthogonal unit vectors (ai, a2,
』1 } 丁1m 八mJ八4八J n八1 - . .2     mmhm八nmm1n 11mm n4n1八1' 八八H．在八小mm1n 八r11= m . . 八n＋八＝1ir , . . 14八m八
a3J. [he ordered set jv1J二1 represents the scalar components of the vector V. where
inc unit vector set {a i ｝너 , snans inc tnree-aimensionai tucnaean vector snace. AflV
vector U in tins snacCcan be decomnosed into three vector comnonents lu ia i 1'
(see Figure 2.ld).        O, , Ab匈
    The addition and scalar multiplication of vectors in 吐is space are defined by:

   1. Ui-V= {ui+ vi, u2+ v2, u3+ v3}.
   2. kV = {kvi, kv2, kv3}.




                                                            U3n3
              a3


         ai            a2


                                                                           V - v3a3


                          (a)
                                                                            (b)




                                                            r3n3


                   V - v3a3 - vial                                             I

      vial                                               vial


                       V - v3a3
                         (c)
                                                                            (d)
          디CURE 2.1 （力thogonal d凹ompositi이i of a ye야or in Euclidean spac已
 8         MATHEMATICAL PRELIMINARIES


  .    addition to these
      In
                           . ons, vectors    a
 aiso ooey me commutative ana associative laws:
                               operati.
                                                                                                     .    in
                                                                                                                         由ree-
                                                                                                                                       dimensional   乍ucidean space

      l. U+ V= V+ U.                        0cr州m岫心沖
      2. (U+ V) +w= U+ (V+ W).                                                           c&妃oC-卜寸i此




                                                                                         [
      We may represent a vector by a column matrix,



                                                                                                         U U U
                                              =                                                  1
                                                                                                               l

                                                                                 V
                                                                                             1
                                                                                         1
                                                                                                               n
                                                                                                               乙
                                                      H1


                                                                                                                                                              (2.5)
                                                                                                               n
                                                                                                               4
                                                                                                               U
                                              H




since all of the mathematical rules above apply to column matrices. We define the
length of a vector similar to the definition of the norm of a function, by


                                                  ；듀耳 ,/
                                              IV'小＝                                                                                                           (:．旬
The scalar pr에uct (inner product) of two vectors is a very important operation in
vector algebra that we should consider here. It is defined by

                                          U · V := 1UI IVI cos LU, V

                                                  =        ulVl + U2V2 + U3V3

                                                                                                                                 LI!
                                                  =        [ui
                                                                                         U2                         U3]          iJ)
                                                                                                                                 t나
                                                                                                     r



                                                                                 nnn
                                                                                                          尸




                                                                                                                 U U U
                                                                             e
                                                                                     l
                                                                                                                                                                                      m
                                                                                                                   l
                                                                                                                                                                                  m
                                                                                                          1
                                                                         1
                                                                                     4
                                                                                     1                    1

                                                                     1
                                                                                                          1
                                                                                                                   八
                                                                                                                   J1
                                                                                                                                                              (2.7)       1
                                                                                                                                                                              1
                                                                                                                                                                                          H1




                                                                                     八
                                                                                     4
                                                                                     U                             m
                                                                                                                   4J
                                                                                                          H
                                                                 L
                                                                                                                                                                      ]
                                                                                                                                                                      ]
where the superscript李indicates matrix 虹a珽position and娩is the symbol f야小朗－
mtion. It is known that the scalar product obeys the commutative law: U. V = V . U.
Two vectors U and V are o月hogon口l to each other if U . V = 0. We define the
projection of a vector onto another vector by

                    U. V
                    1；可 니J " a『
                           = projection of U in the direction of aU
                           = a component of U in the direction of aU.                                                                                        (2.8)

Projection is an important concept which will be used often in later discussions. If
one needs to find the component of a vector in a given direction, simply project the
vector in that direction by taking the scalar product of the vector with the unit vector
of the direction desired.
                                                                      BASIS FUNCTIONS       9

   We may now extend this concept of basis and projection from the three-
dimensional Euclidean space to an N-dimensional vector space. The components of
a vector in this space form an N x 1 column matrix, while the basis vectors Ia ;V'Y
rorm an onnogonai set sucn mat

                           ak · at = dk , t                Vk, tEZ,                     (2.9)

where 3k,t is the Kronecker delta, defined as


                                                           口．
                                                      1,   k= f
                                                                                    (2.10)
                               8k,   t=          {=
One can obtain a specific component vj of a vector V (or the projection of V in the
direction of aj) using the inner product

                                               vj = V · a3,                         (2.11)

and the vector V is expressed as a linear combination of its vector components,


                                          V=
                                                      ＞二vkak.                       (2.12)


It is well known that a vector can be decomposed into elementary vectors along the
direction of the basis vectors by finding its components one at a time. Figure 2.1
illustrates this procedure. The vector V in Figure 2.la is decomposed into VP =
V - v3a3 and its orthogonal complementary vector v3a3. The vector V,, is further
decomposed into via1 and v2a2. Figure 2.id represents the reconstruction of the
vector V from its components.
    The example shown in Figure 2.1, although elementary, is analogous to the
 wavelet decomposition and reconstruction algorithm. There the orthogonal compo-
nents are wavelet functions at different resolutions.


2.3   BASIS FUNCTIONS

We extend the concept of Euclidean geometric vector space to normed linear spaces.
That is, instead of thinking about a collection of geometric vectors, we think a均ut a
collection of functions. Instead of basis vectors, we have basis functions to represent
arbitrary functions in that space. These basis functions are basic building blocks for
functions in that space. We will use the Fourier series as an example. The topic of
Fourier series is considered in more detail in Chapter 3.

Example: Let us recall that a periodic function PT (t) can be expanded into a series


                              PT(t) = ＞二 Ck少叫                                           (2.13)
 10     入4ATH［叭4ATICAL PREE 小시NA뫼ES

 where T is the periodicity of the function, w = 2ir/ T = 2兀f is the fundainen-
 tal frequency, and ej710勺t is the nth harmonic of the fundamental frequency鹿亘曲
 tion (2.13) is identical to (2.12) if we make the equivalence between PT (t) with V,
 ck with vk, and eJI(蜘t with ak. Therefore, the function set {ejk蜘' }kEZ forms the
 basis setfor the Fourier space of discrete frequency. Here Z is the set of all integers,
 {. .. , -1, 0, 1, . . .1. The coefficient set {Ck}kEZ. is often referred to as the discrete
 spectrum . It is well known that the discrete Fourier basis is an orthogonal basis.
 Using the inner product notation for functions                                      \


                                                侮h)        =   /,    !(!   ）瓦了dt,
                                                                                                   (2.14)


 where the overbar indicates complex conjugation, we express th orthogonality by

                    1   fl/               h

                    京 /                       ejC蜘teeJt的tdf= 8k.C                   Vk,   te   .   (2.15)

 We may normalize the basis functions (with respect to unit ehergy) by dividing
 them with .J . Hence {eik的n/ /fJkEZ forms the orthonormal basis of the discrete
 Fourier space.


 2.3.1 Orthogonality and Biorthogonality
아thogonal expansion of a function is an important tool for signal analysis. The
  coefficients of expansion represent the』magnitudes of the signal．牟omponents. In the
 탓삐pie aoo,ve' 唯三쀼藝뜨쁘므므쯔．측匹戰：                      尸m,ne arnputua斗S .O1』me narmonic
,irequency O1 me signal. u ior som. e.parucular si望
                                                  ，ai pr.ocessing 叩jecuv.e we aeciue
 to minimize ior m.aie zerotcertain narrnomc rre9uencies sucn.as n吐z noise). we
 simpiy aesign a nner at mat irequency to reject me noise. it is inereiore meamngrui
 to decompose a signal into components for observation before processing the signal.
    q恤略onal deco呻osition 可 a 毗nal is straightfor꿔ard, and the con叩utation 可
 the coefficients is simple and efficient. If a function 1(r) E L2 is exnanded in terms
 or a certain ormonormai set j中k(t) jEZ C i二 we may wnte              !

                                                                    00

                                                      只r) = ＞二 Ck中k(t).                            (2.16)
                                                               k=-oo

 We compute the coefficients by t삯：ing the inner product of the fun tion with the basis
 to yield


                              (.
                                   /，似）               :   /:f (t）而而dr
                                                  工，斗吻(t)而而dt
                                                                             BA引S FUNC기이니S      11


                                                    的 Z 如
                                                              k
                                                              Z
                                                             nd
                                                              t
                  11                                          C
                                              尸L




                                   =          Ck.                                            (2.17)
 Computation of an inner product such as the one in (2.17) requires knowledge of the
 function f (t) for all t and is not real-time computable.
     We have seen that an orthonormal basis is an efficient and straightforward way
 to represent a signal. In some applications, however, the orthonormal basis function
 may lack certain desirable signal processing properties, causing inconvenience in
 processing. Biorthogonal representation is a possible alternative to overcoming the
 constraint in orthogonality and producing a good approximation to a given function.
 Let {呱 (t)}keZ E L2 be a biorthogonal basis function set. If there exists another basis
 function set { k (t) }kEz e L2 such that


                         （仇，而）=/：似（!）瓦石dt =6(，《，                                             (2.18)
 the set { k (t) jkEz is called thedijI占aIis of { k(t))k.Z. We may expand a function
 g(t) in terms of the biorthogonal basis


                                    g(t) = ＞二dk中k(i),
                                                            k=O

 and obtain the coefficients by

                                  따 = (g, 而）                                             (2.19)

                                        =L？而dt.                                          (2.20)

 On the other hand, we may expand the function g(t) in terms of the dual basis

                                              蛔
                                                        ＞二dkcbk    (t)
                                                                         ,
                                                                                         (2.21)


and obtain the dual coefficients dk by

                                  d1 = (g, 伽）                                            (2.22)

                                                            g(t）伽(t) dt.                 (2.23)
                                       J00-
                                                     。。


We recall that in an orthogonal basis, all basis functions belong to the same space. In
a biorthogonal basis, however, the dual basis does not have to be in the original space.
If the biorthogonal basis and its dual belong to the same space, these bases are called
心emiorthogona1. Spline functions of an arbitrary order belong to the semiorthogonal
class. More details about spline functions are considered in later chapters.
12     MATHE入4ATICAL PREL小시NARIES

   We use geometric vectors in a two-dimensional vector space to illustrate the
biorthogonality. Let the vectors




                                  61=
                                                L2 _
                                                                 [:
                                                                                 }
form a biorthogonal basis in the two-dimensional Euclidean space. The dual of this
                                                                                                                =   [二
                                                                                                                            [;}
basis is

                                                 r-
                                                                         '
                         81
                                                                                       1I
                                                                                                  ,       b2=
The bases are displayed graphically in Figure 2.2. We can compute the dual basis
in this two-dimensional Euclidean space simply by solving a set of simultaneous
equations. Let the biorthogonal basis be


                                        h=
                                                                      LX2J
                                                                      fxi]
                                                                                        I     ,
                                                                                                         LY2
                                                                                                      62出i
and the dual basis be
                              mfu
                              1)                                                                      阡
                                1=                        1LU2
                                                                                                                    ［viV2
                    石l
                                                                                                      b1
                              \
                                             \
                                                      \
                                                          \                                 ,1/



                                                                             \              b2
                                                                                 '食＼
         FIGURE 2.2 Biorthogonal basis in two-dimensional Euclidean space.
                                                                                      LOCAL BASIS AND RIESZ BASIS         13

    The set of simultaneous equations that solves for b1 and b2 is


                                                             ( bl, f;) =1
                                                             (b2, f;)=0
                                                                                                                       (2.24)
                                                             (bi,I4= o
                                                             (b2, b2) = 1.

 This process can be generalized into a finite-dimensional space where the basis vec-
 tors form an oblique (nonorthogonal) coordinate system. It requires linear matrix
 transformations to compute the dual basis. This process will not be elaborated upon
 here. The interested reader may refer to El].


 2.4    IOCAI BASIS AND RIESZ BASIS

  꿔e have considered orthogon키 bases of a g勿b끄 nature in pr四蜘s sections ［中（1) :
  r E (- 以, 以)]. Observe that sine and cosine basis functions for Fourier series are
- defined on the entire real line (- oo, 以）) and therefore are called global bases. Many
  bases that exist in a finite interval of the real line [小(t) : I E (a. b1 satisfy the ortho으-
  onality or rnortnogonallty requirements, we call tnese local bases. I no j-laa[ t嶝sls單＝
 .th료요如出趾好跏刈立QL쵸locaL如血．

 丑ra仰九 1: TheH口口r bas加 is described by 吻Ik (t) == XE0, 1) (t 寸 k), k c Z, where


                                              XI0,I)(t)                                1                               (2.25)
                                                                 11J,          otnerwise
                                                                               0三t<
                                                                 !l,
 is the characteristic function. The Haar basis clearly satisfies the orthogon심ity con-
 dition

                    (中jj,   )(:
                              ),中H.       k
                                               (t)
                                                     )   =   /:        XF0, (t
                                                                          l)
                                                                                      -   j)x[o,I)   (t   -   k) dt.

                                                         = '5j,k.                                                      (2.26) "
               //                     느




    To represent a global function f (t), t e (- cc, OO) with a local basis 中(t), t e
 (a, b), functions that exist outside the finite interval must be represented by inte-
 ger shifts (delays) of the basis function along the real line. Integer shifts of global
 functions can also form bases for linear spaces. The Shannon function 中SH(t) is an
 example of such a basis.

 Example 2: The Shannon function is defined by

                                                                         sin 7r1
                                                         中SH(t) ==                                                     (2.27)
                                                                               irt
14        MATH타너ATICAL PREL小IINA뫼ES


and the basis formed by


                         中SH,
                           k(t) = '叩才， kZ                                                                                  (2.28)
is an orthonormal basis and is global. The proof of the orthonormality is best shown
in the spectral domain.
   Let g(t) E L2 be expanded into a series with basis functions {kk(t))kEZ:

                                                g(t) =                            ck0k    (t)   .                          (2.29)
                                                                              k

The basis set (0k (t)}kEz is called a Riesz basis if it satisfies the ft llowing inequality:

                      R네Ck ii弓2 5 ilg(t)112 5 R2 加kl准                                                                      (2.30)




                                                                                                                       1
                                                                                          2
                      R내Ck峰5 ＞二Ck中k(t) 5 R2 lick II和                                                                       (2.31)
                                                         k

where 0 < R1 5 R2 < 的 are called Riesz bounds. The space t is the counte聊rt
of L2 for discrete sequences with the norm defined as

                                                                                          1/2
                                                                                                ＜的．                        (2.32)
                                                 =
                                                                    \k                /
                                                         (二iCki2)
                                           《2
                               lCkIi
An equivalent expression for (2.30) in the spectral domain is


                      0 < R1기知＋2兀kr5R2＜的1       k
                                                                                                                           (2.33)
The derivation of (2.33) is left as an exercise. A hat over a function r枷esnts its
Fourier仕ansform,
                  ,a topic discussed in Chapter 3. , ,      , . H          . .

hU Al = 八．2 = i, inc oasis is oruionormai. inc bnan呵Lo聊sis an example ol.a
Kelsz nasls mat is ortnonormal, since rae spectrum or me Sflan걱On tunction is I in
      .
me mrervai L- lr, jrj . 1-lence


                                       刃8SH佃＋2兀可 三 1.                                                                      (2.34)
                                       k

If the basis functions {中(t - k) : k e 7L} 缸e not orthonormal we can obtain an
orthonormal basis set {中上 (t - k) : k E Z} by the relation

                          싸. .                                                 中（w)
                         171日느 1 /1) 1
                         거尸
                                            H
                                                                                                                           (2.35)
                                                                              ( + 22rk)
                               \1月／/        Hm                                                            m   ] ／口 1
                                                                                                              1 / 乙
                                                                                                    I2j
                                                     f              k    I0
                                                                                  -
                                                               DISCRETE LINEAR NORMED SPACE       15

 The Reisz basis is also called astable basts in the sense that if


                                        gi(t) =Z뿌可D
                                                          J


                                        g2(t) = ＞二口｝2）吻（r),
                                                          I

 a small difference in the functions results in a small difference in the coefficients,
 and vice versa. In other words, stability implies that


                                                                                    2 1
                                                                                      肛
                                                   112 H                       ej
                                                                      n         n
                                                                           (
                 small IIgi   (t)
                                    -   g2
                                             (t)
                                                              small
                                                                1

                                                                      t11U
                                                                       \
                                                                                              (2.36)



2.5 ［기SCRETE LINEAR NOR人任D SPACE

A discrete linear normed space is a collection of elements that a七 discrete sequences
of real or complex numbers with a given norm. For 食 discrete normed linear space,
the operation rules in Section 2.1 are applicable to discrete linear normed space as
well. An element in an N-dimensional linear space is represented by the sequence

                         工（n) == 仁（0),工（1), . . . , 工（N- 1)},                                 (2.37)

and we represent a sum of two elements as

  w(n) = x(n) + y(n) = fx(0) + y(0)' x(1) + y(l). ... .x(N - 1) + y(N - 1)).

                                                                                              (2.38)

The inner product and the norm in discrete linear space are defined separately as


                      似（n),y(n))＝二x(n)j7(n) ：油ev- r恤't                                        (2.39)



                                    lixil=(", )"' =1쭈' ("兀' :，們 ("·的）
Orthogonality and biorthogonality as defined previously apply to dis口ete bases as
well. The biorthogonal discrete basis satisfies the condition


                      （吻（n),3j(n))=＞二吻（n）万1(n) =8i,j1                                     (2.41)
                                                      n


For an orthonormal basis, the spaces are self-duaj; that is,

                                                   中／ == 中J.                              仁42)
16           入4ATH티너ATICAL PREL小시NA뫼ES


Example 1: The discrete Haar basis, defined as

                                                                      的rn = 0, 1
                             蜘，                                                                                                 (2.43)




                                                                                              1
                                             I士
                                         :
                                              to,
                                                                      otherwise,

is an orthonormal basis formed by the even translates of Ho(n). The Haar basis,
however, is not complete. That is, there exist certain sequences that cannot be repre-
                                                                                                                                         =
sented by an expansion from 小is basis. It requires a complementary space to make
it complete; The complementary space of Haar is




                                                        스扼 크扼 q
                                                                      如rn = 0
                               月     n                                 =
                                                                                                                                (2.44)
                                                                      for n = 1

                                                                      otherwise.

The odd translates of H1(n) form the complementary space, so 印y real sequence
can be represented by the Haar basis.

E뇨Zn甲加2: The sequence


                       D2(n)={ '茄 "茹 ";{ '引                                                                                     (2.45)


is a.finite sequence with four members. whose integer translates fori卞i an orthonormal
basis. [lie proot or ortilonormality is len as an exercise.          1


2.6          APPROXIMATION BY ORTHOGONAL PROJECTION

Assuming that a vector u(n) is not a member of the linear vector bpace V spanned
by W'k}, we wish to find an approximation uj7 E V. We use the orthogonal projection
of u onto the space V as the approximation. The projection is defined by

                                                                                                                                (2.46)


We
         remark here that the approximation error u                     -       u        is
                                                                                              orthogon    4l
                                                                                                                   to the space    V.
     m "at is,                   ,                  ,     ,       .             ,,   ,



                                (u- i{up,   中k)} ==
                                                 =0                             '1k.
                                                                                                               ;
                                       rj 1 (Pi     1J                          V 凡1


                                                    1:
                                 (1{ e



Furthermore,  the mean  square error
                               err0r (MSE)
                                     UVibl二）of such an a1가）
                                                       approximatibn
                                                           rOXlrnanO1l is minimum.
                                                                                                          .         .   .   .


rnrnlelln0re1 [ne rnean SqUare              01 SUC1l                   lS 1lll1nrnUna.
n        .         .             '           r.               .   .         ,                     .   .




   To prove the minimality of the MSE for any orthogonal projqction, consider a
function g e L2[a, b] that is approximated by using a set of orthonk)rmal basis func-
                                              APPROXIMATION BY ORTHOGONAL PROJECTION                                                       17

 tions {砂k : k = 0. . . . .N -1) such that

                                                                             N- I
                                          g(t) 심 gc(t) = 二 c1 1(t),                                                                  (2.47)
                                                                             j=0

vith
With
                                                               ci = (g，中／）·                                                          位48)

The pointwise error eC (t) in the approximation of the function g(r) is

                                                                                               N- i
                                  E小） =   g(t)    -       g
                                                               (t)
                                                                         =   g
                                                                                 (t)
                                                                                       -              c3b (t)   .
                                                                                                                                     (2.49)
                                                                                               j=0

We wish to show that when the co師cient sequence {cjI is obtained by orthogonal
projection given by (2.48), the MSE Ik.(t) 112 is minimum. To show this let us assume
that there is another sequence {d : j = 0. .. ..N - 1} which is obtained other than
by orthogonal projection, which also minimizes the error. Then we will show that
c3 =d; j =0. ....N- l, thuscompletingourproof.
   With the sequence {dj} we have

                                                                             N- i
                                          g(t) 勺 edO) = ＞二 d吻（t)                                                                    (2.50)
                                                                             j=0

and
                                                      2
                                                                /        철二i             졀二i   \
 卄Ed
       (t）
             卄2   =
                      g(t) 스二d中j(t)                           = ( g(t) 卞 乙 刃中八t), g(t) - 乙 刃中小）)
                                   j=0                               \                 j=O                                    j=0      I
                                  N- i                                   N- I                             N- i
                  = (g, g) 스二刃佃八n引스二可（g，中八t))+ 乂d尸
                                   j=0                                   j=0                              1=0
                                  N- I            N- i                           N- I
                      (g,g) 스二的스7k/ +＞二玎．                                                                                           (2.51)
                                   j=0            i= 0                             j=0

To complete the squ缸e of the last t뇨ee terms in (2.51), we add and subtract
꽈引寸to蛔d




                                                              Z厠 mZ向
                                                                                       2
                            （尤）
                                  卄2      0
                                          b   工
                                                      N- i               吻
                                                                         刃             m
                      卄Ed
                                                                                           n
                                                                                           乙           匈
                                          O
                                          凸   工
                                                                         幻
                                                                         勻             的              mZM           ;J
                                                                                                                         八乙

                                                                                                                    C               (2.52)
18       人lATH타며ATICAL PREL小시NARIES


                                                                         N- i

                                       =       IIEc II2 + ＞그dj
                                                       (X)
                                                          戶＝0
                                                                                     -    cJ12.
                                                                                                                                (2.53)


It is clear that to have a minimum MSE, we must have d = cj; j
and hence the proof.


2.7      MATRIX ALGEBRA AND LINEAR TRANSFORMATION

We have already used column matrices to represent vectors in thite-dimensional
Lucliclean spaces. Iviatrices are operators in tflese spaces. We give4 Drier review or
matrix, aigeora ifi tills section and uiscuss several types or special n}atnces mat Will
De uselul in me.understanding or time-domain analysis or wavelets 目na nlter nanKs.
lor details, readers 町e rererred to [zj.


2.7.1         Elements of Matrix Algebra
     1   11    11   1   1        1         1       1         r   .   1        .                     1         n        1

     I. Definition. A matrix A, = [Aif] is a recta.ngular array or e11men15. ine.ele-
        meri.ts may oe reai nurnoers, compiex.numoers, or poiynom1as. I ne nrsr.inte-
        ger.muex, i, is mle row muicator,. asia me secona integer inoex, 7 ,.is tue coiur끄
        indicator. A matrix is inflnite it I, 3 -+ no. An m x n matrix i$ displayed as

                                                             A11              A12   A13
                                                             A21              A22
                                               A                                                                                (2.54)
                                                             A31
                                                                                                        Amn
        If m =      A is a suu町e matrix.
                            n.               N x 1 c。        ma교x        An。ne c。            lumn                 (O       lv   lunm   'i
        represen四 an N -mmensionai vector.
     2. Transposition. The transpose of A is At, whose element is A/i. If the dimen-
        sion of A is m x n, the dimension of At is n x m. The transposition of a column
        (Nx l) matrixisarow (l xN) matrix.
     3. Matrix sum and difference. Two matrices may be summed if they have the
        same aimensions:

                                                   C= A 土 B ＝수 C1 = Aj 土 夙3.

     4. Matrix product. Multiplication of two matrices is meaningful
        mensions are compatiole. 1ompatwii.ity means mat tile numDPr O1 columns.in
         me nrst matrix must De tile.same as tile numoer O1 rows in tflf second matri.lx.
         Irme dimensions or Aana li are m x p.and p xq, respectivelt, tile dimension
         01 L = in               is m x q. m1le eiement Lij is given oy

                                                                     U
                                                                     C              P
                                                                                    Z日   A   O
                                                                                             B
                                MATRIX ALGEBRA AND LINEAR TRANSFORMATION                 19

        The matrix product is not commutative since p x q is not compatible
                                                                            with
        mx p. In general, AB 尹BA.
    5. Identity ,natnx. An identity matrix is a square matrix whose major diagonal
       elements are ones and whose off-diagonal elements are zeros.


                                                                        0000
                                                00




                                                             000l00
                                                      000
                                4




                                                    1
                                                    d
                                                0   0000
                                                                      m
                                                                      0
                                I
                                                 l1
                                                                      0000l0
                                                      =


                                                l00000                          l
                                                                            1
   6. Matrix minor. A minor S1 of matrix A is a submatrix of A created by deleting
      t加 油 row and jth c이umn of A· 가ie d恤毗ion ofSU is (m - 1) >< (n - 1) if
      the dimension of A is m x n.
   7. Determinant. The determinant of a square matrix A is a value computed suc-
      cessively using the definition of minor. We compute the determinant of a
      square (m x m) matrix by

                                                 m

                             det(A) = 刃- 1)勻匈det(S1j).
                                                i=1

      The index j can be any integer between [1, m].
   8. Inverse刃iatri工. A 나s the inverse of a square matrix A such that A 'A = I =
      i%Ad . We compute the inverse by


                                기                 *) (- i
                                     =
                                                 1
                                                 (A)                        (S)!).
                                                        1)
                                    -
                                                               "'
                                                                      det
                                    -     det
        If det(A) = 0, the matrix is singular, and A1 does not exist.


2.7.2     Eigenmatrix
A linear transformation is a mapping such that when a vector x E V (a vector space)
is transfonned, the result of the transformation is another vector, y = Ax E V. The
vector y, in general, is a scaled, rotated, and translated version of x. In p町ticular, if
the output vector y is the only scalar multiple of the input vector, we call this scalar
the ligenvalue and the system an eigensystem. Mathematically, we write

                                         y = Ax = tx,                                (2.55)

where A is an N x N matrix, x is an N vector, and .t is a scalar eigenvalue. We
determine the eigenvalues from the solution of the characteristic equation

                                    det(A 기 zI) = 0.                                 (2.56)
20      MATHE入4A기CAL PREL小시NAR任S


If x is an N x 1 column matrix, there are N eigenvalues in this system. These eigen-
values may or may not all be distinct. Associated witfl eacn elgenvalue is an eigen-
vector. Interpretations of the eigenvectors and eigenvalues depend on the nature of
the problem at hand. We substitute each eigenvalue pj into (2.56) to solve for the
eigenvector xi. We use the following exa삐e to illustrate this procedure. Let



                                                                                        0 l n4J
                                             [ 3                       -1
                             H

                                          A= I- 1                         2
                                             L 0                       -l

be the transformation matrix. The characteristic equation from (2.56) is

                                                  r3H/1 - -1                                      0그
             det(A - IL!) = det I                               1         2 -／工          - -
                                                  L             0            -1          3- IL]
                             = (3 기｛) [(2 m /{)(3 H /{) 1 l] 中 (3 m                                                    M)
                             = (3 - 肛）（尸 - l) (IL 小 4) = 0

and the eigenvalues are / t = 4, 1, and 3. We substitute 尸 = 4 into ( .55),

                         [
                         尸


                         1


                         1


                         1




                                 2U l 0           dl n乙 l
                                                                0 1l
                                                                J
                                                                그
                                                                          nhh뇨
                                                                                                       e   m
                                                                                                               H




                                                                                                                   H
                                                                                                                   누




                                                                                                               H




                                                                                                       ]   ]
and obtain the following set of linear equations

                                                  H工1 e 工2+ 0 = 0
                                          H工1- 2工2 小 工3= 0                                                                  (2.57)

                                                          0- 工2 1 工3 = 0.

This is a linearly dependent set of algebraic equations. We assume thatxi =aand
obtain the eigenvector e3 corresponding to 尸 = 4 as

                                                            1
                                          a           -I        .           a ；亡 0.                                         (2.58)
                                                            1

The reader can compute the other two eigenvectors as an exercise.




                                              [
2.7.3   Linear Transformation
Using the example of the eigensystem in Section 2.7.2, we have



                                                      3l0 4         d2너       0 l 八4J
                                              e
                                  h


                                                          3
                                                      H




                             均                1
                                                                       forj = 1, 2, 3,
                                              L
                                              MATRIX ALGEBRA AND LINEAR TRANSFORMATION                                             21

and the eigenvectors corresponding to the eigenvalues are
                                                                                                                    m




                                                                                                                    1




                                                                                                                                位59)
                                =H
                 ei =     [i]        ,                    e2 =        [_         ],
                                                                                                            e3      1




                                                                                                                    L




From the definitions of eigenvalue and eigenfunction, we have

                                Ae/ = ／勻ej                                      for j = 1, 2, 3.                                (2.60)

We may rearrange this equation as

                        A [ei            e2          e3} = [/{1e1                            IL2e2               IL3e3}.        (2.61)

To be more concise, we put (2.61) into a more compact matrix form,




                                                                 miL m
                                                                  肛0
                                                                                      0 仰0
                                         E
                                         A                  E
                                                                                                                           1H


                                                                           0
                                                                                                   L003
                                                            E                                                              =
                                                                                                                                (2.62)

where /i is a diagonal matrix and E is the eigenmatrix. If the matrix E is nonsingular,
we diagona血e the i恤rix A by premu螂lying (2.62) by E小

                                                          E 'AE = p..                                                           (2.63)

Therefore, we have used the eigenmatrix E in a linear transformation to diagonalize
the matrix A.


2.7.4   Change of Basis

One may view the matrix A in the preceding example as a matrix that defines a linear
句毗em


                                                                                                   [
                                                                                                       l
                                                                                                   r
                                               1 1
                                                                                                       工

                                                  'l
                                                                                                   1
                                                                                        A                                       (2.64)
                                                                                                       ）口
                                                 Y2 =
                                                [Y
                                     Y=                                          =
                                                                                                       工
                                                                                                   1
                                                                           Ax
                                                                                                       n
                                                                                                       4U
                                                LY3J                                                   工




The matrix A is a transformation that maps x C R3 to y e R3. The components
of y are related to that of x via the linear transformation defined by (2.64). Since
el, e2, and e3 are linearly independent vectors, they may be used as a basis for R3.
Therefore, we may expand the vector x on this basis:

                                         x=          x;     ei   +x              e2+          x;
                                                                                                       e3
                                               = Ex',                                                                           (2.65)
22      入lATH타너ATICAL PREL小시NA뫼ES


and the coefficient vector x' is computed by

                                          x, = E노．                            伍66)

The new coordinates for the vector y with respect to this new basis ecome

                                         y/ = EH'y




                                                                              (2.67)

Equation (2.67) states that we have modified the linear system y = Ax by a change
of basis to another system, y' = p.x', in which the matrix 肛 is a diagonal matrix. We
call this linear transformation via the eigenmatrix the simiIariiy transformalion.


2.7.5    Hermitian Matrix, Unitary Matrix, and Orthogonal Tra sformation

Given a complex-valued matrix H, we can obtain its Hermitian,        h, by taking the
conjugate of the transpose of H, namely

                                          Hh :=斤.                             (2.68)

The two identities

                                  (Hh)       '   =   H

                                  (GH)' = HhGh

obviously follow from the definition.
   Let the basis vectors of an N-dimensional vector s mace be b1 i = 1, ... N
where b is itself a vector of length N. An o凡hogonal basis me. s that the inner
product of any two basis vectors vanishes:

                     (bj,b) = [b/ ] '[ bi] =하，j          Vi, j E 兀             (2.69)

For complex-valued basis vectors, the inner product is expressed b

                               (by, b』
                                     「) = [b1}' mi l.
If the norm of b1 is 1, this basis is called an o月honormal basis. We form an N x N
matrix of transformation P by putting the orthonormal vectors in a C八v as

                               P= [bi, b2. ... .bN] .                          (2.70)

Since

                                 [b/ ]' [b,] = 하, j,                           (2.71)
                                                                                                      DIGITAL SIGNALS      23

it 白lb꿔s that

                                                 php ==1                                                                (2.72)

and

                                             I小 == P니．                                                                  (2.73)

In addition to the column-wise orthonormality, if P also satisfies the row-wise or-
thonormality, PP' = I, matrix P is called a unitary (or or加normal) matri乂.


2.8     DIGlTAt SIGNALS

In this section we provide some basic notations and operations pertinent to signal
processing techniques. Details may be found in [3].


2.8.1    Sampling of Signal
Let x(r) be an energy-limited continuous-time (analog) signal. If we measure the
signal amplitude and record the result at a regular interval h, we have a discrete-time
signal

                     x(n) :=x (乙i) ,                          n= O, 1. .. ..N- i,                                       (2.74)

where

                                                 r7i= nh.

For simplicity in writing and convenience of computation, we use x(n) with the
sampling period h understood. These discretized sample values constit口te a signal,
called a digital signal.
   In order to have a good approximation to a continuous bandlimited function x (t)
from its samples {x (n)}, the sampling interval h must be chosen such that
                                                               兀
                                                     h <       -Th
                                                             H 52 '
where 252 is the bandwidth of the function x (t) [i.e., 分(w) = 0 for all w > f] . The
choice of h above is the Nyquist sampling rate, and the Shannon recovery formula



                           x   (t)   =
                                         n
                                             ;
                                             Z
                                                 x
                                                      (nh)
                                                                 Sm:

                                                                      'r   (t-
                                                                                 (t
                                                                                      -
                                                                                          nh)
                                                                                                nh)
                                                                                                                        (2.75)


enables us to rec' ivt r the original analog function.x(t). The proof of this theorem
is most easily carried out using the Fourier transform and Poisson's sum of Fourier
series. We shall defer this proof until Chapter 3.
24        入4ATH티너A기CAL PRE니N시NARIES

2.8.2      Linear Shift-Invariant Systems

Let us consider a system characterized by its impulse response h( ). We say that
the system is linearly shift invariant if the input x (n) and the output '(n) satisfy the
凡加Wi雎 system relations:
   Shift invariance:

                                              工（n) =＝수 y(n)
                                                                                                           (2.76)
                                              x(n - n') =수 y(n - n').

     Linearity:

                              xi(n) =＝斗 yi(n)                  and 工2(n) ＝斗 Y2(fl)
                                                                                                           (2.77)
                              x1(n) +mx2(n) ===: yi(n) +my2(n).

 In general, a linear shift-invariant system is characterized by

                  工1 (n - n') + 刃i工2(fl - n') ＝수 力（n 尸 n') +my2伽 H ').                                     (2.78)



" 2.8.3    Convolution

 Discrete convol.    ution,
                               also
                                    as moving averages,
                                      known
                                                                the      output re-
                                                                                 defines
                                                                                               input-
 lanonsnip or. a linear snirt-mvananr system. I ne matnematicai ueniiuun oi a jinear
 convojution is

                                              y (n) = h (n) 水 工（n)

                                                     = ＞二h(k - n）工（k)
                                                           k

                                                     =   ＞二工
                                                          k
                                                            （k- 九（k) n）
                                                                             .
                                                                                                            (2.79)



  We may express the convolution sum in matrix notation as


                                                                                                        工（-1)
        y (- l)
                              h(l)            h(0)       h(- l)    h(- 2)                               工（0)
        y (o)
                              h(2)            h(l)       h(0)      h(- l)   h(- 2)                      工（1)
        y (l)
                                              h(2)       h(l)      h(0)     h(- l)         h(- 2        工（2)
        y (2)


                                                                                                            (2.80)

                                                                      causal
  As an examp也 迂 h(n) = 吃 {, 未 {} and 工（n) = (1, 0, 1, 0, 1 0, 1) are
  sequences, the mathx equation for the input-output relations is
                                                                                                                                                                                                                                                                          DI(기TAL 듸GNALS                       25




                         그4l4l2l2l卜2l2l2l卞4l4 0 0e
                                                                      l



                                                                                           1
                                                                      U

                                                                               l
                                                                       4 1



                                                                                           l
                                                                               m

                                                                                            m
                                                                                4 l

                                                                                            4 l
                                                                                  14 l

                                                                                              e
                                                                         lm
                                                                          4



                                                                                               4 4
                                                                                     m4

                                                                                                 lH
                                                                                                  4 l
                                                                                                    m4
                                                                 그
                                                         m




                                                                                                                l
                                                                                                                14 l
                                                             4
                                                                                                                   44 1
                                                                                                                      1m
                                                                                                                       4 l
                                                                                                                         e4
                                                                                                                                                                                                                                                                   工（- 2) = 0




                                                                                                                                          l
                                                                                                                                          m4 l
                                                                                                                                             14 l
                                                                                                                                                中4 l
                                                                                                                                                   H4
                                                                                                                                                                                                                                                                   工（-1) = 0




                                                                                                                                                            1
                                                                                                                                                            1U
                                                                                                                                                             4 l
                                                                                                                                                               14 l
                                                                                                                                                                  14 l
                                                                                                                                                                                                                                                                   工（0) == l




                                                                                                                                                                     14
                                                                                                                                                                                                                                                                   兀（1) = 0




                                                                                                                                                                          l
                                                                                                                                                                          14 1
                                                                                                                                                                             l1
                                                                                                                                                                              4 l
                                                                                                                                                                                U4 l
                                                                                                                                                                                   m4
                                                                                                                                                                                                                                                                   工（2) = l




                                                                                                                                                                                             l
                                                                                                                                                                                             e4 l
                                                                                                                                                                                                14 1
                                                                                                                                                                                                   1竹
                                                                                                                                                                                                    4 1
                                                                                                                                                                                                      11
                                                                                                                                                                                                       4
                                                                                                                                    1 1

                                                                                                                                                                                                                                                                   x (3) =0   .                        (2.81)




                                                                                                                                                                                                                    l
                                                                                                                                                                                                                    14 l
                                                                                                                                                                                                                       U4 l
                                                                                                                                                                                                                          m4 l
                                                                                                                                                                                                                                                                   工（4) = l




                                                                                                                                                                                                                             m4
                                                                                                                                                                                                                                                                   工（5) = 0




                                                                                                                                                                                                                                             l
                                                                                                                                                                                                                                             小d
                                                                                                                                                                                                                                              1 ]
                                                                                                                                                                                                                                                H4 l
                                                                                                                                                                                                                                                   14 l
                                                                                                                                                                                                                                                      H4
                                                                                                                                                                                                                                                                   工（6) = l
                                                                                                                                                                                                                                                                   兀（7) := 0
                                                                                                                                                                                                                                                                   工（8) = 0

                                                     4
                                                                                                                                                                                                                                                    H




 The output signal is seen to be much smoother than the input signal. In fact, the
 output is very close to the average value of the input. We call this type of filter a
 S刃wothing or aver口ging filter. In signal processing tern琨 it is called a 勿刊刃口ss／汝er.
    On the 毗er hand, if the i呻ulse response of the filter is h的
                                                                    니｛, 글小 냑｝,
 we have a d｛和rentiating／끄把r or 肛脚兀issfi／招r. With the input signal 工（n) as be的re,
 the output signal is




                                                                       4 0 0
                                                     4 0 0


                                                                                4l 4 0 0
                                                                                                      4l
                                                                                  4l
                                                                                                   l    4 0 0
                                                                     4lH


                                                                                                   4l
                                                                                l
                                                                                                     4l
                                                                     l
                                                                     寸
                                                     l
                                                     4




        l
        卞
                                                                                                                                                        0 0 1
                                                                                                                              0 l



         4 l
                                                                                                                                H
                                                                                                                                4l



           1
                                                                                                                                  尸



            2 l
                                                                                                                                  4l
                                                                                                                                                            4l
                                                                                                                                    U
                                                                                                                                    4l



              U2 l
                                                                                                                                      e
                                                                                                                                      4 0 0
                                                                                                                                                                                                                                                                                                       1
                                                                                                                                                                                                                                                                                                       1
                                                                                                                                                                                                                                                                                                       H




                 中
                                                                                                                                                              4l

                  2 l
                                                                                                                                                               4l

                    H2 l2 l
                                                                                                                                                                 4 0 0

                          弓q l
                                                                                                                                                                                                                                                                                                           1
                                                                                                                                                                                                                                                                                                           1




                       1     4
                                                                                                                                                                           0 0 l

                              4 l
                                m4 0
                                                                                                                                                                               m
                                                                                                                                                                               4l1
                                                                                                                                                                                 4le
                                                                                                                                                                                   4l1
                                                                                                                                                                                     4 0 0
                                                                                                                                                                                                                                                                                           工（-2) = 0
                                                                                                                                                                                                                                                                                                                H
                                                                                                                                                                                                                                                                                                               1
                                                                                                                                                                                                                                                                                                               H




                                                                                                                                                                                                   0 0 i
                                                                                                                                                                                                       4l41
                                                                                                                                                                                                                                                                                           工（- 1) == 0




                                                                                                                                                                                                          4l4 0 0
                                                                                                                                                                                                                                                                                                           나
                                                                                                                                                                                                                                                                                                                    m




                                                                                                                                                                                                                                  0 0 l
                                                                                                                                                                                                                                                                                           工（0) = l




                                                                                                                                                                                                                                      卞
                                                                                                                                                                                                                                      4lH
                                                                                                                                                                                                                                        4l卞
                                                                                                                                                                                                                                          4l1
                                                                                                                                                                                                                                            4 0 0
                                                                                                                                                                                                                                                                                                                1       U
                                                                                                                                                                                                                                                                                                               1




                                                                                                                                                                                                                                                                                           兀（1) == 0




                                                                                                                                                                                                                                                           0 0 l
                                                                                                                                                                                                                                                               4l4l
                                                                                                                                                                                                                                                                  4l
                                                                                                                                                                                                                                                                                           工（2) = 1




                                                                                                                                                                                                                                                                    4 0
                                                                                                                                                                                                                                                                                                                    1
                                                                                                                                                                                                                                                                                                                            H




                                                                                                                                                                                                                                                                           0               工（3) = 0            H        中
                                                                                                                                                                                                                                                                                                                                =
                                                                                                                                                                                                                                                                                                                                1




                                                                                                                                                                                                                                                                           0 l
                                                                                                                                                                                                                                                                                           工（4) = l




                                                                                                                                                                                                                                                                             14 l4 l
                                                                                                                                                                                                                                                                                   小4 l
                                                                                                                                                                                                                                                                                                                            1




                                                                                                                                                                                                                                                                                           工（5) = 0




                                                                                                                                                                                                                                                                                      44
                                                                                                                                                                                                                                                                                           工（6) = l
                                                                                                                                                                                                                                                                                                               1                나




                                                                                                                                                                                                                                                                                           工（7) = 0
                                                                                                                                                                                                                                                                                           兀（8) = 0
        0
                                                                                                                                                                                                                                                                                                   4




                                                                                                                                                                                                                                                                                                   (2.82)
The oscillation in the input signal is allowed to pass through the filter, while the
average value (dc component) is rejected by this filter. This is evident from the near-
zero average of the output, while the average of the input is 글.

2.8.4                                  z-Transform
The z-transform is a very useful tool for discrete signal analysis. We will use it often
in derivations of the wavelet and filter bank algorithms. It is defined by the infinite
26      MATH티너ATICAL PREL小IINA뫼ES


sum

             H(z) = ＞二h (k）乙k
                           kEZ

                         = . .. , h(- l)zl + h(0) + h(l)z 1 + h(2)乙12 +                                                 (2.83)

The variable zel represents a delay of 1 unit of sampling interval; z_M means a
delay of M units. If one replaces z by eJ ', the z-transform becomes the discrete-
time Fourier transform, discussed in more detail in Chapter 3:

                           月（乙）z=e3'' = H(e/') = ＞二h(k)eH-"".                                                           (2.84)
                                                                                                      kEZ

We use these notations interchangeably in future discussions. One important property
of the 乙岫nsform is that the 乙岫ns的rm of a linear discrete cony아ution becomes a
product in the z-transform domain:

                          y(n) = h(n) *x(n) ='                                                    Y(z) = H(z)X(z).      位85)


2.8.5    Region of Convergence
The variable z in the z-transform is complex valued. The z-transform, X (z) =
工農小x(n)z小'2, may not converge for some values of z. The region of conver-
pence (ROC) of a z-transform indicates the region in the comple'c plane in which
all values of z make the z-transtorm converge. Iwo sequences may nave the same
z-仕anstorm but with ditterent regions ot convergence.

Example 1: Find the z-transform of x(n) = a'2 cos(won)u(n), where u(n) is the unit
step function, defined by

                                                 (4)          =                                   n> 0
                                                              =
                                                                                                  otherwise.
                                         8
                                         u       (n)                          1。
                                                                               11,   ,




SOLUTION: From the definition of z-transform, we have
                                    凹


               x   （乙）     =   ＞二口           ' cos                (c幻n)                  Ze   "



                                    m
                                                           eJ'0 + eeJr3
                           =                 "
                                                                              2                   Z   "
                               n=O
                               Z口
                           극匠（. ，的尸）
                                   ' 扈回M)"
                                - Ln=O                                                                    n=0

                                                                          1                                     1
                                    21   1             -    ae3빠- 1 +                                 1- 町佃z-       i
                                                         DI(고TAL 引GNALS   27



1.2




           x(n)




                  0
                                                           n n·．
                                                                n


                                            a
                                   O O O

       1
                                        1            1              1
      -5          0                    10           15              20

                                    Im(z)




             FIGURE 2.3   Sequence and ROC (a ＝二 0.9).
28      MATH티너ATICAL PREL小시NA뫼ES


                       1- 口 cos(wo）尸
                                                                                                           ROC: Izi > al .
                                                                                         '
                  1 尸 2口 cos (o幻）z寸l + 口2乙-2

The case where a = 0.9 and wo = 10r is shown in Figure 2.3.
  枷ec洌 C口se工‘

     1. Ifa= landw0= 0, we have

                                                                     1 - ze'
                          r / rn-
                          나 小／              1 中 2z 1 + 乙小2

                                                                                                  ROC니기＞ \
                                                l-
                                                                             '
                                            1
                                                                             ;!
                                                                         -
                                                                1,
                                       =
                                                            -        z

     2. Ifa= 1, wehave

                  lr r7\ -    1 小 cos(o幻）z-1
                                                                                                       1         ROC: IzI> 1.
                  " ' 勺" - 1- 2cos(o幻）z中l +ze

     3. Ifwo= 0, wehave

                                                                     1 尸 (7之-1
                          Yr口＼ H
                          " \q/ - 1 - 2az 1 + 口2之-2
                                           1
                                                                                                  ROC: IzI > Ia I .
                                      - 1- az11


2.8.6    Inverse z-Transform

The formula for recovering the original sequence from its z-transforn involves corn-
plex integration of the form


                            x
                                (n)
                                           ==        2rj/
                                                                                  ,!(:
                                                                                             ):
                                                                                                   '       "市，
                                                                                                                                     (2.86)


 where the contour is taken within the ROC of the transform in the counterciock-
 wise direction4 For the purpose of this book, we shall not use (2.86) to recover the
 sequence. Since the signals and filters that are of interest in this book are rational
 functions of z. it is more convenient to use partial fractions or long division to re-
 cover tne sequence.

Example 2: Determine the sequence x (n) corresponding to                                                                     如ilowing 乙‘
transform

                    z- 1                           乙 -l
        X (기= .    n =. '             . =. =  n   . ,,   』＼』1.                                                      ROC         > 1.2.
              (Z 小 U.／八z -            l. Z)  之乙 - 1.！妃 + U. 54
                                                                                        EXERCISES      29

SOLUTION: Using long division, we have

            ,, . .   -1 . n n 卜） . n n거 각 . 0.897C2 - 0.7308z日
            A （乙) = z 十 u.yz 十 (ia3 IZ 十
                                              乙2- l.9z+ 0.84   "
Obviously, x (0) = 0, x(l) = 1, x (2) = 0.9, x (3) = 0.87. .. .
                                                                .x (n) is a right-sided
infinite sequence since the ROC is outside a circle of radius
                                                              r = 1.2.
   If ROC: zl < 0.7, x(n) is a left-sided sequence. We
                                                         obtain

            -           -i+ z           1      1 7.     l.9 '
         X (Z) ==     n     ,,   八 = 4: =H + :=H 1 l = :== 1 Z + · · ·
                    U.84- 1.9z+ 之乙    U.84   U.84 \    U. 54J
using long division. The sequence {x(n)) becomes a
                                                     sequence of ascending pow-
ers of z and is a left-sided sequence where x (0) = -1/
                                                        0.84 = -1.19, x(- 1) =
1/0.84(1 - 1.9/0.84) = -1.5, x(- 2)



2.9   EXERCISES

1. Let u = (- 4, -5) and v = (12, 20) be two vectors
                                                       in the two-dimensional
   space. Find -5u, 3u + 2v, -v, and u + v. For arbitrar
                                                        y a, b E R, show that
   IauI+ Ib미 三 Iau+ b미．

2. Expand the function f (t) = sin t in the polyno
                                                   mial basis set {t', }n =
   0, 1, 2, . . . Is this an orthogonal set?

3. The following three vectors form a basis set: ei
                                                      = (1, 2, 1); e2 = (1, 0, -2);
   e3 = (0, 4, 5). Is this an orthonormal basis? If not, form
                                                              an orthonormal basis
   t뇨ough a linear combination of ej, k = 1, 2, 3.

4. Let ej = (1, 0) and e2 = (0, 1) be the unit vectors
                                                           of a two-dimensional
   Euclidean space. Let x1 = (2, 3) and x2 = (- 1, 2)
                                                          be the unit vector of a
   nonorthogonal basis. If the coordinates of a point
                                                      w are (3, 1) with respect to
   the Euclidean space, determine the coordinates of the
                                                         point with respect to the
   nonorthogonal coordinate basis.

5. Let ei = (0.5, 0.5) and e2 = (0, -1) be a biortho
                                                     gonal basis. Determine the
   dual of this basis.

6. Sh。
     w that if
                    La2l
                    [all
                           a121    1bi1
                           a22j LZ72J
                                          =
                                                   LC2I
                                                   [cii
                                                                C121
                                                               C22J 尸2J
                                                                       1띠   f。
                                                                                 r all biand b-,    then
  A = C.


                              A=
                                     [二
                                          :   ],
                                                          B=
                                                               [;2
                                                                       1]


  Form (AB)Tand BTAT, and verify that these are the same.
                                                          Also check if AB is
  equal to BA.
30           人4ATHEMATICAL PREL小시NA뫼ES



7. Find the eigenvalues and the eigenvectors for matrix A.



                                                                 尸11L
                                                                   八4V dl 0
                                                                                         0 八乙
                                                                              l n乙 n乙
                      1




                          =
                                                  A

                                                                                        3

           恥fin 血e tra耐orm m如xPw址ch m山es 尸 'AP a diagon기 matrix.

 8. Find the convolution of x(n) and D2(n) where

                                   x(n) =(l, 3, 0, 2, 4) forn= 0, l, 2, 3, 4

           and D2(n) is given in (2.45). Plot x(n) and h(n) = x(n) * D2 n) as sequences
           of n.

 9. Find the z-transform of the following sequences and determine the ROC for each
    of them:
                                 n> 0
    (a) 工（n) ==
                                 n <0.
                                                1 <n <m
           (b) 工（n) =                           m +1 <n <2m - 1
                              0,
                                                otherwise.
10. Find the z-transfonn of the system function for the following小screte systems:
    (a) y(n) = 3工（n) -5工（n- i) + 工(n -3)
           (b) y(n) =48(n) - 118(n- 1) +58(n- 4),where

                                                                                        n= 1
                                                6(n)
                                                                                        otherwise.
                                                       =
                                                           {::
REFERENCES

1. E. A. Guillemin, The Mathematics of Circuit Analysis. New York: John Wiley & Sons,
   1949.
2.   Ben
               and James W.
              Noble               Applied Linear Algebra. Upper
                                      Daniel,
                                                                          River,    : Preil-         Sadd걱e   N.
                                                                                                                   J.
   tice Hall, 1988.
3. A. V. Oppenheim and R. W. Schafer, Discrete- flme Signal Processing. Upper Saddle River,
   N.J.: Prentice Hall. 1989.
CHAPTER THREE




Fourier Analysis

Since the days of Joseph Fourier, his analysis has been used in all branches of engi-
neering science and some areas of social science. Simply stated, the Fourier meth以
is the most powerful technique for signal analysis. It transforms the signal from one
domain to another domain in which many characteristics of the signal are revealed.
0ne usually refers to this transform domain as the叩'ettra/ or frequency domain,
while the domain of the original signal is usually the .tJne- oi 8palial domain. The
Fourier analysis includes both the Fourier transform (or Fourier integral) and the
Fourier series. The Fourier transform is applicable to functions that are defined on
the real line, while the Fourier series is used to analyze functions that are periodic.
Since wavelet analysis is similar to Fourier analysis in many aspects, the pur叩se of
this chapter is to provide readers with an overview of Fourier analysis from a sig-
nal analysis point of view without going into the mathematical details. Most of the
mathematical identities and properties are stated without proof.


3.1    FOURIER SERIES

Fourier series and Fourier transform are often separately treated by mathematicians
since they involve two different classes of functions. However, engineers have al-
ways been taught that Fourier transform is an extension of Fourier series by allowing
the period T of a periodic function to approach infinity. We will follow this route
by discussing Fourier series first. The Fourier series representation of a real-valued
periodic function p(t) [p(t) = p(r + T)1 is given by
                                         的

                               p(t) =   ＞二    qkejk的'
                                                                                 (3.1)


with

                            따나／,"""p(t)eU'蜘'小                                    (3.2)


                                                                                    31
 32      FOU뫼ER ANALY듸S

 where aj are the Fourier coefficients and the period T = 2ir/wo with wo being
 the fu磁mental frequency. The set of functions {ek } = {e3k(0t }, k E Z, forms a
 complete orthogonal basis in L2[to, t0 + T]; that is,
                                                      t0+ T

                                                              eketdt = T8k,t.
                                            t。


The coefficient ai written in the form of an inner product,


                                            .，극如／'미，                                                          (3.3)

represents the orthogonal component of the function p(t) in k따）. Hence the Fourier
series is an orthogonal expansion of p(t) with respect to the basis set {ek}. The
representation in (3.1) is exact. However, if we truncate the series to, say, 士N terms
(k = -N. ... .N), there will be some error. As described in Section 2.6, being
orthogonal projections, the Fourier coefficients minimize the mean square of such
error,
   A Fourier series may be represented in other forms. Representation using sine and
cosine functions is given by


                   p(t)＝譽＋＞二（aj cosk蜘i+ bk sink蜘i),                                                           (3.4)
                                   iU            k=
                                                          l
in which the aj and bk are real quantities. Complex representation using only positive
harmonics is written as
                                                               的


                                        =                 +＞二ck cos (k口幻t+ 6k)                                (3.5)
                                                           k=1
                         p
                             (r)
                                            Co
with
                                                      小                      아            니
                                                                                          帥
                                                                                                      r
                                                                                                          1
                                                                                                          師
                     ICkI = \／口｛ +b自                                    ek == tan ' ( -；二 1 ,     1
                                                                                                          m   (3.6)
                                                                                              \
where Ck = lck I eJ80 are complex quantities. Computation formulas for ak and bk are

                                                      2 1T
                                   aj =           -   T jI p(t) cosk蜘tdt                                      (3.   7)
                                   6*                 2       fT
                                   bk =                            p
                                                                       (t)
                                                                             sirik蜘tdr.
                                                                                                              (3.8)

3.2     EXAMPLES

3.2.1    Rectified Sine Wave
Consider a function p (t) = sin t1 as shown in Figure 3.1 with the period T = ir and
coo = 2ir/ T = 2 rad/s. Since the function p(t) is an even function with respect to
                                                                                                                  태AMPLES      33




          -Jr                                 0                                          7r

                                          FIGURE 3.1 Rectified sine wave.


t = 0 [i.e., p(- t) = p(t)], bk = 0 for all k. The coefficients tak) are computed as


                   .나            jJ。
                                   'Jr             sintcos2k                  《小

                                                                              2k)t卄小2枷］ dt
                        =   1
                                          "   帥-
                            Jr
                                 J。
                                                                                                   [ 出： ］
                                      (
                                 1 lcos(l- 2k뇨
                                 7r L  1- 2k                                     ",］그，                   ""'   k)t。
                                 4   1
                                                                                                                             (3.9)
                        -        jr4k2- 1'

Hence the Fourier series of p(t) is given as

                                                                    L
                                                                    2         '+
                                                                              4 oo
                                                                                         毗               l
                                  p(t) = ;= 규 2日 倂 1 l cos 2kt.                               八乙


                                                                               Ic=1


3.2.2     Comb Function and the Fourier Series Kernel KN(t)
In this examole we want to find the Fourier series of a oeriodic imoulse train [i.e.. a
periodic train of the delta function' b(t)j. We write the impulse train with period TI
as
                                                                                00

                                                               Ir   (t)   =    ＞二 8(t-
                                                                              n=-oo
                                                                                                   nT)
                                                                          ＝    乶         akeuI )0t                          (3.10)



    tThis is not a function in the classical sense. It is called a generalizedfunction or distribution. However,
in this book, we refer to 山is as a delt口和nc加n.
 34     FOURIER ANALYSIS

 The Fourier coefficients are given by

                             1 r T/2 1즈1                                           ,, .
                      qk = 卞 /           ' 2. 8(t - nT)e刀' 叩' dt.                                                 (3.11)
                           i   JHr/ Z 7i뇨；)O

 Since the only n that is within the range of integration is n = 0, we find that

                                 aj＝          二
                                              I
                                                  ,              k E Z.

Therefore, the Fourier series expansion of an impulse train 'T (t) is written as


                               1T(t)극，身""'                                                                        (3.12)

It is instructive to examine the behavior of a truncated version                                       (3.12)．七印工舟和）
be the (2N + 1)-term finite Fourier sum of JT (t):

                                                  ]         쓰
                              KN   (t)
                                          =       卞 >;
                                                  m k=-싸
                                                                  6jk的
                                                                          '   ·
                                                                                                                  (3.13)

尺iq'(t) is known as the 只가4?初r sei韶辛kerne1. 가re geometric se ies sum in (3.13) is
carried out to give

                                          1 sin伽+ 뇨幻t
                            KM('t'= m                  ' .   .: .
                             " "    T                 sin(wot/2)
A graph of KN(t) for N = 4 is given in Figure 3.2. We also co巾pute the kernel for
N = 10 and N = 15 but find that the shape of the kernel does no change except that
the oscillation frequency is correspondingly increased for higher values of N. The
main lobes (main peaks) of the graph become narrower as the value of N increases.
The oscillation characteristic of KN(t) contributes to the Gibbs phenomenon, to be
discussed later. These oscillation patterns can be modified by weighting the ampli-
tudes of the coefficients in (3.12). This is a common practice in antenna array de-
sign [1].



                                         KN(t)




                                                            /\                    ／入           \   J              \
                                                      \.-
                                                                         1             .   /              .   /

                      FIGURE 3.2 Fourier series kernel KN(t).
                                                                                      FOURIER TRANSFORM          35




                                                                      ]
                                     /\        /   \                                                 /\




                  -3T                          卄T                0         T                     3T
                                       FIGURE 3.3 Comb function.


   Since KN (t) is periodic, we only need to consider the behavior of the kernel
within the interval [-T/ 2, T/2]. It is clear that t/ sin(wot/2) is bounded in the in-
terval [-T/ 2, T/2] and sin(N + { )wot/ t approaches 8(t) as N tends to infinity [2].
Hence

                                 N-*。。KN(f) = 8(t),
                                  urn                                           ItI         T1
                                                                                             2            <
                                                                                                          H
This procedure is applied to all other intervals [(2k + l) (T/2)], k e 7Z, and the result
is that

                            lim KN(t) = IT(t) = )小8(r -kT) .                                                  (3.14)
                        N-           以）                                   卜너
                                                                          kE也


Jhe impulse tr缸n of (3.12) is called the comb function in the engineering literature
[3] (see Figure 3.3).
   Several important properties of Fourier series, such as Poisson's sum formula,
partial sum, and sampling theorem, require the use of Fourier transform for efficient
derivation. We consider these topics later in this chapter.


3.3   FOURIER TRANSFORM

To extend the Fourier series to Fourier transform, let us consider (3.1) and (3.2).
   The time function p(t) in (3.1) can be expressed using (3.2) as

                                 四        r1   r T/2                              .   ]
                      ,k ？기社,,/2,p(t')e '的"dt' 1e3'蜘'
                     二＝ n    m
                            -=   .

                                     小1 1m                 1                          - j


                            I             0O           I       戶T/2                              1

                    =; .＞二미／',T,I),p(t')e "蜘" dt' k"'蜘'·
                                     k= -的
                                                                                                              (3.15)


We extend the period T to infinity so that c幻 approaches dw and kw0 approaches w.
The summation in (3.15) becomes an integral,
36     FOU뫼ER ANALYS巧

                               i        f아그 r 尸)0           .    . ./          .]   .
                  p(t)＝石t的［J-的p(t')e"-' " dt'j"" dw.                                    (3.16)

The integral inside the brackets is represented by a function p(w):


                                   万（0)   =       /：「  （! 戶" 'dt ',
                                                            '）                          (3.17)

and (3.16) becomes

                               p(t) = J. -- 尸 餉押dw.                                     (3.18)
                                              乙Jr j1 (:K)


Equations (3.17) and (3.18) are known as the 只兀trier trc가呵O刀n／兀功r.
    From here on we use f (t) to represent a time-domain function, while p(t) is re-
stricted to representing periodic time functions. Let's rewrite (3.17) in new notation.
    The Fourier transform of a finite-energy function f (t) E L2(R) of a real variable
t is defined by the integral


                           ．       加）         =   /:/（加-         iw   '   小·
                                                                                        (3.19)

In inner product notation, described in Chapter 2, the Fourier transform can also be
expressed as


                                        f妗니附『j"）·                                       (3.20)

We should emphasize the fact that f (w) is a complex-valued fun tion that can be
expressed in terms of amplitude and phase by

                                        夙이 늬f佃）1ej中佃）.                                  (3.21)

However, th帥iappin只 f如nil妃 如main 可 fO) to that of f (a力 is 'rom R t。            IR (i.e..
irom the t-axis to the w-axis), even though thle real-valued tunctioti J (t) is mapped
to a complex-val出d fin毗油if (o小
 八The interpretation of (3.20) is very important. This equation states that for an 口!,
f (coi) represents the component of f (t) at cot. If we can determine all the compo-
nents of f (t) on the co-axis, a supe叩osition of these components should give back
(reconstruct) the original function f (t):


                                      2,r f：加) ejO)tdw.
                               f(t) = --,                                               (3.22)
Hence (3.22) can be viewed as a superposition integral that produces f (t) from its
components. The integral is referred to as the inverse Fourier tran母orm of f (w). If
the va契ble t represents time, f (co) is called the spectrum of f (t). If t represents
spac已八叫 is called the sj）口ti口／spectru刃1.
                                                             PROPERTIES OF THE FOURIER TRANSFORM                                                                        37

  The Fourier transform is very important in the development of wavelet analysis
and will be used often in subsequent chapters. We will use it as an example to present
some of the properties of the 8-function.
  Let us recall that
                                   戶的

                                   /      f (t) 8(t - y) dt = f (y).                                                                                               (3.23)
                              1/   m的
Consequently, the Fourier transform of 8(t),
                                         1'的

                         8佃）= /                 8(t) e寸jm'dt =e+j的＝1.                                                                                              (3.24)
                                        J -00


From the inverse transform of 8(w), the identity
                                                              1          1' 的
                                        8(t) =                - J       ejmrdw                                                                                     (3.25)
                                                             乙7r .／寸（)0
is established. The inverse transform in (3.22) can now be shown to be

                 1 ／的 升'w) ej0' dw = J. . ／的 .J帥dw ／的 f(t') e.'d' dt'
             2r 上的 " "                                  乙．Jr 工아）                                                      上的 " "


                                            =           굶           f_    的
                                                                          。。           f(t   ')
                                                                                                         J-
                                                                                                              I       CO    ej   (
                                                                                                                                     (t_   t ')   dwdt '
                                                             I. 的

                                                                         f (t 8(t ')                -             t   ')   dt ' =          f (t)   .




                                            =           f_     m


Since the烏m佃枉mmrn帥4de,we may write

                                                    f (r) ＜수 f (w),
meaning that for each function f (t) there is a unique Fourier transform correspond-
ing to that function, and vice versa.


3.4        PROPERTIES OF THE FOURIER TRANSFORM

Since the focus of this chapter is not a detailed exposition of the Fourier analysis,
only the pro比rties that 缸e relevant to wavelet analysis will be discussed.


3.4.1       linearity

If f (t) = au (t) + fif2(t) for some constants a and fi, the Fourier transform

      加）     =    /:/(! ）戶" dt=                 ./:f1                       (t)         e_        .10)        t       dt『月／                ：力          （加-   iou   』！
             = a f (w) + 月 九（U小                                                                                                                                    (3.26)

The extension of (3.26) to the finite sum of functions is trivial.
38                FOURIER ANALYSIS


3.4.2             Time Shifting and lime Scaling
Let the function f (t) be shifted by an 카llount to. The spectrum is changed by a phase
shift.        the spectrum of the shifted function
        Indeed,
                                                              f (t ' " ) expressed by                     fo       (t)        :=
                                                                                                                                                    -           is
                               r （乂                                                                   /1的                                   '           "

                      fo(w) = f             f (t - t0) eHJO)t dt = /                                                     f (u) e1Jm("+'0) du
                              J 100                                                              d =1叩


                            = e_3 t呼佃）늬／佃기小小加'이                                                                                                                          (3.27)

where中(w) is the phase of the original function f (t). The magnitud루of the.spectrum
remains uncnangea tar a snirtea signal. I ne snirnng is incorporat디a into me pnase
term or me spectrum.                                        .                            ,        .            .   .               ,.   ,       .       .   1        ,




     Let a be a nonzero constant; tne spectrum or Ja (t) :== j tar) is gven Dy


                                  五   （w)       :/:f                     (at)      e     ""  '            幽                                                              (3.28)


                                                =               /:f      (u）戶" ' "                    "                  嶝）
                                                                                                                                                                         (3.29)


                                               姑硝）·                                                                                                                      (3.30)

Depending on whether ais greater or .smaller than 1, the spectruIi is expanded or
contractea, respectively. we snail see tins important property occur rrequenuy jater
in the development of wavelet analysis.


3.4.3             Frequency Shifting and Frequency Scaling
The results for frequency shifting and scaling follow in a similar 申ay. If fo(w) :=
fl th - wo),then

                                                            f0(t) = f (t)eJW0i,                                                                                          (3.31)

and if 五(w) := f (aw) for a nonzero value of a, then


                                                            石（!)＝누（計                                                                                                     (3.32)


3.4.4 Moments
The nth-order moment of a function is defined as

                                                       M
                                                       m:
                                                                :=
                                                                     =
                                                                         J
                                                                         g00
                                                                               t
                                                                                   '1f       (t) dt.                                                                     (3.33)

The first-order moment,
                                                                   PROPERTIES OF THE FOURIER TRANSFORM                                             39



                 M1=     /:  -    t f (t) dt
                                 。。                =        (      'j)         -   '   dw   Jo0                       f (t)   e_   t   dt w=O

                         .    .. . Hl df (n)
                     =                                                                                                                          (3.34)
                             _J)       dw
                                                            w=O

    The extension of this formula to the nth-order moment results in

                                                                   j) _fl d'7f(w)                                                               位35)
                                      M, = (_
                                                                            aw"
                                                                                                               w=O


/

    3.4.5   Convolution
    The convolution of two functions fi (t) and f2(t) is defined by

                                      /（    =

                                                                              （力力（!
                                       《）
                                                       p:
                                                       -    。。           fi
                                                                                                      -        ,）力·
                                                                                                                                                (3.36)


    We write (3.36) symbolically by

                                                 f (t) = f1(t) 永 力(t).                                                                          (3.37)

    Notice that if f2(t) is 6 (t), the convolution integral recovers the function fj (t). It is
    well known that a linear system represented symbolically by the block dia酊am in
    Figure 3.4 has the input-output relation given by

                                                 O(t) = h(t) * i (t),                                                                           (3.38)

    where h(t) is the system response function. Hence if i (t) is a delta function, the
    output function O(t) is the same as h(t). For an arbitrary input function f (t) the
    convolution integral

                                      .(!
                                      O(r) =
                                            ):
                                                            J
                                                            p00

                                                             -。。              h(r) i (t           -       r)          dt                        (3.39)


                                                                                                                         O(t)
                                                                              九（t)


                                                                                                                        力（t)
                                                                              h(t)

                                       FIGURE 3.4 Linear system.
40      FO（外IER ANALY듸S

represents a superposition of the output due to a series of input delta functions whose
amplitudes are modulated by the mput signal. It is easy to show that the spectral
domain representation of the convolution integral of (3.36) is given by

                                                                五요址二小 佃汀k功．

3.4.6    Parseval's Theorem
Parseval 's theorem states that

                            乙f(t)I2 dt= },/:m빼' 如·                                                                                           (3.40)

Two functions, f (t) and g(t), are related to their Fourier transfo                                                               炙w) an嬉(w)
via the Parseval's identity for Fourier transform, given as

                                              (f (t), 的）) = .1-.(／佃）, 會佃）).                                                                  (3.41)
                                                                                 乙Jr

This can be shown from
                                          "’ 『              C0O
               '"
               (f(t)
                                                   J f (t)                      g(t.)dr
                                      '
                                           )=
                   'n
                        ,   g
                                (t)
                                                            -   。O




                                                       '"「‘ da))""了
                                                            1


                                              =J괸亡
                                                                                                  ,,   .   -




                                              ＝石t的／(w)
                                                     (t的g(t)eJ'' dt中
                                               긍，/：加豕w) dw
                                               =   },（炙a)
                                                                           )，    會（w)   )·
                                                                                                                                             (3.42)

In particular, with g(t) = f (t), we get Parseval's theorem, given in (3.40). Equa-
tion (3.40) is a statement about the energy content in the signal. It 욕tates that the total
energy computed in the time-domain [f         以t) 2 dt] is equal t+) the total energy
                                          .                          ..   .八     .   戶00     公.    . 12        1   1   1=m1   뇨      .   .
computed in me spectral ciomain L(l/ Z7r) J1凹 1f (w) J awj. lflek'arseval theorem
allows the energy of the signal to be considered in either the spec仁al domain or the
time domain and can be interchanged between domains for conv텨nience of compu-
tation.


3.5     EXAMPLES OF THE FOURIER TRANSFORM

We evaluate the Fourier transforms of several functions that will occur frequently in
various applications. For this purpose we may use the definition given in Section 3.4
directly or use the properties of Fourier transform.
                                                                 EXAMPLES OF THE FOURIER TRANSFORM            41


                     r (t)                                                                     p（口）)




        -T       0                T

               FIGURE 3.5 Rectangular pulse and its Fourier transform.


3.5.1    Rectangular Pulse

The rectangular pulse (Figure 3.5), r (t), is defined by

                                      r (t) = u(t + T) - u(t - T)                                          (3.43)
                                                             ,            띠<T
                                                                                                           (3.44)
                                                 1。
                                                  (1,
                                                                          otherwise.

We obtain

             1(w)    =     /：「        （!   ）戶"          山＝          ／『，
                                                                             e j 'r dt = 2T sinwT
                                                                                            wT    "
                                                                                                           (3.45)

The function (sin wT)/wT, called the sinc function, is the Fourier transform of a
rectangular pulse. We remark here that for T = {, the function i (t 나）= X[o,I)(t)
is called the characteristic function or-.thefirstor4er B-spline. This is an important
function to remember and will be recalled later in the development of wavelet theory.


3.5.2    Triangular Pulse
By convolving two rectangular pulses, we obtain a triangular pulse (Figure 3.6),
which is expressed by

                         Tr (t)                                                                 Tr   (W)
               FIGURE 3.6 Triangular function and its Fourier transform.
42      FOU뫼ER ANALY引S


                            乙（t) = r (t) 水 r (t)                                                                                                             (3.46)



                                            I" ("슭）, " 」'<"
                                                     2T           (i峙）                                ,
                                                                                                                             -2T <t <0

                                                                                                                                                             (3.47)

                                       기        1 0,                                                                         otherwise.

By the convolution theorem we have

                                                                             =
                                                                                 f2TsincoT\ 2
                                                                                                                                                             (3.48)
                                                       (0)
                                                 Tr
                                                                                 \
                                                 t
                                                       (w)                   =            wT
                                                                                          sin2
                                                                                 4T2                                                                         (3.49)
                                                                             =
                                                                                                      (wT)2
                                                                                                          (wT)
If T = {,




                                       T(t）小，!: 烈<e1."
                                                     ]2.
                                                                                                                                                             (3.50)



and乙(w) , =    [sin    /(w/2) The triangular
                      (w/
                              2)
                                                              T = .    called,the                                function.
                                                                                                                                    with
                                                                                                                                                   1/
                                                                                                                                                        2,
secona-oraer Ii-spune, piays an important rote as a seating runcuon 01 tne spiine
wavelet.


3.5.3   Gaussian Function
The Gaussian function.is one of the most important functions in probability theory
and,tfle,analysis of random signals. It plays a. central role.in the (iPbor transform, to
oe ueveiopeu later. t ne uaussian runction wiw UfliL amptituac is e休presseu as

                                                                                    可節．
                                                                             g(t) =                                                                          (3.51)

百（n))can be computed easily as


                                                m m的 m
                             a     m
                                                                                 泂
                                                                                 2
                                                                                 可                        m



                                                n／工 n
                                                    /11
                                                      卜
                                                                                                          加
                                                                                 라        泂                                                k   山
                                                                                                          규
                                                                                                          呻




                                       =   e'          2     '니                      e_
                                                                                               att+              j (0)1h12 dt


                                                                                                                                                             位52)
                                       규                     『           ‘   " ／佃·
                                                                         POISSON'S SUM   43


                       g(t)




-10                0                        10                     -5
                FIGURE 3.7 Gaussian function and its Fourier transfonn.


    It is interesting to note that the Fourier transform of a Gaussian function is also a
Gaussian function. The waveform and its 打ansform 町e shown in Figure 3.7,
    The parameter a can be used to control the width of the Gaussian pulse. It is
evident from (3.51) and (3.52) that a large value of a produces a narrow pulse, but
its spectrum spreads wider on the w-axis.


3.6   POISSON'S SUM

We now return to the Fourier series and discuss Poisson's sum, whose derivation
is made much simpler by using some properties of the Fourier transform. In many
applications it is necess出y to form a periodic function from a nonperiodic function
with finite energy for the purpose of analysis.
   Poisson's sum formula is useful in relating the time-domain information of such
a function with its spectrum. Let f (t) e L2低). The periodic version of 1 (t), called
 f7(t), is obtained tly
                                                       的

                                  f (t) := ＞二 f (t + 2兀n),                           (3.53)
                                                 n==1的

where we have assumed T = 2兀 to be the period of f (t). Consequently, 口加 =
2r/ T = 1, and the Fourier series representation of f7(t) is

                                                            的
                                                                ckejkt
                                        ／汁）= ＞二                                      (3.54)
                                                       k＝卜이）

with the coefficient ck given by



                    q
                    Ck = 2,
                          Ir  -    J2
                                        "   fp
                                                 (t)
                                                       e_
                                                            Itdt


                        =긍，p2,
                           J。r:;f(t + 27rn)eU" dt
                                            nEZ
 44     FOURIER ANALYS巧




                             =
                                 枉；
                                                  [2r f(t         + 2jrn)e      '"    dt
                                      ]           p2兀伽＋1)
                             = ;：스j. /                            /（亨）e小jk（盲-2兀n)d已                    位55)
                               bJT；昆 J27r7i

where a change of variable 盲 = t + 2兀n has been used. Since the summation and
the inte肛ation limits effectively extend the integration over the entire real line R, we
may write


                                      Ck긍，              /:／町八갸
                                                                                                       (3.56)
                                            긍，
                                                    f
                                                        (k)   ,


where the definition of the Fourier transform has been used.                                  mbining (3.53),
(3.54), and (3.56), we have Poisson 's sum formula,


                         易f(t+刎三加少"·
                     J , '= -cU
                                                                                                       (3.57)

                                                                                           陋八（ {m蜘，付
                                                                       lc=-oo    -'

For an 缸bitrary pe加d T, the formula is generalized to


                    ，툐／('「"'）나，且m蜘）""'的'·
                         的                                1        的

                                                                                                       (3.58)


If g(t) is a scaled version of f (r), that is,

                                          g(t) = f (at),                a > 0,                         (3.59)

we have

                                                 百（co)=누（斗                                             (3.60)

Poisson's sum formula for f (at) is


                    多 /(at + 2ran) =二 多 小）
                   n=-뇨                                   乙Jr口 k=：뇨              ＼口／
                                                                                                      位61)

If at is renamed as t, we have

                    으으                                        1        으으    = /L\

                 ，互／(t + 2,ran) =旒，툐兀)"""'"·                                                          位62)

Two other forms of Po.isson's sum will be needed for derivations i!i subsequent sec-
lions. Ifley are statea flere witnout prool. 1fle proots are lent as ex牟rclses.
                                                                                                    POISSON'S SUM       45

                                Z／佃＋2兀k) =＞二只枷小m                                                                    (3.63)
                                kEZ                                   kEZ



                                       w +2兀k '
                                          a                      =              f (ak)        j*0                   (3.64)
                                              /                       i昆
                                                                      51.
                                                                                         e-
 3.6.1      Partition of Unity
  A direct consequence of Poisson's sum is that a basis may be found so that unity is.
. expressed as a linear sum of the hasit . We call this property the partition Qf tinily.
  Let a be l/ 2ir in (3.62). Poisson's sum formula becomes


                                                                                                                    (3.65)


 if the spectrum of a function f (t) E L2(R) is such that

                                f (2Jrk) -_ 8o,k                        forkEZ,                                     (3.66)

 that is,

                                                      f (0) = 1

 and

                                f (27rk) =O                      keZ\ {0} ,

it follows from (3.65) that


                                           Z f (t十n）三1.                                                             (3.67)
                                       neZ

The first and second orders of B-splines are good exa끄［lples of functions satisfying
比Li5 pr아：erty.

Firs卜Order B햐line

                               Ni(t) := X[O,1)(t)

                                                  j
                                 （0)
                                       =
                                            /,1
                           N1    (w)
                                       =               e-
                                                            '"
                                                                     dt
                                            J。                                  '
                           而
                                                                            =
                                                                                    J(i)
                           ／卜           l 小 rJ口J
                           N1(O) =lirn      .    =1
                                   w-+0    JO)
                        Ni(2,rk) =0,                             kcZ\ {0}.
46           FOURIER ANALYSIS

Hence

                                               ＞二Ni(t +k) 三 1.                                              位68)


Second-Order B-Spline

                                    N2(t) = N1(t) * N1(t)                                                   (3.69)
                                                 It,                                           te[ 0, l)
                                               = 12- t,                                        tEtl, 2)     (3.70)
                                                 10,                                           otherwise.

From the convolution property, we have

                                          忍（m) =［刃l(n)
                                                  i (w)]2                                                   (3.71)
                                                                                                    2
                                                                      /1_
                                                                                   ,jw\
                                                                                                            (3.72)
                                                                               e_
                                         N2
                                               (0)       =
                                                                              )Ct)
                                          刃2
                                               (w)       =           (\
Again, we find here that

                                         N2(0) = 1                                                          (3.73)

                                    N2(2兀k) = 0,                                    k e Z \ {0J.            (3.74)

Consequently, N2 (t) also satisfies the conditions for partition of nity. In fact, from
the recursive relation of the B-spline,

                                    Nm(t) = Nm_ i (t) * Ni(t)                                               (3.75)


                                                     =   IJ。' Nm_              1          (t   -
                                                                                                            (3.76)


we    have    Nm     [(1-
                   (w)   =      ／加中，
                               e_    J   ')   sati呱es the requirel巾町아partition可
                                                             which
umty. Hence 莎splmes 01 arbitr町y orders all have ma印ro꺄rty.（可叩lii아"U없rations
for the partition of unity are shown in Figure 3.8.


3.7          SA人4PIJNG THEORE入4

The sampling theorem is funda毗ntally import帥 to digital signal analysis. It states
that if a signal f (t) is bandlimited with bandwidth 2f2, the signal f (t) ca가 b re-
constructed exactly from its sampled values at equidistant grid points. The distance
between adjacent sample points, called the sampling period h, should not exceed
兀/ 52. The function f (t) is recovered by using the formula


                             /（《）＝工／(k九）
                                       "'"［巴뿌， kz·
                                    ICE乙                                  "                     "
                                                                                                            位77)
                                                                                        SA入4PL小dG THEORE人4       47




                       N1(t +2)                                      N1(t)         N1(t- 1)




                   -
                       2                                   0                      1           2



               N2(t+ 3)                                                         N2(c)    N2(t - 1)



                   -2              -1                      0                      1
                               FIGURE 3.8 Partition of unity.




Ifh == 兀／ 2, the sampling frequency /; = 1/h = 52／兀 is called the 的們務ig比．
Theoretically, f (t) can always be reconstructed perfectly from samples if h < 7r/ 52.
In practice, however, we cannot recover f (t) without error due to the infinite nature
of the sinc function.
   Let f (co) be the Fourier transform of f (t):


                                   f (w) = /                f (t)e4j 't dt.

The integral can be approximated using Simpson's rule as

                        ／佃）믄 F(co) = 九＞二／(k九）e'j0k方·                                                         (3.78)
                                                            kEZ

Using Poisson's sum formula in (3.64), we can rewrite F (w) as


                       F(co)   ＝
                                    方＞
                                         kEZ
                                              二／(k九） j!     e'
                                                                       )z



                                    rA 公／a沆 + 2irk\
                               =    ) / 1 .       1              ,

                                    m1=         '                n          I
                                    KE乙             \                    /




                           ：加）七2;‘，小*쑤）·                ICE乙＼'U,
                                                                                                             (3.79)


Hence F(co) contains f (w) plus infinitely many copies of f (w) shifted along the
co-axis. In order for /（口i) to be dis如恤edw油 its copies, the amount of shi此 2'r／瓦
48     FOURIER ANALYSIS




                                                            (a)
                                                                                    S   >




  --1/1\
                                    -
                                        /
                                              c
                                                            (b)
                                                                      \        52

FIGURE 3.9 (a) Undersampling (S = 22r/ h <2Q); (b) oversampling ( = 2ir/ h > 入2).


must be at least 252 (see Figure 3.9); that is,


                                    쭈之22, 』」舌                                               (3.80)

To recover the original function, we introduce a spectral window

                                                                                            (3.81)
                                                                          wi
                                                  =               t
                                  t " .', ,, J,V냠                         otherwise
                                        （m)           !!,
                             i回
and recover f (w) by

                                              f (w) = F(w) W(w).                            (3.82)

From the convolution theorem we obtain f (t):

                                              f (t) = F(t) * W(r).                          位83)

Since 功七） == sin Qt/irt is well known, we compute F(t) from tl忙 inverse Fourier
transform


                       F(t) =士 [:i;
                                 kEZf (kh)e_3 0)e"t dw
                           금구町：
                              「’""'""' dw
                            = hZ f (kh)8(t - kh),
                                        kEZ
                                                                                            位84)
                                              PARTIAL SUM AND THE GIBBS PHENOMENON       49


 where we have used (3.25). The function f (t) is recovered by using the convolution
 如rn叱la


                   f(t)＝九＞二／（丸九）
                              ／巴8（
                            kE石
                                 【－k九）W(r-!)dr     1r H1入J



                        = 九Zf(k硼(t 나幻
                            kEZ



                        --hi;
                           kEZf(kh)S jr(
                                    1努tt-kh)
                                         값)]
                          乞f(k九）
                               "『" 二巴‘끼                                              (3.85)
                          尤e乙


 where we have used 5 Zh = jr. We remark here that (3.85) represents an interpolation
 formula. Since sin[Q(t 卞 kh)]/[Q(t - kh)] is unity at t = kh and zero at all other
 sampling points, the function value at kh is not influenced by other sampled values:


                        f (k九） = YT f (k力）竺쁘 = /（砒）.          U
                                                                                     (3.86)
                                        尤e心
                                        !1=
Hence the function f (t) is reconstructed through interpolation of its sampled values
with the sinc function as the interpolation kernel.



3.8   PARTIAL SUM AND THE GIBBS PHENOMENON

The partial sum of a Fourier series is a least-square-error approximation to the orig-
inal periodic function. ;Let pM(t) be the (2M + 1)-term partial sum of the Fourier
series of a periodic function p(t) with period T:

                                                     M
                             PM   (t)
                                               =   ＞二
                                                   k=＝牛4f
                                                             口kej"的' ,           (3.87)


with the Fourier coefficients given by

                                  i            pT/2
                          aj = 幸 /                     p(t)e卞jk的idt.             (3.88)
                                              J- T/2

Putting ak back into (3.87), we have the partial sum

                          끄  l1 pT/2
                  PM(t) = ＞二 솎 /     p(r)e_ j '蜘' ej '的tdt.                      (3.89)
                           k二初 '               J- T/2

0n interchanging the order of summation and integration, we obtain
50     FOURIER ANALYSIS

                          1 r T/2     ，쓰 ， .. -
                 PM(t) = ; /      p(r) 九 e/ ' 蜘'' H" dr
                          ' J-T12     k三二M
                            1 (T12 . . sin(M +去）(r - r)wo
                         = ;; I   pl.t)        -. 1.. -            drk            (3.90)
                           I 卜T/2              sin흐U- TJ(iJ0

which is the convolution between the orginial periodic function with the Fourier
series kernel discussed in Section 3.2.2. We can easily see that the oscillatory char-
acteristic of KN is carried into the partial sum. If p(t) is a rectangular pulse train or
a periodic function with jump discontinuities, the partial Fourier series will exhibit
oscillation around the discontinuities. This is known as the Gibbs phenomenon. The
percentage of overshoot remains constant regardless of the number of terms taken
for the approximation. As M - 的, the sum converges to the i寸dpoint at the dis-
continuity [4].



3.9   FOURIER ANALYSIS OF DISCRETE-TIME SIGNALS

Since computation of Fourier series coefficients and Fourier trans百orm requires inte-
gration, the function must be describable analytically by elementary functions such
as sine and cosine functions, exponential functions, and terms from a power series.
In general, most signals we encounter in real life are not representable by elementary
functions. We must use numerical algorithms to compute the spectrum. If the signals
缸e sampled signals, the discrete Fourier series and discrete-time Fourier transform
are computable directly. They produce an approximate spectrum of the original ana-
log s培nal.


3.9.1 Discrete Fourier Basis and Discrete Fourier Series
恥ra 昏yen pe加dic sequence with pe加d奴ty N, we have

                          f7(n +mN) = f (n),           mE Z.                      (3.91)

기le Fourier basis f야 this 꺄加小c sequence has only N basis 血n tions, namely,

                   e (n) = e (127r">",         k= 0, 1, .. .,N- 1                 (3.92)

We can easily show the perio小city of the basis set

                                               (k+N)n
                               ek+N = e(/ 2兀／N)

                                      = ej · ej2兀n
                                      = ek                                        (3.93)
                                               FOURIER ANALYS巧 （그F ［긔SCRETE-T小任 引GNALS                                  51

since ej2兀" = 1 for integer n. Therefore, the expansion of f (n) is in the fonn


                               f (n) = ＞二 crkek(n)                                                                   (3.94)
                                                      k=0
                                                      N-i
                                                = Zqke(j2" /N)k",                                                    (3.95)
                                                      k=0

and then we can compute the coefficients by

                                                                                 1P1) hi)
                          .*=
                                                                eO2
                                                (n)         ,
                                 (fp
                                                산二l

                               ＝方2; f,(n）寸j21rk/N) ?1
                                           1
                                                                                                                     位96)
                                       "        片＝0



Equations (3.94) 缸ld (3.96) form a transform pair for discrete periodic sequences and
their discrete spectra. It is quite easy to see from (3.96) that the Fourier coefficients
{ak} 町e also periodic with N.

                               (yk= ak+mN,                                             m e 7L,

万뇨1J까刃el: Find the恥urier ser妃s coeffic妃nts for the sequence

                                       f (n)          =         cos      (-   ./jrn)          .




SOLUTION: The given sequence is not a periodic sequence since we cannot find an
integer N such that f (n + N) = f (n). Consequently, f (n) does not have a discrete
Fou加r series representation.

Example 2: Find the Fourier series representation of

   (a) f (n) = cos(n7r/5), and
   (b) f (n) = {1, l, 0, 0}.

SOLUTION:

   (a) Instead of computing the coefficients direcfly using (3.96), we may represent
       the cosine function in its exponential form,


                            f (n)          =    ;     (e1
                                                                      (2"h10)h2 +         e
                                                                                                  f (2
                                                                                                     "h10)   h1) ·
                                                                                                                     (3.97)

        The peri에icity of this sequence is seen as N = 10. Since (3.97) is already in
        the form of an exponential series as in (3.95), we conclude that
52      FOURIER ANALYSIS


                                                     2
                                                                      k 二＝ 1

                                      aj =                            k= 9                                   (3.98)
                                                    。'   2'   '


                                                                      otherwise.

     (b) We compute the Fourier coefficients using (3.96) to obt曲

                       .1=       (i     +   e_    1(2/4)1o) ,                  k=   0,   1,   2,   3.
         We have

                                                                           k= 0
                                                                      D
                                                                           k= l
                                 (yk                                                                         (3.99)
                                                                           k= 2

                                                                           k =3.

The sequence and its magnitude spectrum are shown in Figure 3.1


3.9.2    Discrete-Time Fourier Transform
If a discrete signal is aperiodic, we may consider it to be a periodic 1 ignal with period
N = oo. In this case we extend the discrete Fourier series analys s to the discrete-
time Fourier transform (DTFT), similar to the extension in the a ialog domain. In
DT工 the time variable (n) is discretized while the frequency va iable (co) is con-
伽riuous since

                                八co= uirn ？쯔나CL).
                                                 N-+oo N

The DTFT pair is given explicitly by
                                                                  的

                                      1w) = Z f(n)eU' m
                                                   n =＝小的

                                            1      r7r 八
                             f (n) =        -     I    f (w)eJ'n'dc入
                                         b7       J17r


Example 3: Determine the spectrum of the exponential sequence

                /（川＝口fl,              VneZ+ := {0, 1, . . . },                           I'기 <          1.
SOLUTION: Using (3.100) yields
                                                     m

                                      f (w) 스그"rj "m
                                                   n=o
                          FOURIER ANALYS巴 OF ［기SCRE丁E-TIME 듸GNALS            53




   1(B      O




 0.8



트0.6



 0.4



 0.2



   0。
             1           2                3      4           5           6
                                          n
                                    (a)
  0.6



  0,5&



  0.4
             0


  0.3



  0.2



  0.1



                          을               k
                                                  4           5          6

                                    (b)
   FIGURE 3.10   (a) Sequency f (n) and (b) its magnitude spectrum ak卜
54      FOURIER ANALYSIS


                                                   的


                                             =    ＞二
                                                  n=0
                                                            （口eHjm)                 "


                                                       I
                                                                                                     (3.102)
                                                  1 1 (aeHftJ) "
We have p이nted out in Chapter 2如t the I玎FT can be的tainedf蜘n the乙-tra耐orm
by replacing the variable z with eJc. For this example the z-岫ns如rm is


                                   F   （之）         =        ）二a           "    之-   n




                                                  스걋戶）"
                                                                          1
                                                  11- （毗小 "
Therefore, replacing the variable z with e3口J yields

                       「（:  ）낳汭＝                       ,.              (',,   ．加）       ＝   加）   ·




The z-transform F(乙) and the DTFT [f (w) = F(Z)I牛ejw] will bc
ably in future derivations and discussions of wavelet construction


3.10    DISCRETE FOURIER TRANSFORM

The integral in the inverse DT江 discussed in Section 3.9 must be evaluated to re-
cover the original discrete-time signal. Instead of evaluating the integral, we can
obtain a good approximation by a 小scretization on the frequencyt(w) axis.
    Since the function f (t) is bandlimited (if it is not, we      it so by passing
it through a lowpass filter with sufficiently large width), w       to discretize the
interval [-52, 52] only, namely
                              27rn                                         N         N
                        (z뇨 = 丙i,                                                                    (3.103)
                                                                      n = 1了，" " " , 三
The integral in (3.19) can now be approximated as a series sum, namely
                                       N-i
                     ／佃n) 斗 九 Z ／位枷如' 肋 = 町佃，                                                        (3.104)
                                       k=0

where
                                             N- 1

                           f (n) = 兄 /(k枷小2砒" /N).                                                   (3.105)
                                                 k=0
                                                                  EXERCISES    55

We ca毗asily verify that evaluation of the discrete Fourier transform using (3.105)
is an O(N2) process. We can compute the discrete Fourier transform (DFT) with an
 O (N log2 N) operation with the well-known algorithm of thefast Fourier transform
(FFT). One of the commonly used FF1' algorithms is that of Danielson and Lanczos,
according to which, assuming N to be such that it is continuously divisible by 2, a
DFT of data length N can be written as a sum of two discrete Fourier transforms,
each of length N/2. This process can be used recursively until we arrive at the D可
of only two data points. This is known as the radix-2 FF1 ' algorithm. Without get-
ting into many details of the algorithm, w址ch the interested reader can obtain from
many excellent books available on these topics, we simply mention here that by ap-
propriately arranging the data of leng仕 N, where N is an integer power of 2 (known
as decimation-in-time and decimation-in-frequency arrangements), we can compute
the discrete Fourier transform in an O (N log2 N) operation. If N is not an integer
power of 2, we can always make it so by padding the data sequence with zeros.


3.11   EXERCISES

1. Verify that the order of taking the complex conjugate and the Fourier transform
   of a function f e L2(- oo, 以）) can be reversed as follows:
                                        ==             大
                                        F（功 = F(- ?7)

   for any q ER.
2. Check that the condition


                                    知        （   (0)   뇨이＝0
   is equivalent to the moment condition


                                        /:P少（!         ）小却
   白r any posi山이nteger number j.
3. Show that the Dirichlet kernel


                   D (u）극（二喀cosku）之盆咨
   Plot the kernel forn = 6.
4. Find the Fourier series of f (t) = ej工t, 17r <t <ir, and T = 27r.
5. Determine the energy-normalized constant A of the Gaussian function g( (t) =
   Ae寸'2 and derive the expression of the Fourier transform.
56     FOU끼ER ANALYS巧

6. Ex把nd Poisso心 없nll 化rmula t叩rbitr缸ype加d T.

7. Derive the following Poisson's sum formulas in the spectral domain:

                            Z／佃＋2兀k) = Z f(k)e 'km
                             k                   k


                      誨1(w +2Jrk)＝쭈／（毗）
                                     「 "'
REFERENCES

1. R. S. Elliott, The Theory ofAntenn口Arr口ys. Vol. 2o태刃cro叩口ye Sc口n蜘g Antenna了, R. C.
   Hansen (Ed.). San Diego, Calif.: Academic Press, 1966.
2. A. Papoulis, The Fourier Integral and Its Applications. New York: 枷Graw-Hi1l Book
   Company, 1962.
3. K. lizuka, Engineering Optics, 2nd ed. New York: Springer-Verlag, 1986.
4. W. W. Harman and D. W. Lvtle. Electrical and Mechanical Networks. An Intmduction to
   The加An口加is. New York: 入4cGraw-Hi끄 Book Compa파，1962.
 CHAPTER FOUR




 Time-Frequency Analysis

  We summarized the Fourier analysis rather briefly in Chapter 3 to refresh the memory
  of the reader and to point out a few important concepts in the analysis that will be
  useful when we discuss 山ne-frequency analysis. We observe from the definition
  of the Fourier transform (3.19) that the integration cannot be carried out until the
  entire waveform in the whole of the real line (- o기 oc) is known. This is because the
- functions ei'r or cos wt and sin wt are global functions. By this we mean that a sm出l
  perturbation of the function at any point along the t-axis influences every point on
  the w-axis, and vice versa. If we imagine the signal f (t) as the modulating function
  for ej 'i, a perturbation at any point on the t-axis will propagate through the entire
  w-axis. A叩ther observation we make on the Fourier transform is that the integral
  can be evaluated at only one frequency at a time. 가is is quite inconvenient from a
  signal processing point of view. Although there are fast algorithms to compute the
  transform digitally,' it cannot be carried out in real time. All necess쾨y data must be
  5啣ed in the mem야yb可아e the discrete or fast F叩加r transform can be co叫川ted.
      Although unquestionably the most versatile method, Fourier analysis becomes in-
  adequate when one is interested in the local frequency Contents of a signal. In other
  words, the Fourier spectrum does not provide any time-domain i寸ormation about the
 브肛旦l. To demonstrate this point, let us examine the function shown in Figure 4.la,
  which represents a truncated sinusoid of frequency 4 Hz in the time domain with
  perturbations near t = 0.7 and t = 1.3 s. We have seen in Chapter 3 that a sinusoid
  in the time domain will appear as a delta function in the frequency domain, and vice
  versa. Observe that the frequency spread near 4 Hz in Figure 4.lb is due to trunca-
  tion of the sinusoid. We conclude from the Fourier spectrum shown in Figure 4.lb
  that the sharp pulse near 4 Hz comes pri刃iarily from the sinusoid of 4 Hz, and the
  small ripples that appear throughout the frequency axis are due primarily to some
  delta functions (sh缸p changes) in the time domain. However, we are unable to point
  Out the locations of these delta functions in the 血ne axis by observing the spec-
  trum of Figure 4.lb. This can be explained simply by the Fourier representation of
  a delta function (3.25). The delta function requires an infinite number of sinusoidal
  functions that combine constructively at t = 0 while interfering with one another de-

                                                                                     57
 58         TIME-FREQUENCY ANALYSIS




                      I      1        I           I    t    I    1     1          1       1

                                                      1.2       1.4   1.6       1.8      2
                                            (a)
   1-
 0.8

 0.6

 0.4

 0.2
  뇨小뇨，
     小小小 r卜1小：
        0
             나口口      5               10          15              20              25
                                          (b)
 FIGURE 4.1 (a) Sinusoid signal with perturbation at t = 0.7 and t = 1.3, and (b) its
 magnitude spectrum.


 structively to produce zero at all points t 尹 0. This shows the ex1 eme cumbersome-
 ness and ineffectiveness of using global functions e30)t to repres/ nt local functions.
 To correct this deficiency, a local analysis is needed to combine both the time- and
 frequency-domain analyses to achieve time-frequency analysis, 1y means of which
 we can extract the local frequency contents of a signal. This is vi1 important, since
 in practice we may be interested in some particular portion of the spec打um only and,
 therefore, we may like to know which portion of the time-domai signal is primarily
 responsible for a given characteristic in the spectrum.
    Conimon sense dictates that to know the local frequency cont " nts of a signal, we
 should first "remove" the portion desired from the signal give and then take the
 Fourier transform of the part removed. Such a time-fre. uenc anal sis method is
m브쁘쁘뜨뾰加序加e tour玘r trans枷n (S"1'FT5犯ef아e we discuss STFT, let us
 discuss the notion of window function, by means of which the desired portion of a
 given signal can be removed.


  4.1       WINDOW FUNCTION

  A desired portion of a signal can be removed from the main s              by multiplying
  the original signal by another function, which is zero outside            nterval desired.
                                                                                                   ＼사八DO＼사 FUNC기ON        59




                                       m




                                      mr                           0                           r
                               FIGURE 4.2 Characteristic function.


Let 中(t) e L2(IR) be a real-valued window function. Then the product f (t)中(t 中
b) =: fb(t) will contain the information of f (t) near t = b. In particular, if 中(t) =
X[1r,r)(r),as shown in Figure 4.2, then

                                                         (r)        tE[ b-               b+
                                                                                                                     (4.
                                (t)
                                           -   {f
                                                               .                T,
                                                                                                                          1)
                          fb
                                                                                                   r)
                                           -        。,
                                                                   。therwise.
 By changing the parameter b we can slide the window function along the time axis
 to analyze the local behavior of the function f (t) in different intervals.
    The two most important parameters for a window function are its center and
 width; the latter is usually twice the radius. It is clear that the center and the standard
 width of the window function in Figure 4.2 are 0 and 2r, respectively. For a general
,window function砂 (t), we define its center t ' 4＼卄en汭 ybi乍e
                                                         1         . 的

                                      r ' := -I          t中(t)I2dt                                                   (4.2)
                                             'I中lIe J-oo
and the root-mean-square (RMS) radius i中 as

                              1 rr0o       -      il/ 2
                      스小 := /, . I / (t -尸）2岫(t)尸小1 .                                                                (4.3)
                            IIQI1 LJ-oo           J
恥r the p缸ticular window of 恥毗 4.2, it is easy to verify that t水 = 0 and 스中 =
r/ J. Therefore, the RMS width is smaller than the standard width by 1/ J.
    The funct帥 中(t) descr小ed above 뼛th fim把 스中 is called a time 叩地O比 跏II-
larly, we can have a frequency window中(w) with'center w' and the RMS radius스多
defined analogous to (4.2) and (4.3) as
                                                                                                                               V
                               0 ' ：卄／                             ：이0叫              '   dw,
                                                                                                                     (4.4)
                                                                                                                      V
60      TIME-FREQUENCY ANALYSIS



                   '幷由比（0)- " )' 巨(w)I2dwJ
                                        r, .oo                                              기112
                                                                                                   (4.5)


As we luiow, theoretically a function cannot be limited in time and frequency simul-
taneouslv. However, we c띠l have 小(fl such that both 스小 and 스了 are both finite; in
such a case the tunction 中(t) is called a time-frequency winaow. It is easy to venry
that for the window of Figure 4.2, c戶 = 0 and 스中 = OO. This window is the best
(ideal) time window but the worst (unacceptable) frequency window.
   A figure of merit for the time-frequency window is its time-frequency-width
pr어iuct A中스多， which is bounded from below by the uncertainty principle and is
given by


                                            A皿8之｛                     ,                            (4.6)

where the equality holds only when 中 is of the Gaussian type (see Section 3.5.3).



4.2   SHORT-TIME FOURIER TRANSFORM

In the beginning of this chapter we indicated that we could obtain the approximate
freciuencv contents of a signal f (t) in the neighborhood of some desired location
in time, say t = b, by first windowing the tunction usmg an appropnate window
function 中(t) to produce the windowed function fb(t) = f (t)中(t - b) and then tak-
ing the.Fourier transform of fb(t).This is the short-time Fourier transform (STFT).
rormally,. we can denne me sii可i. or a runduon j (t) wirn resp4ct to me winuow
lunction q (t) evaluated at tne location (b, 亐) in me ume-trequency piane as
                                         亨）                    00

                        아／(b,                                                         di'
                                                    :=
                          (5， )
                         G,
                              ,f                    :=         。。   f (r)中b,t   (t)
                                                                                                   (4.7)


where

                                       仍,的）:= 中(t 4戶和．                                             (4.8)

The window function 中(t) in (4.7) is allowed to be complex and atisfies the condi-
tion


                                   8   (.)=              /‘，   中（t)dt尹『

In other words, 中(a) behaves as 孕lowpass filter. That is, the spectrum is nonzero at
co= 0. Because of the windowing nature of the STFF, this transform is also referred
to as the 岫m가ved Four油 片an町O刀n or running-wine加叩 只冗srier tran蜘nfl
   Unlike the case of Fourier transform, in which the function f (t) must be known
bOr the entire time axis betore its spectral component at any sing埠 frequency can be
                                                                                  SHORT-TIME FOURIER TRANSFORM                        61

 computed, STFF needs to know f (t) only in the interval in which 中(t- b) is nonzero.
 In other words, G4,f (b, ) gives the approximate spectrum off near t = b.
    If the window function 砂 (t - b) in (4.7) is considered as the modulating function
 of the sinusoid e_ jtt , the STFF can be written as


                         아f (b，亨）                         =
                                                              (/
                                                                   (! 中（t b)
                                                                        )，
                                                                                        -       e-
                                                                                                     '盲
                                                                                                          '）
                                                                                                               ·
                                                                                                                                    (4功
 The function 中b,亨(t) = 中(t - b)eJ亨t behaves like a packet of waves, where the sinu-
 soidal wave oscillates inside the envelope function 中(t). In addition, (4.8) indicates
 that each of these packets of waves behaves like a basis function, so that the STFT
 may be ii吐e叩reted as the coi叩onents of 山帥inc如nf(t) wi吐i respect to this basis
 in the time-frequency plane.


 4.2.1   Inversion Formula
One can recover the time function fb(t) by taking the inverse Fourier transform of
(G中／)(b, 亨）:


                九(t) 如(t - b)f(t)＝츤／已M냐小d.                         乙J
                                                                                                                                  (4.10)
                                                                                  J니刃



The original f (t) is obtained by multiplying (4.10) with 中(t - b) and integrating
with respect to b. The final recovery formula is


            f (t) = 2, II; )H                           de1
                                                                    '                G, (b, 亨)中(t                      b)         (4.11)
                                                                                                                            db.
                                              j:
                                                                             /:
                                                                                                                   -
                                                                                            f
                              (r
                                         J-
                                                   。。


One may observe a similar symmetric property between (4.7) and (4.11), and that of
the Fourier transforms in (3.19) and (3.22).


4.2.2    Gabor Transform
The Gabor transform was developed by D. Gabor [1], who used the Gaussian func-
tion

                                         =                          ／知，
                                                                   '"
                                                                                            a> 0                                  (4.12)
                                   (t)
                                                   +-
                          枷
as the window function. The Fourier transform of (4.12) is

                                   la(a) =e出m2,                                      a > 0.                                       (4.13)

The window property of gq(t) can be computed using the formulas in Section 4.1 to
멉ye t' = U戶 = 0, 스g口 = ＼厄，and 스哀r = 1/긱厄．Observe that A枷 스瓦 = 0.5
attains the lower bound of the unce月ainty principle.
62            TIME-FREQUENCY ANALYSIS

4.2.3 lime-Frequency Window
Let us consider the window function 中(t) in (4.7). If t ' is the center and A中 the
radius of the window function, then (4.7) gives the information of the function f (t)
in the time win血川：

                                               [r ' +b1A中，r ' +b+ A中］.                          (4.14)

To derive the corresponding window in the frequency domain, app'y Parseval's iden-
血y (3.41) to (4.7). We have


                                   Gf
                                          (b, 亨）   =   /:f (t   (t   -   b)   e_
                                                                                   jlt dt       (4.15)


                                               ＝和Jtbf：加加小’"‘油
                                                   =e"3盲' ［炙0)）쥼(二；]' (b),                      (4.16)


where the symb이 " V" represents由帥싸erse Fourier빳耐毗i. Observe that (4.15)
has a fo맷 5帥1町 to (4.7). If cv' is 仕比 此nter and 스中 is the radi뺏可 如 w岫ow
function 中(w), then (4.15) gives us information about the function f (w) in the inter-
val

                                              [n)' ＋盲中A8, a)' 卄＋A司．                             (4.17)

Because of the similarity of representations in (4.7) and (4.15), the ST可 gives in-
formation about the function f (t) in the time-frequency window:

                               [r* +b - A中，r ' +b+ A中］ >< [n)' ＋盲1스8, m' 卄＋A可．                  (4.18)

Figure 4.3 represents 肛aphically the notion of the time-frequency window given by
(4.17). Here we have assumed that t求 = nJ木 = 0.



4.   2.   4   .   Properties             of STFT                                            .




LineariTy . Le.t f. t) =. a力(t) + 戶j2(t) ne a.linear c인PDma9 or two tunctions
fj (t) ana 52t) witn weigflts a ana p ineepenaent ott. m1len me b It'! O1 J it),

                                        아f (b, 亨） = 口（G中／D(b, 亨） + 月（G中／))(b, 盲）                (4.19)

is the linear sum of the ST可 of the individual function. Hence STFF is a linear
transformation.
                                                  SHOR下T小4E FOU뫼ER TRANSFORM               63



     U)



                                                                        2A中


                                                                                 2Aa
                                                 2八中


                                                                2A多
                       2A砂


                         기
                                      2八a

                                                                         1
                                                                         1


                                                                             勿
                         b0                        bl                                  t
 FIGURE 4.3 Time-frequency window for short-time Fourier transform (t* = n戶 = 0).




Time Shift Letting f0(t) = f (t 尸 to), then


              아九（b，亨）         /:/(!
                              =             -   !.）中（t-   b）    戶" dr


                             J    -   00
                                      。。／（啣＋

                              = eHj亨i0 (G巾／)(b- to膺）.
                                                               枷) tte-J 0 dt
                                                                                       (4.20)

Equation (4.20) simply means that if the original function f (t) is shift- 1 by an
amount t0 in the time axis, the location of ST可 in the time-frequency 4 omain
will shift by the same amount in time while the frequency location will remain un-
changed. Apart from the change in position, there is also a change in the phase of the
STFT which is directly proportional to the time shift.

Frequency Shift Letting f (t) be the modulation function of a carrier sign1 ej的1
sucn wai

                                      九(t) = f (t)／呵·,                                 (4.21)

then the STFT of f0(t) is given by
64      TIME-FREQUENCY ANALYSIS


                  아／b(b考）      =    /:f    (t)e"的'中（       『－               b)e " ' 』！

                               = 아f (b, 盲 -wo)·                                          他22)

Equation (4.22) implies that both the magnitude and phase of the ST丁 of f0(t)
remain the same as those of f (t), except that the new location in the t-a domain is
shifted along the frequency axis by the carrier frequency c幻.



4.3     DISCRETE SHORT-TIME FOURIER TRANSFORM

Similar to the discussion of Section 3.10, we can efficiently evaluate the integral of
(4力 as a series sum by appropriately sampling the function f (t) and the window
function 砂(t). In its discrete form, the short-time Fourier transform can be repre-
sented as
                                       N小 l
                   아f (b丙）勺九Z八加(tk4加-J亨" " ,                                             (4.23)
                                       k=O

where

                                   = kh,       k = 0. . ...N - 1                         (4.24)

and

                                                       N
                                                                                N
                         冬, = 2프프．                                              2
                                                                                m
                                                                                         (4.25)
                           "  Nh '            n=   小   三   '    "   "   "   '




In particular, when h = 1, we have


                   Gt,f (n, n小 Z f (k欣卜 毗寸21rkn/N)·                                      (4.26)



4.3.1    Examples of STFT
We use an example similar to the one used in [2] to show the computation of the
ST江 and the effect of the window width with respect to resolution. The signal

             f (t) = sin2兀vit + 5in27rv2t + K [8(t - t1) + 8 (t - t2)]                   (4.27)

consists of two sinusoids at frequencies of vi = 500 Hz and 1)2 = 1000 Hz and
two delta functions occurring at t1 = 192 and t2 = 196 ms. We arbitrarily choose
K = 3. We apply a rectangular window to the function and compute the STFT for
four different window sizes. The signal and the window function are both sampled
at 8 kHz. The window size varies from 16 to 2 ms and the corresponding number
                                                                                    DISCRETE GABOR REPRESENTATION                                65


                       2

                       ]




 따 U 그 t C O 0 >
                       0


                       너



                       2       1 1 1 I I I 1 l i i i 1 l i i   i111l ii i1l i i i 11i j11I11I I I 1I II111       1 1 1 1 I I 1 l i i i   I I I

                           0                      512           1024             1536                                                     2048
                   -
                                                                                                             1
                                           Time index (8000 samples/sec; 1 unit = 0.125msec)
                                      FIGURE 4.4 Signal for which the STFF is shown in Figure 4.5.

of samples in the windows are 128, 64, 32, and 16, respectively. Since 1 e delta
functions are separated by 32 samples, window sizes equal to or 肛eater ' an 32
samples are not narrow enough to resolve the delta functions.
    To corn멕te the STFT, we apply the I下T algorithm to th叩ro加아 可thesi: ial and
the window function. We compute a 128-point FF1' each time the window is moved
to the right by one sample. Figure 4.4 shows the function f (t), and the re.ults of
these STFTs are given in Figure 4.5.
   Initially, when the time window is wide, the delta functions are not resol able at
all. However, the two frequencies are well distinguished by the high resolution of
the window in the spectral domain. As the window size gets smaller, we begin to see
the two delta functions while the frequency resolution progressively worsen$. At a
window size of 16 samples we can distinguish the delta functions quite eas1y, but
the two frequencies cannot be resolved accurately. To resolve events in the fre自uency
and time axes, we must compute the STF1' every time we change the window size.
Computation load is a serious issue in using STFT for signal processing.




「「芬云三am
 ：      (4.28)
66        TIME-FREQUENCY ANALYSIS


2000

                                         2스中 = 16 msec
1500


1000


 500


     0
      0              0.05           0.1              0.15             0.2

2000


1500
                                         2스中 = 8 msec

1000


 500


     0
      0             0.05            01               0.15             0.2

2000


1500                                     2A4 = 4 msec

1000


 500



                    0.05            0.1             0.15              0.2

2000


1500                                     2스中 = 2 msec

1000


 500

                                     1                  1          II
                    的5              0.1             0.15              0.2

FIGURE 4.5 STFF of signal shown in Figure 4.4 with di且erent window width (2스中); hori-
zontal axis is time (second) and the vertical axis is frequency (Hz).
                                                              CONTINUOUS WAVELET TRANSFORM                                     67


for -的5 b,흐 < 的.. The Gabor transform is dense over the t-f plane. Corip,u.t.atio,n
ioau ior we ( iaDor .ffansrorrn in 呼．m았.is quite neavy. we may, insteaa I ('hZo).,
compute me aiscreuzea version ot ('f.zo). i nat is, we compute呼.zO) omy私 a set oi
points on me r- j plane:
                               數）
                                               /
                                      =            '00

                   吼／(5.
                     (bn,，
                   Ggaf
                                      =                  f(t)           ga
                                                                                 (t         -   bn)
                                                                                                           e_   j "t   dt
                                          J
                                4k)
                                               -    。。



                                      =   (1        (t)   ,   ga
                                                                   (t
                                                                             -        bn)
                                                                                                  eilkt)
                                      = (f(t), Pn,k(t)).                                                                    (4.29)

The last expression of,.(4.29) is the inner product of the function with the function
中n,k(l) =g口．(i - b71)e" ' . m'ne function f (t) maybe recovered under the쩍CStX1Cted
condition Lii                                                               I

                          f (t) = Zn Z吼f (b耐加a(t b加亨"·                                                                      (4.30)
                                      k

Equation (4.30) is known as the Gabor expansion, in which (Ggf) (bn, k)
role of coefficients in the recovery formula

                            f(t) = ZZ아.加규k)4n,k(t).                                                                         (4.31)
                                      n        k

The function 中n,k(t) is a Gaussian-modulated sinusoid. Spread of the function is
controlled by a, while the oscillation frequency is controlled by 盲k. These "bullets"
of the r- f olane form the basis of the Gabor exnansion. Since the Gaussian function
nas tne minimum size or a time-rreuuencv winaow. it nas tne ni으nest concentration
oi energy in tue r- r plane. mne uaoor Dasis Pn.klj) appears to ne a usenii pasis ror
signal renresentation. However, it lacks basic nroner口es such as orthogonalltv. corn-
Dieteness. and indenendence needed to achieve simnie renresentations and emcient
computation.



4.5   CONTINUOUS WAVEIET TRANSFORM

The STFF discussed in Section 4.4 provides one of many ways to generate' a time-
freauencv analysis of signals. Another linear transform that urovides such analv-
ses is the inte으ra1 (or continuous) wavelet transform. 'Ihe terms continuous wavelet
transtorm (LW I I ano i nte2rat wavelet transrorm (1W 11 will De used intercnangeaniv
tn刃ugflout tnis 000K. i-'ixea time-rrequency resolution or me a it ' i poses a serious
constraint in many applications. In addition, developments on the discrete wavelet
transform (DWT) and the wavelet series (WS) make the wavelet anuroach mare suit-
arne tnan tne a ii너 I ror signai ana image processing. 10 clarity our points, let us
observe that the radii 八中 and 스多 of the window function for STFT do not depend
upon location in the t크2) plane. For instance, if we choose 中(t) = g (t) as in the Ga-
68           기入IE-FR日그UENCY ANALY引S


                    A        B                                                  CD
                            r       /                  I
    1




    0




m   10                                                          2                       슘
               FIGURE 4.6 Chirp signal with frequency changing linearly with time.


bor transform (see Section 4.2.2), once a is fixed, so are 八gq and 八亨그，regardless of
the window location in the t-w plane. A typical STFF time-frequency window has
been shown in Figure 4.3. Once the window function is chosen, the time-frequency
resolution is fixed throughout the processing. To understand the implications of such
a fixed resolution, let us consider the chirp signal shown in Figure 4.6, in which the
frequency of the signal increases with time.
   If we choose the parameters of the window function 中(t) [a in the case of g口(t)]
such that 스中 is approximately equal to AB, the STFT as computed using (4.7) will
be able to resolve the low-frequency portion of the signal better, while there will be
poor resolution of the high-frequency portion. On the other hand, if 스中 is approxi-
mately equal to CD, the low frequency will not be resolved properly. Observe that if
 A0 is very small, 스8 will be proportionally large, and hence the low-frequency part
will be blurred.
    Our objective is to devise a method that can give good time-frequency resolution
at an arbitrary location in the t크U plane. In other words, we must have a window
function whose radius increases in time (reduces in frequency) while resolving the
low-frequency contents, and decreases in time (increases in frequency) while resolv-
ing the high-frequency contents of a signal. This objective leads us to the develop-
ment of wavelet functions 砂 (t).
    The integral wavelet transform of a function f (t) e L2 with respect to some
 analyzing wavelet 砂 is defined as
                                               /1m

                              吼／(b, 口） := /           f (t）勿，a(t) dt,                (4.32)
                                              J- oo


    where
    \Vhere

                                砂b.a (t)＝二＝砂！二：므 ,           口＞ 0.                   (4.33)
                                         ..ja a
                                                      CONTINUOUS WAVELET TRANSFORM                             69



！卜呻ran妃ters. b an,d口 꺄옜led．切，兀si口帥and押i叩p叩．甲er옥呻畔如ly.




In addition to satisfy.
                     ing  34), a wavelet is constucted so th it has a high4r order
                                   (4.                                                 at
01 vanisning momenrs. it waveict is sasu 10 nave v게 lsning moments or orae지 m ii



                   L: (t)          tP少    dt =   0,     p=   0,   .   .   .   ,m   -            1.   !   (4.   35)

    Strictly speaking, integral wavelet transfonn provides time-scale analy卜is and
not time-frequency analysis. However, by pro꺄r scale-to-frequency 甘ansfoimation
(discussed later), one can get an analysis that is very close to time-frequency analy-
sis. Observe that in (4.33), by reducing a, the support of *b,a is reduced in tine and
hence covers a larger frequency range, and vice versa. Therefore, 1/a is a me4sure of
frequency. The parameter b, on the other hand, indicates the location of the 加avelet
window along the time axis. Thus, by changing (b, a), W, f can be computed on
the entire time-frequency plane. Furthermore, because of the condition (4.34), we
conclude that all wavelets must oscillate, giving them the nature of small wa 'es and
hence the name wavelets. Recall that such an oscillation is not required for tle win-
dow function in STFT. Compared with the definition of STFT in (4.7), the 如avelet
*b,a (t) t砥es the place of b4. Hence a wavelet also behaves like a windo由 func-
tion. The behavior and measures of wavelet windows 町e discussed in more detail in
Section 4.5.2.


4.5.1   Inverse Wavelet Transform
Since the purpose of the inverse transform is to reconstruct . the .original 舛nction
from its integral wavelet 甘ansform, it involves a two-cimenslonal mtegratKn over
me scale parameter a ana tne translation parameter b. inc expression for the辛nverse
wavelet transform is


               f(t)＝訂：可：二幽／(b刎1/!b,a(t)加，                                                                (4.36)

where C少 is a constant that depends on the choice of wavelet and is given b


                                         c* =/：出뇨＜的·                                                     (4.37)

The condition (4.37),        as the 口dmissibility condition, restricts the cass of
                           known
                                                                                            .



functions mat can be wavelets. In p缸ticular, it Implies that all wavelets mut have
70      기N任-F旺QL兀NCY ANALY듸S

*(O) = 0 [see (4.34)] in order to m川ke the left-hand side of (4.37) a finite number.
For a proof of (4.36), readers may refer to [2, Chap. 2].
   Equation (4.36) is essentially a superposition integral. Integration with respect
to a sums all the contributions of the wavelet components at location b, while the
integral with respect to b includes all locations along the b-axis. Since computation of
the inverse wavelet transform is quite cumbersome and the inverse wavelet transform
is used only for synthesizing the original signal, it is not used as freciuentlv as the
integral wavelet transform for the analysis of signals. In subsequent sections where
the discrete wavelet transform (DWT) is in仕어uced, the inverse ol
useful in data communication and signal processing.


4.5.2    lime-Frequency Window

The definitions of the frequency-domain center and radius discussed in Section 4.1
                                                                                  which
do not apply to wavelet windows because unlike the window of STFT in
#(O) = 1, here the wavelet window 少 (0) = 0. In other words, 砂 (w) exhibits band-
pass filter characteristics. Consequently, we have two centers and two radii for 少(c小
We are interested only in the positive frequencies. Let us, therefore, define the center
nJ.t  and tl'
. . 牛 八＝= J
              'e radr's 스! ,sn
            111m mnJ: ==n - +
                                                       cu' " VJ " m1 vis
                                                                    a '   口a  s
                              八m 1 .1八 4八n . .1. '1 - 4m. . m=1n= . m=. ．· n nn
                                 t 'e均sit"e-tre
                                        "口" V " 니1나V                         H口
W+ U" 나 " ' V ' 나나' U口 U7 V" H' 느1

                      . ., . 席이莎叫勺0)
                      uJ+ ·＝                                                      (4.38)
                             'g陋예2dw
                        崎
                               [   Jr (m 小 m二）이莎(w)I2dw'
                                             W)I dw
                                        /；지莎（m)12
                                                                                  他39)



The definitions for t牛 and 스中 remain the same as those in Section 4.1, with 砂 (t)
replaced by 砂(t). For wavelets the uncertainty principle gives

                                                      工 H2
                                                      1
                                         八
                                                ＋八少
                                         寸
                                         八                                        (4.40)


If t " is the center and 스中 is the radius of 砂(t), then W砂f (b, a) contains the infor-
mation of f (t) in the time window

                         ［口t* +b_ a스中，口t* +b＋口스少］.                                (4.41)

Let us apply Parseval's identity to (4.32) to get an idea of the frequency window:

                                        1 1'的       /r m b\
                     1"4"／砂 f仍' (i)' = ＝二 I   f (t岫 I-    卜It                     (4.42)'
                     " " -, '- , -,    Vi J_。。.' '-' r \ a ) --
                                      =1．玎노叫줍而；抑d0).                              (4.43)
                                       U7I 1/ e (X)
                                             CONTINUOUS WAVELET TRANSFORM                      71


From (4.43) it is clear that the fr띠uency window is


                              （心呼뇨+ ］·
                             11La                                                         (4.44)


Th帥耐岫uen町wind鉀耐uct = 2啣 x 弘計4스砂崎＝螂帥·
   Figure 4.7 graphically represents the notion of the time-frequency window for
the wavelet仕ansform. Comparing Figure. 4.7 with the.corresponding.Figur 4.3 for
     i r i, we ooserve me nexmie nature oi t肥 wmuow in me waveiet 뗘1lsi叩l.                     For
mgner Irequency ( '/ 口．2), me. time winuow is,small, wnereas br .lower i早quency
a.                  .             .      .      .




tii口oJ, toe time winuow is l카ge. ror a nxeu irequency ievei, ( i/ ao), io exam-
nie, both the time and freouencv windows a七 fixed. Recall that in STFF the time-
rrequency winoow is nxeo reg町uless or me rrequency level.


Example:. We per면뜨a,continuous ,wavelet transform on the same functihn used

tor computing we        i r i. we cnoose tne compiex wioriet wavelet,
                                   =1= /4\   m -t '/ 2 h-i5. 336t
                                   甲 \'1 ;＝二 e      ' e =
                                                                        given   L
                                                                                D
                                                                                          IA 4<\
                                                                                          I'.中Jt1JJ


的 con叩ute the CWT

                                     1 fo - -f- -b
                          W1(b，口） = ＝든 /   f (t)少 1=1 dt.
                                    vu J니刃         U




          a)
                                                                        2口2A砂




                                                                                     八＋
                                                                                口2




                                                             八
                                                            2可

                                                    기111
                                                                八
                                                                寸
                            2口0Z＼砂



                             그               知莎＋


                                                                                          >

                          b0 ＋口0i求             b1 + a1尸             b2 ＋口2尸                t
          FIGURE 4.7 Time-frequency window for continuous wavelet transform.
72              TIME-FREQUENCY ANALYSIS



      2000




      1500 尸




 小N工VaCm그g上
       1000




                    IIItIIIIIIIIIIIIIifl!   i!   1                  川ff111！까！’H1nn手！Ilfln1J! !I tllhTUlflll 斗！1111111}끄I!lH!tJ

              500




                                             005                        0.1               0.15                   0.2
                                                                        Time (second)
FIGURE 4.8 Continuous wavelet transform of the signal shown in Figire 4.4 with Monlet's
wavelet.

The results are shown in Figure 4.8. The figure indicates good res伽tion of the events
in both the time and frequency axes. If we choose an appropriate range for a, the
transform needs to be computed only once to capture most, if n0t all, of the events
occurring in the time and frequency domains.


4.6             DISCRETE WAVELET TRANSFORM

Similar to the discrete Fourier transform and discrete short-time Fourier transform,
we have the discrete wavelet transform (DWT). However, unlike the discretized time
ana rreuuencv axes snown earlier in t'ouner analysis. nere we take me aiscrete values
ot the scale parameter a and the translation parameter b in a ditterent way. '[he
interest here is to introduce the DWT and show the relationship between DWT and
IWT. A detailed discussion of the DWT is presented in Chapter 7. Here we just
mention that we will take a to be of the form 2寸 and b to be of the form k25,
 where k, s c Z. With these values of a and b, the integral of (4.3k) becomes

                                   W*       f
                                                 (k2-8,
                                                          2_
                                                               s)   =
                                                                        2s/   2
                                                                                  /:f(t)砂 (2st   -
                                                                                                     k) i   t.          (4.   46)
                                                                                               WAVELET SERIE1               73

Let us now discretize the function f (t). For simplicity, assume the samplinE
be 1. In that case, the integr띠 of (4.46) can be written as

                                  W,11f(k2e5, 2_s) 심 2d12＞二 f (n)*(2sn - k).




                                                    fm(t) = f (t - tm).                                               (4.48)
This gives

                   吼／뇨（k2-             ' ,2-   ')
                                                    =
                                                            2,
                                                                 "   /:／뇨（,）少（2sf- (）山

                                                    毗s/2Z／伽 1 川砂(2' 小k)
                                                                     n


                                                    = 2S/2Zf (n)1fr [2sn -(k -m2')]
                                                                     n


                                                    勺 H／少／[(t1m2' )2e' ,2H' ].                                       !(4.49)
Therefore, we see. that for DWT,. a shift .in time of a function manifests it呻f in. a
raLli.er complicatea way. Kecall mat. a siuri in time ora三unction appear.s asja stun


irequency uomain.


4.7      WAVEIET SERIES

Analogous to the Fourier series, we have the wavelet series. Recall that the i干ourier
n八1.：八』m 八1r;,m1，끼 二111 =1八1二八_1               ：八1m1끼 八_.1.. iJa14八 r八1. r114!. r . . 1m』1＋．·1\14 tI+ \   J戶 r2    111뇨 11d111d
3CIICb CAIbLb WI         IUII뇨UUIIa UIIIJ. II UIC, 101 (UI, IULfl.41011 J \ i)
its waveser senes represenLauon
                      })드IIUUI#
                                , given as              .
                                                                                                          C L     , wr IrnVU




                                          f(t) =＞二＞二切k,，奴，,(r),                                                      1(4.50)
                                                                 S   k


where

                                           奴，小斥2u/2少（21t                       k).                                   k4.51)
74        TIME-FREQUENCY ANALYSIS

The double summation in (4.50) is due to the fact that wavelets have two parameters:
the 仕anslation and scale                   꺄加dic
                                     parameters                    , its
                                                                      "    恥rase如S                                   鈿c如미巾)   Fou加r
is given oy


                                                       p   (t)                   =           二   ckeJki.
                                                                                                                                      (4.52)


Since {eiki : k E 7Z} is an orthogonal basis of L2(0, 2ir), we can obtain Ck as

                                                     Ck = 구나p(t), ej'!).  乙;7r1                                  J
                                                                                                                                      (4.53)

On a similar line, if {少k,S(t) : k, s e Z} forms an orthonormal basis of L2(R), we
can get

                                                  Wk,s =         (f        (r)        ,    *k,   s   (t)
                                                                                                           )nn
                                                                                                                                      (4.54)

                                                                      .              ---             1k              l\
                                                                                                                                      (4.55)
                                                       =21 ' 吼八玉' 키"
Therefore, the coefficients {wk.5 } in the wavelet series expansion: of a function are
nothing but the integral wavelet transform of the tunction evaluatet at certain dyadic
points (k/2s, i/ 2'). No such. relationship exists between Fourier $eries and Fourier
transform, which are applicable to different. cla브ses Of functions; 尸ouner series ap-
plies to functions mat are square integraole in Lu, z,rj, wnereas r'9uner transrorm is
c.-... r . . mn＋．· ,111n .4. 나 n1.'1 ;11 r 2nD\   D八*1. .. ..-.. , a1小 i, 41乞如 1111r1 11rn1r스l스1 1rn114八nm1                           1\114 ', 上
jul    nui11.tiuiia      th1at w17 Ill L, \ LS) . 1Jul.11 WaV1.lt. t 口L111느／口 alit.    vv avS,1八 I tlltliohuthhfl,                    S/Il l.hl느#

other hand, are applicable to functions in L2(R).
   If I砂ic.s (t) I is not an orthononnal basis, we can obtain Wk.s using the dual wavelet
jvfk,s(t) J as wk,S = ( J(t), ck,s(tfl. mne concept ot dual waveiets wui appear in
subsequent chapters.


4.8      INTERPRETATIONS OF THE TIME-FREQUENCY PLOT

Let us briefly discuss the significance of a surface over the time-frequency plane.
Usually, the height of a point on the surface represents the magnitude of the STFT or
the IWT. Suppose the given function is such that its frequency does not change with
山ne: then we should exoect a horizontal line narallel to the time axis in the time-
frequency plOt, corresponding to me frequency Of me tunction. nowever, oecause 01
the finite support of the window function and the truncation of the sinusoid, instead
of getting a line we will see a (widened line) band near the frequency. To understand
it more clearly, let us consider a truncated sinusoid of frequency wo. We assume, for
the pur四se of explaining the time-frequency plot here, that even though the sinusoid
is truncated, its Fourier t翼lsform is represented as 8(w 小 wo).
    By replacing f (w) = 8(m - wo) in (4.16) and (4.43), respectively, we obtain

                                                  1G巾／(b, 釧 == 乙Jr1니a(.幻 냑）1                                                          (4.56)
                               INTERPRETATIONS OF THE TIME-FREQUENCY PLOT                            75


                          1W少／(b, 떼 = 雲1莎（.蜘）1.  二it
                                                                                                  (4.57)


It is clear如m (4.56) and (4.57) th피아地帥nd 1吼／(b可do n depend
upon b.On小．ef扼quency畔is, sinc』e匣(0)！二스and田sum굔gth匣（m).!.4 l,.m 尹，
n1刃n b· Onthe freqUenCy axiS, ShlCe I砂（0)1 =1, and aSS1llll ng that 1中（n끼
u, we wiii get me maximum magnituue or 3 i r i at g = w. i nen mere wiji qe a oanu
around 盲 = wo, the width of which will depend on 스8, the radius of中(co).
,              on of (4.57) is a little complicated
   Interpretati.
                                                       unlike STFT, wav.
                                                             since,          trans-   elet
torm uoes not give a time-Irequency piot wrecuy. Lret us consiaer a point 4r on me
frequency axis such that

                     陋이나卿(I如)I ; WE (0，的）} .                                                      (4.58)

恥r 띠1 prac如al purposes, we may take 可 = 畔．
  Now if 꿔e consider a variable 亨 = 아／a and rewrite (4.5乃 in terms 여由e new
variable , we have


                     吼／(b, 蛙）         =
                                           1
                                          ；二／ ＝二
                                                   Iw,
                                                                                                  (4.59)
                                弓         乙ill           弓




Therefore, the maximum value of the wavelet transform (4.57) will occur a 亨 = wo
with a ban曲帥야 = 蜘，depending on the radius 스計f the wavelet莎（                                  ).
  As our next exa끄［lple, let f (t) = 8 (t -t0). Since this function has all the fr uency
components, we should expect a vertical line in the time-frequency plane a t = to.
Substituting f (t) = 8(t - t0) in (4.7) and (4.32), we obtain

                           IG中／(b, 盲）1 = 陋(t0 - b)I                                               (4.60)


                          1W,1,f(b，때＝ 知쓰，흐                                                        他61)


Explanation of the STFT is straightforward. As expected, it does not depe d on 亨．
We get a vertical line parallel to the frequency axis near b = to with the tim spread
detennined by 스少 For wavelet transform we observe that it depends on e scale
parameter a. Rewriting (4.61) in terms of the new variable , we have



                    吼／(b, 竿）                             ,/亨       \  .   ,   ,   .

                                                                                                  (4.62)
                      \   c !                            叭可(JO - O))
   Although all the freciuencv contents of the delta function in 山ne are indicated by
U1勺司, a is ciear mat as we reauce g, me time spreaa increases. rurtnermore, tne
location of the maximum will depend on the shape of 少(t). Readers are referred to
[4] for more information on the interpretation of time-frequency plots.
          76    TIME-FREQUENCY ANALYSIS


          4.9   WIGNER-V江LE DISTRIBUTION

          We have considered in previous sections linear time-frequency rpresentations of
          a signal. The STFT and CWT are linear transforms because they!satisty me linear
          sIin1trnnsiticrn theorem. That is.

                                       T[a1f1 +a212] =alT[fl] +a2T[f2],                                                              (4.63)

 where T may renresent either the STFT or the CWT. and fi (r') and f7(r) a七 two
 different signals in the same class with coetliclents al and a2. 'I "hese transtorms are
important because they provide an interpretation to the local spectrum of a signal
at the vicinity of time t. In addition, easy implementation and high computation
e什id이icy of their a培이丑bins add 的 their advantages. 0n the o出er hand, these linear
transforms do not provide instantaneous energy information of the signal at a specific
instant of time. Intuitively, we want to consider a transform of the type


                        If (r      -
                                       小_
                                                       3dT
                                                                  dr
                                                                                 =
                                                                                     /:/（
                                                                                        【   -
                                                                                                t)
                                                                                                     f (t   -   t)
                                                                                                                     e_
                                                                                                                          }t
                                                                                                                               dr.
恣瑞客謠絮瑥；之eithin
           enei
               a監究喆穹擢’各繇捻：蒿
around th
defined
       bye time         location
                                            r.   For
                                                             曲s
                                                                       pu叩ose,
                                                                                      the Wigner-Ville dis따bution (WVD) is



                                   。。佃枷 (t - ）戶" 小·
                       W1(t, cv）긍，p0O
                                  J-f                                                                                                (4·的
 The constant l/ 2兀 is a normalization factor for simplicity of computation. We should
note that the linearity pro壯ty no longer holds for the equation above. The Wigner-
Ville distribution is a nonlinear (or bilinear) time-frequency transform because the
signal enters the integral more than once. 0ne may also observe that the Wigner-
Ville distribution at a given time t looks symmetrically to the left and right sides of
the signal at a distance r/ 2. Computation of Wf (t, cv) requires signal information at
i 士r/2 and cannot be carried out in real time.

Example 1: Let us consider a chirp signal that is modulated by a Caussian envelope:


               /(:)=（三）"' .「（푸*芹*）蜘7),                        (4.65)
恕甲，엾；謐然“恕黑ex-Ville器忿                 p(-
                                               黑，恕料，業 "'蜘'
         2ir (a,r-)l/2J005
Wj(t, cv)寸             -。。
                         expiLr_a(t +2r/2)2『）b(t +2r/2)니나
                                                       +fcvo1t+
                                                            『 T\,)jl
                                                                                                                                                         ＼八／IGNER-VILLE I긔ST뫼BU기ON                       77


                                  1 -a (t - r/ 2)2                                                            . -b(t - r/ 2)2                                . I              t\    .
                                                                                                                                                                                                  r
                              xe사기         2                                                                  /       2                                     7m0Lr             三) - JO兀

                            1 Ia\ 1/2 ..2 r的     I- at2                     \
                         = := 1 -)   e "' r  exp { -;--- + jbtt + j口ot - fa兀 I dr.
                              乙Jr                        /                    .／小的                              \             1+                                                      /


                                                                                                                                                                                                      他66)

                            the   Fourier甘ansform                                 of a             Gaussian
                                                                                                                                   function                as given     in
                                                                                                                                                                                  Chapter   3,    牛
                                                                                                                                                                                                 th WVD
nf n (nissi}n sinusoid-modulated chirp is
Using
                                                                                                              「r                                             wo_ bt)
                                                                                                                              at2
                                                         『『（
                                                          Wf (t,                                                                                                                                      (4.67)
                                                                                                                                                                             21
                                                                                                                                                   (w_
                                                                                        1
                                                                              =
                                                                         0)
                                                                              =
                                                                                                     expi-                         2                          a
                                                                                    -
                                                                         w)
                                                                    『，
                                                                                                                    [-




The function and its 꿔VD 缸e shown in Figure 4.9.

Examp加 2: A sinusoidal modulated chirp signal is given by


                                                                                                                                                                                                      他68)
                                                                              f (t)         =exp                         （芹                   『）          蜘《）   ·




        dE＜亡m= m
               m
               m
                   0.5

                       0


                       5                                                                                                                                                                                       的



                       1
                        5                           -4       -3                                                                                                                                         5




             0.4

                   나
                   D
                   0

          2   1
          0   0

        쁨글百E<



                   05




                                                                                                                                                                    m


                           FIGURE 4.9                             Wigner-Ville distribution of a Gaussian-modulated chirp signal.
78                  TIME-FREQUENCY ANALYSIS

We compute the WVD straightforwardly to obtain


                      w/(,, .)＝츤
                       f(t,w)=-    IO ,P
                               乙IL Jh的
                                       explj
                                         rj  b(t+r/2)2 +j蜘(
                                         L
                                                                            )]
                                        r . b(t -r/2)2
                                 >( expl-J       ,.
                                                        . /』 r\ .
                                                       3口勺 1 r - : I -i끄Dr dr
                                        L
                              = 二／느xp(jbtr日娜 -J啣：
                                 hJl J_ (X)

                              =8(w- oio- bt).                                     (4.69)

E노ample 3: We c毗pute the 硼VD 可a 叫的伽的idal signal ejct勺iby setting the
chirp parameter b to zero. Therefore,

                                            ejn加r <＝수8 (w叫coo).                   (4.70)

The WVDs of (4.67) and (4.69) on the time-frequency plane are a straight line with
a slope b and a straight line parallel to the 血ne axis, respectively. They are given
in Figures 4.10 and 4.12. Figure 4.11 shows the WVD of a C
sinusoidal function.




                5
            0

 U
 n              0

 d E ＜亡m4 而m丁
                5




       毗

 6 4
 0 0
                늬




 g글百E <
                노




                                                5   0



                          FIGURE 4.10 Wigner-Ville distribution of a chirps gn毗
                    VVVVV\
               1


0       m
                   戶
                   hU




                   0




d
E ＜亡m口im工          二
                   U




                巧
               너
                            -4
                                  -3        -2
                                                              0      1           2    3              5




        0.8 노

80.6-
    .

읕0.4-.
<
         0.2-.


              S0




                                                     5    0
                                       t                                    (S



                           FIGURE 4.11     Wigner-Ville distribution of a sinusoidal function.




d E ＜亡m口쿄m=
               毗


                   0


                   唾
                             -4   -3        -2
                                                              0      1           2    3          4   5




              口U
              0


   n<     1

   0      0


m乙＝ 仁죠E <




                                                      5   0
                                                                            0)



                        FIGURE 4.12    Wigner-Ville distribution of a Gaussian-modulated sinusoid.

                                                                                                         79
80       TIME-FREQUENCY ANALYSIS

4.10     PROPERTIES OF THE WIGNER-VILLE DISTRIB

There are several general properties of WVD that are important fjr signal represen-
tation in signal processing. Some of them are discussed in this section. It has been
shown [5] that the Wigner-Ville distribution has the highest concentration of signal
energy in the time-frequency plane. Any other distribution that has higher energy
concentration than WVD will be in violation of the uncertainty Drinciple. Further-
more, it cannot satisty the marginal prope作ies c1iscussei in mis sction.


4.10.1     A Real Quantity

The Wigner댄毗di曲bu由n.is always real，肥gardless可whe血申岫．培nal,is real
or compiex. I nis can oe seen oy consiaenng me compiex conjugi比 01 me wigner-
Ville distribution:


                      叫긍，L:s(t_ )s（나）e'"T d
                   吼（t，
                           긍，乙(t +）小白（-"'"
                           = w小，m).                                                          (4.71)

Wigner-Ville distribution is always real but not always positive. Figure 4.13 shows
the WVD of a function that becomes negative near the center. Consequently, WVD
may not be used as a measure of energy density or              den
                                                        probability              中ity.
4.10.2    Marginal Properties
Of particular concern to signal processing is the energy conservation. This is cx-
pressed by the marginal properties of the distribution:


                            /:W1        (t, cv) dw = If (t)I2                                (4.72)


                             /:wf (t, w) d！늬加기" ·                                            (4.73)
                             "    W




Marginal (density) expresses the energy density in terms of one of the two variables
alone. If we wish to find the energy density in terms oft, we simply integrate (sum
up) the distribution with respect to cv, and vice versa. The total energy of the signal
can be computed by a two-dimensional integration of the Wigner-Ville distribution
over the entire time-frequency plane.

            戶 00                 尸00        m         戶 00            尸00                1

     月＝ /          If (t키2dr= /        17佃）Izdw = /                   /     W1(t며）dw dt= l
           V 叫00                                     / 寸0U 1/ H (JU                      1
                                                          QUADRATIC SUPERPOSITION PRINCIPLE                    81




                  U
                  <
                  0




    dE ＜亡m= 나
            mm仁
                  0


                  나
                  ＜
                  0                              +




                  n
                  <
                  0




 쁨글죠E <
      1
                  0


                  2
                  0                                                                         4




                                                                                                        5
                                                                                                    4
                                                                                        3
                                                                              2
                                                                      1
                                                     -5   0
                                                                                   0)


                      FIGURE 4.13   Plot indicating that Wigner-Ville distribution may be negative.



4.10.3                  Correlation Function
We can compute the correlation functions in the time or frequency domains easily
from the marginals. That is,


                               ／小    ')   =   /:/(!)/(！ 小=『！     '）
                                                                              Wj（乙이                         (4.74)


                               枷（0')      =   /:f(0)f (0) dw  + cv')      =       Wi(0, cv')    .           (4.75)


4.11                  QUADRATIC SUPERPOSITION PRINCIPLE

We recall that WVD is a nonlinear distribution where the linear superposition prin-
ciple does not apply. For instance, let a multicomponent signal be


                                                 f(t) = 二 fk(r).                                            (4.76)
                                                           k=1

The Wigner-Ville distribution of this signal is
82            TIME-FREQUENCY ANALYSIS

                                    m                 兀1   m

                    Wf(t, co) =＞二w九（t, w) +＞二 ＞二 w丘．九（L m),                                 (4.77)
                                    k=1           k=1 t =1,t尹k

where Wfk (t, co) is called the auto-term of the WVD, while Wfk (t, co) is a cross-
term defined by


                   Wfkt(t, w）긍，亡fk (나）쨔- je                                                  (4.78)


These cross-terms of the WVD are also called interference terms ,which represent
the cross coupling of energy between two components of a multic omponent signal.
These interference terms are undesirable in most signal processing applications, and
much research effort has been devoted to reducing the contribution ()f these terms. We
must remember that these cross-terms [6, 7] 缸e necess町y for perfisct reconstruction
of the signal. In signal detection and identification applications, w1三 aj七 interested in
discovering only those signal components that have significant e riergy. The cross-
terms are rendered unimportant since reconstruction of the signal i
    In radar signal processing and radar imaging, the signals to be                     a
time-varying spectrum like that of a linear chi叩 or quadratic chirr                     e
STFT or WT to represent a chirp signal loses resolution in the time可requency plane.
However, the WVDs of these signals produce a well-defined concentration of energy
in the time-frequency plane, as shown in Figure 4.10. For multicomponent signals,
the energy concentration of the WVD will be far apart in the time-frequency plane
if the bandwidths of the components are not overlapped too much (see Figure 4.14).



          2


          0


                          10          20     30                40       50                  60
     -2
                                                  t




                     40                                                                50        60



                               0)                                   t

                FIGURE 4.14 Wigner-Ville distributi。
                                                   n 。f a multic。
                                                                mp。
                                                                  nen나       signal.
                                                                  AMBIGUITY FUNCTION      83

However, if this is not the case, certain cross-interference reduction techniques must
be applied, and that leads to the reduction of resolution.



4.12          AMBIGUITY FUNCTION

The ambiguity function (AF) is the characteristic function of the Wigner-Ville dis-
tribution, defined mathematically as



                        A1(u,v)= J:f:e.U 'f+"OWf(t,cv)dtdcv.                           (4.79)

While the Wigner-Ville distribution is a time-frequency function that measures the
energy density of the signal on the time-frequency plane, the ambiguity function is
a distribution that measures the energy dist餉ution over a frequency-shift (Doppler)
and time-delay plane. This is a very important function in radar signal processing,
particularly in the area of waveform design. We shall see some applications of this
function toward the end of this book.
   Apart from a complex constant, we may express the AF in terms of the signal as


                   A1(r, .) 나／乙 (t - 引f ( +Hn dt,
                                   J- oo   \         二/   \   二/
                                                                                       (4.80)

where K is a complex constant. The proof of this relationship can be found in [8].
For further information on the ambiguity function, readers are referred to [9]. Fig-


       1


       0


   쁨 귿 죠 E<

       너
                   10         20           30
                                                 t




 4

 0    0
     /
     n
  m乙그듬E <


     0韶

                                                                                          32


                                      32   -32

                                                              T

                    FIGURE 4.15     Ambiguity function of a chirp signal.
84              TIME-FREQUENCY ANALYSIS

ure 4.15 shows the AF for a chirp signal. This time-frequency reptesentation will be
revisited in Chapte,r        a combination. wavelet packets and the Wigner-Ville
                              9,   where                                                                             of
aismouuon is appueu ro raoar signai aetecuon.



 4.13           EXERCISES

1. Verify that for any function 少 E L2(- o기 아）), the normalized function given by
   少k.s(t) = 25/2少（25t - 幻 伽k, s E Z, t E R, has the same L2 norm as 少 :


                             /:1少（t)I2dt= /:1奴，S（이'dt,                                                                                                             (,sd 7L.
                                                     '2, a >               the window                                               (1
                  the time
                       window
                                                                                                                          ee        .                 .   .   0.    Co며pute
2.
      wicltfls in me
     Consider
                           and trequency domains anti venry me uncertainty principle.
                                               function                             ga           (r)      =




3. 기妃 加mmc作on N2 is defined by

                                                            , . .                    [t,                                       forO< t< 1

                                                                                     1 j,                                  otHer叩is己

     Compute the time-frequency window for N2(t).
   r,1mn.. . , t1八1 n J, /4\ Hn' i r r 나져 rri. i-니2 Ji.Jj.
4. Show that1If (t) II' = 石i느；下／/K；      中／(b，釧“dbd亭

5. Given that f (t) = sin ,rt2, and using the raised cosine as the w ndow function



                                           中（!
                                           t              (t)   ）出，   =        。,         +cos                (rt)              ,               In:
                                                                                                                                         。therwise,   <1

     하ot the window田h江匕d time functions 力(t) == 砂（n - 3)/(t) and 力(t) and their
     spectra.
     Consider the time-frequency atoms or the kernel

                                      1Re［中（t - 4)ej4兀i ＋中（t - 6)e/8兀I]
                                      iRe ［中（t - 4)e '4兀r ＋中（t - 6)e
                                                                     '6兀11 ·
     Plot the spectral energy density of the two time-frequency atoms. Comment on
     the time-frequency resolution of the two atoms.
6. In the CWT, show that the normalization constant l/ ,J万 is needed to give
           忖떼 = 加比떼卜
7. Show that the energy conservation principle in the CWT implies that

                                                                                                                                                                                  쁘구
                   尸 /(t)而dt = + ／的 尸 吼／(b,
                                                                                                                                                                              1
                                                                                                                                                                              b
                   1/   아）                                                L少         J-                oo, ／小以）
                                                      COMPUTER PROGRAMS         85

8. Show that the frequency window wid由 of a wavelet 少 is [(1人m畦 寸 스砂）,
   (1/a)(畔 + 스砂）］·
9. Identify the reason for dividing the frequency axis by 2 in the program wvd.m.



4.14       COMPUTER PROGRAMS

4.14.1      Short-Time Fourier Transform
秀
돔 PROGRAM S七f七 . m
秀
% Short- time Fourier Transform using             Rectangular window [0, 11
% generates Figure 4. 5


돔 Signal

vi = 500; % frequency
v2 = 1000;
r = 8000 ;     돔sampling ra七e
七1 = 0. 192 ; 돔 loca七ion (：江 나le delta         function
亡2 = 0 . 196 ;




k 七f
       = 1: 2048;
       = (k- 1) /r;
       = sin (2士pi出＼jl士七） + sin (2枉竝* 尨女t) ;

k := tl     出 r ;
f (k) =     f (k) + 3;
k = 七2      火 r ;
f (k) =     f (k) + 3;

plo七 ( 七 , f)
axis ([ 0 0. 24 -2 2] )

figure (2)

老 ST1町1 compu七ation

N = 16 % rectangular window width
bo亡 == 0 . 1 ;
hi ＝二 0 . 175 ;

for kk = 1 : 4
  Nb2 = N / 2;
  for b = l: 2048-N+l
    fb = f (b: b+N-l) ;
86      TIME-FREQUENCY ANALYSIS


       fftfb  = abs (fft (fb) ) ;
       STFT (b, :) = fftfb (1:Nb2) ;
     end

毛 Plot

     NColor = 256;
     colormap (gray (NColorfl;
     STFT_min = min (min (STFTH;
     STFT_max = rnax (max (STFTfl;
     STFT = (STFT - STFT_max) * NColor /          (STFT_min -   STFT_max) ;
     time= (0: 2048-N) /r;
     freq = (0:Nb2-1) * r / N;

     axes ( 'position ' , [0. 1 bot 0. 8 hi] )
     image (time, freq, STFT ' )
     axis ( [ 0 0. 24 0 2000) )
     YTickmark = [0 500 1000 1500 2000] ;
     set (gca, 'YDir ' , 'normal ' , 'ytick ' ,YTickmark)

  뇨끄d on;
  N = N 出 2
  bc比 = bc比 + 0 . 225 ;
  clear STFT; clear time; clear           freq;
end

set (gcf, 'paperposition ' , [0. 5 0. 5 7. 5 10] )


4.14.2     Wigner-Ville Distribution
毛
돔 PROGRAM ＼사＼八크 . m
老
% Computes Wigner-Ville         Distribution
돔

돔 Signal

r = 4000 ; 왐 sampling ra七E크
t = (0: 255) / r;
omegal = 2. 0 * pi * 500. 0;
f = exp (i出omegal 女 七） ;

돔 WVD Computa七ion

N=length (f) ;

if (mod (N, 2) == 1)      ;
f = [f 0] ;
                                                      COMPUTER PROGRAMS   87

N = N + 1;
end

N2ml = 2 * N - 1;
Nb2 = N / 2;

for in = l: N
  S = zeros 口．,N鈿江 ) ;
  s (N- (m-i) :N2ntl- (rfl- l) ) = f ;
  s = conj (fliplr    (s) ) .*s;
  S = s (Nb2:N2rnl-Nb2) ;
  shat = abs (fft (s) ) ;
g
% Normalize with the number of overlapping terms
왕
  if m <= Nb2
     sha亡 = sha七 / (2 士 rn - i ) ;
  else
     sha七 = sha七 / (2 士 N - 2 女 In + 1 ) ;
  end

사vd (rn, : ) =shat (l: Nb2) ;
end

움 P1(：比

time = (0:N-l) / r;
freq = (0:Nb2-l) * r            / N / 2;

NCoior = 256;
colortuap (gray (NColor) ) ;
w＼八lmmn = mm1l (mmn (＼小俎） ) ;
＼사＼八1 max = max (max (＼사＼/d) ) ;
w （크 = 佃ivd - 們／（크 max) 女 NC（그bC)r         /   (wvd_min - wvd_ma川 ;

image (time, freq, 小／d ' ) ;

% Because of the finite           support of the signal,     there will
돔 end effec亡5

xlabel ( 'Time (seconds> ' ) ;
ylabel ( 'Frequency (Hz) ') ;
set (gca, 'YDir ' , 'normal ' )
88     TIME-FREQUENCY ANALYSIS

REFERENCES

1. D. Gabor, "뇨oiy of communication:' i. lEE (Lon勿n), 93, PP. 4294457, 1946.
2. I. Daubechies, Ten Lectures 。n Wavelets, CBMS-NSF Ser. Appi. Matl. #61. Philadelphia:
   SLAM. 1992.
3. J. B. 시lan and L. R. Rabiner, "A unified approach to STVF analysis and synthesis," Pr冗.
   of IEEE, 65, pp. 1558-1564, November 1977.
4. A. Grossmann, R. Kronland-Martinet, and J. Monlet, "Reading and understanding con-
   tinuous wavelet transform," in Wavelets, 7m7w-Frequency Methods and Phase Space, J.
   M. Combes, A. Grossmann, and Ph. Tchamitchian (Eds). Berlin: Springer-Verlag, 1989,
   pp. 2-20.
5. T. A. C. M. Claasen and W. F. G. Mecklenbrauker, "The Wigner-Ville distribution: a
   to아 for time-frequency signal analysis: I. Continuous time signals,' Philips J. Res., 35,
   pp. 217-250, 1980.
6. A. Moghaddar and E. K. Walton, "Time-frequency distribution analysis of scattering from
   waveguide cavities," IEEE Trans. Antennas Pmpag., 41, pp. 677-680, May 1993.
7. L. Cohen, "Time-frequency distributions: A review," Proc. 尼EE, 77, b,p. 941-981, 1989.
8. Bou日em Boshash, "Time-frequency signal analysis," in Advances inSpectral Estim口tion
   and Array Processing, Vol. 1, S. Haykin, (Ed.). Upper Saddle River, N.J.: Prentice Hall,
   1991, Chap. 9.                                                     1
9. C. E. Cook and M. Bernfeld, Ra加r Sign口ls. San Diego, Calif.: Academic Press, 1967.
 CHAPTER FIVE




 Multiresolution Analysis

 Multiresolution analysis (MRA) forms the most important building block for the
 construction of scaling functions and wavelets (Chapter 6) and the development of
 algorithms (Chapters 7 and 8). As the name suggests, in multiresolution analysis, a
 凡nction is viewed at various levels of approximations or resolutions. The idea was
 developed by Meyer [1] and Mallat [2,3]. By applying the MRA we can divide a
complicated function into several simpler ones and study them separately. To under-
stand the notion of MRA, let us consider a situation where a function consists of
slowly varying and rapidly varying segments, as illustrated in Figure 5.1. If we want
to represent this function at a single level of approximation, we have to discretize it
using S妃p size (h), determined by the rapidly val如娼 se얍nent. 가小 leads t叱 lai召e
number of data points. By representing the function using several discretization steps
(resolutions) we can significantly reduce the number of data points required for ac-
curate representation. The coarsest approximation of the function together with the
details at every level completely represent the original function. Observe that with
every level (scale), the step size is doubled. This corresponds to octave-level repre-
sentation, familiar in audio signal processing. In addition to this specific example,
there are many situations in signal processing as well as in computational electro-
magnetics, where multiresolution analysis can be very useful.
   In this chapter we begin with an understanding of the requirements of MRA.
Two-scale relations and decomposition relations are explained. Cardinal B-splines,
discussed in Section 5.5, generate an MRA and form the basis of most of the wavelets
discussed in this book and elsewhere. Finally, in Section 5.6 we discuss how to map
a given function into an appropriate subspace before starting an MRA.


5.1 MULTIRESOLUTION SPACES

Let us go back to Figure 5.1. Every time we go down one level by doubling the
step size, we remove certain portions of the function, shown on the right-hand-side
plots. Then there are the "leftover" p缸ts which缸e further decomposed. In Figure 5.1

                                                                                   89
90      MULTIRESOLUTION ANALYSIS


  16
                               h=
                                    1
   8

   0
                          16            24


  16                                            16
   8                                             8
   0                                             0
               8          16            24        0                    16        24


  16                                            16

   8                                             8
   0                                             0
                          16        24


  16                                            16

   8                                             8

   0                                             0
                         16         24            0          8         16        24
                   디CURE 5.1 Multilevel representation of a function




we assign all the functions on the left-hand side to A5 and those on the right-hand
side to WS, where s represents individual scales. Let A5 be generated by the bases
 {中k,s : 2'/ 2中(2't - k); k e Z} and W. by {少k,s : 2'/ 2少(2't - k); k e 7L}. In other
words, any function x5 (t) and Ys (t) can be represented as the linear combinations of
中k.s(t) and 砂k,s(t), respectively.
   Observe that the functions x5_1(t) E A5_1 and y5_ i (t) e W5_1(t) 缸e both
derived from x. E A5. Therefore, we should expect that the bases 中k,s-i of A5_1
and *k.s-i of W5_ i should somehow be related to the bases 中k ,s of A5. Such a
relationsh巾 的내이p in devisit鳩 an 키g이恤m to obtain the func的n5x5_ i andy5니
from x5 more efficiently.                                            1
   To achieve a multiresolution an出ysis of a function as shown k Figure 5.1, we
must have a finite-energy function 中(t) E L2(IR), called a scaling function, that
generates a nested sequence {A1}, namely


                     (0) <H · · . CA_i cA0cA1 C ... 4 L2,
                                                        MULTIRESOLUTION SPACES      91

and satisfies a dilation (refinement) equation

                             中（t) = ＞二go[k] 中（at- k)
                                       k
for some a > 0 and coefficients {go[k]} E Z 2. We will consider a = 2, which
corresponds to octave scales. Observe that the function 中(t) is represented as a su-
pe叩osition of a scaled and translated version of itself-hence the name scalingfunc-
tion. More precisely, A0 is generated by { (. - k) : k E 7LJ and, in general, A5, by
{中k,s : k, s E 7Z}. Consequently, we have the following two obvious results:

                           工（t) e A5 ＜수 工（2t) E 盛＋1                               (5.1)
                           兀（t) E A5 ＜수 工（t+ 2기 E 盛．                              (5.2)
   There are many functions that generate nested sequences of subspaces. But the
properties (5.1) and (5.2), and the dilation equation are unique to MRA.
   For each s, since A5 is a proper subspace of A5+i, there is some space left in A5,
called WS, which when combined with A5 gives us A阡1. 가lis space {W5J is called
the wavelet subspace and is complementary to A5 in A5+i, meaning that

                             A5 fl '入／S = ｛아，          s eZ                      (5.3)
                             A5 4) W5 = AS+L                                     (5.4)
With the condition (5.3), the summation in (5.4) is referred to as a direct sum and the
decomposition in (5.4) as a direct-sum decomposition.
   Subspaces {W5} are generated by 少(t) E L2, called the wavelet, in the same way
as {A5} is generated by 砂(t). In other words, any x5(t) E A5 can be written as

                            자(t) = ＞二aj ,: 中（25t- k),                            (5.5)
                                       k
and any function yS (t) e W5 can be written as

                            升（t) =＞二功k,；砂（25t - k)                               位6)
                                   k

for some coe什icients {ak,s}kEz, {Wk,5}kEZ e e2.
   Since

                       A5+i = W5 q) AS
                             = W5 q3W5m1 由A5-1

                             = wS 4) wSHl 由 w卜그 4) · · · ,                       (5.7)
we have

                                                   W
                                               H
                                   A
                                           如
                                           ＋
92     MULTIRESOLUTION ANALYSIS




                                                 AM




      AM 2                    WM_2



AM日       WM_3




                      FIGURE 5.2          Splitting of MRA subspaces.


  Observe that the {A5 } are nested while the {W5 } a七 mutually orthogonal. Conse-
quently, we have

                         1A fl Am            =    At,
                                                          m> t
                        1WtflWm              =    {0},    t 7드 77i
                        (AtflWm              =    101,    t < m.

A schematic representation of the hierarchical nature of A5 and W5 is shown in
Figure 5.2.


5.2   ORTHOGONAI, BIORTHOGONAL, AND SEMIORTHOGONAL
      DECOMPOSITION

In Section 5.1, the only requirement we had for the wavelet subspace W5 was that it
be complementary to A5 in A5+i. In addition to this, if we also require that W5 上
A5, such a decomposition is called an orthogonal decomposition. Let us explain the
orthogonality of A5 and W5 a little further. For simplicity, let s = 0. For this case,
{ (t -k) : k E Z} spans Ao; similarly, {1i(t -k) : k E Z} spans Wo. Then A0 I W0
implies that

                    /：中      （!）少（!   －   『）dt= .        for all t e Z.          (5.8)
     ORTHOGONAL, BiORTHOGONAL, AND SEMIORTHOGONAL DECOMPOSITiON                                       93

 In gener키, {中(t - k) : k e Z} and {砂(t - k) : k E Z} need not be orthogonal in
 themselves; that is,


                                          /：中（加（ !) dr尹.
                                                     《－
                                         /：少 （!）砂（t       -   t) d《尹『                            (5.1이

   Let us relax the condition that A5 and W5 be o曲明onal to each other and as-
sume that the wavelet 砂k ,s E WS has a dual, *k,了 E W1. Duality implies that the
biorthogonality condition is satisfied, namely

                        (少J,k, uli&m) = 8j,1 · 8t,m,             j, k, t, meZ.                   (5.11)

Although we do not require that W5 上 A5, we do need W1 J A5, the importance
of which will become clear later. Similar to the dual wavelet 砂1 t . we also consider
n J . . n] nnn1·
a dual scaling．mm r . . =1八1·. 八m ;
                  tunct上．on 中k ,了 11 '1n1 mm＝八1.n1八n n11八41n11 11l) A ri
                                    that  generates another MKA jASJ1 ot   L. In other words,
                                                                         八r r 2 - .m n111八m . . . 八＝.J ‘시

中k,s and 砂k,s are associated with the MRA (A小 and 中k ,s and 少k,s are associated
with the MRA (A5).
   Let us summarize our results so far before proceeding to explain their importance.
  ｝江RA (A小

                                 A5+i =A5-s- W5,
                              AtflAm = A1,
                             W1 fl Wm =(0},
                             AtflWm = {0),

   MRA {AS):

                                 A5+i = AS + W1,                  m> t
                              At fl Am == A1,                     m>Z
                             W1 fl Wm = (0},                      t 尹m
                             A1 fl Wm = {0},                      t< m.

                         ll                  nn
                                 시 盛 匈                              bb       mm
                                         斗
                         吼旽              斗   瓦由Wm == ｛아
                                               Wm = (0)

   The decomposition process discussed so far is called biorthogonal decomposition.
To understand its importance, let us briefly point out the procedure of decomposing
a function into scales, as shown in Figure 5.1. The details are left for Chapter 7.
   Given a function x(t) E L2, the decomposition into various scales begins by
mapping the function into a sufficiently high resolution subspace AM, that is,

                    L2 9 工（r) H1+ 工M = ＞二口k,M中（2Mt - k) E Aa小                                   (5.12)
                                                 k
94     MULTIRESOLU기아시 ANALY듸S


No＼人／since

                          AM = WM_ 1 + AM_ i

                                     = WM_ i + ＼入Ii／七2 + AM그


                                     =>              N
                                                     Z向      WMri+ AM_N,                                                         (5.13)


we can wnte


                            抑i       (r)             =   ＞二YM-
                                                             n=1
                                                                                     n    ＋工M-                    N,
                                                                                                                                 (5.14)


where xM_N(t) is the coarsest approximation of xM(t) and

                         x5(t) = ＞二 ak,54 (2't - k) E A5                                                                         (5.15)
                                                     k

                         升(t) = ＞二功t，泄（h ak 吼1                                                                                   (5.16)
                                                     k

Now the importance of dual wavelets becomes clear. By using the biorthogonality
condition (5.11), we can obtain the coefficients { wk,5 I as


                         Wk,s = 2'                   /:        y5   (t)              7   (25t             -       k)       dt.   (5.17)


Recall that少 (25t - k) E W and At 上 W5 fort <s. Therefore, 章y taking the inner
product of (5.14) with 砂k,5(t) and by using the condition (5.11), 申e have


                         Wks = 2
                        『*  ,5             2sf   '        。。XM
                                                         p00
                                                         _                (t)            *(25t                -        k) dt

                                                                                                                                 (5.18)
                                 =         25/       2 w弘』                      （}               ，   士）                ·




The dual wavelet 砂 can be used to analyze a function xM by co puting its integral
wavelet transform at a desired time-scale location, while 少 can be used to obtain
its function representation at any scale. Therefore, we call 少 an nalyzing wavelet,
while 砂 is called a synthesis wavelet.
    Of course, if we have orthogonal decomposition A5 上 W5 with orthonormal
bases {色 砂}, the analyzing and synthesis wavelets are the same. bserve that when
we say orthonormal wavelets, this implies that the wavelets are orthonormal with
respect to scale as well as with respect to translation in a given scal . But orthonormal
scaling function implies that the scaling functions are orthonorm only with respect
to translation in a given scale, not with respect to the scale bee use of the nested
nature of the MRA.
      ORTHOGONAL, BIORTHOGONAL, AND SEMIORTHOGONAL DECOMPOSITION                    95

    A question that arises is: Why do we need biorthogonal wavelets? One of the
attractive features in delegating the responsibilities of analysis and synthesis to two
different functions in the biorthogonal case as opposed to a single function in the
orthonormal case is that in the former, we can have compactly supported symmetric
analyzing and synthesis wavelets and scaling functions, something that a continuous
orthonormal basis cannot achieve. Furthermore, orthonormal scaling functions and
wavelets have poor time-scale localization.
   In some applications discussed in later chapters, we need to interchange the
roles of the analysis and synthesis pairs, {中, 少) and {色 砂}, respectively. In biortho-
gonal decomposition, we cannot do so easily since 砂 and 中 generate two different
MRAs, A and A, respectively. For such an interchange, we need to map the given
function x i- * XM E AM, and then we can use 少 as analyzing and 少 as synthesiz-
ing wavelets.
   In addition to biorthogonal and orthonormal decomposition, there is another class
of decomposition, called semiorthogonal decomposition, for which A5 I W1. Since
in 比is system, the scaling function and wavelets are nonorthogonal, we still need
their duals,夕 and 砂. However, unlike the biorthogonal case, there is no dual space.
That is, 中，中 e A5 and 少， 砂 e WS, for some appr아）niat艮scales. In 曲is system it is
very easy to interchange the r이es of 色 少 with those 可 色 少．
   For semiorthogonal scaling functions and wavelets, we have


           (4)(r - k), 4)(t -t )) = 8k,t        k, Z E Z                        (5.19)
and
                   (少j,k, 7t,rn) = 0          的r/ 尹 Z   and    j，凡Z，刃I E 7L.    (5.20)


기Lie wavelets ｛色 砂｝ are related to｛色 砂｝ as


                                         J)
                   ,   .   .    a   (n
                                                                                (5.21)
                  qw) =        匈(eIm)
and

                  仁（Ct)
                    ) =：出：)                                                     (5.22)

with
                                OO                         m
               夙（ejw) :＝乞 Ii(w+ 2兀k) j2= ＞二 A (k)ej" ',                         (5.23)
                               k=-oo                    k=-茯


where A (r) is the autocorrelation function of x (t). For a proof of (5.23), see Sec-
tion 7.6.1. Observe that the relation above is slightly different from the orthononnal-
ization relation (2.35) in that here we do not have a square root in the denominator.
In Chapter 6 we discuss the construction of all the scaling functions and wavelets
that we have discussed.
96      MULTIRESOLUTION ANALYSIS

5.3    TWO-SCALE RELATIONS

Two-scale relations relate the scaling function and the wavelets at a given scale with
the scaling function at the next-higher scale. Since

                                  中（t) e A0 （二 A1                               (5.24)

                                  少（t) e W0 CA1,                                位25)

we should be able to write 中(t) and *(t) in terms of the bases that generate A1. In
other words, there exist two sequences {go[k]}, {gi [kj} E Z 2 such that

                               中（t) =＞二go[k］砂（2t - k)                           位26)
                                      k

                               少（t) =＞二81[k］砂（2t- k).                           (5.27)
                                          k

Equations (5.26) and (5.27) are referred to as two-scale relations. In general, for any
j e Z, the relationship between A1 and W/ with A1+1 is governed by

                           中（21t) = ＞二go[k］砂（2j+'t - k)
                                          k

                           少（2't) = ＞二gi[k］砂（2/+1t - k).
                                          k

     By taking the Fourier transform of the two-scale relations, we have


                                 如印祠畔）                                          (5.28)

                                 *(w) = Gj(z)a（을）,                              位29)

where
                                              l
                                              d
                                 G0   口
                                      （
                                              小
                                              八乙
                                                  ＞二go[k］
                                                        乙k
                                                                                (5.30)


                                              l 4
                                                2
                                 G1                                             (5.31)
                                      Z
                                                  ＞二gi [k］寸

with     eejm'2. Observe that the definitions in (5.30) and (5.31) differ slightly from
     z=
those used in Chapter 2 for z-transform. An example of a two-scale relation for the
Haar case (H) is shown in Figure 5.3. Expansions of (5.26) and (5.27) lead to

                                的
                                n勻
                     中（nD ==
                                 如小環）                                           (5.32)
                                                             DECOMPOSITION RELATION                   97


       勿／(t) E A0                     勿?(2t) E A1                           中H(2t - 1) E A1
          1                                                                                 1

                                                                     +


   0                    1              0       1/ 2                              0   1/ 2         1




       砂H(t) E W0                     中g(21) E A1                          -砂11(2t - 1) E A1
        1

                                                                     4m
                                                                                 0   1/ 2         1
   0                    1              0       1/ 2




                -
                    1                                                                       -1
FIGURE 5.3 Two-scale relation for HaM case (g0[0] = golil = 1; gil0] = -gl[l] = 1;
g0[k] =g1[k] =0forallotherk).




                            仁（m)
                             (w) = G1
                                   G,.,P
                                      exp (- j '
                                          (1j으．)00
                                                 fl G。exp (- j윽' .                               (5.33)
                                           \   乙/     于 三        \        =7 /
                                                      t= =



Since the scaling functions exhibit the lowpass filter characteristic [中(0) = 1], all the
coefficients {go[k}} add up to 2, whereas because of the bandpass filter characteristic
of the wavelets (r (0) = 0), the coefficients {gi [k]} add up to 0.



5.4    DECOMPOSITION RELATION

Decomposition relations give the scaling function at any scale in terms of the scaling
function and the wavelet at the next-lower scale. Since A1 = A0 + Wo and 中(2t),
中(2t - 1) c A1, there exist two sequences ({ho[k]J, {h1[k]}) ine2 such that

               中（2t) = ）二｛ho[2k］砂（t - k) +hi[ 2k］少（t- k)}
                        k

            中（2t - 1) = ＞二｛九o[2k - 1］中（t 卞k)＋幻［2k - 1］少（r 1 丸）} .

Combining these two relations, we have

            中（2r -t）스二｛九o[2k -Z］中（r - k)＋幻［2k -t］少（t- k)}                                        (5.34)
98      MULTIRESOLUTION ANALYSIS



       中H(2t) E A1               勿K川2EA0                          」H(t)/2EW0




                                                                   =
       1
                                             1/2                     1/2
                             =           1             1   +



                                                                                   1
  0        1/2       1               0
                                                                   O
                                                   1


                                                                            -1/2

                                                                       毗   0
                                                                           W
       勿r (2t 小 1) e A1          中H(t)/2 E A0
                                 1
                                                                           E

                 1
                                             1/2                             1/2
                                                           +


                                     0
  0        1/2       1                             1                               1
                                                       r


                                                                    -1/2

FIGURE 5.4 Decomposition relation for Haar case (h0[0J = h0[ 1] = 1/2; h1[0J =
-h1[-1] = 1/2; h0[k] = hi[k] = 0 for all other k).



for all Z E Z. In gener고, we have


      中（2j"卜Z) =＞기ho[2k -t］中（2js- k)＋幻［2k -t］少느Vt -이· (5.35)
                         k

Figure 5.4 shows an example of decomposition relation for the Haar case (H).



5.5    SPUNE FUNCTIONS

One of the most basic building blocks for wavelet construction involves cardinal B-
splines. Complete coverage of spline theory is beyond the scope of this book. In this
section we describe briefly spline functions and their properties that are required to
understand the topics discussed in this book. For further details one may refer to
many excellent books (e.g., [4-8]).
   Spline func如ns cons奴 可piece刊ise polynomi出s (see F增止e5.5）如med together
smoothly at the break points (knots: to, tl, .. .), where the degr of smoothness de-
ponds on the order of splines. For cardinal B-splines, these bre points are equally
spaced. Unlike polynomials, these form local bases and have        y useful properties
that can be applied to function approximation.
   The mth-order cardinal B-spline Nm (t) has the knot seque       {. ..,-1, 0, l, .. .}
and consists of polynomials of order m (degree m - 1) between the knots. Let
Ni(t) = x[o, 1) (t) be the characteristic function of [0, 1). Then for each integer
m 之 2, the mth-order cardinal B-spline is defined, inductively, by
                                                                                                              SPLINE FUNCTIONS       99



 f (t)




                         I                       I                                                        1                I >   1   t
         to              t1                      t2                                                       i3               t4
                     FIGURE 5.5 Piecewise polynomial functions.




                       川 (t) := (Nm_i 水 N1)(t)                                                                                   (5.36)


                                    :=
                                    :=       J
                                             too
                                             - 。O        Nm_        i   (t       -        x)   Ni   (x)       dx

                                    크                 'Nm_     i   (t        -       x)        d兀                                (5.37)
   A fast computation of Nm (t) form > 2 can be achieved by using the formula [7,
p. 1311


                 Nm(t) = 石늙如(t)＋岩 Nm크아1)
recursively until we arrive at the first-order B-spline N1 (see Figure 5.6). Splines of
orders 2 to 6, along with their magnitude spectra, are shown in Figure 5.7. The most
commonly used splines are linear (m = 2) and cubic (m = 4) splines. Their explicit
expressions 缸e

                                                        t,                           tE[ O, l}
                                                                                     r E[1, 2]                                   (5.38)
                             ,:(,                              ，
                                                                                     elsewhere
                                                 仁》
                                        )＝
                                                  10,
100       MULTIRESOLUTION ANALYSIS




                              N小）

                               1




                               0
                                    0                   1        t

                         FIGURE 5.6         N1, the spline of order 1.




j
                         Ni (t)

0                                                     0
 0                                      1            -20       너0                   10         20
1                        N2(t)                        l                         1/V2(m) 1


0。                                                    0
                                                     -20       너0        0          10         20
1                                                     l


0。
                                                                                               20
1


0。
                                                                                               20
]


0。
                                                                         0          10         20

                                                                         /\
1
                                                                               凶.
                                                                                     (w)
                                                                                           1
                                                      0
      1      2     3    4      5        6            -20      -10        0          10         20
                 FIGURE 5.7    Spline functions and their magnitude spectra.
                                                                       SPLINt FUNCTIONS           101



                          仁 12t+ 12t2- 3t3,
                N4(t) = 卜44 + 6야 - 24尸 +3尸，
                                                                       t E [0, 1]
                                                                       t E [1, 2]
                                                                       t E [2, 31
                          J
                                                                                             (5.39)
                         64- 48t+ 12t2- t3,                            t E [3, 4]
                          to,                                          elsewhere.

   In many applications we need to compute splines at integer p아nts. Table 5.1 gives
spline values at integer locations. The symmetry property can be used to get values
at other points.
   To obtain the Fourier transform of Nm (t), observe that (5.36) can be written as


                                    Nm(t) = (N1 * . . . * Ni)(t).                            (5.40)
                                             나口H/
                                                           m


Therefore,

                                             _e Jw\ m
                                    刃, 佃）나l1 m:
                                              JU)   \      /       )                         (5.41)


since

                         八
                         Ni   (w)
                                      =
                                          7b
                                           ci
                                          J。
                                             e
                                              ... ,.' 山
                                                     dt'
                                                        1- 可3W
                                                          fIn  =
                                                                                             (5.42)




TABLE 5.1 Cardinal B-Splines at Integer Points

         (m - 1)!Nm(k)                                                                (m - 1)!Nm(k)
             m= 3                                                                        m = 11
l               l                                              l                                 l

                                                                           n
                                                                           二 n
             m= 4
                                                                             J 4
                                                            120                             1,013
l                 l                                       1,191                            47,840
2                4                                        2,416                           455,192
                                                                           <
                                                                           U
             m= 5                                        m= 9                           1,310,354
l                l                                            l                          m = 12
                                                                          l
2               11                                          247                                  l




                                                                          n
                                                                          乙 n
             m= 6



                                                                            J 4
                                                          4,293



                                                                              1 <
                                                                                U A
                                                                                            2,036



                                                                                  U
l                l                                       15,619                           152,637
2               26                                      m = 10                          2,203,488
3               66                                            l                         且738,114
             In = 7                                         502                        15,724,248
l                l                                       14,608
2               57                                       88,234
3              302                                      156,190
102                 MULTIRESOLUTION ANALYSIS

    The important property of splines for our pur兀ses is the fact 蜘t they are scaling
l==14 m1: h4 n        mn= n1 : n                              11= m小m 小＝4n               n nm ‘느 . 1 八d4 八n r 八 t-.__                             I_ fl                    -中 刃2_..八1.



IUIIeU%jiIS.          IlitiL                IS, UICIC fl y
                                                      CAISLS "                    SC4U少 r tOt
                                                                                            L ", IT
                                                                                                  ', ILJJ"
                                                                                                       ,fl_
                                                                                                         .  ", L " U "I1 Ui L                                                                                                                               IC    Afl\
                                                                         lVm tr, = 2日goLm, 凡J "mt'i - 凡J "                                                                                                                                                  LJ "냐JJ
                                                                                                     -




                                                                                    k

In Chapter 6 we derive an expression for go[m, k].


5.5.1               Properties of Splines

some important properties or spnnes, reievant to me topics aiscussru in.mis OOOK,.are
aiscussea in mis section witnout giving any proof. rroois or som or we propemes
are ieit as exercises.

      1. Supp Nm = [0, m] with Nm(0) = Nm(m) = 0.
      2.       e ' '+ C'
             Nrn.     (t)     the space of functions that are k tmes continuously
                                            .   C                   2;          is
      .



            airlerentlaDie.                                                          ,        m          .             . .                    .                              .        .                           .             .                      ,    .      .




      .).k+  l)
         IVmI打k]    " am- K " " .                                          i,                     7f is me                       poiynonuai                                               space          pi                uegree                      Ic       oruer

      4. 1아J N...(tIdt= l.
      5. /V軸뇨向小Nm小口）.
      6. Nm(t) is symmetric with respect to the center t'T = m/2, tifiat is,


                                                                         Nm（끌＋!)=Nm（冬《）,                                                                                                   tE 皿                                                             (5.44)


      7. Nm(t) behaves as a lowpass filter [Nm (0) = 1; see Figure ; 7]                                                                                                                                            .                .




      8. Nm(t) has mth order of approximation in the sense that J m (w) satisfies the
         Strang-Fix condition

                     ！匈9=       l
                     11 '1\1m(27rt) = 0,                                                          ke 兀 \ ｛아                                           and
                                                                                                                                                      md                          j= l
                                                                                                                                                                                 /=         l,   ,   .   J    .        ,   ml
                                                                                                                                                                                                                           m-                 l,
                                                                                                                                                                                                                                                   ,        (5.
                                                                                                                                                                                                                                                                  45)

            where D'          the jth-order         denotes                          loc出ly re-          derivative·                              ，        Consequentiy{                                          Nm                    (t)
      . prouuces an poiynomiais or oruer m tsee to, .pp. i i '+-IbIJ?.
      9. ) ,. iV.,,tt - k ) 三 I for all t. 1fli5 nronertv is referred to as me  . partition
                                                                                         . . or.
            11日1느           "       '   "                       "                                                      1     1                    1




    .    unziy, propert.y.     ..                  .    .        .      . .      .     .. . .
    It)" 떠叩兀)SItZV町如(t)           .之 U, fort   E . LU, 刃ii. tiy,virtue or u．르total positivity 山，
            p., 시 pr叩텍恥小叩tines, coeflic뺍的Ia 步叩tine se畔 follow tne snape
            or tne aata. ror instance, ii g(1J = 乙 aJIV (r - J), Lfleflf

                                                                                              a/ 三 0 "If 수 g(t) 三 0
                                                                                af 令 (increasing) ＝수 g(t) 十
                                                                                              aj (convex) 수 g(t) convex.
                                       MAPPING A FUNCTION INTO MRA SPACE            103

       Furthermore, the number of sign changes of g(t) does not exceed that of the
       coefficient sequence {aj). The latter property can be used to identify the zero
       crossing of a signal.
   11. As the order m increases, Nm (t) approaches a Gaussian function (AN,,, A刃, -
       0.5). For instance, in the case of a cubic spline (m = 4), the R卜4S time叫
       frequency window product is 0.501.


5.6   MAPPING A FUNCTION INTO MRA SPACE

As discussed in Section 5.2, before a signal x(t) can be decomposed, it must be
mapped into an MRA subspace AM for some appropriate scale M, that is,

                      工(t) -*工M(t) 4그k,M b(2也- k).                                (5.46)
                                            k
Once we know {ak,M) we can use fast algorithms to compute (ak,s} for s <M. Fast
algorithms are discussed in later chapters. Here we are concerned with evaluation of
the coefficients {ak .M}.
   ii X(t) is Known at every t, we can ontain jak,MJ ny me orrnogonai projecuon IL日
projection) of the signal, that is,


                        따，M= 2"乙而（2"卜，
                                     ）力·                                          (5.47)

However, in practice the signal x(t) is known at some discrete points. The given time
step determines the scale M to which the function can be mapped. For a representa-
tion such as (5.46), we want it to satisfy two important conditions: (1) interpolatory
and (2) polynomial reproducibility. By interpolatory representation we mean that
the series should be exact, at least at the points at which the function is given, mean-
ing that x(k/2M) = xM(k/2M). As pointed out before, polynomial reproducibility
means that the representation is exact at every point for polynomials of order m if
the basis 中(t) has the approximation order m. In other words, x(t) 드 工M(t) for
x(t) E 兀_1. Cardinal B-splines have m order of approximation. In addition, since
they are a local basis, the representation (5.46) is also local. By local we mean that to
obtain the coefficient ak,M for some k, we do not need all the function values; only
a few, determined by the support of the splines, will suffice. The coefficients when
中(t) = N2(t) and 砂(t) = N4(t) are derived below.

Linear Splines (m = 2) Suppose that a function x(t) is given at t = 112M : Z E Z.
Then to obtain the spline coefficients {ak,M } for the representation

                     工（t) -수工M(t) =＞二口k.M N2(2Mr - k),                            (5.48)
                                           k
we apply the interpolation condition, namely

                                 (유）=XM (i유）·                                     (5.49)
104      MULTIRESOLUTION ANALYSIS


By using (5.49) along with the fact that

                    N2(l) = 1 and N2(k) == 0,                                                             k e Z \ {0},    (5.50)
we get


                                          따，
                                                       M=
                                                                    X
                                                                        （츠꿋）
                                                                                                      ·
                                                                                                                          (5.51)
The representa如n (5.48) preserves all polynomials of degree at most 1.

Cubic Splines (m =4) In this case

                      工（DH工MO) 4그k.MN4(2也- k),                                                                            (5.52)
                                                                        k

where [4, p. 117]
                                                k+6                                            .          -
                                                t小                                         /              Ti    \
                             ak,M =             L                   Vk+2_ 2月 兀 \5i；
                                                                                  二i)
                                               n=k- 2                                                 -

and


                                                            四餌 7侄
                                                                                   n= 0
                                                                                   n = 士1
                                                                                   n == 士2
                                   vn =
                                                                                   n = 士3

                                                                                   n == 士4
                                                                                   otherwise.
The representation (5,52) preserves all polynomials of degree at most 3.


5.7   EXERCISES

1. For a given j E Z, a projection P2, f (t) of any given function f (t) E
   L2(- 以）, 以）) onto the hat function space
                                     的


                     匕                                              (23t       -    k) :                      k. Z E《21
                              Ik=-oo
                         =
                              1乶
                                                CkN2
                                                                                               {Ck}
                                                                                                                      J

  can be determined by the interpolation conditions P2,f f (k/2J) = f (k/2J) for all
  k E Z. Find the formulas for the coe砥ients {an } if P2,J/ is written as
                                                                    的

                             尸幻f(r) = Z 따N2(2jt -兀）·
                                                               n=＝小的
                                                                                                                                        EXERCISES   105

2. FortheHaar 砥／av（三It艾




                                     『的）           ::
                                                             N1    (t)
                                                                               =
                                                                                           {!,1
                                                                                                                 朴，
                                                                                                                             [0, )
                                                                                                                               ,   1)
   define

                                     勿／,k，小）=2s/2砂H(2st_ k),                                                               k, s eZ.

   Show the orthogonality relations
              I.
                   아그        .   ,          ...     ,                    ...           .          ,         ,

              /          甲月，k,st') 甲J了，m, j八ii Ut = ('m,k(Js,p,                                                             m, k, p's E Z.
             1/ 나 （X)




   Due to these relations, we say that the set {少月,k,: lk.SEZ forms an orthonormal
   family in L2(- 以그, 的）.

3. Show that the Gaussian function 中(t) = e_t2 cannot be the scaling function
   of a multiresolution analysis. (Hint: Assume that e_t2 can be wri仇en as e t2 =
    :及m ake (2tmt)' for a sequence {ak}kEz inZ2, which has to be true if e_ 2 E
   V0 C V1. Then show that this leads to a contradiction by taking Fourier transfonns
   on both sides of the equation and comparing the results.)
4. Show that the mth-order B-spline Nm (t) and its integer translates form a partition
   of unity, that is,

                                            的
                                            ZNm(tUk) =1                                                         的r all 兀 e R.
                                           t=＝니乂


   (Hint: Use Poisson's sum formula.)

5. Show the f에owing 叩m妃try pr아尼rty 可 Nm(t)


                                     Nm愕卄）= Nm（冬小                                                                          工 E R.


6. Use Exercise 5 to show that


             Jfoe
               -
                。O      Nm
                                     (t+
                                                  k)    Nm
                                                             (t)
                                                                         dt        =
                                                                                           Nm         (m+
                                                                                                                      k)    foranyk
7. Show that the hat function

                                                  M                i 0                                 如r tE[ 0, l]
                                                                    H
                                                                    )
                                                                                       t               for tE[ 1, 2]
                                                                                                       otherwise
106      MULTIRESOLUTION ANALYSIS


     and the function Ni (t) are related by convolution: N2(t) = Ni (t) * N1(t). Find
     the defining equations (the polynomial expression) for the functions given by


                           八／3(t) :== N2(t) 米 /V1(t)

                          N4(t) := N3(t) * Ni (t),      rE li .




5.8     COMPUTER PROGRAMS


5.8.1    B-Splines

g
% PR0GRAM Bspline. m
老
돔 Compu七E크S I그nif arm Bsplines

function y = Bspline (m, x)


y = 0;

왕 Characteris七:i亡 fun（比ion

if     m == 1
     if x >= 0. 0 & x < 1. 0
        y = 1. 0;
     else
        y = 0. 0;
     en（크
end

% Higher order

a = zeros (1, 500) ;

if    m >= 2 & m < 100
     for k = l; m- l
       a (k) = 0. 0;
       xl = x - k + 1;
       if xl >= 0. 0 & xl      < 1. 0
          a (k) = 그＜1 ;
       end
       if xl >= 1. 0 & xl      < 2. 0
          a (k) = 2 卞 xl;
       end
     end

     for p=l: m- 2
       for q=1: m-l- p
                                                                       REFERENCES       107


      a (q)      = ( (x-q+1) * a (q) +(p+q+1_x) *a (q+1) )             / (p+l) ;
    end
  end

  y = a (1) ;
end



REFERENCES

1. Y. Meyer, Wavelets: Algorithms and Applications. Philadelphia: SI사느4, 1993.
2. S. Mallat, "A theory of multiresolution signal decomposition: the wavelet representation,"
   IEEE Trans. Pattern Anal. Machine Intel!., 11, pp. 674-693, 1989.
3. S. Mallat, Multiresolution representation and wavelets, Ph.D. thesis, University of Penn-
   sylvania, Philadelphia, 1988.
4. C. K. Chui, An Introduction to Wavelets. San Diego, Calif.: Academic Press, 1992.
5. I. J. Schoenberg, Cardinal Spline Interpolation, CBMS Ser. 12. Philadelphia: SIAM, 1973.
6. L. L. Schumaker, Spline Functions: Basic Theory. New York: W如y-Interscience, 1981.
7. C. de Boor, A Practical Guide to Splines. New York: Springer-Verlag, 1978.
8. C. K. Chui, M岫加口月口招 卵line工 CBI뇨'IS-NSF Ser. Appl. Math. 54. Philadelphia: SI사'4,
   1988.
CHAPTER S仄




Construction of Wavelets

In this chapter we are concerned with the construction of orthonotmal, semiorthog-
onal, and biorthogonal wavelets. The construction problem is tant mount to finding
suitable two-scale and decomposition sequences as introduced in I 'hapter 5. It turns
out that these coefficients for orthonormal wavelets can easily be c =rived from those
of semior仕ogonal wavelets. Therefore, we first discuss the semio thogonal wavelet
followed by orthonormal and biorthogonal wavelets.           N
   匙帥 如tf아毗 配岫orthogonal wavelet, both中(t) and 叭t) a e in A0, and *(t)
and 少(t) are in W0. Consequently, we can write 中(t) in terms of 1 巾); similarly for
*(t). These relations as given by (5.21) and (5.22) are


                                                                                               (6.1)
                                      ,   .     .        q      (w)
                                  叭           (i)) =    E中   （eJm)
and

                                 知）                 :   E*           (eJ   '   )   ,           (6.2)

with the Euler-Frobenius-Laurent polynomial E1(eJn)) given by


                万／(e30') := ＞二 1f (w+ 2兀시2= ）二 사（ej0J                                          (6.3)
                            k=-oo                                                      k=-oo

We will, theref。 re, c。ncentrate 。n the c。
                                         nstructi。n 。f中 and 少 。nl1
   As the first step toward constructing wavelets, we express {ho [k]},{h1[kj}, and
{gi [k]} in terms of {go[k]} so that only {go[k}} and hence the scaling functions
need to be constructed. jn semiorthogonal cases, all these sequences have differ-
ent lengths, in general. Later we will show that for orthonormal (:ases, all of these
sequences have the same length and that there is a very simple rehLtion among them
which can easily be derived as a special case of the relationship fc1r semiorthogonal
cases. The cons仕uction of a semiorthogonal wavelet is followed b./the construction
of several popular orthonormal wavelets: the Shannon, Meyer, Bal:tle-Lemarie, and
Daubechies wavelets. Finally, we construct a biorthogonal wavelet

108
                        NECESSARY INGREDIENTS FOR WAVELET CONSTRUCTION              109

6.1     NECESSARY INGREDIENTS FOR WAVELET CONSTRUCTION

As p여nted out before, we need to obtain the coefficient sequences {go[k]} and
{gi [k]} to be able to construct wavelets. In this section our goal is to find a rela-
tionship among various sequences. This will help us in reducing our task. Here we
consider the case of semiorthogonal decomposition of a multiresolution space.


6.1.1    Relationship Between Two-Scale Sequences
Recall from Chapter 5 that as a result of the multiresolution properties, the scaling
functions and wavelets at one scale (coarser) are related to the scaling functions at
the next-higher scale (finer) by the two-scale relations, namely

                             中（t) =＞二go[k］中（2t卜k)                                  (6.4)
                                    k

                             少（t) =＞二gi [k］中（2t - k).                              (6.5)

By taking the Fourier transform of the relation above, we have

                                   a(w) =
                                    (m)=G.(:
                                          Go(z)b
                                             ）畔\ ( )                               (6.6)
                                   如斥毗미朴
where z = emjU)/2 and

                              Go
                                       (z)
                                                 :=
                                                      {    K
                                                               go[k]z"             (6.8)
                                                      1
                                                      1
                                   G         （
                                                      H
                                                      2   ＞二gi [k］寸                (6.9)
                                             月



                                                           k
Observe that 中(t) c A0, 砂(2t) c Ai, and 砂(t) E W0. From the nested property of
MRA we know that A0 C Ai and A0 上 W0 such that A0 q) Wo = A1. Orthogonality
of the subspaces A0 and Wo implies that for any Z E Z,

                                   (中(t - t ), 少(t)) = 0.                         (6.10)
Equation (6.10) can be rewritten using Parseval's identity as

             .：打：8(0）可"' 而)dw
             극，/：如m카枷Hjtw dw
             ：押／ ,',:"""G毗）乙而8（判"                                        rjtmdw
110                CONSTRUCTION OF WAVELETS



                                    =51Jo/"" Go(z）可石j18但．+2兀k')1
                                  = 乙it＝              1 ＼乙
                                                                'e-'                                                                          dw
                                        日

                                     1 r 4끄 ,, . .;====
                                  = ;1 r             G0回酉面民(z)戶Zmdm,
                                                     (r0（乙八'1（乙J                                                                                                 (6.11)
                                    'Jr J0

where
       z =     刈2. By partitioning the
                            e_
                                                       limit [0, l into [0,.2兀j and
                                                                             integration
                                                                                                                              4jr.
 2兀, 41rJ, ana wiUi a simple cnange or variaoie, it is easy to veriry mat o.li) is me
same as
         1 f2兀 n, . .====,, . S . ,, . . ,, . . n . . ] Hi
        :;= I  I '아z八11位n如（乙) 十 (J0(m乙八n (1乙'I二中（H乙J 1 e " dw= 0. (6.12)
        乙Jr j0              L                                                                                             J

The expression (6.12) holds 出l Z E 7Z. What does mean,? To understand this,
                                                      for            .   .                               .   it
let us recall mat an miegrarne zir-penoaic runction j (t) nas rae 'ouner senes rep-
resentation

                                              f (w) = Z ctejt(),                                                                                                     (6.13)
                                                                 f

where

                                                     Cl긍，工" f(w）戶"如·                                                                                                 (6.14)

From - the above it is clear that the quantity on the left of j (6.12) .represents
쁘e. t th, Foun뜨 .coet끄드ient .or. a perioaic . function (i斗乙)(ii(Z)1工．
                                                                   中（之) 十
(叭-z)(ii- Z)亡t- Z). since all mese coemcients are zero, it 1꾸p11es m1lat

                                   Go(z)Gi回E比）+ Go(- z石i(- z坦d-z)                                                                                                    (6.15)

for Izi = 1.
   The solution of (6.15) gives the relationship between Gi(z) an Go(z). By direct
substitution, we can verify that

                                             Gi(z) = -cz2"+1Go(- z)E (- z)                                                                                           (6.16)

for any. integer m, and a constant c.> 0 is a solution (6.15). 찌岫out any loss of
generality we can set c = 1. 1ne errect oi rn is,to snirt me inux or me sequence
jgll尺JJ. usually, m is enosen sucn mat tne inuex negins wimn u.

6.1.2             Relationship Between Reconstruction
                        1    r\              1 1 1          in

.        .   .   .ano       uecomposirion ' equ.ences                                      . .       』            』   ．              ,   .,        .             .        ,




Kecali Irom Lnapter 그 mat me scaling lunction at a certam,scaiq (nnerJ can oe ou-
tainea irorn me scaling runcuons ana waveiets at me next ioweiT Icoarse)                         .                                                     .scaie.          ,in




matnematical terms, it means mat tnere exist nnite-energy sequences tno uq j, tn i 1K] j
sucn tnai

                        中（2t - Z) = ＞二｛九o[2k 놔 t］中（t - k) +hi[2k -t］少（
                               NECESSARY 八GRED炬NTS FOR WAVELET CONSTRUCTION                                                                   111

where, as discussed in Chapter 5, {ho[k]} and (hi[k]} are the decomposition Se-
quences.
  By taking the Fourier transform of the decomposition relation, we get


    1-.（읒') e.j0t/2 = 5m.h0[2k -Z]e_jk怖(w) + )'h1[2k
    乙       \ 二/                =r=
                                 凡
                                                                                                    니
                                                                                                     K
                                                                                                                 -Z]..jk唾（m)

            나G0(z）工』o[2k-(]r加* G1(z)＞二』i[2k‘《］.-，나 訂의．
                   I.      k
                           凡                                                                尺
                                                                                            k                             J
                                                                                                                              "   '
                                                                                                                                       'I
                                                                                                                                      '-




The equation above reduces to


   位出- 1戶如如미口似－《］戶(2k_t)w/2) G1(z)
    \   k                                    I                                   \k                                           I


                                                                                 4
                                                                                 l Hn
                                                                                    乙
                                                                                                                   =
                                                                                           VtEZ.                                            (6.18)

  Combining the Fourier transfonns of the decomposition and two-scale relations,
we get


                    [Ho化나耶'叱昞(z)印玉(z) + Hi(-z)]G向' 근
                                                                                                                     2
                                                                                                             for event;                    (6.19)
                    [H (z) - Ho(- z)]Go(z) + [Hi(z) - Hi(- z)]Gj(z) = 0

                                                                                                             for oddt,                     (6.20)

where z = eHjn)/2 and



                                      Ho         (z)
                                                        :=
                                                                      ｛二6.               [(]:'

                                      Hi         (z)
                                                                  ＝
                                                                      泣h1[
                                                                             K
                                                                                         k］乙

These equations lead to


                                  Ho   (z)
                                                       Go   (z)
                                                                        + Hi       (z)
                                                                                         Gj   (z)
                                                                                                         =
                                                                                                             三
                               Ho(- z)Go(z) + Hi(- z)Gi(z) = 0.

The last equation can also be written as

                               Ho(之)Go(- z) + Hi(z)Gi(- z) = 0.                                                                            (6.21)
112      CONSTRUC기ON C汗 ＼八／AVELETS

   In matrix form we have

                       rG0（乙） Gl（기 그 rHo(z）그 rr
                                                                                                                                                    (6.22)
                       [Go(-z) Gi(-z)J ［月i(z)J                                                                                         ［으
the solution of which gives

                                                    1               （키（-z)
                         Ho(z) =                                x                                                                                   (6.23)
                                                    2               八G。G1 (z)
                                                    -
                          Z                               1            Go(- z)
                          月                                                                                                                         (6.24)
                                          = -                       >< 스G, G, (D

with
                     스G。G1(Z) = Go(z)G1(- z) - G0(- z)Gi (乙).                                                                                       (6.25)

  It can be shown that

                                          AG0GI（乙） =c尹月中（z2),                                                                                       (6.26)

where c > 0 and m is an integer. Since 中 generates a Riesz or s able basis, E0 (z)
and hence LG0G1(Z) ;E 0.


6.2    CONSTRUCTION OF SEMIORTHOGONAL SPLINE WAVELETS

The significance of the results obtained l             that we1need to construct
                                                                      .   in.            Section                 6.   1   .   .   is
                                                                                                                                            ,   .



omy me scaling runcuons (i.e., we neea to nnu. oniy me sequenLe tgOLKJL). in tHis
se띤엑we oo帥mese sequences iortne. 뙨mo.rtnogonai spun印싸,.eie跏．町恤，ceo
Dy LflU1 anti, wan.l,g t'j. 1-lere me caruina! Li-spiines iVm ar.e cnosei to oe me ,scaiing
Junctions, we wan snow mnat a finite-energy sequence tgolm, KJJ 9x1sts sucn mat we
s注iiing reiauon

                           Nm
                                    (t)         =
                                                         >g0[                   m,                 k]Nm    (2t            -            k)           (6.27)


is satisfied and therefore N.,,(t is a scaling function. Form = 1. (N (t - k) : k e ZI
rorm an orrnonormai nasis O1 A0. ror mis case we nave aireauy seen mat gotul =
go[lI = 1 (see Figure 5.3). In this section we consider cases for which m 三 2.
    For m > 2, the scaling functions {Nm (t - k) : k e Z} are no longer orthogonal;
that is,

                                J
                                pOO
                                -   。。
                                           Nm
                                                        (t)
                                                                    Nm    (t
                                                                                     -             《) dt                                            (6.28)


for all Z e Z and m > 2. An example of nonorthogonality of N2( ) is 計山＼vn in Fig-
ure 6.1. The f    N2(t)N2(t - )dt is shown by the shaded area, which is nonzero.
                         CONSTRUCTION OF SEMIORTHOGONAL SPLINE WAVELETS                                                           113


                                    N2(t)                                 N2(t - 1)




                   0                     1                                                     2                  3
            FIGURE 6.1 Nonorthogonality of linear spline shown by the shaded area.




 6.2.1 Expression for {g0[k])
Recall from the definition of Nm (t) in Chapter 5 that

                                    Nm(t) = (N1 * ...*N1)(t)


 and that


                                                                                                                               (6.29)
                                    1m
                                              (W)
                                                                    (1_
                                                                                   3Cr)
                                                                                          eJT
                                                                                          ,

From the Fourier transform of the two-scale relation, we have



               Go(z) =；二8.［《，(]:'＝쿠二,（:;                                                                                       (6.30)

                                                                                                  12)
                                                                                           +e_1(0)
                                                                                                            \m
                                                                              k                             )
                                                                              fi
                                                                -




                                                                                                        2
                                                                                                                         加／2
                                                                = 2nl                              + 乙）m         z= e


                                                                =2名（分'·                                                        (6.31)


By comparing the coefficient of powers of z, we get


                                                                          "        '                        0< k< m
                                                                                                                               他32)
                                         幻＝
                   駒肉：
                                                    12
                                                                                          (:
                                                                                                   ),
                              如伽，
                          ：
                                                     I0,
                                                           0,
                                                                                                            otherwise.

   Once we have {go[k]}, the rest of the sequences {gi [k]}, {ho[k]}, and {hi [k]J can
be found by using the relations derived in Section 6.1. The expression of {gi[k]} is
derived below.
114     CONSTRUCTION OF WAVELETS

  For Nm (t), the Euler-Frobenius-Laurent polynomial EN, , (z) takes the form


                          EN, ,(Z) = 多. 1刃, 仁．+2irk) "               1         \ 乙          /
                                             k=-cc
                                                   11日




                                                                         m
                                                         m
                                                         Z
                                                                         A     1
                                                                               k
                                                         如
                                                    rn           I

                                                   ＞二
                                                             -
                                                                                                               (6.33)
                                         =                               N2m       (m+   k)Z'
                                             k=-rn+1

with z := e_ J(D12 and the autocorrelation function

               AN,,,(k)   =   J:
                                   Nrn
                                             (x)
                                                             Nrn (k +x)dx = N2rn                (m
                                                                                                     +k)   .   (6.34)

Finally, by using the relation (6.16), we have


          gi[k] := gl[m, kj = ( 1)k . 2m+1
                                                                               客（加小山， (6.35)
                                                                                            0< k 드 3m 小 2.     他36)

Remarks: Recall that in the expressions for Ho(z) and H1(z), in terms of Go(z) and
Gi (z), there is a term 스 G。G1(z) = ZmEN (z) in the denominator. Consequently, the
sequences {ho[k]} and (h1[k]} are infinitely long, although their magnitude decays
exponentially. These are the sequences that will be used in the development of de-
composition and reconstruction algorithms in Chapters 7 and 8. It is clear that while
G0 and G1 form FIR filters, H0 and H1 are always IIR. We will, however, prove
in Chapter 7 that we can use G0 and G1 for both reconstruction as well as decom-
position purposes. This is a consequence of the duality principle that we mentioned
briefly in Chapter 5.
   The commonly used cubic spline and the corresponding semiorthogonal wavelet
with their duals and magnitude spectra are shown in Figures 6.2 and 6.3. See Chap-
ter 10 for the expressions of commonly used semiorthogonal scaling functions and
wavelets. Table 6.1 gives the coefficients {gl[m, ki) form = 2 through 6.


6.3   CONSTRUCTION OF ORTHONORMAL WAVELETS

Recall from Chapter 2 that the Riesz bounds for orthonormal bases are 1. Therefore,
for o曲onormal scaling functions 中 and the corresponding wavelets 砂, we have

                          民（「／功）= 刃a(w + 2兀k)I2 三 1,
                                                     k

                           「씨 = Z M佃＋2兀k下 三 1,
                          白（
                                  CONSTRUCTION OF ORTHONORMAL WAVELETS                115




       0
   -
       1
           -1   0   1    2    3      4               0          10        20          30
FIGURE 6.2 Linear spline, dual linear spline, the corresponding wavelets, and their magni-
tude spectra.



for almost all cv. Consequently,

                          中（t) == 中（t)     and   少（t) = 少（t);

that is, they a七 self-duals. Remember from our discussion in Chapter 5 that because
of the nested nature of MRA subspaces, the scaling functions a亡e not orthogonal with
respect to scales. Orthonormal scaling functions imply that these are orthogonal with
respect to translation on a given scale. Orthonormal wavelets, on the other hand, are
orthonormal with respect to scale as well as the translation.
   By starting with

                                  (砂(t -t) ,砂(t)) = cS0,t                          (6.37)
116       CONSTRUCTION OF WAVEIETS




  0.2
      0
 -0.2
      0          2          4




             0       2     4    6    8
FIGURE 6.3 Cubic spline, dual cubic spline, the corresponding wavele s and their magni-
tude spectra.



and following the derivation of (6.12), we arrive at the following r; suits:

                           1Go（之） 2 + IGo(- z기2 三 1,     IzI = 1.               (6.38)

For orthonormal scaling functions and wavelets, the relationships. ong the various
sequences {go[k]J, {g1[k]}, {ho[k]}, and {h1[k]} can be obtained f om the results of
Section 6.1 by setting m = 0. These results are summarized below

                           Gi(之) = -zGo(- z)
                                          [l - kj;
                         수 gi[k] = (_ 1Y'g。                                     (6.39)

                       ,G1(Z) = Go(z)Gi(- z) - G0(- z)G1(z) = 4
                     1G。                                                        (6.40)
                                                      CONSTRUC지이니 OF ORTHONORMAL＼사AVELETS                                                          117

 TABLE 6.1 Coefficients Um,k := 2m-l (2m - 1)! gl [m, k] for the Semiorthogonal Wavelet
 (gi[m, k] == (- 川눙山n, 3m 寸 2 - k])

 k                                        k                                            Um,k                           k
             Urn
                                                                                                                                            Um1k
            m-=2                                                                       m= 5                                                m= 6
   0                                          0                                                                        0
                    l                                                                       l                                                        l
  ]
  1 n
    乙


                                          1
                                          1 n
                                            乙 그1나 4


                                                                                                                      111 n
                   6




                                                                                                                          乙 八4나 d
                                                                                        -507




                                                                                                                                1 <
                                                                                                                                                -2,042




                                                                                                                                  U 6
                   -
                  10                                                                   17,128                                                  164,868
            ／札 = 3                                                                  -166,304                                               -3,149,870
  0
                   l                                                                 748,465                                                25,289,334
  l

                                          <
                                          J 6
                -29                                                               -1,900,115                                            -110,288,536
  八
  乙 八4U
                 147                                                               2,973,560                                              296,526,880
                                                                                                                      7 8
              -303                                                                                                                      -525,228,384
 0
            m= 4                                                                                                                          633,375,552
                   l
 l
              -124



 n
 乙 2
   U d
     1 <
       U
              1,677
            -7,904
             18,482
           -24,264



                             Ho(z) +                                       「 ' (" )＋瓦面

                        수力0                                                                                                                   (6.41)
                                   [kJ=
                                                           三go[
                                                                           -kl;
                                   (7)                                 1 /
                                                                                                             l

                             m
                             H1                                                                              mn
                                                                                                              乙
                                                                                                                  X
                                                =
                                                                                       (-
                                                                                                z
                                                                                  Go
                                                                         x
                                                                       7
                                   (z)
                                                =
                                                       -               -                            )
                                                                                            7           =
                                         k]                                1)kg0[k
                        ='                     =                                   +                                                          (6.42)
                                                       2                                                11
                             hi[
                                                       _
                                                                  (_
As an example, for a Haar scaling function and wavelet (see Figures 5.3 and 5.4) ,

             go[0] = go[l] = 1

             gi[0] = 1, gi[lj = -1
                             l
             ho[0] = h0[lJ = -
                             2

             hili0l＝二 /i[l]＝긍
             go[kl= gi[k] =ho[kl= hi[k] =0                                                                    VkeZ\ {0, 1}.

Remarks: One of the most important features of orthonormal bases is that all of
the decomposition and reconstruction filters are FIR and have the same length. This
helps tremendously in the decomposition and reconstruction algorithm discussed in
118     CONSTRUCTION OF WAVELETS

Chapter 7. One of.the disadvanta.ges of orthonormal wavelets is 巾at they generally
Go iiOt nave ciosea-Lorm expressions, nor uoes a compactly suppPrLeu oruionormai
wavelet nave a linear. pnase (no. symm.letry). me importance oi a linear .pnase』.in
signal reconstruction is aiscussecl in Unapter Lit nas also oeen $flown I乙] tnat me
higher-order ortlionorinal scaling lunctions and waveiets nave po)r time-Irequency
localization.



6.4 ORTHONORMAL SCALING FUNCTIONS

In this section. we discuss the commonly,, used. orthonormal .watelets of Shannon,
Meyer, lj arn.ne-Lemane, ari.a uauoecnies. we will aeri.ve orny m1le xpressions.br me
sequence {goLk]J since otner sequences can be obtained Irom 따e relationships ot
becuon 0.1.



6.4.1 Shannon Scaling Function
The Shannon sampling function

                                      未  /. \ . sin兀t
                                      WSH\1) ·＝ Hm卜                              (6.43)
                                                  7rr


is an orthonormal scaling function with 中sH(w) = X(-兀, 兀) (w).        ving the orthogo-
nality of (6.43) in the time domain by the relation

                                 仲SH(t - Z), 中SH(t)) = ao,e                      他44)

is cumbersome. Here it is rather easy to show that the Riesz bounds are 1; that is,

                                 ＞二侈SH(W + 2兀k기2三1.                              (6.45)
                                  k

   The sequence (go[k]} can be obtained from the two-scale relation



                                枷［k]e ""'首，巴·                                    (6.46)


Since the left-hand side of the expression is a 4兀 -periodic funct和n, we need a 4jr-
periodic extension of the right-hand side. In other words, G0( ) is nothing but a
4it -periodic extension of 中sH(w) (see Figure 6.4):


              G0回 그．y的'It］炚Mm泮）= y．知佃＋4'rt).                                     (6.47)
                           ==              \    乙 /     二＝
                       乙
From (6.47) we can get the expression for the coefficients {go[k]}:
                                                         ORTHONOR人IAL SCALING FUNCTI(：가니S                                119


                  8SH(W+ 4兀)                             QSH(W)                              8SH(W- 4功
                                                   1               I       I                                 T
                                                                                                1        I       I




                                                                                                         1111兀
                                                   I               I       I                    I
                                                   I                       I                    1
                                                                                                1
                      I                          I         1               I                    1        1
                     H幻T                       -ir         0                   兀                     4
                      FIGURE 6.4              4ir-periodic extension of中SH(w).




                   ］乙L,/,"" 구SH小며wk'\ dw
                 豹『，
                    극，，勺，:",'"'"多SH
                                  (0)exp(）咎）dw
                    寸，/：如놔쒸』a)
                       ：
                           中SH
                                  （二）
                                          ·

                                                                                                                     他48)

 By using (6.43), we get


                                 I1                                             fork= 0

                   go[k］          ( 1) (k 1)/2                                           dd k
                                 L
                           니
                                                               .   ..          f아.
                                  0
                                 tU
                                                         Kit                   .
                                                                               的r
                                                                               1Or eVe1l
                                                                                   even k ；亡 0.
Figure 6.5 shows the Shannon scaling function and the wavele
                                                                                                    t.

6.4.2   Meyer Scaling Function
The Shannon scaling function 中sH(t) has poor
                                                   time localization (A中sH = 以그). The
reason for this is that in the frequency domain, 砂sn(w
                                                           ) has a discontinuity at -it
and 兀. Consequently, in the time domain, as given by
                                                         (6.43), the function decays as
l/ t and hence its RMS time window width (4.3) i 5
                                                       OO. To improve it, Meyer [3, 4]
obtained the scaling function 砂M,m (w) by applyin a
                                                      g smoothing function near the
discontinuities of 中sti (w) in such a way that the orthogo
                                                           nality condition

                                        I8M,   m
                                                   (W+
                                                                        2兀k)         =   1                           (6.49)
                                  k
is satisfied. In (6.49) the index m indicates the degree
                                                         of smoothness [i.e., the mth-
order corner smoothing function Sm (a)) is rn times
                                                         continuously differentiable].
120         CONSTRUCTIC가나 OF ＼八／AVELETS



                                                                                    1

       0.5
                                     砂S月（t)                                                                   kbSH(w)I



       0.5                                                                          0
        -10                           5                         10                   0                   7r


            1                                                                       1
       0.5                           少SH(t)                                              1少SH(W) I

            0   나




      -0.5

       -1
                                                                                    0
            -10     45           0    5                         10                   0                   jr       2兀
FIGURE 6.5 Shannon scaling function, the corresponding wavelet, at
spectra.




To satisfy the orthogonality requirement (6.38), these corner sm(
should have the f이lowing pr아卿ties:

                                                                                          0

                                                                                              y0 l
                         Sm (y) +Sm(1 1y) = 1,                                                       1
                                                                                        /
                                                                                        V
                         Sm (y) = 0,
                                                                                          y
                         Sm (y) = 1,

Examples of corner smoothing functions are

                                                                              10,           y< o
                                                           so(y) =p,          11,
                                                                                            o드y. 51
                                                                                            y> 1


                                     0/  Hl
                                                                                         y< 0

                                      2
                                      八 1
                                        2
                                          1



                                                    1r !




                                      乙
                         S                V
                                                                                         0 드 y < 0.5
                                                           n
                                                           J乙
                             V
                                          /
                                              尸11
                                                    V/                   VJ   1,         0.5 드 y 51
                                                                     d
                             /
                                                                     1
                                              1                                          y> 1.

  Let Sm (y) be a desirable corner smoothing function. Then
                                                                                                 ORTHONORMAL SCALING FUNCTIONS                                                121


                                                                   m8[ m（知미｝
                                                                                                                                                 回 竺3 프3
                                                                                                                                         쯔
                                                                                                                                                                     竺
                                                  <
                                              H
                                                      卜



                                                                                                                                     3
                                                                                                                                                                 3
            中M,m(W) -                                 4            0,
                                                                                                                               k끼 之

                                                                   1,                                                               wI 5

  The scaling function in the time domain then becomes


     砂M,m(t) =2.j "'만2兀t/3) ＋三 / ' co寸뇨, 佶）]..,I근프（I＋亨）,]d亭 (6.50)
                                  乙Jrt/i                                             . J0          L乙               -'     L '                               J
 For a linear smoothing function m = 0, the integral above
                                                           can easily be evaluated.
 The result is

                        r
                        0                                 2 sin(2irt/3) . 4 4t sin(2irt/3) + cos(47rt/3)                                                                  .
                        M                                                                                                                                                     ..
                  m
                                                          m 八 ＼口
                                                                                                                                                     =
                                                                                                                                                         )
                                                                             2兀t/3           十兀                     야16尸
              1
                                                                                                                                                             '           IO"그 ' J
                                                                                                                                                     /
 For higher values of m, the integral in (6.50) needs to
                                                         be evaluated numerically. In
 Figure 6.6 we show the scaling function and wavelet of Meyer
                                                                for m = 0 and 1.
    As done before, the two-scale coefficients {go[k]J
                                                          can be obtained by a 4jr-
 periodic extension of M,m (W). An example of such an extensi
                                                                     on is shown in
 Figure 6그



                                          =8.[,]r""' 寸出，;
                                        1l


                                        1O乙




                                                                                                 =＞二a4,/m(m+ 4兀k).
Similar to the case of the Shannon scaling function,
                                                                                                                here too we get

                                                                                                        (k\
                                                                                 g0[kJ = 砂4／沁 1 ; } .                                                                    (6.52)
                                                                                              \ 乙/

 Therefore, form = 0, we can obtain go[k} simply by substitu
                                                               ting k/2 for tin (6.51).
Table 6.2 gives the two-scale coefficients form = 1.
   Meyer's wavelets can be obtained by using the two-scale relation
                                                                     s. Since the scal-
ing functions have compact support in the frequency domain
                                                                 , Meyer wavelets are
related to the scaling function in a more direct way; that
                                                           is,


                      1IIM,
                              m
                                  (W)
                                                            =           GI
                                                                               (Z)
                                                                              ／씨 /
                                                                                       M,
                                                                                             m   (을)  ／口八
                                                                                                            z   =
                                                                                                                         exp   (_
                                                                                                                                             j
                                                                                                                                                 )
                                                                                             ＼스
                                                           =            卜
                                                                             乙（Jot-                 （三／
                                                                                            乙J474/ ,m
122   CONSTRU口ION OF＼사AVELE巧




                                伽i;0(t)



                   0        2        4



                                *M;O(t)




                                                          2手
                                                                  誓                    誓
                                                                                1少M: 1(0끼




                                                           2兀     4ir           6兀      8兀
                                                            3      3             3       3
       -2
FIGURE 6.6    Meyer scaling function, the corresponding wavelet, and         eir magnitude spec-
tra.




            1a 11入，/
            中M,m (0) +4r)                 中M,m (W)             伽i,Mm1 4兀）




                                                                        小＼
                -4兀                1誓        0       誓              4n.

                    FIGURE 6.7 4兀-periodic extension ofaM,m (0)).
                                                                 ORTHON아小IAL SCA니NG FUNC기（JNS                                           123

TABLE 6.2 小Vo-Scale Sequence for First-Order Meyer Scaling Function中M:
                                                                       1
        goEni = g0[-nJ                n                        g0[n] =go[-n]                                   n            go[nl =g0[-nJ
 0   1.0635133307325022 13                           0.0018225696961070                                    26            0.0000781583234904
 1  0.6237929148320031 14                           -0.0001225788843060                                    27           -0.0002817686403039
 2 -0.0594319217681172 15                           -0.0019003177368828                                    28           -0.0000686017777485
 3 -0.1762971983704155 16                           -0.0000361315305005                                    29            0.0003520515347881
 4  0.0484777578300750 17                            0.0018514320187282                                    30           -0.0000591760677635
 5  0.0751184531725782 18                           -0.0乂4792529715153                                     31           -0.0002870818672708
 6 -0.0339527984193033 19                           -0.0013039128005108                                    32            0.0001435155716864
 7 -0.0311015336438103 20                            0.0刃7208498373768                                     33            0.0001507339706291
 8  0.0197659340813598 21                            0.0006265171401084                                    34           -0.0001171599560112
 9  0.0110906323385240 22                           -0.0005163028169833                                    35           -0.0000530482980227
10 -0.0089132072379117 23                           -0.0002172396357380                                    36            0.0000282695514764
11 -0.003539083 1203475 24                           0.0001468883466883                                    37            0.0000443263271494
12  0.0025690718118815 25                            0.0001627491841323                                    38            0.0000355188445237




                    =    -z
                              F多
                              1
                              LX=
                                  .

                                  U 00
                                =U的
                                      11寸
                                                     M,
                                                               m   佃 + 2: + 4:k) 1                   1     J
                                                                                                                   M,
                                                                                                                        m   ( )
                                                                                                                            \ 乙/



                   日函加+ 2小瓦佃如] M,m (卦                                                                                                 (6.53)


6.4.3   Battle-Lemarie Scaling Function

Battle-Lemari6 [5,61 scaling functions are constructed by orthonormalizing the mth-
order cardinal B-spline Nm (t) for m 之 2. As pointed out before, the set of basis
functions {Nm(t - k) : k E Z} is not orthogonal for m 之 2. The corresponding
orthonormal scaling function N, (t) can be obtained as
                                                                        八
                                                                        .7   I.   .\

                              秘
                                            （CL力＝
                                                                        1Ym WJ
                                                               ［雹N, , (e卞jW)}1/2
                                                                                       .   . .   .                                    (6.54)

The Battl아Lemari6 scaling func如n 中13L,m (t) 奴 血en,

                                            中BL,m(t) = Z1古（r),

and the coefficients {g0[k]} can be found from

                     l ＜小． , , , k        - (m/2)    Vm
                    ;; ) .Rnl，凡1，乙人 = Gne寸八w／이 = 즈꼰＝근r.
                                                          ,,
                                                                    i
                                                                                                     (W)
                                                                                                                                      (6.55)
                    2乙JUV
                    -   k
                               - -                入／
                                                  "三nU/.2)   "
                                                  " 77i \14/                                                   / 1U/

where z = e卜j(m/2). By combining (6.54) and (6.55), we have



             G恤）=（牛）'［器出 ，二］""
                       ，岩’                                                                                                           (6.56)
124                      CONSTRUCTION OF WAVELETS


As an example, consider the linear Battle-Lemari6 scaling function for which m =
2. For this case we have



                                           人
                                                       ．
                                   ；각耐小小（' 二" /xz4z2++：二기                                                                                               (6.57)


The coefficients {go[k]} can be found by expanding the expression（中
                                                                ，n the.right-hand
siae 雙 ai兀iyn엣uai in 乙 ana men comparing me coemcie쯔S 빠ne liKe 叫ers
or z. inese coemcients can aiso De lOUflO Dy compuung.me r'our牡 coemcienus.or
the right-hand side expression. Observe that (10(1) = I is satlsfleJ, thus giving me


sum of
TABLE 6.3
                   all     {go[      k]   } to   be   2.   In    Tables      6.   3 and 6.4 we   provide
                                  Two-Scale Sequence for Linear Battle-Lemarie Scaling Function砂BL그
                                                                                                                               the c     f   ffi
                                                                                                                                               cients   of the


n                 go[nl= go[2- nj                               n           go[n] = go[2 - n]                                      goln] = go[2 - n]



                                                                                                                                 0 0 0 0m
                                                                                                                      m
                                                                                                                      / 8




   d
   l 八
     二 각
       V 4
         1 <
           V 6
                                                                                                               n    乙 八
                                                                                                               二 八（ n 4
                                                                                                                      U
                  1.1563266304457929                            14         0.0000424422257478              小
                                                                                                                                  0000刃0053986543
                                                                                                                                     1




                  0.5618629285876487                            15        -0.0000195427343909                                        1
                                                                                                                                          28565276
                                                                                                                      O
                                                                                                                      / 0
                 -0.0977235484799832                            16        -0.0000105279065482                                        1
                                                                                                                                          13958989
                 -0.0734618133554703                            17         0.0000049211790530                  ]
                                                                                                               1
                                                                                                                                      000007374693
                  0.0240006843916324                            18         0.0000026383701627
                                                                                                               n
                                                                                                               J
                                                                                                                                           3617852



                                                                                                               n
                                                                                                               二 n
                                                                                                                 4
                                                                                                                 V 4
                                                                                                                   1 <
                                                                                                                     J 6 m
                                                                                                                         / 8
                  0.0141288346913845                            19        寸中0.0000012477015924                                 -0.0000000001908819
   m
   / 8
                 -0.0054917615831284                            20        -0.0000006664097922                                   0.0000000000939609
                 -0.0031140290154640                            21         0.0000003180755856                                   0.0000000000495170
   9
                  0.0013058436261069                            22         0.0000001693729269                                  -0.0000000000244478


                                                                                                               n
                                                                                                               4
                                                                                                               V n
                                                                                                                 4
                                                                                                                 V n
                                                                                                                   J n
                                                                                                                     J n
                                                                                                                       J n
                                                                                                                         J 그
                                                                                                                           J
0 l 八
    乙 n4나


l ll  ]
                  0.0007235625130098                            23        -0.0000刃0814519590                                   -0.0000000000128703
                 -0.0003172028555467                            24        -0.0000000432645262                                   0.0叩0000[X刃0637(刃
                 -0.0001735046359701                            25         0.0000000209364375                  O
                                                                                                               /
                                                                                                                                0.0000000000033504
                  0.0000782856648652                            26         0.0000000110975272                                  -0.에00000000016637
                                                                                                               4
                                                                                                               J




TABLE 6.4                         Two-Scale Sequence for Cubic Baule- 加arie Scaling Function BL;4

n                  go[n] =go[4- n]                              n           g0[n] = g0[4 - n]                  n                   goln] =go[4- n]
 2                1.0834715125686560                            15         0.0026617387556783                  28              -0.0000282171646500
 3                0.6136592734426418                            16        -0.0015609238233188                  29              -0.0000222283943141
 4               -0.0709959598848591                            17        -0.0013112570210398                  30               0.0000146073867894
 5               -0.1556158437675466                            18         0.0007918699951128                  31               0.0000114467590896
 6                0.0453692402954247                            19         0.0006535296221413                  32              -0.0000075774407788
 7                0.0594936331541212                            20        -0.0004035935254263                  33              -0.0000059109049365
 8               -0.0242909783203567                            21        -0.0003285886943928                  34               0.0000039378865616
 9               -0.0254308422142201                            22         0.0002065343929212                  35               0.0000030595965005
10                0.0122828617178522                            23         0.0001663505502899                  36              -0.0000020497919302
11                0.0115986402962103                            24        -0.0001060637892378                  37              -0.0000015870262674
12               -0.0061572588095633                            25        -0.0000846821755363                  38               0.0000010685382577
13               -0.0054905784655009                            26         0.0000546341264354                  39               0.0000008247217560
14                0.0030924782908629                            27         0.0000433039957782                  40              -0.0000005577533684
                                                                    ORTHONORMAL SCALING FUN口IONS    125




           2
           1                                        砂BL:2(t)                           I岵L;2（口川
           0
      -1
                -4     -2                                       6                 10      20



                                                                                       岫BL;4佃）1



               -4 -2        0       2       4       6       8


                                                    砂BL;4(t)                           1少BL;4(U川
                                                                         1

           0
  -
           1                                                             0
            -6 -4 -2            0       2       4       6                        10       20       30
FIGURE 6.8 Battle-Lemari6 scaling function, the corresponding wavelet, and their magni-
tude spectra.



linear and cubic Battle-Lemari6 scaling functions. The linear Battle-Lemarie scaling
function and the wavelet are shown in Figure 6.8.


6.4.4           Daubechies Scaling Function
Battle-Lemari obtained orthonormal scaling functions by orthonormalizing mth-
order cardinal B-splines Nm (t) for m 三 2. However, because of the presence of
ENm (z) in the denominator for the orthonormalization process, the sequence {go[k]}
becomes infinitely long.
   To obtain orthonormality but preserve the finite degree of the (Laurent) poiy-
nomial, Daubechies [7,81 considered the two-scale symbol for the scaling function
中i). 7刃:
126     CONSTRUCTION OF WAVELETS



                                                                                                                                   (6.58)
                                  q回＝                 （牛）                           '    S（小

where S(z) E 7trn_1. So our objective is to find S(z). First,                                                         serve that since
Go(1) = 1, we must have S(1) = 1. Furthermore, we also wai                                                            5（小1) 尹 0, be-
cause if S(- 1) = 0, then z + 1 is a factor of S(z) and hence can                                                      taken out. Now
Go(z) given by (6.58) must satisfy the orthogonality condition, n                                                     ely
                                                                                                      ' "2
                        IGo(z)12 + IG。
                                     (- z)I2 = 1,                                              z = eHj                             (6.59)
                                                                                                         I2 =                      他60)
                                                                                               (_
                                                                                                    z)
                                                                                                                1.
                                                                                         IS
                        수cos畔1叉釧                      ' +8i0 "


By defining

                                                  工 := sin2 으
                                                            4
and
                                           /（功 := Is（之） 2,

(6.60) can be rewritten as (Exercise 11)

                              (1 - 工）tm f （工） + 工mf (1 - 工） == 1




                                           :
                        => /（工） = (1- 工）_m[1_ 工mf (1 卞工）]

                                                            +k                           1k
                                                                                               『凡（1) ,                             (6.61)
                                   =             (m                           -



                                                                                    1)
where the rem小nder Rrn (x) is


  島帥亡（싸기如－功山．砬（싸
              !c=rn '                  /                                                           k=0 \
                                                                                                                       ')   1 '·   (6.62)


Since f (x) is a polynomial of order m, Rrn (x) = 0. Therefore, w have


                                                                                              m
                                                                                              卄r
                              rn- i /      . ,              1\

                IS   (z)I2=   Z (m十1C_
                              !c=0 '
                                                            l)
                                                                 /
                                                                     5ifl2k
                                                                                                         乙 = e 7
                                                                                                                     /2.           (6.63)


The polynomial above can be converted to


                                                      竺2                      mZ山
                                                                                                   kco
                               Is（乙） 2                                                                                             (6.64)
                                                                                    aj cos可 '
                                                             ORTHONORMAL SCALING FUNCTIONS                                        127

where [9, p. 801

                        rn- k- I
                                           ：小，
                                                 1
                                                                  ( : （ =)
                                                                       "'
                                                                      i_. . ,
                                                                                          "
                                                                                              '\        ,   .
                                                                                                        『” 十二：
                                                                                                                           1\
                                                                                                                           '
                 =（小1)k ＞二 2가*                                                                                                  (6.65)
                                                                                              ))
           aj,
                         n=O


Our next task is to retrieve S(z) from IS(z)I2.
  According to Riesz's lemma [10, p. 172], corresponding to a cosine series

                                                                            N
                                                                            Z山+                         t
                                                         竺
                                                                                     n             O        m
                              f (w) =                    2
                                                                                                                                (6.66)


with 口ij. ... .aN e R and a, 尹 0, there exists a poynomial

                                                                       N
                                           g(z) = ＞二bk乙k                                                                        (6.67)
                                                                      k=O

with 口o. ....ajvER, suchthat

                           Ig（해2=／佃）,                                                乙＝eHjm.                                    (6.68)

By applying Riesz's lemma to (6.64) it is easy to verify [9] that S(z) has the following
form:
                    K                  L

         S(z) =Cfl  (z- rk) fl (z- zt)(z-ii),                                                               K+ 2L= m- 1, (6.69)
                k=i         Z=l

where {rk} are the non啣아eal roots and ｛끄｝ are the con叩lex roots of少山SQ기2
inside a unit circle and C is a constant such that S(1) = 1.
   Once we have S(z), we can substitute this into (6.58) and compare the coefficients
of powers of z to get the sequence {go[k]}. We will show the steps to get these
sequences with an example.
   Consider m = 2. For this, we have a0 = 4 and ai = -1, which gives


                                  Is（玔'              =       2    -         cos을



                                                     =       2귿                 （:   +z                ')



            ＝수기S(z)j2＝뉴나缸豹＝mk- ri汗hn ,
                              二                                                               乙                   \    ru /
                                                                                                                                (6.70)
where ri = 2 - .厄. From (6.69), we have

                   S（之）＝그니z                          rl) =                   . l 二（z                            2+ '／三）.        (6.71)
                         1-       ri                                        -i+               ji
       128        CONSTRUC기C가니 OF 叭/AVE LETS

       So, form = 2, we get

                   G。 (z)
                                        =
                                                二
                                                .    (g。
                                                               [O] + g。 z + g。[2]z2 + g。[3]z3)
                                                                             [l]
                                        =（字）'弓［(1『V亂*(1- V히
                                                21   (     '   -4
                                                                             + '   -4
                                                                                        z
                                                                                         『 '                    4
                                                                                                                      z
                                                                                                                          '『 '   4
                                                                                                                                     z ")           .        (6.72)

 Since S(z) is a
 2m.
                            polynomi신
                                                                    of
                                                                         order m, the   length
                                                                                                           of
                                                                                                                    two-scale seq叫ence        for
                                                                                                                                                        加;
                                                                                                                                                              m   is
   Form = 2 and 7, the scaling functions and wavelets, along with their magnitude
 spectra, are shown in Figure 6.9. Two-scale sequences for some Daubechies scaling




                                                                    中D;7(t)                           。’                         岫D,7(n川



                                                                                                       0                   10        20                      30


                                                                                                                                 甲1;7   （口川
                                                                                                      。
                                            0                            5                                                 10
                                                                                                 0-
             -5
                                                                                                                                     20                      30
FIGURE 6.9 Daubechies scaling function, the corresponding wavelet, and their magnitude
spectra.
                                  CONSTRUCTION OF BIORTHOGONAL WAVELETS          129

TABLE 6.5 1\vo-Scale Sequence for the Daubechies Scaling Function

         go[n] = go[-nj      '2        go[n] = g0[-nJ     n         go[n] = go[-n]
              m= 2                         m= 5                       m= 7
0      0.6830127018922193     0      0.2264189825835584    0    0.11以994307456160
1      1.1830127018922192     1      0.8539435427050283    1    0.5607912836254882
2      0.3169872981077807     2      1.0243269442591967    2    1.0311484916361415
3     -0.1830127018922192     3      0.1957669613478087    3    0.6643724822110735
              m= 3            4     -0.3426567153829353    4   -0.2035 138224626306
0      0.4704672077841636     5     -0.0456011318835469    5   中0.끄68350112806179
1      1.1411169158314436     6      0.1097026586421339    6    0.1008464650093839
2      0.6503650005262323     7     -0.0088268001083583    6    0.1008464650093839
3     -0.1909344155683274     8     -0.0177918701019542    7    0.1140034451597351
4     -0.1208322083103963     9      0.0047174279390679    8   -0.0537824525896852
5      0.0498174997368837                  m= 6            9   -0.0234399415642046
              m= 4            0      0.1577424320027466   10    0.0177497923793598
0      0.3258034280512982     1      0.6995038140774233   10    0.0177497923793598
1       1.0109457150918286    2      1.0622637598801890   11    0.0006075149954022
2      0.8922001382609015     3      0.4458313229311702   12   -0.0025479047181871
3     -0.0395750262356447     4     -0.3199865989409983   13    0.0005002268531225
4     -0.2645071673690398     5     -0.1835180641065938
5      0.0436163004741772     6      0.1378880929785304
6      0.0465036010709818     7      0.0389232097078970
7     寸0.아49869893303614      8     -0.0446637483054601
                              9      0.0007832511506546
                             10      0.0067560623615907
                             11     -0.0015235338263795



functions are given in Table 6.5. Readers should keep in mind that in some books
(e.g. [8]), there is a factor of\／三 in the two-scale sequences.


6.5    CONSTRUCTION OF 引0R1HOGONA1 WAVELETS

In previous sections we discussed semiorthogonal and orthonormal wavelets. We
developed orthogonal wavelets as a special case of semiorthogonal wavelets by using



                                                                               (6.73)

One of the major difficulties with compactly supported orthonormal wavelets is that
they lack spatial symmetry. This means that the processing filters are nonsymmetric
and do not possess a linear phase property. Lacking this property results in severe
undesirable phase distortions in signal processing. This topic is dealt with in more
detail in Chapter 7. Semiorthogonal wavelets, on the other hand, are symmetric but
suffer from the drawback that their duals do not have compact support. 가1is is also
     130      CONSTRUCTION OF WAVELETS

     undesirable since truncation of the filter coefficients is necessary for real-time pro-
     cessing. Biorthogonal wavelets may have both symme啣 and compact support.
        Cohen et al. [11] extended the framework of the theory of orthonormal wavelets
     to the case of biorthogonal wavelets by modification of the approximation space
     structure. Let us recall that in both the semiorthogonal and orthonomal cases, there
     exists only one sequence of nested approximation subspaces,

              {O} +-   · · · C A_ C A_ i C A0 C Al C A2 C · · · -+ L2.                            (6.74)
     The wavelet subspace, W5, is the orthogonal complement to A5 within A5+i such
     that

                                      A5 fl W, = {O},              S E Z,

and
                                      AS + WS = A5+1.                                            (6.75)

     This framework implies that the approximation space is ortho叩nal to the wavelet
     space at any given scale s, and the wavelet spaces are orthogona' across scales:

                                       wsJ-wp            匈rs尹p.                                  (6.76)
 In the orthonomal case, the scaling functions and wavelets are orthogonal to their
 translates at any given scale s:

                                       仲k.s(t), 中k,m(t) == Sk,m)

                                      (frk.s(t), 砂k,m(t) = Sk,m).                                (6.77)
In the semiorthogonal case, (6.77) no longer holds for 中 and 中. Instead, they are
orthogonal to their respective duals,

                                      （中k,s(t), 中m ,小）) = 8k,m
                                      (奴,s(t), frm,s(t)) = 8k,m,                                 (6.78)
and the duals span dual spaces in the sense that 了, := sparf4k,5(t)(2t                           - 刃i),
           E z} and W5 :=       (2       ,       E Z}                in Chapter
semiorthogonality implies that A5 = A5 and W3 = W5.
                                                                       .
s,
                                                -
      m,
                             spanf可
                                           't
                                                    m)
                                                         s,
                                                              m,
                                                                           As
                                                                                desribed
                                                                                                     5,
  In biorthogon出 systems, there exists an additional dual nested space:

            ｛아 <- . . .C 及2C 及1C 瓦 C 瓦 C 工2C · · · -                                       L2.   (6.79)
In associati.on with山is nested sequence of spaces is a set.of du띠 wavelet subspaces
(nor nesteaJ w5, S e 丑1, mar compiemenrs me nestea sunspaces As, S E 乙. 10 oe
more specific, the relations of these subspaces are

                                         A5 + W$ = A5+i                                          (6.80)
                                         A5 + W5 = A5+i.                                         (6.81)
                               CONSTRUCTION OF BIORTHOGONAL WAVELETS                131

The orthogonality conditions then become

                                       盛上W5                                       (6.82)
                                       盛上WS,                                      (6.83)

giving us

                               （似,,(r), 派,,（이 = 0                                 (6.84)
                                侮，5(t), lllm.s(川＝0.                               (6.85)

In addition, the biorthogonality between the scaling functions and the wavelets in
(6.78) still holds. The two-scale relations for these bases are

                             中（t) =＞二go[k］中（2t - k)                               他86)
                                    k

                             8(r) =＞二 ho[k]8(2t - k)                              (6.87)
                                       k

                             少（t) =＞二gi[k］中（2t - k)                               他88)
                                       k

                             7(r) =＞二 h1[k]3(2t -k).                              (6.89)
                                       k

   The orthogonality and biorthogonality between these bases give the following
four conditions on the filtering sequences:

                          (go[k - 2m], h1[k - 2n]) = 0                            (6.90)

                          (gi[k - 2m], ho[k 尸 2n]) = 0                            (6.91)

                                (go[k - 2m1, ho[k]) = 8m,0                        (6.92)

                                佃[k - 2m], hi[kj) = 8m,0.                         (6.93)

Bio曲ogonal wavelet design consists of finding the filter sequences that satisfy (6.90)
through (6.93). Because there is quite a bit of freedom in designing the biorthogonal
wavelets, there are no set steps in the design procedure. For example, one may begin
with go[k] being the two-scale sequence of a B-spline and proceed to determine the
rest of the sequences. Another way is to design biorthogonal filter banks and then
iterate the sequences to obtain the scaling functions and the wavelet (discussed in
Section 6.6). Unlike the orthonormal wavelet, where the analysis filter is a simple
time-reversed version of the synthesis filter, one must iterate both the synthesis filter
and the analysis filter to get both wavelets and both scaling functions. We will follow
this approach and defer our discussion of biorthogonal wavelet design by way of an
example in Chapter 7.
 132     CONSTRUCTION OF WAVELETS


 6.6    GRAPHICAI DISPlAY OF WAVELETS

Many wavelets are mathematical functions that may not be described analytically.
As examples, the Daubechies compactly supported wavelets are given in terms of
two-scale sequences, and the spline wavelets are described in terms of infinite poly-
nomials. It is difficult for the user to visualize the scaling function and the wavelet
based on parameters and indirect expressions. We describe three methods here to
display the graph of the scaling function and the wavelet.


6.6.1 Iteration Method
This method is the simplest to implement. We include a Matlab program with this
book for practice. Let us write

              中m+i (t) =＞二 go[k]中m(2t -k) ,           m =0, 1, 2, 3 .. .         (6.94)

and compute all values oft. In practice, we may initialize the program by taking

                                     加(t) = 8(t)                                (6.95)

and setting 加(n) = 8(n) = 1. After upsampling by 2, the sequence is convolved
with the g0[k] sequence to give 勿(n). This sequence is upsampled and convolved
with g0[k] again to give 仇(n), and so on. In most cases the procedure usually con-
verges within 10 iterations. For biorthogonal wavelets, the convergence time may be
longer. Once the scaling function has been obtained, the associated wavelet can be
computed and displayed using the two-scale relation for the wavelet:

                             少（1) =＞二gi [k］中（2t -k).
A display indicating the iterative procedure is given in Figure 6. lC. The figure mndi-
cates the number of points in each iteration. To get the conespondi土lg position along
the time axis, the abscissa needs to be divided by 2m for each iteration m.


6.6.2   Spectral Method
In this method, the two-scale relation for the scaling function is expressed in the
spec仕al domain

                   (m) ==G.(."'
                  3(w)   Go(e3( "2)
                                "))3I을\
                                 !
                                    )4 ( .),          z =6""/'),                他96)

                        =G.(."" /'))G.(r'" /"))8(응)
                                                            GRA타키CAL ［기SPLAY OF WAVELETS                                   133




               2                    3               4                            2           4           6      8           10


                                                                  0


         5         10          15         20        25                           10          20          30     40          50




        20         40          60         80       100                               50           100         150          200




         100                            3凹                                           200          400         600          800


 0                                                                0   :1U三                                           '0
-2        "                                                       -2
  0      500            1000            1500       2000             0                1000         2000        3000         4000
FIGURE 6.10 Iterative procedure to get scaling functions. Abscissas need to be divided by
2m to get the correct position in time.




                                                   N

                                               =fl Go(e"" /")미制
                                                   k=1                           -


                                               =    [J Go
                                                   N-＋以）
                                                            (eu   (m12")
                                                                            )a   (O)   .
                                                                                                                          (6.97)
                                                   k= 1

Since 砂(O) = 1, we may take the inverse Fourier transform of (6.97) to yield

                                         1     !'的 ／싸：주U              :. ,. ,, k . \        乙．.
                        叭t) =石 Jd fl G0(e" "" ")7 es'"' dw.                                                           (6.98)
 134      CONSTRUCTION OF WAVELETS

 To compute (6.98), the user has to evaluate the truncated infin
 take the fast Fourier transform.


 6.6.3   Eigenvalue Method
 This method converts the two-scale relation into an eigen equation. Let us consider
 the two-scale relation by setting x = n to yield the following matrix equation:

                             中（n) = ＞二go[k］中（2n - k)
                                              k


                                       = Z go[2n -m]可m)
                                       = [go(n，刃i)］中（刃2),                                              (6.99)
where the matrix element go(n, m) = go(2n - m). In matrix fqrm, we write (6.99)
as


                   go[O]   go[-l]        go[-21                          砂（0)          砂（0)
                   go[2]   go[l]         go[O]                           中（1)    =
                                                                                     1 中（1)
                   go[4]   go[31         go[2]                           中（2)          中（2)


The eigenvalue 。f this eigemnatrix     s。we can c。
                                         is
                                                  1,
                                                    mpute O) f。    r all integers n.
가lis procedure can be repeated for a twofold increase in resolution. Let x = n/2,
and the two-scale relation becomes

                             可씌 = )八．耐M小k).
                                \ 乙/          中
                                                                                                     (6.100)
                                               尺


By repeating this procedure for x = n/4, n/8. ... .we compute the discretized 中(t)
to an arbitrarily fine resolution.


6.7    EXERCISES

 1. Show that the support of semiorthogonal wavelet, *m (t) = (0, 2m - 1].
 2. Show that the integer translates of the Shannon wavelet 吻(t - k) form an or-
    thonormal basis.
3. Find the cubic polynomial S4 that satisfies the conditions .'4(0) = S (0) = 0,
   S4(l) = 1, S (1) = 0, and S4(x) + S4(1 - x) 三 1. Use this polynomial as
   the smoothing function for Meyer's scaling function and compute the two-scale
   coefficients.

4· 우h애，岫t if如쓰t.),k E Z}.,iS a Ri,esz.basis of和 이叩나L 뜨弘then
      " " ""   is a iciesz oasis or v5 =               Ick,
                                                              sw,
                                                                    IC    U     ror a nxeu S   U. m "at is
                                                                                          EXERCISES   135

                                                             2          (X)


                  A   Z   IakI2드
                                             ＞二 口k中（t - k)
                                                             2
                                                                 <B    ＞二
                                                                      k=-oo
                                                                                          IakI2
   implies that

                                                             2         的

                  A   Z1           akI25      ＞二 口k中k.s(t)
                                                             2
                                                                 드B   ＞二
                                                                      k=-oo
                                                                                    1口k           2


   with the same constants A and B.

5. Show that the following statements 町e equivalent: (a) 佃(. - k) : k E Z} is an
   or血onormal fam幻, and (b)＞二恐a知＋2k兀十미 almost everywhere.
6. Prove that {N1(. 尸 k) : k e Z} is an orthonormal family by using this theorem,
   that is, by showing that


                                         乶 1刃；(w+ 2k玔" =1.
                                     k= -（刃


7. Obtain an algebraic polynomial corresponding to Euler-Frobemus-Laurent
   polynomial EN4(Z) and find its roots, 入i > · · · > A6. Check that these zeros are
   simple, real, negative, and come in reciprocal p缸rs, i.e.,

                                         入l入6 == 入2入5 = 入3入4 = 1.


8. The autocorrelation function F for a given function f E L2(- 的, 以）) is defined
   as


                      「仁）            =    /:/(! f而dt,
                                                    +x)           :（尺


   Compute the autocorrelation function of the hat function N2 and compare it to
   the function N4 introduced in Exercise 7.

9. Construct a linear Battle-Lemari6 scaling function to show that for the hat func-
   tion N2(t), it holds (let z = ei (c0/2) ) that


                          亡 區（w+2kjr)12 和'『4+
                      k＝니)0
                                                                           z   ')
   and


                                          N2(w) =
                                                     芬
 136        CONSTRUCTION OF WAVELETS

       The Fourier 仕ansform of the orthonormalized scaling function N- (t) is given
       by

                                            (w)
                                                     -
                                                         [,
                                                               ;   (_
                                                                            1/w2) (1        z2)   2
                                                                                       -,
                                                              (l/6)(z 2 + 4 + z2)                           2·
                                      耐
                                                                                                      ]l/
                                                         [
       We have shown that the symb이



                                                       Go(z)＝辯去
       Compute the ratio to show that the result is


                                                     (느．
                                                     \
                                                        듸/ ' (1+ n)l/2,
                                                         乙


     where

                                                  [（之-1 + 之）/4] - [（乙-2 + 乙2)/4]
                                     11=                 1 + (z12 + z2)/4]       "
    Use the power series expansions


                (1 +   77)
                             l/2          1+
                                                              嗟             m          끄抑             3          m   小
                                                                                                                     H1




    and

                                   .(.l.. +. -.. H."          픈，. . .
                                           工J. " = ) (- l) Ji (/nHl+     j\ i
                                                                    . ' ' IxJ
                                                  卜넋
                                                   j=O        \   j       /

    as well as the binomial theorem to expand the expression [(1+z)/2]2(1+ii)"2 in
    powers of z and determine the coefficients Rfkl fork = -5. . .1. . 5 by comDarin으
    f1m口 r1r\1.r口n11八11r1;14n r11\i工14;1m; 41m1t, n下 月_c
    me   corresponaing coemcients or z U1 . . . , zV     m c. 11 -4 rm\ r1144 r/ 1 I . m\ /n] 2/ 1 1 am\ '1 /2
                                                            in Uo(z) and [(1十z)/2J口(1+刃) ' '已
    You should use symbolic packages such as Mathe刃atica or Maple for these
    computations.
10. Construction of linear B-spline wavelet: Given the two-scale relation for the hat
    function
                                                              2         1   J／八＼




                                          N2(t) =＞二掘)N2（小k),
                                                         戊＝I)               \


    we want to determine the two-scale relation for a linear wavelet with minimal
    support,

                                          吻（t) =＞二gi[k1N2(2t -                                ,
                                                                                     EXERCISES    137

     using the corresponding Euler-Frobenius-Laurent polynomial E(z) = z 1 +
     4+ z. It was shown that for the corresponding symbols


       Go (z) = !.y.g0[t]/and                   (h回＝!y冊｝:k,                           乙 = eUj
                                                                                             （口）/2),
                 乙 m =                                         乙 H
                    K                                                K



     the orthogonality condition is equivalent to

                     Go(z)Gi(z)E(z) + G0(- z)Gi(- z)E(- z) = 0

    with Iz I = 1. We need to determine the polynomial Gi(z) from the equation
    above. There is no u血lue solution to this equation.
     (a) Show that Gi(z) = (- l/ 3!)六o(- z)E(- z) is a solution of the equation
         above.
    (b) Show that Go(之) = [(1 + z)/2]2.
     (c) Expand Gj(z) = (- l/ 3!)z3Go(- z)E(- z) in powers of z and thus deter-
         mine the two-scale relation for the function 砂N2 by comparing coefficients
         in


                                 1
                                 l H八
                                    乙
                         G                      m
                                                        t
                             Z                      1
                                                    k
                                                            = 크加小批(-z).
                                            Z
                                                        7
                                                        q                                              =
                                                                J!
                                        k
    (d) Graph *2.

11. Complete the missing steps in the derivation of Daubechies wavelet in Sec-
    tion 6.4.4. Note that IS(z)I2 is a polynomial in cos 을．

12. Use the sequence {-0.102859456942, 0.477859456942, 1.205718913884,
    0.544281086116, -0.102859945694, -0.022140543058} as the two scale Se-
    quence {g0[n]) in the program iterate.m and view the results. The resultant
    scaling func如n is a mei油er 可 the Coi如an wavelet syst印or c아加ts [8]. The
    main feature of this system is that in this case the scaling functions also have




                         亡C 亡
    vanishing moment properties. For mth order coiflets


                             t/）砂(t) dt= 0,                 p= O. ... .rn 寸i;


                             rP中（t) dt = 0,                 p = 1, . . . , 刃i 小 1;


                             中（t) dt = 1.


13. Construct biorthogonal wavelets beginning with the two scale sequance {gO[n]}
    for linear spline.
138      CONSTRUCTION OF WAVELETS

6.8     COMPUTER PROGRAMS

6.8.1    Daubechies Wavelet
毛
% PROGRAM wavelet.m
毛
% Generates Daubechies scaling            functions and wavelets

g0 = [0. 68301; 1. 18301; 0. 31699; -0. 18301] ;
k = [0; 1; 2; 3] ;
gl = flipud (go) . 女卜1) . 八｝C;

ngl = length (gl) ;

% Compute scaling       funtion   first

Nlter = 10 ; 왐 intera七ion 七m11le
phi_ new = 1; % initialization

for i. = 1:Nlter
   uni七 ：二 2八 ( i- i ) ;
   phi = conv (g0,phi_ new) ;
   n = length (phi) ;
   phi_ new (l: 2: 2*n) = phi;
    length (phi_new) ;
    if (i == (Nlter小1) )
       phi2 = phi;
    end
end
돔
d七 = 1 . 0 / (2 士 uni上）;
七 = [1: length (phi) ] * dt;
subplc比 (2, 1, 1) , plc比 代，phi)
title ( 'Scaling Function ')

돔 Compu亡e wavele七 using 不scale rela七ion

for i = l: ngl
  a ＝二 (i- i) 女 uni七 + 1;
  b = a + length (phi2) - 1;
  psi2s (i, a: b) = phi2 * gl (i) ;
  psi2s (1,n) = 0;
end

psi   = sum (psi2s) ;
                                                                      REFERENCES        139

d七 = 1 . 0 / (2 出 uni上） ;
七 = [0 :leng七h (phi) -1] 女 d七 -            (ngl - 2)     / 2;
subplot (2, 1, 2) , plot (t, psi)
七1上le ( ' Wavele七 ' )



6.8.2   Iteration Method
돔
留 PROGRAM itera七E크 . m
움
돔 Itera七ive procedure 七（D get scaling function
% generates Figure 6. 10
통

g0 = 10. 68301 1. 18301 0. 31699 - 0.18301] ;

Nlter = 10; % number of interation
phi_new = 1; % initialization

for i = 1:1寸I七er
  uni上 = 2八 ( i- i ) ;
  phi = conv (g0,phi_new) ;
  n = length (phi) ;
  phi_new (l: 2: 2*n) = phi;
  subplot (5, 2, i) , plot (phi) ; hold on;
  heading = sprintf ( 'Iteration     = %.4g ' ,i)
  title (heading) ;
end
윙




REFERENCES

 1 C. K. Chui and J. Z. Wang, "On compactly supported spline wavelets and a duality prin-
   ciple," Trans. Am. Math. Soc., 330, pp. 903-915, 1992.
 2. C. K. Chui and J. Z. Wang, "High-order orthonormal scaling functions and wavelets give
    poor time-frequency localization," Fourier Anal. Appl., 2, pp. 415나26, 1996.
3. Y. Meyer, "Principe d'incertitude, bases Hilbertiennes et algebres d'op6rateurs," Semin.
   Bourbaki, 662, 1985-1986.
4. Y. Meyer, Wavelets: Algorithms and Applications. Philadelphia: SIAM, 1993.
5. G. Battle, "A block spline construction of ondelettes: I. Lemare functions," Commun.
   Math. Phys., 110, pp. 601-615, 1987.
6. P. G. Lemarie, "Une nouvelle base d'ondelettes de L2(Rz)," J. Math. Pures Appl., 67,
   pp. 227-236, 1988.
7. I. Daubechies, "Orthonormal bases of compactly supported wavelets," Commun. Pure
   Appl. Math., 41. pp. 909-996, 1988.
140     CONSTRUC기O卜dOF ＼八／AVELETS


 8. I. Daubechies, Ten Lectures on Wavelets. CBMS-NSF Ser. App. Math. 61. Philadelphia:
    SIAJ吐 1992.
 9. C. K. Chui, Wavelets: A M口片妃matic口／ To可for Sign口／ An口／ys加． Philadelphia: SI사'4,
    1997.
10. C. K. Chui, An Introduction to Wavelets. San Diego, Calif.: Academic Press, 1992.
11. A. Cohen, I. Daubechies, and J. C. Feauveau, "Biorthogonal bases of compactly sup-
    ported wavelets," Commun. Pure App!. Math., 45, pp. 485-500, 1992
 CHAPTER SEVEN




Discrete Wavelet Transform
and Filter Bank Algorithms

 The discussion of multiresolution analysis in Chapter 5 prepares readers for an un-
derstanding of wavelet construction and algorithms for fast computation of the con-
 tinuous wavelet transform (CWT). The two-scale and decomposition relations are
essential for development of the fast algorithms. The need for these algorithms is
obvious since a str小ghtforward evaluation of the integral in (4.32) puts a heavy
computation load on problem solving. The CWT places redundant information on
the time-frequency plane. To overcome these deficiencies, the CWT is discretized
and algorithms equivalent to the two-channel filter bank have been developed for
signal representation and processing. The perfect reconstruction (PR) constraint is
placed on these algorithm developments. In this chapter we develop these algorithms
in detail. Since the semiorthogonal spline functions and compactly supported spline
wavelets require their duals in the dual spaces, signal representation and the PR con-
dition for this case are developed along with the algorithms for change of bases.
Before we develop the algebra for these algorithms, we discuss the basic concepts of
sampling-rate changes through decimation and interpolation.


7.1   DECIMATION AND INTERPOLATION

In signal processing we often encounter signals whose spectrum may vary with time.
A linear chirp signal is a good example. To avoid aliasing, this chirp signal must
be sampled at least twice at its highest frequency. For a chi叩 signal with a wide
bandwidth, this Nyquist rate may be too high for the low-frequency portion of the
chirp. Consequently, there is a lot of redundant information to be carried around
if one uses a fixed rate for the entire chirp. There is the area of multirate signal
processing, which deals with signal representation using more than one sampling
rate. The mechanisms for changing the sample rate are decimation and inte珏）olation.
We discuss their basic characteristics in the time and spectral domains.

                                                                                 141
        142     ［긔SCRETE ＼사AVELET TRANSF아카＼4 ANt) 디LTER BANK ALGO데THMS


        7.1.1 Decimation
    An ii不point dec恤a如nr曲ins only every M由 sai叩le 可 a given signal. In th帥me
    面ma虹 an M-point dec恤ation of an input sequen此 仁伽가 is given by

                                           y（川 = 工（nM)                                                       的rnEZ.                                                              (7.1)

 Figure 7.1 depicts the system diagram of an M-point decimator. The output of the
 decimator may be writ妃n in terms of a nroduct of x(n') and a seQuence of unit im-


                            u(n) =>                           x(n)6(n- kM)                                                          forkEZ,                                      (7.2)
                                              kEZ

 which selects only the kMth samples of x(n). The Fourier serie representation of
 the M-point period impulse sequence (7.2) is

                                                                                                  1 世二l
                               >；枷 H 幽 = 言 乞 戶2,rkn/M·                                                                                                                           (7.3)
                              kEZ                                                                 U1 k=O

Based on the geometric sum

                                                                                                        fork = t4f,                                    tEZ
                                                                                                        otherwise,
                       旨，              ' " ' " /"             -         j。   ,



the identity in (7.3) is     proved.                Writing                             y   (n)          =     u        (nM)            ,        the z-traisform of y      (n)    has
me rorm

                                                                       1 1f二1
                                       Y（乙）
                                          =言   2; X（之i/Me_f 2lrk/M)
                                            小- k=O


                                                                                                                                                                                 (7.4)
                                                                  M旨                               （:    " "       畔）               ,



                                                        "2' k'11
                                                                                                                                                   "



      the
                                                                                                                                            ee
where
             p여nt exponential basis
                  M-
                                            W                           used.function                                          :=                         has   been
                                                                                                                                                                                   In
me spectral aomain, we obtain me discrete卜ourier transtorm L)trl) or y(n) simply




              ｛工（n)}                                                                                                                                                   {y (n)}


                                       디GURE7.1                                         AnM巾아nt decimator.
                                                           DECIMATION AND INTERPOLATION           143

by setting z = e10) to yield

                                  1 世二l
                        9(eJ0)) = 言 2二 分（eit(m_2JnI)1M1).                                        (7.5)
                                                  k=O
The spectrum of the decimator output contains M
                                                   copies of the input spectrum. The
amplitude of the copy is reduced by a factor of l/ M.
                                                        In addition, the bandwidth of
the copy is expanded by M times. As a result, if the spectra
                                                              l bandwidth of the input
signal is greater than ir/M (i.e., 1wi > 7r/M), an M-point decima
                                                                     tor will intr에uce
aliasing in its output signal. We will see later that
                                                       aliasing does indeed occur in
a wavelet decomposition tree or a two-channel filter bank
                                                            decomposition algorithm.
However, the aliasing is canceled by carefully designing the
                                                             reconstruction algorithm
to remove the aliasing and recover the original signal.
    For M = 2, we decimate a sequence by taking every other
                                                                data point. From (7.4),
we obtain


                          Y (z)                  l
                                                 Z山    X         畇                    =



                                            1
                                            1
                                            小
                                            2
                                                 X         4二                               (
                                                                                            +
                                                                                            /
                                                   (
                                                                X(- 乙1/2刀                        (7.6)
                                                   4
                                                                                            H1




and

                      9(6"     )=
                                       ；匡
                                            （e兀    （,/
                                              " ')＋分                  ",
                                                                            ')］·                 (7.7)

The spectrum of 1 (ejw) is shown in Figure 7.2.
  For the sake of simplicity in using matrix form, we conside
                                                              r only the case where
M = 2. W이烙e, 2 加 the subscr巾to represent decima
                                                       tion by 2. We w血e

                                                [y] = [x]12                                      (7.8)




           A
         ＝告 0 퓽
                                                 1全（ejm)1



                                                       兀
                                                                                    A
                                                                                   [급끄 2ir 급끄




               FIGURE 7.2           Spectral characteristic of decimation by 2.
144     미SCRETE ＼사AVELET TRANSF아리i AND 디LTER BANK ALG아리THMS


as



                                 y (H2)                       工（-4)
                                 y (- l)                      工（中2)
                                 y (o)                        工（0)
                                 y (l)               =        工（2)                                           (7.9)
                                 y (2)                        工（4)
                                 y (3)                        工（6)
                                                              工（8)



In terms of a matrix operator, we write (7.9) as



                           0   0
                      l0
                                                                                  工（中2)
        y (- 2)             l1

                                               0l0
                                         00




                                                                                          巾m늬也臼巾i1
                                                                                  工（-1)
        y(- l)             00                        0   0                            工
        y (O)                                         l1        0   0                 X
                                                                                                             (7.10)
        y (l)                                        00          11
                                                                        00   0l
                                                                                      X
        y (2)                                                   00                    X
        y (3)                                                                         工

                                                                                      1
                                                                                  1
                                                                                  m


or

                                   [yl = {DEC+2] [x] .

The shift-variant property the
                           of
                                   decimator
                                             evident when we shilt the
                                                         is
                                                                              colunm                 input
either up or down by a given   number of position. In addition, the iecimation matrix
is an orthogonal  matrix since

                                [DEc1z] ' = [DEC42]t .

Consequently, decimation is an orthogonal transformation.


7.1.2    Interpolation
Interpolation of data means inserting additional data points into the sequence to in-
crease the sampling rate. Let y(n) be the input to the interpolator. If we wish to
increase the number of sample by M folds, we insert M - I zetos in between any
two adjacent samples so that the interpolator output gives


                      x'(n)＝卜    forn=kM, kEZ
                              （劫 otherwise.
                            (0,
                                                                                                             (7.11)
                                                           ［兀C小IAT回N AND 八TERPOLATION          145




      {y（兀）}



                         디CURE 7.3           An M-point intel꾸아ator.


The system diagram of an M-point inte叩olator is shown in Figure 7.3. We can also
write the expression of interpolation in the standard form of a convolution sum,

                             兀'(n) =＞二y(k)3(n - k凡0.                                        (7.12)
                                             k
The spectrum of the interpolator output is given by

                      x' (e/ ') =                          ）枷- kM)戶 "'
                                     n       k

                               =    ＞二 (k) J/
                                     k
                                         y
                                                 e_
                                                            cM0)
                               =    ; (e_ JMO)        ).
                                                                                            (7.13)
The z-transform of the inte叩이如rout四tis

                                     X' (z) = Y (zM).                                       (7.14)
Interpolation raises the sampling rate by filling zeros in between samples. The output
sequence has M times more points than the input sequence, and the output spectrum
is shrunk by a factor of M on the co-axis. Unlike the decimator, there is no danger
of aliasing for interpolator since the output spectrum has a narrower bandwidth than
the input spectrum. The spectrum of a twofold interpolator is given in Figure 7.4.


                                                                   1八. ,.,,. 1     images
                                                                   1.y (e
                                                                        "   J1
                                                                                 /71




               2                                                        4        2
               FIGURE 7.4 Spectral characteristic of interpolation by 2.
146     DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


  Using M = 2 as an example, we write


                          x' (n) = y(n)t2
                                 =                               (n/ 2)                  for n even
                                                                                                               (7.15)
                                                 Jy
                                                  10,
                                                                                         otherwise.

In matrix form we have




                                x' (- 2)                                            y (- l)
                                x'          (-             1)                       0
                                x' (O)                                              y (O)
                                x' (l)                                              0                          (7.16)
                                x' (2)                                              y (l)
                                x' (3)                                              0
                                x' (4)                                              y (2)




As before, we represent the interpolator by a linear matrix operator. It turns out that
the interpolation matrix is the transpose of the decimation matrix




                               l0 000 000             00l00000    00l000
          x'(- 2)                                                                                     y ( 2)




                                                                           0 00l0
          x' (- l)                                                                                    y I)
                                                                                                       (-
          x' (O)                                                                                      y (0)




                                                                                    000 l00
          x' (l)                                                                                      y (1)    (7.17)
          x' (2)                                                                                      y (2)
          x' (3)                                                                                      y (3)


                                                                                              00l
                                                                                                      ）小1)




or we can wnte


                                      [y] = [INTt2] [xl.                                                       (7.18)

   The operations of convolution followed by decimation and interpolation followed
by convolution are two of the most important building blocks of algorithms. They
will be used to build tree algorithms for wavelets and wavelet packets as well as
in two- and three-dimensional signal processing. We show only their time-domain
identities in the following sections.
                                               DECIMAT!ON AND INTERPOLA11ON       147



                                                   似（n)}                {y (n)}
                               {h(n)}


                  FIGURE 7.5 Convolution followed by decimation.



7.1.3   Convolution Followed by Decimation
Mathematically, we express this o比ration by

                              y (n) = {h(n) 永 工（7i)}12 ·                      (7.19)
The processing block dia얍am is given in Figure 7.5. If we label the intermediate
output as u(n), it is the convolution of x(n) and h(n) given by

                             u(n) = Jx(k)h(n
                                    k
                                            出.
The two- 日int decimation gives

                        y(n) = u(2n) = ＞二工（k）九（2n - k).                       I_7.20)
                                               k

7.1.4   Interpolation Followed by Convolution
The time-domain expression of this operatioil is given by

                            y(n) = {g（미H枷小小                                   (7.21)
Using v (n) as the intermediate output, we have

                             y(n) = ＞二v(k)g(n- k).
                                           k
Since v(k) = x(k/2) for even k, we have


                         ，小，각帥n - k)
                                 = ＞二工（Z)g(n- 2Z).                            (7.22)
                                       f

This process is shown in Figure 7.6.


                               加（n) }                                  {y (n)}
                                                    {g(n)}


                 FIGURE 7.6 Interpolation followed by convolution.
148        DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


 7.2    SIGNAL REPRESENTATION IN THE
        APPROXIMATION SUBSPACE

We have shown in Chapter 5 that the approximation subspaces An are nested so that
the subspace Aa그 = L2, A_          = {0}, and An C An+i for anyn E Z. For an
arbitrary finite-energy signal x(t), there is no guarantee that this signal is in any of
these approximation subspaces. That is, we may not be able to find a coefficient 口k,s
such that

                                工（t) =＞二口t，沖(2st - k)                                                                            for some工                                      (7.23)
                                             kEZ

To  make use of the two-scale relations                  a signal        be
                                                                          for
                                                                              one of      processing,                                                 niust                in
these nested approximation subspaces. One way of meeting this requirement is by
projecting the signal into one of the A5 for some s. 가1is is particularly important if
one only knows the sampled values of the signal at x (t = k/2S, k E Z) for some
large value of s.
    Assuming that the signal x(:) is not in the approximation A5we wish to find
x5 (t) E A5 such that

                     工（D   工小）=＞二ak,s
                     工(r) 르 工小） =yh叭 ,k,s(t) Z口k.s,
                                        ,m = y．따, b
                                                 沖（2
                                                  H
                                                    (25t
                                                        k
                                                         -的，
                                                      ' nk                                                      H

                                                                                                                     k
                                                                                                                                                              ;                 (7.24)

煮謐湍：鷺我紫黑：뜸黑巴黑：烈客然헒뺍謬；
using the orthogonal projection of x(t) onto the A5 space.
   C1; .,i1 A   ;1기 11 n. . 11』
                              끼11nn八 八iy r 2 n11』
                                                J 1戶 /1\ 戶 r2 . 1. 』1 nr111il;Jt111 1a r4\ k1기 .1..-..노1111111m八1mn1
   口1l' L.L i1S i ' a buubpaL.c us L. aiiu4(U二 iJ , w口 ..uII凸IU17.1.人S\1J. f1a UI드.uiuIu弓1,II口I
projection or x(t) onto me A5 suospace. men x(t) - x5 (1) is ortnPgona1 to A5 ana
mereiore ormogonai LU me oasis iuncuon Pt,S :

                                     ((x(t) - x5(t)) , 中t ,S) = 0                                                                 VZ E 7L.                                      (7.25)

Consequently, the coefficients are determined from the equation


                                                                                                                                                                                (7.26)
                     侮（!   )，   仇！      )=   (x   (t)       ，   仇！   )=             （구*                                  ,！九小）          ，   仇S
We expand the last equality, yielding


        2''乙(t)4(2'如= 2 [j뇨'『-k巾如］
                          -。。帥 기
                    上니400J 4i                                                                                                                                                   (7.27)


where    we   have
                     made a change of index m                                   =                       '   -   k.               The matrix      fo
                                                                                                                                                                  "of   (7.27) is
                                                           WAVELET DECO入伊O듸T幻N ALGORITHM                                 149



                      cr1        cr0       ci                            a刃i, S                      仁(t), 中m,s)
                                           a0       ci                                                                (7.28)
                                                    (y0


  ＼人／
    here


                                 cm :       /：中           （7）中（t         '
                                                                              m)
                                                                                        dt＝石

 is the autocorrelation of the scaling function 砂 (t). If
                                                          the scaling function is supported
 compactly, the autocorrelation matrix is banded with a finite-s
                                                                      ize diagonal band. If
 the scaling function and its translates form an orthono
                                                            rmal basis, then

                                                         am = 8m,0.

 By assuming an orthonormal basis, the autocorrelatio
                                                       n matrix is the identity matrix
 and the coefficients are obtained by computing the
                                                    inner product,

                                                a刃2,S = 似(t)，砂m,S> .                                                 (7.29)
 If we are given only the sample values of the signal
                                                      x(t) at x(t = k/25), we can
 approximate the integral by a sum. That is,



                            匈」
                                  'S
                                       =   2,
                                                "    乙
                                                              (t)
                                                                         q5 (257-               m)
                                                                                                     dt


                                       」2_SI'二唯小，
                                                《）·                                                                 (7.30)

This equation demonstrates the difference between the scaling
                                                                    function coefficients
and the sample values of the signal. The former are expans
                                                              ion coefficients of an ana-
log signal, while the latter are samples of a discrete-time
                                                              signal. For representation
of a given discrete signal in terms of a spline series of orders
                                                                 2 and 4, we have given
formulas in Section 5.6.



7.3   WAVELET DECOMPOSITION ALGORITHM

Let us rewrite the expression of the CWT of a signal
                                                                                        x (t):


                     w吻．t (b, 口） =                  스而    /:(       (!
                                                                             ）少    （=
                                                                                          ，흐）
                                                                                                       di
                                                                                                            '   .

                                                                                                                    (7.31)
15。        DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITI-I S

Let us denote the scale a = l/ 21 and the translation b = k/2s, where s and k belong
to the integer set 7L. The CW1' of x (t) is a number at (k/2S, 1/2') n the time-scale
plane. It represents the correlation between x(t) and *(t) at that time-scale point.
We call this the discrete wavelet transfor,n (DWT), which generates a sparse set of
values on the time-scale plane. We use

                              . . 1k 1\             (的 . . , It- k/2\ .               .    .
                   w,-". - == 印．.b
                                 '工 { 十.", 十'. 1 = / 工（  (f'itl, I . .; ', 1口，t       (7.32j.'
                    "."         'W \2  .'  2s)     f_아}-----r \ l/ 2S /               "

to represent the wavelet coefficient at (b = k/2S, a = 1/2). A discrete time-scale
map representing the signal x(t) may look like Figure 7.7.
   It is known that the CWT generates redundant information abo的he signal on the
time-scale plane. By choosing (b = k/21, a = 1/2S), it is much mhre efficient using
the DWT to process a signal. It has been shown that the DWT kehps enough infor-
mation of the signal such that it reconstructs the signal perfectly ' from the wavelet
coefficients. In fact, the number of coefficients needed for perfect reconstruction is
the same as the number of data samples. Known as critical sampli樞 this minimizes
redundant information.                                              1
    The decomposition (analysis) algorithm is used most often in 寸avelet signal pro-
cessing. It is used in signal compression as well as in signal identification, although
in the latter case, reconstruction of the original signal is not always required. The




      20


           1   女     女    *     *   *    女    *     *    女     *   *    女    女    女   女    S

      15

  은
  n
       n
       U


                                                                                           S




                                *                                                          S




                          0.2             0.4                0.6            0.6           10

                                                    b
FIGURE 7.7 Typical time-scale grid using the decomposition algori.hm. (Reprinted with
permission from [1], copyright （르）1995 by Springer-Verlag.)
                                                  WAVELET DECOMPOSITION ALGORITHM               151

  algori恤 separates a signal into components at various
                                                                scales corresponding to suc-
 cessive octave frequencies. Each component can
                                                        be processed individually by a dif-
 ferent algorithm. In echo cancellation, for examp
                                                          le, each component is processed
 with an adaptive filter of a different filter length
                                                      to improve convergence. The impor-
 tant issue of this algorithm is to retain all pertinent
                                                           information so that the user may
 recover the original signal (if needed). The algorith
                                                           m is based on the decomposition
 relation in MRA discussed in Chapter 5. We rewrite
                                                              several of these relations here
 for easy reference.
    Let

                    抑+1(t) E A:+i,＝수工：+1(t) = ＞二口k.s+1砂k,s11(t)
                     工，(t)
                             EA, 수     x
                                            (t)
                                                    =
                                                        >2k   口k,   s
                                                                        k,
                                                                             s   (t)
                     y小）E 1砥 놔             y (t) =>2蜘奴，小）.
                                                   k
 Since the MRA requires that

                                     AS+i =A5+ W5,                                           (7.33)
＼入／
  e have

                             抑卄（t) = 工S(t) + ys(t)

               Z口t,，加k.s+巾戶>2따，汭，小）+Z蜘奴，m1                                                  (7.34)
                k                          k                                 k
We substitute the decomposition relation

   砂아뇨H0= Z伽먀그似幻- k나h1 [2k - 1 lfr (2st - k) )                                              (7.35)
                       k
into (7.34) to yield an equation in which all bases a七 at resolut
                                                                  ion s. After inter-
changing the order of summations and comparing the coeffici
                                                               ents of 中k,S (t) and
*k,s (t) on both sides of the equation, we obtain

                              吼 = ＞二幻［2k -Z］吼＋l
                                       t

                              功k,s 스二幻 [2k -Z1 at,5+i
where the right side of the equations corresponds to decima
                                                               tion by 2 after convolu-
tion (see Section 7.1.3). These formulas relate the coeffici
                                                             ents of the scaling func-
tions and wavelets at any scale to coefficients at the next
                                                            higher scale. By repeating
this algorithm, one obtains signal components at various frequen
                                                                      cy octaves. This
algorithm is depicted in Figure 7.8, where we have used the
                                                               vector notation
    a了 := {ak,s},    wS := {Wk,S},    h0 := {ho[kJ} ,                   and h1 := jhi[k})   (7.36)
152     1긔SCRETE ＼八／AVELET TRANSFORM ANI) 디LTER BANK ALE；아리TH人IS




               aS+i




                            ws
               FIGURE 7.8    Single-level wavelet decomposition process.




with k e Z. This decomposition block can be applied repeatedly to the scaling func-
tion coefficients at lower resolution to build a wavelet decomposition tree as shown
in Figure 7.9.
   The reader should note that the wavelet decomposition tree is not symmetric since
only the scaling function coefficients are further "decomposed" to obtain signal corn-
ponents at lower resolutions. A symmetric tree may be constructed by decomposing
the wavelet coefficients as well. This is the wavelet packet tree discussed in Chap-
ter 8.



a4j




      WM니                                     WM M'
                      FIGURE 7.9     Wavelet decomposition tree.
                                                              RECONSTRUCTION ALGORITHM     153

7.4         RECONSTRUCTION ALGORITHM

It is important for any transform to have a unique inverse such that the original data
can be recovered perfectly. For random signals, some transforms have their unique
inverses in theory but cannot be implemented in reality. There exists a unique in-
verse discrete wavelet transform (or the synthesis transform) such that the original
function can be recovered perfectly from its components at different scales. The re-
construction algorithm is based on the two-scale relations of the scaling function and
the wavelet. We consider a sum of these components at the sth resolution:

                 차(t) +y小）= ＞二따,：砂k,s(t) + ＞二功k,，奴,, (t) = 工：+l(r).                      (7.37)
                                       k                      k
By a substitution of the two-scale relations into (7.37), one obtains

        ＞二따,스二go田m'H- 갸 - ) + Z功k,s Z毗岫(2' 끼口卜Z)
        k         t                                       k        t
                                  (2s+lt
             =        a,
                           s+ l            -     ).
                                                                                         (7.38)

Comparing the coefficients of 砂 (2s+It - Z ) on both sides of (7.38) yields

                           口t, +l= Z佃卜羽吼＋毗e羽蜘｝,                                          (7.39)

where the right side of the equations corresponds to interpolation followed by convo-
lution, as discussed in Section 7.1.4. The reconstruction algorithm of (7.39) is shown
graphically in Figure 7.10.



a凡f-M'           A八                            a4f中M'+I   aM_ i        八                   aM
  1m>




                              WM_M'                                            WM_1
    FIGURE 7.10 Signal reconstruction from scaling function and wavelet coefficients.
154     DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITH S          d
   We emphasize here that although the mechanics of computatio             re carried out in
digital signal processing fa針｝ion, the decomposition and reconst           tion algorithms
缸e actually processil培 analogs培nals. 가1e fund跏配ntal idea is toi            'esent an analog
signal by its components at different scales for efficient processin



7.5   CHANGE OF BASES

The algorithms discussed in Section 7.4 apply to all types of 卜caling functions
and wavelets, including orthonormal, semiorthogonal, and biort如gonal systems.
We have seen in Chapter 6 that the processing sequences {o[k], gj[k]}, and
{ho[k], h1[k]} are finite and equilength sequences for compactly supported orthonor-
mal wavelets. In the case of semiorthogonal wavelets such as compactly supported
B-spline wavelets, the processing sequences {ho[kj, h1[k]} are infinitely long. Trun-
cation of the sequences is necessary for efficient processing. T4 avoid using the
infinite sequences, it is better to map the input function into the idual spline space
and process the dual spline coefficients with go[k] and gi[k] that lave finite lengths.
This and the next two sections are devoted to m어ification of t妃 algorithm via a
change of bases.
    We have shown in Chapter 6 that the mth-order spline 吻n = Nm and the cor-
responding compactly supported spline wavelets 吻n are semiorthogonal bases. To
 compute the expansion coefficients of a spli므e series or a spline wavelet series, it
 is necessary to make use of the dual spline 吻n or the dual splii Le wavelet 少m. In
 semiorthogonal spaces, all these bases span the same spline spai:e Sm. For certain
 real-time applications in wavelet signal processing, it is more desi rable to use finite-
 length decomposition sequences for efficiency and accuracy. Ti erefore, it is nec-
 ess띠y to represent the input signal by dual splines of the sam(1order before the
 decomposition process.
    Let us recall the formulation of the multiresolution analysis, in which we have the
  approximation subspace as an orthogonal sum of the wavelet subspaces,

                 AM = 由 七1-h川，由A肛M'
                      = WM_1 由 WMe2 由 · · · q) WM M' e AM小J,                          (7.4.0)

 for any positive integer M'. Consequently, any good approximant xM E AM of a
 given function x E L2 (for sufficiently large M) has a unique (orthogonal) decom-
 position


                               工M =     MZ向
                                          YM尸n + 抑卜M/,                                (7.41)


                        W5
 where x5 E AS, andy5 E    ..Since中m and中m generate the same本IRA while．砂m and
 V'm generate me same wavelet sunspace ta property not possessPc1 ny mortnogonai
                                                                    CHANGE OF BASES      155
  scaling functions and wavelets that are not
                                                  semiorthogonal), we write

                   和(t) = Ek ak,s (2'卜            幻 = 已元畝2st 냐）
                  y5(t) = Zt 功k,泄(2'卜                                                  (7.42)
                                                  幻 = ＞그 毓, j但 '卜 k)
 for each s E Z. To simplify the implementation,
                                                  we have not included the normal-
 ization factor 2s/2.
    If we apply the decomposition formula (7.36) to the
                                                        scaling function coefficients,
 we have

                             口k,s = Z h0 [2k - 日口t,s+1
                             Ws,k = Z h1[2k -t] at,5+ j.                               (7.43)

 Since sequences {h0[k]} and {h1[k}) are infinitely long
                                                             for semiorthogonal setting,
 it will be more efficient to use sequences {go[k]}
                                                       and {gi[k]} instead. This change
 of sequences is valid from the duality principle, which
                                                           states that fg0[k], gl[k]} and
 {h0 [k] , hi [k]} can be interchanged, in the sense that

                                   {go[k] <-* h0 [-k}
                                                                                      (7.44)
                                   如［k] <+ m卜k]
when 中rn and 砂rn are replaced by 砂rn and 少rn. With the
                                                       application of the duality
principle, we have

                             ak,S = 工姑0[t- 2k盛,s+i
                             彷k,s = Z 1gi[t - 앉盛,什1.                                  (7.45)

Howev甲呻ke연vantage of the du띠lty'. pr,n卵틔we need的 transf야m 小e coef-
ncients aj,5 j to tak,s j. we recaii mat oom 叩a g generate me same A space,
                                                                            so
that 砂 can be represented by a series of出

                                中（t) =＞二rj,下（t- k)                                    (7.46)
                                              k

for some sequence {rk}. We observe that this change-of-bas
                                                               es sequence is a finite
sequence if the scaling function has compact support. Indeed
                                                             , by the definition of the
dual, we have



                           『（=
                            rk =   J
                                       fOO
                                       -
                                             中(t)中(t   -
                                                           k) dt.             (7.47)
Therefore, at the original scale of approximation, with
                                                        s = M, application of (7.46)
yields


                               a/. , M =     ＞二rk
                                              t
                                                       口t.   M,
                                                                                  (7.48)
156      DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS



aM




                      WM_I                                          WMHM'
FIGURE 7.11 Standard wavelet decomposition process implemented with change of bases.
(Reprinted with permission from [1], copyright (9 1995 by Springer-Verlag.)

which is an FIR operation. Observe that if we take splines as scaling functions [i.e.,
砂（r) = Nm(t)I, then rk = N2m (m - k); k = 0, 士1. . . . ...-           1 [1J. As we have
seen in previous discussions, the sequences {go[kj} and {gi[k]) in the decomposition
algorithm are finite sequences.
    We can summarize our computation scheme as in Figure 7.11. The computation
of 11k ,s, s = M - 1. . . . .M 寸 M', using aM as the input sequence requires 2M' FIR
filters. The importance of the coefficients Wk,s is that they constitute the CWT of XM
relative to the analyzing wavelet 砂rn at certain dyadic points, namely


      Wk.s =
               2s12
                       (WJIXM)
                                 "
                                      (} )
                                     " ＼乙'
                                             ,   =,
                                                 乙" /
                                                        ,   M   -
                                                                    4r <S   <M,   k C   Z.
                                                                                             (7.49)



7.6   SIGNAL RECONSTRUCTION IN SEMIORTHOGONAL SUBSPACES

The algorithm described in Section 7.4 concerns the recovery of the original data.
In that case, the original data are the set of scaling function coefficients {at,M j at
the highest resolution. Since the original input signal is an analog function x(t) 幻
XM(t) = 已 aC M (2Mt - ), it is necessary to recover the signal by perfor仙g the
summation. Recall that the decomposition algorithm discussed in Section 7.5 pro-
duces the spline and wavelet coefficients in the dual spaces, namely ({瓦小 {fik,巾.
To use finite-length two-scale sequences for the reconstruction, we must express the
coefficients in dual spaces in terms of ({ ak, } , {wk, }) in the spline and wavelet
spaces. In addition, if users need to see the signal component at any intermediate
steps in the decomposition, they would have to use the dual spline and dual wavelet
series. In both cases one can simplify the problem by a change of basis that maps the
dual sequences back to the original space [2]. Since the sequences do not depend on
the scale, the second subscript of the coefficients can be arbitrary. Such sequences
are applicable to mapping between any two different scales.
                      SIGNAL RECONSTRUCTION IN SEMIORTHOGONAL SUBSPACES                         157

 7.6.1 Change of Basis for Spline Functions
 Our objective is to write

                       s(t) = ＞二毓刃, (t- k) = ＞二따Nm(t - k).                                   (7.50)
                                       k                                  k

 By taking the Fourier transform of (7.50), we get

                                A (e/ ')Nm(w) = A (e3' ')Nm(w),                              (7.51)

where, as usual, the hat over a function implies its Fourier transform, and A(e)w)
and A (eJnJ) are the symbols of ta, } and {ik}, respectively, defined as

                     A(e ) :=Zake/tm,                               A(e') :=Z ake'km.        (7.52)
                                       k                                    k

   The dual scaling function Nm is given by

                               Pt! (,..\ 小 協佃）                                 ej口J/2,
                               1 1 m   \1J[/ /   -                  1    z =                 (7.53)
                                                      万Nm (Z2)

where EN,,, (z2) = IJm(W+ 2rk)尸 尹 0 for almost all w since tNm(· -k) } is a stable
or Riesz basis of A0. As discussed in Chapter 6, EN, , (w) is the Euler-Frobenius-
Laurent series and is given by

                              月N, ,（之2) = 1刃m(W + 2,rk기2


                                                 =     ＞二
                                                     k=-m+1
                                                               Nm
                                                                        (m+
                                                                                k)z2t.       (7.54)


It is clear that by multiplying (7.54) by 乙2m_2, we can get a polynomial of degree
2m - 1 in z2. The last equality in (7.54) is a consequence of the relation


         乞 If(w+ 2jrk)I2= 亡 [／므／(t + k)f而d小社띠
        k亡4以）                                    k= -o ) 1=V -u八J                        니
                                                                                             (7.55)
PROOF FOR (7.55): Using Parseval's identity, we have


                 ()
                「（
                 F
                  ()     :=
                         :=
                               J f (t
                                 foO
                                  -
                                   。。                + t) f (t) dt


                         = 訂如이' 小』
                                 CL)
                        ＝亡，효j.2r,(k+1
                            12k,r ' 函）나＝"" dw
158       DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS



                           ＝打,'",立，加『2枷）나-jwtdw.                                                                   (7.56)


It is clear the F(t) is the t th Fourier coefficient of a 27r-periodic function
rmN띠     1 亡느        4.    , 12 ==1. .     . .    . .         .- --'    n. .        ..    .   !  .
 ) i: 4n 1 * （口J .1. 乙L.兀 II ." Witfl tfliS reIQt,nn . ( I ."> Sl tnhlnnl5 n玎ecr1I." It l S eas" [O
＝日k=-co IJ ' '上／ - 1d1\ /1 / 1 ." r! 1111 11l1口 1뇨111L11J11,. \ r ."U7/ 1\J111/ n口 1J11V뇨1工J. 11 l口 V11口J 11J
show that


                            /:，《 刃；而dt       （
                                                 『卄）
                                                                                  =   N2rn      (』
                                                                                                     卄）            (7.57)

with SUppN2rn(t) = [0, 2m].
   Combining (7.51), (7.53), and (7.54) and taking the inverse Founer transform, we
get

                                             ak = ({an} * p[n]) (k),                                               (7.58)




                                   1
                                                       = Y' nlklz1'.                       Izi = 1.                (7.59)
                               EN,     (Z)                 'J   "     "       "             U                      "       '




                               P                       m    mZ닉   A
                                                                                                k 之 0,             (7.60)
                                                                                                                       =




                                                                          l
                                    /\i=                   시                                                       (7.61)
                                                            I-I智，J肖（사 H 入I)
and 사 : i = 1. . . . .2Pm are the roots of (7.54) with AI < 1 and 사入2J7, +i中1 = 1
for i = 1. . . . .Pm. Here Urn = (2m 小 1)! and Pm = m - 1. Observe from (7.54) and
(7.59) that

                                                 l          =             ,            1
                   ＼小 "FL.' =                                                                                      (7.62)
                    =rr "' "        EN,(1)                      Z客rn+iN2m(m+ 'c)
                                                                                                          =   1,
where the last equality is a consequence of the partition of unity property of cardinal
B-splines, described in Chapter 5.
   Roots 사 for linear and cubic splines are given below. The coefficients p[k]} are
given in Tables 7.1 and 7.2. The coefficients p[k] have better decay than {ho[k]} (see
Figure 7.12).
                                      SIGNAL RECONSTRUCTION IN SEMIORTHOGONAL SUBSPACES                                                       159

  TABLE 7.1                      Coefficients {p[kJ} for the Linear Spline Case (p[k} = p[-k])

                                            p[k]
               1
           k
                                                                                       k                                            p[k]
           0                                                                                 8
                                     1.7320510                                                                                0.46023608 x i0콕
           1
           1

                                                                                       O
                                                                                       / 0 l
                                   -0.46410170                                                                              小0.12331990 >( 10콕
           n
           乙

                                                                                         1l l
                                    0.12435570                                                                               0.33043470 x i0巧
           각
           U
                                   -0.33321008 x 10니                                                                        -0.88539724 x 10-6
           4
           냐


                                                                                       n乙 그1V 41 <U
                                    0.89283381 x 10_2                                                                        0.23724151 x 106
           <
           J
                                   -0.23923414 x 102                                                                        -0.63568670 x i0口
                                                                                       l l l l
           /
           b
                                    0.64102601 x 104                                                                         0.17033177 x 10口
           n
           /
                                   -0.17176243 x i043                                                                       -0.45640265 x 10-8


                       Linear spline (m = 2):


                                                   시＝
                                                              -
                                                                  2+        V了＝   },
                                                                                                                                           (7.63)


                                                p[k] = (1l)IkI,Jj (2_ ,三）1 '                                                               (7.64)

                        Ci力ic 叩／mne （刃i = 4):


                                                A1 =              1486946 x
                                                                                  i0- "
                                                        -9.
                                                                                                      =
                                                                                                              A6
                                                              A2 =    -0.
                                                                             1225546                                                       (7.65)
                                                                                                      =   -A5
                                                              A3 =   -0.
                                                                             5352805 =                    -        -   .




TABLE 7.2                       Coefficients {p[kl} for Cubic Spline Case (p[k] = p[-k])

                                           p[k]                                        k
       1
                                                                                                                                  p[k]
   k
0 l 23 4 56 78 9 mH 口 日 니
                                    0.49647341                                     15                                      -0.51056378 x 10e3
                                  -0.30910430                                      16                                        0.27329483 x i04
                                    0.17079600                                     17                                      -0.14628941 x i04
                                  -0.92078239                                      18                                        0.78305879 x l0콕
                                    0.49367899                                     19                                      -0.41915609 x i0니
                                  -0.26435509                                      20                                       0.22436609 x i0니
                                    0.14151619                                     21                                      -0.12009880 x i0U4
                                  -0.75752318 x 10니                                22                                       0.64286551 x 10巧
                                   0.40548921 x 10-1                               23                                      -0.34411337 x 10巧
                                  -0.21705071 x 10-1                               24                                       0.18419720 x i0巧
                                   0.11618304 x 10-1                               25                                      -0.98597172 x 10-6
                                  -0.62190532 x 10-2                               26                                       0.52777142 )< 10-6
                                   0.33289378 x 10小2                               27                                      -0.28250579 x 10-6
                                  -0.17819155 乂 10-2                               28                                       0.15121984 x 10-6
                                   0.95382473 x 104                                29                                      -0.80945043 x i0口
 160               DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


                                                                                           1
       0
                                                             0               1             1



                   스-4 log(1hi［丸］)
  -5
                                                                  - 144 lOg(1/il [t])
                                                        -5
                   合숍4log아m[k])
                                                                    스숍小 log(1ho[k])
                   H4log(Ip[kl)
                                                                    ... log(p[k])
                   - log(1q[k])
                                                                    的＋ log(Iq[kl)
 -10                                                   -10
           0              5          10          15               0         10            20           30
                               k                                                  k
                              (a)                                                 (b)
FIGURE 7.12 Plots of h0[k], h1[k], p1k], and q[k] versus k for (a) linear and (b) cubic
spline cases.




7.6.2          change of Basis for Spline Wavelets
Here our objective is to write

                              r(t) =＞二而k沆따幻＝＞二切艸小a).                                               (7.66)
                                     k                        k

Replacing Nm by 砂rn in (7.53), we get the relationship between 砂m and 砂m. Pro-
ceeding in the same way as before, we get

                                          Wk = ({iI } *q[n])(k),                                   (7.67)
where

                                     .     l          ==5乙帥加k.                                     (7.68)
                               ＞二kl吻n(w+ 27rk）尸              느.1 -
Furthermore, we have

                    I1/'rn佃+ 2兀k)I2 = EN,,,(Z2)EN,,,(Z)EN, ,( Z),                z = 1.            (7.69)
               k
PROOF FOR (7.69): With the help of a two-scale relation, we can write


                                          小p (1' 二’"' )]Nm('「：
                                                                                               2
  刃沆佃仙삐2
       k
                                     ＞二
                                     k                       「"' )                                 (7.70)
                  SIGNAL RECONSTRUCTION IN SEMIORTHOGONAL SUBSPACES                              161

＼人／
  ith
                           G    m    m
                                     二
                           /=   ;
                                J
                                 e
                                           ;＞二gi[              k] '. 12.
                                                                       ej
                                                                                               (7.71)


Now separating the right-hand side of (7.70) into parts with even k and odd k and
making use of the relation (7.54), we can write

        刃沆佃＋2兀硏＝IGi(z平ENm(Z) +IGi(- 釧2EN, ,(-Z).                                               (7.72)
        k

From the relation IGi(z) I = I GO(- Z)EN,,, (- z)I, with Go(z) defined in a similar way
as in (7.71) with gj[k] replaced by go[k], we can write


        ZI*m佃＋2兀k)
        k
                 I2니回-z)I2ENm(1Z) + Go（釧' EN,,(Z)j
                                  x EN,,,(Z)ENm ( Z).                                          (7.73)

Following the steps used to arrive at (7.72), it can be shown that

                1아已fENm( Z나四毗平助,,, (z) = EN,,, (z2).                                           (7.74)

which, together with (7.72), gives the desired relation (7.69).
   The expression for q[k] has the same form as that of p[k] with Urn = -[(2m -
1)!]3, Prn = 2m -2, and A being the r어）ts of (7.69). Observe from (7.68) and (7.69)
that

                                          k]            : ,,
                                                                            ,)                 (7.
                                                               1
                                                    =
                                                        ENm (               l)
                                     q[
                                                    =
                                 k                                                               75)

since EN,,, (1) = 1. Roots 入, and >Jk q[k] for linear and cubic splines are given
below. The coefficients are given in Tables 7.3 and 7.4. The coefficients q[k} have
better decay than {hi[k]} (see Figure 7.12).



TABLE 7.3 Coefficients {q[k]) for the Linear Spline Case (q[kj = q[-k])
    k
                       q[kJ                                        k                    q[kj



                                                                       8 9 0 l
    0
                4.3301268                                                         0.92047740 x i0콕
    1
    1
    1
               -0.86602539                                                       -0.24663908 x i0극
    ）
    느
                0.25317550                                                        0.66086895 x l0巧
    m
    1
    V
               -0.66321477 x 10_I                                                -0.17707921 x i0巧
4
1                                                                  乙
                                                                   n
                0.17879680 x 10니                                                  0.47448233 x 10H6
                                                                   八4V 4
<
U
               -0.47830273 x 10_2                                                -0.12713716 x 10_6
6
                0.12821698 x 10_2                                                 0.34066300 x i0口
/
m                                                                  U
                                                                   1
                                                                   <
1              -0.34351606 x i04                                                 -0.91280379 x 10-8
162                                  DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS

TABLE 7.4                               Coefficients {q[k]} for the Cubic Spline Case (q[k] = q[-k])
t
                                                     qk                                                       k                               qk




 0 l2 3 45 6 7 8 9 0 l 2 3 4 5 6 7
                                             33.823959                                                        18                        0.39035085 x i04
                                           -13.938340                                                         19                      -0.20894629 x i04
                                              9.0746698                                                       20                        0. 11184511 x 104
                                            -4.4465132                                                        21                      -0.59868424 x i0극
                                              2.504188 1                                                      22                       0.32046413 x i0콕
                                            小1.3056690                                                        23                      -0.17153812 x i04
                                              0.70895731                                                      24                       0.91821012 x i0巧
                                            -0.37662071                                                       25                      -0.49149990 x 10巧
                                              0.20242 150                                                     26                       0.26309024 x i0巧
                                            -0.10811640                                                       27                      -0.14082705 x i0巧
                                              0.57940185 x 10_ i                                              28                       0.75381962 x 10 6
                                            -0.30994879 x 10_ i                                               29                      나0.40350486 >< 10小
                                              0.16596500 x 10_ i                                              30                       0.21598825 x 10小6
                                              0.88821910 x 10_2                                               31                      -0.11561428 x 10 6
                                              0.47549186 x 10_2                                               32                       0.61886055 x i0口
                                            -0.25450843 x 10_2                                                33                      -0.33 126394 x i0口
                                              0.13623710 x 10나2                                               34                       0.17731910 x 10力
                                            -0.72923984 x 10-s                                                35                      -0.94915444 x 10出


                 Linear spline (m = 2):


                                                       시      =              7.    179676八 小 '                    긋，
                                                                                                                                                   (7.76)
                                                                                  A2 =
                                                                                               2679492=
                                                                                         -0.
                                                                                                                           -A3
                                                                                  ＞二q[k]       =    3.   0.
                                                                                                                                                   (7.77)


                  Cubic spline (m = 4):


                                                     시    =       8.
                                                                        3698615 x
                                                                                                   i0- '      =
                                                                                                                           A12

                                                     A2 =                          1486955 x
                                                                                                         i0」
                                                                                                           "
                                                                        9.
                                                                  -
                                                                                                                                 Au
                                                                                                                       =
                                                                        5019634 x 10-2
                                                                                                              =
                                                     A3 =
                                                                                                                           A1 。
                                                                   1.
                                                     入4 = 小0.1225546 = !-
                                                                       入9

                                                     A5 = 0.2865251 = !
                                                                              EXAMPLES   163


                                               入6 = -0.5352804 그
                                                                         人7


                                               ＞二q[k] 18.5294121.
                                                            =




7.7        EXAMPIES

In Figure 7.13 we have shown decomposition of a music signal with some additive
noise. Here the music data are considered to be at integer points. Intermediate ap-
proximate functions sj and detail functions r1 have been plotted after mapping the




 40卜                     1
e20 n. .A,.,nn.,.n,,巾.小,W,.d
' 0 r빠뻐텍巾켜뻬作弑神쌔
1
      20   r           .   '   1   '   "        '


-40 나口＝   H1＝                                  나H
    0   200                                    400

      40   r                                                        40

       20 Lk . .AA.AnAI,,.n,,111.1h血．d, 14h,                    Z20
-
     ,'20t-
        0 m捌Y拂拂켸빠肺뻬川牡      "        1  "                '
                                                                ['200
                                                                -




-40 匕                                                           -40


      40   r                               .                        40

윽斗 LA . AA., AA.A.n.JA규..m小, 曾0
()I oLd十뻬뻬巾神邯帥뿌뻬빼寸                                              ,_' 0
中     20   I-              "       "                "           -   20
-40 L                                                           -40


      40   r                                                        40

윽斗 L .. A A.d. n ,AAA . 八八小A... 윽20
m' 0 n伊卄쌔W的뻬W樹V叫쎄們七／ -I 0
 -    20   r                                                    -   20
-40 '-                                                          -40
                   디GURE 7.13 Decomposition of music signal with noise.
164            ［기SCRETE WAVELET TRANSF아tM AND 디tIER BANK ALG아tITH入'is




      10


읗5
                 0.1   0.2   0.3   0.4   0.5


                                                10
                                               e
                                               J
                                                 仄U




       日L나
                 k1
           0     0.1   0.2   0.3   0.4   0.5              0.1   0.2   0.3   0.4   0.5


      10

 （니
U)' 5



       0                            I     I
           0     0.1   0.2   0.3   0.4   0.5              0.1   0.2   0.3   0.4   0.5




                                               1e
                                                nd
      10

 1r)
U)1    5

       0   口＝ mJ1中m규1七m       I     I1    I      01＝ 니1그쏘스4I1          I1          I
           0     0.1   0.2   0.3   0.4   0.5          0   0.1   0.2   0.3   0.4   0.5
FIGURE 7.14 Magnitude spectrum of the decomposed music signal, indicating the lowpass
and bandpass filter characteristics of scaling functions and wavelets, respectively.



dual spline and wavelet coe什icients into the original space with the help of coef-
ficients p[k] and q[k] derived in this chapter. To illustrate the lowpass and band-
pass characteristics of splines and wavelets, respectively, in Figure 7.14 we show
the magnitude spectra of the decomposed signals at various scales. The reconstruc-
tion process is shown in Figure 7.15 using the same sequences ({go[kj}, {gi[kl}) as
were used for the decomposition. The original signal s (t) is also plotted next to the
reconstructed signal sO(t) for the pur螂e of comparison.
    To further expound the process of separating a complicated function into several
simple ones with the help of wavelet techniques, we consider a function composed
of three sinusoids with different frequencies. These frequencies are chosen such that
                                     TWO-CHANNEL PERFECT RECONSTRUCTION FILTER BANK                 165



         40                                                              40
 =20
      H)
                                                                   '20
     0)1   0                                                   p.'
                                                              L,

     -20                                                      -0
     -40                                                                 2。
                                                                         4。
               0        200                       400                      0
                                                              -
                                                                                200           400


         40r                                                             40
   20 1 A. A,.AnnJ,,4. AAU, 小A
                                              .




                                                               20
 0' o n十뼈掛神批뿌뻬뻬뻬寸                                            뇨' 0
  20
 -40 匕
     -
               r                 "        "         "         叫20
                                                              小40


         40    r                                                     40

윽20 h. .n , .Ahk,UHL小．d, 小, Q20
0' 0 nV쌔卄神邯批布빠뻬뻬寸 U 0
 卞
  20
 -40 匕
               r             '        "                      -20

                                                             -40



         40    r                                                   40     卜                   1
Q20 h. .A,., 1n,,加山h小．11, 小, e20 L . . A,., 14S,1,,thAII 1L
才Or빠삑伊掛拂拂脯斟쌔뺘if ' 0 빠쌕掛켸쌔拂掛r
 -20 r
 _40t
                             ' '                             -20 r
                                                             小40 11
                                                                                  ' ]' "
               FIGURE 7.15           Reconstruction of the music signal after removing the noise.


they correspond to octave scales. As can be seen from Figures 7.16 and 7.17, standard
wavelet decomposition separates the frequency components fairly well.


7.8           TWO-CHANNEI PERFECT RECONSTRUCTION FILTER BANK

Many applications in digital signal processing require multiple bandpass filters to
separate a signal into components whose spectra occupy different segments of the
frequency axis. Examples of these applications include a filter bank for Doppler fre-
quencies in radar signal processing and tonal equalizer in music signal processing.
Figure 7.18 demonstrates the concept of multiband filtering. In this mode of multi-
166              DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


                                                                                         15

                         1 1 1 1 1 1 1 1                                                 10
                                                                               小
                                                                               니4
                                                                               니
                                                                                (0
                                                                                         5

                     1                         1                 11
                                                                                         。JU\7니                         .       .
                               0.01           0.02           0.03                             0   1000   2000       3000    4000

                                     1 I        I I                                      2
                         1 1          1 1        1 1
 色으m
                 1

        八U
                                               1                      I.
                                                                               '         0           1          1           +

    -   2    m       1 1                                                             -   2


        2

 e
 旱                                                                     1
                                      1                      1
        0


                           1
                                41
                                               1
                                                             1 1
                                                                      F        g         0

        n
        /
                                                                                     -   2                          H
                                                                                                                    e




        2                      1



                               ?1
                 1                        1              1                 1
 O나얻m
                                                                               三
                                                     y

        0                                                             1
    -   2
                                          1
                                                         4
FIGURE 7.16 Decomposition of a signal composed of three sinusoidi with different fre-
quencies corresponding to octave scales.


band filtering, the spectral bands corresponding to components ofthe signal may be
processed with a different algori血 to achieve a desirable effect on the signal. For
Doppler processing and tonal equalizers, there is no need to recoistruct the original
signal from the components processed. However, there is another form of filtering
that requires the original signal to be recovered from its compolent: the subband
filter bank. The major application of subband filtering is in signal compression, in
which the subband components a七 coded for 町chiving or transmission purposes.
The original signal can be recovered from the coded components with various de-
grees of fidelity.
    We use a basic two-channel perfect reconstruc如n (PR) filter b申k to illustrate the
main features of this algorithm. Filter bank tree structures can be constructed using
                               TWO-CHANNEL PERFECT RECONSTRUCTION FILTER BANK      167



            2                                                2
                                                  e
                                                             1mJ
                                                               n
                                                               U
는． 0                                              二
(0
                                                                                      1
                                                  L
                                                              1
                                                             n
                                                             Z
                    .    1     1口     1      I
                                                                 n
                                                                 U
     -21-
                0       0.01        0.02   0.03                      0.01   0.02   0.03

                                                             n
                                                             <


                                                  e
                                                  ?          0




                                                        -2
            2


윽0                                                    0나乎



     -2
FIGURE 7.17 Decomposition of a signal with t뇨ee frequency components (continued from
Figure 7.16).



this basic two-channel filter b카lk. A two-channel filter bank consists of an analysis
section and a synthesis section, each consisting of two filters. The analysis section
includes a highpass and a lowpass filter that are complementary to each other so that
information in the input signal is processed by either one of the two filters. The block
diagram for a two-channel PR filter bank is shown in Figure 7.19.
   The perfect reconstruction condition is an important condition in filter bank the-
ory. It establishes the unique relationship between the lowpass and highpass filters
of the analysis section. Removal of the aliasing caused by decimation defines the
relations between analysis and synthesis filters. We elaborate on these conditions in
much greater detail below.
 168     DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS




                                                                          (!)

                                                                     y (t)
                                                                      1
                                                                 y,
                                                    1




                                              HN
                                                                y系
                                                                           )
                         FIGURE 7.18 Multiband filter bank.


    The filters in a two-channel PR filter bank are specially designed so that the corn-
nonent s므nals may be reconstr叩ted nerfectly with no loss of infotmation. The out-
put or me niter oani is simpiy a aesayec version or me input signal. ior a two-cnannei
filter bank, the filtering operation is exactly the same as the wavelet algorithm. Be-
cause of the PR condition and the need to remove the aliasing components in the
output, one needs to design only one of the four filters. For further detail on filter
banks and how they relate to wavelet theory, readers are referred te [3-7].


7.8.1   Spectral-Domain Analysis of a Two-Channel PR Filter Bank
Let a discrete signal X (z) be the input to a two-channel PR filter bank as shown in
Figure 7.19 in terms of z-transforms with intermediate output signals. The analysis




x(n)
                                                                                 x*(n)




             디GURE 7．杓 如hannel perfect reconstruction fil：町由.               k.
                                                          iWO-CHANNEL PERFECT RECONSTRU口ION FILTER BANK                                                                                                                                             169

section of the filter bank consists of a lowpass filter Jfo(z) and a 뇨ghpass filter Hi(z).
The convolved output of the lowpass filter Ho(之) followed by a two-p아nt decimation
(4 2) is

                    U(z)                          =           {     [X
                                                                              (z
                                                                                         "2)     H
                                                                                                             (z112)                            + X(- z112)H。                                         (-             -z
                                                                                                                                                                                                                         '12)],                   (7.79)

while the highpass filter Hi(z) with decimation yields

                                                                                                                                                       X                                        m
                                                                                                                                                                                                                                                  (7.80)
                                                                              （尸'
                                                                                                                                                   H
                                                                                                                                                   1




                    『       （:               ）귿                     ［!                     ）月1
                                                                                                               (z112)                          +
For analysis purposes, we assume that the outputs of the analysis bank are not pro-
cessed, so that the outputs of the processor labeled U' (z) and V' (z) are

                                                                                                 U' (z) = U(z)
                                                                                                     V' (z) = V(z).

After the interpolator (t 2) and the synthesis filter bank Go(乙) and Gi(z), the outputs
of the filters are

                U
                        "
                                       (z)                =   {           [X (z)Ho                     (z)
                                                                                                                        Go          (z)        + X           (-
                                                                                                                                                                             z)
                                                                                                                                                                                  Ho            (-
                                                                                                                                                                                                               z)
                                                                                                                                                                                                                         Go         (z)   ]       (7.81)

and

                V
                        "
                                 (z)                  =       三          [X
                                                                                   (z)
                                                                                          Hi         (z)
                                                                                                                        Gi    (z)              + X(- Hi                 z)
                                                                                                                                                                                         (-
                                                                                                                                                                                                          z)
                                                                                                                                                                                                                         Gi   (z)         ].      (7.82)

These outputs are combined sync뇨onously so that the processed output X卓 (z) is

                X*(z) = U" (z) + V" (z)

                                                      =       {          X(z)[Ho                     (z)
                                                                                                                        Go    (z)              + Hi               (z)
                                                                                                                                                                                  Gi ]
                                                                                                                                                                                   (z)
                                                                                         (1乙）[Ho                                               Go                       +H1                                              G1               ]   .   (7.83)
                                                                              乙
                                                                                                                                                                                         （小乙）
                                                                                                                                                       (z)                                                                    （之）
                                                              +!X                                                                         z)
                                                                                                                         (-
The second term of the expression contains the alias version of the input signal [one
that contains X(- z)]. For perfect reconstruction, we may choose the filters Go(z)
and Gi (z) to eliminate the aliasing component. We obt恤 the aliasing-free condition
for the filter bank

                                                                                          Go(z) = 士Hj(- z)
                                                                                          G1(z) = 干Ho(- z).                                                                                                                                       (7.84)

Once the analysis filters have been designed, the synthesis filters are determined au-
tomatically. Choosing the upper signs in (7.84), the output of the filter bank becomes
170      DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


                  X'   (z)       =         {X
                                                       (z)        ［飾（:               ）尸1
                                                                                                      (-
                                                                                                                    z)       －
                                                                                                                                      月i          (z）        蜘（-   z)
                                                                                                                                                                           (7.85)

The perfect reconstruction condition requires that X京 (z) can only be a delayed ver-
sion of the input X (z) [i.e., X* (z) = X (Z)Z_m for some integer rn]. We obtain the
following relations:


            月"(z)Go(z)＋月'(z)G1(z)＝珦（ .' )．므'(.'.' )',，月．
                                                      '(')．少‘).
                                                                                                                                                                           (7.86)

                                 = Ho(z)Go(z) - Ho(- z)Go(- z)                 =                 ri0 (Z八끄八ZJ m                                           n0 (H乙J4J0 (1乙J   (7.87)
                                                                               =2zem.                                                                                      (7.88)

We define the transfer function of the filter bank:


                      ［怖的小如如］
                  T小孚斗；
                             =       _m.
To simplify the analysis, let us also define composite filters C0(z) and Ci(z) as prod-
uct filters for the two filtering paths

                             Co(z) = Ho(z)Go(z) = -Ho(z)Hi(- z)
                             Ci(z) = Hi(z)Gi(z) = Hi(乙)Ho(- z)
                                                = -Ho(- z)Go(- z)
                                                = -C0(- z),                                                                                                                (7.89)

where we have made use of the aliasing-free condition. In term旨 of the composite
fliters, me YK conaiuon Decomes

                                                      Co(z) - Co(- z) = 2z1m                                                                                               (7.90)

and

                                                T(z)              =       二[Co             (z)             -
                                                                                                                         Co      (-    z)               ].                 (7.91)

If we design a composite filter Co(z) that satisfies the condition in (7.90), the analysis
filters Ho(z) and Go(z) can be obtained through spectral factoriztion. We will have
numerical examples to demonstrate this procedure in later sections.
    We note that the transfer function T(z) is an odd function since

                                       T
                                                 (-
                                                             乙)       =   !乙   [C0
                                                                                                 (-
                                                                                                               z)        -            C。 ]  (z)
                                                                      = -T (z).                                                                                            (7.92)

The integer rn in (7.90) must be odd, which implies that Co(z) must contain only
even-indexed coefficients except Cm = 1, where rn is odd. Finding JJ (z) and Hi(z)
                             TWO-CHANNEL PERFECT RECONSTRUCTION FILTER SANK                        171



            IHo(eiw)I                                          IHl(eJa)I
10
 .
0.5




      0                                     플                                      7T

                 FIGURE 7.20       Spectral characteristic of quadrature mirror filter.




[or Ho(z) and Go(z)} to meet the PR requirement is the subject of filter bank design.
Two basic approaches emerged in the early development of PR filter bank theory:
(1) the qua血ature 恤ror filter (QMF) approach, and (2) the half-band filter (HBF)
approach. In this section we discuss the fundamental ideas in these two approaches.

Quadrature Mirror Filter Approach Let us choose Hi(z) = Ho(- z). We have,
in the spectral domain,

                                     Hi(ej(u) = Ho(Hejm)
                                                  = Ho(ej（回+7r) ).                              (7.93)

The spectrum of the highpass filter H1(ei-') is the mirror image of that of the lowpass
filter with the spectral crossover point at cv = 7r/2, as shown in Figure 7.20. The
transfer function becomes

             T(z)＝三［月訊）．斫（:)]=;[H訊）-Ii註：)]=r' ·                                                 (7.94)
Suppose that Ho(z) is a linear phase十 FIR filter of order N, so that

      tA function f E L2(1t) has linear p口se if
                                         f (w) = 士IIcv)Ie山1口a,,
 where a is some real constant. The function f has generalized linear phase if

                                         只功＝會（a加-Jow+b,

 where 百(w) is a real-valued function and constants a and b are also real-valued. To avoid distortion in
 signal reconstruction, a filter must have a linear or generalized linear phase.
                172                       ［긔SCRETE ＼사AVELET TRANSF아깁＼lANE) 디LTER BANK ALG(가리THN仔


                                                                飾（/ '           )=
                                                                                               e
                                                                                                                1(   ",
                                                                                                                          )("             사蜘
                                                                                                                                                                  （.j '            )1
                                                                m (r" ' ) =                    e
                                                                                                   'jE
                                                                                                                 (+         ,
                                                                                                                                /2]
                                                                                                                                      (肛l)                             1飾
                                                                                                                                                                             （.j ("                 '   ）기·
               The spectral response of the transfer function becomes


                                                                                                                                                                                                                        1]
                                                        1             . . . . . .. .. r,                                    . 12
                                      T            )=                 J I2X. 1)                                           (e")                                              1) .. .1 1                              . 121
                                               "
                                                                                                                                                                                      Hi                                                     (7.95)
                                                                                     N_
                                                                                                                                                                               N_
                                          (e
                                                            e
                                                                                                         LI月b
                                                                                                                                      I
                                                                                                                                          "          -            (_
                                                                                                                                                                                                              (e.
                                                                                                                                                                                                                    '        '
             (N 1) is even,
               If
                                  -  '   0 the crossover        TeJ
                                                                   w      2! Thetransfer
                                                                          .=              at
                                                                                                                                                         point
                                                                                                                                                                                        .=
                                                                                                                                                                                               兀/
                                                                                                                                                                                                                                 function
           proauces sev.ere am,lpiituoe aistortion at tnis point, ana.mat violates me,YK require-
           meni. i nerelore, iv musr ye even. ii we wisn LO eni끄ate all ampn甲ue uistornon ior
           even N, we must have the spectral amplitude of Ho(z) and Hi (z),         fying


                                                                               1蜘（/"기 니H1(ej")12 =2.                                                                                                                                         (7.96)

        Observe that the condition (7.96) differs from the normalized form by a factor of 2 on
       the right-hand side. This happens because previously we used a normalizing factor
       in the definition of a z-transform with two-scale and decomposition sequences.
           The trivial solution to (7.96) is the sine and cosine function for 110(e)0-') and
       Hi Ce)口'), which contradict our initial assumption for an FIR filter. Any nontrivial
       linear-phase FIR filter H0 causes amplitude distortion. If the right-hnd side of (7.96)
       is normalized to unity, the type of filter that satisfies 小is normalizdtion is the power
       complementary filter, an 1W filter that can be used in HR-PR filter banks.
          Returning to (7.94), if we restrict the filters to be FIR, Ho(z) can have at most two
       coefficients, so that H (z) has only one term with an odd power of zH1. It is easy to
       see that this solution leads to Haar filters. We discuss these filters further when we
       discuss orthogonal filter banks.


       Half-
              Filter Approach Observe from 89) th if we allo ' only causal FIR
                           Band
                                                                                                                                               (7.
                                                                                                                                                                              at
filters for the analysis filter bank, the composite filter Co is also causal FIR with only
one odd-indexed coefficient. To overcome this restriction, we can design anticausal
or noncausal filters and then add a delay to make them causal. We first simplify the
analysis by adding an "advance" to the composite filter and by m出king use of the
properties of a half-band filter defined below. The composite filter Co is advanced by
m taps, so that

                                                                                                   S(z) = zmCo(z),                                                                                                                          (7.97)

whe,
                    re            S,(z) ,is a noncausal                        filter symmetric with                                                             respect                     to the origin. The PR
ti。
  n                 bec。
                                     mes                                                                                                                                                                                                    condi-



                                                                                                   S(z) + S(- z) = 2                                                                                                                        (7.98)
                                   TWO-CHANNEL PERFECT RECONSTRUCTION FILTER BANK                                                                                                     173

since S(- z) = (- z)mCo(- z) = -zmCo(- z) for odd m. All even-indexed coef-
ficients in S(z) are zero except s(0) = 1. S(z) is a half-band filter satisfying the
白加wing condit奴is:

    1. s(n) =Oforallevennexceptn =0.
    2. s(0) = constant.
   3. s(n) = s(- n).
   4. S(eJw) + S(- eHJ0) = constant.

    This half-band filter is capable of being spectr出ly factorized into a product of two
filters. We use examples to discuss the HBF.
    To find the solution to (7.98), let H1(z) = _z_mHo(_z_ l); the 甘ansfer function
becomes

          T(z)   =
                      三 [Ho
                                        (z)
                                                   H (-             z)
                                                                               -
                                                                                     Hj         (z)
                                                                                                      Ho    (-
                                                                                                                       z)
                                                                                                                            ]
                 =            _m
                                              [_
                                                   Ho         (Z)
                                                                         HO
                                                                                   (Z_
                                                                                                 1)
                                                                                                      (_ 1)      _rn
                                                                                                                            + Ho      (-
                                                                                                                                           z)
                                                                                                                                                Ho   (-
                                                                                                                                                               z-
                                                                                                                                                                    -   ')
                                                                                                                                                                             }.
                                                                                                                                                                                   (7.99)
In view of (7.90), m must be odd. We have the expression

                     (z) =
                                                                                                                                                                                  (7.1叫
                                                   rn
                 T                 l_
                                                        [Ho
                                                                         (z)
                                                                                   Ho     (z-
                                                                                                       ')
                                                                                                            + Ho            (-
                                                                                                                                 z)
                                                                                                                                      Ho   (-
                                                                                                                                                z ')      }.
The filter bank has been designed once the half-band filter has been designed. The
resultant filters are listed as follows:

                                                    S(z) = 月0（乙）H0仁小
                                                   Co(z) = Ho（乙）／了0（尸）z叫rn
                                                   Ci (z) = _Ho(z)Ho(Z_ l)Z_m
                                                   Hi(z) = -zem1五）(- 尸）                                                                                                           (7.101)
                                                   Go(z) = Hj(- z)
                                                   Gi(z) = -Ho(- z)
                                                    T（乙） 나                               [S(z) + S(- z)] .

The lowpass filter Ho(z) comes from the spectral factorization of S(z).

Example 1: We use the derivation of the Daubechies [5] scaling function coeffi-
cients as an ex町llple. Let us recall the conditions on the half-band filter,

                                                                    S(z) + S(- z) = 2.

The simplest form of S(z) other than the Haar filter is

                                               S(z) = (I + z)2(l + zH1)2R(z).                                                                                                     (7.102)
174         DISCRETE WAVEL日TRANSFORM AND FILTER BANK ALGORITHMS

All even coefficients of S(z) must be zero except at 0, where s(0) = 1. Let

                                                           R (z) = 口乙 + b + 口z니

be a.noncausal symmetric filter so that S(z) remains. symmetric. 耳y carrying out the
aigeDra in t 1.1O乙) ana using conciiflons On ) (z), we nave

                                       S(0) = 1        ＝수                                8口 +6b = 1
                                       S(2) =S(- 2) =0 =＝斗                               4a+ b= 0,

giving a = -1 and b = { . The symmetric filter R(z) becomes


            !(:)＝士+ 士－'
                    =        (     1
                                       )   2
                                                [i
                                                          +V + (1      -   .J三)
                                                                                  z_
                                                                                        1]   [i   +V   +   (i   -
                                                                                                                    V亂］
                                                                                                                      ·




This expression is substituted into (7.102) so that we can factor S(z) into a product
of two filters, II (z) and Ho(ze1). The result of 山is spec仕띠 factorization gives a
causal filter:

                                       z_ 2                        +
 Ho         =                                              +
                                           1)
                _       __




                4/                                                     (1-
      (z)
                                                     [i
                                                               v
                             (1+
            =- 2L\
                f(i+ V引/ + (+
                           \
                              'J）
                                I
                                  尸+ 任
                                     \
                                       而z-뇨
                                        /
                                            (l-
                                            \
                                                J訊키
                                                 / I
                4/

            = 0.4929 + 0.8365z ' + 0.224l乙e2 - 0.1294之H3.

Note that these coefficients need to be multiplied by J                                            to get the values given in
Chapter 6.

Biorthoc刃naI Filter Bank A linear-Dhase FIR filter bank is desirable because it
mininuzes pnase ciistortion in signal processing. On the other hand, an orthogonal
FI之 filter bank is also desirable because of its simplicity. One has to design only one
filter, namely H (乙), and all other filters in the entire bank are specified. Biorthogonal
filter banks are designed to satisfy the linear-phase requirement.
    Let us recall the PR and antialiasing conditions with synthesis and analysis filters.
They are

                                           月0回G0（기 + H1回Gi(z) == 2之-m
                                           Go(之)Ho(- z) + Gi(z)Hi(- z) = 0.

We can solve for the synthesis filter's Go(z) and Gi(z) in terms o the analysis filter's
llo(z) and Hi (z). The result is

                                                1Gn(z1             2之Hm I              Hi (- 711
                                                                                                                      (7.103)
                                                LI-hiZ)J           detl'ir] LHhb0.HZ)i
                        i月O-CHANNEL PERFECT RECONSTRUCTION FILTER BANK              175

 where the tr크nsfer matrix is


                             [Tn]=［客勻 出二］·
If we allow symmetric filters

                        J-Io(z) = Ho(C1) 4 ho(n) = ho(- n)

and are not concerned with causality at the moment, we may safely ignore the delay
Zm. This is equivalent to designing all filters to be symmetric or antisymmetric
毗K沁t the or培in. We also recall the defi岫如ns of the co빠os如 filters

                                     Co(z) = Ho(z)Go(z)
                                     Ci(z) = Hi(z)Gi(z).

Using the result of (7.103), we write


                      的仙昞小 끼盜尸
                      Cl小Hi(z)Gi小巴喘(-z)·
If we replace -z for z in the second equation and note that

                             det[Tr(- z)] = - det[Tr(z)},

니／e have

                                      Ci(z) = Co(- z).

The final result is

                                     C (z) + C0(- z) = 2.

We now have a half-band filter for Co (z), from which we can use spectral factoriza-
tion to obtain Ho(z) and Go(z). There are many choices for spectral factorization and
the resulting filters are also correspondingly different. They may have different filter
lengths for the synthesis and analysis banks. The resulting filters have linear phase.
The user can make a judicious choice to design the analysis bank or the synthesis
bank to meet the requirements of the problem on hand. We use the example in [3] to
show different ways of spectral factonization to obtain Ho(z) and Go(z).
   Let the product filter

                  C (z) = H0(z)G0(z) = (1 + z小1)4Q(z)

                        =
                            = l + 9z 2 + 16z-3 + 9zH4 C6)
                                (-
                                                              -      .         (7.107)
176          DISCR日E WAVELET TRANSFORM AND FILTER BANK ALGORIT

Since the binomial (1 + ze1)' is symmetrical, Q(z) must be syn metrical to make
Co(z) symmetrical. An advance of z3 makes S(z) a half-band flit r. The choices of
spectral factorization include

     1.
          月0 (z) = (1 + Z小1)0                   G0 (z) = (1 + 尸）4           (z)
2.
          J70（乙） = (1 + 尸）l                     G0 (z) = (1 + zH1)3         (z)
3.
          Ho(z) = (1 +zH1)2                     Go (z) = (1 + 尸）2
           or (1 + 尸）(2 寸 \／三 叱_1)               or (1 + z寸1)3(2 +
4.
          Ho (z) = (1 + z ')3                   Go(z) =(l+ z ')(
5.        Ho(z) = (1 + rb2 (2 - N唇 H 尸）         Go (z) = (1+ z 1)2



The last choice corresponds to Daubechies' orthogonal filters, 叫hich. do not have
linear phase. The 3/5 filter in the upper line of factorization choiCF. gives a jinear-
phase filter, whereas the lower one does not.


7.8.2 lime-Domain Analysis
The development of filter bank theory is based primarily on spe tral analysis. We
discuss the time-domain equivalent of the theory for enhancement 1f the understand-
ing as well as for the digital implementation of the algorithm.『 hus it suffices to
illustrate the meaning of the terms, filter requirements, and filter s: stems in terms of
time-domain variables.

Causality An FIR filter is causal if the impulse response

                                 h(n) =0       Vn< 0.

The z-transform of h(n) is a right-sided polynomial of z小

                   H(z) := 九（0) + h(l)z니 + h(2）之小2 + · · · + 九（m)z   -m.
If H(乙) is a causal filter, H(ze') is anticausal since

                    H(z小 = h(0) + h(l)z + h(2沽 + · · · + h（川尹，

which is a left-sided polynomial of z. As a result, H(- 戶) is al 10 anticausal since
the polynomial is the same as that of H(ze1) except that the signs of odd coefficients
have been changed:

                   H(- C ') = h(0) 尸 /i(l）乙 + h(2)z2 中 · · · 1 力（m) Zm.

쯔！  ast term has a negative sign i如e assum帥帥 蜘．妃．％呻lize the anti啣“코
tiK niter, we must aeiay me niter Dy me iengtn 01 tHe niter to mi e it causal. rienec

           -Z尸mH（尸）= h(m) - h(m - 1）之-1 + . · · + 九（l)zH                   -h (0）乙H刃i
                         iWO-CHANNEL PERFECT RECONSTRUCTION FILTER BANK                   177

 is a causal filter. If we choose

                                          月0(z) == 月（z)
                                      H1（之） = 1乙em/70(1尸）
                                      Go(z) = Hi(- z)
                                      Gi (z) = -Ho(- z),

 we have a filter bank consisting of causal filters.

PR Requirements Perfect recons仕uction demands that

                                            S(z) + S(- z) = 2.

In terms of the lowpass filter 月0(Z), the equation becomes

                       月o(z)Ho(z小 + H0 (- z)Ho(- 戶）= 2.                               (7.109)

Let us consider the PR condition in (7.109). In the time domain we have

    S(z) + S(-z) =Z ho(n)zH" ＞二ho(m)zm
                        n                      7刃


                       + ＞二方0(n)ZH" ＞二（_1)_(n+rn）方o(m）尹

                   스그o(n)ho(毗 " 尹 + ＞二（_1y "+m）九o(n）力o(m）乙b" Zm
                   =2.                                                                (7.110)

Satisfaction of (7.110) requires that (m + n) be even and we have

                                  乞ho(n)ho伽）乙小" 尹＝1.                                  (7.111)
                                  n.m

The left side of (7. 111) is the z-transform of the autocorrelation function of the se-
quence ho(n). To show this relation, we denote

                        K   (n)
                                  =
                                          ＞二
                                           k
                                             ho(k)ho(k+       n)
                                                                   =
                                                                       ,c   (-
                                                                                 n)
                                                                                      (7.112)
as the autocorrelation function. Its z-transform is written as

                         尺（z) = ZZM帥Mk +n)z "
                                      =        ho (k)   Zho
                                                              (k +n)z            "


                                      스그油Z幻回戶rn-k)                                    (7.113)
178         DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS


which implies that

                                        ic(n) = ho(n) 木 h0（中n).                                               (7.114)

Comparing (7.113) and (7.110) and making the substitution

                                              尺（z) -p S(z)



we have

                               S(z) =＞二Z ho(k)ho(k +n)zH"
                                             n      k

From (7.98) and the that s(2n) = 0 for all integer n, we
                        fact                                                             have       t耳e orthonormality
conwtion required b0r i ' :

                                       ＞二ho(k）九0(k + 2n) ＝하：，小                                                (7.115)
                                        k

This implies the orthogonality of the filter on all its even translates. We apply the
same analysis to the highpass filter hi(n) and get the same condition for hi(n):

                                       Zhi (k)h1(k + 2n) = 匈,0                                                (7.116)
                                        k

                                       ＞二方0(t）九1(k+ 2n) =0.                                                   (7.117)
                                        k

 In
       terms 。f wavelet and    appr。
                                         ximati。
                                               n        functi。   n   basis,   the 。rth。
                                                                                       n。 ality c。
                                                                                                 nditi。
                                                                                                    ｝m
                                                                                                      ns
given above are expressed as inner products:

                                        (ho(k), ho(k + 2n)) = 8n,0
                                        伽（k), hi (k + 2n)) = 各n.0                                             (7.118)
                                        伽0(k), hi(k + 2n力 = 0,

where the approximation basis ho(k) and the wavelet basis hi(k) are orthonormal
to their even translates. They are also orthogonal to each other. If we construct an
infinite matrix [Ho] using the FIR sequence ho(n) such that



                                                                                00
                                                                                                  00
                   h0[0]       ho[l]        ho[2]       h0[3]     0                                      1
                                                                                   八
                                                                                   4
                                                                                   V l
                   0           0            ho[0]       ho[1]     ho[2]


                                                                               0hh00
                               0
                                                                                                         H
                                                                                                00九h000
                                            0           0         h0[0]                                  向
         [Ho] =                                         0         0                                      U
                                                                                                              (7.119)
                       T사O-CHANNEL PERFECT RECONSTRUCTION FILTER BANK              179

it is obvious that

                                   ［月ol［月01 = /                                (7.120)
using the orthonormality conditions in (7.118). Therefore, [H0] is an orthogonal ma-
trix. We define [H1] in a similar way using the FIR sequence of h1(n) and show
that

                                   [H1] [月1]i = 1.                              (7.121)

In addition, the reader can also show that

                           [H1] [Ho]r = [Ho] [H1lt = [0] .                      (7.122)

    Equations in (7.118) constitute the orthogonal conditions imposed on the FIR
filters. This type of filter bank is called an o月hogonal filter bank. The processing
sequences for the Haar scaling function and Haar wavelets are the simplest linear-
phase orthogonal filter bank. Indeed, if we denote

                                硝佃 =              三扼      三扼

and


                              畔（n)=｛士弓들｝
these two sequences satisfy the orthogonal conditions in (7.118). We recall that
linear-phase FIR filters must be either symmetric or antisymmetric, a condition not
usually satisfied by orthogonal filters. This set of Haar filters is the only orthogonal
set that has linear phase.

 Two-Channel Biorthogonal Filter Bank in the Time Domain We have shown
that the biorthogonal condition on the analysis and synthesis filters is

                 C0(z) + Co(- z) = Ho(z)G0(z) + Ho(- z)Go(- z)
                                   =   2.
Writing this equation in the time domain and using the convolution formula yields
the time-domain biorthogonal condition

          ＞二 ho(k)go(f小 k나 (_1)tZ ho(k)go(t - k) =28t,0·                        (7.123)
            k                               k
For nontrivial solution, the equality holds only ifZ is even. 때is results in a biorthog-
onal relation between the analysis and synthesis filters:

                     ＞二 ho(k)go(2n - k) = (ho(k), go(2n - k))
                      k
                                                = 8n.0.                         (7.124)
180      ［긔SCRETE WAVELET TRANSF(：기깁너 ANt) 디LTER BANK ALG아tITH人＼S

The biorthogonal condition can also be expressed in terms of H1(z 的 yield

                     Zm蜘伽 e 幻 = 伽1(k), gi(2n - k))
                      k
                                                    = 各n,O.                           (7.125)

The additional biorthogonal relations are

                              (hi(k), go(2n - k)) = 0,
                                                                                      (7.126)
                              伽o(k),g1(2n -k) ) = 0.

If we consider the filters as discrete bases, we have

                                  lm(k) = gm(- k).                                    (7.127)

The biorthogonal relations become

                             (ho(k), jo(k - 2n)) = Sn,0
                             (h1(k), 百1(k - 2n)) = 8n, 0
                                                                                      (7.128)
                             (h1(k), 츙t)(k 尸 2n)) = 0
                             伽0(k), 百i(k- 2n)) = 0.


7.9     POLYPIIASE REPRESENTATION FOR FITTER BANKS

Polyphase representation of a signal is an alternative approach to discrete signal rep-
resentation other than in the spectral and time domains. It is an efficient representa-
tion for computation. Consider the process of convolution and decimation by 2; we
compute all the resulting coefficients and then cast out half of them. In the polyphase
approach we decimate the input signal and then convolve with only half of the filter
coefficients. This approach increases the computational efficiency by reducing the
redundancy.


7.9.1    Signal Representation in the Potyphase Domain
Let the z-transform of a discrete causal   signal
                                                         separated into segIT1ents of M points
oe wnuen as

   X (z) = 工（0) + 工(1)尸 卄 （2)z寸2 ＋工（3）之U3 + · · ·＋工（凡1' 니 l) z_M+1

            卄（M)z_M卄（M+ 1)戶M+1) 卄(M+ 2)z크싸2)＋·．1
            + 工（2凡f)z小2M ＋工（2凡f + l)z_(2M+1) ＋工（2M + 2) -(2M+2) + . . .
            + x(3M)z_3M + x(3M + l) z_(3M+1) + · · ·                                  (7.129)


          = ＞二 ZHtXt（尹）,                                                              (7.130)
                                 POLYPHASE REPRESENTATION FOR FILTER BANKS                  181

where Xt (zM) is the z-仕ansform of x(n) decimated by M(.4 M). The index t mldi-
cates the number of sample shifts. For the case of M = 2, we have

                              X ( ) = Xo(z2) +zH'Xi (乙2).                                (7.131)


7.9.2   Filter Bank in the Polyphase Domain
For a filter H(z) in a two-channel setting, the polyphase representation is exactly the
same as in (7.131):

                              H(z) = He(Z2) + C1H。
                                                 (z2),                                   (7.132)

where He(z2) consists of the even s町lples of h(n) and H。   (z2) has all the odd sam-
ples. The odd and even parts of the filter are used to process the odd and even co-
efficients of the signal separately. To fonnulate the two-channel filter bank in the
polyphase domain, we need the help of two identities:

                         1.    (4. M) G(z) = G(zM) (4. M) .
                                                                                         (7.133)
                         2.    (t M) G(zM) =G(z) (t M) .

A filter G(z2) followed by a two-point decimator is equivalent to a two-point deci-
mator followed by G(z). The second identity is useful for the synthesis filter bank.
   Let us consider first the time-domain formulation of the lowpass branch of the
analysis filter. Assuming a causal input sequence and causal filter, the output y(n) =
[x(n) * f (n)]4,2 is expressed in matrix form as



                                                                           10 0
                                                                                                   =




                                                                 000
        y (o)         f (O) 0             0         0                             工（0)
        y (1)         f (1) f (0)         0         0                             工（1)
        y (2)         f (2) f (1)         f (0)     0            0         0      工（2)
                                                                                         (7.134)
        y (3)         f (3) f (2)         f (l)     1 (0)        0         0      工（3)
        y (4)         f (4) 1 (3)         1 (2)     f (1)        1 (0)     0      工（4)
        y (5)         f (S) f (4)         f (3)     f (2)        f (l)            工（5)
        y (6)                                                                     工（6)

The output coefficients 町e represented separately by the odd and even p缸ts as

                        [y(n)] = [Ye(fl)1 + (delay) [y。
                                                      (n)],

where

                                                            ry   (0)   m




                                                                                         (7.135)
                           [y(n刀J,   2=     ［兀伽小開
                                                            Ly   (6)   _
182     DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS

The even part of y(n) is made up of the pr에ucts of fe(fl) with Xe(fl) and f0(n) with
x,,(n') nius a delay. The si으nal x(n) is divided into the even and odd parts and they
a七 processea Dy tue even ana ouu parts or me flier, respectively. in mne same way,
the 址ghpass branch of the analysis section can be seen exactly as we demonstrate
above. In the polyphase domain, the intermediate output from the analysis filter is
given by


                   ［就i=r們z)z) I-Ii喘］［씌z)X1(z)
                       [5} IXo    )1
                                   ]                                          (7.136)
                                           (z)   ,(:
                       [H]
                              =
                                           1Xl
                              =
                                     Lz_
                                                       (z)
毗re［小 毗岫曲 蜘in啣蜘ase dom血. In th油毗 man呻, we
obtain the reconstructed sequence X' (z) from the synthesis filter bank as


                  X'(z)= [z 11]［旣玄 出읽］［昨：]
                       =[z_1i][.]［出身］·                                        (7.137)


The PR condition for the polyphase processing ma仕ices is [H] [GJ = I.


7.10    COMMENTS ON DWT AND PR FftTER BANKS

We have shown the parallel between the algorithms of the DWr and the,two-channel
niter oanic. in terms oi numencai.compuiauon, me aigornnms 아 DOLL! ulselpilnes
a七 exactiy tne same. we wouiu itce tO point out several iunuamen[ai unierences
between the two disciplines.

   1. Processing domain. Let us represent an analog signal f (t) n L2 by an or-
      thonormal wavelet series

                                  f(t) = ZZ功k,，奴，5(t).                        (7.138)


       The coefficients wk,s are computed via the inner product

                                   Wk,s = (f (t),仰，s(t)).                     (7.139)

       In much the same way as the Fourier series coefficients, the wavelet series co-
       efficients are time (or analog)-domain entities. From this point of view we see
       that the DWT is a fast algorithm to compute the CWT at a sparse set of points
       on the time-scale plane, much like the FF1' is a fast algorithm to compute the
       discrete Fourier transform. The DW1' is a time-domain tra工lsform for analog
       signal processing. on me otner nana, me flier DaflK aigonwms 町e aesignea
                                                                           EXERCISES      183
          from spectral domain considerations (i.e.,
                                                      highpass and lowpass design) for
          processing of signal "samples" (instead of coefficients).
       2. Processing goal. We have shown that the wavele
                                                              t series coefficients are essen-
           tially the components (from projection) of the
                                                             signal in the "direction" of the
           wavelet 少 at the scale a = 2HS and at the time point
                                                                  b = k2HS. This concept of
          component is similar to that of the Fourier compo
                                                                 nent. The magnitude of the
           wavelet series coefficient represents the strength of
                                                                 the correlation between the
          signal and the wavelet at that particular scale and
                                                               point in time. The processing
          goal of the filter bank is to separate the high- and
                                                                low-frequency components
          of the signal so that they may be processed or refined
                                                                     by different DSP algo-
          rithms. Although the DWT algorithms inherently have
                                                                      the same function, the
          focus of DWT is on finding the similarity between
                                                                  the signal and the wavelet
          at a given scale.
    3. Design origin. A wavelet is designed primarily via the
                                                                    two-scale relation to
        satisfy the MRA requirements. Once the two-scale sequen
                                                                        ces are found, the
       DWT processing sequences have been set. A wavelet can be
                                                                        constructed and its
       time and scale window widths can be computed. In genera
                                                                      l, a filter bank is de-
       signed in the spectral domain via spectral factorization
                                                                 to obtain the processing
       filters. These sequences may or may not serve as the
                                                               two-scale sequences for
       the approximation function and the wavelet. The time-sc
                                                                   ale or time-frequency
       characteristics of these filters may not be measurable.
   4. Application areas. Most signal and image processing
                                                                applications can be car-
      ned out with either DWT or filter bank algorithms. I心om
                                                                      e application areas,
       such as in non-Fourier magnetic resonance imaging,
                                                                  where the processing
      pulse required is in the analog domain, a wavelet is more suitable
                                                                                  for the job
      because the data set is obtained directly via project
                                                            ion.
   5. Flexibility. Since filter banks may be designed in the
                                                              spectral domain via spec-
      tral factorization, a given half-band filter may result in several
                                                                              sets of filters,
      each having its own merit vis- -vis the signal given. In
                                                                   this regard, the filter
      bank is much more adaptable than wavelets to the process
                                                                     ing need.


  Wavel毗 아 fi如r bank? Users mt始tdecide 凡r themselves based
                                                                   아i the pr야氾mat
hand and the efficiency and accuracy of using either one
                                                         or the other.




7.11     EXERCISES

1. For a nositive integer M > 2. set w冬., = exn( i2쭈) fork
          1             1/     He          iri       1   \V   i1了
                                                                    = 1. ....M. Show that



                                茫喘出 帑二．
                                    !c=1         \
                                                                                    (7.140)
184      ［기SCRETE WAVELET TRANSF아U너 AND 디LTER BANK ALG아리TH入IS


   Using this relation, prove that


                11

                       Y   (e    "
                                     "   ')
                                                                                                       (7.141)


   where X (z) = >kX[/]Zk and Y (z) = >二kY[ICIZk are the z- ansform of Se-
   quences fx[k]} and {y[k]}.
2. If the sequence (y[k]} is generated from {x[kj} by upsampling b M, that is,

                                               (]                             jfk E MZ
                                                                                                       (7.142)
                                                                              otherwise,
                                                     =
                                         ,[                     ［缶］
                                                         ｛승
   show that

                                          (v    (e
                                                         ' ')         =   x   (e_
                                                                                    JMC)   )           (7.143)

   的r the respect加ez七ansforms.

3. In the QMF solution to the PR condition, it is found that thi nly solution that
   can satisfy the condition is the use of Haar filters. Why can i other FI之 filters
   satisfy the PR condition?

4. Use the antialiasing condition and the PR condition, find t                                 filter sequences
   ho(n),hj (n),gi(n) if go(n) is the D2 sequence given the ex                                 ple discussed in
   this chapter.

5. Show the validity of the identities given in Section 7.9.2.



7.12     COMPUTER PROGRAMS

7.12.1    Algorithms
毛
% PROGRAM algorithm.m
毛
% Decomposes and reconstructs a function using Daubechies '
邕 wavele七 (m = 2 ) . The mnl上ial coefficien七s are 亡aken as
% the function values themselves.
毛

留 Signal

vl = 100;                       % frequency
v2 = 200;
v3 = 400;
r = 1000;                       %sai叩ling ra七e
                                                    COMPUTER PROGRAMS   185


 k 亡 S
         = 1: 100;
         = (k- i) / r;
         = sin (2如1女vl* 七） + sin (2出pi士＼/2士七） + sin (2士pi火＼T3女t) ;

 돔 Decomposi七1（끄i and recons七ruc七ion filters

 g0 = [0. 68301; 1. 18301; 0. 31699; -0. 18301] ;
 k = [0; 1; 2; 3] ;
gi = flipud (g0) . 出卜1) . 八k;
h0 = flipud (g0) / 2;
hi = flipud (gl) / 2;

% Decomposition process

% First        level   decomposition

x = conv (s, h0) ;
a0 = x (l: 2: length (x) ) ; %downsa四ling
x = conv (s, hl) ;
w0 = x (l: 2: length (x) ) ; %downsmapling

왕 Second level         decc汀uposi上如n

x = conv (a0,ho) ;
al = x (l: 2: length (xfl;
x = conv (ao,hl) ;
wl = x (l: 2: length (xfl;

묻； Plot

subplo亡 (3, 2, 1) , plo亡 佃）
ylabel ( 'Signal ' )
subplot (3, 2, 3) , plot (a0)
ylabel ( 'a_ 0 ' )
subplot (3, 2, 4) , plot (wo)
ylabel ( 'w_0 ')
subplot (3, 2, 5) , plot (al)
ylabel ( 'a_ {-l} ' )
subplot (3, 2, 6) , plot (wl)
ylabel ( '＼사H卜1} ' )
set (gcf, 'paperposition ' , [0. 5 0. 5 7. 5 10] )

宅 Recons七uc匕ion process

% Second level         reconstruction

x = zeros (2*length (al) ,l) ;
x (1: 2: 2*length (al) ) = al (l: iength (al) ) ;
y = zeros (2*length (wl) ,l) ;
y (l: 2: 2*length (wl) ) = wl (l: length (wl) ) ;
186                   DISCRETE WAVELET TRANSFORM AND FILTER BANK ALGORITHMS

x = conv (x, g0) + conv (y, gl) ;
a0_rec = 그＜(4: leng七I니川 -4) ;

毛 Firs七 level recons七ruc七iJ그n

y = zeros (2出leng七h（勺e0) , 1) ;
y (l: 2: 2*length (wo) ) = w0 (l: lerigth (w0) ) ;
x = zeros (2*length (a0_rec) , 1) ;
x (l: 2:2*length (a0_rec) ) = a0_rec;




X yy
  = conv (x, g0) ;
  = conv (y, gl) ;
  = x (l: length (y) )+y;
s_rec = y (4:length (y) -4) ;

돔 Plot

figure (2)
subplot (3, 2, l) , plot (al)
ylabel ( 'a_ (- l} ')
subplo七 ( 3, 2, 2) , plc＞七 佃1)
ylabel ( ' ＼사寸｛-l} ' )
subplot (3, 2, 3) , plot (a0_rec)
ylabel ( 'Reconstructed a_0 ')
subplot (3, 2, 4) , plot 佃0)
ylabel ( 'w_0 ')
subplot (3, 2, 5) , plc＞七 佃尸rec)
ylabel ( 'Reconstructed Signal ')
set (gcf, 'paperposition ' , [0. 5 0. 5 7. 5 10] )



REFERENCES

 1. C. K. Chui, J. C. Goswami, and A. K. Chan, "Fast integral wavelet transform on a dense
    set of time-scale domain:' Nu刃ier Math., 70, pp. 283-302, 1995.
 2. J. C. Goswami, A. K. Chan, and C. K. Chui, "On a spline-based 'ast integral wavelet
    transform algorithm:' in Ultra- Wideband Sh가t Pulse Electromagnetrcs 2, L. Carin and L.
    B. Felsen (Eds.). New York: Plenum Press, 1995, pp. 455나163.
 3. G. Strang and T. Nguyen, Wavelers and Filter Banks. Welleslei, Mass.: Wellesley-
    Cambridge Press, 1996.
 4. P. P. Vaidyanathan, Multirate Systems andFilter Banks. Upper Saddl4 River, N.J.: Prentice
    Hall, 1993.
 5. M. Vetterli and J. Kovacevic, Wavelets and Subband Coding. Upper Saddle River, N.J.:
    Prentice Hall, 1995.
 6.    A.    Akansu and R.
                 N.                         A.        n Signal Dec。
                                                         Haddad,
                                                                    m 。siti。 n.
                                                                       Multires。
                                                                                      Dieg。  ,
                                                                                             luti。
                                                                                                                                        San
    Calif.: Academic Press, 1992.                                     !
 7.    A.   N.         Akansu and M.   J.        Smith             (Eds.   ),      Subband           and Wavelet Transfprm.   Boston:         Kluwer
       Academic, 1995.
CHAPTER EIGHT




Fast Integral Transform
and Applications


In Chapter 7 we discussed standard wavelet decomposition and reconstruction algo-
rithms. By applying an optimal-order local spline interpolation scheme as described
in Section 5.6, we obtain the coefficient sequence aM of the desired B-spline series
representation. Then, depending on the choice of linear or cubic spline interpola-
tion, we apply the change-of-bases sequences (Section 7.5) to obtain the coefficient
sequence aM of the dual series representation for the pur兀se of FIR wavelet decom-
position.
    A typical time-scale grid obtained by following the implementation scheme de-
scnbed in Chapter 7 is shown in Figure 7.7. In other words, the integr出 wavelet
transform (I刃T) values of the given signal at the time-scale positions shown in Fig-
ure 7.7 can be obtained (in real time) by following this scheme. However, in many
signal analysis applications, such as wideband correlation processing [1] used in
some radar and sonar applications, this information on the 1WT of f on such a
sparse set of dyadic points (as shown in Figure 7.7) is insufficient for the desired
time-frequency analysis of the signal. It becomes necessary to compute the 1WT
at nondyadic points as well. By m沚lltaining the same time resolution at all the bi-
nary scales, the aliasing and the time variance difficulties associated with the stan-
dard wavelet decomposition algorithm can be circumvented. Furthermore, as will be
shown in this chapter, computation only at bin쾨y scales may not be appropriate to
separate all the frequency contents of a function.
    An algorithm for computing the IWT with finer time resolution has been intro-
duced and studied by Rioul and Duhamel [2] and Shensa [3]. In addition, there have
been some advances in fast computation of the IWT with finer frequency resolution,
such as the multivoice per octave (MVPO) scheme, 丘rst introduced in [4] (see also
[5, pp. 71-72]) and later improved with the help of下F by Rioul and Duhamel [2].
However, the computational complexity of the MVPO scheme, with or without FF1',
increases with the number of values of the scale parameter a. For example, in the

                                                                                 187
188       FAST INTEGRAL TRANSFORM AND APPLICATIONS

FFF-based computational scheme, both the signal and the analyzing wavelet have
 to be sampied at the same rate, with the sampling rate determined by the highest
 frequency content (or the smallest scale parameter) of the signal, and this sampling
rate cannot be changed at the subsequent larger scale values for any fixed signal dis-
cretization. Furthermore, even at the highest frequency level, where the width of the
wavelet is narrowest in the time domain, the number of sampled data required for the
wavelet will be significantly larger than the number of decompositit1n coefficients in
the pyra끄nid algorithm.
 - - In this chapter we. discuss.the fast integral wavelet transform (1WT) algorithm
Lt,-aj to compute me integral (conunuous) wavelet transtorm on a aPnse set or points
in the 山ne-記카e domain.



8.1    FINER I小任 RESOLUTION

In this section we a七 concerned with maintaining the same time resolution on
eacn scale nv nhim2 in tne noies' aion2 me time axis on eacn scale: mat is.
,1. m , . . n11+ 1,1 』1』1m4小. . 1m 1l7 1. /4= /41J
                                                "'
we want to compute W中工M(n/2",                      1/2'),
                                                   1 /n八
                                                          n  E 也, Sn <J M.
                                                          == 戶 -        --
                                                                           Keiall that the stan-
                                                                           -八小J1 111n1 11m八 n1nm


dard algorithms discussed in Chapter 7 give the IWT values only at dyadic points
 n/2s, 1/2s ; n E Z, s <M}. For finer time resolution, we first observe that for each
fixed n, by introducing the notation

                                                                                                                (8.1)
                                XM，小）                     :=   XM    (!     ＋翕）              ,




we have


              W,/IXM（翕，計2," /:XM(t)砂［2小극n1dt                                           1口        \   乙1'1 / J




                                        = 2s/'乙小줆小't)山
                                                                                                                (8.2)
                                                                      （나）
                                        ＝                        n
                                                吼XM,
Now, since


                             XM   (t)       =      Eak,         M4          (2Mt   -        k)   ,
                                                                                                                (8.3)


we have

                           工M.n(t) = ＞二ak,M4 (2也 +n - k)

                                        = ＞二 an4k,Ma(2Mt - k).                                                  (8.4)
                                                                                                                                             디卜寸ER T小4E RESOLUTION                        189

 Hence we observe from (8.2) that the IWT of工M at (n/2M, 1/2s) is the same as that
 of工M, at (0, 1/2s) In general, for every k E 兀, we even have


                    WXM,
                                        n
                                            (}
                                                  ,
                                                      -1
                                                            )       -




                                                                    -
                                                                              2s12
                                                                                          JI
                                                                                               I:
                                                                                                    -
                                                                                                         XM,
                                                                                                        。。
                                                                                                                   n
                                                                                                                       (t)
                                                                                                                                     少 (2st                -         k) dt


                                                                :2"'乙小由i/i (25t－幻dt
                                                                :
                                                                            2s/
                                                                                      2   /:XM               (t）
                                                                                                                                 砂   （2st-
                                                                                                                                                                ,－
                                                                                                                                                                           츨류） dt


                                                                ＝
                                                                             吼XM
                                                                                              二          "                       '           "   ,
                                                                                                                                                     }),
                                                                                                                                                                                         (8.5)


where s < M. Hence, for any fixed s and M with s < M, since every integer Z can
be expressed as k2M_s + n, where n = 0. . . . .2M나 - 1 and k e 끄, we obtain all
the IWT values.



                                                 吼／M（多斗：2-"'Wt2SM,S                                                                                                                      (8.6)


of 工M at (f/ 2M , 1/2s), t E 끄 and s < M, by applying the standard wavelet
decomposition algorithm of Chapter 7 to the function XM,n. The time-scale grid for
s= M- l, M- 2, andM- 3, butonly t= 0. ... .3, isgiveninFigure8.l.

                                                  ]                                                                              I                     1              I

                20 H                女** 1 = 0                                                                                    AA1 1 = 2                                          叫
                                                 1= 1                                                                            1..             1= 3
                           1
                15

            은
        n
                10
                           1




                5
                           1느 1   5 s                      出 a s        .                                出 a s               .                                 士 a .       .




                                                 0.2                                 0.4                               0.6                                           0.8            10
                                           b
FIGURE 8.1 Filling in "holes" 띠ong the time axis. (Reprinted with permission from [6],
copyright 匣） 1995 by Springer-Verlag.)
190      FAST INTEGRAL TRANSFO帥4 AND APPLICATIONS

  For implementation, we need the notations

                吼 = {mk2」1i,,}tEZ                                                and 瓦＝{ak万M,s}kE冗                            (8.7)

and the notation for the upsamplmg operations

                                           I identity operator                                      for p = 0
                              싸 I-       -          ,                    =   r   1                             1              (8.8)
                              V          1 k까    'a                                                 幻rp 三 1,

꿔here

                   (r{
                   .{1n}    Xn}      =       {yn)
                                             {yn}            with
                                                             Wimy0                   니
                                                                                     _   j。   Xn/   '          for
                                                                                                               f。。  ddn.
                                                                                                                   even n
                                                                                                                              (8.9)

   As a consequence of (8.2) and (7.45), we have, for s = M - 1,

                           (11 *ai)fl := ＞二 . 1[k] n_k,M
                                                                         k

                                                         = ＞二g1[-k1a?;k
                                                                         k


                                                         =           2   (M_ l)I2W,xM,n                 (o赤）
                                                         = an/2,M_1.                                                         (8.10)

In a similar way it can be shown that

                                                        an/2,M_1 = (io *aM)fl.                                               (8.11)

That is, in tenns of the notations in (8.7) and (8.8), we have

                                                        aM_i = 佃010) 水 aM
                                                                                                                             (8.12)
                                                        切M-i = 佃oil) 水 aM.

   To extend this to other lower levels, we rely on the method given in [3], yielding
the algorithm

      瓦l = ((yM_Sj0) 木 a5
                                                                         withs= M, M- 1. ... .M- M'+ l.                      (8.13)
      面s-i = (47M_511) 串 切5 ,
A schem硝c dia얍amf야 it叩le毗nti昭 this algorithm is shown in Figure 8.2.


8.2     FINER SCALE RESOLUTION

For the purpose of computing the IWT at certain interoctave scales, we define an
interoctave parameter:
                                             2N
                                                                                 N >0           and n = l , . . . , 2N -1,   (8.14)
           口” = a兀N := n + 2                             "   '
                                                       FINER SCALE RESOLUTION          191



  aM                    口M                                                                    r

       =＝口    r                    g0
                                           aM_ i                          aM_M' g。




                        g1                             OAJH凡r' gl




                       I
                      凹M니                              凹M-M'
FIGURE 8.2 Wavelet decomposition process with 仕ner time resolution. (Reprinted with
permission from [6], copynght （흐）1995 by Springer-Verlag.)


which gives 2's' 小 1 additional levels between any two consecutive octave levels, as
follows.
    For each k E 兀, s < M, to add 2N - 1 levels between the (s - l)st and sth
octaves, we introduce the notations

                         叱小）= (2' 따）1/2中（2'ant 小 k)
                                                                                     (8.15)
                         町．小斥 (2' 따刈2少O' 咐 中 幻．
Observe that since 1/2 <a,1 < 1, we have


                      {：然，커客叫；-1                                                     (8.16)


As a consequence of (8.16), the RMS bandwidths of中弓1,0 and 砂g,0 are narrower than
those of中 and 砂 and wider than those of 中(2.) and 少 (2.), respectively.
   The interoctave scales are described by the subspaces

                             v: = closL2 (中｛,5 : k E 兀).                             (8.17)

It is clear that for each n, these subspaces also constitute an MRA of L2. In fact, the
two-scale relation remains the same as that of the original scaling function 色 with
the two-scale sequence {go[k]}, namely


                        吼（!)=＞二的［k｝中旬（2t．흐，）·
                                                            1
                                                                                     (8.18)
                                                            k
                                    K              \            口 =   /




It is also easy to see that 砂乞 is orthogonal to V. Indeed,

                    （中孔 砂乙） = （中t.s, 砂k,s> = 0,           t ,kE 兀                    (8.19)
 192      FAST INTEGRAL TRANSFORM AND APPLICATIONS

 for any s E 兀. Hence the spaces

                               H／了＝面切他n :k e 兀）                                           (8.20)

 a氾 the orthogonal complementary subspaces of the MRA spaces V,n. In addition,
 analogous to (8.18), the two-scale relation of砂긍，: and中二"1 remains the same as that
 of 少 and 中，namely


                          姑" (t) 仁蛔
                                  IC
                                                              (刀즈，
                                                                 ）·                      (8.21)


Since ({go[k]}, {gi [kj)) remain unchanged for any interoctave scale, we can use the
same implementation scheme, as shown in Figure 7.11, to compute the 1WT values
at (k/2S an, 1/2뇨力. However, there are still two problems. First, we need to map
xM to VM,.; and second, we need to compute the IWT values at (k/2Man, 1/2'a)
instead of the coarser grid (k/2san, 1/2san).
   Let us first consider the second problem. That is, suppose that x긋r C V} has
already been determined. Then we may write

              珤 = Z枷中（2Mant - 幻 = Z枷m少叩 a)                                               (8.22)
                      k                                       k


for some sequences {ai,M} and {叩,M} E t 2. Then the decomposition algorithm as
described by Figure 7.11 yields

                      切｛,: = (25an)m（珤，少二" )

                           =
                               2sanf:
                                                  x
                                                      (t)
                                                            fr (2scxnt       -
                                                                                 k) dt

                               (2
                                                            fk
                           :
                                        '岫
                                             "'   吼XM             ,
                                                                      +,）·
                                                                                         (8.23)

Now by following the algorithm in (8.13), we can also maintain the same time reso-
lution along the time axis on each interoctave scale for any fixed n. More precisely,
by introducing the notations


                可니吼：也：IJ,,
                        k7LZ and 可니吼，也，},, 兀，                                            (8.24)

we have an algorithm for computing the IWT at the interoctave scale levels:

       a二l = 0r4im' 寸0) 水 a
                                             withs= M, M- l. . . . .M- M'+ 1. (8.25)
       u,?-1= 佃兀fH' gl) 木 a: ,
However, it is clear from (8.23) that the time resolution for each fixed n is l/ 2Man,
which is less than the one for the original octave scales, in which case the time
resolution is 112M. As discussed in Chapter 7, the highest attainable time resolution
                                                                     FINER SCALE RESOLUTION                           193



 a4r                                                                                                     a丸r凡r' gDH
                                                                                                                  aM_Me
              a力r- a                     r                 g0




                                                 g1                           （丁A／小M'E




                                                                                      叫卜M
                                                                                            1        '


FIGURE 8.3 Wavelet decomposition process with finer time-scale resolution. (Reprinted
with permission from [6], copyright （르）1995 by Springer-Verlag.)



in the case of the standard (pyramid) decomposition algorithm is 112M-1 . It should
be pointed out that the position along the time axis on the interoctave scales is not
the same as the original octave levels (i.e., we do not get a rectangular time-scale
grid) (see Figure 8.4). The schematic diagram of (8.25) is shown in Figure 8.3. If we
begin the index n of (8.14) from 0, then n == 0 corresponds to the original octave
level. Figure 8.4 represents a typical time-scale grid for s = M - 1, M - 2, and
M- 3withN= 2andn= 0. .. . .3.




              20 -
                                tttOctave scales       ,.. Inter- octave scales


              15-

        （그
       \\\\


       尸      10-



               5.           1                          .        S    S    S       S         1        S    S   S   S

                    .

                    t   . 1 1.S 1.
                        S        S
                                   1.
                                   1
                                      1
                                      1 S
                                         5 S $ S .S 11
                                                     S S S  S S 1 S S S S S S  S S 1 =
                                                       11 S 1S S I . 11 11 S 1S ' $.
                                     I            I                  I                           1
               0。                            1             1                  1



                                   0.2           0.4                0.6                         0.8               10

                                                           b
FIGURE 8.4 Time-scale grid using the scheme described in Figure 8.3. (Reprinted with
permission from [61, copyright （르）1995 by Springer-Verlag.)
194     FAST INTEGRAL TRANSFORM AND APPLICATIONS

8.3   FUNCTION MAPPING INTO THE INTEROCTAVE
      APPROXIMATION SUBSPACES

Now going back to the first problem of mapping 工M to 긋r, we （中bserve that since
VM ；三 1/．磊， we cannot expect to. have 4 = XM in gener毗 Ho씨ever, if the 八EA
spaces { V5 J contain locally aul me polynomials UP 10 oraer m m me sense mat ior
eacht, 0< t< m- l,

                                   ）二口t ,k中（t -k)                           (8.26)
                                     k

pointwise for some sequence {at,k}kE兀, it is clear that {V '} possesses the same
property. Consequently, the vanishing moment properties of the interoctave scale
wavelets 砂금，了 are the same as those of the original 少. Hence, in cons仕ucting the
mapping of 工M to 4, we must ensure that this 仕ansformation preserves all poly-
nomials up to order m. For the case of linear splines, such mapping can easily be
obtained based on the fact that the coe丘cients in the linear sp如e representation of
a func如n are the function values evaluated at appropriate locations.
   From the points of symme仕y of N2(2Mt) and N2(2Mart), we obtain the ma얹li-
tude of the shift 亨 in the centers (see Figure 8.5):


                           느놔！
                             , 1)＋뇨，                                        (8.27)


and therefore (t금.M as

                         哨，1i= (1- 2M)口o,M + 2M4aI,M.                       (8.28)




          0

                                   H
                                   r
                                                  긁T
FIGURE 8.5 Mapping {ak,M} to {a{,M}. (Reprinted with permission from [6], copyright
匣）1995 by Springer-Verlag.)
     FUNCTION MAPPING INTO THE INTEROCTAVE APPROXIMATION SUBSPACES                   195




         4.0 4.0625            4.25                  4.5                    4.75
FIGURE 8.6 First term of {a工，M} when {ak,Ml starts with k 尹 0. (Reprinted with permis-
sion from [6J, copyright @ 1995 by Springer-Verlag.)


However, if the lowest index of aM is other than zero, alr will not start with the same
index as that of aM. To illustrate this situation, suppose that x(t) has been discretized
beginning with t = 4.25 with 0.25 as the step size (mapping into V2). Then we have


              X2(t) = k ak,2N2(22t - k) =5k a,.2N2孚긔,                              (8.29)
                                                 ' V /
withn = l, N = 2a, = .AsisclearfromFigure8.6, theindexfora d呻notstart
with the same index as a2. It should also be observed that some of the coefficients
n{,2will coincide with ct,2. The next index, c工＋1,2, will then lie between ct+1,2 and
Ct+2,2.
   Taking all of the points above into account, we can obtain a二i from aM by fol-
lowing these steps:

   1. Based on the given discretized function data, determine the starting index of
      毗PLet it 比 可，M ·
   2. Let a7M lie between a1,M and as+1,M.
   3. Let a7M be shifted from aS,M toward the right by 亨 in time. Then starting with
      r = 0, compute

                        可，4i =(1口央厄卄，M+ 2싸口阡1+r.M.                                 (8.30)

   4. Increment i, s by 1 and 亨 by fl/2M+N.
   5. Repeat steps 3 and 4 until 1 - 2M <0. When 1 卞 2M <0, increment r by
      1 and reset 亨 to fl/2M+N. Increment i, s by 1.
   6. Repeat steps 3 to 5 until as+1+r,M t칸es the last index of aM.

   For a general case, the mapping of工M to 4 can be obtained following the method
described in Sections 5.6 and 7.2. For instance, to apply the linear spline interpola-
tory algorithm or the cubic spline interpolato口 algorithm, we need to compute the
 196       FAST 八TEGRAL TRANSF아之M AND APPLICA기ONS

 function values of兀M (k/2Man) orxa/ (k/2M_lan) , k c 兀. These values can eas-
 ily be determined by using any spline evaluation scheme. More precisely, we have
 the following:

      1. For m = 2 (linear splines), it is clear that


           珤(t) = 二口加N2（少啣 나）                                            with 畔，M = 工M             (
                                                                                                         J)
                                                                                                              .    (8.31)
                       k
    2. For m = 4 (cubic splines), we have

                                           珤(t) 4그加N4(깬叩 - k)                                                      (8.32)


 with



                            .加＝,琴,「硏2_2nXM(：人, ),                                                                 (8.33)

where the weight sequence {vn } is given in Section 5.6. Finally, to obtain the input
coefficient sequence { ,M} from {a工,M} for the interoctave scale algorithm (8.19),
we use the same change-of-bases sequence r as in (7.47).


8.4     EXA人시기．.ES

In this section we present a few examples to illustrate the FIWT algorithm dis-
cussed in this chapter. The graphs shown are the centered integral wavelet transform
(CIWT), defined with respect to the spline wavelet 吻n as


                           (b,                                                                                    (8.34)
                 Wmf
                                 a)
                                      :=
                                            a_
                                                 112f00 f(t)*m               (=
                                                                                  ,a   +t   ')
                                                                                                 ) dt,
where
                                                 !'              :   l
                                                                                                                  (8.35)
                                                      H   2m-
                                                                         .




Observe that the 1WT as defined by (4.32) does not indicate the location of the dis-
continuity of a function properly, since the spline wavelets are not symmetrical with
respect to the o增n. The CiWl' circumvents this problem by shifting the location of
the 1WT in the time ax怡 tow町（I the right by 口少．
   The integral wavelet transform of a function gives local time-scale information. To
get the time-frequency information we need to map the scale parameter to frequency.
There is no general way of doing so. However, as a first approximation, we may
consider the following mapping:
                                                                     C
                                                 a F-           f := -,                                           (8.36)
                                                                     口
                                                                       EXA人作LES      197

where c > 0 is a calibration constant. In this book the constant c has been de-
termined based on the one-sided center (口4) and one-sided radius (스寸+) of the
wavelet 少(w), which 게re defined in Chapter 4.
   For the cubic spline wavelet we get a4 = 5.164 and 삭f = 0.931. The cor-
responding figures for the linear spline wavelet are 5.332 and 2.360, respectively.
Based on these parameters, we choose values of c as 1.1 for cubic spline and 1.5
for linear spline cases. It is important to point out that these values of c may not be
suitable for all cases. Further research in 巾is direction is required. We have chosen
c by taking the lower cutoff frequency of 少(w).


8.4.1   IWT of a Linear Fundion
To compare the results obtained by the method presented in this chapter with the
results obtained by evaluating the integral of (8.34), we first take the linear function
which changes slope as shown in Figure 8.7. The function is sampled with 0.25 as the
step size. So for linear splines, it means that the function is mapped into V2, whereas
for cubic splines the function is mapped into V3. We choose N = 1, which gives one
additional scale between two consecu小／e octaves. It is clear from Figures 8.8 and
8.9 that the FIWT algorithm and direct integration give identical results for wavelet
coefficients for octave levels, but there are errors in the results for interoctave levels
as discussed before.




                  0         10        20         30        40         50
                                            t
FIGURE 8.7 Linear function whose WT is shown in Figures 8.8 to 8.10. (Reprinted with
permission from [8], copyright （트）1995 by IEEE.)
198        FAST INTEGRAL TRANSFORM AND APPLICATIONS



        0.10                                                                    - 0.10


                        Linear Spline                  ［거rect lntegroti그n


          0.05 -        a =   0.50                     F기나   Algorithm          - 0.05




                                                                            1       -
                                                                                        0




      -0. 05                                                                    - -0. 05




                                                                                =




                                                                                            0   0
      -0. 10
                                                                                1印
                                                         1                      中




                    。              10    20       30         40

                                              b




          0.1   !       Linear' Spline


                        a =         75   A
                                         .              Direct lntegrc吐k가）


                                                        F1WT Algorith
                                                                                        0.1




          imI
                              0.
                i
            0                                                                   1
      읓


      -0. 1                                                                             -0. 1




      -0. 2                                                                             -0. 2
                    0                    20                   40

                                              b
FIGURE 8.8 IWT of the function shown in Figure 8.7 using the linear spline wavelet for a =
0.50 and a = 0.75. Direct integration is performed with f2(t). (Reprinted with permission
from [81, copyright 匣） 1995 by IEEE.)
                                                                       EXAMPLES       199




        0.02                                           -                  -0. 02
                       Cubic Spline                    Direct Integration

                       a =    0.50                     f기WT 시gorithm




      -0. 02                                                               - -0. 02


                                                             1
               0                       20                   40
                                            b




                                                      11                 - 0.04
                        Cubic Spline                  Direct Integration

                        a =    0.75                   F기汭rr 씨gorithm
                                                                          - 0.02

                   1


                                                                             1




                                                                          - -0. 02




                                                                          - ..0. 04
                                        1                   1
                   0                   20                  4（그
                                            b
FIGURE 8.9 IWT of the function shown in Figure 8.7 using the cubic spline wavelet for a =
0.50 and a = 0.75. Direct integration is performed with 力(t). (Reprinted with permission
from [81, copyright （르） 1995 by IEEE.)
200     FAST INTEGRAL TRANSFORM AND APPLICATIONS

   The importance of the moment property becomes clear from Fi ires 8.8 and 8.9.
In both the linear and cubic cases, when the wavelet is completely side the smooth
region of the 凡nction, the wavelet coefficients (WC) are close to zc )since the func-
tion is linear. Wherever the function changes the slope, the wavelel oefficients have
larger magnitudes. We also observe the edge effects near t = 0 and = 50. The edge
effects can be avoided by using special wavelets near the boundariei. Such boundary
wavelets are discussed in Chapter 10. If we use the IWT instead of the C1WT, the
entire plot will be shifted toward the left, and the shift will continue to become larger
匈r lower levels. For Fi맘且es 8.8 and 的，direct eva岫如nof (8.34) is 面ne with 力(t)
and f3(t), respectively. In Figure 8.10, direct integration is done with f3,1(t), which
indicates that for interoctave levels also, the FIWT algorithm gives results identical
to those obtained with the corresponding approximation function.
   For Figure 8.9, 440 wavelet coefficients have been computed. Direct integration
takes about 300 times the CPU time of the FIWT algorithm. We wish to empha-
size that the ratio of 300:1 is minimal, since with the increase in scale parameter a,
the complexity of the direct integration method increases exponentially, while for
the F1WT it remains almost constant. Furthermore, in the FFT-based algorithm, the
complexity increases with a.




                                                         Direct Integration




                                            b
FIGURE 8.10 IWT of the function shown in Figure 8.7 using cubic spline wavelet for
a = 0.75. Direct integration is performed with f , i (t), the approximation of the function
of Figure 8.7 at s = 3, n = N = 1. (Reprinted with permission from [8] copyright （르）1995
by IEEE.)
                                                                                 EXAMPLES       201




           0.05




      畏，
     -0. 05



                         1       1       I                   I              I

                  0     0.2            0.4                  0.6            0.8      10
                                                      t


     5x 1 o 7                                                                        5x 1 0H7

                       a =    1/ 128              ;       Linear Spline




                                               $Cub          ;c   Spline
               0         I               I                                           0
           읓




    -5x1 0d                                                                          -5x10H7



                   0    0.2            （그. 4                0.6            0.8

                                               b
FIGURE 8.11 Function given by (8.37) and its IWT using linear and cubic spline wavelets
for a = 1/ 128. (Reprinted with permission from [8], copy叩ht @ 1995 by IEEE.)
202     FAST INTEGRAL TRANSFORM AND APPLICATIONS

8.4.2   Crack Detection
As a further example to highlight the importance of the IWT in identifying the change
in function behavior, we consider the following function. For y := 2t - 1         '


                 f(t)   :=   {   -   命y     (4y2 + 16y + 13) ,               t E [0, 2] 1/                 (8.37)
                             [ 姑y(y - l)(y -2) ,                             t e (1/2, 11 .


Figure 8.11 shows the function and its wavelet coefficients for linear and cubic spline
cases. The edge effect has not been shown. Once again, here we observe that for the
cubic spline case, the wavelet coefficients are close to zero in the smooth region of
the function; however, for the linear spline case, the wavelet coefficients are nonzero
in this region since the function is of degree t뇨ee in both intervals. This example
shows that even a physically unnoticeable discontinuity can be detected using the
wavelet transform.




                                                               15




                                                                       7
                                                      C> 10
                                                      m
                                                                   5

                                                                            J ＼누    1                1
                     UH11                         1                0
                     0.01            0.02      0.03                    0   1000    2000      3000   4000

                                                                   2
                                                                   0
                                                       色
                                                       寸
                                                       ＝
                                                                   2




                                                                   2

                                                                   0
                                                           色
                                                           그
                                                           L
                                                                   2




                                                                   2



                                                      뭉            0

                                                               -   2


FIGURE 8.12 Decomposition of a signal composed of three sinusoids with different fre-
quencies corresponding to nonoctave scales using the standard algorithm of Chapter 6.
(Reprinted with permission from [7], copyright （르）1995 by Plenum Press.)
                                                                        EXAMPLES   203



                                                      2



                                                 訃
           八
           乳
           尸
           m
                                    I      I
                        0
                                                 -2
                            0.01   0.02   0.03            0   0.01   0.02   0.03




                                                 e
                                                 ?




        辜

                    2


        읗0
               -2
FIGURE 8.13 Decomposition of a signal with three frequency components (continued from
Figure 8.12). (Repnnted with permission from [7], copyright9 1995 by Plenum Press.)



8.4.3   Decomposition of Signals with Nonoctave Frequency Components
To further emphasize the importance of the F1砥／T algorithm, we consider a compos-
ite function similar to that used in Chapter 7, but with slightly different frequencies
that do not correspond to octave scales. Figures 8.12 and 8.13 indicate the inability
of the standard decomposition algorithm of Chapter 7 to separate those frequencies
that do not correspond to octave scale. Figures 8.14 and 8.15 show, on the other hand,
that by properly selecting the values of n and N, we can separate any frequency band
that we desire.


8.4.4   Perturbed Sinusoidal Signal
Figure 8.16 gives the time-frequency representation of a function that is composed
of two sinusoids and two delta functions, represented as sharp changes in some data
values. Observe that two sinusoids appear as two bands parallel to the time axis,
whereas the delta functions are indicated by two vertical bands parallel to the fre-
 204     FAST INTEGRAL TRANSFORM AND APPLIC기ONS


                         2                                 15




         읗0                                       <:
                                                  Co
                                                           10




                    -2
                             너 'N 'N ' 싸' 쌔 ' 싸' '
                                                싸． 批니匕       1
                             0   0.01     0.02  0.03 0 1000 2000 3000 4000
                         卜 A A A I I I I      A            2
              色
              ＝了                                   ; 0              1   +

                                                       -
                                                           2    -




                         2                                 2

          云 0                                     ;; 0
         Co


               -2
                                                       -
                                                           2

                         2

          됴 0
         00


              -2
FIGURE 8.14 Decomposition of a si酊1al composed of 由ree sinusoids ith different fre-
quencies corresponding to nonoctave scales using the FIWT algorithm with = 1 and N =2.
(Reprinted with permission from [7], copyright (9 1995 by Plenum Press.)


quency axis. As discussed in Chapter 4, the frequency spread is due to the finite
window width of the wavelets.


8.4.5   Chirp Signal
Figures 8.17 and 8.18 show the CIWT of a chi叩 signal with respect to linear and
cubic spline wavelets, respectively. In Figure 8.19 we have shown the CIWT of a
chirped signal by applying the standard wavelet decomposition algorithm. Here the
interoctave scales have been filled with values at the orevious octave scales. Simi-
larly, on the time axis, 'holes" are tilled with values from previous lcations.


8.4.6   Music Signal with Noise
In Figure 8.20 we show the CIWT of a portion of a music signal with additive noise
using the cubic spline wavelet as the analyzing wavelet. Here the music data have
been assumed to be at the integer points.
                                                                   EXAMPLES      205




                                                   2
                                                   占
                                              -2
                    0.01     0.02    0.03               0.01    0.02     0.03




                                             긍 0




              2


         금 0

          -   2

FIGURE 8.15 Decomposition of a signal with three frequency components (continued from
Figure 8.14). (Reprinted with permission from [7], copyright （르）1995 by Plenum Press.)


8.4.7   Dispersive Nature of the Waveguide Mode

As a final example, we find the wavelet transform of experimental data obtained for
the transmission coefficient of an X-band rectangular waveguide. The waveguide is
excited by a coaxial-line probe inserted through the center of the broad side of the
waveguide. The scattering parameter S21, of the waveguide is measured using an
HP-85 10 network analyzer by sweeping the input frequency from 2 to 17 GHz. The
time-domain waveform is obtained by inverse Fourier-transforming the frequency-
domain data. The time response (up to a constant multiplier) and the magnitude (in
dB) of the frequency response are shown in Figure 8.21. It should be pointed out
here that several low-amplitude impulses appeared in the negative time axis, but they
have not been taken into account while performing the wavelet decomposition since
they represent some unwanted signals and can be removed from the plot by proper
thresholding. Furthermore, such an omission will not have any significant effect on
the WC plot of Figure 8.21 because of the local nature of wavelet analysis.
   The cutoff frequency and dispersive nature of the dominant TE10 is well observed
from its time-frequency plot. Because of the guide dimension and excitation, the
206      FAST INTEGRAL TRANSFORM AND APPLIC기ONS


                       000寸




                      000m




          N工口



                      000N



          >UCm그口m느노




                      000n




                                                               기me （引

   FIGURE 8.16                    CIWT of a composite signal with some perturbed data (cubic spline).



                                                                                II '料텍’甘！
                                                                                        }


           0
           씨


          小
          N工
           나 뇨은gg上

                尸
                0




                              n
                              d   山 이0   d                                                       （그
                                         尸




                                                                                             0.5
                                                                                             0
                                                                                             -0. 5
                                                                                             -1 0
                                             0      1           2           3            4

                                                             기me （引
FIGURE 8.17 CIWT of a chirp signal (linear spline). (Reprinted with permission from [61,
copyright (9 1995 by Springer-Verlag.)
                                                                                     EXAMPLES       207




           公工나 녹UCm그口m上
                          0
                          N




                          으
                                                                       it'
                               n
                               d   이0                                                        1.0
                                                                                             0.5
                                                                                             0
                                                                                             -0.5
                                                                                             -1.0
                                                    1           2                        4

                                                             Time （引
FIGURE 8.18 CIWT of a chirp signal (cubic spline). (Reprinted with permission from [6],
copyright (9 1995 by Springer-Verlag.)




          小
          N工
           나 aCm弓m上
                          0씨




                          D




                                        0           ]           2

                                                             Time （司

FIGURE 8.19                    CI刃T of a chirp signal using stand町d wavelet decomposition algorithm (cu-
bic spline).
208      FAST INTEGRAL TRANSFORM AND APPLICATIONS




                           이0




           八N工나 뇨UCm그口m上
                           =0




                                                                        기me （司
FIGURE 8.20 CIWT of a music signal with additive noise (cubic spline). (Reprinted with
permission from [6], copyright （르）1995 by Springer-Verlag.)




           合工口니 勺口mng立
                           0H




                                口
                                    0N1   0寸1   0山1
                                                      0m

                                                                                             0.2



                                                                                             -0.2
                                                           0   5            10          15

                                                                   Time (Nanoseconds)

FIGURE 8.21 CIWT of the experimental data for the transmission coefficient of an X-band
rectangular waveguide (cubic spline). (Reprinted with permission from [8] copyright (9 1995
by IEEE.)
                                                                      REFERENCES       209

next-higher-order degenerate modes 町e TE11 and TM11 with the cutoff frequency
16.156 GHz. This does not appear on the plot. The plot in小cates some transmission
taking place below the lower-frequency operation. There is a short pulse at t = 0
which contains all the frequency components and is almost nondispersive. These
can be attributed to system noise. No further attempt has been made to isolate the
effects of various transitions used in the experiment. The thresholding for Figure 8.21
has been done with respect to the relative magnitude (in dB) of the local maximum
of each frequency and the global maximum. Finally, the magnitude of the wavelet
coefficients has been mapped to 8-bit gray-sc毗 levels. Readers are referred to [9,101
for more applications of continuous wavelet 仕ansform to electromagnetic scattering
data.



REFERENCES

 1. L. G. Weiss, "Wavelets and wideband correlation processing," IEEE Signal Process.
    Magazine, pp. 13小32, January 1994.
 2. O. Rioul and P. Duhamel, "Fast algorithms for discrete and continuous wavelet trans-
    forms," lEE万 Tr口n工 ／可切刃i. T方e（가y, 38, pp. 56外586, March 1992.
 3. M. J. Shensa, "The discrete wavelet 甘ansform: Wedding the A trous and Mallat algo-
    rithms," IEEE Trans. Signal Process., 40, pp. 2464叫2482, October 1992.
 4. A. Grossmann, R. Kronland-Martinet, and J. Morlet, "Reading and understanding contin-
    uous wavelet transform," in Wavelet了， I加e戶re甲ency 兀let加d노 and Phase 枷口Ce, J. N.
    M. Combes, A. Grossmann, and Ph. Tchamitchian (Eds.), Berlin: Springer-Verlag, 1989,
    pp. 2-20.
 5. I. Daubechies, Ten Lectures on Wavelets. CBMS-NSF Ser. Appl. Math. 61. Philadelphia:
    SIAM, 1992.
 6. C. K. Chui, J. C. Goswami, and A. K. Chan, "Fast integral wavelet transform on a dense
    set of time-scale domain," Numer Math., 70, pp. 283-302, 1995.
 7. J. C. Goswami, A. K. Chan, and C. K. Chui, "On a spline-based fast integral wavelet
    transform algorithm," in Ultra-Wideband Short Pulse Electromagnetics 2, H. L. Bertoni,
    L. Carin, L. B. Felsen, and S. U. Pillai (Eds.). New York: Plenum Press, 1995, pp. 455-
    463.
 8. J. C. Goswami, A. K. Chan, and C. K. Chui, "An application of fast integral wavelet
    transform to waveguide mode identification:' IEEE Trans. Microwave Theory Tech., 43,
    pp. 655-663, March 1995.
 9. H. Kim and H. Ling, "Wavelet analysis of radar echo from finite-size target," IEEE An-
    tenn口s Pr口／）口g. M口g口zine, 41, pp. 200나207, Febuary 1993.
10. L. Carin and L. B. Felsen, "Wave-oriented data processing for frequency- and time-
    domain scattering by nonuniform truncated arrays:' lEE万 가an且 An妃nnas 竹叩唱 M口g.
    口之加e, pp. 29-43, June 1994.
CHAPTER NINE




D땅tal 이gnal I가ocessing
Applications



The introduction of wavelets to signal and image processing has pi vided a very flex-
ible tool for engineers to use to create innovative techniques for E lying various en-
gineering problems. A survey of recent literature on wavelet signa processing shows
the focus on using the wavelet algorithms for processing one-dim asional (l-D) and
two-dimensional (2-D) signals. Acoustic, speech, music, and elec ical transient sig-
nals are popular in l-D wavelet signal processing. The 2-D wavele signal processing
involves mainly image compression and target identification. Pro Lem areas include
noise reduction, signature identification, target detection, signal and image compres-
sion, and interference suppression. We make no attempt to detail echniques in these
areas; neither are we trying to provide readers with processing tebhniques at the re-
search level. Several examples are given in this chapter to demonstrate the advantages
and flexibility of using wavelets in signal and image processing.
    In these examples, wavelet algorithms are working in synery with other pro-
cessing techniques to yield a satisfactory solution to the problerti. Wavelet decom-
position plays the vital role in separating the signal into components before other
DSP techniques are applied. Algorithms include wavelet tree, wavelet-packet tree
decomposition, 2-D wavelet or wavelet packet tree decomposition, pyramid or di-
rection decomposition, and others. In signature recognition and t如get detection, the
corresponding reconstruction algorithm is not needed since the卜ignal components
 are either destroyed or rendered useless after processing. In the last two examples,
 the orthogonality between wavelet packets is applied to multicar ier communication
 systems, and the wavelet algorithms are extended to the third dimension for 3-D
medical image visualization. We discuss the extension of the w velet algorithms to
 wavelet packet algorithms and their 2-D versions before we disc iss various applica-
 tion examples.

210
                                                                 WAVELET PACKETS         211

9.1     WAVELET PACKETS

Because of the two-scale relation and the choice of the scale parameter a
                                                                                 = 2S,
the hierarchical wavelet decomposition produces signal components whose
                                                                                spectra
form consecutive octave bands. Figure 9.1 depicts this concept graphically.
                                                                                In cer-
tamll applications, the wavelet decomposition may not generate a spectral resolution
fine enough to meet the problem requirements. One approach is to use the CWT to
obtain the necessary finer resolution by substituting a smaller increment for the scale
parameter a. This approach increases the computation load by orders of magnitude.
Another approach has been discussed in Chapter 8. The use of wavelet packets also
helps to avoid this problem. A wavelet packet is a generalization of a wavelet in that
each octave frequency band of the wavelet spectrum is further subdivided into finer
frequency bands by using the two-scale relations repeatedly. In other words, the de-
velopment of wavelet packets is a refinement of wavelets in the frequency domain
and is based on a mathematical theorem proven by Daubechies [1] (splitting trick).
The theorem is stated as follows:
   If f (. - k) IkEz forms an orthonormal basis and

                                 Fi(x) =＞二 go[kIf(x -k)                                 (9.1)
                                 尻(x) =Zm町伍出，                                           但2)




      0.05




        0
         0         0.5       1        1.5       2       2.5       3       3.5       4
             FIGURE 9.1 Constant Q spectra for wavelets at different resolutions.
212                       DIGITAL SIGNAL PR그1CESSING APPLICATIONS

then {F1(. - 2k), F2(. 尸 2k); k E 7L} is an orthonormal basis of E = span(f (. - n);
fl E Z}.
    This theorem is obviously true when f is the scaling function 巾 since the two-
scale relations b0r 中 and the wavelet tr give

                                                 A/ 今 中（Vt) = ＞二go[k］中（2j+1t 尸k)

                                                 珌 3 少口t) =＞二冊神(2川n幻·

    If we apply this.theorem to the                                spaces, we                                       wavelet pcket subspaces.



                                                                                                                                       !
                                                                                            generate
m
                                                              W3
I ne                         recursive ro       ror waveiet,
                                                        r, i. I1 i.                                                    are                 (A,
                                         尸2t\i) = 乙日8（凡시尸n乙1 叫 凡J
                                                          -        ...                  .


                                                                                                                                           (7.J)
                                                     삐．                                                                                           'i
       generat                                                                 packet                  generation
                                                    k

                                                 肛fl+i (t) =＞二gi[k]／工1(2t - k) k E 乙                                                       (9.4)


where p. = 中 and p.i = 少 are the scaling function and the wavelet,                 For
Z= 1, we have the wavelet packets p. and 尸3 generated by the \                                                                               砂．
This process is repeated so that many wavelet packets can be ge                    the
two-scale relations. The first eight wavelet packets for the Haar ft LflCtion and 中D;3
(also referred to as D3) together with their spectra are shown in F: gures 9.2 to 9.5.
The translates of each of these wavelet packets form an orthogoi1al basis and the
wavelet packets are orthogon키 to one another within the same famil:, generated by an
orthonormal scaling function. We can decompose a signal into mar y wavelet packet
components. We remark here that a signal may be represented by1a .selected. set of
waveiet. pacKets witnout using every waveie1 packet .ior a given ie}'ei O1 resolution.
An.engineering practitioner may . construct an aigorimm .to cnoos tne paCKets b0r
optimizing a certaln measure (sucn as energy, entropy, variance, etcl). isest-nasis anu
best-      are two
                 level
                           algorithms      signal representations.
                                       popular
                                                                         for
                                                                               can fi                                        尸eaders         nd
these alg。rithms    [2]           in             .




9.2                      WAVELET PACKET ALGORITHMS

The decomposition tree for wavelet packets uses the same deco )osition block of
two parallel filtering channels followed by decimation by 2 (4. 2) i in the wavelet al-
gorithm. Any coefficient set in the tree may be processed by this b :k. In the wavelet
decomposition tree, only the approximation coefficient sets {a} in [gure 7.9 are pro-
cessed for different resolutions s, while the wavelet coefficient set w} are outputs of
the algorithm. In wavelet packet decomposition, the wavelet coefficient sets {w} are
also processed by the same building block to produce wavelet packet coefficient sets
l,rl. We see from Figure 9.6 that for each set of N coefficients. we obtain two coef-
ncient sets of IV/ Z length alter processing ny me oecomposnion DoCK. I ne numner
                                                                                         WAVELET PACKET ALGORITHMS                      213


                                               Haar --0
                     1.5                                                                                             Haar --1
                                                                                         1.       5
                             ]
                                                                                                  1
                    0.5
                                                                                         0.5
                             0
                                                                                              0
          -0.5
                                                                                         0.5


                         5
                          0        0.2                                             -1.5
          -         1.
                                           0.4       0.6     0.8       1               0                 0.2     0.4      0.6     0.8       l
                                               Haar --2
                   1.5                                                                                               Haar 小日
                                                                                        1.5
                         l11                                                                  ]
               0.5
                                                                                    0.5
                         0
                                                                                              0
              0.5
                                                                                    0.5

                                                                                              ]
                         5。
                                  0.2                                                    5
      -
               1.
                                          0.4       0.6     0.8                                         0.2
                                                                                    1.
                                                                                                                0.4      0.6     0.8
                                           Haar --4
          1.5                                                                                                    Haar --5
                                                                                   1.    5
                         1
                                                                                         ]        HH




          0.5.
                                                                                   0.5
                     0
                                                                                         0
      -0.5
                                                                                  -0.5
              -1
      -1.5
          0                      0.2                                              -1.5
                                         0.4       0.6     0.8     1                                   0.2     Q4        0.6    0.8     1
                                          Haar ---6
      1.5                                                                                                       Haar --7
                                                                                  1.5


                                                                                  0.5

                                                                                        0

                                                                            -0.5


               5。
                                 0.2     0.4                                        5。
-1.
                                                   0.6     0.8     1                                   0.2
                                                                            -1.
                                                                                                               0.4      0.6     0.8     1
                                         FIGURE 9.2        Wavelet packets of Haar scaling functi。
                                                                                                 n.
214        DIGITAL SIGNAL PROCESSING APPLICATIONS


                                                              F에,ier Tran＄幻no of Haar




0



0.7



0.6



0.5



0.4



0.




                                      1
                                          幻
                                              잃
                                                  나
                                                      Y
                                                          3
                    FIGURE 9.3 Magnitude spectra of Haar wavelet packets.


    of coefficient sets is 2"' if the original coefficient set is processed for m resolutions.
    Figure 9.6 demonstrates the wavelet packet tree for m = 2.
       It is imoortant to keei track of the indices of the wavelet Dacket coefficients in
    the decomposition algorithm. "1O achieve perfect reconstruction, it a coetticient set
    has been processed by ho[n] and (4, 2) , the result should be processed by go[n]
    and (十 2). The same order is applicable to hi[n] and gi[nl. Far example, if we
    process a set of data first by ho[n} and (4, 2) followed by hi[ I and (4, 2), the
    resulting signal must be processed by (十 2) and gi En] and then fol owed by (十 2) and
    go[n] to achieve perfect reconstruction. Thus signal processing us' g wavelet packets
    requires accurate bookkeeping of different orders of digital flit. "ng and sampling
    rate changes.


    9.3    THRESHO나기NG

    Thresholding is one of the most commonly used processing too. in wavelet signal
    processing. It is widely used in noise reduction, signal and imag『 compression, and
    sometimes in signal recognition. We consider three simple thres .lding methods [3]
                                                                                   THRESHOLDING                215


                       Daubech旭s 3 --0
                                                                                 Daubechies 3 --1




         0       1          2       3          4       5           0                  2       3            4       5
                      Daubechies 3 --2
                                                                                Da나bech治s3-小：3




                                                                           1         2        3            4       5
                      Daubec비as 3 卞 4
                                                                               Daubechies 3 --5
     2




                                                                                          \\
     1

     0
                                                                                                  ／沙
-1
-2
     0       1          2       3          4       5                   1          2       3            4       5
                     Daubechies 3 --6
                                                                               Daubechies 3 --7

                                                                                                  1




             1          2       3          4       5           0       1         2        3            4       5
                     FIGURE 9.4         Wavelet packets of Daubechies 3 sc出in
                                                                                 g function.
216          ［기GITAL SIGNAL PROCESSING 사가기ICATIONS



                                    Fourier Transform of Daubechies 3

         0




0.7 나                                                八
                                                             OOO。

0.6 口



0.5



0.4



0.3



0.2 口



0.1 -.




                FIGURE 9.5 Magnitude spectra of Daubechies 3 wavelet p: ckets.




here: (1) hard thresholding, (2) soft thresholding, and (3) perceni. ge thresholding.
The choice of thresholding method depends on the application. We discuss each type
briefly.



9.3.1         Hard Thres卜山Iding

Hard thresholding is sometimes called gating. If a signal (or a c. " fficient) value is
below a preset value, it is set to zero. That is,


                                   y=！즈 fo‘벼之a
                                          [U       IOflX1 <U,
                                                                                  (9.5)


 where a is the threshold value or the gate value. The graphical representation of
 the hard threshold is shown in Figure 9.7. Notice that the grap is nonlinear and
 discontinuous at x = a.
                                                                THRESHOL긔NG    217



                   Decomposition                        Reconstruction




FIGURE 9.6 Block diagram for the decomposition and reconstruction algorithms for
wavelet packets.


9.3.2   Soft Thresholding

Soft thresholding is defined as

                       y= ! sgn(x)f (I치- a) f叫지之a
                          (U,                                                 (9.6)
                                            torixi < a.



                                        Y




                                                    7
                                         , ' 7t/4
                                                                    x
                                                （了       1




                           FIGURE 9.7   Hard thresholding.
218      DIGITAL SIGNAL PROCESSING APPLICATIONS



                                                     Y




                        -   1           -a
                                                                                              >
                                                         a                        1




                                FIGURE 9.8 Soft thresholding.

The function f (x) is generally a linear function (a straight un \s'ith            to             巾                                 si아肥           be
chosen; see Figure 9.8). However, spline curves of t血d or fourthl.        m1lay oe useu                               fruer                  .




to effectively weight values greater than a-. In some signal compre1fsion appucauons,
using a qua如atic spline curves of order m > 2 may a什ect the co
a small 계llount.                                                                ratio " y         甲pression
9.3.3   Percentage Thresholding

In certain applications such as          compression,        a bit                as-
signed to th1e compressed tile, it is more advantageous to set      in percentage of
                                                                                                              4uota           has          been
                                             image                    where
wavelet coefficients to zero to satisfy the quota requirement.      case, the setting
of the threshold value a is based on the histogram of the coefficie         the total
number of coefficients. The thresholding rule is the same as hard           mg once
we have determined the threshold a.

9.3.4   Implementation
Implementations of the hard, soft, and percentage thresholding methods are quite
simple: One simply subtracts the threshold value from the magnitude of each coef-
ficient. If the difference is negative, the coefficient is set to zero. If the difference is
positive, no change is applied to the coefficient. To implement soft thresholding by
using a linear function of unit slope, the thresholding rule is

                       1J =
                       .1 -
                                !sgn(x)(I키- O) 피지- a찐
                                I (                      :J? 1 =1 1           -        - r\                                                       但7)
                                I. U
                                   --                    l1 1工1 1
                                                         UIAI   1U -                   - --
                                                                                      <-U.
                                                  八TERFERENCE SUPPRESSION          219

9.4   INTERFERENCE SUPPRESSION

The Wigner-Ville distribution and other nonlinear time-frequency distributions
                                                                                    are
often used in radar signal processing. Although they are not linear transformations,
they have an advantage in that a linear chirp signal appears as a straight line on the
time-frequency plane (see Chapter 4). However, the nonlinear distribution of a miii-
ticomponent signal produces interference that may have a high amplitude to cover up
the signal. This example combines the Wigner-Ville distribution decomposition and
the wavelet packets to suppress the interference [41. We take the signal with interfer-
ence and decompose it optimally into frequency bands by a best-basis selection [2].
We then apply the WVD decomposition to each of the wavelet packet signals. The
cross terms are deleted in the distribution before reconstruction. 가is approach keeps
the high resolution of WVD, yet reduces the cross-term interference to a minimum.
   From the viewp여nt of time-frequency analysis, an or血onormal wavelet 少 gen-
erates an orthonormal basis {砂f,k}, j, k e Z, of L2(R) in such a way that for each
j e 7L, the subfamily {少j,k : k e Z} is not only an orthonormal basis of W, but is
also a time-frequency window for extracting local information within the sth oc-
tave band H := (2J+l스享，21+2스享］
                             , wh町. 스享is the RMS bandwidth of the
wavelet. Unlike wavelets for which the width of the frequency band H, increases
with the frequency ranges, wavelet packets are capable of partitioning the higher-

&텍uency octaves to yield bert町 I比quency resolution.                 朗 discussed in
Chapter 4, is the standard deviation of 砂 relative to the positive frequency range
                                                           跳re
                                                                       스享，
(0, 的). Let {尸7i} be a family of wavelet packets corresponding to some orthonormal
scaling function po = 砂, as defined in Section 8.1. Then the family of subspaces
[／긍= (p.(. - k) : k c Z), n E Z+, is generated by {/t,j, and W can be expressed
as

                       ws= [／了" 缸。
                                 "+l4）···由U긍"" -I.
Inaddition, foreachm =0. ....2J -1, andj= 1, 2. .. ,thefamily

                              ｛尸2j+m（· - k) : k E Z}

is an orthonormal basis of U ' +m. The jth frequency band H is therefore partitioned
into 2J subbands:

                            H7Z,    m= 0. ....2J- l.                            (9.10)

Of course, the orthonormal basis in (9.8) of U긍'+m provides time localization within
the subband H71. Any function s (x) E L2 (R) has a representation


               蛔
                     ZZ       ＞二 出'm批2j+m(t中n) =＞二Sj,m(t),
                     j=1 m=0 n=-아그
                                                                               (9.11)
                                                                 f.m
220     DIGITAL SIGNAL PROCESSING APPLICATIONS

where dJm = (s(t), 尸21+m(t - n)), and the component

                                Sj,   m         (t)     =   ＞二
                                                             n
                                                                   d   'm,       i2j+ m   (t        -   n)
                                                                                                                                          (9.12)


represents the signal content of s (t) wi仕in the mth subband of the J
   L江 us rwnic     we vv V Li 101 4 IiIUIL1C0111101ICflL 51g1141,

              =1!1 1=1   /     J,.                11入 ttn     n4             /     J1\
              WVL)了(t, J) = LW '1J5j.mtt, J)
                                                      f.m


                                                      +2               ＞二
                                                            j,m,k,川m尹月；J尹k
                                                                                          WVDsj,m，           斗，
                                                                                                                    ，包／              ）·
                                                                                                                                          (9.13)


   Equation (9.13) partitions the tra小tional WVD into two subset卜. The 血st sum-
mation in (9.13) represents the auto-term, whereas the second sumrLation represents
the cross-terms between components in each subband to be considered as interfer-
ence. By removing this interference, we obtain the wavelet packet-based cross-term-
deleted representation (WPCDR), given by

                             比PCDR5(t, f) =Z WVD3,,,,(t, f).                                                                              (9.14)
                                                                       小m

We remark here that the WPCDR actually gives the auto WVD of the signal com-
ponents within each subband; therefore, it is quite effective and is perhaps the best
choice for analyzing a multicomponent signal. In addition, the WPCDR is compu-
tationally advantageous, since both decomposition and representation can be imple-
mented efficiently.

Best-Basis Selection Equation (9.8) is actually a special case of

                             Wi = [／王k由｛／却曲·由U嵩‘-i                                                                                        (9.15)

when k = j. Equation (9.15) means that the jth frequency band
tioned into 2', k = 0, 1. ....j, subbands

                                     J7}   '끼
                                                              m= 0, ... ,2" 1l.                                                           (9.16)

    The uniform division of the frequency axis and the logarithmic division for
wavelets are just two extreme cases, when k in (9.16) takes on the values of j and
0. respectively. In fact. k is allowed to vary amon으 Hi. I = 1. 2. . . . . so that the
subbands adapt to (or match) the local spectra ot the signal and theteby yield the best
representation or the best basis of the signal. The best basis can bd obtained by mml-
imizian the global cost functional or entronv. Specifically, the followin으 al으orithm
is used in tzj to nna we adapted Irequency sunnana or me equivalent nest Dasis:
                                                                                                                          1.
                  H "                                                        if E
                                                                                    (H.                       (H+              2m)
                                                                                               m)       <E
           니                                                                 +E（바" '跏" )                                                  (9.17)

                  jk+i.2m u月y1,2m4+1, otherwise,
                                                                                           FAULTY BEA뫼NG 引GNATURE IDEN기디CATION                                                                                   221


 where Hk,m represents the adapted freuuencv subband and E(H卜m) den。          tes the
 entropy of the local spectrum of the signal resthcted to the H?",
         1m뇨小   小        =dJy   1l   =         1   1   4   1   1    11小       H+        Jy11               !   1                   .   .   '              1   '   11   rrk     . 1
                                                                                                                                                                               "1d "




    /utnougn me mimmum entropy-Dasec best basis is usetul ror applications to seg-
 mentation in speech processing, it is not effective in our case, since the resultant
 小stribut油나似ds interferenc已 w帥iod妊y the algori如ito yield

                                                                                                                                                      if V&(H                          <0
                                                                                   'm
                                                                                                                                                                                             '
                                                                          H
                                                                                                                                                                         'm)
                                                                          fik+l'2m u月｝+1,2m+1 otherwise,
 where
            (H denotes the variance of the
                    V&
                                         'm)
                                                               and a   a       thresh-                                     local
                                                                                                                                               spectrum
                                                                                                                                                                                        is
 old. The idea behind this algorithm is that a narrow analysis band should be used
                                                                                                                                                                                                 preset
  when the local spectrum is well concentrated or when a small variance is obtained,
 while a wide band should be used when the local spectrum is spread or variance is
 large. We note in passing that a best basis is usually obtained between the third and
 fourth layers, since deeper layers may yield some adverse effects due to the ampli-
 tude increase in their spectral sidelobes.
    Once we have chosen a best basis, the signal is readily expressed as

                                                               m              以） 少-1               00

                                                                          ZZ Zj;k,
                                                                              d miL2k+m(23ekt_ fl)
                                                                          j= l m=O n=-00
                                                                                                                                                                                                          =




                                                                                                                                                                                                              (9.18)


where dm = (s(t), /.L2k+m(2JHkt 卞 n)) and
                                                                                               Z
                                                                                                       1
                                                                                                                       m
                                                                                                                                           m                  H        m
                                                                                                   얘
                                                                                                                   仰
                                                                                                                                                                                                              (9.19)
                                                                                           n
The WPCDR with a best-basis selection is given by

                                                                   WPCDR5(t, f) =Z
                                                                                 j,m
                                                                                     WVD ,(t, f).                                                                                                             但20)


    We apply this algorithm to a bicomponent signal consisting of a sinusoid and a
linear chirp signal. When compared with the WVD (see Figure 9.9), the WPCDR
of the same signal shown in Figure 9.10, the interference is suppressed. Figure 9.11
shows the 砥／PCDR with a best-basis selection produces the highest resolution on the
time-frequency plane.


9.5             FAULTY BEARIt늬（; 引GNATURE 山[NT仟ICATION

9.5.1               Pattern Recognition of Acoustic Signals
Acoustic signal recognition has gained much attention in recent years. It is applicable
to the recognition of ships from sonar signatures, cardiopulmonary 小agnostics from
222    DIGITAL SIGNAL PROCESSING APPLICATIONS


                                         WVD distrib川on




               m
               E=




                     20                        60           80       100     120
                                              frequency

FIGURE 9.9 꿔VD of a bicomponent signal. (Reprinted with per恤sion from [4], copyright
匣） 1998 by Wiley.)



                          WPT-based WVD-seiies time-frequency distflbution




        量250
                                                                                   득
                          50            100               150        200       250
                                              frequency
FIGURE 9.10 WPCDR of a bicomponent signal. (Reprinted with permission from [4], copy
right9 1998 by Wiley.)
                                   FAULTY BEARIF나G 引GNATURE IDEN기디CATION              223


                                 wPco日 with the best bas冶 S이ection
           500

           450

           400

           350

           300
          m
          E=
           250

           200

           150

           100

               50

                                                                                {
                          50           1伉1               150         200      250
                                             frequency

FIGURE 9.11 Best-basis WPCDR of a bicomponent sign毗 (Reprinted with pennission
from [4], copyright （흐）1998 by Wiley.)




heart sounds, safety warnings and noise suppression in factories, and recognition of
different types of bearing faults in the wheels of railroad cars. The basic goal of
acoustic signal recognition is to identify an acoustic signal pattern from a library of
acoustic signatures. Practically all acoustical signature patterns 缸e statistical in na-
ture, and they are also highly nonstationary. Using wavelets to extract feature signals
for recognition has 얍eat potential for success.
    To recognize an acoustic pattern reliably, it is necessary to have a set of distinctive
features forming a feature vector for each pattern. These feature vectors from differ-
ent pa仕erns are obtained by applying many data sets belonging to a particular event
in order to train a recognition algorithm such as an artificial neural network (ANN).
Alter we obtain the feature vectors through training, they are stored in a library and
used to compat七 \w恤 fe欲ure vec奴s from unknown even奴
    In this example [5] we apply wavelet techniques and an ANN to identify sev-
eral different types of faults in the wheel bearings of railroad cars. For information
purposes, we show the acoustic signal and its spectrum of a data set with a known
bearing defect (see Figure 9.12).
    The American Association of Railroads (AAR) provides us with acoustic signals
of 18 different types of bearing faults in two classes of sizes, the E-class and the
F-class. Each data set is about 0.5 megabite sampling at greater than 260 kHz. Each
bearing was tested under two different load conditions, and the wheel was rotating at
NNb




                                                         1

      FIGURE 9.12   (a) Acoustic signal emitted from a faulty bearing.
      FIGURE 9.12 (b)Spectrum of the acoustic signal in (a).

NNm
        226          DIGITAL SIGNAL PROCESSING APPLICATIONS



                Railroad defective                                                                         Sensors                            AID Sai叩ling
               wheel bearings under                                                                                                           at> 260kHz
                     evaluation                                                         1Microphone                                           or at 196k}妃
                                                                                        1Tachometer
        . Two loads                                                                     1Accelerometer                               Microphone
        130-80 mph per 10mph
                                                                                                                                      data only
        1Two bearing classes E & F
        . 16 known bearing conditions
        1Two is玎앉町y cons五t徊ns                                                                                                        Wa+e1et multires。
                                                                                                                                                     iuti。
                                                                                                                                                         n 。r
                                                                                                                                     FFT spectrum generation
                                                                                                                                            processing


                                     O旺小ne trais血埋
                                     of NN classifier with                                                    Feature                           Feature
                                     training data sets:                                                                  <
                                                                                                            normalization   Known              extractii月l
                                                                                                                                feature
                                                                                                                  口요旨니
                                     1F-class only                                                                                           1FF1' feature
                                                                                                                                vect이S
                                     1F-class o川y                                                                                            1CWT features
                                     . Both F and F classes                                                                                  1DWT features
                                                                                                               8mHmN큼口HbZ                    1WP features
                                                                    Weights 及 t月ases
                                                                                                                                                     1加known
                                                                                                                                                      feature
        On-line (real-lime)                                              V
                                                                                                             Feature conditioning                     vectors
           "Ia的ificatli月l                                        Cia弱tiler
        of unknown defect
                                           H                                           41                         using the        *Hm1
                                                               Neural networ
                              41m=
              acoustics                                                                                      normalization factors


                    디GURE 9.13 미ock diagram of the faul口bearing detecti여a伽帥m.


equi，
        nt岫 , , 畔ds of 30:, 80
               고，
                                              25꺄, cen：可 , ,         , , : , 田 , sed
                                                                               mph.
                                                                                            Only
                                                                                                                                     小data
for甘aining the feature vector in every case. The recognition algorithm is given in
Figure 9.13.


9.5.2               Wavelets, Wavelet Packets, and [FT Features
丁끼m4 1m. . mkm. 八c n1}t1m.11‘노n ... 4n』
sin. iiumtn. .i UI swilpfl. 口 ass .a,，느111 hm뇨1U1 .-i, .,. ..,, s12 ps,, c,,....,,e;,-,.. .-,c .i14 c. ..,.....
          ,.
                                        ii u. alnrn,'i.6. uata 10 5, I1fl 1 'JIiU (1it1Ui1 Ut                               -
                                                                                                                                                    tin. .   ILatUi

vec山rs cor eacn tecniuque is uescnoeu oeiow.

Wavelet Feature Extraction

         1. Perform the discrete wavelet decomposition on the signal (中WT) to the twelfth
            level of resolution,
         2. From the wavelet coefficients of each of the 12 resolution and approximation
            coefficients, compute the average energy content of the coefficients at each
            resolution. There are a total of 13 subbands (12 wavelet subbands and one
            approximation subband) from which features are extracted. The ith element of
            a feature vector is given by

                                               U
                                               i
                                                   1
                                                       d
                                                           1
                                                                W

                                                                         l m
                                                                         m            m
                                                                                      ZH
                                                                                       n
                                                                                       二 1
                                                                                         功
                                                                                           L


                                                                                                   J
                                                                                                       :
                                                                                                                  i= 1, 2. ....13,                           (9.21)
                                     FAULTY BEARING SIGNATURE IDENTIFICATION                                     227

     where ni = 211, fl2 = 210, fl3 = 29, ... , fl12 = 20, 7i13 = 20; v      is the
     ith feature element in a DWT feature vector; n, is the number of samples in
     an individual subband: and w2. is the ith coefficient of the ith subband. As a
     result, a iiw I reature vector is tormea as given Dy


                                       V1 畦"，·．·，W키' ·
                                  "" 니dwt                                                                    (9.22)

Wavelet Packet 斥ature Extraction

  1. Perform the wavelet packet multiresolu如n analysis to the fifth level of res-
     olution to obtain 32 subbands. Each subband contains a total of 128 wavelet
     packet coefficients.
  2. From each subband at the fifth level of resolution, compute the average energy
     content in the wavelet packet coefficients such that

            W

            1
            i
                     l m
                     1     꺄
                           ZH P                      l   八J口         八4U     八乙
                                                                                   and n, =128   =
                                                                                                           Vi,

                                                                                                             (9.23)

     where v ' ' is the ith feature in a wavelet packet feature vector, n1 is the number
     of sample in each subband, and Pi,j is the jth wavelet packet coefficient in the
     ith subband. The WP feature vector is represented as follows:

                                                                                  Uwp
                                                                                  l)                         (9.24)
                                                                                        't
                                  VWP-
                                         -
                                             {vwpJ
                                                     1         wp尸
                                                                     ．   .    ,         J    .




Spectral Feature Extraction We also use the traditional FFT approach to solve
this problem for the sake of comparison. The FFT feature vectors are cons仕ucted
的加wi雎 the same pattern.

   1. From the 212 data points, we compute the FF1' and take only the positive fre-
      quency information represented by 212 spectral coefficients.
   2. We divide the spectrum into 32 nonoverlapping bands with equal width. From
      each band we compute the average energy contained in the coefficients. The
      feature element becomes

            m
            i
                 l m
                 H       꺄
                         ZH              i= 1, 2. ....32 and n, = 128                                Vi,     (9.25)



      where S乙 is the jth FF1' coefficient in the ith subband. Consequently, the
     ieawre vector uecome

                                    "' 니此『프'，···，唾｝' ·                                                       (9.26)
 228      DIGITAL SIGNAL PROCESSING APPLICATIONS


 TABLE 9.1 Overall Performa乂e of the Network for F, E, and F and E Class Bearings

 Values (%)                  I1'J'             CWT             DWT                   WP
                                     F＜깃口ss Be口rings
Correct decision            96.06              95.70           92.37                92.87
Misclassification            1.67               1.69            4.56                 2.49
Miss                         2.26               2.61            3.07                 4.64
                                     E-Ch玎s Be口rings
Correct decision            95.96             94.16            87.50                93.76
Misclassification            1.28              2.35             7.05                 2.50
Miss                         2.76              3.50             5.45                 3.74
                                F. 口ndE-Cl口了s Be口rings
Correct decision            95.18             94.22            87.61                92.41
入小sciass小cation              0.93              2.35             8.88                 3.19
Miss                         3.89              3.42             3.51                 4.40

   After the feature vectors have been obtained, we apply the feature vector normal-
ization to separate the vectors farther apart to improve performance of recognition.
These vectors are used to train an ANN. There a七 three hidden neurons in this 시나나.
Details of construction and training of the A寸N are beyond the scope of this book
and we refer the interested reader to [61.

 Results The recognition results obtained using the wavelet techniques combined
 with the ANN 町e astounding. Every fault in every class is identified using the unused
(not for training) portion of each data set. In fact, the two "mystery" (unknown)
bearings containing more than one fault a七 all identified. Although the traditional
FFT approach produces roughly the same results as the wavelet approach, it fails
to recognize the unknown bearing by missing one of the two faults. We conclude
that the new feature extraction methods using DWT and WP are comparable if not
superior to the FF1' approach. The FFT lacks the time-domain information and thus
misses some of the more localized faults.
   The feature vector normalization and conditioning play a key role in the conver-
gence of the neural network while training. Without the normalization, the network
does not converge to the desired network error. Convergence of the network produces
the biases and the weights necessary for testing of the real data. Three hidden layers
are used to improve the convergence. The results are given collectively in Table 9.1.


9.6     TWO-DIMENSIONAL WAVELETS AND WAVELET PACKETS

9.6.1    Two-Dimensional Wavelets
When the input signal is two-dimensional (2-D), it is necessary to represent the sig-
nal components by 2-D wavelets and a 2-D approximation function. For any scal-
                           TWO-DIMENSIONAL WAVELETS AND WAVELET PACKETS           229

ing function 砂 with its corresponding wavelet 砂, we construct three different 2-D
wavelets and one 2-D approximation function using the tensor-product approach.
We write the 2-D wavelets as

                            叫化 y) = 叭卜 i)少(y- j)                               (9.27)

                            出［，
                              三J（工， y) = 砂（x 寸 i）中（y- j)                       但28)

                            山！}（工，y) = 砂（x- i）砂（y- j),                         (9.29)
and the 2-D scaling function as

                             4 i,j （工， y) = 砂（工   i）中（y- /）·                   (9.30)

叫化y), 山刃化y), and 叫，如，力 町m如的ets sin呻hey satisfy

                L i_:叫？(x,y)dxdy= 0                    forj = 1, 2, 3.

The 2-D approximation function and wavelets of the cubic spline are shown in Fig-
ure 9.14. In the spectral domain, each of the wavelets and the scaling function oc-


              2-D scaling function                             2-I) 나av이et 1




          x       4   0        V


                2 [) 나ave厄t2                                   2-C) 나av이et 3




          x       6   0        V

   FIGURE 9.14 Two-dimensional scaling function and the corresponding wavelets.
 230    DIGITAL SIGNAL PROCESSING APPLICATIONS

 cupy a different oortion of the 2-D soectral plane. The spectral di$tributions of each
 of these tour '2-li functions 缸e shown in h2ure 9.1>. the sPectral bands that are Ia느
 beled low-lu므h (LH). Lu아l크ow (HL) and hi2I卜寸ii으h 仕iH) corresr)ond to the soectra
 of the wavelets 4I!4f] (x. v). M = 1. 2. 3. The l。
                                                  w-l。w (LU) band c。   rresponds to the
  -u approximation function. 't"he terms 勿w- and high- refer to whether the process-
ing filter is lowpass or highpass. The decomposition of a 2-D signal results in the
 well-known hierarchical pyramid. Due to the downsanipling operation, each image
is decomposed into four subimages. The size of each subimage is only a qua八er of
the original image. An example of hierarchical decomposition of a gray-scale image
is given in Figure 9.16.




                              WY

                               /1




砂（nb)V7（口）y)            可Wx）少m功                  砂（Wx）砂（Wy)




                                                                               >.   wx
叭따岫(Ci功                 中（Ci）上）中（WY)             叭nh岫(Ci功




少（W土）V7 (nb)            中（Ci）工）少（WY)             少 (Wx)lfr (WY)



FIGURE 9.15 Regions on the 2-D spec甘al plane occupied by the 2- scaling function and
wavelets.
                        TWO-DIMENSIONAL WAVELETS AND WAVELET PACKETS            231




          FIGURE 9.16 Two-dimensional wavelet decomposition of an image.



9.6.2   Two-Dimensional Wavelet Packets
Two-dimensional wavelet packets are refinements of the 2-D wavelets similar l-D
case. Using the notation /ik(x) to represent the kth wavelet packet belonging to the
approximation 鈿ction jio(x) = 中 (x), a tensor product of any two wavelet packets
generates a 2-D wavelet packet. That is,

                            肛k , e（工， y) = 秘k（工）／化(y).                       但끄）

Consequently, there 町e many 2-D wavelet packets that can be chosen to form bases
in L2 for signal representation. For example, in the l-D case we use the two-scale
relations for three levels, resulting in 23 = 8 wavelet packets, including the LLL
232     DIGITAL SIGNAL PROCESSING APPLICATIONS

components of the approximation function. Taking the tensor        Ct of any two
packets, we obtain 64 different 2-D wavelet packets, including     D approxima-
tion functions

                               尸0,0（工， y) = 尸0（工）尸0(Y).                      (9.32)

There are too many 2-D wavelet packets to be shown individually.   o examples of
2-D wavelet packets are shown in Figure 9.17.




               100
                                                             100
                          50
                                                   50
                                     0   0




                                                                       150




                                             (b)
                     FIGURE 9.17 Two 2-D Haar wavelet packets.
WAVELET AND WAVELET PACKET ALGORITHMS FOR TWO-DIMENSIONAL SIGNALS                    233

9.7     WAVELET AND WAVELET PACKET ALGORITHMS
        FOR TWO-DIMENSIONAL SIGNALS

9.7.1    Two-Dimensional Wavelet Algorithm
We have discussed in previous sections that the 2-D wavelets are tensor products
of the l-D scaling function and the wavelet. Corresponding to the scaling function
中 and the wavelet 少 in one dimension are three 2-D wavelets and one 2-D scaling
function at each level of resolution. As a result, the 2-D extension of the wavelet algo-
rithms is the 1-D algori仕m applied to both the x- and y-directions of the 2-D signal.
Let us consider a 2-D signal as a rectangular matrix of signal values. In the case
where the 2-D signal is an image, we call these signal values PIXEL values cone-
sponding to the intensity of the optical reflection. Consider the input signal CJ (m, n)
as an N x N square matrix. We may process the signal along the x-direction first.
That is, we decompose the signal row-wise for every row using the l-D decompo-
sition algorithm. Because of the downsampling operation, the two resultant matri-
ces are rectangular of size N x N/2. These matrices are then transposed, and they
are processed row-wise again to obtain four N/2 x N/2 square matrices, n帥ely,
寸1(m, n), d尸似n)，才1(m, n), andd卄m, n). The subscripts山he d matri-
ces correspond to the t뇨ee different wavelets. The algorit노n for 2-D decomposition
is shown in Figure 9.18. This procedure can be repeated for an arbitrary number of
times to the ct(m, n) matrix (or the LL component), and the total number of coeffi-
cients after the decomposition is always equal to the initial input coefficient N2. An
example of the decomposition is shown in Figure 9.19.
   If the coefficients are not processed, the original data can be recovered exactly
through the reconstruction algorithm. The procedure is simply the reverse of the
decomposition except that the sequences are {go[k], gi [k]} instead of {h0[k], h1[k]}.
Care should be taken to remember upsampling before convolution with the input




                          x                                                   LL
                            [k

                                                                              LH

                                                                              HL
                         h, [k

                                                                              HH
 FIGURE 9.18 Block diagram of the two-dimensional wavelet decomposition algori恤n.
234      DI(고TAt 듸GNAt PROCESSING 사가기ICATIONS




        FIGURE 9.19   A two-dimensional hierarchichal decomposition of an image.


sequences. The perfectly reconstructed image is identical to the original image in
Figure 9.20.


9.7.2   Wavelet Packet Algorithm

The 2-D wavelet packet algorithm mimics the l-D case. It sim月y reoeats the alco-
nt끄lls nrsr aiong tne x-airecuon ano men along the y-clirection. 八ot only is the LL
component (the approximation function comDonent) decomnosekl to obtain further
aetaiis 01 me image, me other wavelet components (LI-I, I-IL, HI-I) 게e also turther
decomposed. For example, starting with an original image with size 256 x 256, a 2-D


                                                                  f
wavelet decomposition of this image will result in four subimages of size 128 x 128.
Lon빤끄嶝. me aecomposition, one get욘 坦三I) wav.ele印呻란叩bimage叫｝吃e
叫 x 아. 1he computational algorithm tor 2-I) wavelet packets           no more ditticult
                                                          IMAGE COMPRESSION         235




        FIGURE 9.20 Perfect reconstruction from components shown in Figure 9.19.


than that for the 2-D wavelets. It requires orderly bookkeeping to keep track of the
directions (x or y) and the filters that have been used in processing. It is necess町y to
reverse the order to reconstruct the image from its wavelet packet components. An
example of 2-D wavelet packet decomposition of an image and its reconstruction is
shown in Figures 9.21 and 9.22.


9.8     IMAGE COMPRESSION

9.8.1    Image Coding
There exist in the literature many coding schemes for image compression. The basic
idea of compression is to try to reduce the average number of bits per pixel to ad-
equately represent the image. Image compression is urgently needed for very large
medical or satellite images, both for reducing the storage requirements and for im-
proving transmission efficiency. Coding schemes 缸e classified as lossless (recov-
erable) and lossy (nonrecoverable) types. Compression ratios a七 usually very low
(approximately 10 or less) for lossless coding. Schemes like the Huffman code, run-
length code, arithmetic code, predictive coding, and bit plane coding belong to the
lossless class. Lossy coding methods may be constructed through a variety of ways.
236      DIGITAL SIGNAL PROCESSING APPLICATIONS




            FIGURE 9.21     A 2-D wavelet packet decomposition of an image.



We will use the zero-tree algorithm to demonstrate the application of wavelets to
image compression.


9.8.2   Wavelet Tree Coder

In general, tree coders [7] use a tree structure which takes advantage of the cone-
lation between the discrete wavelet coefficients (DWCs) in each of the three spatial
directions (i.e., HL, LH, and HH), as shown in Figure 9.23. That means that if a
DWC at a higher decomposition level is smaller than a specified threshold, there is a
great possibility that all of its children and grandchildren are smaller than the thresh-
old. Thus, all of these insign戶cant DWCs can be encoded with one symbol. The
encoding of a significant DWC may need more bits. Many tree structures have been
                                                         小4AGE Co入4PRESSION       237




FIGURE 9.22 Perfect reconstruction from wavelet packet components shown in Fig-
ure 9.21.

developed for improving the efficiency of encoding the locations of the correlated
DWCs, such as EZW, SOT, and GST
   A brief description of a generic tree coder is as follows:

   1. The DWCs are selected in groups with decreasing thresholds such that larger
      DWCs are encoded earlier.
   2. The first threshold is selected to be an integer T0 = 2.', where j is the nearest
      integer 5 log2 max IDWCI and the kth threshold is Tk = To/2", that is, the
      uniform quantization.
   3. Choosing the t뇨eshold Tk, all the locations of this group of DWCs, C1, j with
      Tk 5 ICi,1I < Tk_ l, 町e encoded with a tree structure, and signs of these
      enc에ed DWCs 毗 also appended. This process is called the dominant pass.
   4. Those C ,j encoded in previous higher thresholds are refined to a better ac-
      curacy by appending the bit corresponding to Tk. 가1is process is called the
      subordin口te p口ss.
   5. W反th decrea鈿g thresh이ds, the leading 乙라ob出 可 encoded DWCs are saved
      to achieve compression.
   6. The number of bits in the coded bit stream from a tree coder can be further
      reduced using a lossless ent아y coder (e.g., an a血hmetic coder [8]).
238      DIGITAL SIGNAL PROCESSING APPLIC지ONS



         LL3             HL3                   HL2
                  '
                      - e乂그 -

                                          E三，
             ［갔
          唾            '쌤        「                   111
                                                           뇨


                                     '.        HH2
         LH2\

                  뇨                       늄｝    .




          LH1               :
                            ':
                            q                              4   '




FIGURE 9.23 Spatial correlation and parent-child relationship among wavelet coefficients
at different resolutions.


9.8.3   EZW Code
Initiated by Shapiro [9], the zero-tree structure combined with bit plane coding is an
efficient compression scheme for the discrete wavelet transformation. The embedded
zero-tree wavelet (EZW) coding scheme has proven its efficiency and flexibility in
still image coding in terms of image quality and computation simplicity. Also, the
EZW image coding algorithm generates an embedded bit stream in which informa-
tion is sent to the decoder in the order of its importance; importance is judged by
how much the information reduces the distortion of the reconstructed image. This
embedded technique has two important advantages. First, the bit rate control allows
one to stop the coding process at any point. Second, the image can be reconstructed
from a point where the encoded bit stream has been disrupted, 寸ven with reduced
quality.                                                              J
    As an entropy coder, the zero-tree coder takes advantage of 컥he correlation be-
tween interlevel subbands of DWCs. Four symbols, ZTR, POS, NEG, and IZ, are
used in the zero-tree. A刀R, zero-tree root, represents a DWC and all of its descen-
dants if they 게：e insignificant, and it is the symbol that gets most of the compression.
 A POS or NEG symbol stands for a significant DWC with a positive or negative sign.
                                                                              小IAGE Co入4PRESSIO卜4   239

 An IZ represents an insignificant DWC with at lea戚 one significant descendent. It
                                                                                   is
 this symbol that reduces the compression since more symbols are needed for encod-
 ing its descendants. With the definitions above, two bits per symbol on average
                                                                                 are
 needed for each of the four symbols. Without a good follow-up entropy coder
                                                                                 for
 those symbols, zero-tree cannot get good compression results. Also, all of the en-
 coded symbols must be reordered so that the entropy coder can achieve compression
 on them. Both of these procedures increase the computation overhead.



 9.8.4   EZW Example
We use a well-designed example similar to the one appearing in Shapiro's original
paper [9] to demonstrate the procedure. The EZW is a successive approximation
algorithm. It uses the dominant pass and the subordinant p口ss recursively to achieve
the approximation. The coefficient map of this example is shown as follows:



                          58        41   -44   -17         -
                                                                8        13          5        8
                          29   -47        42   -13              3        4      卞    l       10
                          22   -14        25    -9
                                                               35   -11              6        7
                     -9
                               -11 -16               12   -3
                                                                         6          14   ＝느   1
                    -13             2      0   -11             0    -30             15        7
                          10   -5
                                           9         4    -7
                                                                    -
                                                                         l     -9
                                                                                              0
                    -22             4    -13         3         6    -8
                                                                                    11        5
                          9    -
                                    l      9   -12             2         5          9    -
                                                                                              3


    Following the steps outlined in Section 9.8.3, we find the largest value to be coded
is M = 58. The nearest power-of-2 integer 2j ? 58/2 = 29 is 25 = 32. We set the
initial t뇨eshold value T0 = 32 = 25. We then use this t뇨eshold and compare it with
all of the coefficients in a dominant pass, described below.
   In wavelet-甘ee coding, not only do the values of the coefficients need to be coded,
the location of the coefficients must also be known to the decoder. The EZW makes
use of the parent-children relationship between coefficients in adjacent coefficient
maps to record the location of a given coefficient. This relationship is embedded in
the EZW code to reduce the coding overhead. 가lis relationship is best shown in
Figure 9.23. The coding procedure is listed as follows.


   1. For the first dominant pass, the threshold is set at 32 and the results of the code
      assignment are given in the following table. We assign a symbol to each of the
      codeable values:
240      DIGITAL SIGNAL PROCESSING APPLICATIONS

                               Reconsti기C妃d                                    Recoi好truc把d
       Value         Symbol        Value           Value      Symbol               Value
         58           P                48           -16          ZTR                  0
         41           P                48            12          ZTR                  0
         29           ZTR               0            -8          Z                    0
       -47            N             -48              13          Z                    0
       -44            N             -48                3         Z                    0
       -17           乙FR               0              4          Z                    0
         42           P                48            35          P                    48
       -13            ZTR              0            -11          Z                    0
         25          乙FR               0             -3          Z                    0
         -9           ZTR              0               6         Z                    0



  2.   After the first dominant pass has been completed, the first     isub。  rdinate          pass
       refines the coded values. Only those significant values (P e1nd N) are coded
       in this pass. The symbol P in the first subordinate pass staLes that the value
       lies in the interval (64, 32], and the symbol N, in the interval (- 64, 32] The
                                                                                  -        .




       subordinate pass refines these values by narrowing the inte너val from (64, 32]
       to (64, 48] and (48, 32]. If the value is in the upper interva'1, the subordinate
       pass appends a "1" to the code, a "0" if the value lies in the ld)wer interval. The
       six significant values now have the following code file:


       Coefficient                               Reconstructed                    Binaly
       Magnitude              Symbol              Magnitude                    Representation
           58                   I                      56                         111010
           41                   0                      40                         세11001
           47                   0                      40                         101111
           44                   0                      40                         101100
           42                   0                      40                         101010
           35                   0                      40                         100011


       This completes the first iteration of both passes. The user has to remember that
       in the subordinate pass, if a "1" is appended to the code, oile has to subtract
       the refinement amount, n出llely 16 in this case, from the vahie that is over the
       threshold for this pass. For example, the coefficient 58 ha북 58 - 32 小 16 =
       10 yet to be refined by the next iteration. In addition, th4 user should also
       remember that the coded values are now replaced by zer（닉 in the coefficient
       map and will not be coded from later iterations.              i
                                                                                                                  小4AGE Co入4PRESSION                                         241

3. We repeat step 1 with the second dominant pass with a threshold T1 = 16. We
   have the following codes from this pass:


   Coefficient                                        Reconstructed                         Coefficient                                              Reconstructed
     Value                        Symbol                 Value                                Value                   Symbol                            Value




                                                                                                                           ZZZZZZZNZZZZNZZZZZZ
                                                                                                                                                           0000000가0000겨000000
        29                        p                               24                          -11




                                                                      겨0겨000겨0짜000000000
        17-
                                  N                               1

                                                                                                3
                                                                                                -
      -13                         ZTR                                                           6
        22                        p                                                           卜13
      -14                         乙11<                                                          2
         9    -
                                  Iz                                                           10
      -
        11                        ZTR                                                           -5
        25                        p                                                            -22

                                                                                                4   l0
                                                                                                            1




         9    -
                                  ZTR
      -16                         N

                                                                                                 /0
        12                        ZTR




                                   ZZZZZZZZ
                                                                                                                       4




         8
                  l



                      八
              H
                      4
                      나 4
                        A
                        口 d
                          1 <
                            1
                            U 8
                                                                                               -30
                                                                                                         n
                                                                                                         / l
                                                                                                                                                 e




                                                                                                                                                 1




                                                                                                         6

                  1
                                                                                                        8
                                                                                                                                                 1



                      l

                                                                                                        n
                                                                                                        乙 <
                                                                                                          1
                                                                                                          U
                  0
                  H




                  1


4. The second subordinate pass will separate the intervals more finely by divid-
   ing all intervals at their midpoints. Hence we have intervals (64,56], (56,48],
   (48,40], (40,321, (32,24], and (24,161. This pass also updates all previous code
   files. The value to be compared with in this pass is 8. The updated code file
   becomes:

  Coefficient                                                                              Reconstructed                                            Binary
  Magnitude                                   Syn小이                                         Magnitude                                            Representation




                                               l



                                                                                                 印MM恥M拍羽m加羽加加 羽
                                                  ll
      58




                                                      0l00l00 l
                                                                                                                                                      111010
      41                                                                                                                                              101001
      47                                                                                                                                              101111
      44                                                                                                                                              101100
      42                                                                                                                                              101010




                                                1
                                                1   l
                                                    1
      35                                                                                                                                              100011
      29                                                                                                                                              011101
      17                                                                                                                                              아以）01
      22                                                                                                                                              010110
      25                                                                                                                                              011001
      16                                                                                                                                              010000
      22                                                                                                                                              010110
      30                                                                                                                                              011110
242               DIGITAL SIGNAL PROCESSING APPLICATIONS




                         FIGURE 9.24 Origin키 image for EZW image codin.


   The   passe，
                       町.：叩eated b恥.出雎由.         如心h이d
                                                           by half each1
                                                                       ime.
                                                                                        I，키，the co-
efficients are coded, we have a lossless code. The compression ratio achieved in this
manner is limited. High compression ratio is achieved using EZW followed by a
lossless en甘opy coder. The user may stop coding at any time or when the bit budget
is exhausted. We have a lossy compression scheme wherein users may control the bit
nuaget nut cannot control me compression ratio. An on으ina1 image and the image
recoverea rrom t.LW cooing 缸e snown in 1igures 9.24 and 9.Z: .

9.8.5             Spatial-Oriented Tree
Said and Pearlman [10,111 discovered set partitioning principles tr)             the
                                                                              improve          per-
formance up to 1.3 dB over that of the zero-tree method. They dbserved that there
is a spatial self-similarity between subbands, and the discrete wavelet coe卄icients
(DWCs) are expected to be better magnitude ordered if one moves downward in the
pyramid following the same spatial orientation. Based on this 9bservation, a tree
structure called a spatial orientation tree (SOT) is used to define 4ie spatial relation-
ship of the DWCs in the hierarchical structure. Three main con4epts are pro刃sed
by Said and Pearlman to adapt the SOT to obtain better perform4nce in image cod-
ing: (1) partial ordering of the transformed image by magnitude and transmission of
coordinates via a subset partitioning algorithm, (2) ordered bit p너ne 甘ansmission of
                                                           小4AGE CO入作RESSION          243




                 FIGURE 9.25 Decoded image at compression of 30:1.




refinement bits, and (3) exploitation of the self-similarity of the DWCs across the
various scales.
    For the SOT [10-12], only two symbols, zero and one, are used, and each symbol
has a different meaning at a different p毗 of the tree. The symbol one may represent
(1) a significant DWC, (2) the negative sign of a significant DWC, (3) the case that
any one of the four children is significant, or (4) the case that any of the grandchil-
dren is 計帥而cant. The syn小이 zen比애Id indicate (1) an insign而cant DWC, (2) the
positive sign of a significant DWC, (3) the case that all four children are insignifi-
cant, or (4) the case that all grandchildren are insignificant. To maintain the SOT for
the DWCs along with the different scales, 血ee lists are used as follows:


   1. US, list of insignificant sets, is a list of the roots of a tree for further tracing,
      and types A and B of the roots of the tree are used interchangeably to obtain
      better adaptability.
   2. LIP, list of insignificant pixels, is a list of the DWCs that are not roots of the
      tree currently but are the candidates to be placed into the LSP.
   3. LSP, list of sign加ant pixels, is a list of the DWCs that have been encoded and
      are to be further refined.
 244      ［거（긔TAL SI(고너AL PROCESSIF니C APPLICATIONS

 9.8.6    Genera血ed Se作鈿iilarity Tree
 Based on the SOT, a generalized seif-simila也y tree (GST) coding algorithm has
 been cons甘ucted that can handle images of any size and any gray level [13]. In the
 GST, the wavelet decomposition/reconstruction algorithm with boundary reflection
 techniques is used so that perfect reconstruction can be achieved. Analysis of the
 GST coder shows results comparable to the origin고 SOT coder for images of dvadic
 size, ana it even outperiorms me aui br images or nonayamc siz.



 9.9     人시CROCALC汗ICATl0卜4 CLUSTER DETECTION

 The majority of early breast cancers are indicated by the nresen托 of one or more
 clusters or microcalcilications on a mammogram. Although breastlcancer can be ta-
 tat, women nave one or me mgnest cnances or survival among cancer types ii me
 tumors can be detected and removed in an early stage. Thus the detection of micro-
 calcifications with minimal false- 兀sitive rates is critical to screeni如 mammograms.
Microcaiclilcations are small dePosits ot calcium phosphate hvclrdxide in breast tis-
 sue witn sizes raging irom IJ.UD to 1.0 mm in diameter wnxcfl appear as ongnt specKs
on photonegative x-ray film [14]. They are difficult to detect because they vary in
size and shape, and they are embedded in parenchymal tissue stri. ctures of varying
density [15].
    Screening mammograms have been one of the main thrusts in e health care pro-
gram of the United States. However, even partial compliance with the rule set by
the ACR would produce a huge volume of data to be read by a limited number of
radiologists. Consequently, human error can run the percentages of false negatives
(a true target missed) up to 20 percent [16]. If a computer-aided-diagnostic (CAD)
algorithm were designed and constr口cted, it could serve as a second opinion to help
the radiologist by pointing out suspicious regions in the mammo으r게r1l needing a more
detailed diagnostic screening. '11115 application example attempts t0 show how a two-
dimensional wavelet ovramid algorithm workin으 in conjunction with other image
processing tecnniques can identiry me microcalcmcations in mammograms and 1O-
calize the suspicious regions.


9.9.1    CAD Algorithm Structure

Success in signature recognition depends strongly on the featurds one can extract
from a signature. The more distinct the features, the higher the success rate for
making a Positive Identitication. Ihe most imoortant obiective itr the detection and
recognition ot microcalcitications is to remove the background itoise and enhance
the object to be identiFied. We use several traditional image processing techniques to
work with the wavelet decomposition algorithm to achieve this objective. Decision-
m曲ng rules in 5이ne 可these algorithms 缸e goal oriented and there的re 毗 까的向I
dependent. Parameter choices often depend on the data to be analyzed. The CAD al-
gorithm for microcalcification cluster detection in a highly textured and cluttered
                                          入시CROCALCIFICATION CLUSTER DETECTIC가니              245


                          11耳反l d坦仕teed                            G巴rl拙e an in好 1刃ith
                           H日nhiTigr可n                             all detected ixeJs th y

                      回거I In慰e Fmtitioil唯
                                                              CFAR-lllce a1 壯ye 仕ie寸U님I'띵
                                                                Ir evah日d匹 a thre寸t1d
                   NorIirar in與忙 elim吐毗1l                      毋yen eanh detected F才：配lard
                    for ea산1parIit1ored in慰e               仕E g加en 佃院 삯ann (or FP) 口吐沚iii却
                                                                   1뵤妃 Gai姓an PDF

    U
     !
     m벼
      匕H
                  Warelet 1iyramida1 aiim dii土이月l
   m員H旨mb      Ire텍契 m（刃n4X妓fion & remi甘nrtlon              Irit［沚 di蜘크II땅 可 t比 1虹els 且rvivl： 唯
   亡g＝旻 나          11/i仕1W四elet C뇨rUin op巴Bil이r              1：比 出a*Ive 缸ed띠Idix뇜 1d［뇜 ARTQ
  H五Hm亡乞小니     coeffli뵤ertrentval, thee삯Ukil꺄L ad               with a given vigilare七［目汪lrmr
                            an甲tin（斌Ion

                                                             F可配 cli月L町 di포그mnu斌向IIyi뵤四
                                                              railol（띵i曲5'prantice: at기nfrr 可
                    鼠tnt比 fdl iir叩es fmm                    bi야月Inearh cli風口 arel tl blot) 섧；C心
             t比 F恥nnldal aid dli毛Cti0l月Immi胤rlxmlorE
                          pixel tt lixel
                                                               Pre配a仕E 0啣ii뇨哨 1刃Ith
                                                                fin日(cli斑r辰O1 Iraik才i아好
                    Hi幽哈mm Ui耐Uldir평 arel
                                                             d口比m 四er 仕E 0叱froti甲liii蛇e
                       dark1uxel rentival
                                                                      to ttr ra丑olo깹L引：5

    디GURE 9.26 미ock dia酊帥of the microcalcification clu毗r dete아ion a培on曲a.


background is illustrated in Figure 9.26. The image processing techniques used in
this CAD algorithm include nonlinear image enhancement, wavelet pyramidal and
directional image decomposition and reconstruction, wavelet coefficient domain op-
erations, dark pixel removal, constant-false-alarm-rate (C-FAR) adaptive threshold-
ing, adaptive resonance theory clustering, and false cluster discrimination.


9.9.2    Partitioning of Image and Nonlinear Contrast Enhancement
We partition the mammogr缸1l to be analyzed simply by dividing the image into a
number of equal-sized subimages. In this case the size of the mammogram is 1024
 x 1024 and we divide it up into 64 subimages of size 128 x 128. Each partitioned
subimage is processed separately to bring out locally significant details of the in-
put image with image contrast enhancement. This step provides better localization
for detection of the targets. Since wavelet processing is known to handle the image
boundary better than DCT, we are assured that information is not lost in the parti-
tioning. We use cubic mapping to suppress pixels with low gray-scale values and to
enhance pixels with large gray-scale values.


9.9.3    Wavelet Decomposition of the Subimages
We decompose each subimage using the wavelet decomposition algorithm so that
the high-frequency components of the subimage are singled out. There are many
choices of wavelets in this applications. We chose the Haar wavelet after examining
all of Daubechies' orthogonal and biorthogonal wavelets and the coiflets, because the
246      DIGITAL SIGNAL PROCESSING APPLICATIONS


spatial-domain window of the Haar wavelet is very small for bettdr soatial localiza-
tion. i-nnner-oraer waveiets rena to avera므e ana Diur me nign-rreuuencv information
to Produce a low-게aplitude wavelet coemcient.                      I
   Iwo types of wavelet MKA tree decompositions, pyramidal and directional de-
compositions, are applied    simul帥eously
                                             to the same subirnag. The pyramidal
                                                     .     .



싸iici uecomposes orny me suooanu. image oDtalnea mrougn we LL-Su.DDanu in
tne, coiumn ana row rnr，凹tion at eacfl level Of resolution (LUK.
                                            .                  .     e airectioflal
                                                                        m}
iviic/\, on me omer nana, aecomposes images in oniy one airecrion. I ne aecompo-
sition wavelet coefficient maps of these two MRA trees are shoWn in Figures 9.27
and 9.28.


9.9.4    Wavelet Coefficient Domain Processing

Once we have the wavelet coefficients computed as shown in the preceding section,
the goal of processing these coefficients is to retain only the signifi中ant wavelet coef-
ficients that pert缸n to microcalcifications and other high-frequency information. Pro-
cessing these coefficients includes removal, thresholding, and amplification. These
缸e operations without a user interface; we must generate rules and parameters to
guide these operations.
    To retain high-frequency information that contains microcalcifications and other
high-frequency noise, the wavelet coefficients in the lower-resolution subbands
are removed. For each partitioned subimage, we compute the 멥oba1 (all wavelet
coefficients in the subimage) standard deviation-to-mean ratio (3SMR) and local




      FIGURE 9.27 Hierarchical wavelet dec。 siti。
                                          mp。   n 。f a segmenteJ mamm。
                                                                     gram.
                                             入시CROCALC汗ICATION CWSTER DETEC지ON                    247




     FIGURE 9.28 Directional wavelet decomposition of a segmented mammogram.



(wavelet coefficients in one subband of the subimage) standard deviation-to-mean
ratio (LSMR) for the removal of coefficients containing low-frequency or insignif-
icant high-frequency information. Let us denote Yg,k and Yj,k as the GSMR and
LSMR computed from the wavelet coefficients of the kth subimage. The wavelet
coefficients Wj,k (.) are set to zero according to the following rules:

        Wj.k(·) = 0             for coefficients in subband f                if Yg,k > Yj,k
        retain in subband j for further processing                                             (9.33)
                                                                             1fYg,k 5 Yj,k.

We use the mean and standard deviation, 均,k and (jj .k, from each subband to set the
thresholding and amplification criterion. The rule is stated as follows:

                 10
                            ,       .                ifwj, k
                                                               (.
                                                                    )   I-
                                                                             'j, k+ 2.5 X Jf
    Wj,k (.) =        ial,k]    ..                                                             但34)
                 IaD' L；仄］X빠'k('J
                      abs                            O{nem '"e"
                                                     otherwise.
                        仄］X Wj'k( ')
                      LILj.kJ
After the operations in the wavelet coefficient maps have been completed, we recon-
struct the image using the remaining subband coefficients. The reconstructed images
have a dark background with white spots representing the microcalcifications and
high-frequency speckle noise. To differentiate the microcalcifications and noise, we
use histogram thresholding and dark pixel removal.
     248        DIGITAL SIGNAL PROCESSING APPLICATIONS

     9.9.5      Histogram Thresholding and Dark Pixel Removal
     Since the reconstructed images also contain information that is not relevant to the
     microcalcifications, we need to filter out this erroneous information. The histogram
      뇨eshold requires the peak value of the histogram of a given gray scale g1玘ak1 We
     formulate the following thresholdi唯 rule:

                        vr (X, y) r0, ifvr (x, y) <(gpe毗+ l) +0.5 X
                                                                                                       (9.35)
                        vr (x, y) rem缸n unchanged for further processin

where crZ and /4 are the standard deviation and mean obtained from all nonzero
(nz; pixeis in me reconstructea images. and vr (x. v) is me valUe ot me Ix. v)tli
pixei in me reconstructea image. Alter tins sten. me LAD a으ontiim adds the two
images together in a spatially coherent tasluon to torm a composite image in which
all microcalcification information is contained.
    We now refer back to the origi洌 image. Since the pixel intensity from the micro-
calcification is greater than 137 in an 8-bit (256 levels) linear gray scale, we make
use of this information to formulate a dark pixel removal threshold as follows:

               Vr（兀 y) = 0                      ifVr (X, y) =0
               Vr (X, y) = 0                    if Vr
                                                    （工，    尹0 and
                                                          y)            u  5 ／妃r뇨＋0.5 >< (y0띵
                                                                                （工，       y)
           Vr（工nz, Yn之） = Vr（工， Y)              11 Vr（兀 Y) 尹 0 and u（工， y) > 尸org + 0.5 )< aorg,
                                                                                                       (9.36)
                                                                                                       /i)



 where /iorg and Oorg are the mean and standard deviations obtained using nonzero
pixels in the original input mammogram and u(x, y) is the pixel value of the (x, y)th
pixel in the original image.
    After the dark pixels are set to zero, p毗ntial 耐crocalcification regions (PMRs)
are identified in the enhanced image. The nonzero pixel locations indicate potential
sites of microcalcifications. These sites are then made the cent中rs of 5 x 5 pixel
PMRs. Etch of these PMRs must go through a CFAR-like detector to reduce the
number of PMRs to a manageable level. The CFAR acts like a probabilistic discrim-
inator. The PMRs with high probabilities are retained for further 4nalysis. Hence the
5 x 5 pixel region acts like a window through which an adapti中e rule is set up to
determine its probability as a microcalification. To evaluate the C恥R threshold, one
needs the mean and standard deviation from the PMR, an a prior! probability distri-
bution, and a desired false alarm rate. The detailed theory of CFAR is beyond the
scope of this book; interested readers are referred to [17].


9.    9.   6   Parametric ART2 Cl    .usterin
                                                    .g         .   .m       ,         .        .   .     ,   ,,,




I ne suspicious regions are rormea oy using .AK.! (aaaptive .resf)nance tfleory L>. j)
witu a viguance.lacror, Pu, or 乙그 pixels, in mis exampie appilcaion, we cnoose tne
searcn region ro oe an area corresponaing to i cm x 1 cm, wnicn flas approximately

恥押，出乷鉀，蠶器們斗낱，
            ：幣， 堵뺨甲,' 쌉，嶝，“二
                                      入4ULTICAR뫼ER COMMUF미CATION SYSTE人4S            249




              FIGURE 9.29 Clusters detected in a segmented mammogram.


microcalcifications whose individual size must not exceed 5 x 5 pixels. If an initial
cluster does not meet this criterion, it is declared a false positive (FP) cluster and
removed from the list of suspicious regions.


9.9.7   Results

 We have applied this CAD algorithm to 322 mammo얍ams obtained from the MIAS
MiniMammographic Database of England. We found 150 truly suspicious regions
 and 1834 false alarms with 37 undeterminable regions. When we compare the re-
 suits from the algorithm with the biopsy results (which came with the data set), all 31
 true positives (TPs) were correctly recognized, with one false negative (FN). There
 were 119 false positives (FPs). In terms of sensitivity, the CAD algorithm achieved
between 87 to 97 percent accuracy. In terms of the number of FPs, it attains 0.35 to
5 per image, with 0.04 to 0.26 FN per image. These results compare favorably with
respect to results from other CAD algorithms as well as statistics from the radio-
logical community. An original mammogram and the algorithm output of the same
mammogram are shown in Figures 9.29 and 9.30.


9.10    MULTICARRIER COMMUNICATION SYSTEMS

Multicarrier modulation is the principle of transmitting data by dividing the data
stream into several parallel bit streams, each of which has a much lower bit rate.
250     DIGITAL SIGNAL PROCESSING APPLICATIONS




           FIGURE 9.30 Comparison of clusters detected with a true positive.


Each of these substreams modulates an individual carrier. Figur申 9.31 shows the
bl어：k diagram of the transmitter of a multicarrier communication system (MCCS).
A serial-to-par키lel buffer se얍llents the information sequences into frames of N1
bits. The N1 bits in each frame are parsed into M groups, where the ith group is
assigned n1 bits so that                                            1
                                   M-1
                                   ＞二
                                   i=0
                                         ni   =   Nf.                          (9.37)


It is convenient to view the multicarrier modulation as having M iadependent chan-
nels, each operating at the same symb이 rate 1/ T. The data in each channel are
modulated by a different subcarrier. We denote the signal input to the subchannels
by S1, i = 0. .. ..M - 1. To modulate the M subcarriers, we use an orthogonal basis
4:' = ｛中｝{｛玉lsuch that

                                  仲m, 仇） = E8m,t.

9.10.1 OFDM Multicarrier Communication Systems
Orthogonal frequency-division multiplexing (OFDM) is a speci4l form of MCCS
with densely spaced subcarriers and overlapping spectra. It abandons the use of
steep bandpass filters that completely separate the spectra of individual subcarriers.
Instead, OFDM time-domain waveforms 게e chosen such that mutual orthogonal-
                                                     八4UUICARRIER COM入4UNICA기ON SYSTE人IS                         251




                                            Pulse-Shaping Filter 1
                                            cos(wt)[u(t) - u(t - T0)]




                                X2(k)
                                        >
  X (k)       Serial
                                            cos(2w1)Eu(t)卜 u(t - T0)]                                           s(t)
                to                                                                          Summation
              Parallel

                                                           i
                                                           1




                               XN(k)        Pulse-Shaping Filter N                 SN (t)
                                    >                                                   >
                                            cos(Nwt)[u(t) - u(t - T0)]




                                                     (a)
            Matched-Filter 1
                                                삔少 力（kT0 + T) Decision                      Y1(k).
            cos（口片）[a (t) - u(t    凡）]               r ;= 尺T0 + T




r (t)
        +
            Matched-Filter 2
            cos(2w1)fu(t) - u(t - T0)]
                                                y三
                                                     9/Y       y2   (kTo+
                                                                            T)   Decision
                                                                                            Y2(k)
                                                                                                     Parallel
                                                     i == 尺／[) + T                                     to
                                                                                                     Serial
                            1
                            1
                            1
                            1
                            1




            Matched-Filter N
            cos (Nwt)[u(t) - u(f - T0) ]
                                              므9/ YN(kTO+ T) Decision                       蜘 （k)
                                                                                                >
                                                     t = KT0 + T




                                                     (b)

        FIGURE 9.31      A multicarrier communication system: (a) transmitter, (b) receiver.
252      DIC기TAL 引GNAL P烈）CESSII니G APPLICATIONS


ity is ensured even though subcarrier spectra may overlap. OFDM is more robust
against time-domain impulse interference, due to its long symbol tiklle, which tends
to average out 岫 effects. 아；   DM 없小carriers n刈 lose their mutua如rthogonality if
high-frequency errors occur in the channel. As shown in Figure 941, the operating
principle is simple. The data are transmitted on several subcarrier. The spectra of
the subcarriers may overlap, but the mutual orthogonality is ensured These subcarri-
ers are summed together and 甘ansmitted over the channel. On the r印eiver end of the
channel, the signal received is sent in parallel to the matched filters 1n each subchan-
nel. The output of the matched filter is sampled before the decisio is made on the
signal. In general, each subchannel uses the binary phase-shift key1(BPSK) scheme
[18] to represent the signal.                                           i
    When the channel behaves well and does not introduce frequeny dispersion, the
bit error rate (Pe) is very small. The imperfection may be due to noise in the chan-
nel. On the other hand, when frequency dispersion is present due to time variation
of the channel par町leter, P increases. Phase jitters and receiver frequency offsets
introduce interchannel interferences that degrade the 凡.


9.10.2    Wavelet Packet-Based MCCS
I始tead of the sine or cosine functions used in the OFDM, WP-based MCCS uses dif-
ferent wavelet packets as the time-domain waveforms. If the approximation function
砂 generates an orthonormal set in the L2 space, the correspondihg wavelet pack-
ets are guaranteed to be orthogonal. The subcarriers are now wa＼才elet packets, and
the matched filters in the receiver are designed accordingly (see Fi뇽ure 9.32). Since
there are a large number of wavelet packets to be chosen for th4 subcarriers, our
experiment chooses those whose spectra are very close to those of the OFDM. Un-
der this condition, we can m毗：e a fair comparison between the results of these two
systems.
    The curves in Figure 9.33 represent the 尸e verse symbols per seond. Without any
 frequency offsets, all system performances are very close to being the same. When
the frequency offset is 10 percent, the wavelet packet system perfoif毗 slightly better
than the O日：)M. When we stress the system by allowing 25 perc4nt offset, the WP
 system works far better than the OFDM. In particular, the Daubech1es D3 orthogonal
WP system seems to be the best. Comparing the spectra of the sibcarriers in both
 systems, they are very similar. However, there appears to be an optirnal set of wavelet
packets through which the system produces the best performance under a highly
 stressed system. An iterative and an analytical approach are being investigated.


9.11     THREE-DIMEN引ONAL 入4E［기CAL I人fAGE V巧UALIZATION

Medical image visualization is becoming increasingly popular for甘lanning treatment
and surge．텍 Medical쁘ages captured by van毗 in쁘艸．ents a甲的-dimensional
gra．艸ye! signal요 的기 image.recol好tructeQ irom. z-ii soc띤艸vi'交빽cn more
inrormanon aoour surraces anu iocaiizauon OJ oojects in a 于li space. inc meuicai
                                    THREE-D小4EN引ONAL 入iE［기CAL 小lACE 니SUALIZATION                                       253




                                  X1(늬1 삐S心Shapi肥
                                                「ut釘1                          s (t)
                                           WPj/ (t)




                               X2(k)       Pulse-Shaping Filter 2              s2 (t)
                                       >
  X (k)       Serial                                                                    >
                                                                                                                      s(t)
                                           WP2, (t)                                         Summation
               to
              Parallel                                       1
                                                             1
                                                             1
                                                             1
                                                             1




                               XN(k)       Pulse-Shaping Filter N              SN(t)
                                     >
                                           WPN/ (t)




                                                   (a)
            Matched-Filter 1                  수，         /       力（kT0+ T)                        Y1(k)
        今                                                                    Decis如n
            WP1 (T - r)
                                                   t= KT0+ T




        수
            Matched-Filter 2                  으抄才 ）쁘브 2 Decision                                  Y2 (k)
                                                                                                       >   Parallel
r (t)       WP2/ (T - t)                                                                                               s(t)
                                                  r = KT0 + T                                                to
                                                                                                           Serial
                             II
                             1

                             SS




            Matched-Filter N                  므少 YN(k기）+T) Decision
            WPN/ (T - t)
                                                                                            )쁘；
                                                  r = KT0 + T



                                                  (b)
        FIGURE 9.32        A multicanier communication system: (a) transmit妃r, (b) receiver.
254             DIGITAL SIGNAL PROCESSING APPLICATIONS


                                                  P5 vs· 특）/N0
 100




 10口




                           Analysis A f=O
 10-i                      Sim네計ed A 忙0
                           An히ysis A f=0.1斤0
                           Simulated A f=0.1/To
                           Analysis A f=0.25/To
                           Sim네ated 八 f=0.25斤0

                                         4            5          7                    9   10
                                                  Eb小I0 (dB)


FIGURE 9.33 Probability of error vs. signal/noise ratio for the D-3 wavelet packet multi-
carrier communication system for various frequency offsets.




community has increasingly taken advantage of recent advances in communication
and signal processing technology to improve diagnostic accuracy and treatment plan-
fling. Through teleradiology, it is now possible to have surgeons making diagnoses
and plan treatments for a patient who lives at a remote location. This is possible by
transmitting 2-D images of the infected region of the patient and reconstructing the
image in 3-D at a place where a group of experts can make an accurate diagnosis of
the disease. Several problems that have hindered the progress of this work include:



             st。rage requirements.       D data sets occupy huge며emory    and
      storing them for easy retrieval is an important issue.
                                                                             space,
   1.   Large                                3-
   2. 乙7w transmission rate. Channel bandwidths for telephone lines or ISDN
      lines are small, thus slowing down the transmission speed.
   3. 刃w-speed i刃iaRe reconstruction. Rendering algorithms i s complex, and it
      takes time to maneuver these huge sets or aata.
                         THREE-DIMENSIONAL MEDICAL IMAGE VISUALIZATION                  255

    We use a 3-D wavelet decomposition and reconstruction algorithm for compres-
sion of 3-D data sets. For region of interest (ROI) volume compression, the ad-
vantages of using wavelets are that (1) upon reconstruction from a spectral-spatial
localized representation of highly correlated 3-D image data, a more natural and
artifact-free 3-D visualization is produced, even at high compression rates; and (2)
the localized nature of the transform in the space and frequency domains allows for
ROI transmission of data.



9.11.1      Three-Dimensional Wavelets and Algorithms

Similar to the 2-D wavelet, 3-D wavelet decomposition can be performed for discrete
volume data by a filtering operation, as shown in Figure 9.34.
   After a single 3-D level wavelet transform, the volume data would be decomposed
into eight blocks, as shown in Figure 9.35. The 3-D volume can be approximated by



                                                                z
                                                                         J
                                           y           {ak}             C (x,y,z) (LLL)

                                   (aJ
                                                                        J
                 x                                                     미偶y,z) (LLH)



               { 屯｝
                                                                         J
                                                                        d2(x,y,z) (LHL)

                                  { t\ }
                                                                       J
                                                       { bk }          미仇y,기 (LHH)
 J+i
c (x,y.z)



                                                                         J
                                                      I ak J            d4(x,y,z) (HLL)

                                 { aj
                                                                        J
                                                      { b)             d5(x,y.z) (HLH)



               {b I

                                                                        J
                                                                       d6(x,y,z) (HIlL)

                                 { t\ }

                                                                       d (x,y.
                                                                                 z)
                                                                                      (HHH)

FIGURE 9.34 Block diagram of a three-dimensional hierarchical wavelet decomposition
algorithm.
256      DIGITAL SIGNAL PROCESSING APPLICATIONS




                                                          111                 珏LL




>\
                                                          LHL             HI-IL




                     x



         FIGURE 9.35 Labeling wavelet coefficient sets in eight different octants.


using
                                  Z
                                  m                                               /Mm
                仁
                少        VJ
                              卞             沖        寸    y        中
                                                                   7J
                                                                    今乙   口（   中

                                                                                   1)   ,




where 中（工， y, 乙） = 中（工）中（y）中（z) and a二,m,1 is the scaling function coefficient. We
can add the details by adding the 3-D wavelet functions at the resolution 2-'

                    ＞二 [（너）n.m.／砂l(2j! - 兀 2y + m, 2j - /)
                    n.m.I


                         +（며뇨,rn.／少km- 兀 갇 - m그J- /)
                         + 佃机 .m.!砂3 (2j工 H 兀 2y 小 m, 2j 니）

                         + 叫) n.rn.／少4(2뇨 - n, 2y - m, 2 -1)

                         + （岫n.m.／砂5 (2／工 - n, 2y - m, 刃 -1)

                         + (W)n,rn,i砂6 (2X - n, 2 ' - m, 2 - 1)

                         + （며）n.m.／砂7 (2jX 中 n, 2y - 刃i, 2/ 小 /)],                          (9.38)

where w{ through w4 are the wavelet coefficients. We can reconstruct the original
3-D function volume to any refinement by adding some of the details listed above.


9.11.2    Rendering Techniques
Rendering is the process of generating images using computers. In data visualization,
our goal is to transform numerical data into graphical data, or graphical primitives,
                            THREE-D小4ENSIONAL M日긔GL 小4AGE VISUALIZA지ON                   257

  for rende由g. Traditional tech血ques assumed that when an object was rendered, the
  surfaces and their interactions with light were viewed. However, com끄［lon objects
 such as clouds and fog are translucent and scatter light that passes through them.
 Therefore, for proper rendering, we need to consider the changing properties inside
 the object.
     When we render an object using surface rendering techniques, we m어iel the ob-
 ject mathematically with a surface description such as points, lines, triangles, poly-
 gons, or surface splines. The interior of the object is not described or is represented
 only implicitly by the surface representation.
     One of the key developments in volume visualization of scalar data was the
 marching cubes 키gorithm of Lorenson and Cline [191. The basic assumption of this
 technique and its higher-dimension counterpa式S is that a contour can pass through
 a cell in only a finite number of ways. A case table is constructed that enumerates
 all possible topological states of a cell given combinations of scalar values at the
 cell points. The number of topological states depends on the number of cell vertices
and the number of inside-outside relationships a vertex can have with respect to
the contour value. A vertex is considered to be inside a contour if its scalar value is
larger than the scalar value of the contour line. Vertices with scalar values less than
the contour value a七 said to be outside the contour. For example, if a cell has four
vertices and each vertex can be either outside or inside the contour, there are 24 = 16
possible ways that contour lines can pass through the cell. There are 16 combinations
for a square cell, but these can be reduced to four cases by utilizing symmetry (see
Figure 9.36). Once the proper case is selected, the location of the contour-cell edge
intersection can be calculated using interpolation. The algorithm processes a cell and
then moves or기1arches to the next cell. After all cells are visited, the contour will be
complete. (Note: The dashed line in Figure 9.36 in出cates a contouring ambiguity.)
    In summary, the marching algorithm proceeds as follows:


   1. Select a cell.
   2. Calculate the inside-outside state of each vertex of the cell.
   3. Create an index by storing the binary state of each vertex in a separate bit.




                          0 = less than iso-value of interest

                          1 = greater than is아va뇨e 可 in把rest

FIGURE 9.36 Inside-     outside relationship of a square whose vertices have numerical value
either higher or lower than a set threshold.
258            DIGITAL SIGNAL PROCESSING APPLICATIONS




                                                        口口II I            I1111

                                                        口
                                                        1
                                                          口II1111
                                                           II11口
                                                          U I II I
                                                          1               I11口
                             (a)
                                                                         (b1)
               FIGURE 9.37 Region of intemst: (a) in original image, (b) in s肛bimages.



    4.     the
         Use
                      to
                     index      the top아ogical state of the cell ina ase table.
                                   look
                                          up
    D. Uaicuiaie Inc contour locations for each edge in mne case tabl仁.


9.11.3          Region of Interest
Due to the localized nature of wavelets in freuuencv and space domains. ROI re-
nnement can De acnievea Dy adding details oniy in tfle regions required. 1-'igure 9.3/
shows the ROI in the original image and in the wavelet domain for two levels of
aecom刃sinon. I nus waveiets can De a useful tool for comDressionL as tne ima으e can
be approximated by first reconstructmg the lowpass coefficients, 4nd the detail can
比 restored to the ROt solely by transmitting the appropriate 川ghpass coefficients
in the ROt. The results of 仕1is volume rendering using a 3-D wavelet algorithm are
shown in Figures 9.38 to 9.40.


9.11.4          Summary
The 3-D wavelet decomposition and reconstruction algorithm is us4ful for 3-D image
visualization. It improves the speed of the rendering algorithm and achieves data
compression by using an ROI approach.


9.12           COMPUTER PROGRAMS

9.12.1          Two-Dimensional Wavelet Algorithms
돔
% PR0GRAM a1gorithm2D.m
8
                                                      COMPUTER PROGRAMS          259




FIGURE 9.38 Multiresolution rendering of 93 slices of 64 x 64, 8-bit image using iso-
surfacing with the marching cubes algorithm.




 FIGURE 9.39 Low-resolution rendering except for the ROI(nose portion of the head).
260   DIGITAL SIGNAL PROCESSING APPLICATIONS




FIGURE 9.40   Low-resolution rendering except for the ROI (left-side ear portion of the
head.)




% Decomposes and reconstructs a 256x256 image using
% Daubechies ' wavelet (m = 2) . The initial coefficients
돔 are 七aken as 七he func亡1（그n values themselves.

돔 tes七 ima<犯

picture = 256 * ones (256) ;
for i = 1: 256
  picture (i, i) = 0;
  picture (i, 257-i) = 0;
end

image (picture)
title) 'Original    Image ' )

老 Decomposi亡ion and recons七ruc匕ion fil七ers

g0 = [0. 68301; 1. 18301; 0. 31699; -0. 18301] ;
k = [0; 1; 2; 3] ;
gl = flipud (go) . 士卜1) . 八k;
h0 = flipud (go) I 2;
hl = flipud (gl) / 2;
                                                   COMPUTER PROGRAMS   261

 % Decomposition process

 왐 First   level   dec이npo Si上ic끄l

for k 'l: 256
    s= [0; 0; picture ( : ,k) ; 0; 0] ;
    x=conv (s, h0) ;
   a=x (l :2: length (川) ;     %dowiisa四ling
   x=conv (s, hl) ;
   w=x (l: 2: length (x) ) ;   %downsmapling
   C (: ,k) =[a; wi;
end

for k=1: 256+8
    s=r0t90 ([ 0 0 C (k, : ) 0 0] ,3) ;
    x=conv (s, h0) ;
   a=x ( 1 : 2 : leng나I ( 川 ) ;  %downs帥pling
   x=conv (s, hl) ;
   w＝그＜(l: 2: leng七t니川 ) ;       돔downsrnapl ing
   CC (k, : ) =rot90 ( [ a; w] ) ;
end

LL=CC (l: 132, l: 132) ;
HL=CC (133: 264, l: 132) ;
LH=CC (1: 132 , 133 :264) ;
HN=CC (133: 264, 133: 264) ;



figure (2)

 axes ( 'position ' , [0. 1   0. 5 0. 3 0. 3] )
 image (LL)
 亡a上le ( ' LL ' )
axes ( 'position ' , [0. 5    0. 5 0. 3 0. 3] )
image (LH)
 title ( 'LH')
axes ( 'posi上如1l ' [0. 1      0. 1 0. 3 0. 3J )
image (HL)
七a上le ( ' HL ' )
axes ( 'position ' , [0. 5    0. 1 0. 3 0. 3J )
image (HH)
七 a上le ( 'NH ' )

clear C
clear CC

% Second level     decompostion

for k=l: 132
262      DIGITAL SIGNAL PROCESSING APPLICATIONS


   s=LL (: r k) ;
   x=conv (s, h0) ;
   a=x (1: 2: leng나l (x) ) ;     %downsampling
   x=conv (s, hl) ;
   w=x (l: 2: length (x) ) ;     %downsmapling
   C ( : ,k) =[a; WI ;
end

for k=1: 128+8
   s=r0t90 (C (k, : ) ,3) ;
   x=conv (s, h0) ;
   a=x (l: 2: length (xfl;     %downs帥lpling
   x=conv (s, hl) ;
   w=x (1: 2: length (xH;      %downsmapling
   CC (k, :) =r0t90 ( [ a; WI) ;
end;

LL_LL=CC (1: 68, 1: 68) ;
HL_LL=CC ( 69 : 136, 1: 68 ) ;
LH_LL=CC (1: 68, 69: 136) ;
HH_LL=CC (69:136, 69: 136) ;
clear C
clear CC

% Reconstruction Process

智 Secon（크 level     recons七ruction

s= [LL_LL LH_LL; HL_LL HH_LL I;
for krrl: 136
    x= zeros (136, 1) ;
    x (l: 2:136) =rot90 (s (k, l: 68) ,3) ;
    y= zeros (136, l) ;
    y (l: 2: 136) rrOt90 (s (k, 69: 136) ,3) ;

   x=conv (x, g0) +conv (y, gl) ;
   C (k, : ) =r0t90 似 ( 4 : leng匕1（川 -4) ) ;
end

s=C;
clear （二

for k=l: 132
   x= zeros (136, l) ;
   x (l: 2: 136) =s (l: 68, k) ;
   y= zeros (136, l) ;
   y (l: 2: 136) =s (69:136, k) ;

      x=conv (x, g0H-conv (y, gl) ;
                                                  COMPUTER PROGRAMS   263


   C ( : ,k) =x (4: length (x) -4) ;
end
LL_rec=C;
clear C

% First      level   reconstruction

s= [LL_rec LH; HL HH] ;
for k=l: 264
    x= zeros (264, l) ;
    x (l: 2: 264) =rot90 (s (k, l: 132) ,3) ;
    y= zeros (264, 1) ;
    y (l: 2: 264) =ro七90 (s (k, 133: 264) ,3) ;
    x=conv (x, g0) +conv (y, gl) ;
    C (k, :)=rot90 佯 (4 :ler珂th（川 小4) );
end

s =C;
clear    C

for krl: 260
   x= zeros (264 r1) ;
   x (l: 2: 264) =s (l: 132, k) ;
   y= zeros (264, 1) ;
     y (l: 2: 264) =s (133: 264, k) ;

   x=conv (x, g0) +conv (y, gl) ;
   C (: ,k) =x (4: length (x) -4) ;
end

picture_ rec=C (3: 258, 3: 258) ;

figure (3)
image (picture_ rec)
title ( 'Reconstructed Image ' )


9.12.2    Wavelet Packets Algorithms
害
% PR0GRJl4 waveletpacket.m
돔
뚬 Wavelet packe七 decomposi．亡ion and recons匕ruc亡ion (：汪 a
% function using Daubechies ' wavelet (m = 2) . The initial
% coefficients are taken as the function values themselves.
묻

毛 Signal

vl   = 100;              % frequency
264         DIGITAL SIGNAL PROCESSING APPLICATIONS


v2 = 200;
v3 = 400;
r = 1000;                 %sampiing rate




k 七 S
        = 1: 100;
        = (k- i) / r;
        = sin (2女p1士＼11士七） + sin (2出pi出＼12出亡） + sin (2出pi出＼13女t) ;

毛 Decot따＞Os'上1（丑i and recons七ruction filters

g0 = [0. 68301; 1. 18301; 0. 31699; -0. 18301) ;
k = [0; 1; 2; 31 ;
gi = flipud (go) . 士卜1) . 八k;
h0 = flipud (go) / 2;
hi = fiipud (gi) / 2;

% Decomposition process

돔 Firs七 level        dec（끄uposition

x=conv (s, h0) ;
a=x (1: 2: length (x) ) ; %downsampiing
x=conv (s, hl) ;
w=x (l: 2: length (xfl;   %downsmapiing

%second level decomposition
x=conv (a,h0) ;
aa=x (i: 2: iength (x) ) ;
x=conv (a, hi) ;
aw=x (l: 2: length (x) ) ;

x=conv (w, g0) ;
wa=x ( 1 : 2 : len드作h 佯） ) ;
x=conv (w, gi) ;
ww=x (l: 2: length (x) ) ;

% Reconstruction process

% Second level         reconstruction

x= zeros (2*iength (aa) ,i) ;
x (l: 2: 2*iength (aa) ) =aa (l: length (aafl;
y=zeros (2*length (aw) ,i) ;
y (l: 2: 2*length (aw) ) =aw (l: iength (aw) ) ;
x=conv (x, g0) +conv (y, gl) ;
a_rec＝그＜(4 : leng나l（川 -4 ) ;

x= zeros (2*iength (wa) ,l) ;
x (i: 2: 2* length (aw) )=wa (l: length (wa) ) ;
                                                                         REFERENCES        265

y=zeros (2*length (尸w) ,l) ;
y (l: 2: 2*length (ww) )=ww (l: length (ww) );
x=conv (x, h0) +conv (y,hl) ;
w_rec＝그＜(4: leng七l니川 -4) ;

% First     level reconstruction

y=zeros（깐leng나l (W小rec) , 1) ;
y (l: 2: 2*length (w_rec) )=w_rec (l: length (w_rec) );
x=zeros (2*length (a_rec) , 1) ;
x (l: 2:2*length (a_rec) )=a_rec;

x=conv (x, gO) ;
y=conv (y, gl) ;
y=x (1:length (y) )+y;
s_rec=y (4 : length (y) -4) ;



REFERENCES

  1. I. Daubechies, Ten Lectures on Wavelets, CBMS-NSF Set. App!. Math. 61. Philadelphia:
      SIAM, 1992, 326 pp.
  2. R. R. Coifman and M. V. Wickerhauser, "Entropy-based algorithmls for best basis selec-
      tiOfl,' ' 旭F百 가ans. Info刀月． The이y, 38(2), pp. 713-718, 1992.
 3. B. Vidakovi6 and P. Muller, Wavelets for Kids. Durham, N.C.: Institute of Statistics and
      Decision Sciences, Duke University, 1991.
 4. M. Wang and A. K. Chan, "Wave!et-packet-based time-frequency distribution and its
      application to radar imaging," mt. J. Numer Model.: Electron. Networks Devices Fields,
      11巾p. 기-40, 1998.
 5. H. C. Choe, Ph.D. dissertation, Texas A&M University, College Station, Texas, 1997.
 6. D. K. Ku and F. B. Shin, Pattern Recognition and Prediction with Applications to Signal
      Characterization. Wo어bury, N.뇨 American Institute of Physics Press, 1996.
 7. T. F. Yu, Ph.D. dissertation, Texas A&M University, College Station, Texas, 1997.
 8. M. Rabbani and P. W. Jones, Digital Im口ge Compression Techniques, Vol 1T7. Belling-
     ham, Wash.: SPIE Press, 1991.
 9. J. M. Shapiro, "Embedded image coding using zero甘ees of wavelet coe卄cients," IEEE
      Trans. Signal Process., 41(12), pp. 3445-3462, 1993.
10. A. Said and W. A. Pearlman, "Image compression using a spatial-orientation tree," IEEE
     mt. Symp. on Circuit and Systems, pp. 279-282, 1993.
11. A. Said and W. A. Peariman, "A new, fast, and efficient image codec based on set parti-
     tioning in hierarchical trees," i万E Trans. Circuits Syst. 玩deo Technol., 6, pp. 243그50,
     1996.
12. A. Said, "An image multiresolution representation for lossless and lossy compression:'
    IEEE Trans. i刃age Process., 5, pp. 1303-1310, 1996.
13. N. W. Lin, D. K. Shin, T F Yu, J. S. Liu, and A. K. Chan, "The generalized self-sim
                                                                                        ilarity
     tree coder," Technic口l Repo斤. College Station, Texas: Wavelet Research Laboratoty,
    Texas A&M University, 1996.
266             DIGITAL SIGNAL PROCESSING APPLICATIONS


14. M. E. Peters, D. R. Voegeli, and K. A. Scanlan, in Brea缸 Imaging, R. L. Eisenberg (Ed.),
    New York: Ch玎chill Livingstone, 1989.
15. R. N. Strickland and H. I. Hahn, "Wavelet transforms for detecting mi rocalcification in
    mammo으rams." IEEE Trans. Med. Imacing. 15. DD. 218-229, 1996.
16.   D.   A.     McCandless,
                                S.   K.
                                          R。
                                                  ffmeister,
                                               gers,   J.   W.   H。
                                                                      D.   W.       and
                                                                                Ruck,   寸   ‘.   A.   Raines,
    B. W. Suter, "Wavelet detection of clustered microcalcification," Proc. SPIE Wavelel
    肉叩乙 2762, pp. 388-399, 1996.
17. P. P. Gandhi and S. A. Kassani, 'Analysis of CFAR processors in nonh(
    ground," IEEE Trans. Aemsp. Electron. Syst., 24(4), pp. 427-445, 1988.
18. J. G. Proakis and M. Salehi, Com,nunicat加n Systems Engineering, Upper Saddle River,
    N.J.: Prentice Hall, 1994.
19. W. E. Lorenson and H. E. Clime, "Marching cubes: A high resolutior
    struction algorithm," Comput. Graphics, 21(4), pp. 163-169, 1987.
CHAPTER TEN




Wavelets in Boundary
Value Problems

All of the applications discussed so far deal with processing a given function (signal,
image, etc.) in the time, frequency, and time-frequency domains. We have seen that
wavelet-based time-scale analysis of a function can provide important additional in-
formation that cannot be obtained by either time- or frequency-domain analyses.
There is another class of problems that we quite often come across that involve
solving boundary value problems (BVP). In BVPs functions are not known explic-
itly; some of their properties along with function values are known at a set of cer-
tarn points in the domain of interest. In this chapter we discuss the applications of
wavelets in solving such problems.
    Much of the phenomena studied in electrical engineering can be described math-
ematically by second order partial differential equations (PDE). Some examples of
PDEs are the Laplace, Poisson, Helmholtz, and the Schrodinger equations. Each of
these equations may be solved analytically for some, but not for all cases of inter-
est. These PDEs can often be converted to integral equations. One of the attractive
features of integral equations is that boundary conditions are built-in and therefore
do not have to be applied externally [1]. Mathematical questions of existence and
uniqueness of a solution may be handled with more ease with the integral form.
    Either approach-differential or integral equations-to represent a physical phe-
nomenon cai小ev妃＼wed in terms of an 아壯ator operati雎 on a叩nknown function in
order to produce a known function. In this chapter we deal with the linear operators.
The linear operator equation is converted to a system of linear equations with the help
of a set of complete bases which is then solved for the unknown coefficients. The fi-
nite element and finite difference techniques used to solve PDEs result in sparse and
banded matrices, whereas integral equations almost always lead to a dense matrix; an
exception being the case when the basis functions, chosen to represent the unknown
functions, happen to be the eigen functions of the operator.
    Two of the main properties of wavelets vis-a-vis bound缸y value problems are
their hierarchical nature and the vanishing moments properties. Because of their hi-

                                                                                  267
 268      WAVELETS IN BOUNDARY VALUE PROBLEMS

erarchical (multi肥solution) nature, wavelets at different resolutions are interrelated,
 a property that makes them suitable candidates for multigrid-type aiethods in solv-
ing PDEs. On the other hand, the vanishing moment property by virtue of which
wavelets, when integrated against a function of certain order, make the integral zero,
is attractive in sparsifying a dense matrix generated by an integral equation.
    A complete exposition of the application of wavelets to integral and differential
equations is beyond the scope of 曲s chapter. Our objective is to provide the readers
with some preliminary theory and results on the application of wavlets to boundary
value problems and give references where more details may be fcun4. Since most
often, in electrical engineering problems, we encounter integral e4uations, we will
emphasize their solutions using wavelets. We give a few exa卿les f commonly oc-
curring integral equations. The first and the most important step in solving integral
equations is to transform them into a set of linear equations. Both conventional and
wavelet-based meth어is in generating matrix equations are discussed. Both the meth-
ods fall under the general categories of meth어 of moments (MoM) We will call the
meth에 with conventional bases (pulse, triangular, piecewise sinusd)id, etc.) conven-
加nalMo)%小while theme由odw沚i wavelet bases will be referred to鈿 叩avelet M川4.
Some numerical results are presented which illustrate the advantag4s of the wavelet-
based technique. We also discuss wavelets on a bounded interval. Some of the tech-
niques applied to solving integral equations are useful for differeijtial equations as
well. At the end of the chapter we describe briefly the applicatiois of wavelets in
PDEs and provide references where readers can find further information.


10.1    iNTEGRAl. EQUATIONS

Consider the following first-kind integral equation


                                /（工／)r （工，工／) dx' = g（工）,                        (10.1)
                           fb
 where f is the unknown function and the kernel K and the funct on g are known.
가血 equation, depending on the ke毗1 and 奴 lin丘侄 of integrati毗 is referred to by
小卄erent names, such as F노edholi瓦 Volterra, convo加tion, and the Weiner-Hopf血把．
gral equation. Such integral equations appear frequently in practice [2]; for instance,
in inverse problems in which the objective is to reconstruct the function f from a
set of known data represented in the functional form of g, one en다）unters first-kind
integral equations. In some electromagnetic scattering problems, d4scussed next, the
current distribution on the metallic surface is related to the incident field in the form
of an integral equation of type (10.1) with Green's function as the kernel. Observe
that solving for f is equivalent to finding the inverse transform ofg with respect to
the kernel K; in particular, if K(x, x') = r片i ' , then f is nothiig but the inverse
Fourier transform of g. We assume that (10.1) has a unique solution. Although we
discuss solutions of first-kind integral equations only, the method cn be extended to
second-kind [3, 4] and higher-dimension integral equations [5] wi寸h little additional
work.
                                                                                          INTEGRAL EQUATIONS         269

   As an example of (10.1), consider that an infinitely long metallic cylinder is il-
luminated by a TM (transverse magnetic) plane wave as shown in Figure 10.1. An
integral equation relating the surface current distribution and the incident field can
be formulated by enforcing the boundary condition

                元 )< 月（p) = 介 )< [Ei(p) + 且（P)] = 0,                                                     /) E S,   (10.2)

where E, E, and ES are the total, incident, and scattered electric fields, respectively.
The surface of the cylinder is represented by S. For the TM plane wave incident field,

                   互i =z 하， Hi =i 川， and                                                   J ＝乏 Jsz,               (10.3)

where, as usual, Hi is the incident magnetic field and J is the induced electric current
on the surface of the cylinder. This electric current is related to the incident field and
the Green's function by an integral equation,



                          Jw仰            j (t G(t, dl
                                             Jz         ')             t   ')     ' =     E (t),                   (10.4)
＼入／
  here

                                                                                                                   (10.5)
                       G(t,     t   ')   ＝        亡日｛        "   ［幻巾            （()   -   ,(
                                                                                               (   '기］   ,




                                                                                      H力 t


     z.               x
FIGURE 10.1 Cross section of an infinitely long metallic cylinder illuminated by a TM
plane wave.
270                          WAVELETS IN BOUNDARY VALUE PROBLEMS

with k0 = 27r/Ao, and 入0 denoting the wavelength. E is the z-4omponent of the
r_ _,,___ 4 _i_ _ 4 , _ n_ i,                       1 .            (2) ·              .1                            i   i_ ,   ,              TI                   _ I_ _i r_ ___ 1! _J_ r _ 1           fl TI
inciueilt   elecuTic acm                         anu i,
                                                              l0       - .   is me seconu-KJnu                                     ,rianKei
                                                                                                                                                                           iuncuon.     ui oruer         v. Here,


므：e contour or integration nas oeen parainetenzeo wan respect to me cnoru lengtH.
Inc nem component nj can oe expressea as

                                          月批）= E0 exp[jko（工（t) cos吻 +y (t) sin吻）],                                                                                                                         (10.6)

where 吻 is the angle of incidence.
.   .   .lt   i        is ciear mat (1O.4) is or me form.n O1 equation (1O.1) our oDect1ve is to solve
                        .                                                         .                                                           .                                  .




(1O. ror me unKnown current clistrioution J之 and compute me raar cross section
                  4)             .



Iist/DJ; Inc latter oeing given oy


                                                    RCS                           ,             IE{ I2                       喘k긍 .,, . 2
                                                    小1 = 凡op二；=; = 1=＝놔 나油I--,                                                                                                                             (10.7)
                                                    人0      1e才』    ojr


where no = ＼厄고瓦 is 毗no帥 constant and

                                     小／
                                            ,exp［如                                     《   '）
                                                                                                 啣日t                               ')             sin0)                          ]J (t dt')
                                                                                                                                                                                              '.           (10.8)
                                             C
    Scattering from a thin perfectly conducting strip, as shown in Figure 10.2a, gives
rise to an equation similar to (10.4). For this case we have

                                                              ph
                                                             I   , , , . n,  F  i-
                                                             / . 六y口 八八乙乙 月i乙 = 乙y（乙J,
                                                                                                                    '                                                        .

                                                                                                                                                                                                           (10.9)
                                                                                                      _     _   F       i_
                                                                                                                                                              i.
                                                         .,   -n
where G(乙 z') is given by (10.5).
  As a final example, consider scattering from a thin wire as shown in Figure 10.2b.
Here the current on the wire and the incident field are related to each other as
                                                             ft
                                                        j,         I   (z
                                                                             ')
                                                                                      K,        (z,       z') dz ' =                          -           E
                                                                                                                                                                   '
                                                                                                                                                                                                         (10.10)
                                                   J-          1                                                                                                       (z)           ,
where the kernel K功 is given by


                  Kw(z, z') = '47rJWE0
                              . l " 吹jkoR)
                                       !d '
                                                  R) x (2小낢나k和2R21
                                            1(l+ik。
                                            L                 -  J




                            可（z) = 万osin 0 exp(jko乙 c050).

This kernel is obtained by interchanging integration and differe'itiation in the in-
tegrodifferential form of Pocklington's equation and by using tie reduced kernel
distance R = [a2 + (z - z')2]112, where a is the radius of the wire [6].
   The first step in solving any integral or differential equation is to convert these into
a matrix equation which is then solved for the unknown coefficiens.             us rewrite                                                                                                         Let
                                                                     INTEGRAL EQUATIONS      271




                                                  x



                                                                 -


                                                                         z

                                            (a)
                                          k1퓌
                                            2a

                                            (b)
FIGURE 10.2 (a) Thin half-wavelength-long metallic strip illuminated by a TM wave; (b)
Thin wire of length 入/2 and thickness A/1000 illuminated by a plane wave.




(10.1) as LKI = g, where



                          뇨／
                          LKf=  =   /,b   j f (x      ')K(x, x') dx '.                    (10.13)

The goal is to transform equation (10.1) to a matrix equation

                                            Ac= b,                                        (10.14)

where A is a two-dimensional matrix, sometimes referred to as impedance matrix, c
is the column vector of unknown coefficients, and b is another column vector related
to g. Computation time depends largely upon the way we obtain and solve (10.14).
In the following sections we describe conventional and wavelet basis functions that
are used to represent the unknown function.
 272     WAVELETS IN BOUNDARY VALUE PROBLEMS

 10.2   人4ETHOD OF 人4O人4ENTS

Method of moments [7] is probably the most widely used technique for solving in-
tegral equations in electromagnetics. In conventional MoM, the boundary of inte-
肛ation is approximated by 小scretizing it into many segments. Then the unknown
function is expanded in terms of known basis functions with unknown coefficients.
These bases may be global (entire-domain), extending the entire length [a, b], or
they may be local (subdomain), covering only a small segment of the interval, or a
combination of both. Finally, the resultant equation is tested with the same or differ-
ent functions, resulting in a set of linear equations whose solution gives the unknown
coe玗Ic妃nts.
   The unknown function f (x) can be written as

                                /（工） ＞二
                                      「.
                                       =
                                             n
                                                    A.
                                                         （工）
                                                               ,
                                                                                        (10.15)

where the IA,, I form a comolete set of basis functions. For an exact reoresentation
or j (X) we may neeu an innnite numner or terms in me series anove. However, in
practice, a finite number of terms suffices for a given acceptable error. Substituting
the series representation of f (x) into the original equation (10.1), we get

                                  N
                                 ＞二 C.LKA. 勺 g.                                         (10.16)
                                 n=i
恥r the present如cus如n we assu毗N to be large enough so that如represe
                                                                             nta如n
above is exact. Now by taking, the inner .product of (10.16) with a.set of weighting
junctions or resting junctions tm : m = i, ..., MJ we get a set or 'inear equations

                 N
                ＞二Cn(m, LKAn) = (em, g),                       m = 1, ... , M           (10.17)
                n=1
which can be written in the matrix form as

                                [Amnl[cnl = [bml,                                       (10.18)
where

          Amn = (音m, LKAn),            m = 1, . . . , M,             n = 1, 1. . ., N
           bm = (亨m, g),               m =       1. .. ..M.
    Solution of the matrix equation gives the coefficients {cn} and thereby the so-
lution of the integral equations. Two main choices of the testing lunctions are: (1)
 m (X) = 8(x - Xm), where Xm is a discretization point in the domain, and (2)
亨m（功 = Am（카 In the former case the method is calledpoint m口tc肋섕，whereas the
latter method is known as Galerkin method. Observe that the operator LK in the pre-
ceding paragraphs could be any linear operator-a differential as well as an integral
operator.
                                                        WAVELET TECHNIQUES         273

10.3     WAVELET TECHNIQUES

Conventional bases (local or global), when applied directly to the integral equations,
generally lead to a dense (fully populated) matrix A. As a result, the inversion and
final solution of such a system of linear equations are very time consuming. In later
sections it will be clear why conventional bases give a dense matrix while wavelet
bases produce sparse matrices. Observe that conventional MoM is a single-level ap-
proximation of the unknown function in the sense that the domain of the function
([a, b], for instance), are discretized only once, even if we use nonuniform discretiza-
tion of the domain. On the other hand, wavelet-MoM is inherently multilevel in na-
ture.
   Beylkin et al. [8] first proposed the use of wavelets in sparsifying an integral
equation. Alpert et al. [3] used waveletlike basis functions to solve second-kind in-
tegral equations. In electrical engineering, wavelets have been used to solve integral
equations arising from electromagnetic scattering and transmission line problems
[5,9-23]. In what follows we briefly describe four different ways in which wavelets
have been used in solving integral equations.


10.3.1    Use of Fast Wavelet Algorithm

In this method, the impedance matrix A is obtained via the conventional meth叱
of moments using basis functions such as triangular functions, and then wavelets
a七 used to transform this matrix into a sparse mat奴 [9,10]. Consider a matrix W
formed by wavelets. The transformation of the original MoM impedance matrix into
the new wavelet basis is obtained as

                             WAWT . (VyT)1lC = Wb,                              (10.19)

which can be written as

                                    A1iJ ·ctiJ = b1U,                           (10.20)

where WT represents the transpose of the matrix W. The new set of wavelet trans-
formed linear equations are

                                   A功 = WAWT

                                    cw = (WTy 'c                                (10.21)
                                    b1iJ = Wb.

TF比 5아uti이i vector c is then given by

                              c= WT (WAWT) _IWb.

For orthonormal wavelets WT = WH' and the transformation (10.19) is unitary sim-
ilar. It has been shown in [9, 10] that the impedance ma甘ix A功 is sparse, which re-
duces the inversion time significantly. Discrete wavelet transform (DW기 algorithms
can be used to obtain A功 and finally the s아此on ye야아 C.
274            WAVELETS IN BOUNDARY VALUE PROBLEMS

10.3.2          Direct Application of Wavelets
In another method of annlvin2 wavelets to integral eciuations, wa놔elets are directly
applied; that is, tirst the unknown function is represented as a superposition 01
wavelets at several levels (scales) along with the scaling function a'
before using Galerkin's method described previously.
   Let us expand the unknown function f in (10.1) in terms of the scaling functions
and wavelets as
                                                                                   尺（s)                                          K (s0)

                                     /（工）= ＞二   Z 功k.，奴，,（工）+ Z 口k,s。bk,s。仁）
                                           s=s k=Kl
                                                                                                                                                                   (10.22)
                                                                                                                                k=K1

It should be pointed out here that the wavelets {少k, } by themse'ves form a corn-
plete set; therefore, the unknown function could be expanded entirely in terms of the
wavelets. However, to retain only a finite number of terms in the expansion, the scal-
ing function part of (10.22) must be included. In other words, {少k,s}, because of their
bandpass filter characteristics, extract successively lower and lowefr frequency corn-
ponents of the unknown function with decreasing values of the sale parameter s,
while 中k,s。, because of its lowpass filter ch町acteristics, retains the lowest-frequency
components or the coarsest approximation of the original function.
   In (10.22), the choice of so is restricted by the order of wavelet; while the choice
of si1 is governed by the physics of the problem. In applications nvolving electro-
magnetic scattering, as a rule of thumb, the highest scale sn shouIkl be chosen such
that l/ 2'8+l does not exceed 0.l入0.                                   i
    The expansion of f given by (10.22) is substituted in (10.1), 1and the resulting
equation is tested with the same set of expansion functions. This rdsult gives a set of
linear equations as

                          [[
                                     A中，   中！
                                                                  [A中，          少！        ][.        [   "*
                                                                                                                                   m
                                                                                                                                   1
                                                                                                                                   1
                                                                                                                                                但 司
                                                                                                                                                      打   r
                                                                                                                                                          느
                                                                                                                                                              /

                                                                                                                                                              士    (10.23)
                                                                                                                                                                                  m
                          나A砂. j [A少，中iJLL功n.sjn,s J
                                                                                                                                                              J
                                                                                                                                   1
                                                                                                              ，」..]*]=
                                                                                                                                                          1
                                                                                                                                   1
                                                                                                                                                                                  ]
                                                                                                                                   L
where

                                                                         [A中,中］ := 仲k's。
                                                                                       , (LK似,m))k,k,                                                              (10.24)
                                                                                         , (LK砂n,s))k'.n.s
                                                                         [A中, 寸］ := （中k's。                                                                         (10.25)

                                                                         [A砂,中］ := （少可,." (LK似,,0))k,.,.r                                                          (10.26)

                                                                         [A少, 少］ := （少可,s', (LK呱 ,:)).,1,可,.                                                       (10.27)


                                                                          (/,  ,     !)
                                                                                     g)   :=   L f(x)
                                                                                               /,b                        g(x) dx,
                                                                                                                                                                   (10.28)




In (l?
                                                         （뇨／)(1)
                                                             (x)
                                                         (LKf)                            :=
                                                                                          :=   j f(x
                                                                                               /,b                       ')   K(x, x') dx'.
                                                                                                                                                                   (10.29)

        .23)    ,   [w,
                               ,S,   ]n,   5    .   is           a one-dimensional vector and                                          should         not b confused   with   a
Lwo-oimensionai mauix. riere me muex n is vaneo nrsL ior a nxeu vaiue O1 S.
                                                                           WAVELET TECHNIQUES      275

   We can explain the denseness of the conventional MoM and the sparseness of
the wavelet MoM by recalling the fact that unlike wavelets, the scaling functions
discussed in this book do not have vanishing moments properties. Consequently, for
two pulse or triangular functions 中l and 勿 (usual bases for the conventional MoM
and suitable candidates for the scaling functions), even though 仲i. 中2) = 0 for
nonoverlapping supports, ( i, LK中2) is not very small since Lk中2 is not small. On
the other hand, as is clear from the vanishing moment property,


                     /:t   "llrm   (t)   dt =   0,   p   =    0.
                                                                   .   .   .   .   m   -   1,
                                                                                                (10.30)

the integral vanishes if the function against which the wavelet is being integrated
behaves as a polynomial of a certain order locally. Away from the singular points,
the kernel usually has a locally polynomial behavior. Consequently, integrals such as
(LK少n,5) and the inner products involving the wavelets are very small for nonover-
lapping supports.
   Because of its total positivity property, the scaling function has a smoothing or
variation diminishing effect on a function against which it is integrated. The smooth-
ing effect can be understood as follows. If we convolve two pulse functions, both of
which are discontinuous but totally positive, the resultant function is a linear B-spline
that is continuous. Similarly, if we convolve two linear B-splines, we get a cubic
B-spline that is twice continuously differentiable. Analogous to these, the function
LK中k ,SO is smoother than the kernel K itself. Furthermore, because of the MRA
properties that give

                              (中k,s, 吻．r) = 0,               s 5 s',                            (10.31)

the integrals (中k' n, (LK砂fl. )) and (砂 ' ', (LK伽.5。)) are quite small.
   Although diagonally dominant, the L A中，中J portion ot the matnx usually does not
have entries that a七 very small compared to the diagonal entries. In the case of
conventional MoM, all the elements of the matrix are of the form (砂k ,S, (L K中k .$)).
Consequently, we cannot threshold such a matrix to sparsify it. In the case of the
wavelet MoM, the entries of [A中,中] occupy a very small portion (5 x 5 for linear and
11 x 11 for cubic spline cases) of the matrix, while the rest contain entries whose
magnitudes are very small compared to the largest entry; hence a significant number
of entries can be set to zero without affecting the solution appreciably.


10.3.3    Wavelets in Spectral Domain
In all of the preceding chapters, we have used wavelets in the time (space) domain.
In previous sections, the local support and vanishing moment properties of wavelet
bases were used to obtain a sparse matrix representation of an integral equation. In
some applications, particularly in the spectral domain methods in the electromagnetic
problems, wavelets in the spectral domain may be quite useful. Whenever we have a
problem in which the unknown function is expanded in terms of the basis function in
 276     WAVELETS IN BOUNDARY VALUE PROBLEMS

 the time domain w川le the numerical computation takes place in the1spectral domain,
 we should look at the time-frequency window product to determiie the efficiency
of using the particular basis function. Because of the nearly optinial time (space)-
frequency (wavenumber) window product of the cubic spline and the corresponding
semiorthogonal wavelet, the double integral appearing in the transmission line dis-
continuity problems can be evaluated efficiently. In this section we consider an ex-
ample from a transmission line discontinuity to illustrate the usefulness of wavelets
in the spectral domain.
    Transmission-line configurations are shown in Figure 10.3. Formulation of the
integral equation for these configurations is not the purpose of this section. Read-
ers may refer to [5, 24, 25] for details on such formulation. The integral equation
obtained is


                      f A(k., ky)f (kY)ak(-ky) dk: dk = 0                       (10.32)

with


                  A(k：匈＝d, k)J訊吐必，外                                             (10.33)


where Gyy is the appropriate Green's function and cos2 k p and n2k工p refer to
even and odd modes, respectively. The functions fy(ky) k(ky) are e Fourier trans-
forms of the basis functions representing the y-dependence of the agnetic current.
To find the propagation constant kye of any infinite transmission lin we assume that
all the field and current distributions have their y-dependence as e jkyey . It is
                                                                                   easy,
for this case, to arrive at


                                                                                (10.34)
                            L,
                                  A曲(kx,    kye)
                                                   dk:   -
                                                             0.
   Since the transverse dimensions of slots (strips) are very small c mpared with the
wavelength, we assume that the current distribution, sufficiently a ay from the dis-
continuity, is due to the fundamental mode only. Near the discont uity, in addition
to the entire domain basis functions resulting from the fundame I mode, subdo-
main basis functions are used to expand the unknown current (ma etic or electric)
to account for the deviation caused by the presence of higher-o r modes gener-
ated by the discontinuity. We use three different sets of subdomai basis functions:
(1) piecewise sinusoids (PWSs), (2) cubic B-splines, and (3) a corn ination of cubic
B-splines and the corresponding serniorthogonal wavelets.
   For cases (1) and (2), the longitudinal variation of current is given as

                                                    K
                      方（y) = Sj (y) 士 rsr (y) +＞二nt中k(Y),                      (10.35)
                                                    k=O
                                                         WAVELET TECHNIQUES         277




       TThl
           )            남2d놔E- 2s- k--2d늬
          / 트 , Ft


                                              (a)
                        k口d- +E口s   +E口d- I
              f4t

              C。, .t。

                                          (b)
FIGURE 10.3 (a) Open coupled-microstrip; (b) Short-circuited coupled slot line with uni-
axial substrate,




where K > 0 and plus and minus signs apply to transmission line configurations
with strips (Figure 10.3a), and with slots (Figure 10.3b), respectively. Ideally, the
magnitude of the reflection coefficient F should be 1; we will see, however, that
11기< 1, indicating the pseudo nature of such terminations, as shown in Figure 10.3.
The entire domain functions s1 and Sr, representing incident and reflected waves,
respectively, are given below.
 278     WAVELETS IN BOUNDARY VALUE PROBLEMS

                            /       7r \
           斗（y) :=COSkyey U ( Hy - =H J - jS1flkyeY U(- y)                                                                                                                  (10.36)
                                                           \                             二凡U口
                                                               \                                              /




                                                 }
                                                                                            / V           /




          햐（ky) =
                            [ex小쑤，）긔
                             忙；
                              了,『居「8(k       )
                                             (
                                             +
                                                                                                                              ky
                                                                                                                                                                       川
                                                                                                                                                t
                                                                                                                                        e
                                                                                                                                                8                  k
                                         1

                                                                                                                                                   /
                                                                                                                                                       V
                                                                                                                                                                            (10.37)


                                                                                    므） +j Si毗, eY U(- y)                                                                   (10.38)
           Sr           =   COSkye，                                                  乙凡17戶
                                                                                        / V           /
                                                                                                          /




                                                                                                                                        }
                (y)
                                                 吐y-
                    I     /     Jr 凡， \    ]
          Sr (ky) = 1 exp (- ji       ) +j 1
                            1=               \                     /   V   /                  H




                             x {
                                     Lky 居  4 r = 나口 I-
                                         k{, - k乙
                                                Jr ' 寸 2
                                                                                                  ky
                                                                                                  各                      H
                                                                                                                         1
                                                                                                                             )
                                                                                                                             [
                                                                                                                             ]
                                                                                                                             (
                                                                                                                             +
                                                                                                                             1 k
                                                                                                                                   V/
                                                                                                                                        e
                                                                                                                                                t
                                                                                                                                                8
                                                                                                                                                  VJ
                                                                                                                                                           t
                                                                                                                                                                   e       (10.39)


where kye is the propagation constant for the fundamental mode and U(y) is the
Heaviside function, defined in the usual way as


                                                                                                                  V/ y       00
                                                                                                                                                               ＞
                                                       U(y) =                                                                                                              (10.40)
                                                                                   11,
                                                                                         。,
                                                                                                                                                           <
                                                                                                                                                           小
가比 subdomain basis function 似 如r the pi凹ewise sinusoid case is

                      cbk (y) :=fl[ y+ T(k+ 1)]                                                                                                                            (10.41)


                      「（,):＝口；
                             匕나 '：
                                「1【      t u,                                                                     eisewnere
                                                                                                                                                                           (10.42)



                      &((,):("'""""『*了꼰’； ,了 / """ 各：片" '                                                                                                                  (10.43)

with 0 < T < 兀/2kye. For the cubic B-spline case,

                                 ,   .                 ,   ,           /y                                         \
                                                                                                                                                                           (10.44)
                                                                               .          1       .           .

                             甲k Y) := IY4 1 - 十 凡 十 {+ j
                                          \ T         I


                             a(ty) == re （奸2)k小 叱r/2) ]"                                                                                                                   (10.45)
                                              1 凡V r / 乙 1                                            느                  /         r        /




  For the third choice of basis function, we have the following epresentation of
力（y):

                                                                           0   N (s)                                                            K佃o)
        月（y) = s肋 士 氏(y) + ＞二 Z 吼仇,巾）+ ＞二 ak "k,s。(Y), (10.46)
                                                                       s=긔J n=0                                                                 k=0
                                                                                                                                                       WAVELET TECHNIQUES                               279

where N(s), K (s0) 之 0, sj <0, and

                  ,                , , /2S y                                    , . .\
                 甲k,s == IV4 1 -=                                          十凡十'       1                                                                                                              (10.47)
                                 t              \                                    /
                  .                , 12sv . , . n \
                 V/kJ := V'4 I 11二 + 凡 + 7)                                                                                                                                                          (10.48)
                                             \ r                                          I

      少k,s (kr)
                                  和[ /("큐"" ] QI\ 三_. / J [                                                           1H
                                                                                                                                        /kVr\
                                                                                                                                              乙
                                                                                                                                              "
                                                                                                                                                         [sin
                                                                                                                                                                    1
                                                                                                                                                                        (kT/
                                                                                                                                                                             I
                                                                                                                                                                                 2s+
                                                                                                                                                                                       +2
                                                                                                                                                                                            2)
                                                                                                                                                                                                 j
                                                                                                                                                                                                 y
                                                                                                                                                                                                     (10.49)

                          1                               /   3kV                   凡，    \
                Q(ky) := --,                              Icos-;--120coskV+ 1191cos 寸- 1208I
                                   乙＞乙U                   \                     乙                                           '                                   乙                       /


                                   x sin4                         竺．
                                                                                                                                                                                                     (10.50)
                                                                       4
Observe that the definitions of 砂k,s and 砂k,S are slightly different from those used
in previous chapters. The time-frequency window products of PWS, cubic spline,
and the cubic spline wavelet are 0.545, 0.501, and 0.505, respectively. Observe that
the product for the linear spline is 0.548; therefore, the double integral as discussed
before will take about the same time to compute in both cases.
    Application of the Galerkin method with the basis functions described previously
leads to a set of linear equations, the solution of which gives the desired value of the
reflection coefficient r. For the first two we have

                                                                                                                                                                                                     (10.51)
                                                    [ [A,
                                                      [4P」
                                                         ］ [4
                                                           [Ap, i[
                                                                ][         i]                 「，    q]
                                                                                                    .]                     [ck小[   I,                    Be]             ,




where in the case of cubic splines, the matrix elements take the form

                                                                                                                           (k Y r/ 2)
                                   / /
                                                                                                                                                  ]4
                                                                                 (k:,
                                   'oo              'oo
                                                                                                               [sin
                                                                                              k7)
           i
                                                                                                                           kyr/2
                                                                       們
 바，        1=
 A,
                  21kye
                                 J。 j。
                            뇨
                  2！
                            cos[   (p + 1 ir/ 2 kye r)y k’ ye, + j cos[ (p + 1) krI dk dk, (10.52)             目
                                         ]
                                                              -                                            -   k2
                                。
                                ,'cc 。
                                         AHM (kX,（,)       (k y r/ 2
                                         ..oo
                                                                                                                                         ]8
                                         / " " （뇨                   )
                                                                                                    fsin
Ap,q =
4P.
      q=          212]
                  2
                                                           kr/ 2                    ky)
                          x cos[(p - q + 1) ky 1] dk工 dky ,                                                                                                                                          (10.53)

withp = 1. . . . .M+ 2andq =2. . . . .M+ 2. MatrixelementsforthePWScanbe
written in a similar way. In both cases, we observe that

                           Ap,q = Aq_i,p+i, p = 1. ... .M + 1                                                                                                                                        (10.54)

                                   = Ap小I,q_1, p= 2. . . . .M+ 2;                                                                                      q =3. . . . .M+ 2,                            (10.55)

indicating the symmetry and Toeplitz nature of the major portion of the matrix.
280      WAVELETS IN BOUNDARY VALUE PROBLEMS

    For the discontinuity problem, we find that the third representation, (10.46), does
not rive much advantane over the second one. Unli妃 the scatterinc oroblem in which
 the domain 01 the unknown tunction may be several wavelengths long, bOr most ot the
 discontinuity problems, the domain of unknown is approximately one wavelength,
 since the effect of discontinuity on the current distribution is localized. The size of
the matrix in the case of the discontinuity problems is usually small compared with
the scattering problem. Consequently, achieving sparsity of the malrix may not be a
major concern. On the other hand, the spectral integrals associated with each matrix
element in the case of the discontinuity problems usually takes a C()nsiderably large
amount of CPU time. Faster computations of these integrals are achieyed using cubic
splines due to their decay pro氾rty which is better than that of PWS [see (10.43) and
(10.45)]. For further details on the numerical results for the reflec Lion coefficients,
readers are referred to [5, 24, 25].


10.3.4    Wavelet Packets
Recently, discrete wavelet nacket (DWP) similarity transformatio노S has been used
to obtain a higher degree of sparsilication 01 the matrix than is achievable using the
standard wavelets [21]. It has also been shown that DWP method gives faster matrix-
vector multiplication than some of the fast multipole methods.
   In the standard wavelet decomposition process, first we map the given function
to a sufficiently high resolution subspace (VM) and obtain the approximation coeffi-
cients {ak,M} (see Chapter 7). The approximation coefficients {ak, el} and wavelet
coefficienis { wk,M_l } are computed from {ak,M}. This process con flues, that is, the
coefficients for the next lower level M - 2 are obtained from {ak,      i }, and so on.
Observe that in this scheme, only approximation coeffiecients {ak,j} are processed at
any scale j; the wavelet coefficients are merely the outputs and re amll untouched.
In a wavelet packet, the wavelet coefficients are also processed whi h, heuristically,
should result in higher degree of sparsity since in this scheme, the requency bands
are further divided compared with the standard decomposition sche e.



10.4     WAVELETS ON THE BOUNDED INT[RVAI

In previous chapters we described wavelets and scaling function defined on the
real line. If we use these functions directly to expand the unknow function of an
integral equation, some of the scaling functions and wavelets will ye to be placed
outside the domain of integration, thus necessitating the explicit en brcement of the
boundary conditions. In signal processing, uses of these wavelets le d to undesirable
jumps near the boundaries (see Figures 8.8-8.10). We can avoid is difficulty by
penodizing the scaling function as [26, Sec. 9.3]

                              叱 := 乞吼仁 +Z);                                    (10.56)
                                        WAVELETS ON THE BOUNDED INTERVAL                    281

where the superscript p implies the periodic case. Periodic wavelets are obtained
similarly. It is easy to show that if 中(2n-k) = 8k.0. which is generally true for the
scaling functions, then >Jk （工 - k) 三 1. If we apply to (10.56) the last relation,
which as discussed in Chapter 5 is also known as the partition of unity, we can show
that ｛中g,0}U｛砂f,,; S E 兀＋ := (0, 1, 2, . . .), k = 0. .. . .2S - l} generates L2([0, 1]).
   The idea of periodic wavelets has been used by [18-201. However, as mentioned
in [26, Sec. 10.7], unless the function that is being approximated by the periodized
scaling functions and wavelets is already periodic, we still have edge problems at the
boundaries. Therefore, we follow a different approach to account for the boundary
effects. We apply the compactly supported semiorthogonal spline wavelets of [23,
27, 28], which are specially constructed for the bounded interval [0, 1]. Other ways
of obtaining intervallic wavelets are described in [29, 30].
    As we discussed in Chapter 5, splines for a given simple knot sequence can be
constructed by taking piecewise polynomials between the knots and joining them
together at the knots in such a way as to obtain a certain order of overall smo야hness.
For instance, consider a knot sequence (0, 1, 2, 3, 41. With this sequence we can
construct the cubic spline (m = 4) by taking polynomials of order 4 between knots,
suchas[0, 1), [1, 2)... . .andjoiningthemtogetherat 1, 2, and3 sothattheresultant
function (cubic spline) is in C2, that is, up to its second derivative is continuous
in [0, 4). In general, cardinal B-splines of order m are in cm寸2. However, if we
have multiple knots, say for ex띠llple (0, 0, 1, 2, 3), the smoothness at the point with
multiple knots decreases. It is easy to verify that the smoothness decreases by r - l
at a point with r-tuple knots. Observe that at the boundary points 0 and 1, the knots
coalesce and form multiple knots. Inside the interval, though, the knots are simple,
and hence the smoothness remains unaffected.
   恥r s e 72七let {t｝亡쓰出 be a knot sequence w油耐뺘kn毗仙and 1 and
simple knots inside the unit interval, that is,

                        dm+l
                         - m+1 -=tsm+2
                                   -m+2 -= . . · -= i 05 -= 0
                             t{ =k2H5, k= 1                              2S -1           (10.57)
                            r S = i S1+
                                -  2+1l =-   ·   ·   ·   -=   r
                                                              42s+   S   m_ 1   -   01
For the knot sequence (10.57) we define the B-spline (m 之 2) as [31, p. 108]

              Bm,s，小:= (thmHm[t加｛+1'                                      tSk+m］小m工埠寸    (10.58)

where [t . ....tj+m]t is the mth-order divided difference of (t - x)少 with re-
spect to t and (x)+ := max(0, x). Wavelets can be obtained from the correspond-
ing spline scaling functions. Instead of going into the details of constructing scaling
functions and wavelets on a bounded interval, we provide their explicit formulas in
Section 10.9. Interested readers will find details in [23, 27, 28].
   The support of the inner (without multiple knots) B-spline occupies m segments,
and that of the corresponding semiorthogonal wavelet occupies 2m - 1 segments.
At any scale s the discretization step is l/ 2L which for s > 0 gives 2S segments in
282         WAVELETS IN BOUNDARY VALUE PROBLEMS

[0, 1]. Therefore, to have at least one inner wavelet, the following c ndition must be
satisfied:

                                                                       2s 之 2m -1.                                          (10.59)

Let s0 be the scale for which the condition (10.59) is satisfied. Then for each s 之 se,,
let us define the scaling functions 中m,k,s of order m as

                 I Bm.Sn. t (21150X),                                                         k = -m + 1. ....-1
    m.k.s (X) := { Bm.sn.2s_m_k(1 - 25_s0x),                                                  k = 2S - m + 1, ... 2S 놔 1 (10.60)
                 I Bm,s。,0(2S+S0X - 2_s0k),                                                   k = 0. ... .2S - 77i

and the wavelets 砂m,k,s as

.       .   .   -   lu/
                          Fm,
                                      (2s                                                     tk       =-m+ l. ....-1
                                                                                                k1     =2s_ 2m+ 2. . . ,25_ m
                                kso
                                                           , . .        ,c-          cn   .

Vm,k,s（兀J '= 1 Vm,2'- 2쓰寸．k,s0(i - . 二，. " 兀J'
                                            "s0x)
             1Vm,0,so（乙 U兀 4 乙 'V凡J,                                                                   =0. ... .2s_ 2꺄+ 1.
                                                                                                                            (10.61)

Observe that the inner scalinR functions (k = 0. .. ....- m) and the wavelets (k =
U, · · . 1 乙" m= 乙刃2 十 1) ai七 me s跏ne as inose ror me nonnouno缸ycase4 m nere 町e 刃2- 1
boundary scaling functions and wavelets at 0 and 1, and 2S - m + 1 inner scaling
functions and 21 - 2m + 2 inner wavelets. Figure 10.4 shows all the scaling functions
and wavelets for m = 2 at the scale s = 2. All the scalman functiois for m = 4 and
s = 5 게re snown in riqure ju..ia. wnne rmmire iu.그o nives only we corresponain으
nounuary wavemets near x = U anu one inner wavemet. m ne rest or tne inner waveiets
can be obtained simply by translating the first one, whereas the boundary wavelets
near x = 1 are the mirror images of wavelets near x = 0.


10.5        SPARSITY AND ERROR CONSIDERATIONS

The study of the effects of thresholding the matrix elements on the sparsity and
error in me solution is me ooiecnve or mis supsecuon. nv rnresnoiazne we mean
settin으 t山se elements 01 tflC matrix to zero tnat 出e smaller (lfl ma으nmtuoei man
some positive number d (U 5 d < 1), called the tlzreshola para枷eter, times tile
largest element of the matrix.
   Let Ama, and Andn be the largest and the smallest elements of the matrix in
(10.23). For a fixed value of the threshold parameter 8, define percent relative er-
ror (Ci) as

                                                                       Ilfo 小／제2                       . ,,,,
                                                    EA ;=                                          x   i1八J                 (10.62)
                                                                             IIf(川2
and percent sparsity (S8) as

                                                                                                                            (10.63)
                                                     so:           =     N    "而N8             x       100
                                                        SPARSITY AND ERROR CONSIDERATIONS                                    283




    1.0                                                                 1.0
    0.5                                                                 0.5                            y2,    2,   0   (X)
         0                                                                   0
-0. 5                                                               -0. 5
-   1.   0                                                          -1. 0
             0   0.2                  0.4   0.6   0.8   1.0                      0   0.2   0.4   0.6         0.8             1.0
    1.0                                                                 1.0
    0.5                 2
                   1/       .2   ,1   (x)
                                                                        0.5
         0                                                                   0
-0. 5                                                               -0. 5
-1. 0                                                               -   1.   0
             0   0.2                  0.4   0.6   0.8   1.0                      0   0.2   0.4   0.6         0.8             1.0
                                                              (b)
FIGURE 10.4 (a) Linear spline (m = 2) scaling functions on [0, 11; (b) Linear spline
wavelets on [0, 11. The subscripts indicate the order of spline (m), scale (s), and the position
(k), respectively. (Reprinted with permission from [231, copyright (9 1995 by IEEE.)
284         WAVELETS IN BOUNDARY VALUE PROBLEMS




 0.5
                                             _3

                                                                                                           3
                                                  (x)
                                        3,
                                 砂4.
                                                                                                       ,       , m2

    0
                                                                                                  砂4                  (X)
-0. 5

-1 0
        0    0.2   0.4     0.6         0.8              1.0                     0.2   0.4   0.6        0.8                  1.0


 0.2                                                                 0.2

    0                                                                  0

-0. 2                                                               -0. 2

        0    0.2   0.4     0.6         0.8              1.0                 0   0.2   0.4   0.6        0.8                  1.0
                                                              (b)
FIGURE 10.5 (a) Cubic spline (m = 4) scaling functions on [0, 1]; (b) Cubic spline
wavelets on [0, 1]. The subscripts indicate the order of spline (m), scale (s). and the position
(k), respectively. (Reprinted with permission from [231, copyright （르） 1995 by IEEE.)
                                                                           NUMERICAL EXAMPLES                                     285


 TABLE 10.1 Relative Magnitudes of the Largest and Smallest Elements of the Matrix for
 Conventional and Wavelet MoM (a = 0. lA0)

                           Conventional                         Wavelet                                      Wavelet
                              MoM                             MoM (m= 2)                                   MoM (m= 4)
 AmaX                            5.377                        0.750                                        0.216
 Am1l                            1.682                        7.684 )< 10田                                 8.585 x 10-13
 Ratio                           三400                         9.761 x 106                                  2.516 x i01'
 Source: Reprinted with permission from [231, copyright @ 1995 by IEEE.


In the above, f represents the solution obtained from (10.23) when the elements
 whose magnitudes are smaller than 8Amax have been set to zero. Similarly, N3 is
 the total number of elements left after thresholding. Clearly, f (x) =
                                                                         f (x) and
N0 = N2, where N is the number of unknowns. If we use the intervallic wavelets
of Section 10.4 in solving (10.1), then number of unknowns (N) in (10.23), interest-
ingly, does not depend on s0. This number N is

                                          N= 2' .+1+ m- l.                                                      (10.64)
   Table 10.1 gives an idea of the relative magnitudes of the largest and smallest
elements in the matrix for conventional and wavelet MoM. As expected, because
of their higher vanishing moment property, cubic spline wavelets give the higher
Amax/Arnie ratio.
   With the assumption that the [A中,中] part of the matrix is unaffected by the thresh-
olding operation, a fairly reasonable assumption, it can be shown that

                S      -            1     (210 + m             (2S0            2)   ]           l00
                                                          N2
                                                                                                      .'        ,,,.'


                 V," 4 r            N                                               ]" IuJ,
                                                                                                                                   "
                                                     -
                  ,"
                                                                                                                ' IU.03)
                            fl
                                                                                        .   .
                                                         1)
                                                                      +m
                                                                           -
                                                                                                                        "
                                                                                                                            65)
where N is given by (10.64).
   As mentioned before [see (10.64)], the total number of unknowns is independent
of s0, the lowest level of discretization. However, it is clear from (10.65) that the
upper limit of S3 increases with the decreasing values of so. Therefore, it is better to
choose so = f1og2(2m - 1)], where lxi represents the smallest integer that is greater
than or equal to x.


10.6     NUMERICAL EXAMPLES

In this section we present some numerical examples for the scattering problems de-
scribed in Section 10.1. Numerical results for strip and wire problems can be found
in [14]. For more applications of waveletsto electromagnetic problems, readers may
refer to [22].
   The matrix equation (10.23) is solved for a circular cylindrical surface [23].
Figures 10.6 and 10.7 show the surface current distribution using linear and cubic
286     WAVELETS IN BOUNDARY VALUE PROBLEMS




             瓦
                           卄
             Nm그
             ＼
                               O
                                    0/   1
                                                   Convent向n이 M아／                         /
                                   朴     i
                                         1
                                                                                          =


                                   O               밖ave沌tM아.1

                     100
                                                                                /
                                                  m= 2                     /

                    N
                    mb 능

                                                         二
                                                                      /
                                                              /
                           0


                   mmO工4
                                                         'I   '
                                                                  1
                                                                          1 /        1




                   -100



                           ？石＝0.1? o                              I<- 2 a버

                                             1           1                           1

                           0                 50         100                         150

                                                    中

FIGURE 10.6 Magnitude and phase of the surface current distribution on a metallic cylinder
using linear spline wavelet MoM and conventional MoM. (Reprinted with permission from
[23], copyright 匣） 1995 by IEEE.)
                                                                        NU入征RICAL EXAMPLES   287




             瓦
             Nm그
             ＼
                                    50                 100                             150

                                                   中


                                         -   -   - Convention이 M아d
                                                   나eyelet M아d

                      100

                                                 m= 4



                   N
                   m= 늠 mm은a
                                                                   /
                               0                               /   1     1   J十 寸戶
                                                                                       -I-
                               /                   1   J       "

                                                   /:,     -




                 -100
                                                                                  l中
                                                                       畔m= 2 a내

                                                           1
                               0    50                 100                             150

                                                   功

FIGURE 10.7 Magnitude and phase of the surface current distribution on a metallic cylinder
using cubic spline wavelet MoM and conventional MoM.
288      WAVELETS IN BOUNDARY VALUE PROBLEMS




              d8오




                    8                              1



                                      Convent向n이 M아d
                                      밖ovelet MoM

                    6            m= 4




              d
              8=    4



                                               니十＞
                 2                                      ol$
                 0
                        0        50               100           150

                                              少
FIGURE 10.8 Radar cross section of a metallic cylinder computed using linear (m = 2) and
cubic (m = 4) spline wavelet MoM and conventional MoM.
                                                                                             NUMERICAL EXAMPLES               289


                  15                                                                                    100

                                  m= 4
                                   "        1   1   .1   /   "
                                                                 "




                                                                                                        80

                 10




                                                                                                              수m니 力 죤 口 유 K
             소
             巴 b占 K
                                                                                                       0
                                                                                                       b
                                                                                                       八




                                                                                                        0
                                                                                     Error              4
                          ＜
                              n
                                  m= 2
                                                                                     Sparsity
                      나
                                                                                                       20
                                                             r나八／               入H    m = 4

                                        1
                                    尸
                                                                        2x10-
                                                                                3     3x1。   －3
                                                                                                    4x183

                                                                     Thre計1이d (a)
FIGURE 10.9 Error in the solution of the surface current distribution as a function of the
threshold parameterS. (Reprinted with permission from [23], copyright （르）1995 by IEEE.)




 splines, respectively, for different sizes of the cylinder. The wavelet MoM results
 are compared with the conventional MoM results. To obtain the conventional MoM
 results, we have used triangular functions for both expanding the unknown current
 distribution and testing the resultant equation. The conventional MoM results have
 been verified with the series solution [32]. Figure 10.8 gives the radar cross section
 for linear and cubic spline cases. The results of the conventional and wavelet MoM
 agree very well.
    The effects of 8 on the error in the solution and the sparsity of the matrix are shown
in Figure 10.9. The magnitude of error increases rapidly for the linear spline case.
Figure 10.10 shows a typical matrix obtained by applying the conventional MoM. A
darker color on an element indicates a larger magnitude. The matrix elements with
8 = 0.0002 for the linear spline case a七 shown in Figure 10.11. In Figure 10.12 we
present the thresholded mat奴 (8 = 0.0025) for the cubic spline case. The [A*,*]
part of the matrix is almost diagonalized. Figure 10.13 gives an idea of the point-wise
error in the solution for linear and cubic spline cases.
   It is worth pointing out here that regardless of the size of the matri兀 only 5 x 5
in the case of the linear spline and 11 x 11 in the case of the cubic splines (see the
to니eft corners of Figures 10.11 and 10.12) will remain una且ected by thresholding;
a significant number of the remaining elements can be set to zero without causing
much error in the solution.
                                                                                                                         ＝
                                                                                                                         口
                                                                                                                             口
                                                                                                                             1
FIGURE 10.10 1 'pical gray-scale plot of the matrix elements obtained using conventional
MoM. The darker color represents larger magnitude.




                                                                                                                                 11 1




               1 i 1 ! 1 !
               小
                                                                                         1   1   1
                                                                                         i   i   i       I   l   l



                                                                                                                                 1 1 i
                                                                                         1   I       I   l   l   !
                                                                                                         I       I
                                                                 !   i   I   I       I
                                                                 I       1 1     1   1   1   1       I
                                                                                 1       1   I   I   I   !   ,

                                                                                                                                 1 1
                                                                                                 1       '   I
                                                     1   1   1   1   1   1                                                       1
                                                             1   1   1   1   1   1
                                                                     1   l   i   i   i   !
                                                                             I   I   1   1   1   1



                                                                                                                                 !
                                                                                                                                 H
                                                                                                                                 1

               i             !       1   i   1           ::                                                                      1

               !                     1   !   1   1               1
               1 I               I           I                       1
                             I   I           I   I                       1
               i             1   1           1   i
                             !                                                   t


                             i   I   I                                                   1
                                                                                             1
                             1                                                                   1
                                                                                                     1


                                                                                                             1


                                                                                                                     1
                             1       1                                                                                           1 1
              二



FIG URE 10.11 Typical gray-scale plot of the matrix elements obtained using linear wavelet
MoM. The darker color represents larger magnitude. (Reprinted with permission from [23],
copyright @ 1995 by IEEE.)

290
                                   SEMIORTHOGONAL VERSUS ORTHOGONAL WAVELETS       291


                                       1 1
                                       1 1
                                       1
                       1 1     [       1




               i   1   1   !   1




              1e                                                       二
FIGURE 10.12 Typical gray-scale plot of the matrix elements obtained using cubic wavelet
MoM. The darker color represents larger magnitude. (Reprinted with permission from [23],
Co아叩ht @ 1995 by IEEE.)




10.7   SEMIORTHOGONAI VERSUS ORTHOGONAI WAVELETS

Both semiorthogonal and orthogonal wavelets have been used for solving integral
equations. A Comparative study of their advantages and disadvantages has been re-
ported in [141. The orthonormal wavelet transformation, because of its unitary sim-
ilar property, preserves the condition number (K) of the original impedance matrix
A; semiorthogonal wavelets do not. Consequently, the transformed matrix equation
may require more iterations to converge to the desired solution. Some preliminary
results comparing the condition number of matrices for different cases are given in
Table 10.2 [17].
   In applying wavelets directly to solve integral equations, one of the most attractive
features of semiorthogonal wavelets is that closed-form expressions are available for
such wavelets. Most of the continuous orthonormal wavelets cannot be written in
closed form. One thing to keep in mind is that, unlike signal processing applications
where one usually deals with a discretized signal and decomposition and reconstruc-
tion sequences, in the boundary value problem we often have to compute the wavelet
and scaling function values at any given point. For a strip and thin wire case, a corn-
parison of the computation time and sparsity is summarized in Tables 10.3 and 10.4
[14].
292     WAVELETS IN BOUNDARY VALUE PROBLEMS




                                  6 n0 h0 6
                                              = 0.0000                                ／尸
                      回
                      H                       = 0.0001          m= 2
                 6x104                        = 0.0002          a=0.1入0
                                              = 0.0005



                 瓦
                                     4




                 N
                 m그
                 ＼
                 2x10e
                              7
                          /
                                                         卄ol,
                                          50                        100         150

                                                                中

                                              1                                  1




                                  6666
                                              = 0.0000                                 尸尸＝




                                              = 0.0004          m= 4                         1
                                                                                             回




                 6x103                        = 0.0010          0=0J入0
                                              = 0.0025



             1
             0
             山
             가
             ＼
             N
             m
             )
                 2x104

                                                         니十＞
                                                                          ol'
                                                                                 1
                      0
                          0               50                        100         150

                                                                中
FIGURE 10.13 Magnitude of the surface current distribution computed using linear (m = 2)
and cubic (11 = 4) spline wavelet MoM for different values of the threshold parameter 各.
(Reprinted with permission from [231, copyright （트） 1995 by IEEE.)
                               SEMIORTHOGONAL VERSUS ORTHOGONAL WAVELETS                                 293



TABLE 10.2 Effect of Wavelet Transform Using Semio代hogonal and Orthonormal Wavelets
on the Condition Number of the Impedance Matrix. Original Impedance Matrix Is Generated
Using Pulse Basis Functions

                                                                                           Condition No. K
Ba前S
and                   No. of       Octave                                             Before          After
Transform            Unknowns      I尤ye!            8         S各           E8        Thre밗iold     'I뇨esh아d

Pulse and none            64           NA         NA          0.0    2.6 x 10巧          14.7
I뇨lse and
  semiorthogonal          64            1      7.2 x 10-2     46.8        0.70          16.7          16.4
Pulse and
  orthonorm십              64            1      7.5 x 104     59.7         0.87          14.7          14.5



                TABLE 10.3 Comparison of CPU Time per Matrix Element for
                Spline, Semiorthogonal, and그rthonormal Basis Function

                                                         Wire                      Plate

                Spline                                   0.12s                  0.25 x 10H3s
                Semiorthogonal wavelet                   0.49s                      0.19s
                Orthonormal wavelet                      4.79s                      4.19s

                Source: Reprinted with permission from [14], copyright 匣）1997 by IEEE.


   As discussed in previous chapters, semiorthogonal wavelets are symmetric, hence
have generalized linear phase, an important factor in function reconstruction. It is
well known [26, Sec. 8.1] that symmetric or antisymmetric, real-valued, continuous,
and compactly supported orthonormal scaling functions and wavelets do not exist.
Finally, as discussed previously, in using wavelets to solve spectral domain problems,


TABLE 10.4 Comparison of Percentage Sparsity (S8) and Percentage Relative Error (es) for
Semiorthogonal and Orthonormal Wavelet Imped카lce Matrices as a Function of Threshold
Parameter (8)

                      Number of                               Sparsity                  Relative Error
                      Unknowns                                  S                             E8
Scatterer/
Octave              Semi-      Ortho-       Threshold      Semi-     Ortho-           Semi-         Ortho-
Levels           orthogonal    nonnal           8       orthogonal   normal        orthogonal       normal

Wire/                29           33        1 x 10-6        34.5         24.4      3.4 x 104      4.3 x 1013
 j = 4                                      5 x 10-6        48.1         34.3          3.9        1.3 x i04
                                            1 x i0小         51.1         36.5         16.5        5.5 x 10-2
Plaid/               33           33        1 x l0콕         51.6         28.1       1 x 10卞4          0.7
  j = 2, 3, 4                               5 x l014        69.7         45.9          4.7            5.2
                                            1 x l013        82.4         50.9          5.8           10.0

S이sir巴‘ R町)nnted with permi駱ion from [14], C아싸right (9 1997 by IEEE.
294      WAVELETS IN BOUNDARY VALUE PROBLEMS

we need to look at the time-frequency window pr어uct of the basis. Semiorthogonal
wavelets approach the 아油nal value 可 the ti毗小frequency produc :, which at 0.5 is
very fast. For instance, this value for the cubic spline wavelet is 0 505. It has been
shown [33] that this product approaches to co with the increase i i smoothness of
orthonormal wavelets.



10.8    DIFFERENTIAI EQUATIONS

An ordinary differen由l equation (ODE) can be represented as

                               Lf（功 = g（工）, 工 E [0, 1]                             (10.66)

with

                                   ,      끈八    . . d
                                   iJ =    / . a3（兀) 二＝;                           (10.67)
                                          !1=        a兀J
                                          3= )


and some appropriate boundary conditions. If the coe侄icients {a1I are independent
of x, then the solution can be obtained easily via a Fourier method. However in ODE
case, with nonconstant coefficients, and in PDEs, we generally use finite element or
finite difference type methods.
   In the traditional finite element method (FEM), local bases 게re used to represent
the unknown function and the solution is obtained by Galerkin's method, similar
to the approach described in previous sections. For the differential operator, we get
sparse and banded stiffness matrices that are generally solved usi4g iterative tech-
niques, the Jacobi method for instance.
    One of the disadvantages of conventional FEM is that the condition number of
the sti妊ness matrix grows as O(h 2), where h is the discretization step. As a result,
the convergence of the iterative technique becomes slow and the slution becomes
sensitive to small perturbations in the matrix elements. If we stu4y how the error
decreases with iteration in iterative techniques, such as the Jacobi nethod, we find
that the error decreases rapidly for the first few iterations. After that, the rate at which
the error decreases slows down [34, pp. 18-21]. Such methods are also called high-
frequency methods since these iterative procedures have a smoothing effect on the
high-frequency portion of the error. Once the high-frequency portion of the error
is eliminated, convergence becomes quite slow. After the first few iterations, if we
could re-discretize the domain with co缸ser grids and thereby go to lower frequency,
the convergence rate would be accelerated. This leads us to a multigid-type method.
    Multigrid or hierarchical methods have been pro兀sed to overcorle the difficulties
associated with the conventional methods [34-50]. In this techniqu one performs a
 few iterations of the smoothing method (Jacobi-type), and the internediate solution
and the operator are projected to a coarse grid. The problem is sol中ed at the coarse
grid and by interpolation one goes back to the finer grids. By going back and forth
between finer and coarse grids, the convergence can be accelerated. It has been shown
                                                             EXPRESSIONS FOR SPLINES AND WAVELETS          295

for elliptic PDEs, that for wavelet-based multilevel methods, the condition number is
independent of the discretization step, that is, K = O(1) [45]. The multigrid method
is too involved to be discussed in this chapter. Readers are encouraged to look at the
references provided at the end of the chapter.
    Multiresolution aspects of wavelets have also been applied in evolution equations
[49, 501. In evolution problems, the space and time discretization are interrelated to
gain a stable numerical scheme. The time-step must be determined from the smallest
space discretization. 가is makes the computation quite complex. A space-time adap-
tive method has been introduced in [50] where wavelets have been used to adjust the
space-time discretization steps locally.



10.9       EXPRESSIONS FOR SPLINES AND WAVELETS

We provide formulas for the scaling functions Bm,O,k (X) and the wavelets *m.k,0(X)
fork = -m + 1. . . ..0 andm = 2, 4. Formulas atthe sc出eso canbe obtainedby
replacing x by 25x and scaling the intervals accordingly.

                                                                                   工 E [0, 1)
                                                                                                       (10.68)
                     Bm,   _m+     i,   .(x)           =   {g'    "1   '   ,       otherwise

                                                           ［于              工E [0, 1)
                                                                                                       (10.69)
                                                           1t r兀
                             .                 .   .



                                        0（工J                               工 e Ii, 乙J
                                                                           omer叩ise.
                                                              U,
                            ij2,   O,                  =           '           .    .




Formulas for cubic spline scaling functions except for B4,_3,0 町e given in Ta-
ble 10.5. Formulas for B2,_1,0 and B4,_3,0 can be obtained from (10.68). Tables
10.6 to 10.8 contain the formulas for the wavelets. Functions are zero outside the
intervals given in the tables. An empty entry indicates that the function is zero in the
interval.
   It should be pointed out that the scaling functions and wavelets described in this
book can also be computed from their Bernstein polynomial representations [51,
Sec. 4.4; 52, pp. 11-13]; however, the formulas presented here are direct and easy to
implement.



TABLE 10.5 Cubic Spline Scaling Functions B4,k,o for Different Values of k [6 x
B4,k ,O(x) = 玎＝0咐']: 口0, 口l, 口2, 口3 如r Various Intervals
Interval                   k= -2                                       k= -1                        k= 0
[0, 1)              0, 18, -27, 21/2                                0, 0, 9, -11/2                   0, 0, 0, 1
[1, 2)              12, -18, 9, -3/2                               -9, 27, -18, 7/2              4, -12, 12, -3
[2, 3)                                                              27, 卞27, 9, -i              -44, 60, -24, 3
[3. 4)                                                                                          64, -48, 12, -1
Source: Reprinted with permission from [231, copyright （트）1995 by IEEE.
296                WAVEL日S IN BOUNDARY VALUE PROBLEMS



                      TABLE 10.6 Linear Spline Wavelet 少2,k,0 for Different 져alues


                                                                                                                                   느
                      of k [6 x 少2,k,0（工） = 口0 + a1工］: 口0, 口i for Different Interv쾨
                     1H=                  =HHH11.                                  =1HH1H=                                    m그




                     Interval                                               k= -1
                      1mm叫1HH=                                  1H1HnH니




                      [0.0, 0.5)                                             -6, 23                                            (   二1
                      [0.5, 1.0)                                            14, -17                                           4;                -7




                      [1.0, 1.5)                                             -10, 7                                         -19, 16
                      [1.5, 2.0)                                              2, -i                                         29, -16
                      [2.0, 2.5)                                                                                             - [7, 7
                      [2.5, 3.0)                                                                                              3 1               -
                     品毗e: R叩rin妃d with permission from [23}, copyright （르）1995 by 工EEE.




TABLE 10.7 Cubic Spline Wavelet 砂4k,0 fork = -3, -2 [5040x少4,k,o(                                                                  k) ＝兄캄0口i工'1:
a0, al, a2, a3 for Various Intervals

Interval                                            k = -3                                                               k=-           -2
[0.0, 0.5)                 -5,097.9058, 75,122.08345,                                        1,529.24008, -17,4( 65853.                    4.
                             -230,324.8918, 191,927.6771                                       39,663.39526, -2dP1,328.27397
[0.5, 1.0)                 25,795.06384, -110,235.7345,                                      96.3035852, -8,8071039551.
                             140,390.7438, -55,216.07994                                       22,468.15735, -l: 2, SM.78201
[1.0, 1.5)                 -53,062.53069, 126,337.0四2,                                       -37,655.11514, 104     2167.          1447.
                             -96,182.03978, 23,641.5146                                        -90,786.09884, 2 P,886.63674
r 1   r   八 r\ \           r r   /1ir0   /1r尸11mn      r\ /1 n 戶1 d r     J/ n d             1 4 n   1\ r노尸1 尸1r) r\ 0     n n /                     ,.,＼八．
                                 ,LUO. LU! UJ,                                                       ,yu, .,o7o,         -z. .)u U /O.Jy) 1,
                                                                                                                                   匕nn
                                                     e 7L, JL+ .＝戶tu乙斗7

                                 49,592.35723, -8,752.795836                                     136,631.1078, -25,650.52030
[2.0, 2.5)                 -31,922.33501, 39,961.3568,                                       -212,369.3156, 281 237.0648,
                             -16,550.59433, 2,271.029421                                       -122,326.7213, F乙509.11789
[2.5, 3.0)                 8,912.77397, -9,040.773971,                                       184,514.4305, -195 023.4306,
                             3,050.25799, -342.4175544                                         68,177.47685, -7 891.441873
[3.0, 3.5)                 -904, 776, -222, 127/6                                            -88,440.5, 77,931.51-22,807.5, 2218
[3.5, 4.0)                 32/3, -8, 2, -1/6                                                 21,319.5, -16,148.5.4,072.5. -342
[4.0, 4.5)                                                                                   -11,539/6, 1,283.5, -285.5, 127/6
[4.5, 5.0)                                                                                   125/6, -12.5, 2.5, - 1/6

Source: Reprinted with permission from [23], copyrig址 匣） 1995 by IEEE.
                                                                         REFERENCES         297


 TABLE 10.8 Cubic Spline Wavelet少4,k,O fork = -1, 0. [5040 x少4,k,O(工) = i:3=:。aix']:
 a0,口i , 口2, 口3 白r 切加us Intervals

Interval                      k= -1                                      k= 0
 [0.0, 0.5)     -11.2618185, 68.79311672,                0, 0, 0, 1/6
                  -242.2663844, 499.28435
[0.5, 1.0)      330.8868107, -1,984.098658,              8/3, -16, 32, -127/6
                  3,863.517164, -2,237.904686
[1.0, 1.5)      -9,802.095725, 28,414.84895,             -360.5, 1,073.5, -1,057.5, 342
                  -26,535.43044, 7,895.077856
[1.5, 2.0)      75,963.58449, -143,116.5114,             8,279.5, -16,206.5, 10,462.5, -2,218
                  87,818.80985, -17,516.97555
[2.0, 2.5)      -270,337.7867, 376,335.5451,             -72,596.5, 105,107.5, -50,194.5,
                  -171,907.2184, 25,770.69585              7,891.5
[2.5, 3.0)      534,996.0062, -590,065.0062,             324,403.5, -371,292.5, 140,365.5,
                  214,653.0021, -25,770.66691              -17,516.5
[3.0, 3.5)      -633,757.5, 578,688.5,                   -844,350, 797,461, -249,219,
                  -174,931.5, 17,516.5                     77,312/3
[3.5, 4.0)      455,610.5, -355,055.5,                   4,096,454/3, -1,096,683, 291,965,
                  91,852.5, -7,891.5                       -77,312/3
[4.0, 4.5)      -191,397.5, 130,200.5,                   -1,404,894, 981,101, -227,481,
                  -29,461.丘乙기8                             17,516.5
[4.5, 5.0)      41,882.5, -25,319.5,                     910,410, -562,435, 115,527,
                  5,098.5, -342                            -7,891.5
[5.0, 5.5)      -10,540/3, 1,918, -349, 127/6            -353,277.5, 195,777.5, -36,115.5,
                                                           2218
[5.5, 6.0)     36, -18, 3, -1/6                          72,642.5, -36,542.5, 6,124.5, -342
[6.0, 6.5)                                               -5,801.5, 2,679.5, -412.5, 127/6
[6.5, 7.0)                                               343/6, -24.5, 3.5, -1/6
Source: Reprinted with permission from [23], copyright @ 1995 by IEEE.



REFERE卜寸CES

 1. G. B. Arficen and H. J. Weber, M口the月iati口1 Met九ds五7r Phy缸Cs打． San I万ego: Aca-
    demic Press, 1995.
 2. G. M. Wing, A P月mert가tIn比gr口／Equ口片O1玎 O／甘玘Fir缸町nd. Philadelphia: SIAM, 1991.
 3. B. K. Alpert, G. Beylkin, R. Coifman, and V. Rokhlin, "Wavelet-like bases for the fast
    solution of second-kind integral equations," S!AMJ. Sd. Comput. 14, pp. 159-184, 1993.
298      WAVEL日S IN BOUNDARY VALUE PROBLEMS


 4. J. Mandel, "On multi-level iterative methods for integral equations of die second kind
    and related problems," N刃ier. Mark, 46, pp. 147-157, 1985.
 5. J. C. Goswami, "An application of wavelet bases in the s꺄ctral domain analysis of trails-
    mission line discontinuities, ' m1t. J. Nwner Model., 11, pp. 41-54, 1998.
 6. J. H. Richmond, "Digital solutions of the rigorous equations for scattering problems,"
    Proc. IEEE, 53, pp. 796-804, August 1965.
 7. R. F. Harrington, Field Computation by Moment Methods. New York: IEEE Press, 1992.
 8. G. Beylkin, R. Coifman, and V. Rokblin, "Fast wavelet transform and numerical algo-
    rithms I," Commun. Pure Appi. Ma疏, 44, pp. 141-183, 1991.
 9. R.  L. Wagner, P. Otto, and W. C. Chew, "Fast waveguide mode computation using
    wavelet-like basis functions," 旭L万Micn）叩口ye GuiL加d Wave I石瓦，3, pp. 208-210, 1993.
10. H. Kim and H. Ling, "On the application of fast wavelet transform to the integr심-equation
    of electromagnetic scattering problems," Microwave Opt. Technol. L名tt., 6, pp. 168-173,
    March 1993.                                                               1
                                                                              1
11. B. Z. Steinberg  and  Y. Leviatan, "On the use  of wavelet  expansions  iii method of mo-
    ments," IEEE Trans. Antennas Propag., 41, pp. 610而19, 1993.
12. K. Sabet出dui and L. P. B. Katehi, "Analysis of integrated millineter-wave and
     submillimeter-wave waveguides using orthonormal wavelet expansion目" IEEE Trans.
    凡伽rowa比 Theory 兀ck, 42, pp. 2412-2422, 1994.
13. B. Z. Steinberg, "A multiresolution theory of scattering and diffraction," Wave Motion,
    19, pp. 213-232, 1994.
14. R. D. Nevels, J. C. Goswami, and H. Tehrani, "Semi-orthogonal vrsus orthogonal
    wavelet basis sets for solving integral equations:' IEEE Trans. Anten片as Propag., 45,
    pp. 1332-1339, 1997.
15. Z. Xiang and Y. Lu, "An effective wavelet matrix transform approch for efficient
    solutions of electromagnetic integral equations," IEEE Trans. Ante기i古（is Propag., 45,
      pp. 1332-1339, 1997.
16. Z. Baharav and Y. Leviatan, "Impedance matrix compression (IMC) using iteratively
    selected wavelet basis:' IEEE Trans. Antennas Propag., 46, pp. 226-23 3, 1997.
17. J. C. Goswami, R. E. Miller, and R. D. Nevels, "Wavelet methods for soliing integral and
    differential equations:' in Encyclopedia of Electrical and Electronics Ezgineering, J. H.
    Webster (ad.). New York: John Wiley & Sons, to appear in February 1999.
18. B. Z. Steinberg and Y. Leviatan, "Periodic wavelet expansions for anal 'sis of scattering
    from metallic cylinders:' IEEE A,切卿5 '가VP昭万oc. Symp., 2小23, 삐le 1994.
 19. G. W. Pan and X. Zhu, "The application of fast adaptive wavelet expansibn method in the
     computation of parameter matrices of multiple lossy transmission lines,' IEEE Antennas
     Propagat. Soc. Symp., 29-32, June 1994.
 20. G. Wang, G. W. Pan, and B. K. Gilbert, "A hybrid wavelet expansion 申nd boundary el-
     ement analysis for multiconductor transmission lines in multilayered (1ielecthc media:'
     IEEE Trans. Microwave Theory Tech., 43, pp. 664-675, March 1995.
 21. W. L. Golik, "Wavelet packets for fast solution of electromagnetic int乍느gral equations,"
     IEEE Trans. Antennas Propag., 46, pp. 618-624, 1998.
 22. 旬光cial Issi妃 on Way毗ts in Elec的magne出s, mt. / Numer. !化del. 月Id
      Devices Fields, 11, 1998.
                                                                      REFERENCES        299


23. J. C. Goswami, A. K. Chan, and C. K. Chui, "On solving first-kind integral 叫uations
    using wavelets on a bounded interval," 旭EE Trans. Antennas Propag., 43, pp. 614-622,
    1995.
24. J. C. Goswami, A. K. Chan, 缸ld C. K. Chui, "Spectral domain analysis of single and cou-
    pie microstrip open discontinuities with anisotropic substra把5," 伍万El｝口月且 Micro叩口ye
    Theory Tech.,44, pp. 1174-1178, 1996.
25. J. C. Goswami and R. Mittra, "Application of FDTD in studying the end effects of slot
    line and c아danar waveguide with anisotropic substrate," JE万 Tran且 Mi口V叩口ye Thee가y
    Tech., 45, pp. 1653-1657, 1997.
26. I. Daubechies, Ten Lectures on Wavelets. CBMS-NSF Ser. Appl. Math. 61, Philadelphia:
    SIAM, 1992.
27. C. K. Chui and E. Quak, "Wavelets on a bounded interval,'' in Nu比rical Mathem口tics
    Approximation Theory, Vol. 9, D. Braess and L. L. Schumaker (eds.). Basel: Birkhuser
    Verlag, 1992, pp. 53-75,                    .
28. E. Quak and N. Wey加h, "Decomposition and reconstruction algorit그ms for spline
    wavelets on a bounded interval," App!. Compu. Harmon. 凡1al., 1, (3), pp. 217-23 1, June
    1994.
29. A. Cohen, I. Daubechies, and P. Vial, "Wavelets on the interval and fast wavelet trans-
    form," Appl. Comput. Harmon. An口l., 1, 1, pp. 54-81, December 1993.
30. P. Auscher, "Wavelets with bound町y conditions on the interval," in Wavelets:. A Tutorial
    in Theory and Applica卄ons, C. K. Chui (ed.). San Diego, Calif.: Academic Press, 1992,
    pp. 217-236.
31. C. de Boor, A Practical Guide to Splines. New York: Springer-Verlag, 1978.
32. R. F. Harringto凡 Time-月切勿lon&? 月lect凡功m甲妃吐c Fields. New York: McGraw-Hill Bosh
    Company, 1961.
33. C. K. Chui and J. Z. Wang, "High-order orthonormal scaling functions and wavelets give
    poor time-frequency localization," Fourier An끄. App!., pp. 415나26, 1996.
34. W. Hackbusch, Mu!啣ridA佃加小 and肉刎ic口tion工 Ne텍 York: Springer-Verlag, 1985.
35. A. Brandt, "Multi-level adaptive solutions to bound띠：y value problems," Math. Comput.,
    31, pp. 33小390, 1977.
36. W. L. Briggs, A Multigrid Tutorial. Philadelphia: SIAM, 1987.
37. S. Dahlke and I. Weinreich, 'Wavelet-Galerkin methods: An adapted biorthogon키
    wavelet basis,' Constr Approx., 9, pp. 237-262, 1993.
38. W. Dahmen, A. J. Kurdila, and P. Oswald (eds.), Multiscale Wavelet Methods for Partial
    D刃色肥ntia/ 方qu口ti이玎． San I거ego, Calif.: Academic F노ess, 1997.
39. H. Yserentant. "On the multi-level splitting of finite element spaces," Numer Math., 49,
    pp. 379나12, 1986.
40. J. Liandrat and Ph. Tchamitchian, "Resolution of the lD regularized Burgers equation us-
    ing a spatial wavelet approximation:' NASA Repo月, ICASE, No. 90-83, December 1990.
41. R. Glowinski, W. M. Lawton, M. Ravachol, and E. Tenenbaum, "Wavelet solution of lin-
    ear and nonlinear elliptic, parabolic, and hyperbolic problems in one space dimension,"
    in Computing Methods in Applied Sciences and Engineering, R. Glowinski and A. Lich-
    newsky (eds.), Philadelphia: SI사14, 1990, pp. 55-120.
42. P. Oswald, "On a hierarchical basis multilevel method with nonconforming P1 elements,"
    Numer Math., 62, pp. 189-212, 1992.
300      WAVELETS IN BOUNDARY VALUE PROBLEMS


43. W. Dahmen and A. Kunoth, "Multilevel preconditioning," Numer Math., 63, pp. 315-
    344, 1992.
44. P. W. Hemker and H. Schippers, "Multiple grid methods for the solution of Fredholm
     integral equations of the second kind," Math. Comput., 36, Janu川y 1981.
45. S. Ja卄ard, "Wavelet methods for fast resolution of elliptic problems," SIAM J. Numer
     Anal. 29, pp. 965-986, 1992.
46. S. Ja卄ard and Ph. Lauren9ot, "Orhonomal wavelets, anlysis of operators, and applications
     to numerical analysis:' in Wavelets: A Tutorial in Theory and Applications, C. K. Chui
     (ed.). Boston: Academic Press, 1992, pp. 543而01.
47. J. Xu and W. Shann, 'Galerkin-wavelet methods for two-point boundary value problems,'
    Numer Math. 63, pp. 123-144, 1992.
48. C. Guerrini and M. Piraccini, "Parallel wavelet-Galerkin methods using adapted wavelet
    packet bases," in Wavelets and Multilevel Approximation, C. K. Chui and L. L. Schu-
    maker (eds.) New Jersey: World Scientific, 1995, pp. 133-142.
49. M. Krumpholz and L. P. B. Katehi, "MRTD: new time-domain schemes based on mu!-
    tiresolution analysis," IEEE Trans. Microwave Theory Tech., 44, pp. 555-571, 1996.
50. E. Bacry, S. Mallat, and G. Papanicolaou, "A wavelet based space-time adaptive numer-
    ical method for partial differential equations," Math. Model. Numer Anal., 26, pp. 793-
    834, 1992.
51. C. K. Chui, An Introduction to Wavelets. San Diego, Calif.: Academic 까ess, 1992.
52. C. K. Chui, Multivariate Splines. CBMS-NSF Ser. App!. Math. 54. Philadelphia: SIAM,
    1988.
Index



Acoustic signals, 221                   local, 13, 272
Adaptive resonance theory, 248           orthonormal. 11
Admissibility condition, 69             Riesz, 13
시gorithms:                               semiorthogonal, 11
   CAD, 244                             stable, 15
   computer programs, 184, 258, 263     subdornain, 272
   decomposition, 149                 Battle-Lemarie wavelet, 123
   FF1-based. 200                     Bernstein polynomial, 295
   filter bank. 141                   Best basis selection, 220
  marching, 257                       Binary phase-shift key, 252
  pyramid decomposition, 210          Binary scales, 187
  reconstruction. 153                 Binomial theorem, 136
   three-dimensional wavelet, 255     Biorthogonal basis, 11
   two-dimensional wavelet, 233       Biorthogonal decomposition, 93
   wavelet packet, 210, 212, 234      Biorthogonal filter bank, 174
   zero-tree. 236                     Biorthogonality condition, 93, 179
Aliasing, 143                         Biorthogonal wavelets, 95, 108, 129
Ambiguity function, 83                  Cohen, Daubechies, and Feaveau, 130
Analyzing wavelet, 94                 Bit plane coding, 235
Antialiasing condition, 174, 184      Boundary condition, 269
Approximation subspace, 148           Boundary value problems, 267
Arithmetic code. 235                  Boundary wsvelets, 281
ART, 248                              Bounded intervsl, 280
Autocorrelation, 95, 135, 149         BPSK, 252
Averaging filter, 25                  B-斗小ne, 45
                                      BVP, 267
Basis functions, 9
  biorthogonal, II                    CAD algorithm, 244
  dual, 11                            Cardinal B-splines, 112
  entire-domain, 272                  Causal filter, 176
  global, 272                         Causality, 176
  Haar, 13                            Centered integral wavelet transform, 196

                                                                                 301
 302      Ir니［:)［三x

 Change of bases, 21, 154, 157, 160           Digital signal processing, 210
 Chirp signal, 68, 204                        Dilation (refinement) equation 91
 Chui-Wang wavelet, 112                       Dilation parameters, 69
 CIWT, 196                                    Direct sum, 91
 Cluster detection, 244                       Direction decomposition, 210
 Coding:                                      Direct-sum decomposition, 91
    arithmetic, 235                           Dirichlet kernel, 55
   bit plane, 235                             Discontinuity problem, 276
   entropy, 238                               Discrete Fourier basis, 50
   EZW, 238                                   Discrete Fourier transform, 54
   I-luffman, 235                             Discrete Gabor representation, 65
   image, 235                                 Discrete short-time Fourier tr出lsform, 64
   lossy, 235                                 Discrete-time Fourier transform, 52
   predictive, 235                            Discrete wavelet transform, 67 72
   runlength, 235                             Dispersive nat工re, 205
   wavelet tree, 236                          1兀pp岫，83
Cohen, Daubechies, and Feaveau wavelet, 130   Doppler frequencies, 165
Coiflets, 137                                 DTFT, 52
Comb function, 33                             Dual basis, II
Computer programs:                            Duality, 93
  B-spline, 106                               Duality principle, 155
   I -D algorithm, 184                        Dual scaling function, 157
  2-D algorithm, 258                          Dual spline, 154
  iterative method, 139                       Dual wavelet, 93
   short-time Fourier transform, 85           DWT, 67, 182
   wavelet, 138                               Dyadic points, 156, 187
   wavelet packet, 263
  Wigi硏-Ville distri加如n, 86                   Edge effect, 281
Condition number, 291                         Eigenmatrix, 19
Contini工ous wave노ttrans拓rm. 67                Eigensyatem, 19
Conventional bases, 273                       텨genv曲Se, 19
Cos싸entional M아vi, 268                        Eigenvalue method, 134
Coi싸이ution, 24, 39, 147                       Eigenvectors, 20
Corner smoothing functions, 120               타ec甘oma帥etic scattering, 268
Correlation function, 81                      Elliptic PDEs, 295
Crack detection. 202                          Embedded zerotree wavelet, 238
Critical sampling, 150                        Entire-domain basis, 272
Cubic spline, 159, 162                        Entropy coder, 238
Cut-off frequency, 205                        Error considerations, 282
CWT, 67, 150                                  Euclidean vector space, 7
                                              Euler Frobenius Laurent polynomial, 108, 114,
Dan妃Is이land Lanczos, 55                               157
Daubechies, 211                               Evolution problems, 295
Daubechies' orthogonal filters, 176           EZW, 238
Daubechies wavelet, 125
DCT, 245                                      False positives, 249
Decimation, 142, 147                          Fast integral transform, 187
Decomposition relation, 97, 151               Faulty bearing, 221
Design origin, 183                            Feature extraction:
Determinant. 19                                 spectral, 227
DFT, 55                                         wavelet packets, 227
I거什erential equatiol心，294                       wavelets, 226
Differential operator, 272                    FEM, 294
Differentiating filter, 25                    FFT, 55. 226
                                                                               INDEX      303


FFT-based algorithm, 200                       Hard thresholding, 216
Filter bank, 141, 180                          Hat function, 84
Filter bank algorithms, 141                    HBF, 172
Filters:                                       Hermitian matrix, 22
   averaging, 25                               Hierarchical methods, 294
   biorthogonal, 174                           Hierarchical wavelet decomposition, 211
   causal. 176                                 High frequency methods, 294
   differentiating, 25                         Highpass filter, 25
   filter bank, 141, 180                       Hist唯ram t뇨esh이小ng, 248
   FIR, 114, 156, 172                          Huffman code, 235
   half-band, 172
   HBF, 172                                     Identity matrix, 19
   highpass, 25                                 lIR filters. 114, 172
   IIR, 114, 172                                Image coding, 235
   lowpass, 25, 102                             Image compression, 210, 235
   noncausal symmetric, 172                     Image visualization, 210
   perfect reconstruction, 177                  Impedance matrix, 271
   PR condition, 167, 184                       Inner product, 8
   PR filter bank, 166, 182                     Integral equations, 268
   PR requirements, 177                        Integral operator, 272
   QMF, 171                                    Integral wavelet transform, 67
   quadrature mirror, 171                      Interference suppression, 210, 219
   smoothing, 25                               Interoctave approximation subspaces, 194
   two-channel biorthogonal filter bank, 179   Interoctave parameter, 190
Finer scale resolution, 190                    Interoctave scales, 190
Finer time resolution, 188                     Interpolation, 144, 147
Finite element method, 294                     Interpolator, 145
Finite-energy function, 90                     Interpolatory representation, 103
FIR filters, 114, 156, 172                     Ii如叩retations, 74
First-kind integral equation, 268              Intervallic wavelets, 281
FIWT, 196                                      Inverse, 19
Fourier method, 31                             Inverse wavelet transform, 69
Fourier series, 31                             Inversion formula, 61
Fourier series kemel, 34                       Iteration method. 132
Fourier transform, 35                          IWT, 67
FPs. 249
Frequency scaling, 38
                                               Knot sequence, 281
Frequency shifting, 38, 63
Functional, 5
                                               Linear function. 197
Gabor transform, 61                            Linear operator, 272
Galerkin method, 272, 274, 279                 Linear phase, 171
Gaussian function, 42, 103                     Linear spaces, 5
Generalized linear phase, 171                  Linear spline, 159, 162
Generalized self-similarity tree, 244          Linear transformation, 18
Gibb's phenomenon, 50                          Linearity, 37, 62
Global basis, 272                              Local basis, 13, 272
Graphical display, 132                         Logarithmic division, 220
GST, 237                                       Lossy coding, 235
                                               Lowpsss filter, 25, 102
Haar, 96
Haar basis, 13                                 Mammogram, 244
Haar wavelet, 105                              Marching algorithm, 257
Half-band filter, 172                          Marginal properties, 80
  304      it비가沃


  Matrix:                                        Orthogonal decomposition, 10, 92
     determinant, 19                             Orthogonal frequency division multiplexing,
     eigenmatr奴, 19                                     250
     eigensystem, 19                             Orthogona냐的畔t幻n, 16, 148
     eigenvalue, 19                              O出sonom俎I basis. 11
    eigenvectors, 20                             Orthonormalization, 14
    Hermitian, 22                                Orthonormal scaling function, 118, 212
    identity, 19                                 Orthonormal wavelets, 108, 114
    inverse, 19
   minor, 19                                    Psrseval identity, 157
    singular, 19                                Parseval's theorem, 40
    sparse, 273                                 Partial sum, 35, 49
   transpose, 18                                Partition of unity, 45, 102, 281
   unitary, 23                                  Pattern recognition, 221
 MCCS, 250                                      PDE. 267
 入1ean s（和are error, 16                         Percentage thresholding, 218
 Medical image visualization, 252               Perfect reconstruction, 177
 Method of moments, 268, 272                    Periodic wavelets, 281
 Meyer Wavelet, 119                             Photonegative x-ray, 244
   corner smoothing functions, 120              Piecewise sinusoids, 276
 Microcalcifications, 244                      Plane wave, 269
Minor, 19                                      Point matching, 272
入4아느4, 268                                     Poisson's sum. 35, 43
Moment property, 200                           Polynomial reproducibility, 103
Moments, 38                                    Polyphase domain, 180
Morlet wavelet, 71                             Polyphase representation, 180
Moving average, 24                             POS, 238
MRA, 89, 151                                   PR condition, 167, 184
MRA space, 103                                 Predictive coding, 235
Multicarrier communication systems, 210, 249   PR filter bank, 166, 182
Multivoice per octave, 187                     Processing domain, 182
卜vi山tigrid, 294                                Processing goal, 183
Multiresolution analysis, 89                   Product filter, 175
Multiresolution spaces, 89                     Projection, 8
Music signal, 204                              PR requirements. 177
MVPO, 187                                      P砥요 276
                                               Pyramid decomposition, 210
NEG, 238
Neural network, 223                            （外4F, 171
Noise reduction, 210                           Quadratic chirp, 82
Noncsussl symmetric filter, 172                Quadratic superposition principle, 81
Nondyadic points, 187                          Quadrature mirror filter, 171
Nonlinear contrast enhancement, 245
Nonlinear ti毗寸requency 毗tn加如ns, 2四             Radar cross section, 270
Norm, 6                                        Radar imaging, 82
Normalization factor, 155                      RCS, 270
Nosmed linear space, 6                         Reconstruction algorithm, 153
Nyquist rate, 47                               Reconstruction process, 164
                                               Rectangulsr time-scale grid, 193
Octave levels, 191                             Region of convergence, 26
ODE, 294                                       Rendering techniques, 256
OFDM, 250                                      Riesz basis, 13
Order of approximation, 102                    Riesz 1兀un小！14, 114
Orthogonal, 92, 291                            Riesz lemma, 127
                                                                             INDEX        305

RMS bandwidths, 191                        Target identification, 210
Runlength code, 235                        Testing 凡llctions, 272
                                           Thin strip, 270
Sampling, 23                               Thin wire, 270
Sampling theorem, 35, 46                   Three-dimensional wavelets, 255
Scalar product, 8                          Thresholding, 205, 214, 275, 282
Scaling function, 91                          hard, 216
Scattered electric fields, 269                histogram, 248
Second-kind integral equations, 273           percentage, 218
Semiorthogonal, 92, 108, 291                  soft, 217
Scm油卄ogona比as奴 II                          Time-dom帥 analys奴 176
Semiorthogonal decomposition, 95           Time-domain biothogonal condition, 179
Scm油th昭on키 叩line way이ets, 112              Time-frequency analysis, 57
Semiorthogonal subspaces, 154, 156            continuous wavelet transform, 67
Shannon 凡nc如n, 13                             discrete Gabor representation, 65
Shannon wavelet, 118                          discrete short-time Fourier transform, 64
앍iift-invanant sys把ms, 24                     discrete wavelet transform, 67, 72
Short-time Fourier transform, 60              Gabor transform, 61
Signal representation, 148                    integral wavelet transform, 67
Signature identification, 210, 221            short-time Fourier transform, 60
Singular matrix, 19                           time-丘口神이托y window, 62
引ots, 276                                     time-frequency window, 70
Smoothing filter, 25                          time-frequency window product, 60, 279
Smoothing 凡ncti(月i, 120                       uncertain勺 principle, 60
鈿ftt뇨esh이di略 2l7                              wavelet series, 73
SOT, 237                                   Time-frequency window, 62, 70
Space-time adaptive method, 295            Time-frequency window product, 60, 279
Sparse matrices, 273                       Time-scale analysis, 69
Sparsity, 282                              Time-scale grid, 187
Spatial oriented tree, 242                 Time-scale map, 150
Spectral-domain analysis, 168              Time scaling, 38
Spectral domain methods, 275               Time shifting, 38, 63
Spectral feature extraction, 227           Tonal equalizer, 165
Spectral method, 132                       Total positivity, 102, 275
Spline functions, 98                       TP, 249
Splines. 45                                Translation, 69
  computer programs, 106                   Transn小計이lline, 276
  cubic, 159, 162                          Transmission line discontinuity, 276
   linear, 159, 162                        Transpose, 18
  properties, 102                          Transverse magnetic, 269
Spline wavelets, 160                       Tn妃 posit加es, 249
Splitting method, 211                      Two-channel biorthogonal filter bank, 179
Stable basis. 15                           Two-channel perfect reconstruction, 165
Stable numerical scheme, 295               Two-dimensional wavelet algorithm, 233
Standard wavelet decomposition, 149, 189   Two-dimensional wavelet packets, 231
STFT, 58, 67                               Two- dimensional wavelets, 228
Strang-Fix condition, 102                  Two-scale relations, 96, 153
Strips, 276
Subdomain basis. 272                       Uncertainty principle, 60
Surface current distribution, 269          （力lit쾨ymatrix, 23
Synthesis transform, 153                   Unitary similar, 273
Synthesis wavelet, 94
                                           Vanishing moments, 69, 275, 285
Target detection, 210                      Vector spaces, 7
306      爪DEX


Waveguide, 205                                  two-dimensional, 228
Wavelet coefficient, 150, 246                  Wavelet series, 73
Wavelet decomposition, 149, 245                Way毗ts此spaces, 154
Wavelet feature extraction, 226                Way이et t吼hn띠出s, 273
Wavelet MoM, 268                               Wavelet tree coder, 236
Way毗印acket a培orithms, 기0, 212, 234             Weighting functions, 272
Wavelet packet based cross-term deleted        Wideband correlation processing, 187
       representation, 220                     Wigner-Ville distribution, 76, 83, 219
Wavelet packet feature extraction, 227          auto term, 80, 220
Wavelet packets, 84, 152, 211, 226, 252, 280    cm仰毗r pro酊ams, 86
Wavelet packet tree decomposition, 210          cross term. 80, 220
Way이炚5.                                         properties, 80
 Battle-Leman, 123                              wavelet packet based cross-term deleted
 biorthogonal, 129                                   representation, 220
 boundary, 281                                  WPCDR, 220
 Chui-Wang, 112                                Window 鈿ction, 58
 Cohen, Daubechies, and Feaveau, 130            center, 59
 coiflets, 137                                  radius, 59
 Co呻uter progran瑀 138, 139                      time丘equ巴乂y window, 62
 Daubechies, 125                                time卄equency 텍indow 皿oduct, 60
 graphical display, 132                         uncertainty principle, 60
 Haar wavelet, 105                               width, 59
 intervallic, 281                              WPCDR, 220
 入4eyer, 119                                   WS, 73
 Morlet, 71
 orthonormal, 108, 114                         Zero-tree algorithm, 236
 periodic, 281                                 ZTR, 238
  Shannon, 118                                 z-transform, 25
 斗小ne, 112                                        inverse z-transfonn, 28
  three-dimensional, 255                          region of convergence, 26
