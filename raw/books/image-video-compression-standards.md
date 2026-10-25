---
source_url: /run/media/yutae/Data/Image_Video_Compression_Standards.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: dbe324ec269120171a584d21f8c81d91b4fdb20e80f112f8b2ce368d0d55d86d
---
# Image and Video Compression Standards: Algorithms and Architectures (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출 (~861,798 chars). 일부 토큰은 인식 오류로 깨짐 (한/영 혼용 OCR 산출). 원문 PDF(`books/Image_Video_Compression_Standards.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Image and Video Compression Standards: Algorithms and Architectures
- authors: Vasudev Bhaskaran, Konstantinos Konstantinides (Hewlett-Packard Laboratories)
- edition: 1st, second printing 1996
- year: 1995
- publisher: Kluwer Academic Publishers (Boston / Dordrecht / London)
- pages: 371 (pdfinfo)
- scope: JPEG, MPEG-1/2, H.261, MPEG/Dolby AC-3 audio, wavelets/VQ
+ source file: `Image_Video_Compression_Standards.pdf` (sha256: `dbe324ec26912017…`)
+ extract: `pdftotext -layout` @ 2026-10-25, 861,798 chars

## Chapter structure (from TOC)
| # | topic | page |
|---|-------|------|
| 1 | Compression Fundamentals — taxonomy, selection issues | 1 |
| 2 | Lossless Compression — Huffman (Voorhis), arithmetic, JPEG lossless, Group 3/4, JBIG | 15 |
| 3 | Lossy Image Compression — rate-distortion, DCT coding, fast DCT | 53 |
| 4 | Lossy Video Compression — motion estimation/compensation, sub-pel | 87 |
| 5 | The JPEG Standard — DCT, quant tables, entropy, modes, extensions | 129 |
| 6 | The MPEG Video Standards — MPEG-1 & MPEG-2 coding + syntax | 161 |
| 7 | The H.261 Video Coding Standard | 195 |
| 8 | Processing Requirements — complexity measures, load distribution | 207 |
| 9 | RISC and DSP Cores | 215 |
| 10 | Architectures for the DCT — vector, distributed arithmetic | 225 |
| 11 | Hardware for Motion Estimation | 237 |
| 12 | Hardware for Entropy Coding | 249 |
| 13 | Implementation of JPEG Processors | 263 |
| 14 | Integrated Circuits for Video Coders | 271 |
| 15 | Multimedia Enhancements for RISC (HP-PA, UltraSPARC) | 289 |
| 16 | Standards for Audio Compression — MPEG audio, Dolby AC-3 | 297 |
| 17 | Nonstandard Techniques — VQ, subband coding | 315 |
| A/B | Abbreviations, Internet Directory, References, Index | 335-371 |

## Original text (all 372 pages)

                 IMAGE AND VH)EO
             COMPRESSION STANDARDS
              Algorithms and Architectures




                      Vasudev Bhaskar
                  Konstantinos Konstan
                  Hewle玎下口ckard Laboratories




                                              Quantization    Entropy
                                  DCT   Hm令


                                                             Enc以抑四


                                                Inverse
                                              Quantization


1
    Motion
                                                Inverse
                                                  DCT
1댜少"""'"


                      M아幻n                      다an祀
                   Compensation                 Memory
             느a
嘴
1心느
  i
   IMAGE AND VIDEO
COMPRESSION STANDAR冷
 A臼01亡力msa兀dArc力初ectures




               by



     Vasudev Bhaskaran
 Konstantinos Konstantinides
 月ewlet卜J）       口bor口tories
         口ckard I，




             的
   KU八VER ACAD目4IC PUBLIS王JERS
      Boston I Dordrecht / London
Distributors for North America:
Kiuwer Academic Publishers
101 Philip Drive
Assinippi Park
Norwell, Massachusetts 02061 USA

Distributors for all other countries:
Kiuwer Academic Publishers Group
I가stributi이i Centre
Post Office Box 322
3300 AH Dordrecht, THE NETHERLANDS




Library of Congress Cataloging-in-Publication Data

A C.I.P. Catalogue record for this book is available
from the Libr出y of Congress.




CopyrightO 1995 by Kluwer Academic Publishers. Second Printing 1996.

All rights reserved. No part of this publication may be reproduced, stored in
a retrieval system or transmitted in any form or by 쏘ly means, mechanical,
photo-copying, recording, or otherwise, without the prior written permission of
the publisher, Kiuwer Academic Publishers, 101 Philip Drive, Assinippi Park,
Norwell, Massachusetts 02061

Printed on acid-free paper.

Printed in the United States of America
                                                 CONTENTS




PREFACE

1   COMPRESSION FUNDAMENTALS                                     l
    1 .1   Introduction                                          l
    1.2 Background                                              2
    1.3 Compression Taxonomy                                    5
    1.4 Issues in Compression Method Selection                  12
    1.5 To Probe Further                                        14

2   METHODS AND STANDARDS FOR LOSSLESS
    COMPRESSION                                                 15
    2.1    Introduction                                         15
    2.2 Preliminaries                                           15
    2.3 Huffman Encoding                                        18
    2.4 Huffman Decodin2                                        22
    2.5    Huffman Codes with Constrained Length                24
    2.6 Constrained-Length Huffman Codes - Ad-Hoc Design        31
    2.7 Constrained-Length Huffman Codes - The Voorhis Method   33
    2.8    Arithmetic Coding                                    37
    2.9 Implementation Issues                                   42
    2.10 Standards for Lossless Compression                     43
    2.11 To Probe Further                                       50

3   FUNDAMENTALS OF LOSSY IMAGE COMPRESSION                     53
    3.1    Introduction                                         53
viii                                  IMAGE COMPRESSION STANDARDS




        3.2   Preliminaries                                    54
        3.3   Basic Coding Schemes for Lossy Compression       60
        3.4   DCT小的ed Codir坦                                   65
        3.5   Fast Algorithms for the DCT                      77
       3.6    Rate-Distortion Performance of the DCT           85
       3.7    To Probe Further                                 85

4      FUNDAMENTALS OF LOSSY VIDEO COMPRESSION                 87
       4. 1   Introduction                                     87
       4.2    Video Coding Basics                              88
       4.3    Rate-Distortion Functions in Video Coding        93
       4.4    Motion-Compensated Prediction                   105
       4.5    A姮orithms 如r入4otion Estin猛lion                  108
       4.6    Sub-pixel-Accurate Motion Estimation            122
       4.7    Multipicture Motion Estimation                  126
       4.8    To Probe Further                                127

5      THE JPEG STANDARD                                      129
       5.1    Introduction                                    129
       5.2    DCT-based Coding                                130
       5.3    Processing of Color Images                      133
       5.4    Design of Quantization Tables                   135
       5.5    Entropy Coding                                  139
       5.6    JPEG Modes of Operation                         145
       5.7    Implementation Issues                           150
       5.8    JPEG Extensions and Applications               154
       5.9    To Probe Further                               157

6      THE MPEG VIDEO STANDARDS                              161
       6.1    Introduction                                   161
       6.2    The MPEG- I Video Standard                     162
       6.3    MPEG-I Implementation Issues                   180
       6.4    The MPEG-2 Video Standard                      182
       6.5    To Probe Further                               193
C아玎ents                                            ix




7    THE H.261 VIDEO CODING STANDARD              195
     7.1 Introduction                             195
     7.2 The H.261 Video Coding Standard          198
     7.3 Implementation Issues                    202
     7.4 Future Directions                        205
     7.5 ToProbe Further                          206

8    PROCESSING REQUI之EMENTS                      207
     8.1 Introduction                             207
     8.2 Measuring Complexity                     208
     8.3 Distributing the Load                    211
     8.4 To Probe Further                         212

9    RISC AND DSP CORES                           215
     9.1 Introduction                             215
     9.2 TheRISCCore                              215
     9.3 The DSPCore                              218
     9.4 RISC versus DSP                          221
     9.5 To Probe Further                         222

10   ARCHITECTURES FOR THE DCT                    225
     10.1 Introduction                            225
     10.2 Vector Processing                       226
     10.3 Distributed Arithmetic for the DCT      228
     10.4 Commercially Available DCT Processors   234
     10.5 To Probe Further                        235

11   HARDWARE FOR MOTION ESTIMATION               237
     11 .1 Introduction                           237
     11.2 Data Flow Design                        238
     11.3 Sub-pel Motion Estimation               243
     11.4 Implementation Examples                 244
     11.5 To Probe Further                        247
x                                   IMAGE COMPRESSION STANDARDS




12   HARDWARE FOR ENTROPY CODING                            249
     12.1 Introduction                                      249
     12.2 Encoder Implementation                            250
     12.3 Decoder Implementation                            253
     12.4 Variable-Length Coding in JPEG                    258
     12.5 To Probe Further                                  259

13   IMPLEMENTATION OF JPEG PROCESSORS                      263
     13.1 Introduction                                      263
     1 3.2 Data I/O and Memory Interface                    264
     13.3 ColorConversion                                   265
     13.4 Commercially Available JPEG Processors            266
     13.5 To Probe Further                                  269

14   INTEGRATED CIRCUITS FOR VIDEO CODERS                   271
     14.1 Introduction                                      271
     14.2 Video Signal Processors                          272
     14.3 Dedicated Coders                                 282
     14.4 To Probe Further                                 286

15   MULTIMEDIA ENHANCEMENTS FOR RISC
     PROCESSORS                                            289
     15.1 Introduction                                     289
     15.2 Generic Operations in Video Processing           290
     15.3 Multimedia Enhancements in the HP-PA             291
     15.4 Multimedia Enhancements in the UltraSparc        294
     15.5 To Probe Further                                 296

16   STANDARDS FOR AUDIO COMPRESSION                       297
     16.1 Introduction                                     297
     16.2 MPEG Audio Encoding                              300
     16.3 MPEG Audio Decoding                              304
     16.4 Layer Coding Options in MPEG                     307
     16.5 The AC-3 Coding Standard                         308
Contents                                             xi




     16.6 Hardware Implementation of Audio Codecs   312
     16.7 To Probe Further                          313

17   NONSTANDARD COMPRESSION TECHNIQUES             315
     17.1 Introduction                              315
     17.2 Vector Quantization                       316
     17.3 Subband Coding                            321
     17.4 Video Coding Schemes for the Desktop      330
     17.5 To Probe Further                          331

A    ABBREVIATIONS AND SYMBOLS                      335

B    INTERNET DIRECTORY                             341

REFERENCES                                          345

INDEX                                               363
                                                        PREFACE



This book presents an introduction to the algorithms and architectures that form
the underpinnings of the image and video compression standards, including
JPEG (compression of still-images), H.261 (video teleconferencing), and
MPEG-i and MPEG-2 (video storage and broadcasting). In addition, the
book covers the MPEG and Dolby AC-3 audio coding standards and emerging
techniques for image and video compression, such as those based on wavelets
and vector quantization.

The emphasis of the book is on the foundations of these standards, namely,
techniques such as predictive coding, transform-based coding, motion esti-
mation, motion compensation, and entropy coding, as well as how they are
applied in the standards. We avoid the implementation details of each standard.
However, we do provide all the material necessary to understand the workings
of each of the compression standards, including information that can be used
by the reader to evaluate the efficiency of various software and hardware
in삐帥妃ntations conf아而旽 to these standards. We place particular e呻hasis
on those algorithms and architectures that have been found to be useful in
practical software or hardware implementations.

No prior knowledge of image and video compression theory and architectures
is assumed; however, some background in high-level hardware design is
expected for the better understanding of the chapters covering the hardware
implementation of the standards.

Chapters 1 to 4 review the fundamentals of image and video compression. In
Chapter 1 we cover the key principles of image compression and explain the
basic terminology. We present a compression taxonomy and discuss design
issues and tradeoffs in selecting a compression algorithm. In Chapter 2 we
review methods and standards for lossless compression, including differential,
Huffman, and arithmetic coding. We present several practical algorithms for
the design of Huffman codes, and we describe the lossless JPEG algorithm
xiv                                 IMAGE COMPRESSION STANDARDS




and the standards for lossless facsimile transmission (Group 3, Group 4, and
JBIG). In Chapter 3 we examine techniques for lossy compression. We
review the source-coding theorem and compute the rate-distortion function
for several image models relevant to image compression. We place particular
emphasis on DCT-based coding, and describe several schemes for the efficient
implementation of the DCT. In Chapter 4 we present the fundamentals of
video coding, including motion estimation and motion compensation.

In Chapter 5 we describe JPEG and its application to the compression of still-
images. We cover recent extensions to JPEG and the JPEG-based standard for
color facsimile. In Chapter 6 we describe the coding algorithms and syntax
for the MPEG- i and MPEG-2 video compression standards, and in Chapter
7 we provide an overview of the H.261 standard for video teleconferencing.
Similarities and differences among these video compression standards are also
presented and reviewed.

Next, we move to the hardware implementation of the standards. In Chapter
8 we define a measure of computational complexity, and we use it to measure
the complexity of various algorithms used in the standards. Bearing in mind
that most hardware implementations of the standards are based on either RISC
or DSP cores, in Chapter 9 we review the principles of RISC and DSP designs
and describe their main differences and similarities. Even though we present
the latest designs in image and video processors, we place more emphasis
on the designs of the core algorithms; that is, the discrete cosine transform
(Chapter 10), motion estimation (Chapter Il) , and entropy coding (Chapter
12). In Chapter 13 we describe architectures for the JPEG standard, and in
Chapter 14 we discuss programmable and dedicated video processors for the
MPEG and the H.261 standards.

In Chapter 15 we review recent developments in the design of multimedia-
enhanced general-pu恥se RISC processors, such as the PA7IOOLC from
Hewlett-Packard and the UltraSPARC from Sun Microsystems. In Chapter
16 we present the key standards on audio coding, and we describe in more
detail the MPEG and Dolby AC-3 coding schemes. In Chapter 17 we provide
an overview of techniques based on vector quantization and wavelets. Such
techniques are used in many proprietary image and video compression schemes
and may play a significant role in future standards.
Preface                                                                      xv




Appendix A provides a summary of abbreviations used in the text and can be
used as a quick reference for the various standard image formats (SIF, CIF,
and CCIR 601). Information about sites with public software implementations
of the standards is included in Appendix B.

The material in this book is partitioned into the following categories: fun-
damentals, video standards, architectures, audio standards, and emerging
techniques. However, most of the chapters are self contained and allow the
reader to easily switch from one category to another.

This book is aimed at the professional who wants to have a basic understanding
of the latest developments and applications ofimage compression standards. It
is based on tutorials given by the authors at several forums, including the IEEE
International Conference on Acoustics Speech and Signal Processing, the
ACM Multimedia Conference, and Hewlett-Packard. It provides a reference
for any engineer planning to work in this field, either in basic implementation
or in research and development. It is intended for self-study; however, it can
also be used as a companion textbook in any course on data compression,
video coding,computer architecture, signal or image processing, or the design
of signal and video processors.

Acknowledgments.This book would not be possible without the support from
the management at Hewlett-Packard Laboratories, especially Fred L. Kitson,
Daniel T. Lee, and Ho John Lee. We also thank our colleagues at Hewlett-
Packard for many helpful discussions. Balas K.Natarajan has been particularly
helpful from the beginning of this project and we thank him for many valuable
discussions, comments, and for reviewing parts of this manuscript. We thank
Bob Rau for his comments on our tutorials and Ruby Lee for providing us
with a different perspective on the hardware implementation of the video
standards. We thank Nariman Farvardin and David Daut for their comments
on the computation of the rate-distortion function. We thank Akio Yamamoto
for his help in the example on wavelet coding,Jos Fridman for many valuable
comments and suggestions, and Elias Manolakos.

We also thank Robert Holland, Jr. and his staff from Kiuwer Academic Press
for their support, and Suzanne M. Rumsey for helping with many typesetting
questions. Finally, we dedicate this book to our teachers and to our families,
and especially to Achan, Chechi, Balu, Kishore, Shanti, Paula, Anastasia, and
Anneta.
                                                                                 1
       COMPRESSION FUNDAMENTALS




     1.1 INTRODUCTION
                                                                     ts in algorithms and
       In recent years, there have been significant advancemen
                                                                   audio signals. These
       architectures for the processing of image, video, and
                                                                        On the algorithm
       advancements have proceeded along several directions.
                                                                        fl喊如ds t아educe
       front, new techn自ues have led to如devel啣妃ntofi｝加St
                                                                   ds are extremely vital
       the size of the image, video, or audio data. Such metl16
                                                                  l data. Informally, we
       in many applications that manipulate and store digita
                                                                        ss. We will define
        refer to the process of size reduction as a compression proce
                                                                   ecture front, it is now
        th's rocess in a more formal way later. On the archit
                                                                                  low-cost
"" " "         I ,to put sophisticated compression processes on a relatively
                                                                  devel  oping multim  edia
        single chip; this has spurred a great deal of activity in
        systems for the large consumer market.
                                                               ts is that multimedia
      One of the exciting prospects of such advancemen
                                                                  potential to become
      information comprising image, video, and audio has the
                                                                edia information will
      just another data type. This usually implies that multim
                                                            , stored, and transmitted
      be digitally encoded so that it can be manipulated
                                                              usage to be p rvasiv 只姿b1．屯
      along with other digital data types. For such data
                                                                   different platforms
      it is essential that the data encoding is standard across
                                                              opment of applications ...
       and applications. This will foster widespread devel
                                                      systems fr帥 缸ferent endor .此 싸勿"
       and will 카so promote 蜘啣解劇2幽配among
                                                                   nt of cost-effective
       Furthermore. standardizatioi硫r 1 d to the developme
                                                                           multimed白
      上끄힌與ientati            ch in turn will p四mote the widespread use of
  2                                                                CHAPTER 1




  information. This is the primary motivation behind the emergence of image
  and video compression standards.




  1.2 BACKGROUND
 Compression is a process intended to yield a compact digital representation
 of a signal. In the literature, the terms source coding, data compression,
 bandwidth compression, and signal compression are all used to refer to the
 process of compression. In the cases where the signal is defined as an
 image, a video stream, or an audio signal, the gqnr,c problem of compression
 is to minimize the bit rate of their digital representation. There are many
 applications that benefit when image, video, and audio signals are available in
 compressed form. Without compression, most of these applications would not
 be feasible.

 Example 1: Let us consider facsimile image transmission. In most facsimile
 machines, the document is scanned and digitized. Typically, an 8.5 x 11
 inches page is scanned at 200 dpi; thus, resulting in 3.74 Mbits. Transmitting
 this data over a low-cost 14.4 kbits/s modem would require 5.62 minutes. With
 compression, the transmission time can be reduced to 17 seconds. This results
 in substantial savings in transmission costs.

 Example 2: Let us consider a video-based CD-ROM application. Full-motion
 video, at 30 fps and a 720 x 480 resolution, generates data at 20.736 Mbytes/s.
 At this rate, only 31 seconds of video can be stored on a 650 MByte CD-ROM.
 Compression technology can increase the storage capacity to 74 minutes, for
 VHS-grade video quality.

 There are many other applications that benefit from data compression technol-
 ogy. Table 1.1 lists a representative set of such applications for image, video,
 and audio data, as well as typical data rates of the corresponding compressed
 bit streams. Typical data rates for the uncompressed bit streams are also
 sho＼人／n.

山l世ge, video, and audio signals are     ble to compression due to these
 factors:                           삯幷뇨
Compression Fundamentals                                                               3




                          Application                      Data Rate
                                                   Uncompressed  Compressed
                                                                                                               뇨
                                                        64 kbps      2 - 4 kbps                           1J
                                                                                       人二


   Voice
                                                                                       hJ             N




  8 ksamples/s, 8 bits/sanpie                                                          h                   r
                                                                                                           1니
                                                                         8 - 16 kbps           5\ J
                                                                                           1

                                                        5.07 Mbps
                                                                                                      人
                                                                                                                h
  Slow-motion video (10 fps)
                                        J
                                                                                                                    1
  framesize 176 x 120, 8 bits/pixel
   Audio conference                                        64kbps       16- 64kbps
   8 ksampies/s, 8 bits/sample
   Video conference (15 fps)                           30.41 Mbps      64- 768kbps     4n卜, V '：나


  力a枇size 352 >< 240, 8 bitm滋el
   I거gital audio (stere이                                  1.5 Mbps    128- 1.5Mbps
   44.1 ksa片iples／노 /6 bits／뇨imple
    Video file transfer (15 fps)                       30.41 Mbps           384 kbps
  戶口'nesize 352 >< 240, 8 bits巾ixel
   I乂gital 미deoon CD-RU卜A (30 fps)                     60.83 Mbps       1.5 - 4 Mbps
  戶口枇size 352 >< 240, 8 b加S巾八el
   Broadcast video (30 fps)                           248.83 卜느4bps       3 - 8 Mbps
  戶口枇5比e 720 >< 480, 8 bits/pi工el
    HDTV (59.94 fps)                                     1.33 Gbps          20 Mbps
   戶口枇size 1280 >< 720, 8 bits/pixel

     Table 1.1                Applications for image, video, and audio compression.



    There is considerable statistical redundancy in the signal.

      1. Within a single image or a single video frame, there exists significant
         correlation among neighbor samples. This correlation is referred to
         as spatial correlation.
      2. For data acquired from multiple sensors (such as satellite images),
         there exists significant correlation amongst) samples from these
         sensors. This correlation is referred to as spectral correlation.
      3. For temporal data (such as video), there is significant correlation
         amongst samples in different segments of time. This is referred to as
         te叫刃r口／correlation.

     There is considerable information in the signal that is 虹 jev與｝t from a
     perceptual point of view.
       7n
            '   1,   ".
   4                                                                                CHAPTER 1




        Some data tends to have high-level features that are redundant across
        space and time; that is, the data is of a fractal nature.


   For a given application, compression schemes may exploit any one or all of
   the above factors to achieve the desired compression data rate.

   A systems view of the compression process is depicted in Figure 1.1. The core


                                                              ENCODER


           Digital Image, Video,            1       Source              Channel
                                        늬                               m



           and Au비O
                                   H｛
                                                     Coder                  Coder




                                                              DECODER


           Digital Image, Video,            1       Source           Channel
                                        니                               H



           and Audio
                            <m1＝
                                                    Decoder          Decoder
                                                              <eH
                       Figure 1.1 Generic compression system.


   of the encoder is the source coder. The source coder performs the compression
,,process by reducing the input data rate to a level that can be supported by the
   storage or transmission medium. The bit rate output of the encoder is measured
   in bits per sample or bits per second. For image or video data, a pixel is the
   basic element; thus, bits per sample is also referred to as bits per pixel or
   bits per pcI. In the literature, the term compression ratio, denoted as Cr, is
   also used instead of bit rate to characterize the c旦pability of the compression
 寸system. An intuitive definition of cr is

                                                so工rce coder inp比 size
                                   Cr ：二二
                                                source coder output size
  This definition is somewhat ambiguous and depends on the data type and the
  specific compression method that is employed. For a still-image, size could
Compression Fundamentals                                                         5




refer to the bits needed to represent the entire image. For video, size could refer
to the bits needed to represent one frame of video. Many compression methods
for video do not process each frame of video; hence, a more commonly used
notion for size is the bits needed to represent one second of video.

In a practical system, the source coder is usually followed by a second level
of coding: the channel coder (Figure 1.1). The channel coder translates the
compressed bit stream into a signal suitable for either storage or transmission.
In most systems, source coding and channel coding are distinct processes. In
recent years, methods to perform combined source and channel coding have
also been developed. Note that, in order to reconstruct the image, video, or
audio signal, one needs to reverse the processes of channel coding and source
coding. This is usually performed at the decoder.

From a systems design viewpoint, one can restate the compression problem
as a bit rate minimization problem, where several constraints may have to be
met, including the following:


1    Specified levels of signal quality. This constraint is usually applied at the
     decoder.

     Implementation conplexity. This constraint is often applied at the
     decoder, and in some instances at both the encoder and the decoder.

     Communication delay. This constraint refers to the end to end delay, and
     is measured from the start of encoding a sample to the complete decoding
     of that sample.


 Note that, these constraints have different importance in different applications.
 For example, in a two-way teleconferencing system, the communication delay
 might be the major constraint, whereas, in a television broadcasting system,
 signal quality and decoder complexity might be the main constraints.




 1.3 Co八'IPRESSION TAXONO八'Iv,;
 A typical classification of compression methods is shown in Figure 1.2.
6                                                                                    CHAPTER 1




           Image, Video, and Audio Compression Methods



    Model-Based                               Wave幻rrT卜Based

                                 Los引ess 4a                      기＞ Lossy
                        d스m小＞           뇨                        ＜스／     누＼     >
                Statistical           Universal         Spati키 Don冶仇          Frequency Domain
                                                        Time［兀m계n
                                        Arithmetic
                HGilbert                                나 Delta               日 Filter-Based
                                      - coding
                                                           Modu冶tion
                - Fano                - Len耳）e卜Ziv      - PCM                   - Subband
                                        (LZ) coding
                mHu卄man               -Pattern matching - DPCM                  - Way이et

                - Other               - Other            1比아아．
                                                                               - Other
                                                        1 Quantization

                                                        LOther
    HLinear-Predictive                                                        - Trans幻rn卜Based
     Coding (LPC)
                                                                                - Fourier
      AR, ARMA
    - modeling                                                                  - Karhunen-
                                                                                  Loeve (KL)
    HP이ynomial
                                                                                小 Hadamard
     Fitting
                                                                                - OCT
    中 다actals
                                                                                - Other
    -O히ec卜Based

    - Other


        Figure 1.2              A taxonomy of image, video, and audio compression
        methods.



1.3.1     Lossless versus Lossy Compression


Lossless compression

In many applications, the decoder has to reconstruct without any loss the
original data. For a lossless compression process, the reconstructed data and
the original data must be identical in value for each and every data sample.
This is also referred to as a reversible process. In lossless compression, for a
specific application, the choice of a compression method involves a tradeoff
                                                                                 7
Compression Fundamentals




                                                             is, coding efficiency,
along the three dimensions depicted in Figure 1.3; that
coding complexity, and coding delay.




                                                  Coding Delay
           Coding E仇旭ncy
         -Compression Ratio?

                          Code八力mplex勾r
                       - Memory requirements?
                       - Power requirements?
                       - Operations per second?


                Figure 1.3     Tradeoffs in lossless compression.



                                                                    e or上i뜨 per
 Coding Efficiency: This is usually measured in bits per sampl
                                                   d by the inform ation content
 second (bps). Coding efflciency is usually limite
                                                                      X provides
 or娠匠汾 of the source. In intuitive terms, the entropy of a source
                                                               n theory point of
 a measure for the "randomness " of X. From a compressio
                                                               ess (for example,
 view, sources with large entropy are more difficult to compr
 random noise is very hard to compress).

                                                         efficiency is sometimes
 In literature on lossless compression, the coding
                                                         cessor within the source
 characterized by the entropy at the output of a prepro
                                                           does not increase this
 coder; the implication here is that the source coder
                                                     ce, the source is composed
 entropy figure significantly. Note that, in practi
                                                             an analog source, the
  from a finite-alphabet; thus, the entropy is finite. For
                                                            n schemes, digitization
  entropy would be infinite, however, in most compressio
                                                         entation, which limits the
  of the analog source leads to a finite-alphabet repres
  source entropy.

                                                 ression process is analogous
 Coding Complexity: The complexity of a comp
                                                    the encoder and decoder
 to the computational effort needed to implement
                                                      red in terms of memory
 functions. The computational effort is usually measu
                                                        The operations count
 requirements and number of arithmetic operations.
                                                      per second and is often
 is characterized by the term millions ofoperations
                                                           arithmetic operation
 referred to as MOPS. Here, by operation, we imply a basic
  8
                                                                     CHAPTER 1




  that is supported by the computational engine. In the comp
                                                                 ression literature,
  the term MIPS (millions of instructions per second) is some
                                                                times used. This is
  specific to a computational engin& s architecture; thus, in this
                                                                    text we refer to
  coding complexity in terms of MOPS. In some applications,
                                                                   such as portable
  devices, coding complexity may be characterized by the powe
                                                                     r requirements
  of a hardware implementation.

  Coding Delay: A complex compression process often leads
                                                                   to increased
 coding delays at the encoder and the decoder. Coding delay
                                                            s can be alleviated
 by increasing the processing power of the computational engine;
                                                                      however,
  this may be impractical in environments where there is a powe
                                                                 r constraint or
  when the underlying computational engine cannot be improved.
                                                                  Furthermore,
 in many applications, coding delays have to be constrained; for
                                                                    example, in
 interactive communications. The need to constrain the
                                                           coding delay often
 forces the compression system designer to use a less sophi
                                                            sticated algorithm
 凡r the co呻ress幻n processes.

 From this discussion, it can be concluded that these
                                                             tradeoffs in coding
 complexity, delay, and efficiency are usually limited to a small
                                                                    set of choices
 along these axes. In a subsequent section, we will briefly descr
                                                                  ibe the tradeoffs
 within the context of specific lossless compression metho
                                                             ds.

Lossy compression

The majority of the applications in image or video data
                                                           processing do not
require that the reconstructed data and the original
                                                        data are identical in
value. Thus, some amount of loss is permitted in the recon
                                                             structed data. A
compression process that results in an imperfect reconstruct
                                                             ion is referred to
as a lossy compression process. This compression process is血끄＝
                                                                  ＼모rsible. In
practice, most irreversible compression processes degra
                                                        de rapidly the signal
quality when they are repeatedly applied on previously decom
                                                              pressed data.
The choice of a specific lossy compression method involv
                                                            es tradeoffs along
the four dimensions shown in Figure I .4. Due to the additi
                                                                onal degree of
freedom, namely, in the signal quality, a lossy compressio
                                                           n process can yield
higher compression ratios than a lossless compression schem
                                                              e.

Signal Qualily: This term is often used to characterize the signa
                                                                  l at the output
of the decoder. There is no universally accepted
                                                   measure for signal quality.
Compression Fundamentals                                                    9




                                    Sign削 Qua肝V
                               - Bit error probability?
                               - Signal/Noise?
                               - Mean 야出lion score?




                 Coding E所C厄ncy            I               C어出ng Delay
               - Compression Ratio?

                                    Coder Con冽ex什V
                               '- memo미 requirements?
                                - power (mW)?
                                - Operations per second?


                  Figure 1.4    Tradeoffs in lossy compression.



One measure that is often cited is th갸始n코苾O茵前如NR公which can
be expressed as
                               -     encoder input sional enerou         . . 八．
                   A iL - i 'Jbt1310            Si97l毗e72er吼
                                         72OiSe signal
                                         noise         energy／   "         fl

The noise signal energy is defined as the energy measured for a hypothetical
signal that is the difference between the encoder input signal and the decoder
output signal. Note that, SNR as defined here is given in decibels (dB). In the
case of images or video, PSNR (peak signal-to-noise ratio) is used instead
of SNR. The calculations are essentially the same as in the case of SNR,
however, in the nominator, instead of using the encoder input signal one uses a
hypothetical signal with a signal strength of 255 (the maximum decimal value
 of an unsigned 8-bit number, such as in a pixel).

 High SNR 0r PSNR values do not always correspond to signals with percep-
                                    quality is the［延也恥
므껜익旽h quality. .Anoth町 measure 야 如恤process                    摯
프인드wnere me penormance or a compression    is cnaractenzeu ny me
  10
                                                                          CHAPTER 1




  subjective quality of the decoded signal. For instance, a five
                                                                 point scale such as
  very ann아'ing, 如刃蜘g, si蜘ny 如吻ing, perce까洌e but not
                                                                     annoy呻，and
  imperceptible might be used to characterize the impairment
                                                                  s in the decoder
  output.

 In either lossless or lossy compression schemes, the
                                                         quality of the input
 data affects the compression ratio. For instance, acqui
                                                            sition noise, data
 sampling timing errors, and even the analog-to-digital conve
                                                                  rsion process
 affects the signal quality and reduces the spatial and tempo
                                                                ral correlation.
 Some compression schemes are quite sensitive to the loss in correl
                                                                       ation and
 may yield significantly worse compression in the presence of noise
                                                                     .
 Both lossless and lossy compression methods fit within
                                                           the general model
 depicted in Figure 1 .5. Most of the compression standards that
                                                                 are described

        Image, Video, and                    Lossless Coding
                        니   Preprocessor                       Entropy Coder
                 HH＝




        Audio Data
                                                                               F令
                                     Lossy Coding

                                 V
                            Additional
                            Processing


        Figure 1.5     Lossless and lossy compression coding framework.


in this book fit within this framework and employ both
                                                        lossy and lossless
compression schemes to achieve high coding efficiency.
                                                       These compression
methods will be described in detail in later chapters.



1.3.2    Variable Bit Rate versus Constant Bit Rate

From Figure 1 .3, the tradeoffs employed in the selection of
                                                               a lossless corn-
pression method can lead to several types of coder design
                                                           s. In one approach,
one can envision a coder where the coding delay is fixed. This
                                                                could lead to a
lossless coder where the coding efficiency fluctuates from
                                                            sample to sample,
but the output symbols are delivered at a constant rate. On the
                                                                   other hand,
if coding delay is not critical, one can process multiple samples
                                                                   at a time to
Compression Fundamentals                                                       11




obtain a higher coding efficiency. In this case, the encoder output datasize
is fixed, but output symbols are delivered at irregular time intervals. Thus,
depending on the application environment, one can obtain either fixed length
symbols at irregular time intervals or variable length symbols at constant time
intervals. Note that, using the generic coder structure shown in Figure 1.1, it is
possible to convert a variable length source-coder output bit stream to a fixed
length c方annel-coder output bit stream.

In the case of lossy compression, the tradeoffs shown in Figure 1.4 can lead
to several classes of coders. In one approach, the coding efficiency could be
constrained to a fixed value. For such coders, the signal quality would tend to
fluctuate. Such a coder might be required in a communication system where
the transmission rate cannot exceed a specified value. Another application
of such coders is in storage applications with fixed storage capacity. These
coders are referred to as constant bit rate coders. If the transmission or storage
requirements are not fixed and if the user desires specific quality at the output
 of the decoder, then the coding efficiency can be allowed to fluctuate. These
coding schemes are referred to as constant qualizy or variable bit rate coders.



1.3.3    Single- or Multiple-Sample-Based Compression

Within the compression taxonomy shown in Figure 1.2, one can classify the
coding schemes as single- or multiple-sampled-based approaches. Single-
sample-based compression schemes process one input sample at a time and
generate a compressed representation for each input sample. In the case of
image or video data, such schemes are referred to as pixel-based or pet-based
schemes. Multiple-sample-based schemes process several input samples at a
time and generate one or several compressed representations for the entire set
of input samples. For image or video data, such compression methods are
referred to as block-based schemes. The benefit of block-based compression
over pel-based compression is well founded in Shannon's coding theorem,
 where it is shown that if the the blocklength increases, then the coding
 efficiency can reach its theoretical limit. However, block-based schemes tend
 to have higher complexity than pel-based schemes.
 12                                                                CHAPTER 1




1.3.4     Comparison of Compression Domains

 Compression processes can exploit redundancies in the data across space, time,
 or frequency. Single-sample-based compression schemes are often spatial-
 domain or time-domain based; in this case, there are no inherent bit savings if
 frequency domain approaches are adopted. Block-based compression schemes
 fit into three main categories: spatial-domain-based, time-domain-based or
 frequency-domain-based. If a group of samples is highly correlated in
 the spatial domain, then it tends to also have a very compact frequency-
domain representation; thus, a frequency-domain-based compression process
is preferred for such datasets. For multidimensional data, such as video, that
have both spatial and temporal components, a hybrid spatial- and frequency-
domain approach is adopted. Such hybrid techniques are the basis of all the
image and video compression standards which will be discussed in subsequent
chapters of this text.




1.4 ISSUES IN COMPRESSION METHOD
    SELECTION
In this chapter, we have introduced some fundamental concepts related to
image, video, and audio compression. When choosing a specific compression
method, one should consider the following issues:


      Lossless or lossy.    This is usually dictated by the coding efficiency
      requirements.

      Coding efficiency. Even in a lossy compression process, the desirable
      coding efficiency might not be achievable. This is especially the case
      when there are specific constraints on output signal quality.

      Variability in coding efficiency. In some applications, large variations in
      coding efficiency among different data sets may not be acceptable.
        戶伊h卜m.
      Resilience to transmission errors. Some compression methods are more
      robust to transmission errors than others. If retransmissions are not
      permitted, then this requirement may impact on the overall encoder-
      decoder design.
                                                                                13
Compression Fundamentals




                                                                   tant to keep the
    Complexity tradeoffs. In most implementations, it is impor
                                                                     n applications
    overall encoder-decoder complexity low. However, certai
    may require only a low decoding complexity.
                                                                   ession methods
    Nature of degradations in decoder output. Lossy compr
                                                                 artifacts depends
    introduce artifacts in the decoded signal. The nature of
                                                                 degre   e to which
    on the compression method that is employed. The
                                                                      application to
    these artifacts are judged objectionable also varies from
                                                             an  interp  lay between
    application. In communication systems,there is often
                                                                uced by the coder.
    the transmission errors and the coding artifacts introd
                                                                       m design.
     Thus, it is important to consider all types of error in a syste
                                                                   need to support
     Data representation. In many applications, there is a
                                                           is performed to derive
     two decoding phases. In the first phase, decoding
                                                              ing. In the second
     an intelligible signal; this is the case in data brows
                                                                     y signal. One
     phase, decoding is performed to derive a higher qualit
                                                                            require a
     can generalize this notion to suggest that some applications
                                                                      n context, we
     hierarchical representation of the data. In the compressio
                                                                     n methods. The
     refer to such compression schemes as scalable compressio
                                                                       standards that
     notion of scalability has been adopted in the compression
     are described later in the text.
                                                                        applications,
     Multiple usage of the encoding-decoding tandem. In many
                                                      rm  multip  le encod  e-decode
     such as video editing, there is a need to perfo
                                                                            ion. This
     operations using results from a previous encode-decode operat
                                                                             schemes,
      is not an issue for lossless compression; however, for lossy
      resilience to multiple encoding-decoding cycles is essential.
                                                                    In a system
     Interplay with other data modalities, such as audio and video.
                                                                  compr  ession
     where several data modalities have to be supported, the
                                                                elements. For
     methods for each modality should have some common
     instance, in an interactive videophone system, the     audio compression
                                                                       the video
     method should have a frame structure that is consistent with
                                                                     rements on
     frame structure. Otherwise, there will be unnecessary requi
                                                                     .
     buffers at the decoder and a reduced tolerance to timing errors
                                                             onment,there will
     Interworking with other systems. In a mass-market envir
     be multiple data modalities and multiple compressio n syste ms. In such an
                                                                  another may
     environment, transcoding from one compression method to
                                                                      frame by
     be needed. For instance, video editing might be done on a
                                                                     t temporal
     frame basis; hence, a compression method that does not exploi
  14
                                                                   CHAPTER 1




       redundancies might be used here. After video editin
                                                             g, there might be a
       need to broadcast this video. In this case, temporal redun
                                                                  dancies can be
       exploited to achieve a higher coding efficiency. In such
                                                                 a scenario, it is
       important to select compression methods that support
                                                               transcoding from
       one compressed stream format to another. Interworki
                                                              ng is important in
       many communications environments as well.




1.5 TO PROBE FURTHER
In this chapter, we have briefly reviewed some of the basic
                                                            concepts associated
 with the compression of image, video, and audio signal
                                                          s. Additional details,
including descriptions of specific compression methods,
                                                         can be found in Jayant
[92]. Some specific applications that are based on the conce
                                                               pts described in
this chapter can be found in Chapter 2 of(1461. These
                                                         basic concepts will be
refined in subsequent chapters as we describe specific
                                                         compression methods
for image, video, and audio.
                                                                     2
八4ETHODS AND STANDAI之DS FOI之
     LOSSLESS COMPRESSION




2.1 INTRODUCTION
Lossless compression refers to compression methods for which the original
uncompressed data set can be recovered exactly from the compressed stream.
The need for lossless compression arises from the fact that many applications,
such as the compression of digitized medical data, require that no loss be
introduced from the compression method. Bitonal image transmission via
a facsimile device also imposes such requirements. In recent years, several
compression standards have been developed for the lossless compression of
such images. We discuss these standards later in this chapter. In general,
even when lossy compression is allowed, the overall compression scheme
may be a combination of a lossy compression process followed by a lossless
compression process as depicted in Figure 1.5. Various image, video, and
audio compression standards follow this model, and several of the lossless
compression schemes used in these standards are described in this chapter.




2.2 PRELIMINARIES
The general model of a lossless compression scheme is as depicted in Figure
2.1. Given an input set of symbols, a modeler generates an estimate of the
probability distribution of the input symbols. This probability model is then
used to map symbols into codewords. The combination of the modeling and
the symbol-to-codeword mapping functions is usually referred to as entropy
  16
                                                                      CHAPTER 2




             Input Symb이




                                                   Symb이－      Codeword
                           D이ay                      To-
                                                                 (>
                                                  Codeword
                            1
                            1
                                                  Mapping
                            f                         A
                            1
                                  Probability
                                    Model


             Figure 2.1     A generic model for lossless compression.



 coding. The key idea of entropy coding is to use short codew
                                                              ords for symbols
 that occur with high probability and long codewords for
                                                           symbols that occur
 with low probability.

  The probability model can be derived either from the input data
                                                                    or from a priori
  assumptions about the data. Note that, for decodability, the
                                                                 same model must
 also be generated by the decoder. Thus, if the model is dynam
                                                                   ically estimated
 from the input data, causality constraints require a delay functi
                                                                   on between the
 input and the modeler. If the model is derived from a priori
                                                                assumptions, then
 the delay block is not required; furthermore, the model functi
                                                                 on need not have
access to the input symbols. The probability model does
                                                             not have to be very
accurate, but the more accurate it is, the better the comp
                                                           ression will be. Note
that, compression is not always guaranteed. If the proba
                                                           bility model is wildly
inaccurate, then the output size may even expand. Howe
                                                              ver, even then the
original input can be recovered without an\' loss.

Decompression is performed by reversing the flow of opera
                                                          tions shown in
Figure 2.1. This decompression process is usually
                                                  referred to as entropy
decoding.
Methods and Standardsfor Lossless Compression                                17




2.2.1   Message-to-Symbol Partitioning

As noted before, entropy coding is performed on a symbol by symbol basis.
Appropriate partitioning of the input messages into symbols is very important
for efficient coding. For example, typical images have sizes from 256 x 256
pixels to 64,000 x 64,000 pixels. One could view one instance of, say, the
256 x 256 image as a single message,64,000 units long; however, it is very
difficult to provide probability models for such long symbols. In practice, we
typically view any image as a string of symbols. In the case of a 256 x 256
image, if we assume that each pixel takes values between zero and 255, then
this image can be viewed as a sequence of symbols drawn from the alphabet 0,
1, 2,.., 255. The modeling problem now reduces to finding a good probability
model for the 256 symbols in this alphabet.

For some images, one might partition the data set even further. For instance,
if we have an image with 12 bits per pixel, then this image can be viewed as a
sequence of symbols drawn from the alphabet 0, 1,..., 4,095. Hardware and/or
software implementations of the lossless compression methods may require
that data be processed in 8-, 16-,32-,or 64-bit units. Thus,one approach might
be to take the stream of 12-bit pixels and artificially view it as a sequence of
8-bit symbols. In this case, we have reduced the alphabet size. This reduction
compromises the achievable compression ratio; however,the data are matched
to the processing capabilities of the computing element.

Other data partitions are also possible; for instance, one may view the data as
a stream of 24-bit symbols. This approach may result in higher compression
since we are combining two pixels into one symbol. In general, the partitioning
of the data into blocks, where a block is composed of several input units, may
result in higher compression ratios, but also increases the coding complexity.



2.2.2 Differential Coding

Another preprocessing technique that improves the compression ratio is
differential coding. Differential coding skews the symbol statistics so that the
resulting distribution is more amenable to compression. Image data tend to
have strong interpixel correlation. If, say, the pixels in the image are in the
order x1,x2,x3,...,XN, then instead of compressing these pixels, one might
process the sequence of differentials y. = 2i - xi_1, where i = 1, 2, ..., N,
18                                                               CHAPTER 2




and x0 = 0. In compression terminology, yj is referred to as the prediction
residual of x:. The notion of compressing the prediction residual instead of
xi is used in all the image and video compression standards. For images, a
typical probability distribution for x, and the resulting distribution for yi are
shown in Figure 2.2.




                           -C> Preprocessing   -=>




       0                        255         -255        0          255

                x. value                              y1 value


      Figure. 2.2 . Typical distribution of pixel values for xi and yi.
      Here, the pixel values. are shown on the. horizontal axis and .tile
      corresponding probability ot occurrence is shown on the vertical
      axis.



Let symbol s, have a probability of occurrence p1. From coding theory,
the ideal symbol-to-codeword mapping function will produce a codeword
requiring log2 去 bits. A uniform distribution for pi (pi 二已 赤), such as the
one shown in the left plot of Figure 2.2, will result in codewords that on the
average require eight bits; thus, no compression is achieved. On the other
hand, for a skewed probability distribution, such as the one shown in the right
plot of Figure 2.2, the mapping function can on the average yield codewords
requiring less than eight bits per symbol and thereby achieve compression.




2.3 HUFFMAN ENCODING
In 1952, D. A. Huffman developed a code construction method that can be
used to perform lossless compression. In Huffman coding, the modeling
and the symbol-to-codeword mapping functions of Figure 2.1 are combined
Methods口nd Standards for I刀ssless Corn까es勍／2                                     19




into a single process. As discussed earlier, the input data are partitioned
into a sequence of symbols so as to facilitate the modeling process. In most
image and video compression applications, the size of the alphabet composing
these symbols is restricted to at most 64,000 symbols. The Huffman code
construction procedure evolves along the following steps:


  1. Order the symbols according to their probabilities.
     For Huffman code construction, the frequency of occurrence of each
     symbol must be known a priori. In practice, the frequency of occurrence
     can be estimated from a training set of data that is representative of the data
     to be compressed in a lossless manner. If, say, the alphabet is composed
     of N distinct symbols s1, s2, ..., SN and the probabilities of occurrence are
     Pi,P2, ...,PN, then the symbols are rearranged so that p 2 p2 2 p3... 2 PN.

  2. Apply a contraction process to the two symbols with the smallest proba-
     bilities.
     Suppose the two symbols are SN_i and SN. We replace these two
     symbols by a hypothetical symbol, say, HN_1, that has a probability of
     occurrence PN-1 + PN. Thus, the new set of symbols has N - 1 members:
     Si } S2, ...,SN卞2, 且N- i .

  3. We repeat the previous step until the final set has only one member.


The recursive procedure in Step 2 can be viewed as the construction of a
binary tree, since at each step we are merging two symbols. At the end of the
recursion process, all the symbols s1, S2, .., SN will be leaf nodes of this tree.
The codeword for each symbol si is obtained by traversing the binary tree
from its root to the leaf node corresponding to si.

 We illustrate the code construction process with the following example
 depicted in Figure 2.3. The input data to be compressed is composed of
 symbols in the alphabet k, 1, u, w, e, r, ?. In Step 1, we sort the probabilities. In
 Step 2, we merge the two symbols k and w to form the new symbol (Ic w). The
 probability of occurrence for the new symbol is the sum of the probabilities of
 occurrence for k and w. We sort the probabilities again and pe而rm the merger
 on the pair of least frequently occurring symbols, as shown in the boxed region
 in Step 3 of Figure 2.3. We repeat this process through Step 6. By traversing
 this process from right to left and visualizing this as a binary tree as shown in
20                                                                                                                        CHAPTER 2




                                                                                             W               k
                                                                                                             1 05
  Symb이 Probability Codeword                                                                                                  step 1
                                                                                0.051                            0.
      k                0.05           10101
                                                                                          (0) {k,                (1) ?
                                                                                                        W}
                                                       step 4                                                                 step 2
                                                                                                        w}
      1                0.2               01
                                                                               .. .．』回列 이
                       0.1              100                                    11                       {{k,w},?}

                       0.05           10100
                                                                                1
                                                                                    (0)                 (1)      1            針ep 3

                                                                           0.1 {{{k,w},?},u}0·2
                       0.3               11            (0) (1)                                1
                                                                                                  (0)                 step5   (14
                                                 0.2    {l,r}        0.2                   0.3 {{{{k,w},?},u},e} 0.3
                       0.2               00

                       0.1             1011              I   (0)             5怡p6                                     삐
          1Merge        Symbols                         ""                     十G.肥rate誌品rds
        Step 1 Step 2                   Step 3         Step 4              Step 5                            Step 6
  k i／怡 e 0.3 e 0.3                     e 0.3          e 0.3               {l,r} 0.4                         ((((k,w),?),u],e)
                                                                                                                   0.6
  I   0.2           I 0.2     I 0.2     I 0.2          {{{k,w),?},u} e 0.3                                   (l,r} 0.4
                                                          0.3
  u 0.1             1 0.2 r 0.2         r 0.2          / 0.2         {{(k，叫까시｝
                                                                          0.3
  w 1/16 U 0.1                U 0.1     ((k, w),?)     r 0.2
                                           0.2
  e 0.3              ? 0.1    ? 0.1     u 0.1

  r   0.2           k 1/16 化빠 ]/8

  ? 0.1              w 1/16


                   Figure 2.3         An example of Huffman codeword construction.



this figure, one can determine the codewords for each symbol. For example,
to reach the symbol u from the root of the tree, one traverses nodes that were
assigned the bits 1, 0, and 0. Thus, the codeword for u is 100.

In this example, the average codeword length is 2.6 bits per symbol. In
general, the average codeword length is defined as

                                                     avg =         >1 iPi                                                              (2.1)
Methods and Standards for Lossless Compression                                 21




where 1, is the codeword length (in bits) for the codeword corresponding to
symbol si. The average codeword length is a measure of the compression
ratio. Since our alphabet has seven symbols, a fixed-length coder would
require at least three bits per codeword. In this example, we have reduced
the representation from three bits per symbol to 2.6 bits per symbol; thus, the
corresponding compression ratio can be stated as 赤 = 1.15. For the lossless
compression of typical image or video data, compression ratios in excess of
two are hard to come by.



2.3.1   Properties of Huffman Codes

According to Shannon, the entropy of a source S is defined as

                           且   （S)   =   ti=   ＞二
                                                「
                                                    ‘1099{
                                                                             (2.2)


where, as before, p, denotes the probability that symbol s2 from S will occur.
From information theory, if the symbols are distinct, then the average number
of bits needed to encode them is always bounded by their entropy. For example,
for the alphabet used in the previous section, the average length is bounded
by 2.546439 bits per symbol. It can be shown that Huffman codewords satisfy
the constraints tj <1 9 <r + 1; that is, the average length is very close to the
optimum. A tighter bound is ij <lavg <p + 0.086, where p is the probability
of the most frequently occurring symbol. The equality is achieved when all
symbol probabilities are inverse powers of two. Thus, the loss in performance
can be viewed as a result of the quantization effect on the symbol probabilities.

The Huffman code table construction process, as was described here, is
referred to as a bottom-up method, since we perform the contraction process
on the two least frequently occurring symbols. In recent years, top-down
construction methods have also been published in the literature.

The code construction process has a complexity of O(N勿92 N). With
presorting of the input symbol probabilities, code construction methods with
complexity O(N) are presently known.

In the example, one can observe that no codeword is a prefix for another
codeword. Such a code is referred to as a prefix-condition code. Huffman
codes satisfy always the prefix-condition. If codelengths I. satisfy the constraint
22                                                                 CHAPTER 2




> 2' <1, then it can be shown that the resulting codewords satisfy the prefix-
condition. Furthermore, the corresponding codewords can be const끄cted as
the first 1, bits in the fractional representation of a1,
                                 i- i
                              ＞二2/,,i = l,2, ···，N·                          (2.3)
                           m=
                                 j= 1


Due to the prefix-condition property, Huffman codes are uniquely decodable.
Not every uniquely decodable code satisfies the prefix-condition. A code such
as 0, 01, 011, 0111 does not satisfy the prefix-condition, since zero is a prefix
for all of the codewords; however, every codeword is uniquely decodable,
since a zero signifies the start of a new codeword.

If we have a binary representation for the codewords, the complement of
this representation is also a valid set of Huffman codewords. The choice of
using the codeword set or the corresponding complement set depends on the
application. For instance, if the Huffman codewords are to be transmitted over
a noisy channel where the probability of error of a one being received as a
zero is higher than the probability of error of a zero being received as a one,
then one would choose the codeword set for which the bit zero has a higher
probability of occurrence. This will improve the performance of the Huffman
coder in this noisy channel.

In Huffman coding, fixed-length input symbols are mapped into variable-length
codewords. Since there are no fixed-size boundaries between codewords, if
some of the bits in the compressed stream are received incorrectly or if they
are not received at all due to dropouts, all the data are lost. This potential loss
can be prevented by using special markers within the compressed bit stream
to designate the start or end of a compressed stream packet.




2.4 HUFFMAN DECODING
The Huffman encoding process is relatively straightforward. The symbol-
to-codeword mapping table provided by the modeler is used to generate the
codewords for each input symbol. On the other hand, the Huffman decoding
process is somewhat more complex.
Methods and Standards for Lossless Compression                                23




2.4.1     Bit-Serial Decoding

For the example shown in Figure 2.3, let us assume that the binary coding tree
is also available to the decoder. In practice, this tree can be reconstructed from
the symbol-to-codeword mapping table that is known to both the encoder and
the decoder. The decoding process consists of the following steps:


  1. Read the input compressed stream bit by bit and traverse the tree until a
     leaf node is reached.

  2. As each bit in the input stream is used, it is discarded. When the leaf node
     is reached, the Huffman decoder outputs the symbol at the leaf node. This
     completes the dec以ing for this symbol.


We repeat these steps until all of the input is consumed. For the example
discussed in the previous section, since the longest codeword is five bits and
the shortest codeword is two bits, the decoding bit rate is not the same for all
symbols. Hence, this scheme has a fixed input bit rate but a variable output
symbol rate.



2.4.2      Lookup-Table-Based Decoding

Lookup-table-based methods yield a constant decoding symbol rate. The
lookup table is constructed at the decoder from the symbol-to-codeword
mapping table. If the longest codeword in this table is L bits, then a 2- entry
lookup table is needed. In our example, L = 5. Specifically, the lookup table
construction for each symbol si is as follows:


     Let c2 be the codeword that corresponds to symbol s,. Assume that ci has
     Ii bits. We form an L-bit address in which the first Ii bits are ci and the
     remaining L - Ii bits take on all possible combinations of zero and one.
     Thus, for the symbol s1, there will be 2'- H1i addresses.

        At each entry we form the two-tuple (si, li).


 Decoding using the lookup table approach is relatively easy:
24                                                              CHAPTER 2




  I. From the compressed input bit stream, we read in L bits into a buffer.

 2. We use the L-bit word in the buffer as an address into the lookup table
    and obtain the corresponding symbol, say Sk. Let the codeword length be
    ik. We have now decoded one symbol.

 3. We discard the first Ik bits from the buffer and we append to the buffer,
    the next Ik bits from the input, so that the buffer has again L bits.

 4. We repeat Steps 2 and 3 until all of the symbols have been decoded.


The primary advantages of lookup-table-based decoding are that it is fast
and that the decoding rate is constant for all symbols, regardless of the
corresponding codeword length. However, the input bit rate is now variable.
For image or video data, the longest codeword could be around 16 to 20 bits.
Thus, in some applications, the lookup table approach rnny be impractical due
to space constraints.

Variants on the basic theme of lookup-table-based decoding include using
hierarchical lookup tables and combinations of lookup table and bit-by-bit
decoding. In the next section, we describe codeword construction methods
that facilitate lookup-table-based decoding by constraining the maximum
codeword length to a fixed-size L.




2.5 HUFFMAN CODES WITH CONSTRAINED
    LENGTH
In the previous section, we described several decoding procedures for Huffman
decoding. For fast decoding, lookup-table-based approaches are preferable.
In many applications, depending on the symbol probabilities, the Huffman
codebook design may yield codewords that may require a large number of bits.
This outcome is possible when some of the symbol probabilities are extremely
small. Thus, lookup-table-based decoding may not be feasible if the memory
requirements are prohibitive. To alleviate this problem, a shortened Huffman
code can be used.

The basic idea of the shortened Huffman code is to view the Huffman code
representation as a hierarchical representation. Suppose, due to lookup table
Methods and Standards for Lossless Compression                                           25




size constraints, we require that no codeword length exceed L bits. Let S be
the set of N symbols Si, Si, ..., SN for which a Huffman code is to be designed.
Let p, be the occurrence frequency for symbol s. We further assume that the
symbols are ordered so that Pi 2 P2 2 p3 · · · 2 PN. The design procedure for a
shortened Huffman code is as follows:


 I. Partition S into two sets S1 and S2 as


                                  S1
                                       =
                                           sjp
                                                     >        유，
                                                                                       (2.
                                                                                         4)
                                       品                               五               (2.5)
                                           키p즈二.                       =




  2. Create a special symbol Q such that its frequency of occurrence is

                                       q=        Z
                                                 iES:?
                                                         刃：
                                                                   ·
                                                                                       (2.6)



  3. Augment S1 by Q to form a new set W. The new set has the occurrence
     frequencies corresponding to symbols in S1 and the special symbol Q. We
     then construct an optimal prefix code for TV using the design procedure
     for unconstrained-length Huffman codewords, as explained in a previous
     section. This design procedure will yield codewords cn for symbols in the
     set S1 and a codeword Cq for the symbol Q. Cq is the shortened prefix-code
     for symbols in S2.
     If Ii is the length of the i-th codeword of S1. then

                                                                       11092 P21 드 L   (2.7)
                        rnaxS,EsllZ = lflQ工S,ESI
     Thus, all symbols in Si yield codewords that are at most L bits. Codeword
     Cq will also not exceed L bits. (j.니 denotes the smallest integer larger or
     equal to x.)


 Huffman encoding of a message string lnim2rn3...mk is relatively straightfor-
 ward.


     For all rn, E S, output the corresponding codeword from c,i.
26                                                                      CHAPTER 2




      For all m, E S2, output the codeword Cq followed by an L-bit fixed-length
      binary representation for in1. (Actually, one can use fewer than L bits,
      since if there are N52 symbols in S2 and N52 < N, then the fixed-length
      binary representation for each m1 is [幻g2 N52] bits).


When the symbol occurrence frequencies are known a priori, one can estimate
the worst-case performance degradation for the shortened Huffman codes as
compared with the unconstrained Huffman code table design.

Let Ish be the average codeword length for the shortened codeword design
approach. Let iw be the average codelengths for 1V, and let H(W) be the
entr야）yf아 [V. 砥／e have
                            la,, = Lw + qL.                        (2.8)
                            H(IV) < ls/t < H(W) + 1.                          (2.9)
Furthermore, la,, is bounded by

                         H (S) < ish 5 H(IV) + qL + 1,                       (2.10)

where H (S) denotes the entropy of S. However,


                       月叫工，『如加切12 q'
                                   1 之 1그 l




               吐 = > M = >2 川og2 근i 5 二刃d09:
                                         log2 1-,n.
                     iES2         i ES2       -             i ES2   "

and

                     尸（S)= 三，P 1092亡工，加2去·
                              1亡 口 l              i t二 D2



Hence,
                       H(S)
                       J7(S) 5/ ,
                              ish , 5/
                                    <H(S)
                                       /(S) +l+
                                             1 + q幻9
                                                 ql。
                                                   g2,1-.
                                                       q
For an optimal unconstrained Huffman code, the average codelength is
bounded by H(S) 드 lnU9 드 H(S) + 1. Hence, the worst-case increase in the
average codeword length for the shortened code is q勿g2 言 bits per symbol
(this function attains a maximum value of 4).

Huffman decoding for shortened prefix codes using a lookup-table-based
approach is similar to the procedure described in the previous section. In
Methods and Standards for Lossless Compression                               27




this case, a two-level decoding is done when the codeword Cq is decoded.
After Cq is decoded, the next L bits are read from the input bit stream, and the
corresponding syn小아 m1 is then con叩uted. W레lustrate the c아le construc如n
process with an example.

Example 1: Let S = so, si, ...,s15. The occurrence frequencies and the
resulting unconstrained Huffman code are as shown in Table 2.1. Here, the
Huffman code table design is based on the approach desc餉ed in the previous
section. The average codeword length is lavg = E｝으O lip1 = 2.694 bits per


                   Symbol si       I가       ii
                                                 Codeword
                      0         0.28200     2    11
                       1        0.27860     2    10
                      2         0.14190     3    011
                      3         0.13890     3    010
                      4         0.05140     4    0011
                      5         0.05130     4    0010
                      6         0.01530     5    00011
                      7         0.01530     5    00010
                      8         0.00720     6    000011
                      9         0.00680     6    000010
                      10        0.00380     7    0000011
                      11        0.00320     7    0000010
                      12        0.00190     7    0000001
                      13        0.00130     8    00000001
                      14        0.00070     9    000000001
                      15        0.00040     9    000000000

           Table 2.1    Unconstrained length Huffman codewords.


symbol. Note that, the longest codeword is nine bits. Thus, a 512-entry table is
needed for lookup-table-based decoding. Let us suppose that only a 128-entry
lookup table can be permitted. Thus, we need to design a seven-bit shortened
Huffman code, that is, all codeword lengths must be less than or equal to seven
bits.

The code table design procedure is as follows:
28                                                                                         CHAPTER 2




  1. We form the two sets S1 and S2. Symbols s8 to s15 belong to S2, since
     7가 < th for i = 8 to 15. The occurrence frequency of the special symbol
     Qis>I｝으81가 = 0.0253.
  2. The codeword design process for the shortened Huffman codes is il-
     lustrated in Figure 2.4. The corresponding Huffman code table for the


  11           01           101          100       0011      0010     00011       00010        0000

     수 ' .     수    ' 1
                            中 수 수 ' 2       ' 3       ' 4     수 수
                                                                ' 5         ' 6     수    ' 7     수Q
0.2820       0.2786       0.1419        0.1389    0.0514    0.0513    0.0153      0.0153       0.0253

                                                                        1            0

                                                                                                      0




                            Figure 2.4            Shor妃ned Hu伽姐n code.


     shortened Huffman codes is shown in Table 2.2. Note that, for all symbols
     in S2 we need a prefix code of four bits followed by a seven-bit represen-
     tation for the specific symbol in S2. The average codeword length is now
     Ish = Z 70iiPi + 二뜬8 llj가 = 2.8057 bits per symb이．


During encoding, if the input symbol is in set S1, then the encoder outputs
the corresponding Huffman codeword. If the input symbol is in set S2, then
the encoder outputs a codeword with the prefix 0000 followed by a codeword
which is the seven bit representation of the symbol in the set S2. For instance,
if, say, symbol s9 is to be encoded, then the Huffman code for this symbol
will be made up of two codewords 0000 and 0001001. Note that, the longest
codeword does not exceed the specified length of seven bits.
兀lerhods and St口nd口rds for I刀ssless Co刃tpression                              29




           Symbol i        I갸       1,
                                         Codeword      Additional
              0         0.28200     2    11
              I         0.27860     2    01
              2         0.14190     3    101
              3         0.13890     3    100
              4         0.05140     4    0011
              5         0.05 130    4    0010
              6         0.01530     5    00011
              7         0.01530     5    00010
              8         0.00720     11   0000          0001000
              9         0.00680     11   0000          0001001
             10         0.00380     11   0000          0001010
             11         0.00320     11   0000          0001011
             12         0.00190     11   0000          0001100
             13         0.00130     11   0000          0001101
             14         0.00070     11   0000          0001110
             15         0.00040     11   0000          0001111

     Table 2.2    Constrained-length (L = 7 bits) Huffman codewords.



Decoding is performed as follows:


 1. We first construct a lookup table as explained in the previous section.
    Huffman decoding for each output symbol is as follows:

 2. From the input bit stream, we fetch bits into a buffer until the buffer has
    seven bits. We access the lookup table location, using the seven bits as an
    address. This lookup table location contains the symbol for the Huffman
    code and the codelengths for the Huffman code. Let mk be the symbol
    and Ik the codelengths.

 3. The first Ik bits in the buffer are discarded by shifting the buffer contents
    to the left by Ik bit positions.

         If mk is not the special symbol Q, mk is one of the symbols
         SO, Si, ..., s7, and thus we have correctly decoded this symbol.
         If mk is the special symbol Q, additional bits from the input bit
         stream are needed for decoding. We fetch ik bits from the input
30                                                              CHAPTER 2




         bit stream to fill up the buffer. The buffer now contains the binary
         representation for one of the symbols s8. s9. ....S15, and thus we have
         correctly decoded a symbol from 52.
          We repeat Steps 2 and 3 until the complete message has been
          decoded.


As illustrated by this example, a shortened prefix code can be decoded with
modest lookup table requirements, and decoding is quite efficient. However,
the average codelengths are worse, comparedto the unconstrained Huffman
code table design. Table 2.3 shows the maximum limits for the additional bits
per symbol for a shortened Huffman code versus an unconstrained Huffman
code. The data in this table are computed for the example cited in this section
and use the bounds derived in this section.


     Lookup Table Size (entries)     Worst case／訊 小 /a四 (b札slsyn小에
                16                               0.42 13
                32                               0.2326
               64                                0.2326
               128                               0,1342
               256                               0.0731
               512                               0.0338

      Table 2.3 Average codeword length 乙h degradations compared
      to an unconstrainea i-iurrman cocie ror various vaiues or L. L ocie
      table size is 2L entries.



The key disadvantage of two-level decoding is that we cannot guarantee a
constant symbol rate at the Huffman decoder output. This may be a requirement
for many applications. In the next section, we describe other approaches to
constrained-length Huffman codeword design. These approaches avoid the
two-level decoding that is needed for the approach developed in this section.
Furthermore, the approaches described in the next section are capable of
yielding an average codeword length which is close to the optimum.
                                                                           31
Methods and Standards for Lossless Compression




2.6 CONSTRAINED-LENGTH HUFFMAN CODES -
    AD-HOC DESIGN
                                                     table design in which the
In the previous section, we developed a Huffman code
                                                          The design entailed
codeword lengths were constrained to be at most L bits.
                                                          on for infrequently
using a prefix code followed by an L-bit representati
                                                        c desig n methodology
occurring message symbols. Here, we develop an ad-ho
                                                           advantage that with
 that does not use a prefix code. This meth어ology has the
                                                        will be constant.
 a lookup-table-based decoder, the output decoding rate

 The codebook design process is as follows:
                                                  s2, ..., SN. We denote this
 Let the N members of the symbol alphabet be s1,
                                                          ed are composed of
 as the set S. Messages that are to be Huffman encod
                                                     ncies (probabilities) for
 symbols in S. We assume that the occurrence freque
                                                       occurrence probability
 each symbol in S is known; the i-th symb丑 s, has the
 denoted as p.

                                                            threshold T = 2 L
     Foram瞰imum code꿔ord len맘加f L bi奴 吼 define a

      Sort si,i = 1, 2, ...,N so thatpk 2 Pk4-1.

      For each pi, if p, 5 T, setp2 = T.
                                                           the uncons缸ained-
      Design the codebook using the modified pi values and
      length Huffman code table design approach.

                                                            will exceed L bits.
 Since p. is restricted to at most 2色 no codeword length
                                                                will be at least
 However, this ad-hoc design does not guarantee that there
                                                                 may be overly
 one codeword that has L bits. Hence, this design approach
                                                   that result fro m this ad-hoc
 aggressive. In Table 2.4, we show the codewords
                                                             d Reordered.) The
 design method. (Ignore for the time being the column labele
                                                             us section.
 symbol frequencies are the same as those used in the previo
                                                        n of this table, have a
  The resulting codewords, shown in the fourth colum
                                                                  ord length lavg
  maximum codeword length of seven bits and an average codew
                                                              gth Huffm  an code
  of 2.7308 bits per symbol. Note that, the unconstrained-len
                                                            bits and would yield
  table would have required a maximum code length of nine
                                                                ted, constraining
  an average code length of 2.6904 bits per symbol. As expec
 32                                                                        CHAPTER 2




                                                                 Reordered
           Symbol i          I入        I    Codeword         1     Codeword
              0           0.28200     2     11               2     11
              l           0.27860     2    01               2     01
              2           0.14190     3     101             3      101
              3           0.13890     3    100              3     100
              4           0.05 140    4    0010             4     0010
              5           0.05 130    4    0001             4     0001
              6           0.01530     6    001100           6     001100
              7           0.01530     6    001101           6     001101
              8           0.00720     7    0011110          6     000010
              9           0.00680     7    0011111          6     000011
             10           0.00380     7    0011100          6     000000
             11           0.00320     7    0011101          6     000001
             12           0.00190     6    000010           7     0011110
             13           0.00130     6    000011           7     0011111
             14           0.00070     6    000000           7     0011100
             15           0.00040     6    000001           7     0011101
             lavg
                      I              1 11 2.7308       i1        12.7141

      Table 2.4 Constrained-length (L = 7 bits) Huffman codewords -
      Ad-hoc design.



the codeword lengths results in a slightly worse average code length. Also
observe that symbols s8 to s11 have codewords with more bits than symbols
s12 to s15, even though they have a higher probability of occurrence. This is
due to the fact that some of the probabilities were set to the threshold T and
hence the ordering among the probabilities is obscured.

Intuitively, we expect symbols with a low probability of occurrence to require
longer codewords. Thus, in our ad-hoc design approach, we can apply this
notion to rearrange the final codewords. Rearranging is done by simply sorting
the codeword lengths in ascending order of magnitude and associating this
sorted list to the corresponding list of codewords. The use of post sorting on
the symbol lengths yields the codeword lengths shown in the fifth column.
The average codeword length has now been reduced to 2.7141 bits per symbol.
This ad-hoc design has a lower average codeword length than the prefix-code
Methods and Standards for Lossless Compression                                  33




design approach developed in the previous section. The average codeword
length can be lowered further using a method that we describe in the next
section.




2.7 CONSTRAINED-LENGTH HUFFMAN CODES -
    THE VOORHIS METHOD
This method yields codewords with an average length that is close to the
optimum, subject to the constraint that no codeword exceed L bits. The design
process is in three steps.


  I. If the message is composed of symbols drawn from a set of symbols
     Si, S2, ..., SN and if the symbol occurrence frequencies 釘e known a priori,
     sort the symbols so that 끄' 之 P2... 2 PN.

  2. Determine codeword lengths 11,12, ..., /N that minimize >I쑈l 12p1 subject
     to the constraint 1 <Ii <L.
     For uniquely decodable codes, we also require that >2各 2_li 드 1. The
     resulting codeword lengths will be such that 1 5 1l 5 12... 5 IN 드 L.

  3. Thei寸h codeword is the f耐I. bits of the fraction con叩uted by ＞二답 才h.


The major difficulty in this process is in the second step, namely, in the
calculation of the codeword lengths. The algorithm due to Voorhis proposes a
recursive solution. The recursion assumes that codeword lengths 11,12, ..,i,--l
have been found so far. Hence, the binary representation for the corresponding
codewords, denoted as c1, c2, ..., c,._1, is known. Define
                             k    = lr_i,                                    (2.15)
                                             r 小I

                              S   =   少d H Z 少'）·                            (2.16)
                                             i= 1


 Then s k-bit prefixes are available for the codewords Cr, ..., cN. This is referred
 to as the [k,r,s] problem, and the goal is to find an optimal way to partition
 s k-bit prefixes of codespace among the codewords Cr, ..., eN, subject to the
 condition I. E [k, L]Vi E [r, NJ. The computational steps for determining the
 codelengths 11,12, ..., IN by solving the [k,r,s] problem are as follows.
      34                                                                                    CHAPTER 2




 1.        forkE[1. L]
               for r E [i, 112i71(\ T - l. 2h:
                    for s e [N 이 ' + 1. nun (2.V - 2r. 2k - r + 1)]
                            砂k.r,s = ＞二.
                                      ，느小1-':
2.
           fork= L 中1. ...,1
               for r = min(N - 1. 9k) . . . ..1
                    for s = inin(N - r. 2「' - r + 1). ....f (N 口 ' + l) 2k山
                            ifs ＜二 I.（入' - n2"
                                             「e/" ] + 1
                                       寸，k.r.s =         L 'i- m. i . r,2s

                            이se
                                       的k,r,s = FlU 11(六Pr + 1 'k.r+1,s-1, 砂k+1,r,25)

3.         k= 1. i'= 1. s= 2

4,         jfk 二二／』or N - r + 1 드 s go to step 8

5.
           if (N 口 ')2_ L > (s - i) 2+k go to step 7

6.
           if kp1 + 砂k,r+1,s-1 < I'k+i.r.2s go to step 8

7.         k = k + 1, s = 2s, go to step 4

8.
           1r = 凡 7' 二＝ 1' + 1. S = S 中 1

9,
           if7' 드Ngotostep4


      At this point, we have computed the codelengths 11. 12, ..., 'N. These codelengths
      minimize ＞二；느 11p, and satisfy the constraint 1 5 11 드 /2... 5 IN 5 L. The
      codewords corresponding to these code lengths can be computed as

                                  10
                                                    1.
                                                                                                 (2.17)
                                (11                                                              (2.18)
                                                         H二
                                                   9-
                                                                                2
                                          =        '         2니&             =2, 3. ..,N.        (2.19)
                                                              9
                                                              H
                                                   k= 1

      The i-th codeword is the binary representation of a, t끄ncated to the first I:
      bits.

      Example 2: We apply the algorithm described here to const끄ct a Huffman
      code table using the symbol probabilities of Example 1. For a Huffman
Methods and Standaruis for Lossless Compression                             35




       Svmb아 i           ／갸        Unconstrained   A小hoc     Voor川S
       0              0.28200      11              II        11
       l              0.27860      10              01        10
       2              0.14190      0i l            10 1      011
       3              0.13890      010             100       010
       4              0.05140      0011            0010      001 1
       5              0.05130      0010            0001      0010
       6              0.01530      0001 1          001100    0001 1
       7              0.01530      00010           001101    00010
       8              0.00720      00001 1         000010    0000111
       9              0.00680      000010          000011    00001 10
       10             0.00380      0000011         000000    0000101
        II            0.00320      0000010         00000!    0000100
        12            0.00190      0000001         0011110   0000011
        13            0.00130      00000001        0011111   0000010
        14            0.00070      000000001       0011100   0000001
        15            0.00040      어刃000000        0011101   0000000
                                   2.6940          2.7141    2.7045
         avg




      Table 2.5       Voorhis method. Constrained-length (L = 7 bits)
      !-1i,ffm!in i 'ngIewr)rils




 codeword length constraint of L = 7 bits, the resulting codewords are as shown
 in Table 2.5. For comparison, we show the codewords for the unconstrained
 Huffman code table and the ad-hoc method described earlier. While both the
 ad-hoc design method and the Voorhis method satisfy the maximum codeword
 length constraint of L = 7 bits, the Voorhis method yields a lower average
 codeword length lavg. We further illustrate the performance of these two design
 methods in Figure 2.5. Here, we have used the symbol probabilities from
 Example 1, and we show the average codeword length for various maximum
 codeword length settings. In all instances, the Voorhis method outperforms
  the ad-hoc method, and the performance gap will widen as the maximum
 codeword length is increased.

 For a message composed of symbols from an N-symbol alphabet, if L =
 log9 N + d, then the Voorhis method has a complexity of O(dN2). The
 ad-hoc design has a lower complexity of O(N log2 N); however, the average
  36
                                                                                            CHAPTER 2




                    4.0




                9 8 7
                        5
                                    1




                          4
                            3 2
                                e




                                l 0 9 8


       小m듬나드gm石b多g8 g띤쁩 ＜
                                        7
                                1




                                            5
                                4




                3 3 3 b
                                1




                      3
                      n 3 3 3 3 3 3 2 2 2 b
                            1




                            1




                                          2 2
                            1




                            1




                                          n
                            1




                        1




                        1




                       1
                                                              朴“＼
                                                                卜卜兮寸HH쁘：娶끄쁘“d4
                       1
                                                                                 Voorhis method
                      1




                                                4   5          6           7          8           9
                                                    Ma川mum length 아 any codeword (b心）


       Fitrnre 2.5 Huffman codeword design. Comnarison of
         11 i    』1   i -  -   - .t                                 average
       coae iengtn  s netwe         - I I -
                             en me au-no      - I . Y 1, -
                                            c ann me voornis metnous.


codeword length is not necessarily minimized amon
                                                         g all possible codeword
choices. In image and video compression standards,
                                                         N is usually large, say,
256 symbols, and the ad-hoc design may be preferred in these
                                                                   instances. Note
that, regardless of the design approach, various imple
                                                         mentations may impose
additional constraints. For instance, in the Huffman tables
                                                              for the JPEG image
compression standard, there should be no Huffman codew
                                                               ord that is all ones;
that is, 11111...I. If the codeword design method yields
                                                            such a sequence, one
can simply take the complement of such a code table. The
                                                                 complement of a
Huffman code table is also a valid Huffman code table
                                                             and will satisfy the
unique prefix condition that is characteristic of all Huffman codew
                                                                       ords.
Me伽ds and St口nd口rds for L刃ssless Co仰res釘아i                                  37




2.8     ARITHMETIC CODING
The Huffman coder generates a new codeword for each input symbol. This
implies that the lower limit on compression for a Huffman coder is one bit per
input symbol. As observed earlier, higher compression ratios can be achieved
by combining several symbols into a single unit. However, in the Huffman
coding context, there is a corresponding increase in complexity in codeword
construction.

Another problem with Huffman coding is that the coding and the modeling
steps are combined into a single process, and thus adaptive coding is difficult.
If the probabilities of occurrence of the input symbols change, then one has to
redesign the Huffman tables from scratch. An alternative to Huffnian coding
is arithmetic coding.

Arithmetic coding is a lossless compression technique that benefits from
treating multiple symbols as a single data unit but at the same time retains
the incremental symbol-by-symbol coding approach of Huffman coding.
Arithmetic coding separates the coding from the modeling. This process
allows for the dynamic adaptation of the probability model without affecting
the design of the coder. Provisions for substituting Huffman coding with
arithmetic coding are contained in many of the image compression standards.
In this section, we briefly describe the basic concepts in arithmetic coding.



2.8.1   The Encoding Process

In the theory of arithmetic coding, a single codeword is assigned to each
possible data set. Each codeword can be considered a half-open subinterval
in the interval [0,1). By assigning enough precision bits to each of the
codewords, one can distinguish one subinterval from any other subinterval,
 and thus uniquely decode the corresponding data set. Like Huffman codewords,
 the more probable data sets correspond to larger subintervals and thus require
 fewer bits of precision.

 We describe the encoding process in arithmetic coding via an example. For a
 comparison with Huffman coding, we use the same alphabet (k, 1, u, w, e, r,?)
 and the same symbol probabilities as in the example shown in Figure 2.3.
 The message to be compressed is the string lluure?. We use ? as an end-
38                                                                                                                                                                                                 CHAPTER 2




of-message marker to terminate the decoding process. Using the Huffman
coder of Figure 2.3, the corresponding codeword would be the 18-bit string
010110이0000111011. For the arithmetic coder, the encoding process is
shown in Figure 2.6.


                                 1
                                                        1 四
Input                                                                      u                              u                              r                               e                          ?

                                 亞 19
                                                                            必： =
             1                                                                          .0714                             .07136 .071312                                                 .0713360
                     ?                                                          /
                                                                                n
                                                            2                       1
                                                                                                      '
                                                                                                                  ?        . ' ' ?   ''  ?                                                              2
                                 H                      나
                                                                                                                          I                                          I
                                                                                                                                                                 r                   1
                                                                                                  I                                                             g                    I
                     r                    r                     r
                                                                                              :
                                                                                              I
                                                                                                                  r                               r        ,'                    r                      r
                                                                                                                                                           S

                                                                                                                                                                                         11
                             H                          H                   H
                                                                                              I                                                           S
                                                                                                                          I
                                                                                                                                                      n
                                                                                              '
                                                                                                          -   -       -                 H1叫   =       m                  m


                                                                                         1




                                                                                                                              1111 11
                                                                                                                                                                                         111
                                                                                         1
                                         e                                              1
                     e                                          e
                                                                                e       1
                                                                                                              e                               e                              e                          e
                                                                                        1


                                                                                                                                                                                              111




                                                                                                                                                                                                    HH尸： L늚
                                                                낟                                                               111                                                            11



                     W U 寸               W U m
                             H
                                                                                                                                                                                               H

                                                                                                                                                                                 W
                                                                                                                                                                                               H


                                                                                                                                              WI '                                                          W
                             H
                                                                           H．쁘- I                         mm미 W                                                                                H

                                                                                                                                1
                                                            U                   U                                                                                                U                          U
                                                                                                              U                  '            U
                             H
                                                                                                                                 1
                                                            __I            mmd = m 1                  =1m                                                                                      H




                                                                    I                   *
                                                                     I          1       I
                 1                   1                      1         I         I        I                    1                                                              1                          1
                                                                       I                  I

                 戶k
                             而
                             叫




                                                                      ：二卜； :：그                                                      :．二k                       ；二k
                                                                                                                                                                                                                b


                                     I           \S         k                                                                                                                                           k
             0                                                         .070             .0710                                                                                            O
                                                      .06                                                                 .07128                      .071336




        Figure 2.6               Arithmetic coding. Example of the encoding process.




1. At the start of the process, the message is assumed to be in the half-
   open interval [0,1). This interval is split into several subintervals,
   one subinterval for each symbol in our alphabet. The upper limit of
   each subinterval is the cumulative probability up to and including the
   corresponding symbol. The lower limit is the cumulative probability up
   to but not including the symbol. For our example, the subinterval ranges
   are given in Table 2.6.
                                             ression                           39
Methods and Standards for Lossless Comp




                           Si    pi   Subinterval
                           k     0.05 [0.00,0.05)
                           l     0.20  [0.05,0.25)
                            U    0.10  [0.25,0.35)
                           w     0.05  따35,0.40)
                            e    0.30 [0.40,0.70)
                            r    0.20 [0.70,0.90)
                            1)
                                 0.10   [0.90,1.00)

                    Table 2.6     Symbol subinterval ranges.



                                                   appears, we select the corre-
  2. When the first symbol in our message, 1,
                                                        t interval. The intervals
     sponding subinterval and make it the new curren
                                                          scaled accordingly.
     of the remaining symbols in our alphabet are then
                                                          it out to have the same
     Intuitively, we take that subinterval and we stretch
                                                          nt. In our example, the
     length as before; however, the scale is now differe
                                                        0.25).
     original [0, 1) interval corresponds now to [0.05,
                                                               the upper limits of
     Let Previousj。 and Previoushi9h be the lower and
                                                           Previ   ous。  ，. = 0 and
     the old interval. In this example, at this stage,
     Pret'iOush19h = 1.
      Let Range = Previoushi9h - Previousz。     凹. After input 1, the lower limit
                                         tO + Range x subintervaii。     凹 of symbol
      for the new interval is Previousi。
                                                                       rly, the upper
      1. From Table 2.6, subinterva1,。，Uof symbol! = 0.05. Simila
                                                             x   subint ervalh19h of
      limit for the new interval is Previousi.,. + Range
      symbol 1. From Table 2.6, subintervali。  功 and subintervaihigh for symbol
                                                                  al are [0.05,0.25).
      1 are 0.05 and 0.25. Hence, the limits for the new interv
                                                           and upper limit of the
   3. After the second input, 1, we compute the lower
                                                                0.05 + (0.25 - 0.05)
      new interval as 0.05 + (0.25 - 0.05) x 0.05 = 0.06 and
       x 0.25 = 0.10.
                                                             the new interval are
   4. For the third input, u, the lower and upper limits for
                                                        and  0.06 + (0.10 - 0.06)
      computed as 0.06 + (0.10 - 0.06) x 0.25 = 0.07
      x 0.35 = 0.074.
                                                              ted using the limits
   5. The calculations described in previous steps are repea
                                                             the current symbol.
      of the previous interval and the subinterval ranges of
                                                               last symbol, ?, the
      This yields the limits for the new interval. After the
 40                                                               CHAPTER 2




                               Si    i   Cu rnpro히
                               k    7      0.00
                               l    6      0.05
                               U    5      0.25
                               텍    4      0.35
                               e    3      0.40
                               r    2      0.70
                                    l      0.90
                               1)
                                    0      1.00

                      Table 2.7     Modified decoder table.



      final range is computed. In our example, the final range is [0.0713336,
      0.0713360).

  6. There is no need to transmit both values of the bounds in the last interval.
     Instead, we transmit a value that is within the final range. In our example,
     any number such as 0.0713336, 0.07 1334, ..., 0.07 13355 could be used.
     We use 0.0713348389. The reader can verify that this number can
     be represented as 24 + 2m' + 2-10 + 2_15 + 2e16, and hence it can be
     represented with 16 bits.


In conclusion, the codeword length for the message lluure? is 16 bits with
an arithmetic coder, 18 bits with a Huffman coder, and 7 x 3 = 21 bits with
a fixed-length coder. Arithmetic coding yields better compression because it
encodes a message as a whole new symbol instead of as separate symbols.



2.8.2    The Decoding Process

The decoding process can be described using the same example. Let us assume
that the message lluure? was enc아led with 16 bits and that the corresponding
fractional value is 0.0713348389. Given the symbol probabilities, shown in
Table 2.6, to each symbol in our alphabet we assign a unique number (i) and
we associate a cumulative probability value cumprob:. For our example, the
modified decoder table is shown in Table 2.7.
Methods and Standards for Lossless Compression                             41




Given the fractional representation of the input codeword value, the following
algorithm outputs the corresponding decoded message. In our example, value
= 0.07 13348389.
     DecodeSymbol (value):
     Begin
         Previous,。iJ = 0.
         Previoush19h = 1.
         Range = Previousht9h - PreviousjO1,,.
         repeat
              Find i such that
                             - t'aIiie才
                   curnprobi <         ，evtous,O, , < curnprob1_ 1.
                                      Range
              Output symbol corresponding to i from the decoding table.
              Update:
              Previoush19h = Previousz。   W + Range * cumprobt. 1.
              Pre仇on旬ow = Pre仇O1LSlow + Range 水 cumprob1.
              Range = Previoushi9h - Previousi。      ，n.
         until symbol  decoded is?.
     End

 We show a few steps of the decoding process in our example.


                         切 = 0, Previoush29h = 1, and Range = I. For
  1. Initially, Previousi。
                             Ran。e us,O' < cumprob5. Thus, the first de-
     i = 6, cumprob6 < value-Prevw
     coded symbol is 1. As per'the algorithm shown above, we update
     Pre伉oushigh, Previous:。凹, and Range to 0.25, 0.05, and 0.2, respec-
     tively.
  2. We repeat the decoding process and we find that i = 6 satisfies again
     the limits c工mprob6 -< ua땅-   0.05 <c工mprob5. Thus, the second decoded
                                。.2。
     symbol is 1. The updated Previoush9h, Previousi。  w, and Range values
     are 0.10, 0.06, and 0.04, respectively.

  3. Repeating the decoding process yields that i = 5 satisfies the limits
     cumprob5 < va땅-。.。40.06 < cum끄rob4. Thus, the third decoded symbol is
     u. As before, we update Previo上sh19h, Pre仇o上s,。凹, and Range to 0.074,
     0.070, and 0.004, respectively.
42                                                                CHAPTER 2




 4. We repeat the decoding process as in previous steps. Finally, we decode
    ?, which signals the end of the message and terminates the decoding
    algorithm.




2.9 IMPLEMENTATION ISSUES
The encoding and decoding processes described in the previous section have
to be modified for a practical implementation of an arithmetic coder. Some of
these design issues are discussed next.


     Incremental Output
     The encoding method we have described generates a compressed bit
     stream only after reading the entire message. However, in most im-
     plementations, and particularly in image compression, we desire an
     incremental transmission scheme.
     From Figure 2.6, we observe that after encoding u, the subinterval range
     is [0.07,0.074). In fact, it will start with the value 0.07; hence, we can
     transmit the first two digits 07. After the encoding of the next symbol,
     the final representation will begin with 0.071 since both the upper and the
     lower limits of this range contain 0.071. Thus, we can transmit the digit
     I. We repeat this process for the remaining symbols. Thus, incremental
     encoding is achieved by transmitting to the decoder each digit in the
     final representation as soon as it is known. The decoder can perform
     incremental calculations too.

     High-precision arithmetic
     As we have illustrated in the example, most of the computations in arith-
     metic coding use floating-point arithmetic; however, most low-cost hard-
     ware implementations support only fixed-point arithmetic. Furthermore,
     division (used by the decoder) is undesirable in most implementations.
     Consider the problem of arithmetic precision in the encoder.
     During encoding, the subinterval range is na口owed as each new symbol is
     processed. Depending on the symbol probabilities, the precision required
     to represent this range may grow; thus, there is a potential for overflow
     or underfiow. For instance, in an integer implementation, if the fractional
     values are not scaled appropriately, different symbols may yield the same
                                                                              43
Methods and Standards for Lossless Compression




                                                           no subdivision of the
    limits for Previottshi9h and Previous,。; that is,
                                                        encoding would have to
    previous subinterval takes place. At this point,
    be abnormally terminated.
    Let subinterval limits Previousi。     功 and Previous,119h be represented as
                                                           subinterval is equal to
     integers with c bits of precision. The length of a
                                                          event s. If we represent
     the product of the probabilities of the individual
                                                          overflow or underflow,
     this probability with f bits of precision, to avoid
                                                   is the arithmetic precision for
      we require f 5 c + 2 and f + c 5 p, where p
                                                            computer, p = 16. If c
      the computations. For arithmetic coding on a 16-bit
                                                              ols from a k-symbol
     = 9, then I = 7. If the message is composed of symb
                                                               cannot be correctly
      alphabet, then 2/ 2 k. Thus, a 256-symbol alphabet
      encoded using 16-bit arithmetic.
                                                           ts in arithmetic coding
      In recent years there have been many developmen
                                                              operations, such as
       that allow fixed-precision arithmetic with simple
       shifts, additions, and subtractions.

     Probability modeling
                                                                 ol probabilities
     Thus far, we have assumed a priori knowledge of the symb
                                                          the arithmetic coder,
     p1. In many practical implementations that use
                                                              processed. This
     symbol probabilities are estimated as the pixels are
                                                                      . A typical
     allows the coder to adapt better to changes in the input stream
                                                                    s. Text and
     example is a document that includes both text and image
                                                              case, an adaptive
     images have quite different probability models. In this
                                                                         entropy
     arithmetic coder is expected to perform better than a nonadaptive
     coder.

                                                          the basis of various
 Huffman coding and arithmetic coding techniques form
                                                     section, we give a brief
 lossless image compression standards. In the next
                                                            rds.
 overview of the techniques used in the compression standa



                                         N
  2.10 STANDARDS FOR LOSSLESS COMPR亡SSIO
                                                          signals over public
  Standards related to the coding and transmission of
                                                     auspic  es of the telecom-
  telecommunication channels are developed under the
                                                        l Telecommunication
  munication standardization sector of the Internationa
                                                       the CCITT. The first
  Union (ITU-T). This sector was formerly known as
 44                                                                 CHAPTER 2




 standards for lossless compression were developed for facsimile applications.
 Scanned images used in such applications are bitonal; that is, the pixels take
 on one of two values, black or white, and these values are represented with
 one bit per pixel.



2.10.1    Facsimile Compression Standards

In every bitonal image, there are large regions that are either all white or all
black. For instance, in Figure 2.7, we show a few pixels of a line in a bitonal
image. Note that, the six contiguous pixels of the same color can be described



                                                  I II
               Figure 2.7 Sample scanline of a bitonal image.


as a run of six pixels with with value = 0. Thus, if each pixel of the image
is remapped from say, its (position, value) to a run and value, then a more
compact description can be obtained. In our example, no more than four bits
are needed to describe the six-pixel run. In general, for many document type
images, significant compression can be achieved using such preprocessing.
Such a mapping scheme is referred to as a run-length coding scheme.

The combination of a run-length coding scheme followed by a I-Iuffman coder
forms the basis of the image coding standards for facsimile applications. These
standards include the following:


      ITU-T Rec. T.4 (also known as Group 3). There are two coding
      approaches within this standard.

       I. Modified Huffman (MH)code. The image is treated as a sequence
          of scanlines, and a run-length description is first obtained for each
          line. A Huffman code is then applied to the (run, value) description.
          A separate Huffman code is used to distinguish between black and
          white runs, since the characteristics of these runs are quite different.
          The Huffman code table is static; that is, it does not change from
                                                                           45
Methods and Standards for Lossless Coinpression




                                                                  each line is
          image to image. For error-detection purposes, after
          coded, an EOL (end of line) codeword is inserted.
                                                               a previous line
       2. Modified Read (MR) code. Here, pixel values in
                                                       This is  followed by a
          are used as predictors for the current line.
                                                              in the MH code.
          run-length description and a static Huffman code as
           An EOL codeword is also used. To prevent error   propa   gation, MR
           coding is mixed with MH coding periodically.
                                                                ique used here
     ITU-T Rec. T.6 (also known as Group 4). The coding techn
                                                                 This code is a
     is referred to as a Modified Modified Read (MMR) code.
                                                             tion mechanisms
     simplification of the MR code, wherein the error-protec
                                                                ll compression
     in the MR code are removed so as to improve the overa
     ratio.

                                                         n (20:1 to 50:!) for
 These compression standards yield good compressio
                                                       osed of natural scenes
 business- type scanned documents. For images comp
                                                               the compression
 and rendered as bitonal images using a haiftoning technique,
                                                         on  the left possesses
 ratio is severely degraded. In Figure 2.8, the image
                                                             whereas the image
 characteristics representative of business document images
                                                   forme r is characterized by
 on the right is a typical halftone image. The




      U
      9


      U
      Q


      니
      n


       CU

       O
       小




                      Figure 2.8    Typical bitonal images.


                                                          code in the facsimile
  long runs of black or white, and the static Huffman
                                                                latter image, the
  compression standards is matched to these run-lengths. In the
 46                                                                CHAPTER 2




                             JBIG - Baselayer        ITU-T Rec. T.6
         Complexity         Three-line template,    2-D runlength,
         Parameters         AT-max = 16             Huffman code
         八'lemory           1589 bytes              1024 bytes
         Bu侄er              Three scanlines         Two scanlines
         Operations         Add, shift              Add, shift, compare
          Compression
         Halftone Image     5.2:1                   1.
                                                       1 5:
         Letter Image       48:1                   33.3:1

       Table, 2.8 Comparative analysis between JBIG and the ITU-T
       KeC. i .0 racsimiie compression sLanclaras.



run-lengths are relatively short, spanning only one to two pixels, and the static
Huffman code is not matched to such runs. An adaptive arithmetic coder is
better suited for such images.



2.10.2    The JBIG Compression Standard

Recently, a compression standard was developed to efficiently compress
halftone as well as business document type images. This is the JBIG
(Joint Binary Image Experts Group) compression standard. Its standards
nomenclature is ISO/IEC IS 1 1544, ITU-T Rec. T.82. The JBIG compression
standard consists of a modeler and an arithmetic coder. The modeler is used to
estimate the symbol probabilities that are then used by the arithmetic coder, as
we have described in a previous section. Previously encoded pixels are used as
a context for the model, and a probability estimate is derived from this context;
thus, with causal modeling, the decoder can mimic the encoder operations
without any additional information for the modeler. Additional features in the
JBIG standard support various image display and browsing modes. In Table
2.8, we provide a simple complexity analysis between the JBIG coding scheme
and the ITU-T Rec. T.6 facsimile compression standard. We also provide
compression ratios for two typical images: a 202 Kbyte halftone image and a
1 Mbyte image, primarily comprised of text. The latter image is referred to
as letter in the table. For business-type documents, JBIG yields 20 percent to
50 percent more compression than the facsimile compression standards ITU-T
                                                                               47
Methods and Standards for Lossless Compression




                                                           n ratios with JBIG
Rec. T.4 and Rec. T.6. For halftone images, compressio
                                                        facsimile compression
are two to five times more than those obtained with the
                                                            compression on a
standards. However, software implementations of JBIG
                                                 slower than implementations
general purpose computer are two to three times
of the ITU-T Rec. T.4 and T.6 standards.
                                                                 each plane
The JBIG standard can also handle grayscale images by processing
of a grayscale image as separate bitonal images.



 2.10.3    The Lossless JPEG Standard

                                                          compression standard.
 Most people know JPEG as a transform-based lossy
                                                           , has been developed
 JPEG (Joint Photographic Experts Group), like JBIG
                                                       descr  ibe this standard in
 jointly by both the ITU-T and the ISO. We will
                                                          we describe briefly the
 greater detail in a subsequent chapter; however, here,
                                                          standard. The lossless
 lossless mode of compression supported within this
                                                          t from transform-based
 compression method within JPEG is fully independen
                                                             tion residuals that are
 coding. Instead, it uses differential coding to form predic
                                                              coder. As explained
  then coded with either a Huffman coder or an arithmetic
                                                                  y; thus, they are
  earlier, the prediction residuals usually have a lower entrop
  more amenable to compression than the original image pixels.
                                                                   usly encoded
 In lossless JPEG, one forms a prediction residual using previo
                                                          prediction residual for
 pixels in the current line and/or the previous line. The
                                                            y can be any of the
 pixel X in Figure 2.9 is defined as r = y - X, where
  following functions:
                                          y= o                              (2.20a)
                                          y= a                              (2.20b)
                                           y= b                             (2.20c)
                                             y= c                           (2.20d)

                                   y= a+ b+ c                                (2.20e)
                                             b- c                            (2.200
                                  !/ ＝二 (1 +
                                              2
                                           m＝
                                                놔




                                           （工 -c
                                                                             (2.20g)
                                  V = b + ;;=1;
                                            2
                                          a+ b                               (2.20h)
                                      y     9
 48                                                                CHAPTER 2




 Note that, pixel values at pixel positions a,b, and c are available to both the



                                      C   b
                                      a   x




                 Figure 2.9    Lossless JPEG prediction kernel.


encoder and the decoder prior to processing X. The particular choice for the
y function is defined in the scan header of the compressed stream so that both
the encoder and the decoder use identical functions. Divisions by two are
computed by performing a one-bit right shift.

 The prediction residual is computed modulo 216. This residual is not directly
 Huffman coded. Instead, it is expressed as a pair of symbols: the category
 and the magnitude. The first symbol represents the number of bits needed to
 encode the magnitude. Only this value is Huffman coded. The magnitude
categories for all possible values of the prediction residual are shown in Table
 2.9. If, say, the prediction residual for X is 42, then from Table 2.9 we
determine that this value belongs to category 6; that is, we need an additional
six bits to uniquely determine the value 42. The prediction residual is then
mapped into the two-tuple (6, 6-bit code for 42). Category 6 is Huffman coded,
and the compressed representation for the prediction residual consists of this
Huffman codeword followed by the 6-bit representation for the magnitude. In
general, if the value of the residual is positive, then the code for the magnitude
is its direct binary representation. If the residual is negative, then the code
for the magnitude is the one's complement of its absolute value. Therefore,
codewords for negative residuals always start with a zero bit.

Example 3: Consider Figure 2.9 with pixel values a = 100, b = 191, c = 100,
and X = 180. Let y = 半；then y = 145, and the prediction residual is r =
145-180 = -35. From Table 2.9, -35 belongs to category 6. The binary number
for 35 is 10001 1, and its one's complement is 011100. Thus, -35 is represented
as (6, 011100). If the Huffman code for six is 1110, then -35 is coded by the
10-bit codeword 1110011 100. Without entropy coding, -35 would require 16
bits.
                                                                              49
Methods and Standardsfor Lossless Compression




              Category            Prediction Residual
                 0                             0
                  I                         -
                                                 1
                                                1,
                 2                        -3, -2, 2, 3
                  3                  -7, ..,-4, 4,..,7
                  4                 -15, .., -8, 8, .., 15
                  5                -31, .., -16, 16, .., 31
                  6                -63,..,-32,32,..,63
                  7               -127,..,-64,64,.., 127
                  8              -255,.., -128, 128, .., 255
                  9              -511, .., -256, 256,..,511
                  10            -1023, .., -512, 512,.., 1023
                  11           -2047,.., -1024, 1024,.., 2047
                  12           -4095, .., -2048, 2048,.., 4095
                  13           -8191,.., -4096,4096,.., 8191
                  14          -16383, .., -8192, 8192, .., 16383
                  15         -32767,.., -16384, 16384,.., 32767
                  16                         32768

                                                           ss JPEG corn-
       Table 2.9 Prediction residual categories for lossle
       pression.


                                                             Thus,the next six bits,
 In the decoder, the category (that is,6)is extracted first.
                                                                the most significant
 011100,correspond to the magnitude of the residual. Since
                                                                    complement of
 bit is zero, the residual is negative. After taking the one's
                                                            The a and b bits have
 011100, the decoded value of the residual r is -35.
                                                              y + 35 = 180.
 already been decoded; thus, y = 145 as before, and X =
                                                       context modeling and
 This notion of using a category table is a form of
                                                            of the prediction
 simplifies the Huffrnan coder. Without categorization
                                                           bet of 216 symbols.
 residuals, we would require a Huffrnan table for an alpha
                                                       codeword construction
 Such a large codeword table would complicate both the
 process and the decoding process.
                                                            images with more than
  Lossless JPEG outperforms JBIG for typical grayscale
                                                          yields better compression
  six bits per pixel. At six bits per pixel or below,JBIG
                                                                 ale version of the
  ratios than JPEG. For typical images, such as the graysc
 50                                                             CHAPTER 2




 halftone image of Figure 2.8, compression ratios in excess of 1.5 to I are
 quite difficult to achieve. The standards committee is currently working
 on developing new lossless compression techniques that can outperform the
 simple single-prediction, single-Huffman table coding method currently used
 in the lossless JPEG compression standard.




 2.11    TO PROBE FURTHER
We have reviewed some of the algorithms and standards for lossless compres-
sion. Huffman coding, in particular, is the most widely used entropy coder
in the standards. A general discussion on entropy coders can be found in any
textbook on information theory (e.g. [55]). The original description of the
Huffman coding scheme can be found in [77]. Variations and performance
bounds for Huffman coding are developed in detail in [56]. Most Huffman
coders have a a complexity of order O(八'log2 N). In [1271, Lu and Chen
present a Huffman code generator with complexity of order O(N). In this text,
we described the bottom-up approach to Huffman codeword construction. A
top-down approach is developed in [108].

In many practical implementations, the maximum codeword length of a
Huffman code needs to be constrained. In this chapter, we described several
approaches for constructing such a code. The Voorhis method [190] provides
a code-construction algorithm that attains the maximum codeword length
constraint and yields an optimum average codeword length. In recent years,
this problem has been revisited, and additional code generation methods are
described in [140], [109], and [126]. Another fast algorithm for optimal
length-limited I-Iuffman codes is described in [110].

Huffman coding methods are amenable to simpler software and hardware
implementations; however, techniques based on arithmetic coding tend to
yield a higher compression ratio. A detailed description of arithmetic coding
can be found in [17]. An introduction to arithmetic coding that also includes
source code is provided in [195]. There are several variants of the arithmetic
coder, such as the Q-coder developed by IBM [135]. The Q-coder is
an extension of the arithmetic coder described in the text. It includes a
probability estimation module for the modeler and replaces time-consuming
multiplications with additions and shifts. In [75], Howard and Vitter present
                                          ression                           51
Methods and Standardsfor Lossless Comp




                                       hmetic coder in which most of the
another reduced-precision binary arit
                                         ups.
operations are performed with table look
                                       s can be found in [811 and [82]. A
The ITU-T Rec. T.4 and T.6 standard                                     ription
                                  nson [78] provides a detailed desc
survey paper by Hunter and Robi                                   desc ribe d in
                                      the JPEG standards are
of the T.4 standard. The JBIG and
                                        . In [11], Arps and Truong provide
the ISO/ITU-T documents [85] and [83]
                                           algorithms for still-image lossless
a detailed comparison of all the standard
                                     up 4, JBIG, and lossless JPEG.
compression, including Group 3, Gro
                                                                     3
             FUNDAMENTALS OF LOSSY
                IMAGE COMPRESSION




3.1 INTRODUCTION
                                                      processes where decom-
Lossy compression of images deals with compression
                                                         al image data. A wide
pression yields an imperfect reconst끄ction of the origin
                                                        oped   for compressing
range of lossy compression methods have been devel
                                                          categories shown in
still-image data. These methods fall into one of the
                                                              concepts of lossy
Figure 1.2. In this chapter, we describe some of the basic
                                                          form the basis of the
compression that have been adopted in practice and that
image and video compression standards.

                                                           compression method
As discussed in Chapter 1, the selection of a particular
                                                            ression method that
involves many tradeoffs. However, regardless of the comp
                                                        tion), there is always a
is being used, given the level of image loss (or distor
                                                                 . We begin this
bound on the minimum bit rate of the compressed bit stream
                                                          s from rate-distortion
chapter by briefly describing such a bound using result
                                                             n schemes, and we
 theory. Next, we describe some practical lossy compressio
                                                          mance bound. Special
compare their performance against the theoretical perfor
                                                        es, since they form the
 emphasis is given on DCT-based compression schem
                                                      rds. We conclude with a
 basis of all the image and video compression standa
 discussion on the fast implementation of the DCT.
 54                                                                                         CHAPTER 3




 3.2 PRELIMINARIES

 3.2.1 A Model for Spatial Correlation in Images

 Image data tend to have a high degree of spatial redundancy. Furthermore,
 image data are eventually presented to a human viewer. Thus, if one views
 a lossy still-image compression system from end to end; that is, from the
 creation of the visual information to the eventual display of the information
 after decompression, then it is p끄dent to exploit characteristics within each
 component of this system so as to generate a compressed stream with the
 fewest number of bits. Within such a system, compression is achieved by
 exploiting both the spatial redundancies within the image and the perceptual
 characteristics of the human visual system so that loss due to compression may
 not be discernible to the viewer.

It is also possible to exploit some higher-level image characteristics or, for
color images, to exploit correlation of data among different color components.
For example, compression schemes based on fractals provide an image
representation based on patterns that are repeated at different scales within the
same image. Since the compression standards are not based on the existence
of such features, we do not discuss any of these compression schemes in this
book.

By spatial redundancy, we imply that pixels are correlated across space. For
any image X, the spatial redundancy can be modeled by a two-dimensional
(2-D) covariance function. A typical isotropic (nonseparable) covariance
function for image data is given by

                               vx (i, j) = O2eH.＼石＝;1
                              C。                    ',                                           (3.
                                                                                                            1)
where .2 is the variance of the image and i and j refer to the distance from the
reference pixel about which the covariance function is defined. If we denote
the 2-D image samples as X(i, j), let

                                                                                  i)1           (3.
                                  =                          ,,』Y.

                       Pi
                                          E[
                                                        r)
                                                X
                                                                     ci_
                                                                           :,1,
                                                                                        ,
                                                    乙［入 1 (i口 기
                                                                                                       2)
                                                    (
                                               피x往기x（幻 m 1)]
                                                                                                (3.3)
                              '
                                      =

                                                        피xm口）]
                        n1\
denote the correlation between two pixels in the vertical and horizontal
directions, where E[ ] is the expectation (or averaging) operator. If we assume
                                                                             55
Fundamentals of Lossy Image Compression




                                                       vertical and horizontal
P1 = P2; that is, there is no difference between the
                                                                   data, typical
correlation of two neighbor pixels, then e口 = p. For image
                                                             of the covanance
values for P1 and P2 are around 0.95. A simple calculation
                                                           covar iance function
function for various values of i and j indicates that the
                                                          finding suggests that
decays rapidly and is quite small beyond i .7 > 8. This
                                                         need   not to consider
compression schemes that exploit spatial redundancy
                                                    the vertical or horizontal
blocks of pixels larger than eight pixels in either
dimension.

                                                 model for the spatial
Under the compression context, this mathematical
redundancy within an image serves two purposes:

                                                        compression system.
  1. It can be used to design components of the image
                                                        and the decompressed
  2. Given that the distortion between the original
                                                              on the lowest bit
     image is D, it can be used to derive a theoretical bound
                                                          scheme. A common
     rate R(D) that is achievable with any compression
                                                               ed and decoded
     measure for D is the mean square error between the encod
                                                             X(i, j).
      images, normalized by the variance of the input signal

                                                               R(D) relationship.
 In the next section, we discuss in more detail the D versus



 3.2.2   Rate-Distortion Function for Images

                                                                    r compression
 Due to the loss of information, lossy compression yields highe
                                                                      compression
 ratios than lossless compression. However, in any practical lossy
                                                             D) and the bit rate of
 system there is a tradeoff between loss or distortion (say
                                                               in bits per encoder
 the compressed bit stream, (say R). Here, R is expressed
                                                         the encoder input. If the
 output symbol, and D is normalized by the variance of
                                                              can be expressed as
 encoder input data are 8-bit pixels, the compression ratio
                                                       minimum bit rate J?min so
  읖. Rate-distortion theo口 establishes the theoretical
                                                           the allowed distortion
  that the compressed input can be reconstructed within
                                                             R relationship. For a
 D. For every compression scheme, there is a D versus
                                                            the minimum possible
  given D, the rate-distortion function R(D) is defined as
                                                                    is independent
  rate R necessary to achieve average distortion D or less. R(D)
                                                                on the underlying
  of the particular compression method and depends only
                                                             measure.
  stochastic model for the input images and the distortion
 56                                                                               CHAPTER 3




 As observed in the previous chapter, in lossless compression, the efficacy of
 a compression method is determined by the entropy of the source at the input
 of the entropy encoder. Furthermore, the entropy of the source depends only
 on the underlying statistical model for the source. Similar observations can be
 made for lossy compression schemes.

In lossy compression, the source-coding theorem states that it is possible
to design a coding-decoding scheme of rate R > R(D) so that the average
distortion is D or less. The converse of the source-coding theorem states that if
a coding-decoding system has rate R <R(D), then it is impossible to achieve
average distortion D or less with this system. These two theorems imply
that R(D) defines the lowest possible bit rate among all lossy compression
methods. When D = 0, R(D) is the source entropy.

Since R(D) defines the lower limit for achievable compression ratio for a
specified distortion D, it would be informative to compute R(D) for an image.
The resulting R(D) can then be used to determine if a desired compression
ratio is achievable in practice.

For the isotropic covariance function defined in (3.1), and a2 = 1, the 2-D
power spectral density of an image X has the form


                                                                                       (3.4)
                       敬（/:,/;)=   : , (/   ：七／
                                                  긍）
                                                          글    :
                                                                   S0
                                                                        (f)   ,




毗町 기厘n加印枷ssume帥如毗r sp吼帥帥ndlimit叱
such that Sx (f, f) = 0 for I > 去. Let P1 = P2 = 0.95, assuming Nyquist
San}PhngandaP
sampling        PrOXinlahn
          and approxima tingem
                             e ' = 1-
                                  l吐； x; then:
                                         then j = 005

It has been shown by Berger that the optimal encoder-decoder tandem yields
distortion D(O) and a minimum rate R(O) given by

           D(G)    =   /:/:mm （日Sx (/ ）可：
                                    「
                                                       :,fy)            吼，
                                                                                       (3.5)
           n/,,\        tm 1的 4小q /', 1 , .' SXr'f工 ' f
                                                      "V)'\ Jr Jr                      /a <\
           R(O)    =   /   /  772OT 1 0긍m92 V八 ' ": ' " y ' )dfdf.",.                  (3.6)
            "          人口D人的叫 \ ' 2勺       （      0         / '- --Is                  "

Parameter 0 takes on all positive real values and generates the function R(D),
which we refer to as the rate-distortion function for this source.
Fundamentals of Lossy Image Compression                                                                            57




For the bandlimited Sx (fx, fV) of (3.4), by varying 0, the function R(D) can
be computed using (3.5) and (3.6). Closed form expressions for D(6) and R(9)
can be obtained as follows:

If f (8) :; 士，

            D(6)        =    何Pf2／       月＼ +   f
                                                    ,   /   1                                       1        \   (3.7)


            R(9)
                             磊小只缸小）),                                                                             (3.8)

and if f（이 > 去 ,
                 D(9)       = 9,                                                                                  (3.9)
                                                                                                             9
                                                                                                            令H
                                                                l e冗                       l1 1n乙
                 R（이 = 島（:。느乞긍
                                                                       \
                                                                                                    O
                                                                                                    +
                           J2 『                                                                                  (3.10)
                                                                                                    U
                                                                                                    O
                                                                           1
                                                                                                        =
                                                                                                        n
                                                                               1
                                                                                   /
where 9 and 4) are defined as
                                                         fo                                                      (3.11)
                                          =                                            }

                                                2冗（f2(0) + ／孑）글
                                     9
                                                       fo                                                        (3.12)
                                          :=
                                                27r(l, +／計글 '
                                41
Figure 3.1 shows the rate-distortion function for various image models. In
this figure, SNR is defined as 101091。去 For the 2-D isotropic model, we
show the R(D) plot computed using (3.7) to (3.10). For comparison, R(D) is
also plotted for an image modeled using a one-dimensional (1-D) covariance
function and for an image with uncorrelated data. If the image is uncorrelated
and the samples have a Gaussian distribution, the corresponding R(D) function
                                                                  be made:
is given by - 1092 去；. From this figure, several observations can

  1. For the same image fidelity, exploiting 2-D correlation in the image leads
     to lower R(D) (more compression) than if the image were assumed to be
     correlated only along one direction. Specifically, for the assumptions on
     which the R(D) calculations were based, a doubling of compression ratio
     is achieved.
  2. If the image is uncorrelated or if the correlation is weak, then there is a
     significant degradation in compression, as seen by comparing the R(D)
  58
                                                                                                 CHAPTER 3




                3.50
                                                                                                                 //
                                                                                                             /
                                                                                                         /
                                                                                                     /

                3.00                                                                             /




                  0
                 U
                 <n<                      Uncorr이카ed                                 .

           0
                                          (Gaussian)
                  0
                                                                                 ,

           0

                 b
                 =d11
            n<




       小m죠Emm＞ 느
               딴 으m工


                1.00                     1-D Correlated
                                                                            2-D Corre冶旭d

          0.50


         0.00

                        0.00      5.00     10.00            15.00     20.00      25.00               30.00
                                                         SNR (dB)



        Figure           3.
                              1 Rate-distortion    pe汗
                                                            "rmance   for
                                                                            various      image
                                                                                                         mod-
         els.
     plots for the Gaussian source model and the 2-D corre
                                                           lation source model.
     A quadrupling of the compression ratio is obtained in the
                                                                  latter case for
     the same image fidelity.

  3. In regions of low image fidelity (low SNR), explo
                                                       iting spatial redundancy
     in both dimensions of the image does not offer any
                                                          significant reductions
     in the compression ratio. In these regions, the
                                                      coding gain provided by
     the better correlation model is offset by the distortion
                                                              introduced in the
     lossy compression scheme.


The R(D) function has several practical uses:
                                                                                  59
Fund口menials可／刃ssy Im口ge Compression




                                                             can be estimated,
    For sources where the correlation coefficients P1 and P2
                                                              ine whether the
    the equations described above can be used to determ
                                                          icial. In a practical
    exploitation of spatial redundancies would be benef
                                                           redundancy has a
    coder, a compression method that exploits spatial
                                                         es that the source is
    higher complexity than a coder that simply assum
                                                                insight into the
    uncorrelated. Thus, the R(D) function can provide some
                                                                 er 1.
    R versus D versus complexity tradeoffs discussed in Chapt
                                                                    ponding rate R
     For practical coders, one can measure D and the corres
                                                                 This comparison
     and compare them against the theoretical limit R(D).
                                                        . In gener  al, it is difficult
     will determine the efficacy of the practical coder
                                                                     nt parameters
     to compare one coder against another, given the differe
                                                                  the performance
     used by each coder. However, one can always compare
                                                                        comparisons
     of each coder against the theoretical limit R(D). These
                                                                     in Figure 3.1,
     can then be used to compare the two coders. Note that,
                                                                     comp    aring the
     the SNR is computed for a unit variance source. When
                                                                    axis has to be
     results of a practical coder against this plot, the SNR
                                                            varian ce  of the source
     scaled appropriately to account for the estimated
                                                                        also be used,
     being compressed. Instead of SNR, peak SNR (PSNR) may
                                                          scaled accor   dingly.
     provided that the horizontal axis in Figure 3.1 is
                                                                    ize the design
     In a practical setting, the R(D) function can be used to optim
     of functional blocks within the encoder and decoder.

                                                                   ale image with
 For example, assume we want to compress an 8-bit graysc
                                                               the  2-D correlated
 a maximum distortion of 20 dB. From Figure 3.1, using
                                                                    corresponds to
 model, the lowest bit rate is close to 0.9 bits per sample, which
                                                           a comp  ressio n ratio of
 a compression ratio of 8.88 to 1. Similarly, if we want
                                                               e is close to 16 dB.
 20 to I (or 0.4 bits per sample), the best SNR we can achiev
                                                             stic image model.
 In the calculations for R(D), we have assumed a stocha
                                                     to the stochastic model is
 For images, using a perceptual model in addition
                                                                ying the power
 more appropriate. This can be done quite simply by modif
                                                                    W(f, fV) is
 spectral density Sx (f, fV) of (3.4) as W(f, fV)Sx (f, f) , where
                                                            l system.
 an estimate of the frequency response of the human visua
                                                                in Figure
 The reader must exercise caution when comparing the R(D) plots
 3.1 with the measured data from a specific coder, since
 60                                                                 CHAPTER 3




      in deriving the closed-form expressions for D and R, some assumptions
      were made regarding the bandwidth of S.v (f工. fy),

      the R(D) function was computed for specific values for the correlation
      coefficients P1 and P2, and these values may change from image to image,
      and

      the distortion metric used in the specific coder may not be the mean-
      squared error (MSE) metric which we have used here.


Later in this chapter we consider two of the lossy compression schemes that
are the basis for the image compression standards, and we compare their
performance against the theoretical rate-distortion bound we have described
here. In another chapter, we will revisit the R(D) formulation and extend it to
video coding.




3.3 BASIC CODING SCHEMES FOR LOSSY
    COMPRESSION
There are two classes of lossy compression schemes for images: sample-based
coding and block-based coding.



3.3.1 Sample-Based Coding

In sample-based coding, the image samples are compressed on a sample-
by-sample basis. The samples can be either in the spatial domain or in the
 frequency domain. A simple sample-based compression method is a scalar
predictive coder such as the differential pulse code modulation (DPCM)
method shown in Figure 3.2. This scheme is very similar to the one used
in lossless JPEG (described in Chapter 2), except that in lossless JPEG there
is no quantization. For each input sample r,7, a residual signal e, is formed
using the prediction signal P,,. P,3 is typically a weighted sum of previously
decoded pixels near xij. If the image is highly correlated, P, will track xij, and
e,3 will consequently be quite small. A typical uniform quantization function
is shown in Figure 3.2b. The quantizer maps several of its inputs into a single
output. This process is irreversible and is the main cause of information loss.
                                                                                61
Fundam?entals of Lossy Image Compression




                                                                  q 11




                                                                           eU




                         (a)                                     (b)



                                                                   ing block
      F.igure 3.2 . . DPCM compression.method. .(a). Encod      quanu zer.
      diagram; (O) input-outpu t cnara cterisu cs oi a typica t


                                                          of xi,, quantizing e,
 Since the variance of 口j is lower than the variance
                                                          e, the lower variance
 will not introduce significant distortion. Furthermor
                                                    compression. As mentioned
 corresponds to lower entropy and thus to higher
                                                      decays rapidly at distances
 earlier, for typical images, the covariance function
                                                     is no benefit to using more
 longer than eight pixels. This implies that there
                                                   Pj. Practical DPCM systems
 thaii an eight-pixel neighborhood when forming
                                                          ple,
 use three previously decoded pixels near x:7. For exam

                     ／긱-7 = Wi秀ii-' + w2上卜13-1 + w3士1尸13,

 where w1, w2, and w3 are constant weights and

                                  土iJ = ／屯 + q13

 denotes the decoder's estimate for x,j.

                                                        range卜255, 255]. The
 If x7 represents 8-bit pixels, then e,7 will be in the
                                                           may occupy the same
 quantizer remaps e:j into the quantized data qjj, which
                                                      their representation. For
 dynamic range as e,3 but require fewer bits in
                                                          the quantized data can
 example, if there are only 16 quantization levels, then
 be represented by only four bits.
                                                             R(D) bound that we
  DPCM coders do not yield performance close to the
                                                        by (3.13). If we assume
  described in the previous section. Let Pj be given
                                                        cient p and if the effects
  an isotropic covariance model with correlation coeffi
                                                            on function for DPCM
  of quantization noise are ignored, then the rate-distorti
   62
                                                                          CHAPTER 3




  can be expressed as


                                                           ]
                                                           1 H9
                                                              尸
                    R(D)DPC.\I = R(D) unc。                        O
                                                                  J   G
                                         rrelated -               O
                                                                  D
                                                                  e   小
                                                                               (3.15)
  where G7, is the gain due to prediction and is given
                                                           by

                                           \       /   2
                               아 = 1 寸＼
                                           .   .




                                       l ＋少寸                                   (3.16)

  For p = 0.95, DPCM coding yields a hit rate that is lower
                                                                   by I .97 bits per
  sample than the bit rate of the uncorrelated source. To visual
                                                                     ize this plot, in
  Figure 3. 1 simply shift down the R versus D curve labeled Unco
                                                                          rrelated by
  I .97. In practice, the effects of quantization noise cannot be
                                                                   ignored, and the
  true DPCM performance is nearly 6 to 10 dB worse than
                                                                  the R(D) bound
  shown in Figure 3. I for the 2-D correlated image model. The
                                                                      computational
 complexity of DPCM is quite reasonable. For example,
                                                               if Pj is computed
 using three prior samples, then computing P, requires three multip
                                                                             lications
 and two additions, computing e,7 requires one subtra
                                                           ction, and forming q1,
 requires one multiplication, for an overall cost of four multip
                                                                       lications and
 three additions per pixel. Since most of the multiplicatio
                                                                ns involve small
 constants, lookup-table-based multiplication or multiplicatio
                                                                 n using shift and
 add operations is sufficient.



3.3.2    Block-Based Coding

 From rate-distortion theory, the source-coding theore
                                                          m shows that as the size
 of the coding block increases, we can find a coding schem
                                                                e of rate R > R(D)
 whose distortion is arbitrarily close to D. In other words
                                                             , if a source is coded
as an infinitely large block, then it is possible to find
                                                          a block-coding scheme
 with rate R(D) that can achieve distortion D. This implie
                                                            s that a sample-based
compression method, such as DPCM, cannot attain the
                                                            R(D) bound and that
block-based coding schemes yield better compression ratios
                                                                 for the same level
of distortion. Many compression techniques have been
                                                            developed to operate
in a blockwise manner. These techniques fall into
                                                      one of two classes: spatial
domain block coding and transform-domain block
                                                       coding.

In spatial-domain block coding, the pixels are group
                                                       ed into blocks and the
blocks are then compressed in the spatial domain. Vecto
                                                         r-quantization-based
methods fall into this category. Vector-quantization (VQ)
                                                           methods require far
                                                                             63
Fundamentals of Lossy Image Compression




                                                   er and are described in more
more processing in the encoder than in the decod
                                                  viewpoint, for the same rate,
detail in a later chapter. From a rate-distortion
                                                    SNR than DPCM methods.
such coders yield images with at least 3 dB better
                                                 grouped into blocks and the
In transform-domain block coding, the pixels are
                                                    as the frequency domain.
blocks are then transformed to another domain, such
Let us define two N x N transformation matrices
                                                                          (3.17)
                     Tb   = 位他아 , u. i= O, 1, ..,N- 1,
                                                                          (3.18)
                     Tr   = {tr (V, j)}.V. j= O, 1, ..,N_ 1.
                                                   then the N x N linear
If the 2-D image in the spatial domain is X,
                                                  TCXT, where T denotes
transformation process can be expressed as Y =
                                                      are also referred to as
the matrix transpose of Tr. The T and Tr matrices
                                                         kernels, T = Tr = T
transformation kernels or basis functions. For symmetric
and Y = TXTt.
                                                         in Y a more compact
 The motivation for transforming X into Y is to obtain
                                                         compression methods
 representation of the data in X. Lossy transform-based
                                                          ion from X to Y and
 achieve compression by first performing the transformat
                                                   in Y.
 then by discarding the less important information
                                                            ed at some point by
 In any practical system, the compression process is follow
                                                           be reversible so that
 decompression. Thus, the transformation process has to
                                                               ic T, there should
  V can be reconstructed from Y. It follows that, for a specif
 be a U such that X = UYUt.
                                                           T include the basis
 Some of the most commonly used basis functions for
                                                               discrete cosine
 functions of the discrete Fourier transform (DFT'), the
                                                            discrete Hadamard
 transform (DCT), the discrete sine transform (DST), the
                                                         (KLT). In Figure 3.3,
 transform (DHT), and the Karhunen-Loeve transform
                                                                 . Dark regions
 we show the output of the transform process for a typical image
 indicate less energy.
                                                          most efficient in terms
  From this figure, it is seen that the KLT basis is the
                                                           acted into the top left
  of compaction efficiency, since all the energy is comp
                                                            its basis functions are
  corner. The DHT basis has poor compaction efficiency;
                                                         the DCT or DST basis.
  rectangular compared to the smoother functions for
                                                           the sense that
  The KLT is considered to be the optimum transform in
64
                                                                            CHAPTER 3




      (a) Test Image                           b) Discrete Fourier transform




     (C)［기screte Co듸ne trans幻rm
                                              (d) Discrete Sine transform




 (e)［긔screte Haclamard 打ans幻rm               (f) Karhunen-Loeve transform



     Figure 3.3        Compaction efficiency for various image transforms.
F刃idamentals可I刃ssy Image C이刃pression                                         65




 1. it packs the most energy in the fewest number of elements in Y,
 2. it minimizes the total entropy of the sequence, and
 3. it completely decorrelates the elements in X.

However, the KLT has several implementation-related deficiencies, including
the fact that the basis functions are image dependent. The other basis functions
such as DFT, DCT, DST, and DHT are image independent. Among them, the
transform output for the DCT basis is seen to be close to the output produced
by the KLT; that is, its compaction efficiency is close to that of the KLT. Since
it has a performance very close to the KLT, the DCT basis is widely used in
image and video compression and is the basis of choice for all the image and
video compression standards. In the next section, we will discuss the basics of
image coding using the DCT basis.



3.4 DCT-BASED CODING
DCT-based image coding is the basis for all the image and video compression
standards. The basic computation in a DCT-based system is the transformation
of an N x N image block from the spatial domain to the DCT domain. For the
image compression standards, N = 8.

An 8 x 8 blocksize is chosen for several reasons. From a hardware or software
implementation viewpoint, an 8 x 8 blocksize does not impose significant
memory requirements; furthermore, the computational complexity of an 8 x
8 DCT is manageable on most computing platforms. From a compaction
efficiency viewpoint, a blocksize larger than 8 x 8 does not offer significantly
better compression; this is attributable to an observation we made earlier with
regard to the dropoff in spatial correlation when a pixel neighborhood is larger
than eight pixels.

 The choice of the DCT in the standards is motivated by the many benefits it
 offers:

     For highly correlated image data (correlation coefficients p1, P2 > 0.7),
     the DCT compaction efficiency is close to that obtained with the optimum
     transform, namely, the K工
66                                                                                                                                     CHAPTER 3




     The DCT is an orthogonal transform. Thus, if in matrix form the
     DCT output is Y = TXTt, then the inverse transform is X = TtYT.
     The tranSf0rnlah0n   8x8DCT i ., which is commonly referred to as the
         transformation AY -*
     forward DCT or simply the DCT, is expressed as

        Yki
              =
              --   "
                   c   C
                       (k)   '}   4
                                  c    (
                                       (l)   ')   5泣小/
                                                  ! =O j= 0
                                                                          (2i+        1)   kir\
                                                                                                  '
                                                                                                      )cos   O5 f
                                                                                                                    "
                                                                                                                        (2j+   161)   lir\   )'   (3. 19)
     where k, I = 0, 1, ..., 7 and
                                                                                      if 丸 = 0
                                                                                                                                                  (3.20)
                                                         咐）    =   1.            1    otherwise

     The DCT transformation can also be expressed in vector-matrix form as
                                                                         !/ = T乙                                                                  (3.21)
     where                                               .....x70, x71, ...,x77}, T isa 64
            x = {x00, x01. .....i:07, x10..r11. ...,x17.
      x 64 matrix whose elements are the product of the cosine functions defined
     in (3.19), and y = {yoo, Yol. ....Yo7, Yio, Yii, ..., y17, ..., Y70, Y71, ..., Y77}.
     The DCT transformation decomposes each input block into a series of
     waveforms, each with a particular spatial frequency. The 64 waveforms
     composing the DCT basis functions are depicted in Figure 3.4. The
     DCT transformation can be viewed as the process of finding for each
     waveform shown in Figure 3.4 the corresponding weight Yki so that the
     sum of the 64 waveforms scaled by the corresponding weights yki yields
     the reconstructed version of the original 8 x 8 matrix X.
     From (3.19) and the orthogonality property of the DCT, the 8 x 8 inverse
     DCT transform (commonly referred to as IDCT) can be derived as
                       口              .7

                   v八늑                              c(k)c(l)            1 (2i + 1)k7r '\                       ( (2j + 1)17r '\
                                                                                                                                                  (3.22)
              =/y.=.9k1
               LL.
               k=0 1=0 Yk1
                                                         4     CO「'\                 l6
                                                                                     16           )' cos I                     16            7'
     where 乙7 = 0, 1, ..., 7. Note that, the computations for the forward and
     inverse DCT are nearly the same. Thus, from a hardware implementation
     viewpoint, the same computation unit can be used for both the forward
     and the inverse DCT.
     An important property of the 2-D DCT and IDCT transforms is separabil-
     ity. The 1-D DCT is computed as


                   :(＝뿌5二2;, cos(（「"", )' "), 山小·，7.
                                                   z=0
                                                                                                                                                  位23)
Fundainen tals of Lossy Image Compression                                                                                                                                    67




                       Figure 3.4                              The 64 8 x 8 DCT basis functions.


     This equation can also be expressed in vector-matrix form as z = Txt,
     where T is an 8 x 8 matrix whose elements are the cosine function values
     defined in (3.23), x = [xo, x1, · . . ,x7] is a row vector, and : is a column
     vector. From (3. 19), the output of the 2-D DCT can be expressed as


                                   小5(   「
                                       (2‘                                                                                                                    ，:)k「). (3.24)
                      臼
         如＝뿌夕c(1)自73 COS 「,,' )' "
                                i= 0 1                     j= 0                              \                                    '           I


     Let
                                                                                                 + 1)                                                                      (3.25)
                                                                      Cos
                                                                                                                              .

                                                                                                                                              = 0, l , · . · . 7
                                            (1)
                                        c
                                                                                                             1ir
                                                                                   (21
                      二il       =
                                             2                                 \                   16                     J
                                                                               (
                                                  j= 0


     4enote the output of the I -D DCTs of the rows of xj. The above equations
     iiirnlv that the 2-D DCT can be obtained by first performing l-D DCTs
     口




      뇨．     rows or Tl7 rotiowea Dy 卜U VLi S or tne COIUWflS or :n · in mairix
                                    C             C   II               I   I             I   1-s   r    r,         ,T '       -   C       I       -   ' I          C   낙     .



     qi tue
                                                                                                                                      .
         :1
              '   -         -                              -      -




     Ootation, Y = TXTt and this can also be expressed as

                                                                      Z            =             TX ' ,                                                                    (3.26)
68                                                                CHAPTER 3




                               Y = TZt = TXTt .                            (3.27)

     From an implementation viewpoint, this row-column approach may also
     simplify the hardware requirements at the expense of a slight increase in
     the overall operations count. This issue is covered in more detail in a later
     section of this chapter.

     The DCT basis is image independent. This is an important issue in
     compression, since an image-dependent basis implies that additional
     computations need to be performed to determine the basis. Image
     independence, however, will result in some loss of performance.

     As observed earlier, the spatial-domain block is decomposed by the
     DCT in terms of the 64 waveforms shown in Figure 3.4. Since each
     Yk! represents the contribution of the corresponding kl-th waveform, the
     characteristics of the human visual system could be easily incorporated
     by suitably modifying yki. Compare this with a spatial domain coding
     technique such as DPCM.In DPCM,it is not intuitively obvious how the
     prediction residual can be modified to account for the characteristics of
     the human visual system.

     The DCT computations as expressed in (3.19)or(3.23)can be performed
     with fast algorithms that require fewer operations than the computations
     performed directly from these equations. Fast algorithms are desirable
     from both a hardware and a software implementation viewpoint. These
     fast algorithms also tend to be parallelizable and thus can be efficiently
     implemented on parallel architectures. We will describe some fast DCT
     algorithms later in this chapter.



3.4.1   A Generic DCT-based Image Coding System

Figure 3.5 shows the key functional blocks in a generic DCT-based image
coding system. This diagram represents the core computation pipeline em-
ployed in all the lossy image and video compression standards discussed in
this text. In the encoder, the DCT process transforms each 8 x 8 block X
into a set of DCT coefficients Y. As noted earlier, each of these coefficients
is the weight associated with the corresponding DCT basis waveform. In the
lossy compression mode, some of the weights will be deleted and thus the
corresponding waveforms will not be used during decompression. The process
Fundamentals of Lossy Image Compression                                  69




                      Image




                                           Spatial-to-DCT Domain
                                      t>       Trans幻rmat幻n
                                                 8 x 8 DCT


                                                     V
                                             Discard Unimportant
                                            DCT Domain Samples
                                               Quantizat佃n


                                                     V
                                              Lossless（沁비ng
                                           아 DCT Domain S카nples
                                              Entropy Coding

                                                     1
                                           Lossy Compressed Data


              Figure 3.5      Generic DCT-based coding system.



of deleting some of the weights is referred to as the quantization process
in Figure 3.5. The quantization process is an irreversible process and is the
only source of loss in a DCT coding scheme. Strictly speaking, even with
no quantization, there may be additional losses related to the implementation
accuracy of the DCT and IDCT. Furthermore, in a transmission application,
there may be additional losses due to noise in the transmission link.

 After quantization, the nonzero quantized yki values are then compressed in
 a lossless manner using an entropy coder. In most applications, the entropy
 coder combines a run-length coder with a Huffman coder. Entropy coding
 specifics are discussed in detail in a later chapter on the JPEG still-image
 compression standard.

 We provide two examples that illustrate the various steps performed during
 compression and decompression in a DCT-based coding system.
70                                                                   CHAPTER 3




Example 1: The DCT coding for a typical image is shown in Figure 3.6. Here,




                        Compress幻n           1    Decompression

                    DCT寸＞   Quantize
                                          극伊 們，,芦,＋就T
                                             1




       Origrna                                                    Decompressed




                                        Coding Error



                   Figure 3.6          DCT coding - an example.


the input 8 x 8 block (labeled original) is taken from a low activity region;
that is, there are very small differences among pixel values in that area. The
F月xel values 如r this 비ock are 엠yen by
Fundamentals of Lossy Image Compression                                                                      71




                    168       161       161                150   154       168      164          154
                    171       154       161                150   157       171      150          164
                    171       168       147                164   164       161      143          154
                    164       171       154                161   157       157      147          132
            x=
                    161       161       157                154   143       161      154          132
                    164       161       161                154   150       157      154          140
                    161       168       157                154   161       140      140          132
                    154       161       157                150   140       132      136          128


Depending on the color space, image pixels of a color component may have
zero or nonzero average values. For example, in the RGB color space, all color
components have a mean value of 128 (assuming 8-bit pixels). However, in
the YCbCr color space, the Y component has an average value of 128, but
the chroma components have an average value of zero. In order to provide
for uniform processing, most standard DCT coders require that image pixels
are preprocessed so that their expected mean value is zero. The subtracted (or
added) bias is then added (or subtracted) back by the decoder after the inverse
DCT After subtracting 128 from each element of X, the 8 x 8 D크 output
block as computed by (3.19) is given by

                                                            0
                                                                                l
                                                                                d         l           b
                                                                                                      n
                               49 -3                             -10
                                                            U
                                                            9
                    214                                                     H                     m




                                                                                      <U 尸 b =
                                                                                         b n U



                                                                                      l
                                                                                                      b
                                                                                                      n
                                                                            n
                                                                   U
                                                                   =
                                                            U
                                                            Q
                              -25 11
                                                            l
                                                            m               <
                                                                            U
                     34                                                     H                     H




                                                                                                  l




                                          8 d1 1l 8 QU 0
                                                             V
                                                             O     U
                                                                   Q            J
                                                                                n                     0
                                4
                                                                                                                  H
                                                                            m


                                                                            0
                                                                            l                         O
                                                                                                      n
                               -
                     -6
                                                             1
                                                             4
                      8       -10                                -15
             y ==                   U
                                    =                        乙
                                                             O                  V
                                                                                O                     4111
                    -12                                          -15                                              m   H
                                                                                      H           H




                          U
                          =         U
                                    O                        U
                                                             Q         1
                                                                       d    小
                                                                                r
                                                                                H                     乙
                                                                                                      n               H




                          乙
                          n         乙
                                    n                        l
                                                             1         l
                                                                       1        D
                                                                                n                 H
                                                                                                      1
                                                                                                      4           H




                          i
                          1         l
                                    m                        乙
                                                             n         d
                                                                       n        乙
                                                                                n                     乙
                                                                                                      n
                                                                            H                     1




At this point, no compression has been achieved. Note that, compared to
X, the DCT-transformed data Y has large amplitudes clustered close to y00,
commonly referred to as the DC coefficient. In general, for a low-activity
block, most of the high-amplitude data will be in the low-order coefficients,
as is the case in this example.
72                                                                                                                              CHAPTER 3




It is the process of quantization which leads to compression in DCT domain
coding. The process of quantization of Yk! is expressed as
                            , / ,,.,\    1 Vi., 士 四奇니 1 . ,                 .                                                        .    .
             :k/     'Otirld, (1 -)
             Zk1 = 17'Oti7id     므＝ ] = I1 .7 '"                k, i,l== 0. .l1, ..., - .
                                                   L TI .J I1 . /r                                                                   (3.28)
                               \qklj     L       qki       J

where q,, denotes the kl-th element of an 8 x 8 quantization matrix Q. ([xj
denotes the largest integer smaller or equal to .r.) In order to ensure that the
same type of clipping is performed for either positive or negative valued Yki,
in (3.28), if yki 2 0, then the two terms in the nominator are added; otherwise
they are subtracted. For this example, if the 8 x 8 quantization matrix is given
by
                         16     11                10        16  24  40                                  51 61
                         12     12                14        19  26  58                                  60 55
                         14     13                16        24  40  57                                  69  56
                         14     17                22        29 51 87                                    80 62
              Q          18     22                37        56  68 109                                 103  77
                                                                                                                                1    (3.29)

                         24     35                55        64 81 104                                  113  92
                         49     64                78        87 103 121                                 120 101
                         72     92                95        98 112 100                                 103  99
then the quantized DCT output is given by

                                                                  =上1
                                                      1
                                                      4b9                                   0
                                                                  l
                                                                                                0 0 0 0 0 0




                                                                                                              0 0 0 0 0 0 0 0
                                        nd Q나 0 41上
                                   ]l

                                                            上
                                                            11    0
                                                                                              U
                                                                                              戶
                                                              ]
                                                              0
                                                                                                                                              H




                                                                              0 0 0 0 0 0
                                                      1
                                                      ]
                                                                                              0 0 0 0 0 0 0



                                                                  0 0 0 0 0
                                                                                                                                              H




                      z ＝二


                                                        0 0 0 0
                                  l
                                  =

                                                                                            U
                                                                                            n

                                        n니 0 0                                              0 0 0 0 0 0 0 0



The process of quantization has resulted in the zeroing out of many of the DCT
coefficients Yki. The specific design of Q depends on psychovisual characteris-
tics and compression-ratio considerations. All compression standards provide
default values for Q. In a later chapter, we describe some of the techniques
used to develop quantization tables.

At this point, the quantized DCT domain representation, Z, has resulted in
significant savings, since only 11 values are needed to represent Z compared
Fund口刃ie7玎als o／乙7ssy／刃rage（勿mpression                                                                        73




to the 64 values needed to represent X; this represents a compression ratio
of 5.8. The matrix Z can be efficiently represented using a combination of a
mn-length coding scheme and a Huffman coding scheme; we will describe the
specifics of such an entropy coder in a later chapter.

Decompression begins with the entropy decoding of the coded bitstream. Since
entropy coding is a lossless compression scheme, the dec어ier should be able
to reconstruct an exact version of Z. Inverse quantization on Z is simply
performed as
                                Zk, == zklqkl .                       (3.30)

In this example, the inverse quantizer output matrix Z is

                                                 l
                                                lO
                                               nV




                                                            00000000   00000000   00000000   00000000
                                               b
                                          0
                                          ll
                           208  44
                                         4
                                         1 n
                                           b
                            36 -24




                                                   000000
                             0   0




                                           00000
                            14 -17
                 2   =
                           -18   0


                             000
                                 0
                                 0
                                 0


After the inverse quantization, the decoder computes an 8 x 8 IDCT of Z
using (3.22). The 8 x 8 IDCT output is given by


                     171   160     149   149       158           166               166                  162
                     174   164     155   154       160           164               161                  156
                     171   164     157   156       158           158               151                  145
                     161   157     154   154       155           151               144                  137
            x=
                     156   155     155   156       156           152               145                  140
                     159   160     160   160       157           153               148                  145
                     161   161     160   156       150           144               141                  139
                     159   158     155   148       139           132               129                  128


Observe that X 7드 X and that the only cause of this coding error is the
quantization of the DCT coefficients. However, in this example, as evidenced
in Figure 3.6, the coding error is not perceptually significant.
74                                                                          CHAPTER 3




Example 2: To better illustrate the properties of the DCT, we include another
example as depicted in Figure 3.7. Here, we have chosen an 8 乂 8 input block




                                    Compression    ;     Decompression




                  小
                  器
                  4寸
                   娜小
                    小
                                誥＋Cu帥tize              > Inve
                                                         Quar，
                                                             竿,,＋程I
     m 屯111蟹  m




                    小 礪111髓 m
                                                   1



        二11n堪

     i1旒k뇨乞客努
     1
     必川兀掌a1:
        Original                                                         Decompressed




                                              Coding Error


     Fig.ure 3.7                DCT coding example for a block in a high-activity
     region.


from a high-activity region. Zooming into this block, from Figure 3.7, we note
that the block has two edge regions. The pixel values for this block are given
by
Fundamentals of L.ossv Image Compression                                                                 75




                    197    184       144    103    130 133  70  51 1
                    200    158       111    141    179 151  70  73
                    172    110       111    179    192 135  95 144
                    118     77       139    193    156 102 128 193
                     73     75       151    163
                                                                     1
                                                   110  84 154 197
            x=
                     54     84       142    122     73  90 160 162
                     50     95       130     71     52 101 146 117
                     68    115       106     55     63 116 118  72


and the corresponding DCT output is

                                                                                 ll
                                                                                  尸b
                 -60       -5      -14     -38         17      15                        7
                                                                                  n
                                                                                  J乙
                  127     139      -40      103      102      -41                      -13
                                                                                  ]1
                 -76      123        22     110    -105       -46                       -8
                                                                                 H
                                     QV
                                                                                  1l
                 -20       -5        29
                                     n乙
                                           -53      -54        18                       11
        Y


                                                                    d1 8 0 nJ乙
                                      =U                                          n乙
                   -4       4         5    -25        -6                                 5
                                      OV                 <U                       H/
                  -3     -10          9    -19                                           6   小




                            0 44
                    QU                ]1      1l         41                       4l
                                                                                         2       H




                                                       4
                                                                                        寸
                    ml                <U      41                                  1
                                                                                  l
                                                                                         4           H
                                                                                                     H
                                                                                                     H




Note that, compared with the Y output of the previous example, the dominant
DCT values are not clustered close to yoo. This is usually the case when the
spatial-domain block is a high-activity block. For this example, we chose a
quantization matrix that yields the same compression ratio as the one obtained
in the previous example. Repeating the same calculations as in the previous
example, the IDCT output is


                    198 182         153     136    145        145            95         32
                    182 159         146     153    152        129            98         81
                    153 124         135     174    159        105           104        150
                    120  95         125     180    153         86           112        203
            x
                     88  84         120     159    130         81           121        211
                     62  93         120     114     92         92           131        173
                     45 112         123      64     52        110           139        114
                     37 127         126      31     27        123           143         72


A comparison of the coding error images in Figure 3.6 and Figure 3.7 indicates
that, for the same compression ratio, we have incurred more error for the
76                                                                           CHAPTER 3




high-activity block. However, from a perceptual viewpoint, the viewer may
find the decompressed image block in Figure 3.7 to be the same as the original
image block; this is because the eye is less sensitive to quantization noise on
edges.

Another way to visualize the DCT coding process for our two examples
is to look at which of the DCT kernels of Figure 3.4 are retained after
the quantization process. Figure 3.8a shows the main DCT kernels for the
low-activity block, and Figure 3.8b shows the main DCT kernels for the
high-activity block. Note that, for the high-activity block of Example 2, some




                                          1 m m呻
                                                                薑 玉
                                                                1 交1
                                                                1 ！
                                                                       n
                                                                       1 낱
                                                                         m
                                                   多
                                                       恥

                                                    葫
                                                   m 斗




           a) Low activity block                           b) H勾h acti너勺 t키ock


     Figure 3.8      DCT kernels retained for reconstruction of 8 x 8
     비ock.


of the high-frequency information-bearing kernels need to be retained for good
image fidelity.

Unlike DPCM, in DCT-based coding, higher lossy compression results in
blurred decompressed images. This is because an increase in compression
ratio implies using larger values for the quantization coefficients qij. Since
most of the larger values are often concentrated in the high frequencies, these
frequencies are zeroed out and cause loss of detail in the reconstructed image.
Fundamentals of Lossy Image Compression                                          77




In these examples, we have illustrated the basic steps in a DCT-based coding
scheme. From a computational point of view, quantization and inverse
quantization require 64 multiplications each. On the other hand, brute-force
evaluation of an 8 x 8 DCT or IDCT requires close to 4,096 multiply-
accumulate operations. In the next section, we describe several algorithms for
the fast computation of the 8 x 8 DCT or IDCT.




3.5 FAST ALGORITHMS FOR THE DCT
From (3.19), computing each DCT coefficient in an 8 x 8 DCT requires 64
multiplications and 64 additions. Thus, 4,096 multiply-accumulate operations
are needed for each 8 x 8 block. This number can easily be reduced if we
use a row-column approach. From (3.23), an eight-point l-D DCT requires 64
multiplications and 64 additions. Using the row-column decomposition, we
need to compute 16 1-D DCTs (eight for the rows and eight for the columns)
向r a total of 1,0겨 m毗ip竝孔cumula妃 叩erations. The separab小typr야)erty
has reduced the computational complexity by a factor of four; however, these
numbers are still quite prohibitive and need to be reduced if we require
real-time completion of the DCT process for a whole image. In recent years,
several fast algorithms for the computation of the DCT have been developed.



3.5.1    Comparison of Fast 2-D DCT Algorithms

Most of the fast algorithms for the DCT exploit the properties of the transfor-
mation matrix T. Essentially, it has been shown that the matrix T of either
(3.21) or (3.26) can be factorized so that T = TLT2...Tk, where each of the
matrices T1, 7'2, ..., Tk is sparse. Sparseness implies that most of the elements of
the matrix are zero. Thus, the transform TX can be expressed as T1T2...TkX.
If the calculations are performed in a sequential manner; that is, if we compute
sk = TkX first and then use the result to perform the next matrix product,
Sk11 = Tk_lsk, then it can be shown that there is an overall reduction of the
number of operations needed to perform the 2-D DCT or IDCT. We avoid the
details of this factorization; instead, we refer the reader to various references
cited in the last section of this chapter. The computational complexity of some
of the most commonly used fast DCT algorithms is shown in Table 3.1. The
first three methods provide a fast algorithm for an eight-point 1-D DCT from
78                                                                CHAPTER 3




          DCT or IDCT Method          Multiplications     Additions
                                      iD       2-D        1-D 2-D
                 卜DChen                16      256         26   416
                  1-D Lee              12      192         29   464
          1 -D Loeffler, L땅enberg      11      176         29   464
             2-D Kamangar, Rao                 128              430
                2-D Cho, Lee                    96              466

      Table 3.1 Computational complexity of various fast DCT algo-
      rithms.



which the 2-D DCT can be computed using the separability property of the
DCT. The last two, methods were developed exclusively for a 2-D DCT. All
these methods offer a significant reduction in complexity compared with the
naive matrix multiplication approach of the previous section. At this stage, the
reader might conclude that a true 2-D method, such as the Cho approach, yields
lower complexity than the separable extensions of the 1-D DCT. However,
from an implementation viewpoint, many of the true 2-D DCT methods have
several disadvantages:


 I. In a software implementation, storage for up to 128 elements is needed.
    In a computer system that is register limited, such storage is not always
    feasible.

 2. Data addressing is highly irregular. In a software or hardware implementa-
    tion, this irregularity leads to additional overhead for address calculations,
    which is not included in the original number of multiplications and
    additions.


Most practical software and hardware implementations of DCT-based coders
use the row-column extension of the 1-D DCT. In some DCT-based coding
schemes, a further reduction in complexity for the l-D DCT approach can be
obtained, as we discuss in the next section.
Fundamentals of Lossy Image Compression                                       79




3.5.2   The Fast Scaled DCT

From Figure 3.5, we observe that the output of the DCT computation unit is
always processed by the quantizer. Excluding clipping effects, the quantization
process of (3.28) can be expressed as Zkl = 誥· Let us assume that in the
matrix factorization ofT = T17느 · · . T, the last (in processing order) matrix T1
can be expressed as T1 = HT1, where H is a diagonal matrix. Then it can been
shown that using T1 instead of T1 will yield a scaled version of yki. By suitably
scaling the quantization matrix entries qk/ by the entries of the diagonal matrix
H, one can reproduce the true Yki during the quantization process. Through
this restricted factorization, the resulting T1 is more sparse than T1 and thus
reduces the overall operations count when calculating the scaled version of
Yki.


As an example, consider the following DCT butterfly operations at the last
stage of a DCT algorithm:

                               yt    =    t,b+ t,a,                       (3.31)
                               !/J   =    tb - t3a,                       (3.32)

where a and b are constants. The above operations require four multiplications
and two additions. If qj and q3 denote the quantization coefficients for y. and
yj, then after quantization zi = 弓1 and z』 = 半. Let c = 웃 . Then the above
operations can be rewritten as

                              !n     = a(t3c + t2).                       (3.33)
                              yj     = a(t1c- t3).                        (3.34)

At first glance, there is no reduction on the number of operations; however,
since y1 and y3 will be quantized, the two multiplications by a can be absorbed
by the quantizer. Let

                                q: =       tjc+ ti,                       (3.35)
                                yJ    =   乙C 中 tj,                        位36)

be the output of the scaled DCT butterfly. The above operations require only
two multiplications and two additions. If cji = ,血 and 4j = 誓 are the scaled
quant油tion coe砥蜘ts, then z戶 繫 = 崇

If we assume that the elements of the quantization matrix do not change during
the coding process, then the scaling of the quantization matrix has a one-time
80                                                              CHAPTER 3




cost of 64 multiplications, and thus its contribution to the overall operations
count is minimal. In Table 3.2, we show the computation complexity of the
scaled DCT approach.


           DCT or IDCT Method        八'IultiF小cations   Additions
                                     1-D       2-D      1-D 2-D
                l-D Winograd           5        80       29   464
                   1-DLee             11       176       29   464
             2-D Kamangar, Rao                  92            430
             2-D Feig, Winograd                 54            462

        Table 3.2   Computational complexity of scaled DCT algorithms.



The scaled DCT method of Feig and Winograd is the most efficient scheme.
The main disadvantage of the scaled DCT method is that it is efficient
only when the quantization matrix is fixed, which is the case for the still-
image compression standard; however, in the video compression standards
the quantization matrix is typically varying at a rate of nearly 600 times per
second.



3.5.3    DCT on a Multiply-Accumulate-based Architecture

In our discussion of fast DCT methods, we have represented the computational
complexity in terms of the number of multiplications and additions. If
in the underlying computation unit the basic operation is a single-cycle
multiply-accumulate operation, expressed as a = bc+d, then the computational
complexity of a fast DCT can be further reduced. We illustrate the basic ideas
using the DCT computational flowgraph of Figure 3.9.

The graph shown here is referred to as a flowgraph for the DCT, and each stage
shows the operations required for the transformation of the input data with
the corresponding T, matrix. Note that, in the flowgraph, cj = cos(끓) and
sj = sin(끓). If we examine this flowgraph, we note that several calculations
can be recast in the multiply-accumulate form. These are shown in Figure
3.10.
                                                                                       81
Fund口ment口Is of Lossy／刃iage Co刃ipression




                                                                s,     10.
                                                                             5 yjO]

                                                                                 4)
                                                                西5y]
                                                                 0.5           叭2]

                                                                   0.5         y[6j

                                                                       0.5     Yll]

                                                                       0.5     yj5]

                                                                       0.5      Yl31

                                                                       0.5     叭7]




        터owgraph n아帥ons

                                             b
                                                    ab


       a7 a+b a11\,-, a
        b-/             b- -- = 尸 入a- b



          Figure 3.9    Flowgraph for the eight-point 1-D Chen DCT.



                                                         a constant (c4) followed
 For example, in Figure 3.lOa, a multiplication by
                                                                 te operations, for a
 by two additions can be recast as two multiply-accumula
                                                    if t2 = 를, then a calculation
 savings of one operation. In a similar manner,
                                                                in Figure 3.lOb, can
 requiring four multiplications and two additions, as shown
                                                           te operations. Since the
 be remapped into only two scaled multiply-accumula
                                                     DCT calculations, the notion
 postmultiply by c2 is done in the last stage of the
                                                              be used to eliminate
 of the scaled DCT, which was discussed earlier, can
                                                          appropriate quantization
  the postmultiply by c2. We can simply scale the
                                                         ultiply . These flowgraph
 matrix entry qki by c2 to account for this postm
                                                                  8 x 8 Chen-based
  modifications lead to a row-column approach for a 2-D
                                                               tions. A comparison
  DCT that requires only 416 multiply-accumulate opera
                                                               3.2 indicates that the
  with the other transforms shown in Table 3.1 and Table
                                                     e.
   multiply-accumulate approach is the best schem
                                                            methods that we have
  A similar exercise can be conducted for all the DCT
                                                                   umulate approach
  listed in Tables 3.1 and 3.2, and in all cases the multiply-acc
                                                              , the operations in the
  yields the smallest number of operations. For the IDCT
  82
                                                                                    CHAPTER 3




                 p = b'c4, e = p+a, I = a-p                     e = bc4+a, I = -b'c4+a
                 1 multiply, 2 additions
                                                 (a)
                                                        2 multiply-accumulate operations

         a
                                                                                     2 e



                           c2                                                       c2 f

             p1 = a'c2, p2 = a 's2, p3 = b'c2,               e = c2[a+b't2J, f = c2[a't2-bj
             p4 = b's2, e= p4+pl, f= p2-p3
                4 multiplies, 2 additions        (b) 2 scaled multiply-accumulate operations


        Figure 3.10          Flowgraph remapping for multiply-accumulate op-
        erations.



flowgraph of Figure 3.9 are simply reversed; that is, operations
                                                                 are performed
from right to left. In this case, the scaling operations are
                                                             combined with the
operations in the inverse quantizer.

This approach lends itself to very efficient DCT implementa
                                                                  tions on con-
ventional digital signal processors, since such architecture
                                                             s include a special
multiply-accumulate unit. Additional implementations for
                                                               the DCT are de-
scribed in a later chapter.



3.5.4    Multiplication-Free DCTs

 A careful examination of the flowgraphs associated with
                                                             the fast algorithms
for the DCT or IDCT indicates that the multiplicatio
                                                     ns are of the type y = c乙
where c is a constant and i is image dependent. The c
                                                         are fractional-valued
constants, and in an integer implementation of the DCT these
                                                                 constants have
to be appropriately scaled. Recently, several approximations to the
                                                                      DCT basis
functions have been developed. The objective of these appro
                                                              ximations is to use
very small integer-valued constants and to replace multip
                                                           lications by simple
                                                                                       83
Fundamentals of Lossy Image Compression




                                                         lication-free DCT and
shift and add operations. These are the so-called multip
                                                   mentation is desirable for
IDCT implementations. Multiplication-free imple
                                                         lier.
low-cost processors that do not have a dedicated multip

                                                   n of a set of basis functions
We give a brief overview regarding the constructio
                                                   implemented without any
that approximate the 8 x 8 IDCT and can be
                                                          the approximate I-D
multiplications. A 2-D IDCT can be implemented using
                                                            approach. The 1-D
IDCT transformation matrix using the usual row-column
DCT computation is of the form

                                 C（서                   ( (2i+ 1)   kir
                                                                                  (3.37)
                          Yk =                :7:mO5
                                  2    乙／                   16
                                       l= 0




             s/ (2,+.1.)kn as the true DCT basis functi。     r i, k
                                                        ns. F。                = 0. 1. ....
 We refer t。c。
               \     ")   I                       has values
 7, the corresponding 8 x 8 matrix, denoted as Tc,

                    1.000              1.000       1.000      1.000   1.000   1.000
    1.000    1.000
                    0.556              0.195      -0.195     -0.55 6 -0.83 1 -0.98 1
    0.981    0.831
                                      -0.924      -0.924     -0.383   0.383   0.924
    0.924    0.383 -0.383
            -0.195 -0.981             -0.556       0.556      0.981   0.195 -0.831
    0.831
                                       0.707       0.707     -0.707 -0.707    0.707
    0.707   -0.707 -0.707
            -0.981  0.195              0.831      -0.831     -0.195   0.981 -0.556
    0.556
                  4 0.924             -0.383      -0.383       0.924 小0.924   0.383
    0.383   -0.92
            -0.556  0.831             -0.981        0.981    -0.831    0.556 -0.195
    0.195

                                                     ct of a diagonal matrix
 Our objective is to express this matrix as a produ
                                                      as T7. As observed in
 and a matrix with integer weights, which we denote
                                                     be incorporated into the
 the section on scaled DCT, the diagonal matrix can
                                                     now be performed using
 quantization matrix. Thus, the DCT calculations can
 the integer-valued matrix TO.

                                                                         :
 For the design of Tc, we impose the following constraints

                                                           identical to that of
   1. The row elements of T must have sign alternations
      Tc.
                                                           all elements of the
   2. If we examine Tc, we find that within a scale factor
                                                                 feature in Tc.
      first row and fifth row are unity. We will preserve this
    84                                                                                                                                 CHAPTER 3




          Furthermore, by a suitable choice of a diagonal matrix, Tc has only seven
          unique values. We will preserve this feature in T.

     3. If we examine values in, say, the second row of Tc, we see an ordered
        data arrangement. T will retain a similar ordering.

    4. DCT is an orthogonal transform. This feature must be preserved in T as
       well.


Based on these constraints, Tc can be expressed in terms of seven constants
a, b, c. d. e, f, and g as




                                                                                                                  9 m e 寸 9 叱 /m
                            9 n e



                                                9 Cr
                                                                             9



                                     0口 工
                                                            9 d


                                        U r
                                                                                          0U


                                                                                                       b r
                                                                                                         J



                                                   / 0 9d
                                          J d
                                                                                                    0U 1
                                                                         d
                                                                         1
                                                                                          r r
                                                                                            1
                                                                                            J
                                                                                                    H
                                                                                                    中
                                                                                                    1




                                                                         e C 9내 r
                                                            吐

                    九      U
                           h
                           1
                                                                                                    e         1
                                                                                                              中




                                                                                                a
                                                                                                1




                                                            크 9 LU r
                                                                                          n




                                                                   7 n          1
                                                                                J 0
                                                                                                              H           H




                            9 Cr
                                                                                                    9 0 e C
                                                                                      d
                                                                                      0
                                     0口 n


                               J d
                                                                                                              H           H        H




                                                                                          1d
                                                                                                                          H        H




                                                eb
                                     e                                                    e                              m         1      e
                                                                                                                                          H




                                     C                                                b
                                                                                      =
                                                                                                                                   卜      H




Without any loss of generality, we require a 三 b 2 c 2 d. Furthermore, we
set g = 1 so as to mimic the first row of T7. To preserve orthogonality, we
require ab = ac + bd + cd. The constraints above can be used in a computer
search procedure to find small integers a, b. ..., f; however, this will yield many
feasible sets. In order to find a good choice among these candidate sets, we
will choose the set or sets that have a high decorrelation efficiency. The
decorrelation efficiency is calculated as follows:


1        Let Y = TcX be the DCT of the 1-D vectorX.

1        We assume that the 1 -D source X is correlated with correlation coefficient
         p and that the corresponding covariance function is the 8 x 8 matrix Cov工
         = p1i_ j1.
         We compute the covariance matrix for Y as Cov, = T7Cov工(Tc)t.

· We蜘毗decorr이ation e耐m8
                     ncyas ' diagaL싸，:，‘『'二쓺딴"·
                                                                              85
Fundamentals of Lossy Image Compression




                                                               relation efficiency
We seek the values a, b, ..., f for which the resulting decor
                                                      c = 6, d = 2, e = 3, and f
approaches one. One set of values is a = 10, b = 9,
                                                                   integer-valued
= 1. For this set, 1'c can be factorized into a product of sparse
                                                              would require 576
matrices, and the corresponding 8 x 8 DCT or IDCT
                                                             to published results,
additions and 192 arithmetic shift operations. According
                                                            es far less hardware
a hardware implementation of the above scheme requir
                                                             antage of the above
than conventional implementations. The primary disadv
                                                                approximation to
scheme is that the coding error is increased, since tc is an
the true DCT basis.



                                   THE
3.6 RATE-DISTORTION PERFORMANCE OF
    DCT
                                                         of DCT in an image
 In the previous sections, we have described the usage
                                                         nt approaches for a
 compression sys把m. Several computationally efficie
                                                   sed.  In an earlier section
 low complexity implementation were also discus
                                                       function for a typical,
 in this chapter, we also provided the rate-distortion
                                                      g scheme approach the
 highly correlated image. Does a DCT-based codin
 rate-distortion function of the source?
                                                           coding system, for
 If we neglect the quantization process in a DCT-based
                                                              le lower than the
 the same SNR, the resulting bit rate is 2.37 bits per samp
                                                        in Figur  e 3.1. In low
 corresponding rate for the uncorrelated source shown
                                                            less than 0.75, the
 SNR regions or for a source with correlation coefficient
                                                                a rate-distortion
 rate improvement will be around I bit per sample. From
                                                                bits per sample
  viewpoint, at very low distortions, a DPCM system is 0.4
  worse than the DCT system.



  3.7 TO PROBE FURTHER
                                                              on. In [18], the
  In this chapter, we introduced the concept of rate-distorti
                                                              d sources and for
  rate-distortion function has been developed for uncorrelate
                                                              istortion function
  sources with correlation along one dimension. The rate-d
                                                     on is descr  ibed in [136].
   for images based on a separable covariance functi
                                                                images, and the
  The isotropic model is considered to be a better choice for
  86
                                                                     CHAPTER 3




  development of the rate distortion function for the
                                                      isotropic model is given in
  [144]. Much of the work reported in this chapter on
                                                      the rate-distortion function
  for 2-D images is based on the developments reported
                                                         in [1871,[60], and [281.

  Over the years, many lossy compression methods have
                                                          been developed for
  still-images. Here, we restricted our discussion to DPCM
                                                            , a sample-based
 coding scheme, and to a DCT-based block coding schem
                                                           e. Motivation for
  using block-based coding can be found in the source-cod
                                                          ing theorem, which
 suggests that block-based coding can approach the rate-distort
                                                                ion bound; a
 recent development of this theorem is in [100]. All the
                                                            image and video
 compression standards discussed in this book employ both
                                                            DPCM and DCT
 coding methods. A detailed discussion of the DPCM codin
                                                            g scheme can be
 found in [93].

 The basis of many block-coding schemes is the transformati
                                                            on of images from
 a spatial domain to the frequency domain. Many transformation metho
                                                                      ds exist
 and are extensively discussed in [44]. The DCT has received
                                                               close attention
 among the transformation methods, due to its use in all the
                                                                  current and
emerging standards in image and video compression. A detail
                                                                ed discussion
on the DCT can be obtained from [166]. Among the fast
                                                             DCT algorithms
we referred to in this chapter, Chen's DCT algorithm is
                                                         described in [166],
Lee's DCI can be found in [Ill], Winograd's DCT can be
                                                           found in [10], the
2-D Kamangar and Rao DCT is described in [971, and the
                                                            2-D Cho DCT is
described in [34]. The development of fast DCT metho
                                                     ds using the concept of
a scaled DCT is provided in [46].

The theory of DCT implementations on a multiply-acc
                                                            umulate architecture
 was developed in [122]. DCT coding systems might be used in
                                                                 the future in low
power devices and in systems that use fairly simple proces
                                                            sors. Multiplication-
free DCT implementations would be quite useful in such
                                                             cases, and one such
development can be found in [5]. The development of fast
                                                               DCT methods for
software as well as hardware implementations is curren
                                                           tly being researched
extensively. In our discussion on the rate-distortion functi
                                                             on for DCT coding,
we ignored quantization effects. A detailed analysis that
                                                              takes into account
the quantization effects as well as the transmission link
                                                          imperfections can be
found in [137]. A more detailed discussion on the hardw
                                                            are implementation
of the DCI is presented in a later chapter.
                                                                       4
             FUNDAMENTALS OF LOSSY
                 VIDEO COMPRESSION




4.1 INTRODUCTION
In the previous chapter, we introduced some of the basic concepts in the
theory of lossy compression of still-images. These concepts can be readily
applied to the compression of image sequences (such as video) as well, by
simply treating each image in the sequence as a still-image. This approach is
inherently simple; however, it does not provide significant compression. For
instance, consider an uncompressed image sequence at a data rate of 166 Mbits
per second. Using a DCT-based coding system on an image-by-image basis,
 for good image fidelity, one can achieve close to 12:1 data compression. Thus,
 the compressed bit rate is close to 14 Mbits per second, which is too high for
 most practical uses. For instance, the bandwidth for digital TV broadcasting
 is close to 4 to 6 Mbits per second. In this case, we need a compression
 ratio around 41:1. In another example, the typical output rate of a CD-ROM
 drive is close to 1.5 Mbits per second. In this case, we need a compression
 ratio around 110:1. Hence, in practical applications with image sequences we
 require at least four times better compression ratios than those we can achieve
  with coders for still-images.

Quadrupling the compression ratio of a still-image coder is non-trivial. In
this chapter, we introduce some of the basic concepts for the compression of
image sequences. These are essentially extensions of the DCT-based coding
techniques employed in still-image coding and form the basis of the video
coding standards that will be described in the ensuing chapters.
 88                                                                 CHAPTER 4




 4.2     VIDEO CODING BASICS

 4.2.1 Image Sequence Model

In the still-image case, we observed that image data tend to have a high degree
of spatial redundancy. Consider now the problem of capturing the movements
of a 3-D object through time (Figure 4.1). In the first image, we capture
a spatial projection of the object, say, in region A. Since this projection is
comprised of pixels from the object, we expect cor이ation within the image. If
the object is moving, it will yield a spatial projection in the next image as well,
say in region X. Thus, we would expect a high degree of temporal redundancy
between neighbor images as well; that is, there is a strong correlation between
pixels in region A in one image and pixels in region X in the next image. The




                                               0   0 0




                                 Time


          Figure 4.1 Temporal correlation in an image sequence.


goal of video compression algorithms is to exploit both the spatial and the
temporal redundancy within an image sequence for optimum compression.

In the last chapter, we described how the 2-D DCT can be used to exploit the
spatial redundancy within an image. In order to exploit both the spatial and the
temporal redundancy, one might suggest using a 3-D DCT instead of the 2-D
DCT. This approach has been shown to be quite effective from a compression
viewpoint; however, the excessive complexity of a 3-D DCT renders this
approach impractical. Instead, most video coders use a two-stage process to
achieve good compression. The first stage uses a method that exploits the
temporal redundancy between frames. The output of this stage is followed by
                                                                          89
Fundamnentals of Lossy Video Compression




                                                 within the frame. The basic
a coding method that exploits spatial redundancy
two-stage process is illustrated in Figure 4.2.




                 frame(t-1)                                frarne(t)




      Stage 1       Processing for reducing temporal redundancy


                    Frame difference      17
      Stage 2
                                               17
                        Processing for reductng spatial redundancy



                 Figure 4.2      Two-stage video coding process.




  4.2.2   Reducing Temporal Redundancy
                                                                   ing temporal
  Intuitively, one might expect that the ideal processor for reduc
                                                            to frame. This is
  redundancy is one that tracks every pixel from frame
 90                                                              CHAPTER 4




 computationally intensive, and such methods do not provide reliable tracking
 due to the presence of noise in the frames. Instead of tracking individual
 pixels from frame to frame, video coding standards only allow tracking
 information for 16 x 16 pixel regions, commonly referred to as macroblocks.
 The macroblock dimension of 16 x 16 is chosen because it provides a good
 compromise between providing efficient temporal redundancy reduction and
 requiring moderate computational requirements.

Let the two contiguous frames in Figure 4.2 be denoted as frame(t - 1) and
frarne(t). In the first stage, we segment frame(t) into nonoverlapping 16 x
16 pixel regions (macroblocks), and for each 16 x 16 block we determine a
corresponding 16 x 16 pixel region in frarne(t - 1). (For the time being, we
ignore how one can find such a region).

Using the corresponding 16 x 16 pixel region from fraine(t 中 1), the temporal
redundancy reduction processor generates a representation for frarne(t) that
contains only the changes between the two frames. If the two frames have a
high degree of temporal redundancy, then the difference frame would have a
large number of pixels that have values near zero. For example, in Figure 4.2,
there is a high degree of temporal redundancy, as evidenced by the similarity
of features in both frames. Thus, the output image of stage I has lower energy
than the original frame and is more amenable to compression.

On the other hand, if frame(t) were completely different than frame(t - 1),
then the temporal redundancy reduction processor may fail to find correspond-
ing regions between the two frames. In this case, one would not expect any
benefit with respect to compression from using the process in stage 1. In video
compression terminology, a compression method that employs only temporal
redundancy reduction is referred to as an inre,frame coder.



4.2.3   Reducing Spatial Redundancy

The output of stage I is a difference frame in which the pixels are spatially
correlated. Thus, one can use a processor that can exploit this spatial
redundancy and thereby yield a compressed representation for I rame(t). This
is the process performed in stage 2 of Figure 4.2. Video coding standards
use a DCT coding method for reducing spatial redundancy. This DCT coding
technique is essentially the same as the one described in the previous chapter.
Fundamentals of Lossy Video Compression                                         91




In video coding terminology, a compression method that employs only spatial
redundancy reduction is referred to as an intraframe coder. The combination
of interframe coding and intraframe coding, as depicted in Figure 4.2, is
referred to as a hybrid (intraframe/interframe) coding method.



4.2.4    Motion Compensation

The process of computing changes among frames by establishing correspon-
dence between frames is referred to as temporal prediction with motion
compensation. We define motion compensation as the process of compen-
sating for the displacement of moving objects from one frame to another. In
practice, motion compensation is preceded by motion estimation, the process
of finding corresponding pixels among frames. If the temporal redundancy
reduction processor employs motion compensation, then we can express its
ou印Ut as
                  e(x, y, t) = I (x, y, t) -I (x -u, y- v, t -1),              (4.1)

where I (x, y, t) are pixel values at spatial location (x, y) in frame(t) and
I (x-u, y- v, t- 1) are corresponding pixel values at spatial location (x- -工, y- v)
in frame(t - 1). The output of the motion estimator, the coordinates (u, v),
defines the relative motion of a block from one frame to another and is
referred to as the motion vector for block at (x, y). Later we describe various
schemes for computing (u, v). I (x 小 u, y - v, t - 1) is referred to as the motion-
compensated prediction of I (x, y, t), and e(x, y, t) is the prediction residual for
 /（工，y, t).

Note that, the notion of temporal prediction and the formation of the
difference signal e(x, y, t) is very similar to the differential coding scheme
(DPCM) described in the previous chapter. The primary difference with
respect to the previous discussion on DPCM is that here we form the temporal
prediction using temporally adjacent samples, which are determined through
the process of motion estimation. Thus, the hybrid coding scheme for video can
be viewed as a DPCM method followed by a DCT coding method. A generic
block diagram of such a hybrid coding scheme is shown in Figure 4.3. Notice
that motion compensation is performed in both the encoder and the decoder,
but motion estimation is needed only in the encoder. A practical coder will
also include buffer memory and additional preprocessing and postprocessing
 functional blocks, which are not shown in this figure. Detailed schematics of
 video coders and decoders will be provided in subsequent chapters.
 92                                                                                    CHAPTER 4




                                              M아幻n               Motion vector (u,v)
                                          Estimat向n



                                              Motion
                                        Compensation

                                                        +
                              e(x,y,t) = I(x,y,t) - I(x-u,y-v,t-1)

                                                        17
                                         0CT Coding

                          Generic Encoder


                                                        V
                                    1
                                          -   Decodin
                                                             g
                                          q e(x,y,I)
               I(x,y,t)                   +             H    I(x-u,y-v,t-1)
                 <
                                          古
                                        Frame
                                                                                 V

                                        Memory

                          Generic Decoder


            Figure 4.3       Generic hybrid video coder and decoder.



Intuitively, one would expect that interframe coding combined with intraframe
coding should yield better compression than either interframe or intraframe
coding alone. In the next section, we attempt to confirm this intuitive
expectation by applying results from rate-distortion theory to different video
coding models. This analysis will provide us in a relative sense the efficacy
of temporal prediction versus direct DCT coding of frames. Even though the
analysis is not very rigorous, readers that are not interested in the mathematical
models of video coding may comfortably skip the next section.
                                                                               93
Fundamentals ofLossy Video Compression




4.3 RATE-DISTORTION FUNCTIONS IN VIDEO
    CODING
                                                             compression scheme
As in the lossy coding of still-images, in a practical lossy
                                                            D and the rate R at
for video, there is a tradeoff between the distortion
                                                                  can be measured
the output of the encoder. The D versus R relationship
                                                           decompressor. Under
for specific implementations of the compressor and
                                                          to derive an information
various assumptions for the video signal, it is possible
                                                                 we refer to as the
theoretic bound for the D versus R relationship, which
                                                              is independent of the
rate-distortion function R(D)for the video source. R(D)
                                                             under  lying stochastic
 particular compression method and depends only on the
                                                           (D) is that for a given
 model for the source. The practical significance of R
                                                          ession rate that can be
 distortion D it provides a bound on the best compr
                                                            R(D)can be used as a
 achieved, regardless of the compression method. Thus,
                                                                     dology.
 measure of the effectiveness of a particular video coding metho

                                                               provide answers to
 Our motivation for determining R(D) is to enable us to
 these questions:

                                                                    g?
     How does intraframe coding compares to interframe codin
                                                            interfame coding
      How do hybrid coding schemes compare to intraframe or
                                                               on warrant its
      alone? Does the added complexity of motion compensati
      use?

                                                        for three video coding
 In particular, we compute the rate-distortion function
                                                          n compensation, (2)
 models, namely, (I) frame differencing with no motio
                                                          motion compensation
 motion compensation with no intraframe coding, and(3)
 followed by intraframe coding.



 4.3.1    Rate-Distortion Function for Frame Differencing

                                                        generic encoder-decoder
  For the purposes of computing R(D), we simplify the
                                                             e 4.4. The motion-
  tandem of Figure 4.3 as shown in the model of Figur
                                                           ced by a single filter
  estimation and motion-compensation blocks are repla
                                                          ed  by the DCT coding
  function h(x, y) and the coding noise n(x, y, t), induc
                                                       elated white noise with
  of e(x, y, t), is modeled as an additive and uncorr
94                                                                 CHAPTER 4




                       小
                                                            D> +

                                                A01
                                 >h (x,y)


             Figure 4.4    Simplified model for interfrarne coding.



constant spectral density D. We further assume that the blocks I (x, y, t)
and I (.r. y. t - 1) are temporally correlated. and we denote by p the temporal
correlation coefficient. This is a simplified model in that a single correlation
coefficient is assumed for the entire frame.

We will also assume that the impulse response of h(x, y) is a single impulse at
J'= u and y = v; that is, we assume that each block I (x, y, t) corresponds to
a shifted (by (11, v)) block in the prior frame. Note that, in this case (u, v) is
not a true motion vector but an arbitrary estimate that remains the same for all
blocks in the frame. We refer to this case asfra,ne differencing without motion
compensation. Note that, there is no added complexity in evaluating R(D) for
nonzero values of n and v, even though in practice by frame differencing we
often imply that u = 0 and v = 0.

For this impulse response, the corresponding frequency response is H(f, f, ) =
ej2i1f』u+ f,,t'). From (3.6), RjD) is computed as the integral of the power
spectral density. From the model in Figure 4.4 and the frequency response
of h(.r. y) we can express the power spectral density of the signal e(x, y, 1) +
n(x. y, t) as

           Sc (fr. fy) = 2(l e PC0S(2:(/1ii + /9iJ)))S/ (/T, /n + Z) .      (4.2)

For S,(f. ft,), the spectral density of a frame, we use the isotropic covariance
model established in (3.1) of the previous chapter. As before, the power
sF思ctr키 density is bandlimited such tha나作 + 考 드 去
The computation of R(D) for this model follows along the same lines as the
computations outlined in (3.7) to (3.10) of the last chapter. D(6) and R(8) can
be expressed in terms of S.(f:..fy) by replacing Sx (f1, fV) with S (ft, f) . Let
R(D)d汀1 denote the rate-distortion function for the case of frame differencing
                                                                                                                                                                    95
Fundameiuals of Lossy Video Compression




                                                     for this                                                                                           function can be
without motion compensation. The integral expression
computed in closed form as
                                                                                                          H
                                                                                                          4D
                                               l 尸n
                                               寸  乙
                          /
                                                                                                                            \
                                                                                  /
                          +                                                                                                                                       (4.3)
                                                                                                                                \
                                               二，log2 ( 뜩 +i ),
                                                        O
                                                                                      /
                                                               나
                                                               O
                                                                                                                                    1
                    R(D)d111 =
                                                                                                                    ］
                                                                             n=
                                                                                          1
                                                                                                                                        1
                                                                                                      \
                                                                                                                                            1
                                                                                                                        上
                                                                                              1
                                                                                                                    / r
                                                                                                                                                1
                                                                                                                      J
                                      )
                                                                                                  \
                                                                                                                                                    /
                                      m                                                                               1
                              2
                                      H
                                          =+
                                               O
                                               乙
                                               n
                                                      OH r/   r11\
                                                                     ］
                                                                         上
                                                                                                          e
                                                                                                          O1
                                                                                                               D乙
                                                                                                                                                                  (4.4)
                                  아
                                               function for an uncorrelated
From the previous chapter, the rate-distortion
source with Gaussian distribution was given by
                                                                                                                            r丁2.
                                                                                                          l                                                       (4.5)
                          R(D)uncorrelated = 흐 1092 弓 "
                                                    frame differencing to be
 Thus, for a video compression scheme based on
                                                    Using (4.3) and (4.5), this
 effective, we require R(D)diff < R(D)unc。rrelated.
                                              the coding noise term D and use
 inequality implies o2, + D <ai. If we ignore
 (4.4), the variance inequality reduces to
                          勿｝(1- pe寸2"凡n그）<d} .                                                                                                                     (4.6)

                                                              玎구 < 닒兀1n2p.
 With son部帥le 毗ebra, this inequality is satisfied 迂而
                                                      is achieved if Vu玎 v2 <
 Let fo = 驃 and p = 0.95, then the inequality
                                                           prediction with frame
 11.38. The implication of this result is that temporal
                                                            displaced by at most
 differencing is effective only if two neighbor frames are
                                                        mon to find displacements
 士2 pixels. In a typical video sequence it is not uncom
                                                            not effective in such
 that are 士7 to 士 15 pixels; thus, frame differencing is
 cases.
                                                          (4.3) for several settings
 In Figure 4.5, we plot the rate-distortion functions of
                                                      the rate-distortion functions
 of K = Vu2 + v2. For comparison we also plot
                                                          source (as defined in the
 for an uncorrelated source (4.5) and a 2-D correlated
                                                             nts greater than eight
 previous chapter). Observe that for frame displaceme
                                                            vement compared with
 pixels, frame differencing offers no compression impro
                                                           as a memoryless source.
  a simplistic compression method that treats the source
                                                               pixel (that is, K = 1),
  Furthermore, even for a displacement that is at most one
                                                             ression ratio compared
  there is only a 25 to 30 percent improvement in the comp
                                                         correlated model (that is,
  with the memoryless case. In all cases, the 2-D
                                                                  better performance
  intraframe coding alone on a frame-by-frame basis) yields
                                                                 temporal prediction
  than frame differencing alone. Thus, one can conclude that
                                                              ression method except
  based on simple frame differencing is not a viable comp
   for regions in a scene that have very little motion.
 96                                                                                               CHAPTER 4




                6.50

               6.00

               5.50

               5.00
                0
                U
                二
                4


             0   0    0
             0        0                  R(D)   .K= 11
            4 U  3 3
                 =


            小m죠Emm\ m亡口낙으m工                                                    R(Dijiff K
                                                                                        ,
                                                                                              =   8
               2.50
                                                                          R(D)diff , K = 1
              2.00

              1.50                                         R       Jiff             0
                                                               (D)diff
                                                                           ,
                                                                               K=
              1.00                                   <｝卞 2-O CorreIated
                                                       (intraframe coding)
              0.50
                                                    Uncorrefated (Gaussian)
              0.00

                              0.00   10.00       20.00            30.00                     40.00
                                                SNR (dB)


        Figure.4.5 Rate-dist.ortion functions for frame differencing,with
        no motion compensation, a uaussian source, ann a z-u correiateo
        source intrarrame cooing).



In the next section, we develop the rate-distortion functions for video coders
that track motion of regions across frames and employ a motion-compensated
prediction to exploit the temporal redundancy.



4.3.2     Rate-Distortion Function for Motion-Compensated Video

Let us assume that regions in block I (x, y. t) have corresponding regions in
block I (x, y, t - 1) at displacement (u, v): that is, (u, v) is the t끄e motion
Fundamentals of Lossy Video Compression                                             97




vector associated with the pixel location (x, y). Motion estimation attempts
to estimate (u, v) and this estimation process will not be error free. The
reason for the estimation error is that in practice I (x, y, t) and I (x, y, t - 1) are
available only on integer-sampled positions for (x, y) even though the change
in position of an object from I rarne(t - 1) to frarne(t) might be less than one
pixel distance. Thus, due to the sampling grid limitations for the frame, the
motion vector accuracy may be limited to 士1 pixel. Methods are known for
reducing the estimation error, but it has been shown by Girod that for typical
video imagery and a frame resolution corresponding to broadcast TV, even
if the motion-estimation error can be reduced below 士0.1 pixels, there is a
negligible decrease in the variance of the prediction error, that is, the variance
of the signal e(x, y, t). Since reduction in prediction-error variance is a good
measure of the compressibility of e(x, y, t), Girod observed that for broadcast
TV it is sufficient to attain a motion-estimation error of 士0.25 pixels.

Procedures for motion estimation will be described in a later section of
this chapter. For now, let us assume a motion-estimation procedure that
yields a motion vector (u, v) with estimation errors denoted by dU and d.
The temporal prediction signal can be expressed as e(x, y, t) = I (x, y, t) -
I (x - u - d, y - v - d, t - 1). Note that, if (u, v) is the true motion vector,
that is, dU = dU = 0, then e(x, y, t) will be zero valued. Referring to Figure
4.4, the estimation error can be easily inco叩orated into this model if we view
h(x, y) as a combination of two filters hi(x, y) and h2(x, y), where hi(x, y) has
the same impulse response as the h(x, y) in the frame differencing case and the
frequency response of h2(x, y) can be written as H2(f, f ',) = eJ2可（/7d,1+/!,d，」）.
Note that, the estimation error vector (d,', d, ) is random. To compute R(D),
we need to determine the power spectral density of e(x, y, t). This requires a
simple modification of (4.2), and the power spectral density is given by

      S (f, fV) = 2(1 - E[pcos(2兀(f1dU + fdO))])Sj(f, f) + D,                    (4.7)

where Sj(f工, fy) is bandlimited as noted earlier. The expectation operator is
needed due to the randomness of (d,',d.). Assume an isotropic displacement
error probability density function for (d,',dU) as


                             』，)＝음.( Y尋亘）,
                          ;（己，                                                   似8)
98                                                                                    CHAPTER 4




where 야 is the variance of the motion-estimation error. The prediction error
variance for e(x, y, t) is computed as the integral of Se(fr, fV) and is given by
                         八J1 r
                                                                     P
                            d
                            =                                                               (4.9)
                                                       n*
                                 .)a
                                 -
                                              (1
                                                       (1+
                                                                     adfO)   2)   ,




where fo is the same as before. From this equation, we claim that temporal
prediction with motion compensation is effective if a, < 야. Applying this
condition to (4.9) leads to the following requirement:

                                                   ＼厚万 -1
                                       r了J <                                               (4.10)
                                         "               亢／0




Thus, for accurate motion-compensation-based temporal prediction, the vani-
ance of the motion-estimation error needs to satisfy the above inequality. This
equation suggests that effective motion compensation requires a high degree of
motion-estimation accuracy relative to spatial variations (fo) and the temporal
correlation coefficient p. For typical values of fo and p, as defined before,
effective motion compensation requires that ad < 4.26. This suggests that
motion estimators with inaccuracies in excess of 士4 pixels will render motion
compensation ineffective.

If the motion-compensated prediction signal e(x, y. t) is coded as if it were an
uncorrelated source (that is, with no additional intraframe coding), then its
rate-distortion function is the same as in (4.5) but with 야 replaced by a2, :
                                                   ]           戶2
                                        l_)        1   I_      (if

                                       11 = 三 i아／2 万 "                                     (4.11)



In Figure 4.6, we plot the rate-distortion function of (4.11) for various
motion-estimation error settings of a,1. For comparison, we also show the
rate-distortion function for a Gaussian uncorrelated source. Observe from this
figure that even for a high motion-estimation error of 士1 pixel, we get a 40
percent improvement in the compression ratio when motion compensation is
employed. We note that reducing the motion-estimation error below 士吉 pixel
does not provide noticeable improvement in the compression ratio. In the
video coding standards for broadcast TV, the motion-estimation error is at
most 士古 pixel. Thus, one can conclude that motion compensation followed by
a simple coding scheme that considers e(x. y. t) as being uncorrelated can yield
a lower rate compared to the case where no motion compensation is used.
Fundam7ientals of Lossy Video Compression                                             99




           3.50


            3.00
                                     Uncorrelated
                  d
                  n   U
                      二   0          (Gaussian)




     百죠Em꼰쁠e으m工
                                        \\\\/          .   寸
                                                               ! 1 pixel

              n
              <
                      0   0                                    t0. 5 pixel

                                                               !0. 25 pixel
                  1
                  d   U
                      二   0
                                                               !: 0.1 pixel
                  1
                  d   0   0


            0.50


             0.00


                              0.00        10.00       20.00        30.00      40.00
                                                    SNR (dB)


            Figure.4.6 .Rate-distortion perfo.rmance for motion-compensated
            preaicuon witn no intrarrame cooing.



Does this interframe-only coding method outperform an intraframe coding
method? In Figure 4.7, we plot the rate-distortion function for the motion-
compensated prediction case (interframe-only coding) and a motion-estimation
error setting of土古 pixel, against the rate-distortion function for 2-D intraframe
coding that was developed in the previous chapter. From this figure, rate-
distortion theory suggests that a video coding method that uses motion-
compensated prediction and does not exploit the spatial redundancies in
e(x, y, t) will not outperform an intraframe-only coding technique.

 In practice, e(x, y, t) is spatially correlated, and hence treating it as such can
 lead to a lower rate. For instance, in the video coding standards, the signal
 e(x, y, t) is further processed by a DCT-based coder. We now define the
 rate-distortion function for the case of spatially correlated e(x, y, t). This
 corresponds to the performance achieved by an ideal compression scheme that
100                                                                                                      CHAPTER 4




                                5.00

                                4.50

                                4.00

                          U
                          Q       =b0

                                                Motion compensation only




              小m中쇼Emm＼ 留즈낙으m工
                                0
                                    0
                                                                                     /
                                                     +1- 0.5 pixel
                                QU


                                U
                                <
                                2   0                                           //
                                                                            /
                                    0
                                                                        /
                                0
                                n
                                <
                                                                                          .

                                                                                     .'




                                                     /
                                  啣                                 /            .




                                                                                Intraframe coding only

                                                   /
                                1.00
                                                                                          (2-O correlated)
                                0.50                            /
                                                            /
                                                       //


                                0.00

                                       000     10.00          20.00                           30.00          40.00
                                                            SNR (dB)


        Figure.4.7 Rate-distortion performance for motion-compensated
        preoiction versus intrairame cooing.



uses motion compensated prediction followed by additional processing of the
prediction residual e(x, y, t).



4.3.3     Rate-아St아如n Function 知rM出on-Corn꺄nsated Video
          Followed by Intraframe Coding

We write (4.7) as

                                 Se(fx, ft,) = 2(1 - po(f工, fV))S1(f工, f,) + D ,                                     (4.12)
Fundamentals of Lossy Video Compression                                    101




where the characteristic function 砂(f1, fr,) is derived from (4.8) as
                                                1
                            砂(f,                                         (4.13)
                                   f,) =((: ,,/;2+ 1)
                                        ((lr。df)2  l)y2

and f = 在而 \Ve den야e 小小S 町）· U蜘 毗basic아pression
for rate, we can express R(D) in integral form as
                       n             ／去 .,      n2(/\' . . \,.           ., , A.
                                                                         딴I. 1什．)
                       R =                                  ,/.,
                                   冗 / ' I l092 ( V = ' 十 1卜｛
                                    J0          \   LI     J

                   a2 (f)    =     2(1- pd(f) )So (f),                   (4.15)

where S0(f) is given by (3.4). Note that, if the motion-estimation method yields
no estimation errors (that is, ad = 0), we modify (4.15) to a2(f) = 2(1中 p)So(f)
and compute R(D) as per the integral in (4.14). Computing a closed-form
expression for R in (4.14) is quite cumbersome; instead, we resort to a
numerical integration procedure to provide the rate R for a specific choice of
D.

In Figure 4.8, we plot this rate-distortion function for various se仄ings of
the motion-estimation error ad. This rate-distortion function yields the rate
that is achievable with a hybrid inte卄rame/intraframe coding method. For
comparison, we plot the rate-distortion function for the interframe-only case
as per (4.11); for this plot, we have set the motion-estimation error to
士- pixel. We note from this figure that exploiting spatial redundancy in
the motion-compensated prediction residual e(x, y, t) can result in nearly 40
percent improvement in the compression ratio for a moderate SNR of 20 dB.

The key question to ask at this point is whether this hybrid interframe and
intraframe coding method can outperform an intraframe-only coding method.
To address this question, in Figure 4.9, we depict a series of rate-distortion
plots. Here, we plot the rate-distortion function for the hybrid coding method
by computing (4.14); this plot is for a motion-estimation error of 吉 pixel. For
comparison, we also show the rate-distortion function for the interframe only
case as developed earlier in this section; this plot is for a motion-estimation
error of { pixel. We also show the rate-distortion function for the 2-D
intraframe-only coding case as developed in the previous chapter. From this
 figure, we observe that exploiting spatial redundancy and temporal redundancy
 lowers the rate by a factor of two compared with the interframe-only case. In
 the literature the factor-of-two improvement has often been cited, but these
 102                                                                   CHAPTER 4




          5.00


          4.50
                                            Motion compensation only
          4.00                                  (+1- 0.25 pixel)

          U
          <
          3     0



        0   0   0
        0       0                  !1 pixel
            U
            <
            2   2
                                    t 0.5 pixel
        口
        n                          !0.25 pixel
       百죠Em띤竺e으m工                  ! 0.1 口xel
                                   !0 pixel

         1.50


         1.00


         0.50


         0.00

                    0.00         10.00             20.00       30.00     40.00
                                                  SNR (dB)


        Figure 4.8         Rate-distortion functions for hybrid video coding.



observations have been based largely on experiments. It is informative to
note that rate-distortion theory is able to predict this gain. Furthermore, at
moderate SNR (say, 25 dB), there is nearly a 30 percent improvement in the
compression ratio for the interframe/intraframe approach compared with the
intraframe-only coding method.
F刃idam라끄als of I刃ssy V油oC아刃／?ressi(刀i                                                            103




                    5.00


                    4.50


                    4.00

                    QU
                         印
                                      Motion compensation only




       8죠Em꼰쁜e으m工
                         m                  (+1- 0.5 pixel)
                    QU


                                                                                    /"
                    n<
                         的


                    2.00

                                                                           //
                    1.50
                                                              '
                                                                  '
                                                                  I"
                                                                       "
                    1.00
                                                              Mot幻n compensat幻n
                                                              and intraframe coding
                    0.50                            '            (+1- 0.5 pixel).


                    0.00

                             0.00   10.00           20.00                   30.00        40.00
                                               SNR (dB)


      Figure 4.9 Rate-distortion functions for hybrid, interframe, and
      intraframe video coders.



4.3.4 Rate-Distortion Functions for Video-A Summary

We summarize all the rate-distortion functions developed in this chapter in
Figure 4.10. This plot indicates the relative performance improvements that
can be obtained through various approaches to video coding, ranging from the
simple case of treating the video source as a memoryless source, to schemes
that exploit spatial correlation and finally to schemes that employ both spatial
 and temporal correlation.
104                                                                                                                CHAPTER 4




                     5.50
                                                                                         Frame differencing only
                     5.00
                                                                                                   \＼뇨         .   “「




                     4.50
                                                 Motion compensation only
                     4    00


                           0
                          二U




       百죠Em쁘竺emHm工
                     Q
                     U


                                     Gaussian uncorrelated                  //

                                                     /
                     口
                     U    00                                          I



                     n<
                           0
                          CU                                                              /
                                                                                              1




                                            /
                                                                                     /
                                                                                /'

                     n
                     <    00                                           //
                                                                            /




                     1.50                                        /
                                                         I   "                                .




                                                    ,/                           .＜卜HH1岫afra毗only
                     1.00
                                                                                                     lnterframe and
                     0.50                                                                            intraframe coding


                     0.00

                               000          10.00                         20.00                    30.00                40.00

                                                                     SNR (dB)


      Figure 4.10                    Rate-distortion functions for various video coding
      schemes.



Caution must be exercised in using the data in these plots, since many
assumptions were used when developing the rate-distortion functions. An
astute reader might observe that at moderate SNR (say, 25 dB), we only
obtain a 4- to 5-fold reduction in the rate compared with the memoryless
coding scheme, while in practice, hybrid coding schemes such as those used
in the video coding standards report much higher rate-reduction factors. Rate-
distortion theory as we have outlined it here does not take into account various
additional techniques used in the video coding standards, including spatial
Fun如刃妃ntals O／乙7ssy Video Compression                                       105




subsampling of frames, skipping of regions in frames, entropy coding, and
switching between intra- and interframe coding.

In an information-theoretic sense, these plots provide the motivation for why
hybrid c어ing methods have been used for video. In the following sections, we
provide details on motion compensation and then describe the hybrid coding
scheme that is the basis for the video coding standards.




4.4 MOTION-COMPENSATED PREDICTION
As noted in the previous section, a hybrid (interframe/intraframe) c어ing
method is quite effective for video compression. A rudimentary video coding
scheme based on this method was shown in Figure 4.3. One of the most
compute-intensive operations in interframe coding is the motion-estimation
process. In this section we will describe in more detail the motion-estimation
process and associated algorithms.

Figure 4.11 illustrates the motion-estimation problem as it is posed in the
video coding standards. Given a reference picture and an N x M macroblock
in a current picture, the objective of motion estimation is to deter血e the
N x M block in the reference picture that better matches (according to a given
criterion) the characteristics of the macroblock in the current picture. As
current picture, we define an image or frame at time t. As reference picture,
we define an image or frame either at past time t - n, for forward motion
estimation, or at future time t + k, for backward motion estimation. In the
more general case of motion estimation, the geometry of the matching block
at the reference picture need not be the same as the geometry of the block in
the current picture, since objects in the real world undergo scale changes as
 well as rotation and warping. However, in the video coding standards, only
 the translatory motion model is assumed for objects in the scene, and thus a
rectangular geometry is sufficient.

The location of the macroblock regions is given usually by the (x, y) coordinates
of their left-top corner. Ideally, we would like to search the whole reference
picture for the best match; however, this is impractical. Instead, we restrict the
search to a [-p, p} search region around the original location of our macroblock
in the current picture. (Many implementations restrict the search range to
 lO6                                                                   CHAPTER 4




     二나尸寸三＝' 긔cture                        Reference Picture



                  N

                        M

            'Aacr야끄ock



                                                         卜p, p] Search region
    ＝甘三' y ce I기cture
         三큰arch region
                                                            V

                                                                 -p
                                                                      U +
                                                    -p
                                                                up
                                                                p

                                                                +

          .'otjon vector (u,v)
                                           (c)
                      Figure 4.11 Motion-estimation process.



卜二 r- :1 Both definitions are equally common.) Let (x + u, y + v) be the
lc:atior. :f the best matching block in the reference picture (Figure 4.llb).
In motic-estimation terminology, the vector from (x, y) to (x + u, y + v) is
rei근rred :0 as the motion vector associated with the macroblock at location
( . :. . C en, the motion vector is expressed in relative coordinates; that is,
we assume that (x, y) is at location (0,0), and thus the motion vector is simply
ex二re;s己＝ as (u, v).

Nc':e tha: our assumption for a common displacement (u, v) for all pixels in
the maCrcblock implies that we are essentially imposing a local smoothness
cor.5trair: on the motion vector field. The local smoothness constraint is only
sausfied for small macroblock sizes. The choice of the dimensions of the
Fun亡7mentals of Lossy Video Compression                                      107




macroblock is the result of tradeoffs among three conflicting requirements.
Specifically,


  1. small values for N and M (from four to eight) are preferable, since the
     smoothness constraint would be easily met at this resolution;

 2. small values for N and M reduce the reliability of the motion vector (u, v),
    since few pixels participate in the matching process; and

 3. fast algorithms for finding motion vectors are more efficient for larger
    values of N and M.


In the video coding standards, N = M = 16.

The coordinate system associated with the motion vector is shown in Figure
4.I1c. For the search region shown in Figure 4.lla, -p < u 5 p and
-p < v <p. For broadcast TV, good performance is obtained at p = 15 for
head-and-shoulders-type video scenes, and at p = 63 for sporting events (high
motion).



4.4.1       The Matching Criterion

Let the pixels of the macroblock in the current frame be denoted as C(x+k, y+l)
and the pixels in the reference picture be denoted as R(x + i + k, y + j + 1). We
define a cost function
                      M- 1 N- i
        .     '   I   t小 1小 .     』          .
 MAE(i, j) = --石 2/ 21 1G(x+ k, y+ 1) -R (x+ i+ k, y+ j+ 1)I, (4.th)
                      k= 0 1=0


where i and j are defined in -p < i < p and -p < j < p. This is referred
to as the mean absolute error (MAE) or mean absolute difference (MAD)
criterion. We define as the best matching block, the block R(x + i, y + j) for
which MAE(i, j) is minimized. Thus, the coordinates (i, j) for which MAE
is minimized define also the motion vector. In (4.16), we use the absolute
value function due to to its computational simplicity. Squaring the difference
(mean squared error criterion) or explicitly computing the correlation between
blocks are other valid choices, but within a typical coding system, the cost
function of (4.16) performs just as well. In video coding terminology, since
108                                                            CHAPTER 4




the match is being performed between rectangular regions, this is referred to
as a block matching criterion, and search techniques to find the (u, v) that
yield the smallest MAE are referred to as block matching algorithms (BMA).
In the next section, we describe several algorithms for block matching motion
estimation.




4.5    ALGORITHMS FOR MOTION ESTIMATION

4.5.1 Full-Search Method

Given (4.16), the simplest method to find the motion vector for each mac-
roblock is to compute MAE(i, j) at each location in the search space. This
is referred to as the full-search algorithm. We estimate the computational
complexity of the full-search (FS) algorithm as follows.

For each motion vector there are (2p + 1)2 search locations. At each search
location (i, j) we compare N x M pixels. Each pixel comparison requires
three operations, namely, a subtraction, an absolute-value calculation, and
one addition. We ignore the cost of accessing the pixels C(x + k, y + 1)
and R(x + i + k, y + j + 1). Thus, the total complexity per macroblock is
(2p + 1)2 x MN x 3 operations. For a picture resolution of I x J and a picture
rate ofF pictures per second, the overall complexity is帑 (2p+ 1)2 x MN x 3
operations per second. Let N = M = 16. For typical values for broadcast TV
(I = 720, J = 480, and F = 30), motion estimation based on the full-search
algorithm requires 29.89 GOPS (Giga operations per second) for p = 15 and
6.99 GOPS 化印 = 7.

Full-search is computationally expensive but guarantees finding the minimum
MAE value. Due to the high computational complexity of full-search, alter-
native search methods are desirable. In the next section, we describe several
heuristic search strategies for motion estimation. These schemes achieve
suboptimum performance at significantly reduced complexity compared to
the full-search method. By suboptimum, we imply that the heuristic search
strategies do not guarantee that we will find the minimum MAE value. The
complexity is significantly reduced either by decreasing the number of search
locations or by computing (4.16) using fewer than M x N pixel differences
per search location. Combinations of these two schemes are also possible.
Fundamentals of Lossy Video Compression                                    109




4.5.2   Two-Dimensional Logarithmic Search

Two-dimensional logarithmic search is very similar to binary search. In
the first step, the [-p,p] search rectangle is divided into two areas: one
inside a [긍, ) (at integer pixel resolution) rectangle and one outside of it.
Furthermore, instead of searching the whole [긍, ] area, we only compute the
MAE function for nine locations: at (0,0) and at the eight major points in the
perimeter of the [긍, ] area. That is, if the distance between these points is
d1, we compute the minimum MAE from the MAE computed at (0,0), (0,d1),
 (0，尸d1), (- 而이， (d1,0), （山，d1), (d1, -d1), (- 呱山）,and （크11，크h). The
distance d1 is given by
                                 d1 _,2ke1,                             (4.17)

where k = 伽g2pl. For example, for p = 7, k = 3 and d1 = 4 pixels. Using
the best match location as the starting point, we then look for the best match
in the eight perimeter points at distance d2 = 亨. We continue this process
until the k-th search, where the eight perimeter search locations are spaced by
one point. After these eight locations have been examined, we determine the
location that yields the smallest MAE.

Overall, logarithmic search examines 8k + 1 search locations and computes
the MAE at each search location using (4.16). For pictures at resolution I
 x J at F pictures/s the computational complexity of logarithmic search is
IJFx (8k+ 1) x3. Forl= 720, J =480, F= 30, andp= 15 (k =4),
logarithmic search requires around one GOP. The complexity of logarithmic
search is only 3.3 percent of the complexity of full-search.

In Figure 4.12, we illustrate the logarithmic search procedure in its more
popular form, referred to as the three-step search (TSS), where k = 3 帥d p
= 7. In videoconferencing applications, p = 7 is found to be sufficient for
good performance. Search locations corresponding to each of the steps in the
three-step search procedure are labeled as 1, 2, and 3.


     In the first step, starting from (0,0), we compute the MAE for the the nine
     search locations labeled 1. The spacing between these search locations is
     d1 = 4. Assume that MAE is a minimum for the search location (-4,0).

     In the second step, using (-4,0) as the center, we search among the eight
     search locations around it labeled 2; the spacing between locations is now
 1 10                                                             CHAPTER 4




        (-7,-7)                                                   (7,-7)




                                                                     (7,0)




        (-7,7)                                                    (77)


             Figure 4.12   Example of a three-step logarithmic search.



    d2 = 守 = 2 pixels. Let us assume that MAE is a minimum at search
    location (-4,2).

    In the third step, from (-4,2) as center, we search among the eight search
    locations labeled 3, and as in the previous step, the spacing between
    search locations is halved to d3 = 1. Assume that the MAE is a minimum
    at search location (-3,1). The search process is terminated at this point,
    since no further subdivision of the search space is possible, and the output
    motion vector is defined by the coordinates (-3,1).


The computation complexity associated with these 25 search locations is 777.6
MOPS (Million operations per second).
Fundamentals of Lossy Video Compression                                       111




4.5.3   Parallel Hierarchical One-Dimensional Search (PHODS)

Unlike the logarithmic search, in this search strategy the search is done
independently along the two dimensions. The search algorithm is as follows:

                                                                         and
 I. For a [-p,p] search region as shown in Figure 4.11, letS = 2[1og2pj
    set the origin of the search space at search location (0, 0). Denote the
    origin as (d自可）.

 2. In parallel, compute the

          i-axis local minimum: Among the three locations (di- S, dj), (di, dj),
          (di + S,dj), find the location that yields the smallest MAE. Set di to
          the i coordinate of this location.
          j-axis local minimum: Among the three locations (di, dj - S), (di, dj),
          (di, dj + S), find the location that yields the smallest MAE. Set dj to
          the j coordinate of this location. Set S = g.


Repeat step 2, until S = 0. The final (di, dj) is the motion vector that yields the
best match for the macroblock in the current picture.

This procedure is illustrated in Figure 4.13 for the case of p = 7. The reader
may want to compare this search process against the search process in Figure
4.12.

First, S =4.


  I. In the first step, for the i-axis minimum, we compute MAE for the three
     search locations labeled xl. Assume that the minimum is obtained at i
     = 0. In parallel, we compute the i- axis minimum using search locations
     labeled yl. Assume that the MAE minimum is obtained at y = 0. Thus the
     new origin is again (0,0).
  2. The spacing is reduced to 2. The i-axis minimum is obtained from the
     search locations centered at the origin obtained in the previous step, and
     these search locations are labeled x2. Assume that the MAE minimum
     is attained at i = -2. For the i- axis minimum, as in the i-axis case, we
     compute MAE for the j-axis search locations labeled y2. Assume the
     MAE minimum is attained at j = 2. Thus the new search origin is (-2,2).
                                                                   CHAPTER 4




   (-7,-7)                                                        (7,-7)




   (-7,7)                         (0,7)                           (77)


                 Figure 4.13    Example of PHODS strategy.



 3. For this step, S = I, and the minimum MAE along the i-axis is determined
    from MAE computations at search locations labeled x3. We can determine
    in parallel the minimum MAE along the j-axis by computing the MAE
    at locations labeled y3. Assume that the MAE minimum along the i- and
    j-axis is attained at (-3,1). Since S = I at the start of this step, no further
    reduction in spacing is possible, and this terminates the search algorithm.
    We declare (-3,1) as the location yielding the smallest MAE and therefore
    the motion vector for the macroblock in the current picture.


For the case of p = 7, we need to examine 13 search locations, which for
斗ames at 720 x 480 resolution and 30 fps corresponds to 404.35 MOPS.
Fundamentals of Lossy Video Compression                                      113




PHODS has two distinct advantages over TSS: (1) the MAE calculations are
parallelizable, and (2) it has a regular data flow, since the search locations are
always along the i-axis and the i- axis.

Both the logarithmic and the PHODS methods belong to the class of fast
algorithms that reduce motion-estimation complexity by reducing the number
of search locations that are used in determining the minimum MAE. For p
= 7, compared to a full-search method, the complexity is reduced from 6.99
GOPS to 404.35 MOPS. Fast algorithms that work in the reduced search space
assume that MAE(i, j) of (4.16) increases monotonically as the search area
moves away from the best-matched location. Such algorithms perform as well
as the full-search method if this assumption holds; however, in practice the
assumption often fails, since not all the search locations are visited, and the
search for a global minimum may get trapped into a local minimum. This is
illustrated in Figure 4.14, which shows hypothetical MAE values for different
search points.

In Figure 4.14a, there is a single global minimum. Thus, the result of the
fast algorithm coincides with the best solution obtainable with full-search.
In Figure 4.14b, there is a global minimum and a local minimum. The fast
algorithm gets trapped in the local minimum and declares X as the location of
the lowest MAE, even though the full-search method would have found the
true minimum at location Y. Thus, fast algorithms such as those described
here may yield a larger motion-compensated prediction error e(x, y, t) than a
full-search scheme.



4.5.4 Pixel Subsampling and Pixel Projections for MAE
         C川culations

An alternative approach to reduce the motion-estimation complexity is to
reduce the number of pixels that are used in computing block differences in
(4.16). The motivation for using a reduced number of pixels is this: since
block matching implies that all pixels within the macroblock have the same
motion, an estimate of the motion can also be obtained with fewer pixels. Pixel
decimation must be done in a careful manner so as not to reduce the motion
estimation accuracy. A strategy for pixel decimation in the context of motion
estimation is shown in Figure 4.15.
                                                                                            CHAPTER 4




                                  MAE
                                                        Result from fast algorithm is
                                                         졔so the best s이Ut幻n




                          1   1    1                I     I  I I 1
                                                             x
                                                        match location
                                              (a)
                                                                The fast algorithm
                                                           is trapped into a local minima




                                                                      x
                                                                mat(才｝ locat向n
                                        (b)
      Figure . .14 '.[AE versus search location. (a) MAE function is
      二Criotc，二C: ft 5earch result is trapped into a local minimum.



三：5 ：·iClma::: pr:;ess is explained as follows. Assume we are using a
之斗S.亡二二h 口i: od. For each 入4AE value, we use only one fourth of the
::xe:5 Pixe:i 1abek:: I are used for computing MAE(i, j) at (0.0) and all
 쿄二＝ xau:·:s 2; : 1). Pixels labeled 2 are used at all search locations
 :: . : . 小 : . Pi키s l亡eled 3 are used at search locations (2i + 1, 2j + i ' . and
二m5 ...bele: - are .ed at all search locations (2i + 1, 2j). By alternating the
::e: ;;: tern5 三二d aS5Ociating a different pattern for each neighboring search
i＼二：二all노. 그ixC:5 within the block are covered within four search locations
a二dhe::亡. aL ::xelc 그 the picture are used in motion estimation. Furthermore,
出l5 三＝그iatr': ri끄n: iizes the possib小ty of n야 considering one-p怏el-wide
                                                                               115
Fundamentals o／乙)S5y V油oCo／까片es汕n




                        1    2    1   2    l       2   j       2

                        3    4    3   4    3       4   3       4

                         1   2    l   2        l   2   ]       2

                         3   4    3   4    3       4   3       4

                         1    2   1   2        1   2   1       2

                         3    4   3   4        3   4   3       4

                         1    2   1    2       1   2       l   2

                         3    4   3   4        3   4   3       4



      Figure 4.15      Pixel decimation for block matching in an 8 x 8
      block.


                                                          e, the computational
 horizontal, vertical and diagonal lines. With this schem
                                                      percent.
 complexity of a full-search method is reduced by 25
                                                            the MAE calculations
 Yet another approach to reduce the pixels used in
                                                              al directions and use
 is to form a projection of the macroblock along sever
                                                                  themselves. This
 the samples along the projections instead of the pixels
                                                                n projection vector
 is depicted in Figure 4.16. Each element of the colum
                                                            n of the 8 x 8 block.
 is the sum of pixels along the corresponding colum
                                                         manner. For a 16 x 16
  The row projection vector is formed in a similar
                                                              calculations in (4.16),
  macroblock, the operations are identical. In the MAE
                                                           differences with the sum
  we replace the sum of absolute values of N x M pixel
                                                                ng row and column
  of absolute values of the differences of the correspondi
                                                                    a factor of 금모旨·
  projections. This reduces the complexity by approximately
                                                             form projections along
  For improved motion-estimation accuracy, we can also
                                                                   ations that require
  various diagonals. In practice, for video conferencing applic
                                                             been   found to provide
  a very high compression ratio, two projections have
                                                       search method. On the other
  accuracy only slightly inferior to that of the full-
                                                          computations required in
  hand, this approach requires only 12.5 percent of the
                                                             d can be combined with
  the full-search method. Note that, the projection metho
                                                             additional computation
  any of the fast search strategies discussed above for
   savings.
 116                                                                                                                                                                                             CHAPTER 4




                                                                                C이umn F가이ection


                                                    1          1                  1                            1               1                 i                    1                      1
                                            -        rm
                                                          -
                                                               r        미
                                                                            h   114       e          41e
                                                                                                                       -        n=
                                                                                                                                             -
                                                                                                                                                 r           m 느      寸        ＝寸
                                                                                                                                                                                     -       I
                                                    1               1             1
                                                                                  1
                                                                                                               1                1                    !
                                                                                                                                                     1
                                                                                                                                                                      1                      1




                                        _
                                                    L.
                                                          P1   J=
                                                                        여 느     =     H                                -                     나   I-
                                                                                                                                                             =            1_
                                                                                                                                                                                     -   I
                                                                1                1                                                               1

                                        : : ; : : : : :
                                                                                                    나－
                      C으尸8흐口三운
                                 나之口二   +나 +      r
                                                      ：                 . 卜     기
                                                                                 1
                                                                                      =m
                                                                                                                       -                 4

                                                                                                                                         -
                                                                                                                                                 1
                                                                                                                                                         미
                                                                                                                                                                 1
                                                                                                                                                                          1
                                                                                                                                                                          1    叫    中
                                                                         =
                                                1              1                                           1               1                     1                   r                   1
                                                                                      '                            -   -
                                                                                                                                                                     十
                                        -
                                                I-
                                                                                                -I
                                                                                                                           I-
                                                          戶             미                                                                                -       1
                                                               t1
                                                                                                                                             -
                                                                                                                                                 r-
                                                                                                                                                                               m    ＝시
                                                                                                                                                                     1
                                  4
                                                1              1                                           1               1         m           1                                       i
                                                                                                           1



                                        _
                                                L         _
                                                               L        = 느     그     ==       =           1       e   m   1H
                                                                                                                                     1H          L       m       n
                                                                                                                                                                     J.
                                                                                                                                                                               H    -
                                                                                                                                                                                         I
                                                1              1                 !                         1               1                     1                        !              l

                                        + : : : : : : :
                                        H       1 1                              1
                                                                                              41m
                                                                                                                           i                     1                        1              1




        Figure 4.16        Row and column projection of pixels in an 8 x 8
        벼ock.



The main disadvantage in using fewer pixels than 16 x 16 is that the motion
vector estimate may be unreliable due to noise in the current and reference
pictures. A summation over 16 x 16 pixel differences has the side benefit of
masking this noise by noise averaging. This effect is reduced when we use
fewer pixels in the MAE calculations.



4.5.5    Hierarchical Motion Estimation

Several fast motion-estimation schemes use a combination of search strategies
that use both fewer search locations and fewer pixels in computing the MAE.
A scheme that combines these two features is widely referred to as the
hierarchical search method. There are many variations of this method, but one
approach is depicted in Figure 4.17.

The motion vector search proceeds as follows:
Fundamentals of Lossy Video Compression                                            117




             Reference Picture




                                                               mH>
                                                                     M야幻n vector




                                 니「"뼝灣口"
                                         ]




                                      「「’"
                                 H ""뼝立클
                                         1
                                                    Motion
                                                   Estimat幻n


      Figure 4.17     A generic hierarchical motion vector search strategy.




  1. We form several low-resolution versions of the current picture and the
     reference picture. In Figure 4.17, we show two low-resolution versions at
     Level I and Level 2 for the reference picture. A similar set of operations
     is performed to obtain low-resolution versions for the current picture. Let
     us assume that the macroblock in the current picture is located at (x, y). In
     Level I and Level 2, the corresponding macroblock is at (플, 블 ) and (둥, 芝 ),
     respectively. Let us also assume that the size of the macroblock at Level
     0 is 16 x 16 and that the motion vector has a dynamic range of 士p pixels.
 lI i                                                                   CHAPTER 4




        '뇨＼'e 5:art t}i亡 motion vector search at Level 2. Here, one can view the
        」．=.＝二as a .- D llection of macroblocks of size either 16 x 16 or 4 x 4. In
        : :a:1 :pp1i：三tions, the latter is sufficient. Furthermore, the scaled version
        ：三 二isear: parameter can also be used; that is, we can use 弓 instead of
            He: e. a: Level 2, we can use any motion vector strategy, such as the
        三．-.:玎ch -Cheme or the logarithmic search scheme that we described
             :e:. with 4 x 4 macroblocks, a search parameter of 弓, and the origin
                 5ear』
                     ．:. located at ( .프．, 享 ). Assume that the MAE is minimized at
                                   '
                                       '*   .   .f   '




        二．:Le，키 1. ..e perform the motion vector search on 8 x 8 macroblocks
         \：二:1亡 o- ::ri of the search located at 愕 + 2 112, 晝 + 2 v2), and a search
        在1H 그f ! - . 1] pixel around the origin. As before, we can use any search
        :：二：i; 1 . .A5: .ime that the MAE is minimized at (n1. t1).

        A: Le」키 0. .;. e locate the search origin at (x + 2 ul, y + 2 vi), and we search
        二a s三ch rc ion off-I, I] pixel around the origin, with a macroblock size
        :：「：亡 : 16 Any search method, including full-search, can be employed.
        卞:e '.::atic: :hat yields the smallest MAE corresponds to the final motion
        . 亡：::' 그utr二：


Nc：亡 :-_:. ::l 卄. . hierarchical search scheme, we reduce both the number of
sea：二 ’．工 a::ons a그d the number of pixels used in the MAE calculations. Let
us 느二쓰i :he 댜그n犯ters for broadcast TV (720 >< 480 at 30 fps), a 16 x 16
ma:: .c·; : size arid a search parameter of p = 15. We will also assume that a
fufl-七a:a: rrieth :.1 is used for motion estimation at each level of the hierarchy.
We e5::工aa亡 the 교mplexity at each level of the hierarchy as follows:


 1 Le '타 :

            二 :ture size = 180 x 120, and macroblock size = 4 x 4.
            N. mhe: of macroblocks = A才Macr。
                                        Pzctue  , stze
                                             ..。ck    , , = 1,350. At 30 fps, we
                                                    szze
            :a ";e 41.500 macroblocks.
            Search :arameter = f 1 = 4.
            卜；...mberofsearchlocations= (2 x 4+ 1)2= 81.
            N_ mhe- of operations per search location = macroblock size x 3 =


         r쓰:I八it' : :rLevel2= 40,500 x 81 x 48= 157.46 MOPS.
                                                                            119
Fundamentals of Lossy Video Compression




 2. Level 1
                                                             8.
    a    Picture size = 360 x 240, and macroblock size = 8 x
                                                                have 40,500
    a    Number of macroblocks = 1,350. At 30 fps, we
         macroblocks.
    1    Search parameter = 1.
    1    Number of search locations = 9.
                                                          block size x 3 =
     a   Number of operations per search location = macro
          192.
                                                            MOPS.
    Complexity for Level I = 40,500 x 9 x 192 = 69.98

  3. Level0

     a    Picture size = 720 x 480, and macroblock size = 16 x 16.
                                                                   40,500
     a    Number of macroblocks = I ,350. At 30 fps, we have
          macroblocks.
     a    Search parameter = 1.
     a    Number of search locations = 9.
                                                                size x 3 =
     口    Number of operations per search location = macroblock
          768.
                                                            MOPS.
     Complexity for Level 0 = 40,500 x 72 x 48 = 279.9

                                                          s 0 through 2 and is
 The total complexity is the sum of complexities in Level
                                                       29.89 GOPS needed for
 507.38 MOPS. This is a significant reduction over the
 a full-search method.

                                                          method is very efficient;
 From a complexity viewpoint, the hierarchical search
                                                          due  to the need to keep
 however, such a method requires increased storage
                                                             e may yield inaccurate
 pictures at different resolutions. Furthermore, this schem
                                                          Since the search method
 motion vectors for regions containing small objects.
                                                                      small objects
 starts at the lowest resolution of the hierarchy, regions containing
                                                       tracked. On the other hand,
 may be completely eliminated and thus fail to be
                                                                immunity to noise.
 the creation of low-resolution pictures does provide some
  120
                                                                     CHAPTER 4




  4.5.6    Performance Comparison of Motion-Estima
                                                                 tion Methods

  For the MAE cn幻on. Table 4.1 summarizes the comp
                                                       utational requirements
  of the four major motion-estimation techniques we descr
                                                          ibed in this chapter.
  In all eases. "A e .5sume 16 x 16 macroblocks and
                                                    a search range of [p, -p]
  pix러S.


     Search            Operations per              Operations for pictures
     Meth叱              \ lacroblock                   720 x 480 at 30 fps
                                                    7) ＝二 15          刃= 7
                      r 2:·，+ 1)2.VM3            29.89 GOPS         6.99 GOPS
   L0：二：m.' 1中       y1: :72／기 + 1 1\' jf3         1.02 GOPS 777.60 MOPS
   PHODS             4l ':72p] + 1)'VM3         528.76 MOPS 404.35 MOPS
   n＝二＝=;           二f- 1)2 + 180] 쓱竿3          507.38 MOPS 398.52 MOPS

        Tabk 4.1 Co.mputationa.l comple.xity and. MOPS
                                                          requir
        iC: '.：二Dus -otion-estimauon aigontnms using me iviir ements
                                                              critenon
        쏘그d a 1:lr ' search range.




In Figure 二．: S. \\ 亡 5 hov. the performance of several motio
                                                              n-estimation meth-
ods. In all 乙ses. : = 15. and we use 16 x 16 macroblocks
                                                            .

 F唯ures -i.. i S; to ; 181. show the motion-compensa
                                                        ted prediction error. If
 motion esti三ltion were perfect, then we would expec
                                                           t an error picture that
 would t足 comple:elv black. Figure 4.18c shows the predic
                                                                tion error for the
case of a z亡꼬-Va..ed motion vector (simple frame
                                                        differencing). The full-
 search methc.d performs the best in that the prediction
                                                         error is close to zero in
most regions of the picture. The logarithmic search schem
                                                               e is inferior to the
full-search a..i the -ierarchical methods, probably
                                                     because the search strategy
gets trappe. :nto :CaI minima. Due to Iowpass filterin
                                                               g, the probability
of getnng Lr.a갸）e口 :nto local minima is reduced in the hierarchica
                                                                        l scheme,
and F唯ure .- i 8f ::dicates that the performance
                                                    is nearly as good as using
full-search.

.AII our discus 'ions have considered macroblock sizes
                                                       of 16 x 16. In practice,
the performan쿄 among the search methods is similar for
                                                           block sizes of 16 x
S or S 노. S. A: smai:er block sizes, such as 8 x 4 and 4
                                                          x 4, the hierarchical
Fundamentals of Lossy Video Compression                                         121




                                                          (d)
                   (c)
                         (e)
                                                                (f)


      Figure. 4.18 nPerforman
                         P        ce comparison of motion-estimation
      rnernocls... .(a) Kererence plcture; ISO) current pi.cture; (C) sirnp！드
      rrame. airrerencing; U) iuii-searcn; (eJ iogaritnmic searcn; I1)
      tnree- ievei nierarcnicai searcn.



 scheme performs much worse than the logarithmic scheme. This is probably
 due to an insufficient number of pixels within the small blocks to obtain
 accurate estimates of MAE. For the fast search methods, visually, the decrease
 122                                                             CHAPTER 4




in block size manifests as block flickering in the reconstructed sequence. In
the case of full-search, the decrease in block size reduces motion artifacts,
since we assign motion vectors to smaller regions of the picture. This also
improves the smoothness of the motion vector field and thus makes the vectors
amenable to compression.

The video coding standards do not specify which motion-estimation method
to use. Any of the methods discussed here is applicable.




4.6 SUB-PIXEL-ACCURATE MOTION
    ESTIMATION
In all our discussions, we have restricted the motion vector estimation to
integer pixel grids. Thus, the motion vector would be pixel or pel-accurate.
The true frame-to-frame displacements are unrelated to the sampling grid, and
thus, one would expect improved prediction if displacement estimates were
obtained at a finer resolution. This implies that we need to determine motion
vectors with fractional or sub-pixel accuracy. The video coding standards
permit motion vectors to be specified to a half-pixel accuracy.

Motion vector estimation with, say, half-pixel accuracy can be easily found
by interpolating the current and reference pictures by a factor of two and then
using any of the motion-estimation methods described in the previous section.
Since this method uses excessive storage requirements,the following two-step
alternate approach is usually prefered. We illustrate the two-step approach in
Figure 4.19.


 1. In the first step, we find a motion vector with integer-pel accuracy using
    any of the motion-estimation methods described in the previous section.
    The resulting integer-pel accurate motion vector (u,v) that yields the
    smallest MAE is as shown in Figure 4.19. Let us denote the corresponding
    MAE as MAE(u,v).

 2. In the second step, we refine the results of the first step to obtain the
    motion vector with the desired half-pixel accuracy. To refine the (it, v)
    motion vector to half-pixel accuracy, we do the following:
                                                                                   123
FunL／口刃ient口／s ofI刃ssy Video C（가npression




          Integer-pel grid                      Ha作pel grid




                                                     Estimated pixel values
                                                     on ha牛p이 grid using
       Pet-accurate                                  pixel values on integer-pel
       motion vector                                 grid
       (u,v) ＼늬；
           (0,0)



                Sub-pet accurate
                mot幻n vector (k力


          Figure 4.19        Ha作pel accurate motion vector estimation.


                                                                         the top-left
          We form eight new search blocks of 16 x 16 pixels, with
                                                                               e 4.19.
          corner of each block being at the locations marked X in Figur
                                                             where m,  n E  [-1,0  ,1],
          These locations are denoted as (u+ 끙, v + 글 ),
                                                                              each   of
          but m and n cannot be both zero at the same time. For
                                                                                  with
          these eight new search blocks, we know only those pixel values
          coordinates matching our original integer-pel grid. The rema           ining
                                                                                 using
          values on the haif-pel grid of Figure 4.19 can be estimated
          simple bilinear interpolation techniques.
                                                                                 eight
          We compute new MAE values by comparing each of these
                                                           . Deno te by MAE     (m,  n)
           search blocks with the original macroblock
                                                                           left corne  r
           the MAE value associated with the search block whose top
           is located at (u + 끙，iJ + 글）·
                                                                                (rn, ii)
           Denote by (k, 1) the position of the block for which MAE
           is minimum. Note that, MAE(u, v) is also included in finding the
           minimum. Thus, (k, 1) is the ha作pel refinement to the integer-pel
                                                                                       n
            accurate motion vector (ti, v), and the final half-pixel accurate motio
                                                               the 丸，1 values do n아
            vector is given by 佃 + 知 + 吉）. Note that,
                                                                                  video
            have to be nonzero values. Depending on the nature of the
                                                                               (u, v) is
            sequence, there will be regions in the picture where MAE
124                                                                              CHAPTER 4




           minimum among the nine MAE values. In such cases, the integer-pet
           accurate motion vector is the right choice.

      A similar procedure can be adopted if motion vectors are needed at, say,
      quarter-pet accuracy.


The pixel interpolation step is compute intensive. In recent years, fast methods
that do not perform the interpolation step to determine sub-pixel accurate
motion vectors have been developed. We briefly describe one such fast
method. The various steps in the fast method are depicted in Figure 4.20.




      卜
                                                      Half pel grid




                        業－
                                                          Location (u,v) - result
                                                          of integer-pel accurate
                                                          m아幻n estim帥on method

                             回

                                                 x2
                                       시
                                                 1
                                   1
                                   1
                                                    D
                                                 1k t
                                                                      yO
                                   下 工           *

                                   I             I
                                           xO
             (b)
                                                                           (d)
                                           (c)
      Figure . 4.20. .Fast method for half-pet..accurate motion .vector
      estimation. (a) integ르r-pei accurate motion vector .estimate; IS기
      comDutation ot MAt, at neighbonng integer-pel aisDlacements;
      (C) integer-pe! ioc.ations usea in computing me iviti.r. minimum
      aiong me nonzontai airection; ! Q) integer-pei iocations usea in
      computing the MAt minimum along the vertical cflrection.
Fun（亡I刃ientals ofI刃ssy Video（勿mpress,切1                                     125




    Let us assume that we found the integer-pel accurate motion vector using
    any of the methods described earlier. The location corresponding to this
    motion vector is shown in Figure 4.20a. Let us denote the corresponding
    MAE value as mO. Since pixel values are known on the integer-pel
    grid, we can compute MAE at the neighboring four locations on the
    integer-pel grid as shown in Figure 4.20b. These MAE values are denoted
    as ml, m2, m3, and m4.

    In (4.16), around the location corresponding to mO, we will model MAE
    as a separable function.

    Along the horizontal (i) direction, this function is of the form p(i) =
    aui 寸 bj + c. Here, a, b, and c are constants and can be explicitly derived
    using p(O) = mU, p(l) = m4, and p(- l) = m3. Using simple algebra, it
    can be shown that for the motion vector to yield the smallest MAE on the
    sub-pixel grid in the i direction, one of the following conditions must be
    met:

      I. If 2(m3 - rri0) < (m4 - mU), the i coordinate of the motion vector is
         one of the three values on the xl line shown in Figure 4.20c.
      2. If (m3 - mU) > 2(m4 - mO), the i coordinate of the motion vector is
         one of the three values on the x2 line shown in Figure 4.20c.

    If neither of these conditions is met, the i coordinate of the motion vector
    is on the xO line shown in Figure 4.20c. Note that, the xl line corresponds
    to a displacement of (u - 0.5), the x2 line corresponds to a displacement
    of (u + 0.5), and the x0 line corresponds to a displacement of u.

    In a similar manner, we model the MAE along the vertical (j) direction as
    a function of the form p(j) = aj - bl + c. Here, a, b, and care constants and
    can be explicitly derived using p(O) = m0, p(l) = m2, and p(- l) = ml.
    Using simple algebra, it can be shown that for the motion vector to yield
    the smallest MAE on the sub-pixel grid in the j direction, one of the
     following conditions must be met:
       1. If 2(ml - mU) < (m2 - m0), the j coordinate of the motion vector is
          at one of the three locations on the yl line in Figure 4.20d.
       2. If (ml - m0) > 2(m2 - mO), the j coordinate of the motion vector is
          at one of the three locations on the y2 line in Figure 4.20d.

     If neither of these conditions is met, the j coordinate of the motion vector
     is at one of the three locations on the yO line in Figure 4.20d.
 126                                                               CHAPTER 4




 For example, if after these tests we find that the i coordinate of the motion
 vector is on the x2 line and that the j coordinate is on the yl line, then the
 haif-pel accurate motion vector is the vector (u + {, v - 古）.

 Thus, one can determine the half-pet accurate motion vector without the explicit
 computation of pixel values on the half-pel grid. Note that, such computations
 are not completely avoidable. If the motion estimator yields a motion vector
 with coordinates at the half-pet grid, then we still need to compute pixel values
 at the half-pet grid in order to compute the motion-compensated prediction
 error.




 4.7 MULTIPICTURE MOTION ESTIMATION
In our discussions on motion estimation and motion-compensated prediction,
 we have restricted attention to the case where the motion estimation is
performed using only one reference picture. In instants of smooth motion,
 there is a great deal of correlation between the current picture at time instant
 t and pictures prior to and after time instant t. Thus, it is beneficial to
compute a prediction of a macrobtock in the current picture using motion-
compensated regions from the pictures prior to and after time instant t. This
is called bidirectional prediction. The motion-compensated prediction for the
macroblock X is simply the average of the the motion-compensated prediction
between X and A and between X and C. This form of prediction is also
referred to as inte叩아ative pred奴而n.

In Figure 4.21, we show the current picture and two pictures denoted as
reference pictures. The motion vector estimated using the reference picture at
time t - m is shown as the vector b, and the motion vector estimated using
the reference picture at time t + n is shown as the vector f. Motion vectors
b and f can be found using the methods for motion estimation described in
the previous sections. Since bidirectional prediction doubles the complexity
of motion vector estimation, several fast methods have been devised; for
instance, one might use b as a hint to search for f.

In the video coding standards, for certain types of pictures, two motion vectors
can be used for a macroblock X. The specific details on when one uses one
Fundamentals of Lossy Video Compression                                    127




           Reference picture   Current picture      Reference picture
              at 恤ne t寸TI         at time t            at time t+n


         Figure 4.21 Multiframe motion-compensated prediction.



motion vector instead of two will be described in the chapter on the video
coding standards.




4.8 TO PROBE FURTHER
In this chapter we intr어iuced the basic concepts associated with the compres-
sion and decompression of image sequences (video). The main difference
between the spatial-domain coding methods discussed in the previous chapter
and the video coding techniques discussed in this chapter are the temporal
extensions, which comprise two functions: motion estimation and motion
compensation. From an information-theoretic viewpoint, the benefits of tem-
poral extension were determined, through the development of rate-distortion
 functions for video coding. Our approach to computing the rate-distortion
 functions parallels the developments in [153], [187], and [60]; we have omitted
many of the details and we direct the reader to these references for further
 details. The modeling of the motion-compensated prediction error, which is
useful in the calculation of the rate-distortion functions, is also discussed in
 [1781 and [61].

 In this chapter, we have focused on motion-estimation methods that find
 the best match between a 16 x 16 macroblock in the current picture and
 a 16 x 16 pixel region in the reference picture. In recent years, it has
 been observed that the translatory-motion model assumption of such motion-
 128                                                              CHAPTER 4




 estimation methods may not be appropriate for many video sequences. A
 generalized block-matching method that maps a 16 x 16 macroblock to a
 deformed (quadrilateral-shaped) region in the reference picture is described
 in [175]. This scheme outperforms the square-region-based block matching
 discussed in this chapter. In most motion-estimation methods, for the best
 match, the mean absolute difference (MAE) cost function is used. An
 alternative criterion based on classifying each pixel is described in [59]. This
 method is claimed to yield good performance for large search windows.

 Over the years, several heuristic motion-vector search schemes have been
 developed; descriptions of some of these schemes can be found in [166],
[58], [115], [198], and [163]. A description of the 2-D logarithmic search
discussed in this chapter can be found in [90]. Its more popular variation,
 namely, the three-step search scheme, is described in [98). The PH0DS
 method of motion vector search discussed in this chapter was first presented
in [30], and comparisons with the three-step search method are provided
in this paper. Motion vector search methods that employ pixel decimation
are developed in [123], and the approaches adopted here yield performance
very close to the full-search method. There have been several motion vector
search schemes that employ a hierarchical decomposition of the current and
the reference pictures, and one of the implementations is discussed in [21].
A hierarchical block-matching method with specific emphasis on hardware
implementation is described in [160]. Additional hardware implementations
for motion estimation are also described in a later chapter.

The video coding standards allow motion vectors to be represented with
sub-pixel (half-pixel) accuracy. In this chapter, we provided a fast method
for determining such motion vectors using a model for the MAE function. A
discussion of the performance using this model versus a model that employs
a squaring function is provided in [95]. There, it is shown that the squaring
function, though mathematically tractable, is not necessarily a good fit to the
MAE.
                                                                        5
                           THE JPEG STANDARD




5.1 INTRODUCTION
Until recently, the Group 3 and Group 4 standards for facsimile transmission
were the only international standard methods for the compression of images.
However, these standards deal only with bilevel images and do not address the
problem of compressing continuous-tone color or grayscale images.

Since the mid- 1980s, members from both the International Telecommunication
Union (ITU) and the International Organization for Standardization (ISO)
have been working together to establish a joint international standard for the
compression of multilevel still images. This effort has been known as JPEG,
the Joint Photographic Experts Group. Officially, JPEG corresponds to the
ISO1IEC international standard 10918-I, Digital compression and coding of
continuous-tone still images or to the ITU-T Recommendation T. 81. The text
in both these ISO and ITU-T documents is identical.

In recent years, there have been many new developments in the field of image
compression. These include new compression schemes based on transform
coding, vector quantization, subband filtering, wavelets, and fractals. The goal
of JPEG has been to develop a general method for image compression that
meets a number of diverse requirements, including the following:


    Be as close as possible to the state of the art in image compression.
    Allow applications (or a user) to tradeoff easily between desired compres-
    sion and image quality.
130                                                             CHAPTER 5




      Work independently of the image type. That is, the method should not
      be restricted by the type of image source, image content, color spaces,
      dimensions, pixel resolution, etc.

      Have modest computational complexity that would allow software-only
      implementations even on low-end computers. Low-complexity hardware
      implementations should also be feasible.

      Allow both sequential (single scan) and progressive coding (multiple
      scans).

      Offer the option for hierarchical encoding, in which a low-resolution
      version of the image can be accessed without a need to decompress the
      image at full resolution.


After evaluating a number of coding schemes, the JPEG members selected a
DCT-based method in 1988. From 1988 to 1990,the JPEG group continued its
work by simulating, testing, and documenting the algorithm. JPEG became a
draft international standard in 1991 and an international standard in 1992. The
JPEG group has not yet completed its mission. It continues to work on future
enhancements. ISO 10918-3, which specifies recent extensions to JPEG, has
already been approved as a draft international standard.

JPEG includes two basic compression methods: a DCT-based lossy corn-
pression method and a predictive method for lossless compression. We have
already examined the lossless compression method in an earlier chapter. In
this chapter, we provide an overview of the lossy JPEG method.




5.2 DCT-BASED CODING
The JPEG standard specifies four modes of operation: sequential DCT-based,
progressive DCT-based, lossless, and hierarchical. Under the lossless mode, a
predictive coder followed by either a Huffman or an arithmetic coder is used
instead of a DCT-based scheme. The details of operation under the lossless
mode were discussed in Chapter 2. To better understand the other modes of
operation, we need first to review the DCT-based coder.
The JPEG Standard                                                          131




5.2.1 JPEG Encoding

Figure 5.1 shows a block diagram of the DCT-based JPEG encoder for an
image with a single color component(grayscale). For color images,the process
is repeated for each of the color components.




               Figure 5.1   Block diagram of a JPEG encoder.


From Figure 5.1, the image is first divided into nonoverlapping blocks. Each
block has 8 x 8 pixels. If any of the dimensions of the image is not a multiple
of eight, then the pixels of the last row or the last column in the image are
duplicated appropriately.

Each block is transformed into the frequency domain by a 2-D DCT. The
standard does not specify a unique DCT algorithm. Consequently, users may
choose the algorithm that is best suited for their applications. The DCT output
coefficients are quantized and entropy coded.

The entropy coder consists of two stages. The first stage is either a predictive
coder for the DC (or [0,0]) coefficients or a run-length coder for the AC
coefficients. The second stage is either a Huffman coder or an arithmetic
coder. Arithmetic coding provides better compression than Huffman coding;
however, there are very few JPEG implementations that support arithmetic
coding. There are three main reasons for this. First, the improvement
in compression (2 percent to 10 percent) does not justify the additional
complexity (especially for hardware implementations). Second, many of the
algorithms on arithmetic coding are covered by patents in the United States
and Japan. Therefore, most implementors are reluctant to pay license fees for
132                                                               CHAPTER 5




minimal gains in performance. Third, the baseline implementation, that is, the
implementation with the minimum set of requirements for a JPEG compliant
decoder, uses only Huffman coding.

In order to facilitate the acceptance of JPEG as an international standard
and because of the various options available during JPEG encoding, the JPEG
committee also defined an interchange format. This interchange format embeds
image and coding parameters(type of compression,coding tables, quantization
tables, image size, etc.) within the compressed bit stream. This allows JPEG
compressed bit streams to be interchanged among different platforms and to
be decompressed without any ambiguity.



5.2.2 JPEG Decoding.

Figure 5.2 shows a block diagram of a JPEG decoder. After extracting
the coding and the quantization tables from the compressed bit stream, the
compressed data passes through an entropy decoder. The DCT coefficients




               Figure 5.2 Block diagram of a JPEG decoder.

are first dequantized and then translated to the spatial domain via a 2-D inverse
DCT. After a block-to-raster translation, the image is fully decoded.
The JPEG Standard                                                           133




5.3 PROCESSING OF COLOR IMAGES
Thus far, we have considered JPEG compression of images with a single corn-
ponent. In practice, images may be represented by multiple color components,
each at a different resolution. For example, most color scanners generate
images with red, green, and blue color components (RGB).

JPEG sets no restrictions on the type of the input color space. Instead, it views
each image as a collection of image components. The maximum number of
color components in JPEG is 255. Each component consists of a rectangular
array of samples (pixels). Each sample may be represented by P-bits of
precision. In JPEG, P can be either 8 or 12 for DCT-based coders and from
2 to 16 for lossless coders.' Images with other pixel resolutions can still be
coded using JPEG; however, pixel values have to be shifted to be within the
resolutions supported by JPEG.

It is not necessary that all color components have the same dimensions. Let x2
and yi denote the horizontal and vertical dimensions for the i-th component.
          昔 and V)
If 三x3- = H)       劈 = i 뇹， then the relative horizontal and sampling factors
for the components (that is, H, and V1) are allowed only the integer values I
to 4. Under the JPEG interchange format, a color image is specified by the
maximum horizontal and vertical dimensions (X = max(xi) and Y = max(y2)),
the relative sampling factors for each component, and the maximum relative
sampling factors (Hmax and Vmax). The maximum dimension supported by
JPEG is 216 = 65,536 samples. Given the above information, the decoder
extracts the dimensions of each component using the following equations:

                             m
                             xi   =
                                  =
                                                                            (5.1)
                                               1
                                                    H,
                                      FXx
                                            I I          , ,
                                      以
                                                                    1
                             yi
                                  =    小v
                                              '丘，
                                                               ］·
                                                                            (5.2)



Example. We want to compress a color 512 x 512 RGB image. Since
JPEG requires each color component to be handled separately, one approach
would be to compress the RGB image by applying the JPEG compression
method on the R, G, and B components separately. In typical RGB images,
there is significant correlation between the color components; thus, from a
compression viewpoint, the ROB space is not an efficient representation for the
표下Gcon叩ression n妃thod. 가re ide키 approach would be to trans如rm the ROB
134                                                             CHAPTER 5




image into another component representation, where each of the components
is decorrelated with respect to each other, and then apply the JPEG method.
In practice, this is done by first transforming the RGB representation into a
luminance and chrominance (or color difference) representation, such as YUV,
YCbCr, or CIELAB. Assume that the image is translated from the RGB color
space into the YCbCr color space. (The reader may want to refer to Appendix
A for the RGB to YCbCr color transformation matrix). There is very little
correlation among the components in this representation. Furthermore, since
most of the spatial information is in the luminance (Y) component, we lose
little information if we subsample the Cb and Cr components by a factor of
two in both dimensions. Thus, even before applying JPEG compression, we
have reduced the image size in half by this simple color-space transformation.

After color-space transformation and subsampling, the image color compo-
nents have the following dimensions: for the luminance component, x0 = I/o =
512; for Cb and Cr, x1 = 工2 = !/l = Y2 = 256. Thus, X = Y = max(256, 512) =
512. The relative sampling factors are H0 = V0 = 2 and H1 = H2 = V1 = V2 = 1.
Thus, 尸m口工 == V.뉴lO工 = 2.



5.3.1   Data Interleaving

Images with multiple components can be stored and processed either with or
without data interleaving. When there is no data interleaving, each component
is stored and processed separately. For example, a 512 x 512 noninterleaved
RGB image would be stored as three separate 512 x 512 8-bit images: one
with the red pixels, one with the green pixels, and one with the blue pixels.

For more efficient storage and processing, the color components can be
interleaved. A data unit is defined as the smallest logical unit of source data
that can be processed by JPEG. For lossless JPEG, a data unit corresponds to
a single sample. For lossy JPEG, a data unit is a single 8 x 8 block of data.
Under color interleaving, the i-th color component is partitioned into small
rectangular blocks of dimension Hi x V, data units. If we select one H: x V
data block from each of the color components, then we form what is referred
to by JPEG as the minimum coded unit (MCU); that is, the smallest group
of interleaved data. Figure 5.3 shows an example of interleaved data ordering
for a YCbCr image. In this example, the Y component is divided into blocks
of 2 x 2 data units, and the Cb and Cr components are divided into blocks of
The JPEG Standard                                                         135




            0 1     2 3 4   5             0 1   2 3      0 1    2 3

        0
        1
            1
            0
                 D 1
                 0 0
                       1 0 0
                       0 0 0
                                      0 . .
                                      1 . .     이      0 . .
                                                       1 0 0   이
        2   0    1 0   1              2 0              2 I
        3   0    1 0   0              3                3


                V plane                   Gb plane       Cr plane
                                           H1= V1= 1     H2= V2- 1
                H0= V0= 2

             MCU1 =V0V。                       2Y。
                      1 Y1。Y11 Cb0Cr00 MCU2= V。               1
                                                3Y12Y13Ct 1 Cr。




                   Figure 5.3   Example of data interleaving.


single data units. An MCU is created by taking the four data units from Y, one
data unit from Cb, and one data unit from Cr. Within one data unit, pixels are
ordered from left to right, top to bottom.

In general, the maximum number of interleaved components is four, and the
maximum number of data units within an MCU is ten. The last restriction is
expressed as
                                 N,
                                      ,



                                ＞二 H1V, <10,                              (5.3)
                                 亡＝l


where N5 is the total number of color components. If the above equation is not
satisfied, the data can still be coded, but in a noninterleaved format.




5.4 DESIGN OF QUANTIZATION TABLES
The principle source of compression in DCT-based coders is the quantizer.
JPEG requires an 8 x 8 quantization matrix for each image component to be
compressed; however, multiple components can share the same quantization
matrix. Each element of the quantization matrix can be any integer value
between 1 and 255 and defines the quantization step for the corresponding
DCT coefficients. A quantization matrix with all ones will result in nearly
lossless compression (all the loss will be due to round-off errors). In general,
136                                                              CHAPTER 5




the larger the elements, the bigger the loss and better the compression that can
be achieved.

Aggressive quantization will increase the compression; however, it may also
introduce image artifacts (such as blockiness) and cause image distortion in
the decompressed image. Thus, a good quantization table has to balance the
need for low bit rates with the need for good image quality. The techniques
for the design of quantization tables can be divided into two main classes: (I)
those that are based on human perception and psychovisual experiments, and
(2) those that are based on rate-distortion theory and bit-rate control.



5.4.1   Techniques Based on Psychovisual Experiments

Techniques based on human perception define the elements of the quantization
matrix from visibility thrqsholds for the DCT basis functions so that any loss
due to quantization is perceptually irrelevant. These visibility thresholds are
determined from a series of psychovisual experiments that can be described
analytically as
                                U1. = ？工O+ 恥Lt.                           (5.4)
Given a viewing image u1., a uniform background itO, and a stimulant function
ui, the test person has to determine the value of the variable 'y that yields a
just-noticeable difference between tLO and Ut. In practice, a DCT basis function
is superimposed on a uniform background, and the intensity (功 of the basis
function is increased until it becomes just noticeable.

Lohscheller was among the first to determine visibility thresholds for the 2-D
DCT basis functions. His work led to the definition of the two quantization
tables listed in Annex K of the standard. One table can be used for either
grayscale images or for luminance components, and the other can be used
for chrominance components. For example, the elements of the quantization
matrix for the luminance component are given in (3.29). Use of these tables
is optional; however, experience has shown that they are quite robust and
applicable to a wide range of images and applications.

As mentioned before, quantization tables based on psychovisual experiments
will yield decompressed images of very good quality; however, image quality
or overall compression may not be satisfactory for certain applications. In
T九e.／尸EG 針and口rd                                                                137




those cases, one can tradeoff between image quality and data compression by
uniformly scaling the original quantization table by a quality factor.

For the two quantization tables listed in the standard, a quality factor of one
half will yield decompressed images indistinguishable from the originals. For
additional compression, quality factors from one to five are typical. Figure 5.4
shows the effects on image quality and compression ratio for quality factors
(q) of two and four. At q = 4, the compression ratio doubles; however, there is
significantly more blockiness in the background of the image.




        (a) q= 1, 15.25:1          (b) q = 2, 22.37:1       (c) q =4, 31.24:1



        Figure 5.4     Quality of reconstructed images for different quality
        factors.




5.4.2     Techniques Based on Bit-Rate Control

In contrast to the design techniques that are based on general psychovisual
experiments, techniques based on bit-rate control generate quantization tables
based on the statistical properties of an image. Results from the theory of
human perception may also influence the final design; however, the emphasis
here is on bit-rate control. A simple design technique is described next.

Let r denote the desired average compressed bit rate. (Note that, this is the
bit rate before the Huffman coder.) If we allocate b3 bits per quantized DCT
138                                                                            CHAPTER 5




coefficient, then
                                 1 二二
                                 1七 )  ) b, , 二＝ 1".                                 (5.5)
                                 64 乙日｛日
                                    i= 1 J=l



Given an image, let B be the number of 8 x 8 blocks in the image and let
Yk [i, j] denote the (i, j) output DCT coefficient for the k-th block. Let
                                                                       B
                                                                 ]


                       /-Lt.J = inean(y[i.기）= 言乞y小，jl,                               位6)
                                                                     krl

and let                                                      B
                                             1
                                             .1 V r    r · ,i       ]2
                    升，j= Var(y[i, j}) = ;;      7 . [Ykj',.Jj - 尸i,jJ                (5.7)
                                             0          =H

                                                k=1

denote the mean and the variance for each of the output DCT coefficients. The
key idea of the rate-control method is to allocate more bits to the coefficients
with larger variances. From rate-distortion theory, the optimum bit allocation
is given by

                                    ］工 mn乙
                                             四畔，j                          (5.8)
                              r +

                                                                           j
                           =
                          히2
                                        r         기 1/64 "
                                                 [1i,        j o ,



For images with eight bits per pixel, the maximum range of the AC coefficients
is from -1023 to 1023. Given that this range needs to be divided into 2b, equal
quantization levels, the elements of the quantization matrix are given by

                                  nr. n       2046
                                  Lg [i, JJ = 고二'                                   位9)


For the same perceptual quality, the above procedure generates quantization
tables that yield higher compression ratios than the quantization tables listed
in Annex K of the standard. Recent proposals try to combine the two design
techniques; however, the design of quantization tables is still an open problem.
In a way, the design of quantization tables is related to the very difficult
problem of developing a mathematical model for the human visual system.
The JPEG Standard                                                              139




5.5 ENTROPY CODING
The last processing block in JPEG is the entropy coder. This block improves
overall performance by performing lossless coding on the quantized DCT
coefficients. The entropy coder employed in the JPEG standard is not a
straightforward implementation of the Huffman or arithmetic coding methods
described in Chapter 2; instead, the quantized data are preprocessed by a
run-length coder whose operation will be described later in this section. If the
entropy coder employs Huffman coding, then one or more sets of Huffman
tables (the maximum number of Huffman tables is eight) need to be specified
by the application. There are no default tables, but most applications use the
Huffman tables listed in the standard. JPEG imposes only two restrictions on
the Huffman tables:(1)no codeword may exceed 16 bits, and(2)no codeword
may be the all ones sequence (that is, FF16).

The arithmetic coding option in JPEG requires no external table specifications
since it is able to adapt to the image characteristics. However, for improved
performance, optional statistical tables can be used.

The baseline JPEG implementation uses Huffman coding only. It also restricts
the number of Huffman tables to four: two for the AC components and two
for the DC components. This is not a major constraint, since most applications
operate on luminance-chrominance data and use one set of Huffman tables
for the luminance component and one set of tables for the chrominance
components. This restriction can also be bypassed if one uses noninterleaved
data. In that case, a new set of tables may be loaded before the decompression
of each color component. Details for the baseline Huffman coder are presented
next.



5.5.1    HufTman Coding of the DC Coefficients

Figure 5.5 shows a block diagram of the Huffman coder in baseline JPEG. Let
DCi and DC2_1 denote the DC coefficients of blocks i and i - 1. Due to the
high correlation of DC values among adjacent blocks, JPEG uses differential
coding for the DC coefficients. For 8-bit-per-pixel data, DC differentials
(DCi - DCi_1) can take values in the range [-2,047, 2,047]. This range is
divided into 12 size categories, where the i-th category includes all differentials
that can be represented by i bits. The entries for these categories are the same
140                                                                               CHAPTER 5




                          Size           듸ze    DC Huffman
                                           1>                  m쇠 引ze i amplitude 1
                                                   Table
                  HH>
                          Ta비e
                                                                      dew。
                                                                  DC c。  rd
                                                  amplitude


      AC
               日un-length   H>
                                 value
                                           Size
                                                calculation
                                                    size
                                                              AC Huffman
                                                                                          1
                                                                           뇌 run/siz이 amplitude i
                                                    H日＋




                  Coder                    Tab旭                 Table
                                                      -




                                                                                  AC codeword
                                 run

 OCT coefficients in zig-zag order



                 Figure 5.5          Huffman coding in baseline JPEG.


as the first 12 categories in Table 2.9. Thus, after a table lookup, each DC
differential can be described by the pair (size, amplitude), where size defines
the number of bits required to represent the amplitude, and amplitude is simply
the amplitude of the differential. Given a DC residual value, its amplitude is
computed as follows: if the residual is positive, then the amplitude is simply its
binary representation with size bits of precision; and if the residual is negative,
then we take the one's complement of its absolute value. From this pair of
values, only the first (the size) is Huffman coded.

For example, if the DC differential has an amplitude of 195, then from Table
2.9, size = 8. Thus, 195 is described by the pair (8, 11000011). If the Huffman
codeword for size = 8 is 111110, then 195 is coded as 11111011000011.
Similarly, -195 would be coded as 1111 1000111 100. Huffman decoding
is quite simple. From the input bit stream, we first decode the size = 8
information. Then, the next eight bits in the input bit stream directly give the
amplitude of the DC differential, which we decode according to the value of
its most significant bit.
The JPEG Standard                                                             141




5.5.2    Huffman Coding of the AC Coefficients

For 8-bit pixels, AC coefficients make take any value in the range [-1023,
1023]. As before, this range is divided into 10 size categories, and each AC
coefficient can be described by the pair (size, amplitude). After quantization,
most of the AC coefficients will be zero; thus, only the nonzero AC coefficients
need to be coded.

AC coefficients are processed in zig-zag order. Figure 5.6 shows the
conventional and the zig-zag ordering of elements in an 8 x 8 matrix. Zig-zag
ordering allows for a more efficient operation of the run-length coder.




                                                                     叫




                                                                     H




         回                                       (b) Zig-zag order
           Conventional order



        Figure 5.6    Conventional and zig-zag ordering in an 8 x 8 matrix.


A run-length coder yields the value of the next nonzero AC coefficient and a
run; that is, the number of zero AC coefficients preceding this one. Hence, each
nonzero AC coefficient can be described by the pair (run/size, amplitude). The
value of run/size is Huffman coded, and the value of the amplitude (computed
as in the case of the DC differentials) is appended to that code.

 For example, assume an AC coefficient is preceded by six zeros and has a
 value of-18. From Table 2.9, -18 falls into category 5. The one's complement
 of -18 is 01101. Hence, this coefficient is represented by (6/5, 01101). The
 142                                                                                                                               CHAPTER 5




pair (6/5) is Huffman coded, and the 5-bit value of -18 is appended to that
code. If the Huffman codeword for (6/5) is 1 101, then the codeword for-18 is
1 10101101.

There are two special cases in the coding of AC coefficients, as follows: (I)
The run-length value may be larger than 15. In that case, JPEG uses the
symbol (15/0) to denote a run-length of IS zeros followed by a zero. Such
symbols can be cascaded as needed; however, the codeword for the last AC
coefficient must have a nonzero amplitude. (2) If after a nonzero AC value all
the remaining coefficients are zero, then the special symbol (0/0) denotes an
end of block (EOB).

A Coding Example. Assume that the values of a quantized DCT matrix are
왬 'en (in 기g-zag order) by

                      H
                      9d1 J            lH


                                                                                                    00000000
                                         9




                                                                                                               0 0 0 0 0 0 0
                          n            0
                                       n
                                                         -21           10           -15
                                                            0                        U
                                                                                     Q
                                                                       7
                                                          乙
                                                          n
                                       H




                                                                       工
                                                                       1
                                                                       4
                                                                                                                               中




                         0 0 0 0 0 0       0 0 0 0 0 0                                0 0 0 0 0 0
                                                                                                                                   H




                                                           0 0 0 0 0    0 0 0 0 0
                                                                                                                                       (5.10)


                                                                                                    00000000
                                                                                                           U
                                                                                                           n
                                                                                                           八


If the DC value of the previous block is 40, then DC1 - DC': _1 = 2. This can
be expressed as the (size, amplitude) pair (2, 2). If the Huffman codeword for
size = 2 is Oi l, then the codeword for the DC value is 01 1 10.

Table 5.1 shows the codewords for the AC values. For Huffman codewords,
we use the tables given in Annex K of the JPEG standard document for
luminance AC coefficients (Table K.5). For this example, \ 'e need 82 bits to
encode the AC coefficients and five bits to encode the DC coefficient, for a
total of 87 bits or an average bit rate of 끎 = 1 .36 bits per pixel. If the input
resolution was eight bits per pixel, then the compression ratio is 듦 = 5.88.



5.5.3   Compression Efficiency of Entropy Coding in JPEG

From the discussion on entropy coding of the DC and AC coefficients, we note
that the entropy coder employed in the JPEG standard is not a straightforward
了方e JPEG St口nd口rd                                                    143




     '1
          Value   Run/Size   Huffman Code   Amplitude   Total Bits
144                                                                                 CHAPTER 5




To illustrate the benefits of run-length coding, Figure 5.7 shows for a typical
grayscale image the output bit rate with and without a run-length coder. The


              5.50
                                                      Huffman or arithmetic coder only
              5.00
               印
               4




         m 印 的 駒 的 的


         4 3 31 2 2 t




         =m츠욘쓰me으띤亡口尸a尸＝ O                                                   \\\

                                                                                   \\
                                                      Run-length coder followed     \

                                                                                        \
                                                                                         \

                   仙                                  by a Huffman or an arithmetic coder
                                      뇨
                                      뇨
                                                                                             \



                                             '“丘




                  啣
                                                   “卜卜卜卜小卜卜小小＋                                    ;




                               0.50            1.00                1.50                          2.00
                                           Quality factor



       Figure 5.7            Effects of run-length coding on data compression.

top plot shows the output bit rate when an ideal Huffman or arithmetic coder is
applied directly to the output of the DCT quantizer in Figure 5.1. The bottom
plot shows the output bit rate when the ideal Huffman or arithmetic coder is
preceded by a run-length coder. Bit rates are measured for various settings
of the quality factor used to scale the quantization table. For a quality factor
of one, the bit rate with a run-length coder is nearly four bits per pixel lower
than the bit rate of an entropy coder alone. This is largely attributable to the
efficient run-length representation of the zig-zag ordered AC coefficients. As
the quality factor increases, more of the quantized AC values will be zero, and
as expected, the benefits from a run-length coder are even higher.
                                                                            145
llze JPEG Standard




5.6 JPEG MODES OF OPERATION
                                                          of operation, JPEG
As mentioned before, in addition to the lossless mode
                                                      ssive, and hierarchical.
defines the following other modes: sequential, progre



5.6.1   Sequential Coding
                                                     ion. Image blocks are
Sequential coding is the most common mode of operat
                                                       from top to bottom.
coded in a scan-like sequence, from left to right and
                                                     before the end of the
Transformed and encoded blocks can be transmitted
                                                   tial decoding before it
image Similarly, the decoder may begin sequen
                                                      shows an example of
receives the complete compressed image. Figure 5.8
sequential coding.




                  Figure 5.8 Example of sequential coding.




 5.6.2 Progressive Coding
                                                           sequentially, but the
 In progressive mode, image blocks are also processed
                                                      scan yields the full image
 coding is completed in multiple scans. The first
                                                                scans. This mode
 hut without all the details, which are provided in successive
                                                          during each scan only
 requires that the output of the DCT is buffered so that
                                                                         e coding
            ()rmation from the DCT coefficients is encoded. Progressiv
 partial in1'
                                                       and decod  e the additi onal
 allows a user to preview a rough version of an image
                                                             that are allow for
                                                                            ed
 information only if necessary. There are two procedures
                                                               ximation.
 progressive coding: spectral selection and successive appro
  146
                                                                       CHAPTER 5




  Consider 8 x 8 blocks of quantized DCT coefficients
                                                      as shown in Figure 5.9.
  We view each block as a three-dimensional(3-D)
                                                 object, where depth denotes



           zero
        frequency




                                                                             LSB


                                 highest                         MSB
                                frequency
                    (a) Spectral selection      (b) Successive approximation


            Figure 5.9 Description of progressive coding in JPEG.

 the arithmetic precision of the quantized coefficients. Under
                                                                  spectral selection,
each block is divided into frequency bands,and each band
                                                              is transmitted during
a different scan. For example, in Figure 5.9a, the DCT
                                                            output is divided into
four scans. Scan 1 includes the DC coefficient and the
                                                         first two AC coefficients
(counted in zig-zag order), Scan 2 includes the next seven
                                                                   AC coefficients,
Scan 3 includes another 11 AC coefficients, and Scan
                                                         4 includes the remaining
AC coefficients. For most images, most of the inform
                                                            ation is contained in
the DC and the first few AC coefficients. Thus,
                                                     encoding and transmission
of the first scan of coefficients will provide adequate
                                                          information for a rough
preview of the image. Encoding and transmission of
                                                         the remaining scans just
adds progressively additional detail.

Figure 5.10 shows an example of progressive codin
                                                          g based on spectral
selection. Figure 5.lOa shows the output image after
                                                        decoding only the DC
coefficients. The image is rather blocky, but we can
                                                     still get a rough preview
of the image. Figure 5.lob shows the output image after
                                                             decoding the DC
and the first three AC coefficients. The diagonal edges
                                                          of the house are still
blocky. Figure 5.l0c shows the decoded image at full spectr
                                                             al resolution.

Under successive approximation,given a frequency band,the
                                                            DCT coefficients
are divided by a power oftwo before encoding. This schem
                                                         e allows the encoder
                                                                            147
The JPEG Standard




            (a) DC only.     (b) DC F出Us 伽St three      (c) Full res이ut向n
                               AC components.



      Figure 5.10 . Example of JPEG,progressive coding using, spectral
      selection. (a). vecouing or trie UL coernciern onty; 四) ueco; a9
                                                               cients cj
      or tne vu anu me rirst tnree (in zig-zag oruerJ iu coein
      decoded image at full  spectr al resolution.


                                                           preview, and the least
to transmit the most significant bits first, for a rough
                                                          For example, in Figure
significant bits later, for decoding at full resolution.
                                                      ssive approximation scans.
5.9b, the DCT output is encoded using three succe
                                                         the same power of two
In the decoder, the coefficients are scaled back by
                                                      schemes may be combined
before computing the IDCT. The two progressive
 or used separately.



 5.6.3 Hierarchical Coding
                                                              as a sequence of
 In hierarchical mode, each image component is encoded
                                                                eo叱ma! image
 夕ames. The 佈st fr帥이s usually a low妃so恤帥 ver如nofth
                                                         ential frames 比tween
 (possibly downsampled). Subsequent frames are differ
                                                        nce reconstructed corn-
  source components (possibly downsampled) and refere
                                                       using either lossy JPEG
  ponents (possibly upsampled). Frames can be coded
                                                                  lossless JPEG
  or lossless JPEG. The two modes can be mixed only when
                                                               ss.  Hierarchical
  is used for the last stage of DCT-based hierarchical proce
                                                               ts. For example,
  coding is useful when there are multiresolution requiremen
                                                         ys on workstations and
  an application may support both high-resolution displa
  low resolution displays on personal computers.
   148
                                                                       CHAPTER 5




  Figure 5.11 shows an example of a three-level hierarchical coder.
                                                                         From the


                 x4
                                                                  x뇨




                                                                            x,
                          Encoder                          Decoder



                 Figure 5.11    Three-level hierarchical coder.

original image X, we generate two subsampled versions: X2,
                                                             where the image
is subsampled by a factor of two on both dimensions; and
                                                         X4, where the image
is subsampled by a factor of four on both dimensions.
                                                      Note that, subsampling
may also be preceded by a low-pass filtering operation
                                                          to reduce aliasing
effects. JPEG poses no requirements on these preprocessin
                                                          g operations.

The encoded image consists of three frames: S1, S2, and S3.
                                                                   Frame Si is
simply the X4 image compressed. Using only Si, the decoder can extrac
                                                                              t a
low-resolution estimate of the original image (X). S2 (unco
                                                                mpressed) is the
difference image between X2 and an estimate of
                                                      X2 (X) after upsampling
X4 by a factor of two. Using Si and S2, the decoder can extrac
                                                                    t a medium
resolution estimate of the input X (X',,,). Similarly, S3 (unco
                                                                mpressed) is the
                                                                           149
The JPEG Standard




                                                          on X2 and X4. The
difference image between X and an estimate of X based
                                                         X.
reader can verify that, under lossless compression, X' =
                                                       The first image (a) is
Figure 5.12 shows an example of hierarchical coding.
                                                    . Images (b) and (c) are
the original image shown at full resolution (200 dpi)
                                                     factors of two and four,
subsampled versions of the original (subsampled by
respectively).




                                                       a   (C)
                                               (b)
                         (a)
      Figure 5.12. Example of hierarchical coding. (a) Origin    al; (b)
                 b y a tactor Or two;(C)subsa mplea ny a tactor or tour.
      sutsampiea


                                                                   g processes
 To summarize,the essential characteristics of the main JPEG codin
 are given as follows.


   1. Baseline Process
                                                                        .
           Coding: DCT-based, sequential, one to four color components
           Resolution: eight bits per pixel.
           Huffman coding; two AC and two DC tables.
      .    Interleaved and noninterleaved scans.

   2. Extended DCT-based Process

           Coding: DCT-based, sequential or progressive.
   150
                                                                     CHAPTER 5




               Resolution: 8 or 12 bits per pixel.
               Huffman coding or arithmetic coding; four AC and four
                                                                       DC tables.
        .     Interleaved and noninterleaved scans.
   3. Lossless Process

              Coding: Predictive, sequential.
              Resolution: From two bits per pixel to 16 bits per
                                                              pixel.
              Huffman coding or arithmetic coding; four DC tables.
        1     Interleaved and noninterleaved scans.
   4. Hierarchical Process

              Coding: DCT-based or lossless process.
              Multiple frames (non differential and differential).
        1     Interleaved and noninterleaved scans.


JPEG has been developed for the compression of still-images
                                                             ; however, the
proliferation of low-cost hardware for JPEG has led to
                                                        the development of
an additional mode of operation for video sequences: motio
                                                            n-JPEG. Under
motion-JPEG, each frame of a video stream is compr
                                                      essed independently
using the baseline JPEG algorithm. However, there is no
                                                        standard syntax for
motion-JPEG coded streams, and encoded data may not
                                                      be able to be decoded
across different platforms.




5.7 IMPLEMENTATION ISSUES
The specific implementation of the JPEG standard depen
                                                           ds on the application
requirements and whether a software or a hardware implementa
                                                                tion is adopted.
In this section, we will address several issues relevant to the
                                                                implementation
of the baseline JPEG standard.



5.7.1       Hardware versus Software Implementation

Using a scaled DCT,such as the one described in Chapter 3, JPEG
                                                                compression
of a 640 x 480 RGB image requires close to 23 million operat
                                                               ions. Thus, a
The JPEG Standard                                                            151




typical general-purpose processor can compress such an image in less than a
second.

Computation of the DCT requires close to 45 percent of the overall time.
In Chapter 3 we described several algorithms for computing the 8 x 8
DCT and IDCT. In a software implementation, the scaled DCT method of
Winograd and Feig, which requires 80 multiplications and 464 additions, is a
good choice. A scaled DCT method is particularly advantageous for JPEG,
since the quantization tables are fixed for the entire image. In a hardware
implementation, a DCT method that has a more regular dataflow, such as the
Chen DCT, is preferable.



5.7.2 IDCT Complexity

An 8 x 8 IDCT requires the same number of operations as the DCT. However,
for most JPEG compressed images, the 8 x 8 block that is input to the IDCT
is quite sparse. In a software implementation, the sparseness can be exploited
to realize a more efficient evaluation of the IDCT. For instance, in a smooth
region of an image, one would find that the corresponding DCT blocks have
all AC coefficients set to zero. For such blocks, the IDCT is simply a scaled
version of the DC coefficient that is copied to all the 64 locations in the block.
Similarly, in regions of low activity, one may only need to compute simpler 2
 x 2 or 4 x 4 IDCTs. The appropriate IDCT can easily be determined from the
 output of the Huffman decoder.



5.7.3    Arithmetic Precision Requirements

For eight bits per pixel data, the output of the 8 x 8 DCT will yield DCT
coefficients that have a dynamic range between -1,023 and 1,023. Determining
the requirements for arithmetic precision in the DCT requires a careful study
of the flowgraph associated with the specific DCT method. In general, using
12 bits of precision for the constants in the DCT flowgraph and 16 bits
of precision for all arithmetic operations yields the same output quality as
32-bit floating-point arithmetic. In Chapter 7, we provide a standard testing
procedure for determining the accuracy of the IDCT, assuming that the DCT
 output is not quantized.
152                                                                CHAPTER 5




5.7.4    JPEG Coding Tables

JPEG specifies no default coding tables; however, most implementations use
 the example tables described in the Annex K of the ISO document. Designing
custom Huffman tables is relatively easy. One can use either the techniques
described in Chapter 2 or a similar method described in Annex K of the
standard. However, the design of custom quantization tables is not trivial. In
a previous section, we described a design method based on bit-rate control
before the entropy coder. Recently, Ratnakar and Feig have proposed the
design of quantization tables that are optimum in a rate-distortion sense; that
is, if the user specifies the desired rate for a specific image, say, 0.5 bits per
pixel, then this design method will provide the quantization tables that achieve
this rate, provided that a custom Huffman table is used. Note that, JPEG does
not have an explicit rate-control; hence, this design method is a useful tool for
providing rate-control within JPEG. However, this design method is image
specific.

For a typical grayscale image, Figure 5.13 shows the effects of custom coding
tables on the output bit rate of a JPEG coder. Several observations can be
made from these plots.


    Using the example quantization tables at compression ratios around 40:1
    (0.20 bits per pixel for the 8 bits per pixel grayscale image), custom
    Huffman tables yield nearly 1 dB performance improvement over the
    example Huffman tables. Performance gains greater than 0.5 dB usually
    yield visible differences between the corresponding reconst기cted images.
    At compression ratios around 10:1, custom Huffman tables are not
    beneficial.

    Using the example Huffman tables, custom quantization tables yield
    better performance only at low compression ratios. At high compression
    ratios, there is significant mismatch between the actual statistics of the
    DCT output and the assumed statistics for the design of the example
    Huffman tables. Hence, at least for grayscale images, it seems that there
    is no benefit using custom quantization tables with the example Huffman
    tables.

    The best performance is attained when both custom quantization tables
    and custom Huffman tables are used. In this case, there is a 1 dB
    to 2 dB performance improvement compared to using the example
The JPEG Standard                                                                                  153




         1.00

         0.90
                                Exan巾沌quan似카幻n
                                and Huffman tables
         0.80                                                             / // 1
                                                   JPEG standard)
                                                       -             .


                                              K,
                                (Annex
         0
         0 나／

                        Example ciuantizat幻n                        ,/
         0   0          table, custom r4uttman                 \"
           nb
                        tables                                               r>1
         0   0
                                                                             R(D）야川mized
                                                           /                 quantization table,
       승즘＞石Vm늪工
           二U                                                                examp旭 Hu伽nantables


         0.40                                                  R(D) optimized quantization
                                         /'
                                                   <H-         table, custom HUffman
                                                               tables
         0.30
                           /

         0.20

         0.10
                24.00   26.00             28.伏）       30.00              32.00     34.以   36.00

                                                    PSNR (dB)



     Figure 5:1.3 JPEG coder performance for example and custom
     coding tames.


    tables. However, this approach requires the redesign of the tables on an
    image-by-image basis. It also requires more than one pass through the
    encoding process, thus, increasing the computational complexity of JPEG
    compression; the decompression complexity is not affected since table
    descriptions are part of the compressed bit stream.


The above data is for a grayscale image. For color images, SNR or PSNR
is not necessarily the best measure of perceptual image quality. From our
experience, using the example Huffman tables, custom quantization tables can
yield better performance even at high compression ratios.
   154
                                                                       CHAPTER 5




  5.7.5    Color Conversion and Display Considerations

  For image compression of RGB images, the RGB to YCbC
                                                               r color transfor-
  mation may represent up to 39 percent of the overall comp
                                                               ression process.
  Similarly, in many applications, there is a need to decom
                                                               press a YCbCr
  JPEG image and display it as an RGB image. Furthermor
                                                                e, the Cb and
  Cr components are usually half the resolution of the Y
                                                           component; hence,
  during the color conversion process, the Gb and Cr comp
                                                            onents have to be
  upsampled to facilitate the conversion to RGB. Upsamplin
                                                           g, color converting,
  and displaying of an image may represent 33 percent of the
                                                                 computational
 complexity of the JPEG decompression
                                             process. Color conversion using
 lookup tables can be used to speed up the process. In
                                                         recent years, there is
 a trend towards implementing the color conversion
                                                     and upsampling functions
 in the display system hardware, and thus eliminating the overh
                                                                ead associated
 with the display.



 5.7.6    The JPEG Compressed Data File Format

 The JPEG standard specifies an interchange format
                                                     so that compressed images
 can be reconstructed reliably. However, the interc
                                                    hange format only provides
 information pertaining to the image dimensions, resolu
                                                             tion of each of the
 components that make up the image, and the quantization
                                                               and Huffman code
 tables that are used in the compression process.
                                                     JPEG does not explicitly
 specify the color space that is used in compression.
                                                          In recent years, a de
facto standard, referred to as the JPEG file interc
                                                     hange format (JFIF), has
evolved and is supported by many image processing applic
                                                              ations. This format
is a superset of the JPEG interchange format and suppo
                                                          rts either grayscale or
YCbCr images. The bit-stream syntax of JFIF also provid
                                                              es for inclusion of
a thumbnail RGB representation of the image; this can
                                                          be used for browsing
and cataloging pu下）oses.




5.8      JPEG EXTENSIONS AND APPLICATIONS
Part 3 of the JPEG standard (ITU-T Recommendation T.84
                                                                or ISO/fEC 10918-
3) specifies requirements and guidelines for encoding and decod
                                                                      ing extensions
to the processes defined in Part I . It is currently a draft intern
                                                                    ational standard
The JPEG Standard                                                             155




and is expected to become an international standard by the end of 1995. There
are four major extensions defined in this part: variable quantization, selective
refinement, tiling, and a new image-interchange format.



5.8.1   Variable Quantization

In lossy JPEG,the amount of loss or compression is controlled by the elements
of the quantization tables. JPEG allows quantization tables to be redefined
prior to the start of a new scan, but not within a scan. The variable quantization
extension introduces a quantizer scale factor that may be used to scale the
original quantization matrix on a block-by-block basis. This scale factor may
be coded in the compressed bit stream at the start of any 8 x 8 block. This
extension does not apply to the baseline JPEG process.

This extension allows for greater control on image quality and compression
ratios. For example, in an image with both text and graphics, one may use
different scale factors for blocks characterized as image and different scale
factors for blocks characterized as text. Since text regions and image regions
tend to have different statistical properties, the different scale factors in these
areas should allow for more efficient coding of the image.



5.8.2 Selective Refinement

This extension allows for the selective refinement of parts of an image. The
three different types of selective refinement are hierarchical, progressive, and
component.

Hierarchical selective refinement is used in the hierarchical mode of operation.
It allows the encoder to specify which areas of the image are coded in greater
detail than the rest of the image. In the decoder, the differential frames are
then added only to those specified areas.

Progressive selective refinement is used in the progressive mode of operation.
As in hierarchical refinement, the encoder may supply additional DCT data
only for specific regions in the image.
 156                                                             CHAPTER 5




 Component selective refinement may be used in all modes of operation. It
 allows the encoder to specify that a certain region of the image uses fewer
 color components than the total number of components defined in the frame
 header. This extension could be used for the more efficient representation of
 images that combine both grayscale and full color regions.



5.8.3    T小ng

 The tiling extension allows an image to be subdivided into subimages, also
 called tiles. It can be used to represent images larger than 65,535 pixels on
 a side, for random access within parts of an image, or for more efficient
 compression. In simple tiling, the image is divided into an array of non-
overlapping rectangular tiles. All simple tiles have the same size, except
maybe for the tiles at the right and the bottom sides of the image. These
tiles must have the same component identifiers, sampling factors, and entropy
coders; however, each tile may be coded with a different quantization table.
Pyramidal tiling allows multiple resolution versions of the same image to be
stored in the same compressed bit stream. This feature allows access to lower
resolution versions of a larger image. Composite tiling is the most complex
tiling method. Complex tiles may overlap and have different sizes; however,
they still need to have the same component identifiers. It is expected that most
of the future applications will only support simple tiling.



5.8.4   The Still-Picture Interchange File Format (SPIFF)

SPIFF is yet another image file format developed for the efficient interchange
of files containing image data. It is more comprehensive than the JFIF format,
but still not as complex as some other image file formats, such as TIFF. It is
backward compatible with JFIF, but in addition to grayscale and color JPEG
images, it also supports bilevel images and many of the facsimile compression
algorithms.
刀ie JPEG St마idard                                                           157




5.8.5   The Color Facsimile Standard

In November of 1994, ITU formally approved extensions to the Group 3 and
Group 4 facsimile standards for the transmission of continuous-tone images.
The new color facsimile standard uses the Cifi (1976) L5a5b5 (CIELAB) color
space for the representation of color images and the baseline JPEG algorithm
化r data co呻res計on.

In the baseline implementation of the color facsimile pipeline, a scanned 24-bit
RGB image (scanned at 200 dpi) is first translated into the CIELAB color
space using the standard Cifi D50 illuminant. The gamut range is restricted to

                              L'    = [0, 100],                          (5.11)
                                '   = 卜85,85],                           (5.12)
                              6'    = [-75,125].                         (5.13)

This color space was chosen because it provides for a more flexible, relatively
uniform, and device-independent color specification. It also enables the
recei比r to reproduce a hard c叩加f the or增nal image w咐lout ambigi血y.

After color transformation, the chroma components (as and b5) of the image
are subsampled by a factor of two in both the horizontal and the vertical
directions. The subsampled image is coded using the JPEG algorithm (lossy
or lossless), and the compressed bit-stream is transmitted using the st카ldard
Group 3 or Group 4 facsimile protocol. At the receiver, after Group 3 or Group
4 decoding, the image is decompressed, color transformed, and printed on a
color printer.

Optional features of the standard allow for higher spatial resolutions, no color
subsampling, higher precision (12 bits per pixel), and custom color gamut
range.




5.9     TO PROBE FURTHER
The JPEG standard [83] is published in two parts. Part 1 sets requirements and
guidelines for coding and decoding and describes the interchange format. Part
2 describes compliance tests for the processes described in Part 1. A new part
158                                                             CHAPTER 5




(ISO/IEC 10918-3 or ITU-T Rec. T.84) will provide extensions to the coding
processes defined in Part 1.

A good source for the JPEG standard is the book by Pennebaker and Mitchell
[158]. The book includes a complete copy of the ISO document and provides
additional implementation details. For a concise overview of the standard, we
also recommend an excellent tutorial overview by Wallace [191].

Experiments for determining visibility thresholds for the DCT basis functions
using the YCbCr color space are described by Lohscheller and Franke in [124]
and [1251. Similar experiments for the RGB color space are presented in
[159]. The optimal bit allocation for quantization tables based on rate-control
theory is described in the textbook by Jayant and Noll [931. An adaptive
coding scheme based on the same principles is also described by Chen and
Smith [32]. In [37], de Queiroz and Rao weight the image statistics with
a matrix that contains spatial information about the human visual system
(HVS). Recently, quantizer design methods optimal in a rate-distortion sense
have been developed in [168] and [169]. The techniques developed here can
provide a fixed-rate implementation ofJPEG even though the JPEG standard as
developed does not include explicit rate-control. In many cases, a compressed
image will be decompressed, halftoned, and printed. Recently, Vander Kam
et al.[96] were able to improve the compression of grayscale images that will
be printed by taking into consideration both the sensitivity of the HVS and the
frequency characteristics of the printer's halftoning algorithm.

Many imaging applications currently support the JPEG standard. However, to
facilitate the interchange of JPEG compressed data across applications, there
is a need to develop a file format. The TIFF format is widely used in the
imaging community and has provisions for describing a JPEG bit stream. For
the simpler JFIF format details can be found in [68].

The section on the JPEG extensions is based on a recent article by Lee [112].
The details of the color facsimile standard are defined in new Annexes to the
facsimile standards documents. For Group 3, Annex E of ITU-T T.30 [88]
specifies new entries in the DIS and DCS frames of the facsimile communica-
tion protocol and Annex I of ITU-T T.4 [89] describes the appropriate JPEG
syntax and JPEG application markers.
The JPEG Standard                                                    159




There are numerous software and hardware implementations of the baseline
JPEG standard. Sites with public domain JPEG coders are given in Appendix
B. Hardware implementations of the JPEG standard are discussed in a later
chapter.
                                                                       6
    THI二 八4PEG VIDEO STANDAI之DS




6.1 INTRODUCTION
Advances in digital video technology and storage have made it possible to
use digital video into a number of multimedia applications. In 1988, in
response to a growing need for a common format for coding and storing digital
video, ISO established the Moving Pictures Expert group (MPEG) with the
mission to develop standards for the coded representation of moving pictures
and associated audio information on digital storage media. MPEG, formally
known as group ISO-IEC/JTCI SC291WG11, completed the first phase of
its work in 1991 with the development of the ISO standard 11172, Coding
of moving pictures and associated audio - for digital storage media at up to
about 1.5 Mbit/s. This standard is also known as MPEG-I.

In 1990, MPEG started the second phase of its work, namely, to develop
extensions to MPEG- I that would allow for greater input-format flexibility,
higher data rates (as needed by high-definition TV), and better error resilience.
That work led to the ISO standard 13818 (orI띠-T Recommendation H.262),
Generic coding of moving pictures and associated audio. This standard is also
known as MPEG-2. MPEG has already started working on developing new
 coding standards for very low bit rates. This activity is known as MPEG-4
 and the standard is expected to be defined by 1998. All MPEG standards are
 generic; that is, application independent. They do not specify the operations
 of the encoder. Instead, they specify the syntax of the coded bit stream and the
 decoding process. Thus, they provide enough flexibility in the specifications
 so that different vendors can include specific optimization elements.
 162                                                             CHAPTER 6




 The MPEG standards are published in four parts: systems, video, audio, and
 conformance testing. The systems part specifies the system coding layer of the
 standards and defines how data, audio, and video streams can be multiplexed.
 For example, in MPEG-I, the systems layer provides sufficient information
 for synchronization of multiple video streams, random access to the data, and
 buffer management. In MPEG terminology, the video, audio, and data streams
 are generically referred to as elementary streams. Note that, in a system layer
 stream, more than one audio, video and data stream can be included. A detailed
 discussion of the system stream is beyond the scope of this book.

The video part specifies the coded representation of video data and a decoding
process for reconstructing MPEG coded pictures. Audio is an integral part
of the MPEG standards. The audio part specifies the coded representation
of audio coded data and a decoding process. Finally, the fourth part of the
standards provides guidelines for conformance testing.

In this chapter, we cover only the video part of the MPEG standards. The
MPEG audio standards are covered in a later chapter, together with other
algorithms for audio coding and compression.




6.2 THE MPEG-i VIDEO STANDARD

6.2.1   Preliminaries

The MPEG-i video coding algorithm is a lossy compression scheme that can
be applied to a wide range of input formats and applications; however, it has
been optimized for applications that support a continuous transfer bit rate of
about 1.5 Mbits/s (such as a CD-ROM).

MPEG-I uses deliberately the term picture and not frame because it does not
recognize interlaced sources. In interlaced video, each frame is comprised of
fields, namely, a top field and a bottom field. Within a frame of interlaced
video, scanlines from the two fields are interleaved (Figure 6.Ia). Note that,
spatially adjacent scanlines are not temporally adjacent. For example, at 30
fps, the adjacent scanlines are 計th of a second apa比 In progressive (or
noninterlaced) video there is no notion of a field. Unlike interlaced video,
spatially adjacent scanlines are also temporally adjacent. A frame begins from
                                                                                                                                                 163
The MPEG Video Standards




                                                            to the bottom of the
the top left corner and continues through successive lines
                                                             that generated by a
frame (Figure 6. I b). In MPEG- I, interlaced video, such as
                                                       ed coding format before
TV camera, may have to be converted to a noninterlac
                                                        ied within the MPEG- I
coding. This process of scan conversion is not specif
standard.

                        f                          I
                                                          Bottom
         T야）
                                                          field
            field       1
                                                   !
                        1



                                             Spatial-domain representation




                                                                                                                               口 口 口 口 口 口 口 口
                                                              Lines




                                                                        口 口 口 口 口 口 口 口   口 口 口 口 口 口 口 口    口 口 口 口 口 口 口 口
               Lines8       口        口
                                口            口
                            口
                                 口
                                         口
                                             口                                                               믐
                            口            口

                            口
                                 口
                                         口
                                             口
                                                                                                             믐
                                 口           口

                                lit PS   4        time                卜 h/ips 寸                                                time
                            P

                                                 Time-domain representation

                        (a) Interlaced scanning                       (b) Progressive scanning



                                                                   es.
              Figure 6.1 Interlaced and progressive scanning schem


                                                       pment of the MPEG-I
 There were two key requirements during the develo
                                                           m-access capability.
 standard, need for high compression and need for rando
                                                       ess but cannot meet the
 Intraframe coding alone is best suited for random-acc
                                                    confli  cting requirements,
 requirements for high compression. To meet these
                                                      interframe coding tech-
 MPEG resorted to a combination of intraframe and
                                                         it proposed using both
 niques. Furthermore, to improve the compression ratio,
 predictive and interpolative coding schemes.
                                                                                                            ing:
  Compression functions within MPEG include the follow
 164                                                            CHAPTER 6




   1. sample rate reduction in the spatial and temporal domains of both the
      luminance and chrominance components,

  2. block-based DCT for the intraframes and interframes,

  3. block-based motion compensation for predictive and inte叩olative inter-
     frames, and

  4. Huffman coding for the lossless compression of motion vectors and the
     quantized DCT coefficients.


For a picture size of 352 x 240 pixels, at 12 bits per pixel and a picture rate
of 30 pictures per second, MPEG-I compresses the 30.4 Mbits/s bit stream
down to 1.15 Mbits/s. For this compression ratio of 26:1, the picture quality
can be better than that provided with the analog VHS representation. We will
describe the compression method in detail later in this chapter.


The source input format

 The MPEG-i bit-stream syntax allows for picture sizes of up to 4,095 x
 4,095 pixels; however, many of the applications using MPEG-I compressed
 video have been optimized for the SIF (source input format) video format,
 which is a simple derivative of the CCIR 601 format for video frames in
 digital television. According to CCIR 601, a color video source has three
color components: a luminance component (Y) and two color-difference or
chrominance components (Cb and Cr). There are two options for the CCIR
601 spatial resolutions. The first option (for NTSC television systems) uses
525 lines per frame at 60 frames per second. The luminance frame has 720
 x 480 active pixels, and each of the chrominance frames has active 360 x
480 pixels. This is referred to as the 4:2:2 subsampling format. The second
option (for PAL television systems) uses 625 lines per frame at 50 frames per
second. Here, the luminance frame has 720 x 576 active pixels and each of
the chrominance components has 360 x 576 active pixels. To accommodate
compressed rates as low as 1.5 Mbits/s, MPEG-I defines (but does not require)
the source input format. SW sequences have a luminance resolution of 360
><240 pixels per picture at 30 pictures per second or 360 x 288 pixels per
picture at 25 pictures per second. In both cases, the resolution of the chroma
components is half of the luminance resolution in both the horizontal and the
vertical dimensions. This is referred to as the 4:2:0 subsampling format. SW
The MPEG Video Standards                                                     165




pictures can easily be derived from a CCIR 601 frame using filtering and
subsampling.

In MPEG-i, the YCbCr color components are always interleaved. A mac-
roblock is defined as the minimum coded unit and consists of four 8 x 8
blocks of luminance, one 8 x 8 block of Cb, and one 8 x 8 block of Cr (Figure
6.2). The maximum dimension of a macroblock is 16 pixels. Each picture is


                                                4口mmm中- N -c-


                                                            Cb
                  -
                          --


              '=1 I I          8         8
              1b 1- 4--4            기．
                                     戶
                I그그 Cu씨 L
                      V        Cb     Cr                               수
                                                                       M/2
                                                                       寸
                 4:2:0 macr야升ock

                                                           ＜卜 N/2-D-




            Figure 6.2              Definition of a macroblock in MPEG-i.

divided into a series of macroblocks, from left to right and from top to bottom.
This requires that the horizontal and vertical resolutions of each picture are
multiples of 16. If they are not, then the coder adds padding pixels to the
right or at the bottom of each picture that are later discarded by the decoder.
Since the horizontal resolution of 360 pixels in a SIF picture is not divisible
by 16, one can duplicate the last pixel in each line eight times so that the total
number of pixels per line is 368. In an alternative implementation, one can
discard the leftmost four pixels and the rightmost four pixels from each line;
then the remaining picture has 352 pixels per line and is called the significant
pixel area. Table 6.1 summarizes the picture characteristics for the CCIR 601,
the SW, and the significant pixel area formats.

MPEG-i provides a great degree of flexibility; however, it would be unrealistic
to expect that every MPEG decoder could support all coding options. Thus,
MPEG-i defines the constrained parameters bit stream; that is, the bit stream
that every MPEG-i compatible decoder should be able to support. Table 6.2
shows the parameters of a constrained bit stream; however, conforming to
these sets of parameters is still not a requirement of the standard. From Table
166                                                            CHAPTER 6




                  Picture Rate (Hz)        30         25
                  CCIR 601
                  Y                    720 x 480   720 x 576
                  Cb, Cr               360 x 480   360 x 576
                  SIF
                  Y                    360 x 240   360 x 288
                  Cb, Cr               180 x 120   180 x 144
                  Significant Pixel Area for SIF
                  Y                    352 x 240   352 x 288
                  Cb, Cr               176 x 120   176 x 144


      Table 6.1 Picture sizes for the CCIR 601, SIF, and significant
      pixel area formats.


            （노di叩 P針帥祀ter               Maximum Value
            Horizontal picture size     768 pixels
            Vertical picture size       576 lines
            入4acr이)IOCkS                396
            Pixel rate                  396 x 25 macroblocks/s
            Picture rate                30 pictures/s
            Range of motion vectors     +/- 64 pixels
                                        (half-pixel resolution)
            Size of input buffer        327,680 bits
            Bit rate                    1,856 kbits/s


      Table 6.2     Coding constraints for a constrained parameters bit
      stream.


6.2, the constraint on the pixel rate (396 x 25 macroblocks/s) restricts the
picture size to approximately 352 x 288 pixels, which is the significant area
of a SIF image at 25 Hz.
The MPEG Video Standards                                                     167




6.2.2   Picture Types

Some of the common operations on video streams include video editing,
random access, and searches. Support of these operations often conflicts with
the requirements for high compression. MPEG-I defines four different types
of pictures that offer the flexibility to trade off between coding efficiency and
random access.

Intra-pictures (I-pictures) are compressed using intraframe coding; that is, they
do not reference any other pictures in the coded bit stream. They provide for
fast random access, but offer only moderate compression. This situation is
similar to applying lossy JPEG on individual pictures. Predicted pictures (P-
pictures) are coded using motion-compensated prediction from past I-pictures
or P-pictures. The compression for P-pictures is better than for I-pictures, and
P-pictures can be used as reference points for additional motion compensation.
Bidirectionally predicted pictures (B-pictures) provide the highest degree of
compression. They are coded using motion-compensated prediction from
either past and/or future I-pictures or P-pictures. Since B-pictures are not
used in the prediction of other B or P-pictures, such pictures can accommodate
more distortion and hence yield more compression than I- or P-pictures. DC-
coded pictures (D-pictures) are similar to I-pictures; however, only the DC
coefficients from the DCT output are present. D-pictures cannot be mixed
with other picture types and are used mainly for fast searches. D-pictures are
n아 used in 入4PEG-2.

Figure 6.3 shows the relationship among the three main picture types in a
video sequence with eight pictures. Pictures P1 and P8 are I-pictures, pictures
p4 and p7 are P-pictures, and the remaining are B-pictures. In this example,
p3 is coded using motion-compensated prediction from p and p.s. There is
no requirement to use either P-pictures or B-pictures in the MPEG bit stream.
The size of I-, P-, and B-pictures for a typical video sequence coded at SIF
resolution and at 1.15 Mbits/s is shown in Figure 6.4. Note that, B-pictures
require significantly fewer bits than either I-pictures or P-pictures. Increasing
the number of B-pictures between an I- and a P-picture may not lead to better
compression due to a drop off in temporal correlation as the distance between
a B-picture and the corresponding I- and P-pictures increases. In the next
section, we provide a brief overview of the encoding process.
168                                                                CHAPTER 6




        Figure 6.3 Example of inter-dependence among I-, P-, and B-
        pictures in a viueo sequence.


6.2.3     Video Encoder

The MPEG standards do not define an encoding process. They only specify
the syntax of the coded bit stream and the decoding process. Based on these
requirements, Figure 6.5 shows the functions that need to be executed by a
typical MPEG encoder.

Preprocessing. The encoding process usually begins with some preprocessing.
This may include color conversion to YCbCr, format translation (interlaced
to progressive), prefiltering, and subsampling. None of these operations is
specified in the standards.

Motion estimation and compensation. After preprocessing, the encoder
selects the coding type for the input picture. I-pictures require no motion
estimation or compensation. Each macroblock is DCT coded, and the DCT
coefficients are quantized, coded using a variable-length coder (VLC), and
stored into the output buffer. Within each macroblock, processing is performed
on 8 x 8 blocks. In applications requiring constant bit rate, a buffer regulator
may adjust the quantization matrix so that the rate of the compressed bit stream
is relatively constant. For variable bit-rate applications, the regulator function
may not be needed.

The quantized blocks are also inverse quantized (Q기 and transformed into
the spatial domain by an inverse DCT. This operation duplicates the behavior
of the decoder and yields a copy of the encoded picture as it will be seen by
the decoder. That copy is then stored into local memory and will be used
The MPEG Video Standards                                                                169




            160
                             F키cture           Average size         小1 나加仙res
                              1                 156 kbits           m如’ P-pictures
            140                                                     -   B-pictures
                              P   "              62 kbits
                              B                  ] 5 kbits
            120



         0     0     0
         0     8

         l
                     b
                     n

         戶m尸즈芭mN而판그尸으a




              40


              20


                 0
                                       1
                                       1
                                           卄
                                           1




                                                               付       仰                h
                                                                                        11
                                                                                         n
                                                                                         1
                         恤   0 내               0       1 U    0
                                                              0 d
                             0 n                         0
                                                         네
                              仄口 e
                                 뱌
                                                日
                                                         0
                                                         C    0 아              150.00
                                 d
                                 디              b        n
                                                         e    0 아




     Figure 6.4 Example . of bit .distribution among I-, P-, and, B-
                                                        are couea in
     만얀쁘黛，쯔k첵＼凞犁J三 Co配a oit 飢ream. rictures
      ltq기사／bbrDbnj1jrbDsequence.



for future predictive coding. In effect, this operation allows the encoder to
monitor the quality of the transmitted image so that it does not diverge from
the original signal. Since the VLC operation is lossless, there is no need to
include the VLC unit in the feedback path.

If the input is coded as a P-picture or a B-picture, then the encoder does not
code the picture macroblocks directly. Instead it codes the prediction errors.
In 入1PEG termin이ogy, 仕us is referred to as in油升ame predicti比 口ding. For
P-pictures, this process is explained in Figure 6.6. For each macroblock in the
current picture, the motion estimator yields the coordinates (motion vector)
170                                                                                              CHAPTER 6




                                                                 Regulator

                                                                        寸
        Frame                                                    Quantizer                       VLC
                      <> +
                                              0CT   11令
                                      mH>
                  m
                                                                                                Encoder
                                                                             \d>
       Memory

          수                                                             寸                         1
                                                                        （긔
                                                                    (
         Pre-                                                                                   Buffer

                                                                        寸                         1
      口ocessing




                        m
                        Em七 m＞ 듕乞m左
          오                                                        IDCT
                                                                                                Output
        Input                                                           寸

                                                                                   mb乞m> CO등E
                                                                        寸
                                                Motion            Frame
                                                           <mH
                                              Compens帥on         Memory


                                                M아幻n
                                                    수
                                               E帥mation



                Figure 6.5                  Block diagram of an MPEG encoder.


of the macroblock that best matches its characteristics in a search area in the
past picture. The two macroblocks are subtracted, and their difference is then
DCT coded. Any of the block-based motion estimation methods described in
Chapter 4 can be used.

For B-pictures, the motion estimation process is performed twice, once for a
past picture and once for a future picture, so as to yield two motion vectors.
The encoder can form a prediction error macroblock from either of the two
candidate macroblocks or from their average. This process is shown in
detail in Figure 6.7. In MPEG terminology, this is referred to as interframe
interpolative coding. The prediction error is then coded using the block-based
DCT. The quantized DCT coefficients of the prediction errors, together with
the motion vectors are then multiplexed and coded using the variable-length
The MPEG Video Standards                                                      171




                          Pas냐)icture



   Current picture                                       Best matching
                                 (, ,   ）쌀三
                                                         macrob幻ck

                                                         MV: motion vector
        (x y)




                           1   Prediction error

                        To OCT



                     Figure 6.6               Forward motion compensation.


coder. Unlike JPEG, MPEG uses only a Huffman coder for variable-length
coding.

Because of the bidirectional prediction, some reordering of the input pictures
is needed at the encoder so that they are delivered in the correct order to the
decoder. For example, consider the sequence of pictures in Figure 6.3. Since
picture P2 is a B-picture that depends on pictures P1 and p4, it can be encoded
only after the input of picture p4. After reordering of the input pictures, the
correct encoding sequence is P1,P4,P2,P3,P7,P5,P6, and P8. This bit stream
provides the decoder with all the information needed to decode each received
picture; however, the decoder will need to reorder these pictures so that they
can be displayed in the correct order.



6.2.4      Video Decoder

Figure 6.8 shows a block diagram of an MPEG video decoder. As expected,
the circuitry of the video decoder is very similar to the circuitry in the feedback
loop of the video encoder. Input pictures are first Huffman decoded and
their type determined from the header information. For each macroblock, the
172                                                                          CHAPTER 6




                                       Past picture
                                                             Best matching
                     Current picture                            macrob幻ck



                                                             MV : motion vector




                                                      Forward prediction error
         Best ma妃hing
         macro벼ock         ／天7
                                                       Interpolative prediction error
                    Backward
                 prediction error
                                                      F가edicti아）error
                                                              To DOT



              Figure 6.7         Bidirectional motion compensation.


coded coefficients are dequantized and translated into the spatial domain by an
IDCT. Consider the encoded sequence Th ,P4,P2,P3,P7,PS,P6, and p8. For the
purposes of this discussion, we will assume that all macroblocks in a P-picture
are coded as P-macroblocks and all macroblocks in B-picture are coded as
B-macroblocks. MPEG-i offers more flexibility in macroblock coding and we
will discuss this in a later section in this chapter. The decoding process is as
follows:


 1. Input p (I-picture). No motion compensation is performed (the input to
    the multiplexor in Figure 6.8 is set to zero). Compute the IDCT and save
    the output into a display buffer and in the previous picture store.

 2. Input p4 (P-picture). For each macroblock, compute the IDCT and
    perform motion compensation; that is, add the area pointed to by the
    motion vector in the the previous picture store to the output of the IDCT.
    The reconstructed picture is saved in the future picture store.
The MPEG %'jat ," .')i 1n(Iar(Is                                                                                  173




                                                                     step size

               Input data
                                       Buffer +       VLC
                                                     Decoder


                                                                                       IDCT

                                                                                       소，
                                                                                            +
                                                                                                Decoded data
                                                     picture store i
                                                                             k,
                                                          Previous
                                                      .
                                              +                      수                           Bu什er        >
                        <
                                 1/2
                                                                                                         H{
                            ＝日




                  X그＞
                                       <H
                            口               1             Future
                                                     picture store
                                                                                  <4
                                 M에on compensat幻n



               Figure 6.8                   Block diagram of an MPEG decoder.


 3. Input p (B-picture). Compute the IDCT and perform bidirectional motion
    compensation; that is, using the two motion vectors, access the pixel values
    in the corresponding regions in the previous and future picture store areas,
    and compute a prediction for P2. Sum the IDCT output and the prediction.
    Since p. is the picture following Pi in display order, P2 can be displayed
    now. Note that. B-pictures need not be stored in the picture store area
    since they are not used in forming the predictions of subsequent pictures.

 4. Input p3 (B-picture). Repeat the steps performed for decoding P2. After
    displaying Th, p4 (decoded in Step 2) is displayed next.

 5. Input p7 (P-picture). Repeat the steps performed for p4. However, the
    reconstructed picture needs to be saved in the previous picture store; this
    overwrites p in the previous picture store.

 6 Input m and p, (B-pictures): Repeat the steps outlined for P2. Note that,
   predictions for p and PG use p4 and p7. After p and P6 are decoded, we
   first display Pt and then the pictures p5, PG. and p7.
174                                                               CHAPTER 6




This completes the decoding of one group of pictures. For the next group,
starting from P8, these decoding steps are repeated. Since at most three pictures
have to be kept in store at any given instant, an MPEG-I decoder needs at
least a half Mbyte of memory for SIF resolution pictures. Note that, the order
of display for the pictures is defined in the presentation time stamp that is
contained in the system layer.



6.2.5 Structure of the Coded Video Bit stream

The MPEG-I syntax for the coded video bit stream has a hierarchical repre-
sentation with six layers: (1) a sequence layer,(2) a group of pictures layer,
(3) a picture layer,(4) a slice layer,(5) a macroblock layer, and (6) a block
layer.

The sequence layer is the top coding layer. It includes a sequence header and is
followed by one or more groups of pictures. It ends with a sequence-end-code.
Among the information included in the sequence header are the vertical and
the horizontal size of each picture, the pixel aspect ratio, the picture rate
in pictures per second, the bit rate in units of 400 bits/s, and the minimum
buffer size needed by the decoder (in units of 2,048 bytes). A single bit also
specifies whether the coded stream meets all the requirements of a constrained
parameter bit stream or not. In addition, the header may also include the DCT
quantization matrices for intra- and nonintra pictures and optional user data.
The default quantization matrix for intra-pictures is the one specified by the
JPEG standard for luminance components. For nonintra pictures, all values
of the default quantization matrix are equal to 16. The rationale for uniform
quantization might be that nonintra pictures provide error information; hence,
there is no reason to favor any particular set of frequency components. In
contrast, in I-pictures, the frequency components are directly related to the
activity within the picture.

A group of pictures(GOP)is a set of pictures in contiguous display order. It
has to contain at least one I-picture. A GOP can begin with either a B-picture
or an I-picture and must end with either an I-picture or a P-picture. If the first
picture is an I-picture or a B-picture that does not depend on the pictures of the
prior GOP,then this GOP can be coded and displayed independently from any
other group. This is defined as a closed GOP. The header of a GOP includes
The MPEG Video Standards                                                      175




timing information, a closed-GOP flag, extension and user data. Figure 6.3
shows a closed GOP with a GOP size of seven.

The picture layer defines the coding information for each picture. Because
of the possibility of reordering P-pictures and B-pictures, the header provides
a temporal reference number that can be used to define the display order of
a picture. Additional header data provide information about the picture type,
synchronization, and the resolution and range of the motion vectors.

Each picture is divided into slices. Slices can be as big as the whole picture. and
as small as a single macroblock. In case of data cor끄ption, the information in
the slice headers allows for a smoother recovery by the decoder. For example,
in the case of transmission errors, a decoder can drop a slice and not the whole
picture. A slice header contains information for its position within a picture
and a quantizer scale factor, between one and 31, that can be used by the
decoder to dequantize the coded DCT coefficients. Specification of quantizer
scale factor allows the encoder to perform rate regulation at the slice level.

A slice is divided into macroblocks. The header of the macroblock defines the
macroblock type, positional information, codes for the horizontal and vertical
motion vectors, and which blocks within a macroblock are actually coded and
transmitted. Optionally, the encoder may include macroblock stuffing. The
pattern "0000 0001 111" is a stuffing code and can be inserted into the bit
stream wherever the encoder detects the possibility of a buffer underfiow.
This stream is ignored by the decoder. Macroblock stuffing is not permitted in
MPEG그．

Figure 6.9 summarizes the syntax layers in the coded MPEG bit stream.



6.2.6    八lacr아)10Ck Co曲ig

As mentioned before, there are three main picture types in MPEG: I-, P-, and
B-pictures. However, even within a single I-, P- or B-picture, macroblocks can
be coded differently. The decision trees for coding macroblocks is shown in
Figure 6.10. This section summarizes the main options in macroblock coding.
176                                                                                                            .. 4; \!’》i iR ti




                         GOP-i                    GOP-2                             GOP-N         )
                                                                                                  1
                                                                         Sequence 1aver
                                   V
                 r                                入
                       IBBPBB...P                      1 아oup이口ctur的카er
                 ＼뇨                                /




                         帥ce-i
                         slice-2                              mb-I           mb-2                mb-n

                                                                                                        //
                         slice-N
                                                                                             Slice layer
                 \h느
                                       I

                       Picture layer
                                                              0 1        YCbCr
                                                              2 3        回 回／
                                                              Macr야）幻ck 冶yer                     8 x 8 block



             Figure 6.9                Syntax layers in MPEG-I video coding.


1-pictures

I-pictures are coded without motion compensation; however, the MPEG syntax
allows each macroblock to be coded using a different effective quantization
matrix. After the DCT, each DCT coefficient is quantized by dividing it
by the corresponding element of the intra quantization nmtrix. For the DC
coefficients, the quantization step is always fixed at eight. For the AC
coefficients, the quantization step depends not only on the value of the
corresponding element in the quantization matrix but also on the value of
the quantization scale factor. Given the DCT output Dc/1i. j]. a quantization
matrix Q[i, j}, and a quantization scale factor q, the quantized AC coefficients
(QDct[i, jj) are given by

                                                                                         1   .                            (6. 1)
                                           QDct        ［自j]          =   "   짧；      1
Each quantized coefficient is clipped in the range f-255, 2551. The scale factor
q is defined in the header of each slice; however, it can also ha redefined in
the header of each macroblock. In MPEG terminology, this sedle factor is
referred to as MQUANT. Referring to Figure 6.10, we note that niacroblocks
                                                                                                    177
The MPEG Video Standards




                 Change MQUANT                    >
     口cture
                 No change to MQUANTD>
                                                                        Change MOUANT
                                                         Coded
                                                                        No chanse to MQUANT
                                              Inter
                                                         N아（沁ded

                                                                        Change卜爪孔ANT
                 Perform motion
                 compensation                 Intra
                                                                        No change to MQUANT


     P picture                                                          Change MOUANT          (>
                                                         Coded
                                                                        No change to MQUANT>
                                              Inter
                                                          N아（沁ded                  (Skipped)

                                                                        Change MQUANT
                 Set motion vector
                 to zero                       Intra
                                                                        No change to MQUANTC>



                  Forward motion compensation
     B pictur艮
                  Backward          compensation
                  1nterpotajeo motion compensation ／二＼
                                                             町）
                             motion
                                                  [>              ＼스)
                                                      Change MQUANT
                                      Coded
                                      C0ded     卜 卜把ch帥 . e to MQUANT
                   IntE玎
                                      Not Coded        Ma beski. .ed

                                                      Change MQUANT
      （勾
                    ntra
                                                卜 No change to MQUANT




           Figure 6.10     Decision trees for coding macroblocks in I-, P, and
           D-plcwres.

                                                              coded using a new
 in I-pictures are of two types, namely, macroblocks that are
                                                               ANT.
 MQUANT and macroblocks coded using the previous MQU
 178                                                              CHAPTER 6




After quantization, the DC coefficients are differentially coded in a way similar
to the method in JPEG. That is, each differential value is coded using a (size,
amplitude) pair. From this pair, the size is Huffman coded and defines the
number of bits used by the amplitude. As in JPEG, the AC coefficients are
scanned in zig-zag order and coded using run-length and level (or amplitude)
information. However, the coding details in MPEG-I are somewhat different
from JPEG. In JPEG, each AC coefficient is represented by a (run/size,
amplitude)pair, where the run/size information is coded with a variable-length
code. MPEG does not use any size information. Instead it provides Huffman
codes for the most frequent run/amplitude values. Run/amplitude values that
are not listed in the table are coded by an escape code followed by separate
Huffman codes for the run-length and the amplitude.

Example. Consider the case of coding the run-length/amplitude values of
2/2 and 2/25. Since amplitude = 2 can be represented by two bits (10) and
amplitude = 25 can be represented by five bits (11001), in JPEG we would
have to code the pairs (2/2, 10) and (2/5, 11001). In MPEG,2/2 can be coded
directly as 00001000. The symbol 2/25 is not listed in the coding tables; hence,
one has to use the escape code (000001) followed by the Huffman codes for
run-length = 2(000010) and amplitude = 25(0001 1001).


Coding ofP-pictures

P-pictures are also divided into slices and macroblocks; however, because of
the motion-compensation process, the encoder has far more coding choices
for each macroblock. The coding choices are depicted in Figure 6.10. The
decisions are summarized as follows.


    Decide if you want to set the motion vector to zero. In many cases, the
    prediction error using a nonzero motion vector may be close enough to
    the prediction error for this macroblock assuming a zero-valued motion
    vector. Since nonzero motion vectors require additional coding bits, it
    is more efficient to code this macroblock using the zero-valued motion
    vector. A simple rule of thumb is to use nonzero motion vectors only if
    the minimum prediction error is at least 1 .1 times smaller than the error
    calculated for the zero motion vector.
    Decide if you want to code the macroblock as an intra- or inter-type
    macroblock. In many cases,it may require fewer bits to code a macroblock
                                                                             179
了he 九I尸EG 1乞／eo 針andards




                                                                    gs to a P-
     as an intra-macroblock (1-macroblock) even though it belon
                                                             to a high level of
     picture. This may happen if motion estimation fails due
     temporal activity.
                                                                       ization, all
     Decide if a macroblock needs to be coded or not. If, after quant
                                                              block is not coded.
     coefficients in the macroblock are zero, then that macro
                                                                     . Decoding
     Such a macroblock is referred to as a skipped macroblock
                                                               of corres  ponding
     of such macroblocks requires only a simple copy
                                                                a macroblock is
     macroblocks in the previous picture. In all cases, when
                                                                be coded. There
     coded, not every block within the macroblock needs to
                                                           cients within one or
     may be cases, where after quantization, all coeffi
                                                                  six-bit pattern,
     more blocks in a macroblock will be zero. In such cases, a
                                                           to the decod  er which
     referred to as the coded block pattern, will indicate
                                                                     . Note that,
     of 'he six blocks within the macroblock have been coded
                                                           all block  s within an
     i-pictures cannot have skipped macroblocks, and
     1-macroblock have to be coded.
                                                                   er may
     Decide if MQUANT needs to be changed or not. The encod
                                                            r overflows or
     decide to change MQUANT if it estimates possible buffe
     underfiows.



 Coding of B-pictures
                                                          very similar to the
 The selection of the macroblock types in B-pictures is
                                                         e 6.10, the decisions
 selection of macroblock types in P-pictures. From Figur
 can be summarized as follows.

                                                                    olated motion
      Decide if you want to use forward, backward, or interp
      compensation.
                                                                type or as an
      Decide if you want to code the macroblock as an intra-
      inter-type macroblock.
                                                              The entire mac-
 1    Decide if a macroblock needs to be coded or not.
                                                        block was an inter-type
      roblock can be skipped only if the previous macro
      macroblock and its motion compensation is good enough.
                                                                changed or not.
       Decide if the quantizer scale (MQUANT) needs to be
 180                                                             CHAPTER 6




 As in the P-picture case, even when a macroblock is coded, some of the blocks
 within it may be skipped if all the quantized DCT values within these blocks
 are zero. The coded block pattern will indicate which of the blocks within a
 macroblock are coded. The ISO document provides several guidelines for the
 efficient selection of macroblock types; however, none of these is mandatory.

 In Table 6.3, we show a distribution of I-, P- and B-macroblocks for 150
 pictures of an MPEG-l coded video sequence. The MPEG-i encoder uses a
 GOP of 15 pictures with two B-pictures for every P-picture, and the coded bit
 rate is 1.15 Mbits/s. Zero MV refers to macroblocks that are coded using a
 zero motion vector. Note that, for B-pict玎es, there is a considerable number


          Picture                    入lacr아：)lOCk Type
           Type       I        P          B     Zero MV    Skipped
             I      3,300
             P        897    8,587               5,128        568
            B           60   7,356    22,845                  429

       Table. 6.3 . Example of the distribution of different macroblock
       types in a viueo sequence.


of macroblocks that are coded using predictive (P) macroblocks. This usually
occurs when there is a scene change or when objects present (absent) in a
P-picture before a B-picture disappear (appear) in the P-picture following that
B-picture.

As mentioned before, MPEG-i allows for skipped blocks within a macroblock.
For example, for the data in Table 6.3, Table 6.4 shows the number of the 8
x 8 blocks that are actually coded. If all blocks were coded, then we should
have a block count that is six times the macroblock count shown in Table 6.3.




6.3 MPEG-i IMPLEMENTATION ISSUES
Complexity estimates for the MPEG-i decoding of SIF resolution pictures,
suggest that software-based decoding is well within the realm of general-
purpose processors. Table 6.5 shows a typical breakdown of the computational
The MPEG Video Standards                                                  181




             Picture              入lacr아：)lOCk Type
              Type        I         P        B     Zero MV
                I       19,800
                p        5,382   30,730                18,146
                B          360    8,176    18,853

     Table 6.4 Example of the number of 8 x 8 blocks that are actually
     coded in a video sequence.



load among the decoding functions in MPEG-I. Note that, the data here is
based on simulations of SW resolution pictures coded at 1.15 Mbits/s and
h' ' ' '.; two B-pictures for every P-picture.


                     Decoding Function                   Load (%)
         Bit stream header parsing                           0.44
         Huffman decoding and inverse quantization          19.00
         Inverse 8 x 8 DCT                                  22.10
         Motion compensation                                38.64
         Color transformation and display                   19.82

     Table 6.5 . Example of the distribution of the computational load
     in 上virtu- i uecoulng.




There is a general belief that the IDCT is the most compute-intensive task in
MPEG-I decoding; however, this is not always true. If the encoder performs
motion estimation and rate control effectively, then, as shown in Table 6.4,
IDCT is not required for many of the blocks. In such cases, as shown in Table
6.5, motion compensation may be the most compute-intensive task. Note also
that YChCr to RGB color transformation and upsampling is as expensive as
the IDCT.

Scaled DCTs could be used in MPEG coders; however, frequent changes of
the quantization scale will decrease their overall computational efficiency. In
MPEG, unlike JPEG, pixel values in one or more pictures are used in the
reconstruction of subsequent pictures; thus, careful attention should be paid to
  182                                                              CHAPTER 6




 the accuracy of the IDCT, so that noise due to arithmetic precision does not
 influence the picture quality.

 The MPEG- 1 constrained parameter set does not deliver video quality that is
 acceptable for broadcast applications. Towards this end, the MPEG-2 standard
 has been developed using many of the principles of MPEG-I coding. In the
 next section, we provide a brief overview of the MPEG-2 video standard.




 6.4    THE MPEG-2 VIDEO STANDARD
MPEG-2 is the outcome of the second phase of work by MPEG. The original
goal of MPEG-2 was to define a generic standard that could be applied to
as wide a class of applications as possible and to support compressed bit
streams at rates close to 5 Mbits/s for NTSCIPAL quality or close to 10
Mbits/s for near studio video quality. Among the original requirements were
(1) compatibility with MPEG-I, (2) good picture quality, (3) flexibility of
input format, (4) random access capability, (5) fast forward, reverse play, and
slow motion capability, (6) bit stream scalability, (7) low delay for two-way
communication, and (7) resilience to bit errors. Bit stream scalability is defined
as the ability to discard portions of the bit stream, but still render the encoded
bit stream at reasonable quality.

MPEG soon realized the following: (1) There was no reason to restrict the
maximum coded bit rate to 10 Mbits/s. MPEG could successfully support
higher bit rates; for example, 80 to 100 Mbits/s for HDTV applications.
(2) It would be impossible to define a single standard that could satisfy all
requirements. (3) Most applications would use only a small subset of the
features offered by the standard. Hence, MPEG decided to adopt a toolkit-like
approach; that is, MPEG-2 is a collection of tools defined in such a way as to
satisfy the requirements of specific major applications.

The range of coding support provided by MPEG is divided into profiles and
levels. For each profile/level, MPEG-2 provides the syntax for the coded bit
stream and the decoding requirements.

A profile is a defined subset of the entire bit stream syntax specified by
MPEG그 The four profiles are Simple, Main, Main+, and Next. Within a
The MPEG Video Standards                                                       183




profile, a level is defined as a set of constraints imposed on the parameters of
the bit stream, such as picture resolution or maximum bit rate. For each profile,
the four levels are Low (for SIF resolution pictures), Main (for CCIR 601
resolution pictures), and High- 1440 and High (for HDTV resolution pictures).
Before we discuss the specific constraints for each profile-level pair, we need
to describe some of the coding extensions in MPEG-2.

The MPEG-2 syntax has two categories: (1) Nonscalable syntax which is a
superset of the coding syntax for MPEG-I, with additional extensions that
support the coding of interlaced signals; and, (2) scalable syntax, which allows
for a layered coding of the video stream. Decoders can either decode the basic
stand-alone layer for a signal of lower quality or use the additional layers to
increase the quality of the decoded signal.

Like MPEG-i, MPEG-2 is a lossy video compression scheme, based on
DCT coding, block-based motion compensation, predictive and interpolative
interframe coding, and Huffman coding. Many of these functions are similar
to the ones in MPEG-i and we refer the reader to the previous section for the
coding details. In the following sections, we highlight the functions that are
either new to MPEG-2 or are extensions of those found in MPEG-i.

MPEG-2 is backward compatible with MPEG-I; that is, an MPEG-2 decoder
should be able to decode an MPEG-I coded stream. Using the scalable
syntax, the lower layer of an MPEG-2 signal could also be decoded by an
MPEG-i decoder, but this is not required. Here, we will primarily focus on
the nonscalable syntax. Some of the new features supported by MPEG그 are
discussed in the following sections.



6.4.1    Interlaced Pictures

MPEG-2 supports both interlaced and noninterlaced pictures. Fields in an
interlaced picture can be coded separately (field pictures) or they can be
interlea 'dd and coded as one picture (frame pictures). Like MPEG-i, all input
pictures can be coded as I-, P- or B-pictures. If the first picture of a coded
frame is an I-field picture, then the second picture can be either an I-field
picture or a P-field picture; that is, the first field can be used as a predictor for
the second field. If the first picture is a P-field or a B-field picture, then the
 second field-picture has to be of the same type as the first field-picture.
 184                                                             CHAPTER 6




 6.4.2   C이or St出sami川ng

 As in MPEG-i, input pictures are coded in the YCbCr color space; however,
in addition to the 4:2:0 化rmat used in 入4PEG工 入4PEG그 카so supports the
4:2:2 and 4:4:4 color subsambling formats. In the 4:2:2 format (also known
as CCIR 601 format), the chrominance components have the same vertical
resolution as the luminance component, but the horizontal resolution is halved.
In the 4:4:4 format, all components have identical horizontal and vertical
resolutions. Table 6.6 shows picture sizes for a 60-Hz CCIR 601 signal
using three different subsampling formats. From Table 6.6, a CCIR 601 input


               Color              P江eIs per line x lines
             Component        4:2:0      4:2:2         4:4:4
                Y           720 x 480 720 x 480 720 x 480
                Cb          360 x 240 360 x 480 720 x 480
                Cr          360 x 240 360 x 480 720 x 480


       Table 6.6 Active pixels . for a 60-Hz CCIR 601 signal using
       vanous suosampting rormaLs.


signal has 720 active pixels per line. In practice, a preprocessor to the coder
removes the eight leftmost pixels and the eight rightmost pixels to generate
a picture with 704 pixels per line so that an integral number of macroblocks
are obtained for each row. The informative section of the MPEG documents
include various filtering and picture conversion techniques.

Figure 6.11 shows the macroblocks used in the 4:2:2 and 4:4:4 formats.
Macroblocks in the 4:2:0 format are identical to that of MPEG-i. A 4:2:2
macroblock has four blocks of Y, two blocks of Cb, and two blocks of Cr. A
4:4:4 macroblock has four blocks of Y, four blocks of Gb, and four blocks
of Cr. When the coded bit stream has no scalable extensions, then all blocks
within a macroblock are 8 x 8. With scalable extensions, macroblocks may
contain scaled blocks with lower resolutions, such as I x 1, 2 x 2, or 4 x 4.
The sti끄cture of the luminance n狙cr아加cks is different f아 fra毗 DCT coding
and field DCT coding, as shown in Figure 6.12. In frame DCT coding, all
blocks contain data from both the top field and the bottom field. In field DCT
coding, the top two blocks have data from the top field and the bottom two
Thd MPEG Video Standards                                               185




                     Y     Cb       Cr   Y        Cb      Cr

                    4:2:2 macroblock         4:4:4 macr야引ock



          Figure 6.11    The 4그2 and 如：4ma아0바ocks in MPEG그


blocks have data from the bottom field. For chrominance blocks, all blocks
are interlaced (as in frame DCT coding).

                     8          8                  8           8

              8                                                    8


              8                                                    8




                  Frame DCT coding              Fie'd DCT coding



        Figure 6.12 Structure of luminance macroblocks in frame and
        field DCT coding.




6.4.3     Prediction Modes and Motion Compensation

In MPEG-2, the picture sequence can be either a collection of frame pictures
or a collection of field pictures. Two classes of prediction are supported,
namely, frame prediction and field prediction.
186                                                                    CHAPTER 6




Field andframe prediction

For field pictures, predictions are made independently for each field from
reference fields. This is similar to what is done in MPEG-i, with each field
considered an independent picture.

In frame prediction, predictions are formed from reference frames, which may
have been coded using frame or field prediction. If a frame picture is assumed
to have originated from two fields, then both fields must have the same coding
type, except for the case when the first field is an I-picture, in which case the
second field of this frame can be an I- or P-picture.

Figure 6.13 shows examples of the different prediction modes for frame
pictures. Frame pictures may use both field and frame predictions. In frame
prediction (Figure 6.13a), the whole (usually interlaced) frame is considered a
single picture. In field prediction, each frame is treated as two separate fields.




                    Reference frame               Current frame
                                 (a) Frame prediction




                                                                     Bottom ti이d
                                                                     of frame

      Reference frame                  Reference frame

        (b) 日eld predict向n                    (C) Field prediction


       Figure 6.13      Examples of prediction modes for frame pictures.


A motion vector can point either to a field in another reference frame or to a
field in the current frame. For example, in Figure 6.13b, the first field (which
can be either the top or the bottom field) can be predicted either from the top
The MPEG Video Standards                                                     187




or the bottom fields in a reference frame. In Figure 6.1 3c, the second field (the
bottom field in this example) can be predicted either from the bottom field of
another frame or from the top field of the current frame. The above examples
can easily be extended to other cases. Field prediction modes are beneficial in
coding interlaced scan video. For progressive scan video, frame prediction is
sufficient.

In MPEG-2, unlike MPEG-i, all motion vectors are specified at half-pixel
resolution. Let (tz, v) denote the motion vector of the luminance components
in a macroblock. Due to subsampling of the chroma components, their motion
vectors are given by (f-, ) for the 4:2:0 format and by ( -,v) for the 4:2:2
format. For the 4:4:4 sampling format, the chroma components use the motion
vectors uf the luminance component without any scaling.

Oince MPEG-2 video may be used in harsh broadcast environments, some
immunity to transmission errors is needed. In a compressed video bit
stream, erroneous reception of motion vectors can be catastrophic, unlike, say,
erroneous reception of some of the high frequency DCT coefficients within
an 8 x 8 block. Thus, the MPEG그 syntax has provisions for including
specially coded motion vectors, referred to as concealment motion vectors,
within intra-macroblocks. The assumption here is that the transmission of intra
macroblocks is done in a more reliable manner.

To improve prediction efficiency, MPEG-2 provides two additional motion
compensation modes. The 16 x 8 motion-compensation mode allows a 16 x
16 macroblock to be treated as an upper 16 x 8 region and a lower 16 x 8
region. Each of the 16 x 8 regions is then independently motion-compensated.
Thus, a 16 x 16 P-macrobiock will have two motion vectors; likewise, a B-
macroblock will have four motion vectors. The 16 x 8 motion-compensation
mode is only allowed for field pictures.


Dual-prime motion compensation

Another motion-compensation mode provided in MPEG-2 is the dual-prime
mode. The dual-prime mode is applicable only to P-pictures and to GOPs that
have no B-pictures between these P-pictures and the reference pictures. This
motion-compensation mode for frame and field type pictures is illustrated in
Figure 6.14. For frame pictures, two motion vectors are associated with each
field. For instance, in Figure 6.14a, motion vectors v1 and 刃v1 are associated
 188                                                                                                             CHAPTER 6




                        vi


                                                                                                              Current
                                                                                                       /pvi   Picture
                        V2
       A可erence                    Current                                   Reference
        Frame                       Frame                                      Frame
       (a) Field prediction in frame picture                                 (b) Field predict幻n in field picture


       Figure 6.14           Dual-prime prediction mode in frame and field
       pictures.



with the top field and motion vectors v2 and 끄v2 are associated with the bottom
field of the current frame. Let vi(x), pvi(x), v2(工), and pv2(x) denote the
horizontal components of the motion vectors Vt, pvl, v2, and pv2. The vertical
(y) components are denoted in a similar manner. In dual-prime prediction,
motion vectors pv1 and pv2 are derived from v1 and v2 as follows.

Consider the derivation of pvi. Since pvi is a motion vector from an opposite
parity field, namely, from the bottom field in the reference frame to the top
field in the current frame, the existing motion vector v1 is scaled to reflect the
temporal distance between the fields. First, a correction is made to the vertical
component of the motion vector to reflect the vertical shift between lines of the
top and bottom fields. Second, a small differential motion vector 8 is added.
The appropriate choice of a is determined by the encoder. In a similar manner,
we can derive pv2. From the MPEG-2 document, the relevant equations for
frame picture prediction, as depicted in Figure 6.14, are given by

                                               i '1
                             Pu1（끼     =                            +万                                                  (6.2)
                                                      (x
                                                   2
                                                                )
                                             穹2 1『d(9),
                                                                             (x)
                                                                                   ,
                             끄V1(!/)   =                                                                                (6.3)
                                                   xv
                             pV2（끼     =                                     『万                                         (6.4)
                                               3
                                                                    (x
                                                           :2
                                                                         )
                                                                                       （7)
                                                                                             ,


                                               3 x v2
                             끄V2(y)    =                                      + 1+ 8                                    (6.5)
                                                                    (y
                                                   2
                                                                         )
                                                                                                 (y)
                                                                                                       ,
where 8(x) and 8(y) can take the values in -1, 0 or 1. Note that, pv1 and pv2
are not included in the encoded bit stream; instead, along with v1 and v2, the
The MPEG Video Standards                                                     189




corresponding (5 is included in the bit stream so that the decoder can derive 끄v1
and pv2.

For the field picture shown in Figure 6.14(b), the relevant equations for 끄v1
are
                                        v'
                               （끼
                               1
                                    =
                                                   * 万         ,            (6.6)
                                             2
                                                         （7)
                         Pt,
                         PU'（功 = 斗y2 l+d(y).
                                             (x)
                                                                            (6.7)



6.4.4 DCT and Quantization

MPEG-i uses only two quantization matrices for the DCT coefficients: one
for intra blocks and one for nonintra blocks. In MPEG-i, the quantization
matrices can be changed only at the sequence level of the hierarchy, whereas,
in MPEG-2, the matrices can be changed at the picture level. For the 4:2:2 and
the 4:4:4 formats, MPEG-2 allows for more efficient coding by supporting
the use of different quantization matrices for the luminance and chrominance
components. Thus, one can use two matrices for luminance blocks (intra
and nonintra) and two matrices for chrominance blocks (intra and nonintra).
Quantization of the AC coefficients is simil缸 to the process in (6.1). In MPEG-
 I and MPEG-2, the quantizer scale factor can be changed on a macroblock
basis in order to achieve a constant bit rate at the encoder output. The method
 to change the quantizer scale factor is not part of the MPEG- i and MPEG-2
standard.



 6.4.5 Profiles and Levels

Table 6.7 summarizes the key characteristics of the profiles and levels defined
by MPEG그 Picture resolution is given as pixels per line multiplied by the
number of lines. The Bit rate data refer to the maximum compressed bit rate
supported by the input buffers of a decoder. Areas with "N/A" indicate that
there are no conformance restrictions for these variables. It is expected that
early implementation of the standard will only support the Main profile at the
Main level. The Main profile provides the basic functionality of MPEG-2 and
is expected to be supported by most of the initial applications. The Next profile
includes hierarchical representation and is suitable for terrestrial broadcasting.
190                                                                                    CHAPTER 6




                                                               Profiles
              Levels                        Nonsca始ble                          馱alable

                                     Simple           Main            入lain+              Next
                                      4:2:0           4:2:0           4:2:0               4:2:2

               入lax res이utionl        N/A         1920x 1152/60           N/A        I920x 1152160
               rate (H기
               Mm . resolution/       N/A                N/A              N/A         960 x 576/30
      High     rat이H기
                                                                                     100 (all layers)
               Bitrate (Mbits/s)                                                     80 (base-+-mid)
                                      N/A                 80              N/A
                                                                                     25 (base layer)
              卜lax res이utionl
                                      N/A         1440x 1152/60 1440x 1152/60 1440x 1152/60
              rate (H기
      Hi만1-
               Mmn. resolut向nl
                                      N/A                ！口A       720 x 576/30      720 x 576/30
      1440     rate (H기
                                                                   60 (all lay crs) 80 (all layers)
               Bitrate (Mbits/s)      N/A                60        40 (base+mid) 60 (base+mid)
                                                                   IS (base layer) 20 (base layer)
               Max resolution/
                                   720 x 576/30    720 x 576/30    720 x 576/30      720x 576/30
               rate (H기
               Mmn. resolution/
                                      N/A                N/A              N/A        352 x 288/30
      Main     rate (H기

                                                                   15 (all layers) 20 (all layers)
               Bitrate 小lb小／s)         15                15                        15 (base+mid)
                                                                   10 (base layer) 4
                                                                                     (base layer)
               入Ia乂 resolut幻n/
                                      N/A          352 x 288/30    352 x 288/30            N/A
               rate (H기
               Mm1l. resolution/
      Low                             N/A                N/A              N/A             N/A
               ra妃 (H기

                                      N/A                          4 (all layers)
                                                          4                               N/A
               Bitrate 小lb心八）
                                                                   3 (base layer)




              Table 6.7       Profiles and levels in MPEG-2 video coding.


The Main+ profile is a superset of the Main profile but a subset of the Next
profile. It allows for a gradual move from the Main profile into the Next
profile. The Simple profile is a low-cost version of the Main profile. Coding
is similar as in the Main, but without any bidirectional prediction.
The MPEG Video Standards                                                      191




Levels are related to picture resolution. The upper bound on the Main level
resolutions corresponds to the CCIR 601 picture format. The High-1440 and
High level resolutions correspond to picture resolutions for HDTV. The Low
level resolutions correspond to the SIF format.

A decoder that can decode bit streams at a certain profile/level should be
able to decode also all bit streams of lower profiles/levels than its own. The
only exception is that decoders of the Simple profile at Main level are also
required to decode Main profile at Low-level bit streams, that is, MPEG-I
coded streams.



6.4.6   Scalable Bit streams

A new feature of MPEG-2 is bit stream scalability, which allows for a layered
representation of the coded bit stream. The MPEG-2 syntax allows for four
basic modes of bit stream scalability: data partitioning, SNR scalability, spatial
scalability, and temporal scalability. These basic scalability schemes can be
combined to form a hybrid scalability scheme.


I九玎a 恥rtiti(城ng

With data partitioning, the bit stream is split into two layers, called partitions.
For example, the first partition may include all critical header information
(such as headers and motion vectors), and the second partition may include
the remaining bit stream. This mode is intended for use in applications that
can allocate two channels for a single bit stream.


SNR scalability

SNR scalability can be used in applications that support video transmission at
multiple quality levels. All layers have the same spatial resolution but different
video qualities. The lower layer is coded by itself and provides the basic video
quality. The enhancement layers are coded as to enhance the basic quality by
providing refinement data for the DCT coefficients of the lower layer. SNR
scalability provides for better resilience to transmission errors. For example,
the enhancement layers can be sent over a channel with poor performance, and
the lower layer can be sent over a channel with better error performance.
 192                                                                 CHAPTER 6




 Spatial scalability

With spatial scalability, the bit stream is divided into layers of different spatial
resolution (this is similar to the hierarchical coding in JPEG). The lower layer
is coded by itself to provide the basic spatial resolution. The enhancement
layers can use the spatially inte叩olated lower layer to provide a video stream
at the full spatial resolution. Layers may have different frame sizes, frame
rates, or chrominance formats. In a typical application, the lower layer may be
MPEG-I compliant at SIF resolution, whereas the enhancement layer might
be used to generate CCIR 601 resolution video.


 Temporal scalabilily

Temporal scalability allows the migration from systems with low temporal
resolution to systems with higher temporal resolution. In this case, the
lower layer is coded by itself and provides the basic temporal rate, and the
enhancement layers are coded with temporal prediction with respect to the
lower layer. The lower layer and the enhancement layers can be combined to
generate a stream at full temporal resolution. All layers have the same frame
size and chrominance formats but different frame rates.

In summary, MPEG-2 is a superset of MPEG-I and some of the features in
MPEG-2 that are not found in MPEG- l are shown below:


    Support for both interlaced and noninterlaced pictures.

    Support for 4:2:0, 4:2:2, and 4:4:4 subsampling schemes.

    Motion compensation based either on interlaced frames or noninterlaced
    fields and frames.

    Improved picture quality through new options for the quantization of the
    DCT coefficients and alternate zig-zag ordering.

    New syntax for scalable bit streams.


The MPEG-2 standarization process is still evolving. It is now proceeding
키ong two direct幻ns:
The MPEG Video Standards                                                      193




      Extensions to MPEG-2. These extensions include video coding with 10
      bits per pixel, higher quality audio coding, and specifications for interact-
      ing in real-time, as well as specifications that will allow applications to
      interact directly with MPEG compressed bit streams.

      Development of a coding standard for very low bit-rate applications
      (MPEG-4). It is a common belief that the techniques that have been the
      basis for MPEG- i and MPEG-2 may be inadequate for MPEG-4, since the
      bit-rate targets for MPEG-4 will be around 8 to 64 kbits/s. The MPEG-4
      standard is expected to be completed by November of 1998.




6.5      TO PROBE FURTHER
The MPEG-I and MPEG-2 standards are described in the ISO documents [84)
and [86]. In addition to the systems, video, audio, and conformance testing
parts, MPEG-2 will also include a fifth pa戊 (13818-5 software) that will
provide software-based coding models for the first three parts in the standard.
The video portion of MPEG-2 has also the nomenclature Recommendation
ITU-T H.262. The standardization process itself is described by Chiariglione
[33]. Early descriptions of MPEG-I can be found in [54] and [138]. A good
overview of the systems part in MPEG-I is given by Maclnnis [128].

For MPEG-2, an early overview of the standardization process and the coding
requirements is given by Wells [192]. The data in Table 6.7 are based on
a similar Table given in [148]. MPEG- l and MPEG-2 support constant
bit-rate and variable bit-rate encoding. Bit-rate control is primarily achieved
by changing the quantizer scale factor. However, the specific mechanism by
which the quantizer scale factor is changed is not specified in the MPEG-I
and MPEG-2 standards. The MPEG-2 test model document [87] provides one
approach for bit-rate control. A brief description of the test model can be found
in [43]. Bit-rate control is an area of active research. Various approaches
 suitable for MPEG-I and MPEG-2 can be found in [99], [40], [29], [162],
[48], and [62]. Most of these techniques are based either on concepts from
control system theory or on image classification. Various researchers have
also attempted to develop functional models that relate bit rate to the quantizer
 scale factor, much like the rate-distortion functions we described in previous
 chapters. Recently, MPEG-2 was chosen for the video coder of the Grand
194                                                            CHAPTER 6




Alliance HDTV system for North America. A general overview of this system
is given by Hopkins [74].

Video generation, preprocessing, post processing, and display are not defined
by the standards, but are integral parts of any video coding system. There are
many fine textbooks on color and digital television, including [79] and [1731.
The CCIR 601 standard for digital TV is described in [11.

Software implementations of MPEG coders have been reported in [20],[42],
and [19]. Sites with public-domain MPEG encoders and decoders are given in
Appendix B. Hardware implementations of MPEG coders are described later
in this book.
                                                                         7
                THE H.261 VIDEO CODING
                              STANDARD




7.1 INTRODUCTION
In recent years, there have been significant developments in videoconferencing
and audiovisual services. First, data rates in digital telecommunication services
have been constantly improving. For example, integrated services digital
networks (ISDNs) may provide switched transmission services at data rates
close to 2 Mbits/s. Second, the latest technology for the coding of video
signals allows videoconferencing signals to be compressed down to 64 kbits/s,
the equivalent of a single telephone voice channel.

In the late I 970s, the telecommunications industry realized that Continuous
growth of audiovisual services was possible only through international stan-
dards. Customers expected and demanded video terminal equipment to have
the same level of compatibility as other telecommunication equipment, such
as modems and facsimile machines. In the early 1980s, the CCITT Rec-
ommendations H.120 and H.130 were the first international standards for
videoconferencing. The two standards provided guidelines for transmitting
PAL or NTSC television signals at data rates close to 2 Mbits/s. The conversion
between PAL and NTSC was integrated into the coding process.

However, these standards found acceptance only in Europe. Manufacturers
in the United States and Japan continued to develop and market proprietary
video coding techniques that offered better signal quality at data rates lower
than 2 Mbits/s. In the late I 980s, a new collaboration among telecommunica-
tion operators and manufacturers of videoconferencing equipment led to the


                                       ]Q드
196                                                                       CHAPTER 7




development of the H.261 video coding standard. This is also known as the P
 x 64 standard because it describes video coding and decoding methods at the
rates p x 64 kbits/s, where p is an integer from I to 30. H.261 was ratified in
Geneva in December of 1990.

A video teleconferencing system processes not only video but also audio and
ancillary digital data. Thus, additional considerations have to be made for audio
compression, data multiplexing, and overall system control. Recommendation
H.320 is a complete family of standards, and defines the technical requirements
for narrow-band visual telephone systems and terminal equipment.

Figure 7.1 shows the block diagram of a generic, H.320 compliant, visual
telephone system and which Recommendations are relevant for each one of the
blocks. Video equipment includes cameras, monitors, and video processing


      1
      1                            H.261                       H.221
      1
              Video                Video                      Fran怡
      1
           Equipment               Codec                    Structure
      1
                               H.2001AV.250-Series




                                                                            8m七으드 노b名mZ
      1
              Aud幻                 Audio
                                                     0이ay
           Equipment               Codec
                                                            MUX/OMUX
              T-Series. I{.200/AV.270-Series

                 Telematic Equipment

          H.242. H230. H.221
             System
                                       End寸0-end
             Contr이
                                   Network Signaling        .400-Series

                                                H.320




      Figure 7.1 . Block diagram of a generic visual telephone system,
      anu associateu tc.ecommenuauons.

units. Audio equipment includes microphones, speakers, and audio processing
units. Telematic equipment includes data terminals and visual aids such
as electronic blackboards or a still-picture transceiver. The system control
The H.261 Video Coding Standard                                           197




unit performs end-to-network signaling and end-to-end control to establish
a common mode of operation among terminals. The video and the audio
codecs perform video and audio compression and decompression. A delay
in the audio path compensates for the video coding delay and allows the
system to maintain audio and video synchronization. The mux/dmux unit
multiplexes audio, video, and data into a single bit stream during encoding
and demultiplexes them during decoding. Finally, the network interface
provides the interface between the networks and the terminal as defined in the
1.400-series Recommendations.

H.320 refers to a number of Recommendations, including:


    H.261: A video coding algorithm for compressing signals at data rates
    from 64 kbits/s to 1,920 kbits/s.

    G.722, G.726, and G.728: A series of algorithms for the compression
    of audio signals at data rates from 16 kbits/s to 64 kbits/s. These
    Recommendations are examined in more detail in Chapter 16.

    11.221: This Recommendation specifies the frame structure for multiplex-
    ing video, audio, and data into a single bit stream.

    11.230 and 11.242: These Recommendations specify the handshaking
    pr야ocol北etween 11.320 compliant equ巾毗nt.

    H.233: This Recommendation allows manufacturers to select from three
    methods of encryption in their 11.320 compliant equipment: DES, used in
    the United States; SEAL used in Japan; and BCRYPT, used in the United
    Kingdom. The H.233 Recommendation has not yet resolved the issue of
    how to pass the encryption keys from one location to another.


In the remainder of this chapter, we examine in more detail the H.261
Recommendation.
198                                                                CHAPTER 7




7.2      THE H.261 VIDEO CODING STANDARD

7.2.1     The Common Intermediate Format

One of the major problems in defining an international standard for video-
conferencing was the fact that there exist two different line and picture rate
television standards. NTSC, used in North America and Japan, uses 525 lines
per interlaced picture at 30 pictures per second. On the other hand, most of the
other countries use 625 lines per interlaced picture at 25 pictures per second.
To eliminate the problem of interoperability among systems with different
formats, a new common intermediate format (CIF) was adopted. Both the 625
and the 525 line systems need to include pre- and postprocessing modules to
convert to and from CIF.

CIF is a noninterlaced format. It is based on 352 pixels per line, 288
noninterlaced lines per picture at 30 pictures per second. These values
represent half the active lines of a 625/25 television signal and the picture rate
of a 525/30 (NTSC) signal. Therefore, 625/25 systems need only to perform a
picture rate conversion and NTSC systems need to perform only a line-number
conversion.

Color pictures are coded using one luminance and two color-difference
components (YCbCr) as specified by the CCIR 601 standard. The Cb and
Cr components are subsambled by a factor of two on both the horizontal and
vertical directions and have 176 pixels per line and 144 lines per frame. The
picture area covered by these numbers of pixels and lines has an aspect ratio
of 4:3. Table 7.1 summarizes the characteristics of a CIF frame.


                           C이or           Image size
                         component      (pixels x lines)
                            Y              352 x 288
                            Cb             176 x 144
                            Cr             176x 144


        Table 7.1 Picture characteristics of the common intermediate
        format (CIF).
The H.261 Video Coding Standard                                                                                                  199




For low bit-rate applications, in addition to CIF, video coders may also use
a quarter-CIF (QCIF) format, which has half the number of pixels and lines
required for CIF. Support for CIF coding and decoding is optional; however,
all coders must be able to operate using QCIF.



7.2.2    H.261 Encoding

Like MPEG, the H.261 encoding algorithm uses a combination of DCT coding
and differential coding. Figure 7.2 shows a block diagram of an H.261
video encoder. The main elements are frame prediction, DCT transformation,


                                                                              Coding Control
                                1NT日A

        Fran祀                                             >                                    Quantizer              VLC
                       > +                                      Mux                OCT H>                       H>
                                                -
                                                           >                                                         Encoder
                  H{
                                                                       m4>
        Memory
                                            -
                                                                 :
                                                                                                      （긔
                                                                                                  (
          수             工NTER
        NTSC                                                                                                          Buffer
          to
                                                                                                           A
                                                                                                           1V




                            mEm늡 m＞ 小乞乞m左
         C下


          十
         Input
                                                                                                 IDCT                  Error
                                                                                                                     Correct幻n
                                            0       -
                                                           >
                                                                Mux
                                                          t＞긔
                                                                                                                         4,
                                                                                                                      Output
                                Loop                                         Motion             다ame
                                                                     Compensation               Memory
                                                        口口mH
                                Filter

                                       수                                       A
                                                                        卜加tion
                                                                      Estimation




                 Figure 7.2                                    Block diagram of an H.261 video encoder.

 quantization (Q), and variable length coding (VLC).
200                                                               CHAPTER 7




The DCT coding path is similar to the one used in JPEG and MPEG. A video
frame is first translated into a CIF frame and then stored into frame memory.
Noise filtering or other signal preprocessing can also be performed at this
stage. Similarly to the operations in JPEG, the DCT operates on 8 x 8 picture
blocks. Four luminance (Y) blocks and one Cb and one Cr color difference
block are combined to form a macroblock.

Note that, frame prediction is done in a manner similar to that in MPEG-I, with
the exception that only I-pictures and P-pictures are used. The macroblock
organization and the classification of a macroblock as an intra-type or inter-
type follows the approach in MPEG-I. Differential coding allows the DCT
coder to operate on either input macroblocks (INTRA mode) or the differential
macroblocks between the current frame and the prior frame (INTER mode).
Not all macroblocks need to be coded and transmitted. For example, at low bit
rates, macroblocks (and up to three full frames) can be skipped. The criteria
for choosing either to transmit or skip a macroblock or the control mechanism
for intra- or inte汗rame coding are not part of the standard and may vary
dynamically, depending on the complexity of the input signal and the output
data rate constraints.

Following the DCT, the output DCT coefficients are quantized, coded using a
variable length coder (a Huffman coder in this case), and stored into an output
buffer. By monitoring the capacity of the buffer, the coder can perform data
rate control dynamically. The rate control strategy is not specified in the H.261
standard; here, approaches similar to that adopted for MPEG-I can be used.
A proposal for rate-control is included in the informative part of the H.261
document.

Since H.261 is a predictive coder and since transmission errors may cause
significant image quality problems, a BCH(5 11,493) coder is used to add parity
bits for error detection and correction. However; the use of error detection and
correction is optional for an H.26 1 decoder.

Because of the use of predictive coding, the encoder needs to monitor the
quality of the transmitted image so that it does not diverge from the original
signal. After an inverse quantization (Q ') and an inverse DCT (IDCT), the
encoder is able to reconstruct a frame as it will be seen by the decoder. The
reconstructed frame is stored into frame memory. Note that, since the VLC
了方eH.261 Video（勿ding Standard                                               201




operation is lossless, there is no need to include the VLC unit into the feedback
path that generates the prediction frames.

As shown in Figure 7.2, the prediction path may also include optional circuitry
for motion estimation and compensation, and a spatial loop filter. The role of
the ioop filter is to minimize the prediction error by smoothing the pixels in
the previous frame. The loop filter is a separable 2-D filter that operates on 8
 x 8 blocks. The corresponding 1-D filter is a three-tap finite impulse response
filter. At block edges, the filter coefficients are 0, 1, and 0. Otherwise, they
                                                                             and
are { , 去, and 去. Recent studies suggest that tap weights of 0.1248, 0.7495,
0.1248 yield nearly a I dB improvement in signal quality when an accurate
motion-estimation technique is used. On the other hand, for a less accurate
motion-estimation method, the H.261 recommended tap weights may be more
appropnate.

The compressed data stream is arranged hierarchically into four layers: picture,
group of blocks (GOB), macroblock (MB), and block.


     A picture is the top layer.

     Each picture is divided into groups of blocks (GOBs). A GOB is either
     one-twelfth of a CIF picture or one-third of a QCIF picture.

.    Each GOB is divided into 33 macroblocks.

     Each macroblock consists of six 8 x 8 blocks, that is, four blocks of
     luminance (Y), one block of Cb, and one block of Cr.



7.2.3    The H.261 Video Decoder

Figure 7.3 shows a block diagram of the H.261 video decoder. After optional
error correction, the compressed input is buffered and processed by the variable
length decoder. The decoded data are parsed and then processed by an inverse
quantizer and an inverse DCT. Depending on the transmission mode (1NTRA
or INTER), macroblocks from a prior frame may also be added to the current
data to form the reconst끄cted data. The decoded CIF data may then be
converted to the appropriate display format.
202                                                                                           CHAPTER 7




                                                                       step 듸ze



               Error                                     VLC
                        나＞ Buffer                 H>
             Correction                                 Decoder

                                                                                   心
                                                          뇨으Um> C으石E
                i:   }
                            Inter/Intra I
                              mode 1                                              IDCT
            Input data
                              0
                                                                                   寸
                                  -      >
                                        t>
                                              Mux                                  +      Decoded data

                                                                                   寸
                         Loop                          M이幻n                       Frame
                                      ＜山＝    ＝미
                                                                        <mH
                         Filter                   Compensation                Mem이y



            Figure 7.3      Block diagram of an H.261 video decoder.


7.3 IMPLEMENTATION ISSUES
Not all implementation details are specified by H.261. This gives manu-
facturers the opportunity to tailor their implementations to suit their target
applications and to provide for product differentiation. Among the details
that are open to variations are rate-control mechanisms, motion-estimation
algorithms, and preprocessing and postprocessing algorithms.

In early field trials of H.261 codecs, it was noted that small variations in the
implementation of the inverse DCT between two coders may yield noticeable
picture artifacts. To resolve this problem, the H.261 Recommendation provides
guidelines for measuring the accuracy of a particular implementation of the
inverse DCT. The procedure to test the accuracy of an IDCT is outlined in
Annex A of the H.261 standard and consists of the following steps: (1) generate
random data in a specified range, and form 8 x 8 data blocks, (2) perform a
DCT on each block, (3) perform an IDCT, and (4) measure peak, mean, and
mean square error between the original data and the output of the IDCT. To
be H.261 compliant, the following conditions must be met:


      For any pixel, the peak error should be less than 1.0, the average error
      (over 10,000 blocks) should be less than 0.015, and the mean square error
      should be less than 0.06.
The H.261 Video Coding Standard                                                 203




    Overall, the average error should be less than 0.0015, and the mean square
    error should be less than 0.02.

     All zeros in must produce all zeros out.


In addition to the above conditions, the standard requires that there is at least one
intraframe coded macroblock for every 132 interframe coded macroblocks.
This number corresponds to four GOBs or to one-third of a CIF picture.
Intraframe coded macroblocks flush out any errors that defeat the error-
correction circuitry and allow for the errors in the frame prediction to be
reset. For better coding efficiency, most implementations of H.261 prefer not
to perform intraframe coding on all the macroblocks of a picture. Instead,
they perform intraframe coding on a few macroblocks in every picture using a
rotational scheme.

H.261 shares much functionality with the MPEG video coding standards.
However, even though the key coding algorithms are the same, the two
standards target different applications with different requirements in data
rates, picture quality, and end-to-end coding delay. Table 7.2 shows the main
differences between H.261 and MPEG.

Presently, there is a great deal of interest in developing software implementa-
tions for H.261 on general-purpose processors. Due to the motion estimation
마ocess, encodin卽ss坦nificantly more co呻l아 than decoding. In fact, 蜘如n
estimation may be close to 60 percent of the overall computational load. One
way to reduce the computational load is by reducing the search-range in motion
estimation.

In H.261, the maximum range for a motion estimation vector is [-15, 15]
pixels. Using the maximum range in all H.261 applications will not necessarily
improve the quality of the compressed signal. H.261 applications can operate
at various bit rates, ranging from 64 kbits/s to 1,984 kbits/s. At high frame
rates, the temporal distance between frames is smaller; thus, one can afford to
have smaller search ranges. At low frame rates, the situation is reversed, and
 one needs larger search ranges for better image quality.

Furthermore, videoconferencing primarily deals with scenes where most of
the movement is in the head and the shoulders. Experiments show that one
can use a smaller, diamond-shaped, search region, instead of the conventional
 204                                                                 CHAPTER 7




                      MPEG                            H.261
          Uses CIF, SIF, or higher         Uses QCIF or CIF
          spatial resolutions.             spatial resolutions.
          Variable image aspect            Fixed 4:3 aspect ratio.
          ratio (defined in the header).
          Uses groups of pictures.          No notion of GOPs.
          I, P. and B macroblocks.          No B macroblocks.
          Typical bit rates are            Typical bit rates are
          around 1.1 Mbits/s.              around 384 kbits/s.
                                           Max. bit rate is 2 Mbits/s.
          No restrictions on               Only 1, 2, or 3 skipped
          skipped pictures.                pictures allowed.
          Sub-pixel accurate               Pixel accurate
          motion vectors.                  motion vectors.
          Typical motion vector            Typical motion vector
          range is +1- 15 pixels.          range is +1- 7 pixels.
          The end-to-end coding            Used mostly in interactive
          delay is not critical.           applications. End-to-end
                                           delay is very critical.

       Table 7.2 Main differences between the MPEG and the H.261
       standards.



rectangular-search region, with no noticeable loss in video quality. Several
search regions are depicted in Figure 7.4a. From Figure 7.4b, at very low
bit rates (64 kbits/s), and frame rates below 10 fps, motion estimation using
the diamond-shaped search region b ([-8, 8] pixels) yields virtually the same
video quality as motion estimation using the square-search region a ([-15, 15]
pixels). At high bit rates (1.5 Mbits/s), for typical videoconferencing scenes,
there appears to be no benefit using a large search range. The shaded squares
in Figure 7.4b, show the best motion-estimation schemes for various cases of
practical interest. For these search ranges, the computational complexity of
motion estimation can be reduced by at least eighty percent.
The H.261 Video Coding Standard                                                  205




                                                a (1-15, 151 pixels)
                                           』口
                                           c ((-6, 6] pixels)

                                                e ([극 2] pixels)




                                                f (No motion compensation)


                      (a) Search regions


                           1.5 Mbitsls, 30 fps
                   41.00   384 kbits/s, 15 fps

                   40.50

                   40.00

                   39.50   128 kbits/s,


           小m으工石
                   0
                   0
                   3U
                    O


                           64 kbits/s, 7.5 fps
                   38.50

                   38.00

                   37.50
                           嘔圄 Best operating p이nt
                   37.00
                           a         b              c         d        e     f
                                                   Search region
                                                        (b)
     Figure 7.4. .Search regions and video quality for typical H.261
     encoalng. (a) viarnono-snapea .searcn regions; ID) viaeo quatity
     ror me corresponoing searcn regions.


7.4 FUTURE DIRECTIONS
ITU is presently developing a video conferencing standard for the general
switched telephone network (GSTN) and mobile radio. This standardization
effort is referred to as H.324 and is expected to be approved later in 1995.
The H.324 suite is a recommendation for real-time voice, data, and video over
 V.34 modems on the GSTN telephone network. It consists of five documents:
206                                                               CHAPTER 7




(1) H.324 systems,(2) H223 multiplex, (3) H.245 control, (4) H.263 video
codec, and (5) G.723 speech codec. H.261 provides coded video at bit rates
64 kbits/s and above, whereas the H.263 video coding standard proposed for
H.324 will provide coded video around 26 kbits/s.

ISO is working on MPEG-4 and will develop standards for audiovisual services
that can operate below 64 kbits/s. The ITU effort is intended to be a near-term
solution, whereas the long-term solution for very low bit-rate audiovisual
services might be a merger of the ITU and ISO efforts.




7.5 TO PROBE FURTHER
The H.320 and H.261 Recommendations are described in the ITU documents
[67] and [66]. In [25], Carr provides additional details on the early efforts
for the development and testing of a video teleconferencing standard. The
methodology adopted for the development of H.261 and the evolution of the
standard is discussed in [147]. Brief descriptions of the H.261 standard and
comparisons with JPEG and MPEG are also prcsented in [138] and [7]. The
role of the ioop filter in H.261 is investigated in detail in [153]. The status of
H.324 is summarized in [174].
                                                                      8
      PROCESSING REQUI之EMENTS




8.1 INTRODUCTION
In Chapters 1 to 7, we have examined the core algorithms of the image and
video compression standards without regard to their hardware implementation.
However, ease of implementation and low processing requirements are among
the key factors that influenced the final recommendations of the standards
committees. In the past, the computational needs of intensive image-processing
tasks were satisfied with expensive custom multiprocessor systems. However,
the standards committees believed that it would be easier for the industry to
accept the new standards if low-cost implementations were possible.

The latest RISC (reduced inst끄ction set computers) architectures have enough
compute power for the implementation of some of the video standards. For
example, workstations from DEC and Hewlett-Packard can perform MPEG-i
decompression at 30 frames/s (fps) now and real-time MPEG-2 decompression
perhaps in the near future. For video teleconferencing using the H.261 standard,
general-purpose processors can already encode and decode 8 to 10 QCIF frames
per second. However, even the latest designs cannot adequately address the
processing requirements of some of the standards, such as real-time MPEG
encoding. In such cases, custom hardware may be necessary. In the next eight
Chapters, emphasis will be on the hardware implementation of the image and
video compression standards. Specifically, in this chapter we examine their
processing requirements. In later chapters we discuss design tradeoffs, the
most common hardware designs for the core algorithms (like the DCT, motion
estimation, and entropy coding), and IC designs of various video processors.
208                                                                           CHAPTER 8




8.2 MEASURING COMPLEXITY
There are many different measures of algorithmic complexity. For example,
in digital signal processing, one measure is the number of multiplications and
additions. For the video compression standards, a good measure of complexity
is the number of required RISC-like operations. For example, the evaluation
of ri = a + b, where a and b are data stored in external memory, and ri is a
processor register, requires two data loads and one addition, for a total of three
operations. For signal and video processing algorithms, the total number of
operations is usually expressed in MOPS (million operations per second) or
in GOPS (giga operations per second).

Example.（노nsider the MOPS requir帥ents f야 co呻岫ng a two-d油ens幻nal
(2-D) DCT on a QCIF frame. Using row-column decompositions on 8 x 8
blocks, a 2-D DCT can be computed by performing 1-D DCTs on the rows of
the input data matrix followed by 1-D DCTs on the columns. An eight-point
l-D DCT is given by
                                 S

                          Vi=   >二CjkXk,
                                k=1
                                          i   =   l,   2,   ．   ·   ·   ，8,
                                                                                    (8.1)


where y, denotes the output elements, Xk denotes the input data, and C1k denotes
the DCT coefficients. From the above, this implementation requires at least:
eight image data loads, eight coefficient data loads, eight multiply-accumulate
operations, and one data store operation, for a total of 25 operations per pixel.
Because of the row-column decomposition, an 8 x 8 DCT will require 2 x 25
 x 64 = 3,200 operations. In a YCbCr QCIF frame, with a 4:2:0 sampling ratio,
Y has 176 x 144 pixels and Cb and Cr have 88 x 72 pixels each. A complete
frame has 594 8 x 8 blocks. At 15 fps, the total number of operations is 15 x
594 x 3,200 = 28.5 MOPS. For a CIF frame, a similar implementation would
require 114 MOPS.

Following the same approach, one can estimate the processing requirements
of the various compression algorithms for different frame sizes and data rates.
Table 8.1 shows the MOPS requirements for compression and decompression
using H.261 on CIF resolution sequences at 30 fps. These estimates were
computed assuming fast implementations of the DCT or IDCT algorithms and
logarithmic (instead of exhaustive) searches for motion estimation.
                                                                            209
Processing Requirements




                          Compression                MOPS
                ROB to YCbCr                             27
                Motion estimation                       608
                (25 searches in a 16 x 16 region)
                lnter-flntraframe coding                  40
                 Loop filtering                           55
                 Pixel prediction                         18
                 2-D DCT                                  60
                 Quantization, zig-zag scanning           44
                 Entropy coding                           17
                 Frame reconstruction                     99
                 Total                                   968

                 Decompression
                 Entropy decoder                          17
                 Inverse quantization                      9
                 Inverse DCT                              60
                 Loop filter                              55
                 Prediction                               30
                 YCbCr to RGB                             27
                 Total                                   198

                                                                n and de-
       Table 8.1 MOPS requirements for H.261 compressio
       compression.


                                                       200 MOPS and that is
 From Table 8.1, decompression requires approximately
                                                          DSP (digital signal
 now easily achievable by several general-purpose RISC or
                                                           than 1,000 MOPS
 processing) processors. However,an encoder requires more
                                                           a general-purpose
 of processing power, which is outside the capabilities of
 processor at this time.

                                                            mentation of MPEG,
  Table 8.2 shows MOPS estimates for the baseline imple
                                                                s computed with
  for different frame sizes, and different percentages of frame
                                                              tes are for 30 fps,
  bidirectional motion estimation (B-frames). These estima
                                                      is, color transformations),
  assuming no preprocessing or postprocessing (that
                                                           assume that a HDTV
  no audio, and no other system-related operations. We
                                                                 1440 level). For
  frame is 1440 x 1152 pixels(MPEG-2, Main profile, High-
 210                                                                       CHAPTER 8




                    Compression           SIF        CCIR 601     HDTV
                    No B-frames           738           3,020     14,498
                    20% B-frames          847           3,467     16,645
                    50% B-frames        1,
                                          011           4,138     19,865
                    70% B-frames        1,120           4,585     22,012
                    Decompression
                    No B-frames               96          395      1,898
                    20% B-frames             101          4巧       1,996
                    50% B-frames             108          446      2,143
                    70% B-frames             113          466      2,241

       Table 8.2 MOPS requirements for MPEG compression and de-
       compression ar iu rps.



comparison, Figure 8.1 shows the trends in computing power for general-
purpose DSPs, RISC processors, and programmable image processors. From



            10000 -
                                               Programmable
                                               Video Processors




          m口O>
             1000 -
                                 Programmable DSPs




                 100 H山                                 Gener키 Purr兀Se
                                                        Micr야玎ocessors




                          1989   1991         1993     1995       1997     1999



       Figure 8.1 Trends in the performance of programmable proces-
       sors.

the data in Figure 8.1, it is clear that general-purpose processors will need
                                                                                            211
Processing Requirements




                                                 be used for real-time video
to integrate additional features before they can
encoding and decoding.




8.3 DISTRIBUTING THE LOAD
                                                  in JPEG, MPEG, and H.261
In Figure 8.2, we show the main processing flow
                                                        y that is common among
encoding. Note that, there is considerable functionalit
                                                     e three key functions: (1)
these three compression standards. They all includ


                                            JPEG Coding Functions
                                                                                        1
                                                                         >   Entropy i
                                OCT   Hd>
                                                Quan虹카ion     HH=   m{



                                                                             Encoding I

                                                     古
                                                                                        1



                                                  Inverse
                                                Quan打乙ition                      V
       V                                              立                        Buffer

     M에Kfl                                         Inverse
                                                     DCT
    Es恤nat幻n
                          Predicted Picture


                 M아ion                            Ref이ence
           나＞ Compens帥on   <＝
                                叫

                                                   Memory




       Figure 8.2   Main processing flow in JPEG, MPEG, and H.261
       encoding.

                                                     the DCT coefficients, and
 the computation of the DCT, (2) quantization of
                                                        onal functions, namely,
 (3) entropy coding. MPEG and H.261 share additi
                                                                on to these key
 motion estimation and motion compensation. In additi
                                                             icant computational
 operations, any implementation must also allocate signif
                                                     audio processing, data 110,
 power for data preprocessing and postprocessing,
                                                                    g may include
 and host and display interface. For example, data preprocessin
                                                         (RGB    to  YCbCr), and
  noise filtering, deinterlacing, color transformations
                                                      interlaced transformations,
  subsampling. Postprocessing may include raster-to-
 212
                                                                 CHAPTER 8




 color transformations, and audio-video synchronization. Since no single
 programmable processor has enough processing power for all these operations,
 parallel processing architectures are not uncommon for video processors.

 Until recently, there were few commercially available video processing ICs.
Furthermore, their functionality was limited to low-level operations, such
 as filtering. This was due to the limitations in circuit integration and that
 only low-level imaging functions had a large enough range of applications
 that could justify the development of special hardware. The emergence of
standards for image and video compression opened new market areas, such
as multimedia computing, video set-top units for interactive television, and
HDTV. It is now commercially viable for IC manufacturers to invest in the
design and development of a new generation of image and video processing
ICs.

Designs of video processors range from fully custom architectures with
minimal programmability to fully programmable multiprocessor architectures.
Their architecture depends on the speed requirements of the target application
and the constraints on circuit integration, pe汗ormance, power requirements,
and cost. Regardless of the implementation details, the general design theme
is to use either a DSP or a RISC core processor for main control and special
hardware accelerators for the DCT, quantization, entropy coding, and motion
estimation.




8.4    TO PROBE FURTHER
 The main scope of this chapter was to present some estimates of processing
 complexity for the image and video compression standards. In related work,
Fujiwara et al. [49} and Guttag et al. [65] present similar results for the
real-time implementation of the H.261 standard. Guttag et al. estimate the
total number of operations to be close to 1,200 MOPS, very close to our
estimate. Fujiwara et al. use a more conservative RISC model and thus provide
much higher MOPS estimates. For example, they estimate that a single
multiply-accumulate operation will require five (instead of three in our model)
instructions. Without using fast algorithms for the DCT, and by assuming
full search (instead of logarithmic search) for motion estimation, their total
estimated number of operations is approximately 3,400 MOPS. However, in
Processing Requirements                                                   213




relative numbers, there is general agreement that motion estimation is the most
compute-intensive operation, requiring nearly 60 percent of the processing
power of a H.261 or MPEG encoder.

In [201], Zhou et al. provide a detailed analysis of the MOPS requirements
for MPEG video decompression on a general purpose RISC-like processor.
For a 4 l뇨1bits/s, CCIR 601 input stream, they estin垠te that re카七n祀 MPEG그
dec以ling requires close to 400 MOPS. The authors count one multiplication as
 four generic operations and assume that each group of pictures (GOP) has one
I-frame, four P-frames, and 10 B-frames. The above estimate does not include
 the computational requirements for the final color conversion from YUV to
RGB.
                                                                         9
                           RISC AND DSP CORES




9.1 INTRODUCTION
As noted in the previous chapter, most video compression ICs utilize either a
RISC or a DSP core as their central controller and processing unit. By RISC or
DSP core we imply a standard programmable processor, without the 110 pads,
buffers, and associated circuitry. These parts are replaced by custom circuits
that interface to the rest of the architecture. The main goal in using a processing
core is to take advantage of existing hardware and software resources (such as
arithmetic processing units, memory, operating system support, and language
compilers) and to minimize the design time of a more complex and dedicated
IC. In this chapter we describe the basic architectures of a RISC core and a
DSP core and some of their similarities and differences.




9.2     THE RISC CORE

9.2.1    Architecture

The fundamental principle of reduced-instruction-set computers is to achieve
high performance with the minimum amount of complexity. As a result,
instructions are very simple and perform mostly register-based operations.
Register-to-register operations allow most of the instructions to take place
inside the chip. This allows for faster implementation (shorter clock cycles)
and simpler control. A RISC core dec어jes and executes load, store, arithmetic,
  216
                                                                         CHAPTER 9




                                                    MEMORY DATA BUS

                                                                   中


                                                            工雖韓吐      工詐奭
                                                                   MUX
                                                \
                中
                                 \ /
                                 1




          REGISTER                          二
            디LE
                                                H




                                        룬
            中

                                                     1




                                      MEMORY ADDRESS BUS

                    Figure 9.1       Block diagram of a RISC core.



and control transfer operations. The only instructions that
                                                            access external data
are the load and store operations. During arithmetic opera
                                                            tions, the processor
will read two registers, perform an operation, and store back the
                                                                  result into the
register file.

Figure 9.1 shows a typical data path of a RISC architecture
                                                                   . It includes a
register file with source and destination latches, an ALU
                                                           (arithmetic and logic
unit) and a program counter (PC). A RISC processor
                                                       may also have additional
registers for data and instruction addressing or other contro
                                                              l related functions.
Most RISC designs use the same ALU to compute both
                                                            algebraic operations
and memory addresses for load and store operations. The
                                                           justification for such
a design is that because during load and store operations
                                                          the ALU is not busy,
such an implementation does not cause any perfor
                                                    mance penalty.

Table 9.1 shows three typical RISC instructions from
                                                       the Berkeley RISC-I
processor: an integer add, a memory read, and a condi
                                                         tional jump. Their
corresponding instruction formats are shown in Table
                                                       9.2. For register-to-
register instructions, an operation (specified by OPCO
                                                       DE) is performed on
the registers specified by SRCI and SRC2, and the result
                                                             is stored in the
RISC and DSP Cores                                                        217




   ][nstruction    Operands           Operation           Comments
       ADD        Rs, S2, Rd       Rd = Rs + S2        Integer addition
       LDL        (Rx)S2, Rd       Rd = M[Rx + S2]     Memory load
       且4P        CON, S2(Rx)      尸C = I코工 + S2       Conditional jump

                  Table 9.1   Examples of RISC instructions.



           OPCODE     DEST     SRC1 SRC2
           OPCODE     DEST     SRC1 I匹MEDIATE OPERAND
           OPCODE     DEST        IMMEDIATE OPERAND

              Table 9.2 Examples of RISC instruction formats.



register specified by DEST. In some instructions, the last field may denote an
immediate operand instead of a register source. For memory accesses, SRC1
specifies the index register and SRC2 specifies the offset. Data is exchanged
by the register specified in DEST. For program control instructions, like
branches, multiple operand fields may be combined to generate a PC-relative
address.

Typical RISC processors execute on the average only one instruction per cycle.
Superscalar designs may execute multiple instructions per cycle by utilizing
in parallel the ALU and the floating-point unit.



 9.2.2     The Processing Unit

The original RISC machines had a very simple ALU and no on-chip multiplier.
Multiplication was performed using shift-and-add instructions or external
math coprocessors. Now, many designs include dual fix-point ALUs and
an additional on-chip floating-point unit that can operate in parallel with the
 ALUs.

 RISC architectures were developed as general-purpose compute engines.
 As such, they provide support for virtual memory addressing. Because of
 218                                                                          CHAPTER 9




                          Ins打uction
                            Cache

                                                                Data Bus
                    中                                ＜그＝m七：
                                                          >

                  F키SC                 F幻ating   8m亡으드
                                        Point
                   Core
                                        Unit     aOEm>

                    수                    수                         =>
                              寸
                                                         4口H{
                                                                Address Bus
                            Da治
                            Cache
                                                 수

              Figure 9.2      Typical RISC-core based architecture.



their high-speed internal clock, it is not cost effective to connect external
memory directly to a RISC core. Instead, a RISC core communicates
with external memory via data and inst끄ction caches. Figure 9.2 shows a
typical configuration of a RISC-core based architecture. It includes the core
processor, an instruction cache, a data cache, and a memory-management unit.
The memory interface unit usually includes a translation look-aside buffer
(TLB) that translates the virtual addresses to physical memory space.




9.3     THE DSP CORE

9.3.1   Architecture

In contrast to RISC architectures that were developed for general-purpose
computing, DSP designs are optimized for the efficient implementation of
digital signal-processing applications. The core operation of most DSP
algorithms is the multiply-accumulate operation 1' = b + ax. Hence, it is
not surprising that DSP architectures are optimized for this operation. For
example, to execute the operation r = r + a x, where r denotes an accumulator
register, a typical general-purpose processor would require two memory loads
RISC and DSP Cores                                                                    219




        Program Address Bus

                      V                         V                    V
                   Pro아am                     Data                 Data
                                             RAM-A                RAM-B
                   LAM/ROM
                      L:i
                                                                         Data Bus-A
                                                                         Data Bus-B


                                         Program Data Bus

                             AGU次                            Multii川er
        Program
        Con打이                AGU-B                             ALU
                                                             Registers
                             Address
                            Generation                      Accumulators
                                                             다ocessing
                                                               Unit


             Figure 9.3       Block diagram of a typical DSP core.



(for reading a and x into local registers), one multiplication, and one addition,
for a total of four instructions. A programmable DSP can execute the same
operation using a single instruction by using multiple data and instruction
buses and by exercising in parallel all the internal function units.

Figure 9.3 shows the block diagram of a typical DSP core. It has a Harvard
architecture, i.e., separate data and instruction buses and separate instruction
and data memories, a processing unit, two data memories with their own
address generation units (AGUs), a program controller, and program memory.
The processing unit includes a parallel multiplier, an ALU, accumulators, and
registers.



9.3.2   Instruction Format

Most DSPs have a very long instruction width ( VLI끼 format. All instructions
are of the same size and execute in a single cycle. Each field of an instruction
 220                                                             CHAPTER 9




        ALU          AGU- l      AGU그          PC         IM?汀EDIATE
       OPCODE       OPCODE      OPCODE       OPCODE        OPERANDS

                 Figure 9.4    Typical DSP instruction format.



         Instruction    Operands      Operation        Comments
         RPTB           S            RE= S            Repeat a block
                                     RS := 尸C + 1     of instructions
         MPYF3          Si's끽 1끄     Z끄 = Si )< S2    Multiply-
         II ADDF3       S3, S4,D2    D2 = S3 + S4     Accumulate

                  Table 9.3    Examples of DSP instructions.



controls a separate unit of the architecture. For some instructions, multiple
fields may be combined or shared for immediate ope及nds (Figure 9.4). In
a typical cycle, a DSP will fetch the next instruction, do two simultaneous
data reads and one data write, perform a multiply-accumulate and an ALU
operation, and update all data address generation units.

To demonstrate the special nature of DSP instructions, Table 9.3 shows
two instructions from the T卜4S320C30 processor. Other DSPs have similar
instructions. The first entry (RPTB) is a repeat-block instruction. It allows
a block of instructions to be executed repeatedly without any ioop penalty.
RE is the repeat-end register and is loaded with the address of the end of the
block (5). RS is" the repeat-start address register and is loaded with the next
value of the program counter. The number of times the loop will be repeated
is determined by the value of a separate repeat-counter register (RC).

The second entry in the table shows a multiply-accumulate instruction. The
two vertical lines next to ADDF3 show that addition will be executed in
parallel with the multiplication. The source operands (Si - S4) can be either
register values or pointers to memory locations. If they are address pointers,
then addressing operations can be performed in parallel with the multiply-
accumulate operation. For example, the value of an address pointer could be
incremented or decremented by a specified value.
RISC and DSP Cores                                                          221




Efficient data- address generation is very important for DSPs. Hence DSPs
are the only processors to incorporate modulo-like arithmetic in data-address
generation or hardwired support for bit-reverse address generation. These
features are essential for the efficient implementation of filtering or FFT
algorithms.

Since most of the DSP algorithms have short processing loops, most of the
time-critical data, and usually all the instructions,fit on-chip. Thus, most DSPs
have simple memory interface circuitry and no data or instruction caches. For
110 intensive operations they rely on internal or external DMA (direct memory
access) units. Architectures with limited internal instruction memory and data
paths may also have a loop-instruction cache for storing instructions for a loop
operation.




9.4 RISC VERSUS DSP
Both RISC and DSP processors share the same philosophy: simpler is
faster. Hence, both have simple addressing schemes and a limited number
of instructions. Both rely on fast access to the on-chip data, either in local
memory (DSPs) or registers and caches (RISC). In general, DSP cores can
provide better performance than RISC cores, specially for signal-processing
applications. However, RISC architectures have better support in operating
systems and compiler design and they can be used in a larger range of
applications. The VLIW structure of a typical DSP makes it very difficult to
program them and to fully utilize their processing power. DSPs have more
efficient loop control (zero overhead loops) and data addressing but limited
data-space addressing power. In general, companies with long history in
DSP design prefer to use and expand their DSP cores for the design of video
 processors. On the other hand, new developers of video ICs tend to use RISC
cores, most probably because they provide better programming flexibility and
faster time to market.
 222                                                            CHAPTER 9




 9.5 TO PROBE FURTHER
 Both RISC and DSP architectures are relatively new. In the mid-1970s, G.
 Radin led the development of the first RISC-like processor, the IBM 801
 minicomputer [165]. However, RISC designs did not find their way into
 low-cost workstations until the late 1980s, after the success of the RISC and
 MIPS projects at the Universities of Berkeley [176] and Stanford [71]. The
 book on computer architecture by Patterson and Hennesy [156], the leaders
 of the Berkeley and Stanford projects, covers in depth all the hardware and
 software design issues in the development of a modern RISC processor. For
 a detailed description and evaluation of specific RISC architectures, a book
 edited by Slater [1801 has articles on most of the commercially available RISC
 processors.

In related work, Patel and Douglas [155] describe the architectural features of
the Intel i860, and Shacham eta!.[177] present the series 32000/EP processor
from National Semiconductors. Both of these processors merge DSP-like
functionality into a RISC core. The 32000/EP is a 100 MIPS/50 MFLOPS
superscalar RISC processor with two integer units, a floating-point unit, and
a DSP unit with a 16 x 16 fix-point multiplier. Special instructions allow
the efficient implementation of complex-arithmetic operations, a feature very
useful in DSP algorithms like the FF1'.

Programmable digital signal processors became very popular after the success-
ful introduction of the first TMS320 processor (the TMS320!0)from Texas
Instruments (TI) in 1982. Since then, TI continues to lead in the DSP market
with a complete family of fix-point and floating-point processors[184]. Other
major developers of DSPs are AT&T, Motorola, Analog Devices, LSI Logic,
Zoran, and SGS-Thomson. Many of them are expanding now in the video
processing market.

A detailed description of the design of a typical DSP processor is given by
Fellman et al. [47]. A recent book edited by Bayoumi and Swartzlander
[16] covers the current developments in the design of programmable DSPs,
DSP cores, and image processors. For a more detailed description of specific
designs, Michalina [134] presents a very good overview of the DSP cores
available from SGS-Thomson. The Motorola and TI DSP cores are described
in [113] and [103]. For a short description of most commercially available
RISC and DSP Cores                                                223




DSPs, EDN, a trade magazine published by Cahners Publishing, publishes
annually a DSP-chip directory [118].
                                                                 10
   Al之（표-IlTECTUl之ES FOR THE DCT




it).! INTRODUCTION
                                                          DCT in digital image
Due to the importance of the two-dimensional (2-D)
                                                         s algorithms and archi-
processing, particularly in video compression, variou
                                                                 methods can be
tectures have been proposed for its implementation. These
                                                             includes techniques
divided into two main categories. The first category
                                                                DCT is a typical
from linear matrix analysis and decomposition. Lee's fast
                                                             es algorithms from
example of this category. The second category includ
                                                               algorithm fits into
polynomial and number theory. For example, Winograd's
                                                       into algori thms that either
this class. Both categories can be further partitioned
                                                                ple, with a row-
use or do not use row-column decompositions. For exam
                                                          using one-dimensional
 column decomposition, the 2-D DCT can be computed
                                                          ithms that do not use
 DCTs, allowing for simpler implementations. Algor
                                                                     nt but require
 row-column decompositions are more computationally efficie
 complex hardware.
                                                            thms is the number
In general, a basis of comparison of the various DCT algori
                                                            for a VLSI imple-
of multiplications and additions they require. However,
                                                                     e complexity
mentation other factors are also important. These factors includ
                                                   and  powe    r,  comp  lexity of
of control logic, requirements for memory, size,
                                                           transf   orm  using  the
interconnect, and efficient implementation of the inverse
                                                              lications but have
 same hardware. Polynomial transforms require fewer multip
                                                             amon     g processing
 irregular structure and complex interconnection schemes
                                                                 nt for small-size
 elements. Furthermore, they are not as computationally efficie
                                                                   re implementa-
 transforms. Hence, these algorithms may be used for a softwa
 226                                                                                CHAPTER 10




 tion on a general purpose processor, but they are seldom the basis for dedicated
 DCT processors in video codecs.

 Single-chip video codecs need to integrate the DCT-IDCT hardware with a
 core processor, an entropy coder, and other circuitry. For such strict size
 requirements for the implementation of the DCT, two techniques seem to
 be widely used: (I) vector processing using four parallel multipliers and (2)
 parallel processing using distributed arithmetic. These designs have a regular
 structure, have simple control and interconnect, and achieve a good balance
 between performance and complexity of implementation.




10.2     VECTOR PROCESSING
Using matrix notation, let F denote the output of an N x N DCT for input 1.
Then
                                F = CfCt,                            (10.1)
where C is a matrix with the cosine basis functions, and Ct is the transpose of
C. Using a row-column decomposition, F can be computed using 1-D DCT
transforms as
                                  Y= Cft,                               (IO.2a)

                                       F = CYt = CfCt,                (10.2b)
where }' is an intermediate product matrix. (The columns of Y correspond to
the output of the I -D DCTs of the rows of f.) A 2-D transform can thus be
computed by applying l-D transforms, first on each row off and then on the
transpose of 1
             「'. Figure 10.1 shows a block diagram of such an architecture.

For N=8, (10.2) can be written as
                                   8

                     Yk,1 = >二 Cm,(fk,m, 1, k = 1. 2. ...,8.                             (10.3)
                                  m=1

From (10.3), the evaluation of each row of Y requires eight eight-point inner
products. However, due to the special properties of the DCT coefficient
matrix, it can be shown that
                                       4

                      Yk,
                            ! =    Z
                                  m=1
                                           Crn,
                                                  1Uk,m,   1=
                                                                1,
                                                                     3,
                                                                          5.
                                                                               7,
                                                                                        (10.4a)
Architectures for the DCT                                                       227




                                             Transposition
                                               Mem이y




                                                             b卜弓m
                       尸＝ 쇼드   Hm卜늠m                         弓스弓O
                n
                                              1-O DCT                  [>

                =
                                                                    Output



      Figure 10.1 . Architecture for two-dimensional DCT using row-
      coiumn transrormauon.


                                        4

                      Yk,1= 乞 Cm,1Vk,m, I = 2,4,6,8,                         (10.4b)
                                       m=1

where Uk,m = fk,m + fk,8-m+1 and Vk,m = fk,m - fk,8-?IL+1, for m = 1 to
4. The above equations imply that an eight-point DCT can be computed
using two four-point DCTs, provided that one preprocess the original data to
generate the u and v sequences. (This is usually the first stage in most of
the butterfly-based fast DCT algorithms). Using the above formulation, the
number of multiplications is reduced by a factor of two and each row of Y can
now be computed using eight four-point inner products.

Figure 10.2 shows a block diagram for the implementation of the 1-D DCT
using an array of four multipliers. The preprocessor computes the n and v data.
Each column-multiplier is a parallel multiplier based on the modified Booth
algorithm. The four products from the multipliers, after appropriate scaling,
are summed into the output accumulator. A Wallace tree-adder is usually used
at this stage. In pipelined mode, this architecture allows a four-input inner
product to be computed each cycle, and an eight-point DCT to be computed in
eight cycles.
228                                                                               CHAPTER 10




                       工                       Pre-Processor
                                                                          立

                                                                  中g工닝8
              中
                                   H                                          m
                                   ＞口 工 닝 8
              긍
                                               +                              g
                                                                              工
                       느으H으＝ =>
              工
                                                   쁠읕三＞                            졀읕三＞
                                                                          느
                                                                              1
              1
                                                                              卜
                                                                          m
              卜
                                                                              m
                                                                          言
              m
                                                                              0
                                                                          三
                                                                          T
                                                                              0
              8
                                                                          큘
                                                                                  古
                                               Accum너카or


                                                              +
         Figure 10.2         Eight-point DCT using four parallel multipliers.


10.3 DISTRIBUTED ARITHMETIC FOR THE DCT
Distributed arithmetic is a technique that allows the hardware implementation
of a sum of products without using multipliers. By storing first a finite number
of intermediate results, a sum of products can be obtained through repeated
additions and shifting operations and without the use of any multiplications.
The technique allows the design of signal processors with a reduced gate count
and a very regular structure. Hence, it is ideally suited for integrating a DCT
processor into a video codec.



10.3.1    Technical Overview

Consider the evaluation of the following sum of products:
                                                          N


                                              y=   Z
                                                   m=1
                                                              amxm,
                                                                                          (10.5)
Architectures for the DCT                                                                                      229




where Xm denotes the input data and am are fixed coefficients. Assuming
(mostly for convenience and without loss of generality) that each Xm is a two's
complement binary number with B-bits of precision and that 佃m < 1, then
Xm can be expressed as
                                                                  B- i

                                   玩 = 出繫나 >＞恥끼                                                             (10.6)
                                                                  ;=   l

.., km小 . (3) :n 111八 :.i1 L: + ,..c_ n.1』4 k,1n ', , . 'd . , 4 nr 4; +144.. 1) 八，. 1              尸r1m4 n11,\ . , 스
 WlIUlG 工m I3 L1lG Jill    VU UI ;Lnl aiiu iia> a vaiuL; Ut 1;7IUl [ U UI j.                        \ l liL/. au 'J v뇨

formulation implies a decimal point next to the most significant bit (x뗏)). For
example, 1001 = -1 + 吉 = -0.875.

Substituting (10.6) into (10.5) yields

                                                     I   .,            B-
                                                                       쓰：Ji        ..      ]
                                        N
                            y=
                                        二
                                              am H' 胃 +                      , xY2"" 1 ·                    (10.7)
                                   mrrl
                                                     L
                                                     1                     7=1
                                                                           jrri            J

After an interchange of the order of summations,

                                 旦二'1스＝                  . ']                     스－           ..
                         y스나乞. am' 끼21'스；
                                 7= 1
                                        . amx累' '
                                            Lr1；二L            i                   711= 1
                                                                                                            (10.8)


Let
                                                                   N
                                        夙他和）= ＞二amx${).                                                     (10.9)
                                                                  m= i


Since xiV may only be either 0 or 1, FN(a, x(j) ) can take only 2" possible
values. These values can be precomputed and stored in a lookup-table (or
ROM). Substituting (10.9) into (10.8), yields
                                  B- i
                                          FN(a, x(0) ).
                           y = > 蜘他和）2' -                                                                 (10.10)
                                   j= 1


This is the key expression for the implementation of a sum of products using
distributed arithmetic. Multiplication by 2_i corresponds to a right shift by
one bit, hence, y in (10.10) can be computed using repeated table look-ups,
additions, and shifts.

Figure 10.3 shows a block diagram for the implementation of (10.10). Data
is processed bit-serially, the least significant bit first. After each cycle, the
230                                                                                                                                                     CHAPTER 10




       Figure 10.3 . Block diagram of a ROM-accumulator unit for the
       imp=ementation or sum or proaucts using aistrlDutea aritlimetic.


output of .he accumulator is shifted by one bit. The final sum is computed in B
cycles. Tr.:s circuit is commonly referred to as a ROM-accumulator (RAC).

As 帥exairple, IetN= 2, B= 4, a1 -0.125, a2 =-0.75, 幻 =-0.625 (1011), and
'2 = 0.25 0끄0). Table 10.1 shows the values of F2(a, xW) = a1x1j) + a2x1j)
for .7 = 0. : . 2, and 3. For convenience, the decimal point is shown explicitly.
From (1010) and B = 4. the summation can be expanded as


                                                                   (.
                                                                  r2    1)
                                                                                                 尻（O,   T   (7)
                                                                                                                        )
                                                                                       0
                                               d7)
                                                     0            0
                                                     0            l                    (i2= 1.010
                                                     l            0                    ai =0.001
                                                     I            l                    ai +Q2 = 1.011



                            Table 10.1 Lookup table data - Example.




  9=                        (3)
                                           '         + F2            (10.11)     (2)
        {{j   2   (a,   x
                                                                                                  i + F2
                                                                             x
                                                            (a,
                                       2
                                  )]
                                                                      (                )]   2_                    (a,       x   (1)
                                                                                                                                                i
Given (10.11), Table 10.2 shows the input and output data flow in the ROM-
                                                                                                                                      )]   2_       -    F2   (a,   x   ")
                                                                                                                                                                             ).
accumulator unit for this example. After four cycles, the final sum is y =
-0.265625 1.101111).
Architectures for the DCT                                                    231




             Bit     Input Data                      Adder
              j      Il (i)   (i)
                            2;2     Input-A       Input-B     Output
              3         I     0     0.001         0.000       0.001
              2         I     I     1.011         0.0001      1.0111
              1         0     0     0.000          1.10111    1.10111
              0         1     0     -0.001         1.110111   1.101111

         Table 10.2    Example of data flow using distributed arithmetic.



10.3.2    Implementation of the DCT

The design methodology of the previous section can now be directly applied
to the hardware implementation of the DCT using distributed arithmetic. For
B bits of data precision, let
                                              B- i

                                              k.m9-i
                            fk,m = -f｛았 + ＞二 /(i)                         (10.12)
                                              j= i


and                                           8

                             尻（Ci, /{'") ) = ＞二 CTfl,lfI之                 (10.13)
                                           tn=1


where f之 denotes the jth bit of /k,m. From (10.3), using distributed
arithmetic, an eight-point DCT can be computed as
              B- i

         1- ＞二尻（ci, f{") )2ej -F늉（.Cl,nfk
      11숯，                             /(0) ), 丸，1= 1, 2, .. . ,8.        (10.14)
              i= i




As before, each Yk,i can be computed using the ROM-accumulator unit shown
in Figure 10.3, where the size of the ROM is 256 words. The size of the
ROM can be reduced to only 16 words if we take into consideration that an
eight-point DCT can be computed using two four-point inner-products (see
equation (10.4)). In either case, an output will be available after B cycles.
However, since each row of Y (Yk,i, 1k,2, · · ·, Yk,8) utilizes the same fk,m data,
all row elements can be computed in parallel.
232                                                                 CHAPTER 10




Figure 10.4 shows a parallel implementation of the eight-point DCT-IDCT
using distributed arithmetic. For each row, first, the fk data vector is loaded


       k   Bus                  Uk   Bus
                                     BUS           Vk   Bus                 yk        Bus


                                                        日AC                  D          C


                                                        RAC                  0 H


                                                        日AC                  D HK


                                                        日AC                  D H


                                                        日AC                  DH
                                                        目AC                  0 -C

           0
                                                        日AC   中   口H＞   戶
                                                                             D    -
                                                                                        ::>
                                             -c=
                                                        RAC                 D



      Figure 10.4 Parallel implementation of an eight-point DCT using
      distributed arithmetic.

into the input registers (denoted by D). Then, data are processed bit-serially
by the bit-serial adders or subtractors to generate the u and v data. Two data
buses distribute the bits into eight ROM-accumulator units. Each RAC has 16
words of memory for the forward DCT and 16 words for the inverse DCT.
After B cycles, the outputs from the RAC units are loaded into the output
registers and then transferred sequentially to memory.
Architectures for the DCT                                                        233




10.3.3    Doubling the Speed of Distributed Arithmetic

In most video applications, the bit-length of the input data is usually eight bits;
however, to comply with the accuracy requirements specified by the standards,
DCT architectures employ a higher internal dynamic range. For 16 bits of
precision, an array of eight RAC units can complete an eight-point DCT in
16 cycles. This is half of the input data rate into the DCT unit. The output
rate can be increased by either doubling the clock of the DCT unit (not always
possible or desirable) or by increasing the processing rate of a RAC unit.

To increase the processing rate in distributed arithmetic, the RAC unit can
be modified to process two bits at a time from each operand. For example,
(10.11) can be rewritten as
       [F2(a, x(3) )2中' + F2(a, x(2) )]2e2 + [F2(a, x(') )2 ' - F2(a, x(0) )J. (10.15)
  y=

If we can access two F ( ) values simultaneously, then operations within a pair
of brackets (El) can be performed in one cycle and y can be computed in two
cycles. Similarly, an N-point sum of pr에ucts (see (10.10)) can be expressed
as
                             B/ 2

                   y = ＞二FN(a, x(2Jc中i) )2尸（2k-i)
                             k=1
                             B/ 2- i
                                       FN(a, x(2I) )2_2c_ FN(a, x(0) ).      (10.16)
                         +   ）二
                              k=i


The above formulation allows odd-numbered and even-numbered bits to be
processed in parallel.

Figure 10.5 shows the architecture for a modified RAC unit that process data
at double the speed. Data is still processed bit-serially, but two bits at a time.
This design requires an additional adder and twice the ROM size of the original
design. For 16-bit data, an array of eight modified RAC units can compute an
eight-point DCT in eight cycles; that is, at the same speed as an array of four
 parallel multipliers.
  m
                                                                          CHAPTER 10




                             ROM 伯r
                                                  >        1/2
                             Odd Bits
                                             H{
          r.
                             ROM 化r                   jH
                                                                 古 V
                                                                 Accum.
                                         ,        >        +
                             Even Bits
                                                                            y


               Figure 10.5     Block diagram of a modified RAC unit.


10.4 COMMERCIALLY AVAILABLE DCT
     PROCESSORS
SGS-Thomson makes three DCT (IDCT) ICs. The STV3200 operates at a
maximum pixel rate of 15 MHz and supports block sizes from 4 x 4 to 16
 x 16. The STV3208 is a dedicated 8 x 8 DCT IC and operates at pixel rates
up to 20 MHz for double precision or up to 27 MHz for single precision.
Both IC5 use nine bits (tw& s complement) for input pixel data and 12 bits
for coefficient and output data. The IMSA12l can perform 8 x 8 DCTs, 8
>S IDCTs. or low-pass filtering. It supports pixel rates up to 20 MHz. Its
dynamic range is 12 bits for input and output data and 14 bits for the fixed
coefficients. Internally, it uses distributed arithmetic with 16 bits of precision.

The Zoran ZR36020 is an 8 x 8 DCT-IDCT IC. It supports data rates of
15 and 21 Mbytes/sec. The Zoran processor complies with the normative
requirements of the JPEG standard regarding DCT or IDCT accuracy. It uses
16 bits of precision (two's complement) for the coefficients and either eight or
nine bits of precision for the data (unsigned, with or without internal shift by
128. or in two "s complement).

From LSI Logic. the L64735 is a DCT processor for 8 x 8 data blocks. It uses
12缸ts喀ned DCT coeffici帥ts and supports a max油帥 data rate o口이4Hz.
For higher data rates, the L64730 DCT processor can operate at 40 MHz. A
separate DCT quantization processor, the L64740, is also available.
Architecturesfor the DCT                                                   235




10.5 TO PROBE FURTHER
The efficient implementation of the 2-D DCT is still an area of active research.
Wolter et al. [196] provided the basis of our classification of 2-D DCT
algorithms. A detailed description of an architecture that uses two four-
multiplier arrays is given in [91]. The authors also provide extensive details
on the design and configuration of the transposition memory. A similar
four-processor architecture is also used by Ruetz et al. [172] for the DCT
processor in a multichip H.261 coder from LSI Logic. The SGS-Thomson
chip-set for image compression is described in [12].

The first widely known description of distributed architecture was published
in the early 1970s by A. Peled and B. Liu [157]. A tutorial by White [194]
provides additional examples and optimization techniques. M. T. Sun et al.
were among the first to present a DCT implementation based on distributed
architecture [182]. A design that uses the modified RAC unit is presented in
[189]. Distributed arithmetic can also be used in butterfly-based data flows.
Such a design is described in [361. The integration efficiency of distributed
arithmetic is best demonstrated in the work by K. Aono et al. [9], where a
DCT core is part of a single-chip video codec.
                                                                   11
                   HARDWARE FOR MOTION
                            ESTIMATION




11.1     INTRODUCTION
Typically, two consecutive frames of a video sequence are very similar. This
observation is the basis of block-based motion-compensated coding, where a
frame is coded based on its difference from another frame. In practice, frames
are divided into blocks. For a block in the current frame (called the reference
block), motion estimation is the process of finding a block in the prior frame
that matches best (according to a given criterion) its characteristics. A motion
vector identifies the position of the best block relatively to the reference block.
The search for the best matching block is done in a rectangular 町ea (called
the search window) around the relative position of the reference block. Figure
11.1 shows a search window that extends p pixels to the left and top and p - 1
pixels to the right and bottom of an M x N reference block. This is usually
referred to as a [-p, p - 1] search window. In most video applications, the
reference block is 16 x 16 pixels and the search window is 31 x 31 pixels (p
= 8).




There are many criteria and techniques for finding a motion vector. The mean
absolute error (MAE) criterion offers a good tradeoff between accuracy and
complexity. Under the MAE criterion, for a displacement vector (i,i) ' the
distortion between two blocks is defined as
                   入才 寸 1 N- i

         D（自j) = ＞二 ＞二 Irm,n - Sm+i,n+j , i,3 E [-p,p小 1],
                   m=O n= O
238                                                                                           CHAPTER 11




        -p
                       0           j   N-i                         N+p-2


             i                                  -       -    I
                                                             1
                                                             1
                                                             1
                        ／즈
                                            '       -       "'   勺＼,   Candidate Block
                                                                       (from another frame)
       M-i
                        / \
                             ;\'        "




                     / N
                                                                   Search window
                                                                    [-I工 p川
                                                                   万／
      M+p-2
                 Reference             卜加tion Vector (ii)
                  테ock


      Figure 11.1 Search window in motion estimation with range
      [-p,p- 11.


where r is the reference block and s is a candidate block. The motion vector
is the displacement vector for which D(i. j) is minimum. When the reference
block is compared with all possible candidate blocks in the search area, the
process is called full-search block matching.

Suppose the evaluation of r = r + a - bl requires five operations (two data
loads, one addition, one subtraction, and one absolute value), using full-search,
at least 5M1\T(2p)2 operations are required for one motion vector. For video-
conferencing at 15 fps (using CIF frames, 16 x 16 blocks, and p = 8), close
to two GOPS are required for motion estimation. Since no single processor
can achieve such high throughput, a variety of parallel architectures have been
used for the hardware implementation of motion estimators.




11.2 DATA FLOW DESIGN
Without loss of generality, let us consider the problem of motion estimation
for blocks of 16 x 16 pixels and a search range of [-8,71 pixels. If we shift
the coordinate system so that there are only positive pixel indexes, Figure
Ha凡／ware for Moti가'iE釘加恤i이'1                                                    239




11.2 shows the pixel coordinates for a 16 x 16 reference block and the
corresponding 31 x 31 search window. During the block-matching search, the


                    (00)        (0,15)     (0,30) (0,0)
                       S                                r




                                                              (15,15)
                                                     Reference Block
                           SI        s2

                    (30,0)                 (30,30)
                           Search Window



      Figure 11.2 . Modified pixel coordinates for a 16 x 16 reference
      DIOCK anu its i I x i i searcn winuow.

four corner pixels of the search window are used only once, however, all other
pixels are used in multiple search positions. For example, pixel s0,15 is used in
the evaluation of 16 different distortions: D(0,0), D(0, 1), · · ·, D(0, 15). If the
pixels from the search window memory are distributed to multiple processors,
then one can compute multiple distortions in parallel.

Figure 11.3 shows such an implementation of a motion estimator using a
one-dimensional array processor with 16 elements. Each element in the array
can compute a separate distortion value, and 16 distortion values can be
computed in parallel. To compute all 256 distortions, the reference block has
to be repeatedly scanned and processed 16 times. Since the width of the search
window is double the width of the reference block, improved performance can
be achieved by using two data ports for the search memory. Port si receives
data from the left half of the search window and port s2 receives data from
the right half (see also Figure 11.2). Data from both ports are distributed to all
proces計咽 이en妃nts that select the appr아）nate inputt뇨ough a 剛lti幽xer.

Table 11.1 shows in more detail the pixel data flow for the parallel computation
of the first 16 distortion values. Pixels from the reference block and the
search window are processed sequentially, row by row. For a given vertical
displacement i (i = 0, 1, · · ·, 15), PE-0 computes D(i,0), PE-1 computes
D(i, 1), and PE-15 computes D(i, 15). Pixels from the reference block move
240                                                                CHAPTER 11




        Reference             Search Window
       미ock Memory               Memory

                                            t2




        mux                 mux                       mux

         6 \7               寸 \7
          la-bi              la-bi                     la-bi


         古寸                 古也                        古     百H
         Accum.             Accum.                    Accum.



                  PE-O               PE-1                        PE-15
                                                                         MV
                           COMPARATOR UNIT                           d>




      Figure 11.3 Architecture for motion estimation using a 16-
      processor array.


among processors through a series of delay latches. Hence, a pixel that is
available to one processor at time t, it will be available to the next processor
at time t+1. Referring to Figure 11.3 and Table 11.1, the operation of this
motion estimator can be described as follows.

Let acc) denote the accumulator register for processor j. At time t = 0, PE-0
computes acco = 1i'0,o - s0,0卜 No data is available to the other processors.

At t = 1, PE-0 computes acc0 = acc0 + 1To.1 - 80,11. Pixel ro,0 is now available
to PE-l, which computes acc1 = 1i-o,o - so.il.

At t = 15, pixel r0,0 reaches the last processor and from this time on all
processors will be utilized 100 percent.
Ha,dware for Motion Estimation                                                                    241




 Cycle          Input Data                               Processor Inputs
 Time         r     sl     s2                PE-O             PE-1                   PE-15
     0     ro,o       3o,o               To,o, so,o

     1     TO,i       SO,l               r0,1, s0,1        T0,0, 80,i

     2     TO,2       30,2               To,2, 30,2        r0,1, sO,2


                                         i                 :.
     14    TO,14      30,14              TO,14, 3o,i.      T0,13, SO,14
                                                                                   T0,o, So,i5
     15     T0 ,15    SO,15              TO,15, SO,15      T0,14, SO,15
                                                                                   To,l, SO,16
     16    ri, 0      Si,o      SO,lO    Ti,O, Si,0        T0,15, 50,16
                                                                                   TO,2, S 0,17
     17    nl ,i      31.1      SO,17    ri, 1, Si,l       r1,0, Si,i



                                                                                   TQ,15, SO,30
      30    Tl,14     Si,14     50,30    T1,14, 51,14       T1,13, Sl,14
                                                                                   Ti,0, S1,15
      31    T1.15     Sl,15     S0,31    TI,15, Si,i5       Ti,14, Sl,15




     240    T15,0     515,0     Sl4,16   T1S,0, S1S,0           TI4,15, 814,16     Ti4,1, Si4,i6




     255    T15 ,15   S15, j5   S14,31   r15,15, 515,15         Ti5,14, S1s,i5     Ti5,0, S1S,15

     256                        SlS,16                          Ti5,15, Sl5 , l6   Ti5,1, Sis,i6

     257                        S1S,17                                             T15,2, S15,17




     270                        S1S,30                                             T15,15, S15,30




       Table 11.1 Pixel flow for computing the first 16 distortions using
       a 16-processor array.



 At t = 16 all three input ports are active. Port r receives the second row of
 the reference bl。 ck, port'sl receives the second row of the left half of the
 search wind。 w, and port s2 receives the first row of the right half of the search
 wind。  w. PE-0 computes acc。= acc0 + Inl,0 - si,ol and PE-1 to PE-15 compute
                                           2, ..., 15.
 acCj = accj + 1 TO,16_ j - so,iol, j = 1,

                                                                             0)
 At t = 255. PE-O processes the last pixel from the reference block and D(0,
 will be available ' to the comparator unit at the beginning of the next clock
 cyIe. Processing will continue in processors PE-1 to PE-15 and at each of the
 242                                                                      CHAPTER 11




next 15 cycles a new distortion value will be generated. Since the distortion
values are generated sequentially, the evaluation of their minimum can be
computed with a single comparator.

From Table 11.1, the first 16 distortion values will be computed in 271 clock
cycles. However, as shown in Table 11.2, processing for the next set of
distortions (D(1,0), D(1, 1), · · ·, D(1, 15)) can begin at t = 256, as soon as
D(0, 0) is computed. To compute the ith set of 16 distortion values, the


   Cycle            Input Data                          Processor Inputs
   Time        r       sl      s2           PE小             PE-1         PE-15
     256     ro,o     Si,o    S15 .16    r0,0, Si,0      r15,15, Sl5,16   r15,i, S15,16
     257     r0,1     s1,1    s1517      r0,1, s1,1      7'0,0) Si,i      r15,2, S1S,17



       270   r0,14    Si,14   S15 . 30   r0,14, S1,14    V0,13, S1,14     r15,15, S15,30
       271   T0,15    S1,15   815.31     TO,15, S1,15   1'O,14 , Si,15    r0,0, S1,15


       Table 11.2      Modified pixel flow for fully pipelined motion esti-
       mation.


reference block is scanned as before, but input from the search window starts
at the ith row, with pixel s,.0. Following this computational pipeline, all 256
distortion values will be computed in 16(16 x 16) + 15 = 4,111 cycles.

Consider now block sizes of 8 x 8 pixels. For the same search range, full-
search motion estimation requires one-fourth of the operations required for
block sizes of 16 x 16, but a frame has four times more 8 x 8 blocks than
16 x 16 blocks. Even though the computational requirements for each frame
are independent of the block size, this may not be true for the 11O, specially
in multiprocessor implementations. For example, for an 8 x 8 block and a
[-8,7] search range, the width of the search window is three times larger than
the width of the reference block. Hence, for 100 percent processor efficiency,
the architecture of Figure 11 .3 will require three (instead of two) parallel data
ports for the search window.
Hardw口refor A了Oti(刀iE釘加iation                                              243




11.3 SUB-PEL MOTION ESTIMATION
Many video applications require motion estimation with half-pel or quarter-pel
resolution. Sub-pel motion estimation can be performed in two stages. The first
stage computes a motion vector with integer pixel resolution. The second stage
refines the resolution to a sub-pel level. For example, for ha作pel resolution,
the second stage needs to perform 16 additional searches, corresponding to all
possible horizontal and vertical displacements by -1, -0.5, 0, and 0.5 pixels.
For quarter-pel resolution, 64 additional searches are required per motion
 vector. Since input data blocks have integer only pixel resolution, sub-pel
motion estimation requires additional circuitry for pixel interpolation.

Figure 11.4 shows a block diagram of a sub-pel motion estimator. Both the


                 Reference                t>       Integer
                터ock Memo마          Hd>
                                               M아ion Estimat幻n



               Search Window                   F기xel lnterp이ation
                   Men狗마
                                                   Fractional
                                          t> Motion Estimation

                                                       1
          Figure 11.4    Architecture for sub-pel motion estimation.

integer-resolution and the fractional-resolution blocks can be designed using
linear array processors, similar to the one we described in the previous section.
For pixel interpolation, Figure 11.5 shows a block diagram of a circuit that
can be used for quarter-pel interpolation. In a motion estimator, two of
these circuits should be used, one for interpolating between rows and one for
interpolating between columns.
244                                                             CHAPTER 11




                                                            x
                                   乂2
                                                            (3x+y)I4

            x
                                                            (x+y)/2
            y

                                                            (x+3y)I4
                                   y12


                Figure 11.5   Circuit for quarter-pel inte叩olation.


11.4 IMPLEMENTATION EXAMPLES
The computational power of a multiprocessor motion estimator depends on
the number of processors and the number of 11O ports. As the next three design
examples demonstrate, the architecture of Figure 11.3 can easily be modified
to support higher data rates and different coding requirements.



11.4.1 A 32-processor Array from LSI Logic

The L64720 from LSI Logic is a general-purpose motion estimation IC. It
supports either 16 x 16 blocks and a [-8,7] search range or 8 x 8 blocks and a
[-4,3] range. Multiple ICs can be used to increase either the block size or the
search range.

The core of the L64720 is a linear processor array similar to the one shown in
Figure 11.3, except that it includes 32 processors instead of 16. The L64720
has three input ports: one for the reference data and two for the search window
data. On-chip memories double buffer the input and output data to minimize
the main memory bandwidth requirements.

A motion vector is computed in 229 cycles for 8 x 8 blocks and in 2,237
cycles for 16 x 16 blocks. At 30 MHz, a single IC can process CIF frames and
16 x 16b1ocksat30fps.
                                                                            245
Hardware for九fO加n Estin瓦it幻n




11.4.2     A 2-D Processor Array from SGS-Thomson
                                                                 on is a general-
Like the IC from LSI Logic, the ST13220 from SOS-Thoms
                                                       either eight  or 16 pixels
pur山se motion estimator. The block height can be
                                                           le of four. However,
and the block width can be any number that is a multip
                                                      ns restrict the maximum
for eight-bit pixels, internal precision consideratio
                                                        range is [-8,7] pixels.
practical block size to 16 x 16. The maximum search
                                                          processing array with
The ST13220 computes distortion values using a 2-D
                                                      a single distortion. The
256 elements. Each processing element computes
                                                        o心ate in parallel. The
motion vector is computed using 16 comparators that
                                                         nce block and three for
processing array has four data ports: one for the refere
                                                             window is divided
the search window. As shown in Figure 11.6, the search
                                                               of 15 pixels. The
into six blocks. The three left-most subwindows have a width


                            0            14         22

                                 Swi          SW4

                            7
                                 SW2          SW5

                           15
                                 SW3          SW6
                            22

                                   Search Window



         Figure 11.6   Subdivision of the search window for 8 x 8 blocks.

                                                           . Motion estimation
 right-most subwindows are as wide as the reference block
                                                            (initialization), the
 is performed in two operational cycles. In the first cycle
                                                                 are performed.
 three left-most subwindows are loaded, but no computations
                                                               subwindows are
 In the second cycle (block sequence), the remaining three
                                                                  , the processor
 loaded in parallel with the reference block. During this cycle
 computes the 256 distortions and their minimum.
                                                             scan line) blocks
 In video-frame processing, two consecutive (and on the same
                                                           s, only half of the
 share half of their search window pixels. For such block
                                                             n vector. After a
 search window memory needs to be updated for each motio
 2- 6                                                                                        CHAPTER 11




 sng1e initial:zation c:.cle in the beginning of each scan line, a motion vector
 can be compu:亡d e '. 亡二 It x -V cycles, the time required to load each reference
 b:ock. The s그::1 Jpports pixel rates of up to 18 MHz.



 11.4.3      A Half-pet Motion Estimation IC from NEC

 F끝ure 11 .7 shmws a b1ock diagram of the NEC interframe prediction IC. This


              F- -e 二0nt＝忙戶 and
               AD＝三：s$ 3e＝亡i: r




                                                                          V
                               二＝
        SRA卜1                ': . ：크$5
                                                                 Memo미

                                                                                                     To DC丁

                              然泛
                                                                      V                                 >
                                                 啣帥
                                                                                                 -
                                                            Array Processor         Butler           Unit
                                                            For Second Level
                                                      m吐＞
                                                            Search.            H너Prediction卜｛>
                                                            16 PEs.

                                         伽師V帥.
                                                            『鈿a曲Units

                        i   a <= Register                     18x18 Register
                    1          1"r尸do나                           Window             Mem이y

               r.
                    =               스


        Figure 11.7           표ock diagram of a sub-pci motion-estimation IC
        irom 八 上二L尸．


IC is part of a three-chip set for MPEG-I video coding. The motion estimator
part of the IC ccmpu: s motion vector searches in a [-15,15] search window
and supports predicti '. e coding for both P-frames and B-frames. For half-pet
motion estimation. th:s design uses a two-step search strategy. The first step
is performed on a } s吐）sampied area and provides a motion vector with 2-pet
accuracy. This stage uses a 16-processor array and a 24 x 24 local register
array. Using the 18 , 18 window obtained from the first step, the second
step generates a moti0n vector with half-pci accuracy. This stage uses another
16-processor array 如d a 18 x 18 local register array. Frames for I-pictures
                                                                            247
/／口rdw口reforMoti（가lEstim口ti(刃l




                                                           sed via an on-chip
and P-pictures are stored on external SRAM, which is acces
frame controller and a local address generator.




11.5     TO PROBE FURTHER
                                                           y suited for parallel
Algorithms for full-search motion estimation are ideall
                                                          rrency  of operations.
implementations due to the regularity and the concu
                                                    ibed by Yang et a!. from
The architecture of Figure 11.3 was first descr
                                                       mapping the full-search
Bellcore [200]. Using a formal methodology for
                                                     Komarek and Pirsch [106]
motion-estimation algorithm into systolic arrays,
                                                   example, for N x N blocks
propose several 1-D and 2-D architectures. For
                                                        ssor array with N data
 and displacement area [-p. p - 1], an N x N proce
                                                           1) cycles. Low-cost
 ports can compute a motion vector in (2p)(N + 2p -
                                                   number of 11O ports. An N2
 implementations require the mininium possible
                                                               data ports and can
 systolic array by Hsieh and Lin [76] requires only two input
                                                       cycles For HDTV rates,
                                                              .
 compute a motion vector in (N + 2p小 1)2+ 2 + log2N
                                                                n IC using a 2-D
 J.H. Lee et al. [114] present the design of a motion-estimatio
                                                             (eight ports for the
 processing and register array. This IC has 16 input ports
                                                                     output ports.
 reference frame and eight ports for the search window) and eight
                                                                a vertical search
 For 8 x 8 blocks, a horizontal search range of [-32,31], and
                                                                    ting speed of
  range of [-8,7], the authors use 16 chips. The maximum opera
  each IC is 80 MHz.
                                                           [172]. A detailed
 The motion estimator from LSI Logic is described in
                                                              by Artieri et a!.
 description of the SGS-Thomson motion estimator is given
                                                                     ver, each
 [12], [35]. In [35], the 2-D array has only 128 processors; howe
                                                           the input pixel rate.
 processor computes two distortions and operates at double
 The NEC chip-set is described in [183].
                                                               can also be applied
 The principles of designing full-search motion estimators
                                                                  algorithms. For
 to the design of motion estimators that use different search
                                                             s for the three- step
 example, Jehng et al. [94] derive systolic architecture
                                                                 +7] search range,
 hierarchical search algorithm. For 16 x 16 blocks and a [-7,
                                                               es eight processors.
 each of the three stages of the hierarchical algorithm requir
                                                                12
               HARDWARE FOR ENTROPY
                             CODING




12.1 INTRODUCTION
The entropy coder is the last stage in the encoding pipeline of JPEG,
H.261, and MPEG. Unlike transform-based coding, where compression is
lossy, entropy coding is lossless. The entropy coder consists of two main
data compression/decompression units: a mn-length coder (RLC) and a
variable-length coder (VLC).

The RLC encoder compresses an input stream by representing consecutive
zeros by their run length. When a zero run is present, the RLC counts the
number of consecutive zeros until it reaches the last zero or the maximum
zero run length. The RLC decoder reverses the process by generating the
appropriate number of zeros between two nonzero data. An RLC coder can
easily be implemented using a counter, registers, and a few logic gates.

The VLC encoder maps the input source data into codewords of variable
length, concatenates them together, and segments them into 16-bit words.
Compression is achieved by assigning short codewords to input symbols of
high probability and long codewords to input symbols of low probability. The
expectation is that the average size of a codeword will be shorter than the size
of the source input. For a given source-probability distribution, a Huffman
entropy coder is optimal; that is, the average length of a codeword approaches
the theoretical minimum, the entropy of the source.
 250                                                             CHAPTER 12




 Among the standards, H.261, MPEG and the baseline implementation of
 the JPEG specify only I-Iuffman coding for the VLC coder. For improved
 compression, at a higher computational cost. JPEG also supports an arithmetic
 coder that is based on IBM's Q-Coder. Arithmetic coding may yield better
 compression ratios, but due to its complexity and the patent related issues most
 of the hardware JPEG variable-length coders are based on Huffman coding.

In Huffman coding, encoding can be done simply via lookup-tables. The
coding tables are designed based on the statistics of the input source. The
sizes and the contents of these tables are application dependent. For example,
H.261 uses five VLC tables. In baseline JPEG, only the DCT coefficients are
coded and up to four tables can be used: two for the DC coefficients (one for
luminance and one for chrominance data) and two for the AC coefficients.

Decoding is much harder, because codewords have variable length and the
receiver has no prior knowledge of the boundaries between two consecutive
codewords. Huffman coding has the property that no codeword is a prefix
of another code, thus each source symbol corresponds to a unique leaf in
a binary decoding tree. For n symbols, a Huffman tree has n - 1 nodes.
Decoding can be performed by tracing the decoding tree until a leaf of the
tree is reached. Figure 12.1 shows an example of a VLC coding table with the
corresponding decoding tree. The nodes of the tree are numbered from 0 to 6.
From Figure 12.1, given the input sequence bga, the output of the VLC coder
will be 011111000. In the decoder. given the encoded stream 110001110, the
corresponding output will be the sequence eaf.

Both the encoding and the decoding processes can be implemented using finite-
state machines that process one bit at a time. However, bit-serial architectures
may not provide adequate throughput for real-time video applications. Both
bit-serial and parallel implementations of VLC coders will be examined next.




12.2 ENCODER IMPLEMENTATION
As mentioned before, a variable-length encoder maps input data offixed length
into codewords of variable length. Consecutive codewords are concatenated
together and the output is segmented again into words of fixed length (usually
16-bits). The mapping process can be performed either through table look-
/／口r小vare和r Entropy Coding                                                 251




          a                00
                                                              1
          b                01                            G)        b
                                                              0
          C                100
          d                101                                     d

          e                110
                                             1
          f                1110                                    f
                                            （今 1
                           11110                                   g
          g     mm닉＞

                                               （亘） 1      1
          h     口卞｛    >   11111                     0             h

              Encoding Table                Decoding Tree



     Figure 12..1 Example .of a Huffman encoding table with the
     corresponciing oecouing tree.


ups or bit-serially by tracing a Huffman encoding tree. Recently, Lei and
Sun proposed a VLC enc어jer implementation that uses parallel operations to
perform the encoding, the concatenation, and the codeword segmentation in
one cycle, regardless of the length of a codeword.

Figure 12.2 shows a simplified block diagram of the Lei-Sun VLC encoder.
A set of programmable logic arrays (PLAs) stores the Huffman tables and
the length of each codeword. Instead of PLAs, one can also use ROM, RAM,
or content-addressable (CAM) memories. The reason content-addressable
memories work is related to the fact that no Huffman codeword is a prefix of
another codeword. Two 16-bit registers (the upper and lower registers) are
used to buffer the output data. The length of each codeword is accumulated
in a four-bit adder whose output controls the operation of a barrel shifter.
The barrel shifter places the output from the PLA next to the end of the
current bit stream. An OR-logic operation then cascades the codeword with
the existing bit stream. When the sum of the code lengths is larger than 15, the
 adder overflows and the carry-out bit is set to one. This indicates that a new
 16-bit output is ready. The VLC encoder outputs the contents of the upper
register, the content of the lower register is moved into the upper register, and
operations continue as before.
252                                                                                 CHAPTER 12




                                          Data Output
                                                 A

                                                                       古 Carry-out
                         Lower Reg.       Upper Reg.                Mux   <Hm
                                            주
            Data Input         Barrel Shifter
                                                               "'
                                                                                Adder
                                                           '
                                                     卜
                                         Codeword

              Uncoded        Codeword       Code-length
                Word          Table              Table
                                                                    Code-length
             AND-F키ane        OR-F기ane          OF千F기ane

                            VLC TABLES



          Figure 12.2      Block diagram of the Lei-Sun VLC encoder.


Table 12.1 shows an example of the operation of the VLC coder for the
codebook of Figure 12.1 and the input sequence g, b, a, c, b, 工 d. The output
of the barrel shifter is shown underlined. After the first input, g, the adder is


    Input           Upper                     Lower                             Sum     Carry
                   Register                  Register                                    Out
      g       1111000000000000           0000000000000000                          5      0
      b       1111   000000000           0000000000000000                          7      0
      a       1111001000000000           0000000000000000                          9      0
      c       111100100 1000000          0000000000000000                         12      0
      b       1111001001000100           0000000000000000                         14      0
      f       1111001001000111           1000000000000000                          2      l
      d       1010100000000000           0000000000000000                          5      0

            Table 12.1 Example of operation of the VLC encoder.


incremented by five, the length of the corresponding codeword output (11110).
Hardware for Entropy Coding                                                  253




Forb, the output of the VLC table, 01, is shifted by five bits and is appended to
the prior codeword. The adder is incremented by two. After the input symbol
f, the adder overflows. The carry-out bit is set to one and triggers an output
of the data stored in the upper register (11110이001000111). Note that part of
the output of the barrel shifter is stored in the lower register. After the output
of the data in the upper register, the lower register is loaded into the upper
register and the operation continues as before.




12.3 DECODER I八4PLEMENTATION
The decoding of VLC codes is far more challenging than the encoding because
there arc not predefined boundaries between codewords in the received stream.
In this section we present two classes of VLC decoders: constant-input-rate
decoders and constant-output-rate decoders. The constant-input-rate decoder
processes input bits at a fixed rate, but c에ewords are decoded at a variable
output rate. The constant-output-rate decoders have a variable input bit rate,
but they decode a fixed number of codewords per cycle.



12.3.1    Constant-Input-Rate Decoders

The simplest constant-input-rate decoder processes the input bit-serially, one
bit a time. Starting from the root, it traverses the branches of the decoding
tree until it reaches a terminal node. At a terminal" node, the codeword is
fully decoded, and the corresponding symbol can be read at the output of the
decoder. The process then restarts from the root of the tree.

This process can also be described by a model of a finite-state machine (FSM).
Each node of the tree corresponds to a state in the FSM. The output of a state is
either a decoded symbol or a pointer to another state. A single bit can indicate
whether a state is a terminal node or not. The total number of states is one
less than the number of the nodes. If the processing delay for decoding one
bit is td seconds, then the maximum throughput of such an implementation is
iL,bits/s. For a tree with n symbols, the average decoding time per codeword
will be log2rL cycles.
254                                                                          CHAPTER 12




Figure 12.3 shows a block diagram of a Huffman decoder using a ROM-based
implementation of a FSM. The throughput of this architecture depends on the



                                                            Source
                                                            Symb이

                      mmm니乙乙 ＜   뇨mHmm口m工
                                                                             b
                                                                             卜三m
                                                                     尸그쇼三O
                                            +
                                                >
                                                ROM
                                                    >
                                                        Tern이nat幻n

          Input                                            日ag

          b作' tream그B,,,


        Figure 12.3       Block diagram of a bit-serial Huffman decoder.

read cycle of the memory. Each ROM entry has two fields. The first field
is either the next state or a decoded symbol. The second, one-bit, field (or
termination flag) distinguishes between the two cases. The address of the
ROM consists of two fields: the present state and the current input bit. When
a codeword is decoded, the termination flag is 1, and it resets the input state
address to zero. As an example of such a ROM, Table 12.2 shows the ROM
entries for the decoding tree shown in Figure 12.1. In this example, a codeword
will be decoded in 10928 = 3 cycles on average.

For improved performance, the above implementation can be modified so that
the decoder traces multiple bits at a time. Figure 12.4 shows a modified version
of the decoding tree of Figure 12.1 that allows the input to be processed two
bits a time. On the average, a codeword will now be decoded in 쓰욜？흐 = 1 .5
cycles. Since the decoder processes two bits per cycle and not all codewords
have code-lengths that are a multiple of two, the model of our FSM requires an
additional output field to indicate the number of bits decoded at each cycle. For
example, Table 12.3 shows the entries for a ROM-based FSM implementation
of the Huffman tree shown in Figure 12.4. In this example, the extra field
(Next Shift) requires only one bit that indicates whether one (Next Shift = 0)
or two bits were decoded. After a codeword is decoded, the input buffer is
shifted by either one or two bits, depending on the value of this field.
Hardware for Entropy Coding                                                        255




                  Address                          Output
                Node Input                 Next-Node! Termination
                                           Codeword       Flag




                                                                      0
                                               <J 11 /b 八乙




                                                                   0
                   0




                                                             0000
                   0
                                       0
                                       l
                   1 l
                   1
                                       0
                                       l




                                                                            1l
                                                                           1l  d
                                                                              11
                                                                         11
                                 U 6
                                                e n47 r1 4




                               d <

                                                                        11
                                       0




                         V 4
                         4
                       口 八   1 <
                           1 4
                                                                     1 l
                       4
                     乙 n
                                                                  d l
                   口 八
                   J
                   八
                                                                 1
                                       l
                                       0
                                       I
                                                g 1h
                                       0
                                       I
                                                a db
                                       0
                                       l
                                                C 1d
                                       0
                     6
                     /
                                       I

     Table. 12.2 Example .of ROM entries for bit-serial Huffman
     decoding; input is one bit at a time.



12.3.2   Constant-Output-Rate Decoders

Constant-input-rate decoders are very simple; however, they don't provide a
fixed symbol decoding rate. Furthermore, when multiple bits are processed
at a time, the Huffman tree has to be reconfigured and an efficient mapping
of the decoding tree into memory is required. Lei and Sun proposed a PLA
based decoder implementation that decodes each codeword in a single cycle,
regardless of its length.

Figure 12.5 shows a block diagram of the Lei-Sun VLC decoder. Like the
VLC encoder of Figure 12.2, the decoder includes a set of the VLC tables, a
barrel shifter, two data registers, and an adder. The upper register is 16-bits;
that is, as long as the assumed maximum code-length. This guarantees that
one codeword will be decoded in each cycle. Since a codeword can be spread
into two consecutive input segments, the decoder operates on two segments
at a time, stored in the upper and lower registers. The barrel shifter operates
 256                                                                    CHAPTER 12




                                    00
                                                            a
                                    01
                                                            b
                                    10                  0
                                                            C
                              @:)                 @:)
                                                            d
                                             0
                                                            e
                                             10
                                    11

                                         0   11             g
                                                  @)        h


       Figure 12.4 .. Example of a modified Huffman tree for decoding
       IWO oirs at a rime.


                    Address                 Output
                  Node Input        Next-Node! Term.            Next
                                    Codeword   Flag             Shift
                    0        00         a        1               l
                    0        01         b        1               l
                    0        10         2        0               l
                    0        11          1       0               1
                    l        ox         e        1               0
                    1         10         f       1               1
                    1         11        3        0               1
                    2        0x         c        1               0
                    2        IX         d        1               0
                    3        0x         g        1               0
                    3        IX         h        1               0

       Table. 12.3 Example, of ROM entries for bit-serial Huffman
       uecouing; input is two oits at a rime.




like a sliding window on the contents of the two registers. The amount of
Hardware for Entropy Coding                                                     257




                                             Input

                     古
                                     1Data
                Upper Reg.




     VLC TABLES




          Figure 12.5     Block diagram of the Lei-Sun VLC decoder.


shift is controlled by the adder, which accumulates the lengths of the decoded
codewords.

At each cycle, the output of the barrel shifter is matched, in parallel, with all the
entries in the PLA. This is analogous to the operation in a content-addressable
memory. When a match is found, the PLA outputs the corresponding source
symbol and the length of the decoded codeword, and the barrel shifter is
shifted to the beginning of the next codeword. When the adder overflows, this
indicates that the upper register has been fully decoded. The content of the
lower register is transferred into the upper register, the VLC encoder loads a
new 16-bit segment into the lower register, and operations continue.

Table 12.4 shows an example of the operation of the VLC decoder for the
same codebook and encoded sequence described before. In Table 12.4, the
output of the barrel shifter is shown underlined. Starting from the top, a search
for a match of the upper register with a codeword in the codebook yields a
match with "11110," which corresponds to the source symbol g. The adder is
incremented by five, the window of the barrel shifter is shifted by five bits and
a new search yields a match with b. The procedure is repeated until the adder
258                                                             CHAPTER 12




        Upper                   Lower             Sum       Carry   Output
       Register                Register                      Out
   1111001001000111        1011101111000 111          5       0        g
   1111001001000111        1011101111000111           7       0        b
   1111001001000111        1011101111000111           9       0        a
   lllloolool000lll        1011101111000111          12       0        C
   1111001001000111        1011101111000111          14       0        b
   1111001001000111        1011101111000111           2       l        f
   10101011110001 l1       1110111110010XI1KJ         6       0        d

           Table 12.4    Example of operation of the VLC decoder.



overflows (after I). Then the content of the lower register is moved into the
upper register, and a new input is loaded into the lower register.




12.4     VARIABLE-LENGTH CODING IN JPEG
A case of special interest is the variable-length coding of the DCT coefficients
in JPEG. In baseline JPEG, entropy coding is performed in two steps: (1) the
quantized DCT coefficients are converted into pairs of symbols, and (2) these
symbols are variable-length coded.

In the first step, after the run-length coder, each AC coefficient is represented
by two syn化아s:


                        symboll    =   (run-length, size)
                        symbol2    =   (amplitude)


where size is the number of bits required to encode the amplitude of the
coefficient. Both run-length and size are four-bit numbers. The DC coefficients
are also represented by two symbols, but symboll has only size information.
In the second step, symboll is encoded using a variable-length code from a
specified Huffman table and symbol 2 is encoded with a variable length integer
(VLI). Both codes have variable length, but the VLIs are not Huffman codes
Hardware五才En什opv Co（刃ng                                                      259




and cannot be changed. For example, an AC coefficient with a run-length of
1 and amplitude -2 is represented by the pair of symbols (1,2) (-2). 'Using the
default Huffman tables, the corresponding VLC and VLI codes are (11011)
and (01). An important difference between the two codes is that the length of
the VLC is not known until it is decoded, but the length of a VU1 is specified
in the size field of the preceding VLC.

Like encoding, VLC decoding in JPEG is a two-step process. First, symboll
is decoded; the four least significant bits of the decoded symboll specify the
number of bits used to encode symbo12. If the most significant bit (MSB)
of syinbo12 is 1, then the amplitude is positive and the value of the extracted
codeword represents the actual value of a DCT coefficient. If the MSB of
symbo12 is 0, then the amplitude is negative, and its magnitude of the DCT
coefficient is given by the one's complement of the extracted codeword. For
example, if symbo12 = 101, then amplitude = 5. If symbo12 = 011, then
amplitude = -4.

Figure 12.6 shows a modified version of the Lei-Sun decoder for VLC
decoding in JPEG. The front end is the same as before, and the VLC tables
store the codewords and their corresponding run-length, scale, and code-length
information. Additional circuitry uses the output scale value to extract the
VLI code from the barrel shifter. The MSB of the VLI code is used to select
between the inverted and non-inverted VLI values. In parallel, the scale value
is added to the code-length so that the barrel-shifter is shifted to the beginning
of the next VLC code.




12.5     TO PROBE FURTHER
A key problem in the design of any variable-length coder is how to map
efficiently a coding tree into memory. In [1391, Mukherjee et al. present such
a mapping algorithm and describe its implementation in MARVLE, a single
chip VLC coder. MARVLE has a 512 x 12 RAM, a comparator, an adder, and
data and control registers. For eight-bit ascii data and at 83.3 MHz, it yields a
95.2 Mbits/s compression rate and a 60.6 Mbits/s decompression rate. This is
under the assumption of a two to one data compression ratio.
260                                                                                     CHAPTER 12




                                    1Data
                                              Input

                                                  ir＼口r寸
            Upper Reg.        Lower Reg. < 느V니V

                                                                            Carry-out
                                    V
                                              Sum
                   Barrel Shifter
                                                                   Adder
                             Codeword
                                                                   4

              VLC TABLES                                      H>       Local（沁n打이
                                                                                         MSB
                                            Adder
                                            스 6

                              C어Je-len아h                               IV
                                                                             Mux

                                                                              1
                                              Ce口1口




               V                              "   "   "   "



           run-len아h                                                    amplitude        sign



         Figure 12.6       A modified Lei-Sun VLC decoder for JPEG.


Efficient mapping techniques and architectures are also described by Park and
Prasanna [154] and Hashemian [70]. Park and Prasanna continue to use a
single-bit decoder, but their implementation requires less memory. Hashemian
applies his mapping algorithm to the design of a decoder that can process four
bits at a time. Recently, Ooi et al. [149] presented a mapping scheme and an
IC for the VLC decoding of MPEG-I streams. Their architecture processes
three bits at a time and DCT coefficients can be decoded in four cycles or less.
This IC is part of a three-chip set MPEG- i codec from NEC [183]. At 27
MHz, it can process 162 Mbits/s.

The Lei and Sun architectures are described in [117]. The same designs are
also used by Fujiwara et al. [49] in a chip-set for H.261, and by Yang
et al. [199] in a multistandard VLC decOder IC with special hardware for
JPEG VLC decoding. In [27], Chang and Messerschmitt describe parallel
Hardware for Entropy Coding                                            261




implementations of tree-based and PLA-based designs for VLC decoders.
They also propose various PLA design optimization techniques and show how
the Lei-Sun decoder can be modified to dec어je multiple codewords per cycle.
                                                                13
             IMPLEMENTATION OF JPEG
                       PROCESSORS




13.1 INTRODUCTION
Among the image compression standards, the baseline JPEG is the easiest to
implement in hardware. The first single-chip JPEG processor was introduced
by C-Cube Microsystems in 1990. JPEG processors can be found now
in a variety of image and video processing systems, such as video editing
equipment and digital cameras.

Figure 13.1 shows the block diagram of a typical JPEG implementation. The
core of the design implements the baseline JPEG using a DCT unit, the
quantizer, and the entropy coder. Up to four DCT quantization tables and
four Huffman tables can be stored in local memory. In addition to the core
processor, a JPEG IC includes memory and host interface units and local
buffers for pipelined processing and I/O. Depending on the target applications,
a JPEG processor may also include a color converter, a subsampler, and a level
shifter. The processor supports a bidirectional data and processing pipeline for
both compression and decompression.

The implementation details for DCT processors and entropy coders have
already been covered in Chapter 10 and Chapter 12. In the next two sections
we will discuss a few of the design issues for data 11O and color conversion.
We will conclude this chapter with a short description of the commercially
available JPEG processors from C-Cube Microsystems, LSI Logic, and Zoran.
264                                                                      CHAPTER 13




                       Additional features       baseline JPEG


                                                               Huffman
                            sampler          Quantizer         Codec




               b亐m弓읕
                            Level-
                            shifter
                                             0 Tables          H山fman
                                                               Tables

                            converter
                                                     Host
                                                   Interface




      Figure 13.1 Block diagram of a typical single-chip JPEG pro-
      cessor.


13.2 DATA 110 AND MEMORY INTERFACE
From Figure 13.1, a typical JPEG processor supports at least two data buses,
one for the uncompressed data "stream and one for the compressed data stream.
In many designs, an additional data/control bus may be used for interfacing
and control with a local host.

Processing is usually performed on minimum coded units (MCUs). An MCU
can be either an 8 x 8 block for grayscale images or a set of interleaved 8
 x 8 blocks for color images. For example, for 4:2:0 YCbCr data, an MCU
consists of two blocks of Y, one block of Cb, and one block of Cr. An MCU
can contain up to ten 8 x 8 blocks made up from up to four components. For
compression, the input buffer needs to store at least one MCU. For improved
performance, most designs use double (or ping-pong) buffering. This allows
one buffer to be loaded with new data while the data in the other buffer is
processed by the JPEG unit. Since the output of the Huffman encoder has a
variable rate, an output buffer is also needed to smooth the compressed data
flow. The size of the output buffer depends on the worst-case compression
ratio and the response time of the external memory.
Implementation of JPEG Processors                                           265




In most applications pixels are stored in a raster-scan format, however, JPEG
processes the data in 8 x 8 blocks. The raster to block conversion can be
performed either by the host processor, an external dedicated unit or by the
on-chip memory interface unit, using a special address generator. During
decompression, the data has to be reformatted again from 8 x 8 blocks into a
raster-scan format.




13.3     COLOR CONVERSION
The JPEG standard makes no assumptions about the color representation of
the input data. Color planes are treated as independent components and each
component is processed separately. Video sequences are usually stored in
YCbCr format, but color still-images are usually scanned and stored in RGB
format. Since the human visual system is more sensitive to the luminance
rather than the chrominance component of an image, better compression is
achieved if the image is first translated to a different color space, like YCbCr.
Color translation requires the multiplication of the original data with a 3 x 3
color transformation matrix. For example, given three RGB values R, G, and
B, the RGB to YCbCr conversion is given by

              I ' 1   I 0.299          0.587  0.114 1 f R ]
              1Gb 1 = 1 -0.169        -0.331  0.500 1 1 G 1 .             (13.1)
              L Cr J  L 0.500         -0.419 -0.081 j L B J



Using a parallel multiply-accumulate unit, color transformation can be corn-
pleted in nine cycles per pixel. Figure 13.2 shows an alternative implementation
using a barrel shifter and four adders. All operations in (13.1) are executed
using shifts and additions. For example, 0.299 can be approximated by the
sum 2-2 + 25 + 2寸 + 2_8. Hence, 0.299R can be approximated by the sum
R(2)+ R(5)+ R(6)+ R(8), where R(n) denotes a right shift of R by n bits.
Following the same procedure, Y can be obtained from

                     Y   = R(2) +R(5) +R(6) +R(8) +
                           G(1) + G(4) + G(6) + G(7) +                    (13.2)
                             B(4) + B(5) + B(6) + B(8).
 266                                                                                                            CHAPTER 13




                                                  latch
                           [>
                                \\


                                     +                                            latch

                  느m尸느二m
                                         11니＞


                                                                 H八＼
                                                                                   H1


                                                             吐＞
          Input            cL
                                                                 \\


                                                          +                                                 latch

                  Hm느mm
                                                         入             +
                                                        +
                                                                           Hd>
                                                                 /                      l七，
                                                             -
                                                                                              \\
                                                                 ---



                                                >                      +
                                         -
                                                                                  垣뜨h              +   H   吐＞   1H>
                                                                                              /                       Output


                                                latch
                                                0           r>
                                                        +        mux         H>




         Figure 13.2       Block diagram of an adder-based color converter.


Data are loaded from the barrel shifter four at a time. [R(2), R(5), R(6), R(8)J in
the first cycle, [G(1),G(4) ,G(6).G(T)] in the second cycle, etc. A Y value will
be available after three cycles. Using pipelining, a color transformation can
also be completed in nine cycles per pixel. The same circuitry can also be used
for the reverse color transformation: that is, from YCbCr to RGB. For the same
performance, the above implementation requires less hardware than a parallel
multiplier-accumulator, but more complex control. Furthermore, a change in
the color transformation matrix will require changes in the microcode that
controls the barrel shifter.




13.4      COMMERCIALLY AVAILABLE JPEG
          PROCESSORS

13.4.1    ICs from C-Cube Microsystems

C-Cube offers two JPEG processors: the CL550 and the CL560. The CL550
is designed for PC multimedia and still-image based systems. It runs at 30 or
Implementation of JPEG Processors                                         267




35 MHz and can sustain a 2 Mbyte/s compressed data rate. CIF images can
be compressed or decompressed in real time (30 fields/s). The chip has an
on-chip raster to block converter and can also perform color conversion with
a user defined 3 x 3 transformation matrix. It supports eight-bit grayscale,
RGB, YUV, or CMYK and 4:4:4:4 input and output.

The CL560 is a superset of the CL550 and is designed for video applications.
It has an improved Huffman coder that allows codewords to be encoded and
decoded in a single cycle regardless of their length. The CL560 can sustain
a 60 Mbytes/s compressed data rate and can compress and decompress CCIR
601 frames in real time. It has a improved inter끄pt control and can support an
external DMA processor.



13.4.2 ICs from LSI Logic

LSI Logic offers two JPEG processors: the L64745 and the L64702. The low-
cost L64745 requires an external DCT processor, the L64735, and an external
color and raster to block converter, the L64765. The L64745 can perform both
lossy and lossless compression and decompression. At a clock rate of 20 to 30
MHz it can process data at full-motion video rates (27 Mbytes/s). It contains
two AC and two DC code tables and four quantization tables, and it can be
used to generate event statistics for the creation of custom Huffman tables.

The L64702 is a single-chip JPEG processor and very similar to the CL560.
Like the CL560, it can perform format conversion (that is, raster to block)
and color conversion. Subsampling may also be user programmable. During
compression, the processor buffers image data in one of two MCU buffers that
operate in ping-pong fashion. Each buffer is 256 bytes deep. The output buffer
is 32 x 16 bits. The processor provides direct support for VRAM and DRAM
and an asynchronous system interface that gives it the capability to operate
either as a slave device to an external host or as a peripheral device with an
external DMA.

At 33 MHz, the L64702 can process up to 8.25 Mpixels/s for component
sequential (CMYK) or 4.125 Mpixels/s for 2:1:1 RGB and 2.75 Mpixels/s for
1:1:1 RGB. For designs based on the L64702, LSI Logic provides the CW702
core in the CoreWare cell library. This is a reduced version of the L64702.
268                                                            CHAPTER 13




Designers can use the core with other libraries to design JPEG related ICs,
customized for a particular application.



13.4.3   ICs from Zoran

Zoran offers two JPEG processors: the ZR36040 and the ZR36050. The
ZR36040 is a DCT based coder/decoder and requires an external DCT
processor (the ZR36020) and an external controller (the ZR36045). It fully
supports JPEG markers and can process CCIR 601 frames in real time. Data
processing rates can range from 15 to 21 Mbytes/s.

The ZR36050 is a superset of the ZR36040 and is a single-chip JPEG encoder
and decoder. It is one of the few processors that supports lossless JPEG using
one dimensional differential prediction followed by variable-length encoding.
It supports data rates of 21 to 27 Mpixels/s and like the LSI IC it has a
slave/ 가dA bus interface. Unlike the ICs from C-Cube and LSI Logic, the
Zoran processors requires an external raster to block converter and an external
color converter. However, they are the only JPEG processors that allow for
bit-rate control and fast preview (thumbnail images).

Bit-rate control is very useful for systems that due to constraints in memory
sizes require predictable file sizes (i.e., a digital camera). Bit-rate control
may also be required in networking applications where the time allocated
to transmit a compressed image is fixed. Under bit-rate control, the Zoran
ICs perform two computational passes. In the first pass, they collect image
statistics and update the quantization tables. In the second pass, the image is
compressed based on the size constraints and the statistics that were collected
from the first pass.

The Zoran ICs also allow for fast image preview. By decoding only the DC
coefficient in each block, they can generate a thumbnail image, 責 the size of
the original. Generation of thumbnail images can be up to 25 times faster than
full image decompression. This feature can be very useful when previewing
files in an image data base.

Table 13.1 summarizes the key features of the commercially available single-
chip JPEG processors.
Imple刃ientation of JPEG Processors                                           269




    Processor     （그ock     Bit Rate               Key Features
                  (MHz)     小'Ibytes/s)
    CL550          33-35       10.00      CIF at 30 fps, 2 Mbytes/s
                                          sustained output compressed
                                          rate, raster to block and color
                                          conversion.
    CL560            33        16.50      CCIR 601 at 30 fps.
                                          66 Mbytes/s sustained output
                                          compressed rate, raster
                                          to block and color conversion.
    L64702           33         8.25      SIF at 30 fps, raster to block
                                          and color conversion.
     ZR36050       21-27       21-27      CCIR 601 at 30 fps, bit rate
                                          control, lossy and lossless
                                          JPEG, fast preview.

       Table 13.1 Key features of commercially available single-chip
       JPEG processors.



13.5     TO PROBE FURTHER
Ogawa et al. [145] provide an excellent report on the implementation of a
single-chip JPEG processor from Sanyo Electric. The authors provide many
details on JPEG marker code processing, the host interface, color conversion
(their design was described in detail in section 3 of this chapter), and core JPEG
processing. In the Sanyo processor, the DCT is computed using row-column
transformations and two 14-bit parallel multipliers.

Another single-chip JPEG codec is described by Chen et al. [311. In
this implementation, the DCT is computed using distributed arithmetic and
quantization is performed using a parallel multiplier and lookup-tables. A
similar implementation for the DCT and the quantizer is also described by
Bolton et al. [22] for a JPEG processor from SGS-Thomson.

For the commercially available processors, most of the information in this
chapter was taken from their corresponding data books. For the CL550,
additional implementation details are described in [161] and a full description
270                                                           CHAPTER 13




is given in [15]. The JPEG chip-set from LSI Logic is also described in [13].
The Zoran bit-rate control algorithm is presented in [170]. Another JPEG
chip-set with bit-rate control capabilities was also developed by Nakagawa et
al. [143]from Toshiba Corporation. The four-chip set(an encoder, a decoder,
a memory controller, and a card controller) was developed for a digital camera.
Like the Zoran processor, the authors use a two-pass approach to determine
the scaling factors for the quantization tables.
                                                               14
                       INTEGRATED CIRCUITS
                          FOR VIDEO CODERS




14.1 INTRODUCTION
Due the computational requirements of the video standards (H.261 and MPEG),
early hardware implementations were multichip designs, where each major
component such as the DCT processor and the variable-length coder was a
separate chip. For example, in 1992, NEC introduced a three-chip set for
MPEG-I video encoding and dec以ing. The three ICs were an interframe coder
(required only for video encoding), a transform and quantization processor,
and a variable-length coder. Operating at 27 MHz, the chip set could process
SIF resolution frames at 30 frames/s.

In recent years, advances in circuit integration allow single-chip implemen-
tations of video coders. Recent hardware implementations of the video
compression standards fall into two main design categories: video signal pro-
cessors or dedicated coders. Video signal processor designs are programmable
processors with a DSP or RISC core and coprocessing units for compute
intensive operations, such as motion estimation. Dedicated coder implemen-
 tations are video encoders or decoders that are hardwired for the data flow of
a specific standard.

Programmable processors offer the highest flexibility in code design and
implementation; however, for equivalent levels of performance, they require
larger silicon area and dissipate more power than dedicated processors.
Programmable processors also incur significant costs in software developments
tools and system integration. In the remainder of this chapter we examine in
272                                                             CHAPTER 14




some detail various programmable and nonprogrammable video coders, and
we present the key features of some of the commercially available processors.




14.2     VIDEO SIGNAL PROCESSORS
Programmable video signal processors are extensions of general-purpose
digital signal processors (DSPs). They include either a RISC or DSP core
for general purpose processing and control and dedicated coprocessing units
for the efficient implementation of the DCT, motion estimation, and variable-
length coding. The implementation of the DCT, motion estimation, and
entropy coding has already been covered in Chapters 10 to 12. In this section,
we present a system-level design of various video codecs, along with their key
design and performance characteristics.



14.2.1 VSP3

The design of the third-generation video signal processor (VSP3) from NEC
is typical of video codecs with an enhanced DSP core. Figure 14.1 shows a
block diagram of the VSP3 processor. This is a 300-MHz, 1500 MOPS, 16-bit
processor for H.26 1 video teleconferencing. It includes two subprocessors: the
pipelined arithmetic unit (PAU) and the pipelined convolver unit (PCU). The
PAU includes an accumulator, an ALU, and a mmn-max value-detector unit.
The PCU includes a register file (REG. F), a convolver (CONy), an adder, and
a limiter (LMT). The convolver is a parallel 16 x 16-bit multiply-accumulate
unit. Internally, it uses redundant binary arithmetic (that is, it uses the digit
set [-1, 0, 1]) to reduce the delay in the critical path to only 25 gates. (A
conventional binary multiply-accumulate unit would have a critical path delay
of 60 gates.) For improved performance, both the PAU and the PCU use
variable pipelining (six-stage and seven-stage respectively).

Operations for the H.261 standard are divided between these two units
as follows. The PCU performs data conversions, the DCT and IDCT,
loop filtering, and quantization. The PAU performs inte汗rame processing
(differences and additions) and motion vector estimation for which it uses the
mmn-max unit. VSP3 has four single-port data memories (RAM-A, RAM-B,
R사-F, and FIFO) and three dual-port data memories (RAM-C, RAM-D,
integrated Circuits for Video Coders                                                                                273




                        DATAIN               DATAIN




                                                                                                             L 그묘
       C-BUS


                                                                                                            八Y
                                                                        20七i


                                                                                                            ＝
                    6

                    DO <                  DO <                   DO <
                           RAM-A                 RAM-B                  RAM-E          日A卜小F

                                                                                 Vq
                                             4 16-bit DATA BUSES                                1
                                                                  古             古
                                                                                                    0
                                                                                                        1
                                                                                        그O <
          DO <
                                                                                               RAF小［)
                 RAM＜二                            ALU
                                   百1
                               ACC                               CONV           ADD


                                         寸
                                        MIN-MAX                  REG. F         L卜月丁
                             PAU
                                                                          PCU
                                                         F Fr>


                                                         U
                                                             DATA OUT



       Figure 14.1 Block d孕gram of the VSP3 processor from NEC.


and RAM-E), for a total of 114 Kbits of data SRAM and 32 Kbits for
inst끄ction RAM. Each memory has its own address-generation unit (AGU).
The processor also has a sequence-control unit, a host interface unit with
20-bit 11O ports, and a timing control unit that generates internal clocks at two
to 16 times the external clock frequency. VSP3 has two 20-bit address output
ports, two 16-bit input data ports, and one 16-bit output data port. VSP3 was
 fabricated in 0.5 尸m BiCMOS and has approximately 1.2 million transistors.



 14.2.2          VDSP2

 VDSP2 is a second-generation video signal processor from Matsushita Electric.
 Figure 14.2 shows a block diagram of the VDSP2 processor. VDSP2 was
 designed for MPEG-i and MPEG-2 (Main profile at Main level) encoding
 and decoding applications. From a programmer's point of view, processing of
 data is performed on pipelined macroblocks (16 x 16). Inside the processor,
 274                                                                         CHAPTER 14




          Macro-Block Input                  DRAM                Video Out




                   3二'
                                              DRAM - I/O Controller




                          SBM         RBM    VPU0
                          小小
            응 흐          'I小I小小I
            운 읕
            띰 (3          I 1 I
                         ALU
                         小小＝
                                  MPY       ADD
                                                    VPU1       VPU2   VPU3


                           m小
                          DBM WBM CBM


                          寸                                수
                                VLC                 DCT/IDCT          Bus
                                                                      I/F
                                立 주




       Figure 14.2        Block diagram of Matsushita's VDSP2 processor.


processing is done using a SIMD configuration at the block (8 x 8) level. From
Figure 14.2, the SIMD array has four DSP processors (VPUO-3), controlled by
a DSP-core controller. The DSP-core controller includes instruction and data
RAM, a register file, an ALU, a barrel shifter, and a 16 x 16-bit multiplier.
Each of the VPU processors has an enhanced ALU, a 24-bit adder, a 16 x
16-bit multiplier, and five memories (SBM, RBM, DBM, WBM, and CBM)
comprising close to 23 Kbits of RAM per VPU processor. In addition to the
SIMD array, VDSP2 has special circuitry for DCTIIDCT and variable-length
coding/decoding. The DCT/IDCT unit is designed using distributed arithmetic.


For MPEG-2 encoding, one needs two VDSP2 ICs and an external motion
estimator. MPEG-2 decoding requires only one VDSP2. The VDSP2 was
Integrated Circuits for Video Coders                                                 275




fabricated using 0.5 /Jm CMOS. It has approximately 2.5 million transistors
and runs at 100 MHz. It supports a maximum bit-rate of 497 Mbits/s.



14.2.3       VideoRISC

The VideoRISC processor (VRP or CL4000) is a 32-bit RISC-based processor
from C-Cube Microsystems and is used in a variety of video encoding and
decoding products. Figure 14.3 shows a block diagram of the VideoRISC
processor. The heart of the processor is a 32-bit RISC processor with 4 Kbytes




                               나         F키SC Core



                                                                             V
                                Instruction              Data              M아ion
              VLC
                                     Cache               Cache         Estim카or



         口


                                                                             Local
                        Video I/O             Host I/O           DMA I/O    <H>

                                                                             DRAM
                        A
             Video In           V,
                                     ．由的.,       加：
                                                         卽，



      Figure 14.3 Block diagram of C-Cube's VideoRISC processor.

 of inst끄ction cache and 4 Kbytes of data cache. The videoRlSC processor also
 has a variable-length coder and decoder (VLC) and a motion estimator. There
 is no special DCT processor; however, special instructions in the RISC core
 allow eff也帥timp妃m帥ation of the DCT and 야her vic妃o-r이ated 아肥rations.

 The mot卜n estimation unit has 16 subprocessors in a 4 x 4 array, and the
 specific motion estimation algorithm is programmable by the user. The chip
 has also video and host interfaces, 2 Mbytes of local DRAM, and a seven-
 channel DMA controller. For MPEG-I SW quality video, two processors are
 276                                                           CHAPTER 14




 required. For MPEG-2 (in the Main profile at the Main level), eight(NTSC)
 to 10 (PAL) processors are required. In multiprocessing applications, each
 video frame is divided into horizontal stripes, and each stripe is processed in
 a different processor. C-Cube provides a software development environment
 and multiprocessor boards to assist developers in testing and development of
 video processing systems.

The VideoRISC processor runs at 60 MHz and has 1.2 million transistors. C-
Cube recently announced a newer version of the VRP,the VRP2 or CL4100. It
has the same architecture but improved circuitry for variable-length encoding
and decoding of MPEG-2 data streams. A single CL4100 can perform MPEG-
1 encoding or decoding with downloadable code. For real-time MPEG-2
encoding, C-Cube offers the CLM47xx family of products. These are parallel
designs with eight to 13 C-Cube VRP2 processors.



14.2.4 VCP

Figure 14.4 shows a block diagram of the VCP processor from Integrated
Information Technology(lIT). Like the C-Cube processor, the VCP processor




        Figure 14.4   Block diagram of the VCP processor from lIT.

has a RISC-like core (32 bits) and is fully user programmable. The processor
has two main buses: (I) the SRAM bus, which handles instructions and data
Integrated Circuits for Video Coders                                      277




for the RISC processor, and (2) the DRAM bus, which handles uncompressed
data or intermediate data. The two buses typically communicate via the
Huffman coding-decoding unit; however, a special bus-interface unit allows
direct communication too.

Data traffic is controlled by two DMA controllers under the supervision of
the RISC core. The SRAM DMA is a ten-channel DMA controller, and the
DRAM DMA is a five-channel DMA controller. The VCP has separate audio,
host, DRAM, and video input and output buses with dedicated bus controllers.
Audio is processed externally (via a separate DSP); however, the audio bus
allows the mixing (or separation) of video and audio streams.

The VCP is a superset of an earlier chip set from lIT: the Vision processor
(VP) and the Vision controller (VC). The VCP has no instruction cache, but
it has a full 32-bit interface to external SRAM and on-chip boot ROM. The
H.261 and H.221 assist units allow for frame alignment and bit handling in
video conferencing applications. The core math processing of the VCP is
performed in the VP+ processing unit.

The VP+ has functionality similar to that of the earlier VP processor. Figure
14.5 shows a block diagram of the VP processing core. Even though the VCP
has no special circuitry for the DCT and motion estimation, the VP+ core
(Figure 14.5) includes enough processing power to efficiently handle both of
these operations. An array of 16 eight-bit ALUs (which can also be configured
as eight 16-bit ALUs) together with the tree adder can be used for motion
estimation. Direct access to two memories allows one of them to be used for
the reference block and one for the se게rch window.

The VP+ core also includes an array of four parallel 16 x 16-bit multipliers
(MAC array), a register file, and a transposition unit. As we have seen in
Chapter 10, the MAC array in combination with the transposition unit is ideally
suited for computing the DCT. The VP+ can be programmed to do a variety
of operations, including filtering, color conversion, and frame scaling.

 The VCP runs at either 66 MHz or 80 MHz. A single 66-MHz VCP can
 perform MPEG-i video encoding (SIF at 30 fps), or implement an H.261
 codec (CIF/QCIF at 30 fps). An 80-MHz VCP can perform real-time MPEG-2
 decoding (CCIR 601 at 60 fields/s).
 278                                                                                      CHAPTER 14




                    Memory-A i:              Memory-B

                    Sh咐er    <H
                                                        >           168寸朮
                                                                   ALU Array


                                                                    Tree
               Re寸ster 日！e                                          Adder



                                   mm8mCm二
               64 x 64-bit
                                             =CD        /t                            \
                                                             ＞a>    >a>   ＞口＞   ＞口＞
                                                             小
                                                                          H
                                                                    H
                                                                                H
                                                                   Accum너a幻r
                                                                                    I
                                                         MAC Array



       Figure 14.5      Block diagram of the core processor in the VP IC
       rrom ii I.


14.2.5     The VideoFlow Chip set

The VideoFlow chip set from Array Microsystems is the only data-driven
architecture. Unlike traditional processors, which are controlled based on
the instructions fetched by a program counter, in the VideoFlow architec-
ture program instructions are executed based on a processing data-flow and
operand availability. The chip set has two processors; the image compression
coprocessor (ICC) and the motion estimation coprocessor (MEC). The chip
set requires an external (user-defined) control processor for Huffman encod-
ing/decodirig and bit-stream management. Array Microsystems provides a
graphical user interface for its data-flow programming tools. This allows ease
of programming without a need to interact with the internal architecture.

Figure 14.6 shows a block diagram of the ICC processor. The core of the ICC (or
a77 100) is the data-flow control unit. This unit passes control and data tokens
to the other subprocessors, which operate in parallel. Special function units are
used for arithmetic operations, run-length coding, DCTIIDCT, quantization,
and memory interfacing. All instructions are vector-type. Communication
among units is done via control and data tokens. A data token has a header
Integrated Circuits for Video Coders                                                               279




                                    DATA FLOW CONTR아．UN仟

                                     Scalar 나＞ Instruction
                                    F가ocessor
                                      Unit    <H Memory                       Host
                                                                                            Host
  乂Bus                                                                      Interface       {>
                                        寸 수
                  쌥                     Token
                                        Memory    :        Con打이
                                                                              Unit          Bus



                                          6
                          Global Bus




                Video
                               合
                              Token                           OCT &
                                                                             숲
  V-Bus                                       Run-length                  Aflthn比tic
    <     >   Interface     Interface                       C卜U目씨zation
                                                Unit                      P口Om$＄아
                Unit          Unit                            Un心


                 令             合，   畸鈿
                                                                                        /




     Figure 14.6 Block diagram of.the VideoFlow image compression
     processor rrom i\rray lvllcrosystems.


and can include up to four 8 x 8 data blocks. The architecture supports
user-defined instructions for external assist units (like the MEC IC) and can
be customized by adding or removing subprocessor units.

From Figure 14.6, the ICC has three external data buses. In a typical system,
it uses the V-bus to connect to either DRAM or VRAM. the X-bus to connect
to the motion estimation chip, and the host bus to communicate with the host
processor and additional memory.

The MEC companion IC (a77300) has a 12-bit CPU with its own register
file (32 x 12-bit) and barrel shifter. In addition, it includes token and video
buffers. The MEC allows two levels of hierarchical motion estimation for pel
and quarter-pel precision.

Both ICs run at 50 MHz. For H.261, the videflow chip set allows in real time
one CIF encode and two CIF decodes or one QCIF encode and seven QCIF
decodes. For MPEG, it can perform one SIF encode or one CCIR 601 decode
or two SIF decodes. The ICC executes 1 GOPS with 1.8 million transistors.
The MEC uses I million transistors for 7 GOPS.
 280                                                                           CHAPTER 14




 14.2.6    The Multimedia Video Processor

The Multimedia Video Processor (MVP) or TMS320C80 is the latest entry
from Texas Inst끄ments in the DSP market. Unlike other video processors,
the MVP was not designed specifically for the implementation of the video
standards. For example, it does not have any special function units for the
DCT, motion estimation, or Huffman coding. It is a single-chip parallel
processor that can be used in a variety of applications in graphics, signal, and
video processing.

Fig 14.7 shows a block diagram of the MVP. It includes a master processor



                                                f키SC




                                                                                   완二죠mO三m죠쓰O
                                                Core
                                                   h肝：)
                                               D            Video
                                               A      Z;   Contr이



                   GLOBAL CROSSBAR



                                                                     뇨mH죤는OO
                                                           느m卜mC띤H
            I .       L       i         r      V V
           D-RAM    D-RAM   口RA！너     口RAM      MP's
            and      and     and       and       Datal
          卜Cache   卜Cache   卜Cache   I-Cache   I-Cache




       Figure 14.7   Block diagram of the MVP from Texas Instruments.

(MP) with a 100-MFLOP IEEE floating-point unit, four parallel digital signal
processors (DSPI -DSP4), a transfer controller for data transfers and memory
control, local memory, and two video controllers for data capture and display.
MP is a general-purpose RISC processor with an internal floating-point unit.
It uses a 32-bit instruction word and can load or store eight-bit to 64-bit data
sizes. It has a 4 Kbyte instruction cache and a 4 Kbyte data cache. The MP
can be used for control, floating-point operations, audio processing, or 3D
graphics transformations.
Integrated Circuits for Video Coders                                       281




Each DSP unit performs all the typical operations of a general-purpose DSP
and can also perform bit-field and multiple-pixel manipulations. Internally,
it has a splittable (one 16 x 16 or two 8 x 8) multiplier and ALU, 44 local
registers, a barrel shifter, two address generators, and a program-flow control
unit, all controlled by very long 64-bit inst吼tion words. Each DSP has three
parallel data ports for local data, global data, and instructions (L, G, and I).
 A global crossbar switch allows data transfers among the DSP processors and
the RISC core. All processors share 50 Kbytes of SR사d that is divided into
data RAM and instruction caches.

The transfer controller manages the hardware interface between the 0n-
chip and the off-chip memories. The two frame-buffer controllers support
programmable video timing to control both display and capture.

At 50 MHz, the MVP executes more than 2 GOPS. It is fabricated in 0.5
pm CMOS and includes more than 4 million transistors. A single MVP can
perform real-time MPEG-I encoding or decoding (SW resolution). Since the
MYP has an architecture very similar to that of the VDSP2 and no special
hardware for motion estimation, we estimate that multiple MVPs are needed
for real-time MPEG-2 encoding.

In summary, programmable video processors now allow real-time H.261 or
MPEG encoding. However, for MPEG-2 encoding no single-chip solutions are
presently available. Programmable processors integrate more than 1.2 million
transistors and can execute 1-2.5 billion operations per second. (In comparison,
a general purpose 64-bit RISC processor has more than 3 million transistors.)
Table 14.1 shows the key features of the programmable video processors we
described in this section. Except for the VSP3 and the VDSP2, all other
 processors are commercially available. All processors can be programmed to
 implement any of the image and video compression standards. The column on
 key features describes only real-time performance. In column four, MPEG-i
 and MPEG-2 refer to processing of 30 fps video at SIF or CCIR 601 resolution,
 respectively.
 282                                                                     CHAPTER 14




          Processor       （그ock     GOPS                     Key Features
                          (MH기
         VSP3              300            1.
                                                   5   H.261 coder.
         VDSP2             100                         入'IPEG그 coder. Encoder
                                                       requires two ICs and ex-
                                                       ternal motion estimator.
         VideoRISC          60        2.5              Two ICs for MPEG-i
                                                       and 8-10 ICs 向r 入WEG그
                                                       encoding.
         VideoRISC-2                                   MPEG- i coder.
        vCP                 80                         入4PEG- I coder or 入IPEG-
                                                       2 decoder.
        VideoFlow           50        1
                                               .
                                                   0   MPEG- I encoder requires
                                                       external motion estima-
                                                       tor and Huffman coder.
                                                       MPEG-2 decoder.
        MVP                 50       2.0               入4PEG- 1 coder, 八WEG그
                                                       decoder.

       Table 14.1 Key features of programmable video signal proces-
       sors.



14.3 DEDICATED CODERS
Dedicated coders provide limited, if any, programmability and have a dedicated
 architecture or control logic for a specific video encoding or decoding standard.
 There is an expectation that applications using video compression (such as set-
 top boxes for interactive TV, high-definition TV, digital cameras and VCRs,
and desk-top video teleconferencing) will see a huge growth in the next few
years. As a consequence, there is a proliferation of announcements of products
and partnerships related to video compression and decompression. Table
14.2 shows a representative list of commercially available video processing
ICs and their key features. In addition to these processors, related product
announcements have been made by Texas Instruments, Zoran, and others.
For example, CompCore Multimedia has announced that it is developing an
MPEG-1/2 megacell core that IC developers can integrate into video related
力毗gr口ted Circu加 for Vide八뇨lers                                           283




products. Japanese companies like Toshiba and NEC are also developing new
generations of video coders.


      Company           Part No.          Key Features
     AT&T              AV4310    H.261, MPEG-i (no B frames)
                                 encoder (CIF 30 fps).
                       AV4220A   H.261 decoder.
                       AV4i20A   Controller.
                       AV6101    MPEG-2 decoder (no B frames),
                                 30 Mbits/s.
                       AV6I 10   入4PEG그 decoder, 50 入4bits/s.
     C-Cube            CL450     MPEG-i    decoder (SIF).
                       CL480VCD MPEG-I audio and
                                 video decoder.
                       CL9100    MPEG-2 decoder.
     IBM               IBM39-    MPEG그 decoder (（巧 入4bits/s).
                       코vIPEGSI끄
     LSI Logic         L64112    MPEG-I decoder.
                       L64000    入1PEG그 decoder,
                                 set-top box support.
                       L64002    入4PEG그    video and aud幻
                                 decoder.
     SGS-Thomson       STi3400   H.261,  MPEG-i decoder.
                        STi3500  MPEG-2 decoder.

      Table 14.2 Key features of commercially available dedicated
      viueo processors.



From Table 14.2, with the exception of the AV43l0 H.261 encoder from
AT&T, all other ICs are video decoders. This is not surprising, since real-time
video decoders are easier to implement (they don't require motion estimation)
and will he in higher demand than real-time video encoders. Figure 14.8 shows
a block diagram of a typical video decoder. In addition to the MPEG/H.261
decompression core, it also includes a memory controller for glueless interface
to external data RAM, input and output buffers (FIFOs), input and output
buses, and a display controller. The display controller performs operations
like color conversion (YCbCr to RGB), vertical and horizontal filtering, and
 284                                                                                          CHAPTER 14




                                  Header          Huff man             Inverse
                             1>              H>              m   {>
                                  Decoding        Decoding            Quantizat幻n
                                                                                        ＜니＞


                                    M이ion
                                                                          寸              Host Bus

                                                                       Inverse
                                  Compens카ion                           DCT

                                             수
                             H
       Video         Input                                                                ［긔splay
                                    Memo싸 and Display                    Output
                                                                                    Hm{   >
                                        Contr에er
         1吐＞
       Input         F下O                                                  디FO
                ＼뇨
                                                                                    /


                                  P-Frames        Reconstructed
                                  B-Frames           다an犯




               Figure 14.8        Block diagram of a typical video decoder IC.


frame rate conversion (NTSC, PAL, and film). Note that until recently,
audio decompression required a separate processor. However, the CL480VCD
from C-Cube and the L64002 from LSI Logic integrate both video and audio
decoding in a single IC.

Among the processors listed in Table 14.2, the design of the video encoder
from AT&T is of particular interest. The AVP Video Codec chip set
from AT&T was designed for the implementation of low-cost audiovisual
teleconferencing systems that comply with the ITU-T H.320 (Px64) standard.
The three ICs are the AV43 10 video encoder, the AV4220 video decoder,
and the AV4120A video controller. Both the encoder and the decoder include
programmable and nonprogrammable subunits and thus can be considered
hybrids of programmable processors and dedicated processors.

Fig 14.9 shows a block diagram of the encoder. This is a 10.5 GOPS processor
with five main processing units: the memory management processor, the
quantization processor, the DCTIIDCT processor, the entropy coder (VLC),
and the motion estimator. In addition, there is a main controller and video and
host-CPU interface units.
Integrated Circuits for Video Coders                                                                   285




          舍     ""' "

        Memory             Ouantization      OCT. IDCT                         Out
      Management            Processor        다oces＄아                  VLC
                                                                              F下O
         Unit
                                                                                 1
                                                                                                DRAM
                           Buses: Sy없미nData. Address, In地rrupt                             <11小b
                                                                                      二＞
                                          Video Bus                           (：기it
      Contr이             Motion                             Host
                                          Interface   ＜미
                                                                              F下0
     마oces＄아            Estima伯r                           Bus I/F
                                           FIFOs                                2

                                                                                            1


                                  VIDEO BUS V
                                                                 卜，         ,,.:..




         Figure 14.9 Block diagram of the AT&T video encoder.


The memory management and algorithm flow control unit includes a 16-bit
processor with an ALU and three multipliers, two 128 x 16 register arrays and
DRAM interface. The three multipliers are used for color conversion with a
user programmable 3 x 3 matrix. This unit delivers data to and from the rest
of the processor and controls all DMA operations. The quantization processor
implements user-defined algorithms to determine the quantization step to be
used in the encoding process for each macroblock. This is a 16-bit processor
with an ALU, a multiplier, a 512 x 16 cache, and a 144 x 16 register array.

The DCT processor performs the DCT, quantization, zig-zag scan, inverse
quantization, and inverse DCT. This is a SIMD (single-instruction multiple-
data) array of six 16-bit processors, each with an ALU, multiplier-accumulator,
dual memories (for coefficients and data), local registers, and data cache. The
motion estimator is a dedicated array processor of 256 elements, 15 delay
lines, and a 1280 x 16 cache. For motion estimation, the full-search algorithm
with the MAE match criterion described in Chapter 4 is used. Finally, the
variable-length coder (VLC) includes a 16-bit ALU, a register array, 128 x 16
RAM, and a 1K ROM.
 286                                                           CHAPTER 14




The processor runs at 45 MHz and has 1.63 million transistors. It can encode
H.261 CIF resolution frames in real time or MPEG-I (at CIF resolution)
without any B frames. The companion decoder chip includes many of
the functional units of the encoder (e.g., the color converter, and the DCT
processor). It can support a 4 Mbits/s compressed input rate, and thus it
can decode CIF frames in real time. These two ICs are controlled by the
system controller, which also multiplexes and demultiplexes video streams
and performs error correction.




14.4 TO PROBE FURTHER
Digital video processors have evolved from simple extensions of digital
signal processors to powerful multiprocessing architectures. For example,
Enomoto and Yamashina [45] describe the evolution of the NEC video signal
processors: from the 14.5-MHz P-VSP, introduced in 1987, to the 300-MHz
VSP3, introduced in 1993 [80]. A separate MPEG chip set from NEC is
described by Tamitani et at. [183].

The VDSP processor from Matsushita [9] was among the first video pro-
cessors with an on-chip DCT unit and an extended instruction set for video
compression and decompression. The VDSP2, a second-generation processor
from Matsushita, is described in [186] and [4].

For commercially available processors, most of the information in this chapter
is based on data sheets and product catalogs. Trade magazines, like EDN,
Computer Design, and Electronic Design [24] also provide timely overviews
and performance characteristics. Descriptions of the Vision processor and
Vision controller from lIT can also be found in [14]. In [65], Guttag
et al. describe the design philosophy and implementation details for TI's
MVP processor. Performance characteristics of the MVP in a real imaging
and graphics system (the UWGSP from the University of Washington) are
presented by Kim et at. [101]. In [2], Ackland provides a general description
of the AVP chip set. Additional implementation details for the encoder and
the decoder can be found in [167] and [23]. IBM's MPEG-2 video decoder
is described in [181]. An MPEG-l audio and video decoder IC from C-Cube
and JVC is described in [53]. The chip integrates 305,000 logic transistors and
Integrated Circuits for Video Coders                                    287




485,000 memory transistors. At 40 MHz, it can decode two channels of 48
kHz audio and one SIF video stream at 30 fps.

Recently, SGS-Thomson presented a single-chip H.261 codec [69] suitable
for the implementation of video telephone terminals. The chip encodes and
decodes simultaneously 15 QCIF frames per second and can also encode and
decode still CIF images. The chip integrates 573,000 transistors in a 1.56cm2
area. A recent survey paper by Pirsch et al. [160] presents an overview of
VLSI implementations for video decoders and compares them in terms of
speed and silicon area.
                                                             15
     MULTIMEDIA ENHANCEMENTS
          FOR RISC PROCESSORS




15.1 INTRODUCTION
The JPEG and MPEG standards make it easier now to encode and exchange
images and video streams across different computing platforms and networks.
Video in particular has the potential to become just another 成ta type. Real-
time video processing on PCs and workstations is now handled with special
 video boards and custom circuits. This is similar to the way most of the
advanced graphics processing was performed in the 1980s. Special hardware
may yield the highest performance but at a considerable cost to the end user.

General-purpose RISC and CISC processors have significant computing
power but are not well suited for a software-only solution. For example,
some of their main features, such as 32-bit or 64-bit data paths and on-chip
floating-point processing, are not needed in video processing. Therefore,
there is a strong desire among computer manufacturers to enhance existing
architectures so that video processing is integrated into the next generation
general-purpose processors just as graphics processing has been integrated
into today's architectures.

Two workstation manufacturers that have introduced multimedia-enhanced
processors are Hewlett-Packard and Sun Microsystems. The specific features
of these two processors are examined next.
290                                                               CHAPTER 15




15.2 GENERIC OPERATIONS IN VIDEO
     PROCESSING
It is always tempting to enhance a general-purpose processor by adding
special function units. However, this approach violates the fundamental
design principle of a RISC architecture, which states that only the most
commonly used operations are implemented in hardware. Hence, integration
of multimedia enhancements requires first an analysis and understanding of
the generic operations in the video-processing pipeline. Table 15.1 shows the
arithmetic operations required for the main functional blocks of the image
and video compression standards. From Table 15. 1 and an analysis of the


                    Function                  Operations
              C이or transformat由n,      Z C:T,,clip()
              preprocessing, and       佃 + S力／2, (1/4) ＞二？=1 '2
              postprocesslng
              DCT, IDCT                ax + b,   >2   c1x1
              （加antization             xilci
              Dequantization           Sic2
              Huffman coding           data shifts, comparisons
              Motion estimation/       >2 江i 寸 yi1 or ＞二（xi 卞 !/2)2,
              compensation             ,nin(a,b), xi + cxj

             Table 15.1 Generic operations in video compression.


processing pipeline in video compression one can conclude the following:


      Input data and coefficients have usually eight to 16 bits of precision.

      There is no need for floating-point operations.

      The multiply-accumulate operation is very common; however, most of
      the multiplications are with constants.

      Saturation arithmetic, where a result is clipped (clipO) to the maximum
      or minimum value of a predefined range, is common in many operations
      (such as, color transformation).
Multimedia Enhancements for RISC Processors                                 291




In addition to these arithmetic operations, video processing requires efficient
data addressing and 11O. The above analysis indicates that RISC processors
need to handle more efficiently fixed-point arithmetic (specially multiplication)
and to support a more efficient utilization of their longer than necessary
data paths. The two new RISC processors from Hewlett-Packard and Sun
Microsystems attempt to do exactly that.




15.3 MULTIMEDIA ENHANCEMENTS IN THE
     HP-PA
In early 1994, Hewlett-Packard introduced the first general-purpose RISC
processor with built-in multimedia inst끄ctions. The new processor (the
PA7 100LC) and algorithmic enhancements in the decoding algorithms allowed
for the first time real-time MPEG-I video and audio decoding on a desktop
computer without using any special hardware.

The 7I00LC is a 32-bit superscalar RISC processor with two fixed-point
ALUs, a floating point unit, and a memory and 11O controller integrated into
a single chip. This is a low-cost processor with off-chip instruction and data
caches and only a small on-chip instruction buffer. Since video operations
never require more than 16 bits of precision, the key approach for multimedia
enhancements in the HP design was to allow for parallel operations at the
half-word (16-bit) level. For instance, each 32-bit integer ALU was partitioned
so that it could execute a pair of 16-bit arithmetic operations in a single
cycle with a single instruction. Arithmetic operations that were accelerated
using this strategy include add, su加ract, 口ver口ge, sh/｝七肛口m工add, and
shi尼r뇽h卜an小口dd.

Consider the standard ADD instruction:


                                ADD Ra, Rb, Rt,


 where the ALU performs a 32-bit addition on the contents of registers Ra and
 Rb and places the result into register Rt. Assume now that two 16-bit operands
 (al and a2) are stored into the left and right halves of register Ra and another
 two 16-bit operands (bl and b2) are stored in register Rb. Figure 15.1 shows an
 292                                                                              CHAPTER 15




 example of how a 32-bit adder can be used to perform either a 32-bit addition
 or two 16-bit additions. The 32-bit adder is divided into two 16-bit halves.
 When the output cany (c_out) of the lower half is blocked (c_in = 0) then two
 16-bit additions can be performed in parallel. Two 16-bit additions can be


                Ra                                    Rb
                     al                                    bi       b2




                                                                    V
                     ci == al + bi                         c2 = a2 + b2
               16-bit ALU                         C             16-bit ALU
                                                mux
                                                                             ADD or HADD
           \

           32-bit ALU
                                      At
                                           ci




               Figure 15.1            Half-word addition using a 32-bit ALU.

invoked with the new half-word-add instruction:


                                            HADD Ra, Rb, Rt,


whereifRa = [al, a2] andRb= [bl力2],thenRt = [cl, c2J = [(al+bl),(a2+b2)].

This instruction can also be invoked with a signed or unsigned saturation
option. This option clips the 16-bit results so that they do not exceed a preset
maximum and minimum value. This can be expressed as


                            r
                            J r
                              J r
                                J r
                                  J
                                      cl > max        then      cl = max,
                                      ci <mm72        then      cl = mm72,
                            1
                            2 1
                              2 口
                                2 1
                                  2
                                      c2 > mar                                             (15.1)
                                                      then      c2 = max,
                                      c2 <mm7l        then      c2 = mm71.

For signed saturation, max = 215 - 1 and mm7i = _215. For unsigned saturation,
max = 216_ i and mm7l = 0. This operation is particularly useful in pixel-related
operations and replaces 10 conventional add and shift operations. Similarly to
Multi刃wdia Enhanc日刃日玎s for／가SC Processors                                     293




the HADD instruction, there is also a half-word subtract instruction (HSUB)
that allows two pairs of 16-bit values to be subtracted in parallel.

Another new instruction is the half-word average instruction:


                               HAVE／沅, ／깊7, ／社，


where Rt = [ci, c2] = [(al + bl)/2, (a2 + b2) /2]. This instruction is particularly
useful for half-pixel interpolation, since two new pixel values can be computed
in a single cycle. Without this multimedia instruction, this operation would
require four cycles.

The PA7I00LC Cpu has no integer multiplier, hence it is very hard to support
parallel multiplication on half-words. However, in video coding most of the
multiplications involve small constants, and thus they can be performed by
simple combinations of shifts and adds. The original PA-RISC architecture
already had shift-left-and-add operations. These operations perform a left
shift of one operand by 1, 2, or 3 bits before adding the other operand. To
implement this operation on half-words required a simple blocking of the shifts
and the carries between two halves of the integer ALU. The new half-word
left-shift-and-add operation is defined as


                           HSHLADD Ra, Rb, Rt, k,


where Rt = [cl, c2] = [(al << k) + bi, (a2 << k) + b2]. The symbol "<< k'
denotes a left shift by k bits, where k is either 1, 2, or 3. A similar half-
word shift-right-and-add (HSHRADD) instruction was also added. Table 15.2
summarizes the key operations of the new PA-RISC multimedia instructions.



15.3.1    110 and Postprocessing Enhancements

In video decoding, a major percentage of the computations is spent in
postprocessing, which includes color transformations and display I/O. A new
graphics IC allowed HP to move many of these display-related operations into
the graphics controller and thus reduce the CPU load. The main processor
connects directly to the graphics controller via a high-speed system bus. With
294                                                                 CHAPTER 15




              Instruction                          Operation
      (Ra = [al,a2}, Rb = [bl,b2])                (Rt = [cl,c21)
      HADD Ra, Rb, Rt                   Rt = [(al+bl),(a2+b2)]
      HSUB Ra, Rb, Rt                   Rt = [(al-bl),(a2-b2)]
      HAVE Ra, Rb, Rt                   Rt = [(al+bl)/2,(a2+b2)/2]
      HSHLADD Ra, Rb, Rt, k             Rt = [(a! <<k)+bl,(a2 << k)+b2]
      HSHRADD Ra, Rb, Rt, k             Rt = [(al >> k)+bl,(a2 >> k)+b2]

             Table 15.2     New PA-RISC multimedia instructions.



a peak available bandwidth of 100 Mbytes/s. this direct connection allows for
fast data transfers between the processor and the display.

The new graphics IC can handle YCbCr data, perform the up-sampling of the
chrominance components Cb, Cr, and convert YCbCr data to RGB. A special
color-compression unit translates and stores 24-bit RGB pixels into eight-bit
values. Before the final display, the eight-bit values are translated back into
true-color 24-bit values. This allows real-time decompressed video to be
displayed in true-color even on entry level systems that have only eight-bit
frame buffers.




15.4 入IULT끄 'IEDIA ENHANCI呱(ENTS IN THI亡
     ULTRASPARC
In late 1994, Sun Microsystems provided the first details on the architecture
of its new 64-bit processor, the UltraSPARC. Like the HP processor, the
new Sun microprocessor will also incorporate architectural enhancements for
multimedia processing. Sun estimates that a 200-MHz UltraSPARC-based
workstation will be able to decode at least one MPEG-2 video stream in real
time.

The UltraSPARC is a 64-bit superscalar RISC processor with two integer
ALUs, an address-generation unit, and a special floating-point and graphics
unit. The processor can issue up to four instructions per cycle, but there is a limit
of only two integer operations and two floating-point or graphics operations
Multimedia Enhancements for RISC Processors                                 295




per cycle. Most of the multimedia enhancements in the UltraSPARC are in the
floating-point and graphics unit. The floating-point execution unit integrates a
floating-point adder, a floating-point multiplier, and a floating-point divider.
The graphics execution unit includes a graphics adder and a graphics multiplier.

The graphics adder consists of four 16-bit adders and a custom shifter that can
be used to perform single cycle additions, subtractions, merge, expand, and
logical operations. By controlling the carry propagation among the adders one
can compute either four 16-bit additions or two 32-bit additions in a single
cycle. This technique is identical to the one used in the HP-PA, except that in
the HP-PA the partitioning of the data path is performed in the integer ALU.
The core of the graphics multiplier is an array of four 8 x 16-bit multipliers.
They perform three-cycle partitioned multiplications, comparisons, and pixel
distance operations. For graphics applications, the four parallel multiplications
allow the Sun processor to manipulate in parallel the three color components
and the alpha value of a color pixel.

The new SPARC instructions can be classified into five categories: data-
conversion instructions, arithmetic and logical instructions, address-manipula-
tion instructions, memory-access instructions, and the motion estimation
inst끄ction. The data-conversion instructions convert between the various
data types used in the graphics unit. The arithmetic and logical instructions
allow partitioned add, subtract, multiply, and logical operations using either
single or double precision. A 16 x 16-bit multiplication requires two of these
instructions and an extra addition. The address-manipulation instructions
operate on the register files and can be used to concatenate data or extract
data fields. Memory-access instructions allow for partial or block load and
store operations. For example, a block load causes the transfer of 64 bytes
from memory to a group of eight consecutive double-precision floating-point
registers. The new block instructions allow data to be transferred from the
processor directly to the screen at peak rates of up to 600 Mbytes/s.

Of special interest is a new instruction for motion estimation. For eight-bit
data, this instruction computes eight subtractions, eight absolute values, and
eight additions in a single cycle. Thus, computing the minimum absolute error
between two 16 x 16 blocks requires only 32 such instructions, compared to
close to 1,500 conventional instructions.
296                                                             CHAPTER 15




15.5 TO PROBE FURTHER
Designers of programmable video processors were the first to analyze the
video compression pipeline for generic operations [141]. Of particular interest
are the architectural enhancements and the instruction set of the vector pipeline
digital signal processor(VDSP)from Matsushita [9]. Based on a DSP core,
the VDSP is a programmable video processor suitable for JPEG and H.261
coding applications. A special vector-pipeline controller allows the VDSP to
execute arithmetic operations on vector data with a single instruction.

RISC cores are used extensively in video codecs. In [72], Herrmann et at.
present the design of a RISC core with special architectural features for video
processing. For the same clock frequency, their new architecture can process
H.261 coded video twice as fast as a generic SPARC(CY7C601)processor.

The HP PA7100LC chip-set is described in [102] and [188]. Additional
details regarding the software-based MPEG-i decoder from Hewlett-Packard
can be found in [1161 and [19]. Sun's UltraSPARC architecture and the new
instruction set are described in [64] and [104].
                                                                 16
                     STANDA之DS FOR AUDIO
                            COMPRESSION




16.1 INTRODUCTION
Digital audio is an integral part of any video or multimedia application and may
consume a considerable portion of the overall bandwidth. Therefore, efficient
compression of the audio data is as important as the efficient compression of
the video data. There are two main parameters that control the quality and
the bit rate of digital audio: the sampling resolution (that is, bits per audio
sample) and the sampling frequency.

The sampling resolution determines the dynamic range of a signal. For
example, audio compact discs (CDs) use 16-bit samples and provide 96 dB
of dynamic range (96 = 20 1O9io216). The sampling frequency determines how
much of the frequency spect끄m of the original analog signal can be faithfully
reproduced. According to the Nyquist theorem, the sampling frequency has
to be twice as large as the maximum frequency component. For example,
CD recordings use a 44.1 kHz sampling frequency, approximately twice the
maximum frequency response of the human auditory system (22 kHz). In
digital telephony, where high audio fidelity is not as important, signals are
bandlimited to approximately 3.5 kHz and the sampling frequency is 8 kHz.
Table 16.1 shows some typical audio applications and the corresponding
sampling rates.

According to the CCIR recommendations, digital audio in broadcast studio
format requires a sampling resolution of 16 bits and a sampling frequency of
48 kHz. For stereo signals, the corresponding bit rate is 2 x 768 = 1.54 Mbits/s.
298                                                             CHAPTER 16




            Sampling Frequency'           Application
                  (kH기
                    8.00        三
                                1Digital Telephony
                   22.05          Personal Computers
                   32.00          Digital audio and TV
                   44.10          Compact Discs
                   48.00          Digital Audio Tapes, HDTV

      Table 16.1 Sampling frequencies for typical audio applications.



Similarly, the bit rate from a stereo CD is close to 1.4 Mbits/s, and a 10-minute
stereo audio clip requires close to 105 Mbytes of storage. The above data
indicate that efficient storage and transmission of digital audio require some
form of data compression. There are two main compression techniques for
high-fidelity audio: the MPEG audio standard and the AC audio compression
algorithms developed by Dolby Laboratories. Both techniques can achieve
CD-like quality at 128 kbits/s per audio channel (5.5:1 compression).

The MPEG audio compression algorithm is part of the MPEG-i standard
that addresses not only the compression of video and audio but also their
synchronization. Audio can be compressed down to 32 kbits/s for a single
channel.

The AC-3 algorithm is part of the Grand Alliance HDTV system for North
America. Interestingly enough, the Grand Alliance system uses the MPEG-2
standard for video compression. In HDTV, the sampling resolution is 18 bits
and the sampling frequency is 48 kHz. For six channels, AC-3 compresses the
original 5 Mbits/s bit stream down to 384 kbits/s (13:1 compression). An AC-3
standard is currently under development by the FCC advisory committee on
advanced television services (ATSC).

Both MPEG and AC-3 make no assumptions about the source of the input
signal, and they can be applied to both speech and high-fidelity audio.
Compression is achieved by transforming the input signal into the frequency
domain and by removing information that is perceptually irrelevant. A
different coding approach is used by the G.72x standards. These standards
have been developed by the International Telecommunications Union (ITU)
Standardsfor Audio Compression                                            299




specifically for the efficient coding of speech over band-limited telephone
channels. They can be applied in a variety of telecommunication applications,
including tele-conferencing (e.g., together with the H.261 video compression
standard) and voice-data modems. These standards achieve compression by
using predictive coding.

G 721 was the first standard for the coding of speech at 32 kbits/s on channels
with a 300 to 3400 Hz bandwidth. In 1990, G.721 was replaced by the G.726
standard, which allows for compressed data rates at 16, 24, 32, and 40 kbits/s.
Both G.721 and G.726 encode the input data using adaptive differential pulse
code modulation ( ADPCM).

For broadband telephone channels(0 to 8 kHz),ITU has developed the G.722
standard on "7 kHz audio coding with 64 kbitls." This is an enhanced version
of the G.726 standard and uses a subband filter as a front end to two separate
ADPCM coders. The input is sampled at 16 kHz, and the subband filter
separates the input stream into the two subbands of0 to 4 kHz and 4 to 8 kHz.
The higher subband is coded at 16 kbits/s, and the lower subband is coded at
48 kbits/s. The two streams are multiplexed for a total bit rate of64 kbits/s.

For lower bit rates, the G.728 standard achieves speech quality at least as
good as the G.721 but at 16 kbits/s. The improved performance is achieved
by replacing the ADPCM coder in G.721 with a low-delay code excited linear
predictor (LD-CELP). The main principle of a CELP coder is to match a
group of speech samples with a codeword from a code book. Compression
is achieved by transmitting only the index of the optimum codeword. The
optimum codeword is selected so that the mean square error between the input
speech and the synthesized speech is minimized.

Presently, within ITU, a videoconferencing standard referred to as H.324 is
being developed for videoconferencing at bit rates lower than 64 kbits/s. A
speech coding method referred to as G.723 has been proposed as part of the
H.324 standard suite. The 6.3 kbits/s mode of G.723 provides speech quality
equivalent to that provided by the 32 kbits/s G.726 standard.

In the next sections we describe in more detail the MPEG-i and the AC-3
audio standards. Some fast algorithms for the implementation of MPEG audio
are also discussed. We conclude with a short description of commercially
available audio decoders.
300                                                                                        CHAPTER 16




16.2 MPEG AUDIO ENCODING
The MPEG audio coding algorithm is the first international standard for
the compression of digital audio signals. It can be applied to streams that
combine both audio and video information or to audio-only streams. Like
the MPEG video standard, the MPEG audio standard specifies the syntax of
the coded bit stream, defines the decoding process, and provides compliance
tests. This allows for different encoding algorithms, provided that the
encoded data can be decoded by an MPEG compliant decoder. The MPEG
audio compression standard achieves compression by exploiting the spectral
and temporal masking effects of the ear. It uses subband coding and a
psychoacoustic model to eliminate information that is irrelevant from a human
sound-perception viewpoint.

Figure 16.1 shows a block diagram of the MPEG encoder for a single audio
channel. In multichannel systems, the process is repeated independently for
each channel. Input pulse code modulated ( PCM) samples have 16 to 20 bits


                                                                                                           + 小
                                                                                           c>
                           H1
                                                                                      j_
                                                                                 帥r
                                                                    0uantizer,
      Input
                                                                                                             ＝
                                                      느
                                                      mHm
                                                        g
      (PCM)                H2
                    =b
                                                                                                느mXm죠三그＞
                                                                                                           尸＝ 口三0
                             I           1
                             I           1                                                                          +
                             1           I



               \1
                    뇨
                           H32          32i   -   >           >
                                                                    Quantizer．
                                                              scate factors
                                                                                 鈿酊   H
                         subband filtering
                                                                  bit 訓어月ti아）

                                  Masking threshold and
                                  bit allocation calculator
                                  Psycho-acoustic Model



              Figure 16.1 Block diagram of the MPEG audio encoder.

of precision and are sampled at 32, 44.1, or 48 kHz. The first stage of the
encoder is a subband analysis filter that can be viewed as filter bank with 32
band-pass filters. The frequency response of each 512-tap band-pass filter is
derived by frequency shifting the response of a prototype low-pass filter. The
Standards for Audio Compression                                                        301




output of each filter is decimated by a factor of 32 so that for every 32 input
samples the subband filter generates 32 output samples.

In the next stage (the scaler), the output of each subband filter is normalized
by scale factors that will be transmitted together with the compressed bit
stream as side information. Scale factors correspond to the maximum absolute
value of every 12 consecutive output values in each subband. Based on the
frequency characteristics of the input signal and the desired bit rate of the
compressed signal, a psychoacoustic model computes masking thresholds and
bit allocations. This information is used by the quantizer and coder units.
Finally, the quantized subband samples, the scale factors, and the bit-allocation
information are multiplexed to form the compressed bit stream.



16.2.1    Subband Analysis

As mentioned before, the subband analysis filter can be viewed as a filter
bank with 32 filters. Le比떠 deno妃 an au小毗帥뻔e at time t and 瓦（t) denote
the impulse response of the i-th filter. Then the output of each filter can be
expressed as
                                              511

                                s(i) = ＞二 x(t - n)H:(n),
                                              n=O

where
                                                    [(2i   + 1) (n   -   16)
                                =             cos
                                                               64
                                    h
                         (n)
                                        (n)
                     H
                                                                               lr]

and h(n) is the impulse response of the prototype low-pass filter. For
each block of 32 samples, a direct implementation of (16.1) requires 32 x
512 = 16,384 multiply-accumulate operations. MPEG uses a more efficient
implementation derived from the theory of polyphase networks. Polyphase
filters are more efficient because with an appropriate transformation they allow
one to decimate the input of the filter bank rather than the output. Figure 16.2
shows a block diagram of such an implementation. The corresponding flow of
operations as defined by the MPEG standard is as follows:


1   Input: 32 new samples x(i) are shifted into the FIFO buffer.

     Windowing:
                               z(i) = C[i]x(i), i = 0, 1, ' . · ,511,                (16.3)
302                                                                                                                         CHAPTER 16




                                        ＜口
                                                                            512 sample FIFO
                       (i)
                   x
              m＝             十니              k                      k+64                 k+128                      k+448
      32 samples

                                                                                                             C[k+448]
                                                                                                                  니：>




                                                                                                                  s(i) output



                                                                                                                M[i, k]



              Figure 16.2                                 MPEG implementation of the subband analysis
              filter.


      where C[ ] is one of 5 12 coefficients defined in the standard.

口     尸artial calc끄lation:
                                                                                    7

                                                                                         :(i+ 64j),i= O. 1. . · · .63.                (16.4)
                                                                            j= O




      Marrixing operation.'
                                                                            C3
                                                                s(i) = ) .' y(k).\I[i. k]. i = 0. 1, , · ' ,31,                       (16.5)
                                                                            k=O

                                                                            1             16)
      where
                                  3fli.      kJ       =   （】
                                                           O.   6
                                                                    [(2z+
                                                                                X
                                                                                    k_          "]   ·




      Output: Output 32 subband samples s(fl.


From Figure 16.2 and the above flow of operations one can derive the following
equation for the output of the i-th filter.
                                   63             7

              s    )= 二 Z M[i, k] (C{k + 64j}x(k + 64j)),                                                       0, l , · . . , 3l ,   (16.6)
                                   k=O j= O
Standards for Audio Compression                                              303




The above implementation requires 512 + 32 x 64 = 2,560 multiplications
(512 for the windowing operation and 2,048 for the matrixing operation) and
64 x 7 + 32 x 63 = 2,464 additions. The matrixing operation (16.5) is the
most time consuming with 2,048 multiply-accumulate operations.



16.2.2    Fast Matrixing Computation

The computational complexity of the matrixing operation can be reduced
further using a fast inverse DCT (IDCT) transform. Let y(k) be the output of
the partial calculation step (16.4). If

                      I y (16)                丸=0
             y' (k) = 4 y(k + 16) + y(16 - k) k = 1, 2, ..., 16           (16.7)
                      1 y（丸＋16) - y(80卞大） k= 17, 18, ..., 31

then, it can be shown that the output of the matrixing operation can be
computed as
                       31
                . .   t11   1. = .   r 而 .    . .i               -.
               s(i) = ) .y' (k)cosI ; .-(2i+ 1)kI ,i= U, 1, ' ", 31,      (1t.8)
                      -              io4             J
                      k=O

where s(i) is (within a scale factor) the 32-point IDCT of y'. Using a fast
IDCT algorithm, such as Lee's, the IDCT can be computed with only 80
multiplications and 209 additions.



16.2.3    The Psychoacoustical Model

A key, and computationaly intensive, component of the MPEG encoding
standard is the psychoacoustic analysis of the input signal. This analysis
is performed in parallel with the subband filtering operation. The first step
in this process is the computation of the masking curve according to the
frequency-masking properties of the human ear. From the masking curve, a set
of masking thresholds is derived for each subband. Each of them determines
the maximum energy acceptable for the quantization noise in each subband
(that is, below this level the noise will not be perceived). The computation of
the masking curve requires a very accurate spectral analysis of the input signal.
In MPEG, the spectrum of the input signal is computed using a 1,024-point
fast Fourier transform ( FET) of the input samples. From the spectral lines,
304                                                            CHAPTER 16




the psychoacoustic model determines tonal and nontonal components and
determines the final masking curve. Figure 16.3 shows a plot of a typical
masking curve.




                                             frequency


             Figure 16.3 Plot of a typical audio masking curve.


For a given bit rate and perceptually lossless compression, all of the quanti-
zation noise should be below the masking thresholds. However, for low bit
rates this is usually not the case. In such cases, the psychoacoustic model uses
an iterative algorithm that allocates more bits to the subbands where increased
resolution will provide the greatest benefit.

Note that MPEG is not enforcing the use of a psychoacoustic model. For
example, applications that can afford high bit rates can use simpler bit
allocation schemes,such as assigning more bits to the subbands with the lower
signal to noise ratios.




16.3 MPEG AUDIO DECODING
Figure 16.4 shows a block diagram of an MPEG audio decoder. The MPEG
audio decoder reverses the encoding operation by performing the following
steps.


 1. Frame unpacking and parsing: The bit stream is parsed, and the various
    pieces of coding information are demultiplexed.
Standards for Audio Compression                                                                                                     305




   Encoded                                                                                                              PCM
                           Frame                                                                 Inverse
     1Hd>
                                           -    >       Reconstruction                                              -     >
                       Unpacking                                                                mapping
                                                                                      H令
   bit stream                                                                                                           Output




            Figure 16.4 미ock d奴얍am of the卜4PEG aud幻decoder.


 2. Reconstruction.' The bit allocation information is decoded, and the scale
    factors are extracted.

 3. Inverse mapping: Data samples are dequantized and denormalized and
    then processed by a subband synthesis filter.

 4. Output: The output of the subband filter is translated into PCM audio
    samples.


Among these steps, subband synthesis is the most compute intensive. Figure
16.5 shows a block diagram of the subband synthesis filter as defined by
the MPEG standard. From Figure 16.5, there are three main operations in
subband synthesis: (1) the matrixing operation, (2) data shifting, and (3)
the windowing operation. In most implementations, the shifting and the
windowing operations are combined into a single step.



16.3.1      Fast Matrixing Operation

From Figure 16.5, the matrixing operation in subband synthesis is defined as
            31                                 31

  V(i) =    > N{i,
            k=0
                                       = 가이計k+1小＋16小（蜘 = 0,1,.··,63,
                                               k=0
                                                                    (16.9)
where s(k), k = 0 to 31 denote input encoded audio samples. Brute force
evaluation of V(i) requires 32 x 64 = 2,048 multiply-accumulate operations.
Let S denote the 32-point DCT of s, defined as
                                 31


             S   (i)   ＝
                            k=0
                            二.         ［궁；
                                      0s         (2丸＋       1)   i]   s   （丸）   ,i=        0,   1,   "   ·   ，31.
                                                                                                                                 (16.10)
306                                                                                                                   CHAPTER 16




                                 matrixing                                        1024 samples V buffer
                                                                                        i = 0 to 63
                           31
            Input s(i)
                           ZN[i, k] s(k)
                                                          (i)
                                                      V
                     t>                                                                                               1+960

                                                                                                       寸
          32 sam히es        k=0
                                  卜＝0 to 63
                                   A                                    U(64 I 니) =V(1281 +j)
                                      N[i, k]                        U(64 1+32 +j) = V(1281 + 96 +j)
                                                                                  512 samples U buffer

                                                 p.
                                                                15
                                32 PCM <＝그
                                                          Z 빠+ 32i)                                         O   (1]
                          output samples                  i=    0
                                                                                             W(i) = U(i) D[i]
                                                                 j=O to 31
                                                                                                                      -i


                                                                                  windowing



      Figure 16.5         MPEG implementation of the subband synthesis
      filter.


It can be proven that all elements of V in (16.9) can be derived from the values
of S as follows:

                                  r   S   (i+
                                                16)                  i =     O,
                                                                                    1,   "     "   ,
                                                                                                       15
                                  1 U                                i= 16

                   ‘「（」
                     『）={ :＄訂i) 乞忿1j三                                                                                         (16.11)
                                  1 -S(O)                            i= 48
                                  ( -S(i- 48)                        i= 49, 50, " " ' , 63


Figure 16.6 shows a graphical representation of the above equation. If S(i),
the output of the 32-point DCT, is divided in two parts A(i) and B(i), then
V can be composed by the appropriate shifting and manipulation of these
parts. Shapes of data in Figure 16.6 were chosen arbitrary to better show the
symmetries within V.
Standards for Audio Compression                                             307




                         S




                                     ｛그
              V


                             -B（따 /／쓰쁘-J
                                                                (i)
                                                            A
     Figure 16.6 Graphical representation of data dependencies in the
     output or tue matrixing operation in subband syntflesis.


16.4 LAYER CODING OPTIONS IN MPEG
The MPEG audio compression standard defines three layers of compression.
Each successive layer offers better compression performance but at a higher
complexity and computational cost. All three layers support bit rates as low as
32 kbits/s for a single channel.

Layer I is the simplest of all and provides good quality audio at 192 kbits/s.
The highest supported bit rate for Layer I is 448 kbits/s. Layer II codes data
in larger groups, uses a more complex psychoacoustic model, and provides
CD-audio quality at 128 kbits/s per channel. The highest supported bit rate for
Layer II is 384 kbits/s.

Layer III is the most complex of the three and can be used in low-bandwidth
or noisy channels. Like Layers I and II, it uses a subband filter, but the
output of the filter bank is processed further by a modified DCT. Other distinct
features of Layer III include nonuniform quantization, adaptive segmentation,
and entropy coding. Layer III is also performing a better compression of stereo
signals by exploiting the cross-correlation between the left and right channels.
The highest supported bit rate for Layer III is 320 kbits/s. Due to the additional
complexity of Layer III, most of the existing applications use either Layer I or
Layer II.
 308                                                              CHAPTER 16




 16.4.1 MPEG-2 Audio Coding

 The MPEG-2 audio compression standard is an extension of MPEG-I with
 the following added features. .
                                      t

       Multichannel input: MPEG-2 supports up to five high-fidelity audio
       channels plus a low frequency enhancement channel (these six channels
       are also known as 5.1 channels). Thus it is suitable for the compression of
       audio in HDTV or digital movies.

       Multilingual audio support: Up to eight commentary channels are sup-
       ported.

       Lower bit rates: Compressed bit rates down to 8 kbits/s are now supported.

       Additional sampling rates: In addition to the original sampling rates of
       32, 44.1, and 48 kHz, MPEG-2 accommodates sampling rates at 16, 22.05
       and 24 kHz.


In many ways, the MPEG그 audio standard is compatible with the MPEG-i
audio standard. For instance, MPEG-2 audio decoders can decode MPEG-i
audio bit streams and MPEG-I audio decoders can decode the two main
channels of the MPEG-2 audio bit streams.




16.5      THE AC-3 CODING STANDARD
The AC-3 audio coding scheme from Dolby Laboratories was developed
in response to a need to provide high-quality, multichannel, digital audio for
FID1'V and film. For example, a digital film sound system has 5.1 channels
(left, center, right, left and right surround, and a subwoofer.) This audio
information has to be placed in the film without interfering with either the
picture or the analog sound area. It was determined that one could use the
film area between the spocket hole perforations to place a 320 kbits/s error
corrected audio stream. In 1991, Star Trek VI was the first film coded with the
AC-3 system. In 1993, after successful field tests, an FCC advisory committee
recommended the use of Dolby AC-3 for the Grand Alliance HDTV system.
Standards for Audio Compression                                                                                 309




The MPEG-2 committee is presently considering a non-backward compatible
(NBC) extension to the current MPEG-2 audio coding standard. AC-3 is being
considered as a candidate coder that may be supported by the NBC extension.



16.5.1        The AC-3 Encoder

Like MPEG, the AC-3 system uses transform-based coding and a psy-
choacoustic model to eliminate information that is irrelevant to the human
hearing system. A block diagram of an AC-3 encoder is shown in Figure
16.7. The audio input, sampled at 48 kHz, is first transformed from the time

                                                                                              Side

                                        Ideal bit                          Bit 出幻cat幻n    In幻rmation
                                                                      [>
                                        쇰！어：ator                            controller
                                   t.
                                            Mantissas


  Input
          니   Filter       bank
                                        1               Quantizer

                                                           수   B小川1呻tion
                                                                                          너   Mux 吟
                                                                                               Lt     Coded
                                  Exponents
                       V                                                                              stre계11
                                                        Core bit
                 Spec打al
                                                        訓ocator
              enve幻pe




                                               나
              encoder                                      A


                                                    ' pectrd絮： ":'"            Spectral
                                                                               envelope




              Figure 16.7 Block diagram of the AC-3 audio encoder.

domain into the frequency domain using a filter bank. The block size is
512 points and overlapping blocks of 512 windowed samples are transformed
into 256 frequency domain points. According to Dolby, critical sampling
and efficient algorithms allow this operation to be performed with only 13
multiply-accumulate operations.

Each output point of the filter bank is represented by an exponent and a
mantissa. Coding of the exponent allows for a wide dynamic range, while
310                                                             CHAPTER 16




quantization of the mantissa results in quantization noise. The exponents from
each channel represent the overall signal spectrum and are referred to as the
S꺄口r口／enve勿pe. F恂兀nents fr帥 each 벼ock are encoded using one of three
differential coding schemes. The coding efficiency of these schemes ranges
from 2.33 bits per exponent to 0.58 bits per exponent. The AC-3 encoder
selects the appropriate scheme based on the signal characteristics. However, it
is common for multiple blocks to use the same exponent set. In a typical case,
the spectral envelope is sent eveiy six audio blocks (32 milliseconds) for an
average bit rate of less than 0.39 bits per exponent. After the transformation
of the input samples, the encoder determines the optimum bit allocation
and quantizes the mantissas. There are two main bit-allocation strategies
for psychoacoustic based coders: forward-adaptive or backward-adaptive bit
allocation.

In forward-adaptive bit allocation the encoder uses only the input signal to
determine the bit allocation, which is later explicitly coded in the output bit
stream. For example, this is the strategy used by the MPEG audio coder. This
is the most accurate method; however, it consumes significant portion of the
available bandwidth. For example, MPEG (Layer II) may allocate close to 4
kbits/s for this side information. Another advantage of forward bit allocation
is that the decoder requires no prior knowledge of the psychoacoustic model.
This allows the encoder to be updated as needed without affecting the design
of the decoder.

In backward-adaptive bit allocation, the decoder can determine the bit
allocation directly from the encoded data without any side information from
the encoder. This requires that both the encoder and the decoder have
identical copies of the bit allocation scheme. This technique is not as accurate
as forward-adaptive bit allocation, and the psychoacoustic model cannot be
updated after the decoders are built.

AC-3 uses a hybrid forward/backward model. There is a core backward-
adaptive bit allocator that resides on both the encoder and the decoder.
However, the encoder can use any other psychoacoustic model to determine
the optimum bit-allocation. If a comparison between the outputs of the
optimum and the core allocator shows that the default bit-allocation needs to
be improved, then the encoder tries first to modify some of the parameters
used in the core model. If no further improvement is possible with the core
model, then the encoder can explicitly transmit some additional bit-allocation
Standards for Audio Compression                                                             311




information. Since the core algorithm performs well in most cases, only small
changes in bit-allocation need to be transmitted. For multiple channels, bits
are allocated from a common pool of bits.



16.5.2         The AC-3 Dec어ier

A block diagram of the AC-3 decoder is shown in Figure 16.8. The coded


                                                          Mantissas
                                      Inverse quantizer


                             Side in幻rmat幻0
                                                                      V
                                                                                    PCM
                                              Core bit         Inverse filter
                                                                                -     >
                                                                   bank
                                mH>
                                          케ocator
         ＋呻呵
     A
                                                                                    Audio
     bit stream

                                      Spectral env이야）e
                                              de（力der       Ex口m帥1S




               Figure 16.8     Block diagram of the AC-3 audio decoder.

stream is first demultiplexed to generate the spectral envelope, the quantized
mantissas, and any bit-allocation side information. The spectral envelope is
decoded and the mantissas are dequantized using the core bit allocator and
the side bit allocation information. The decoded mantissas and exponents
are combined to form the frequency coefficients and an inverse filter bank
translates the frequency data into PCM audio signals.

The AC-3 bit stream syntax supports the coding of one main audio service
with one to 5.1 channels. Other services, such as information for visually
and hearing impaired, may also be embedded into the AC-3 bit stream.
Single channels may be coded at bit rates as low as 32 kbits/s. The maximum
supported bit rate is 640 kbits/s. The higher bit rate allows for the incorporation
of additional services without compromising the audio quality of the main
service.
 312                                                             CHAPTER 16




 16.6 HARDWARE IMPLEMENTATION
      OF AUDIO CODECS
Most of the commercially available video processors require an external audio
coder or a programmable signal processor for processing the audio. Note
that the amount of audio data in a video stream is by no means insignificant.
Consider the case of recording a movie on a compact disc using a compression
rate of 1.41 Mbits/s (the maximum data rate of a CD). Using a stereo soundtrack
with 128 kbits/s per channel, this rate is divided into 1.15 Mbits/s for the video
and 0.256 Mbits/s for the audio. Thus audio represents 18 percent of the
overall data rate. Timing profiles of an MPEG-I decoder on a general purpose
RISC processor showed that audio decoding and audio-video synchronization
may represent up to 30 percent of the overall decoding time.

Table 16.2 shows the most common arithmetic operations in Layer II MPEG
audio decoding (the symbol % denotes modulo operation). A similar analysis


                    Function                Operations
                 Degrouping          y = c%a, c = c/d
                 Dequantization      11 = (x + a)b
                 Denormalization     y = ax
                 Matr奴ing            y = ax + b, y = ＞二i xici
                 Windowing           y = xa, y = Zi 切i

         Table 16.2   Arithmetic operations in MPEG audio decoding.


of the operations in other audio coding algorithms shows that multiplication
and addition are the most common operations. Hence, general-purpose DSPs
are ideally suited for audio processing.



16.6.1    Commercially Available Audio Decoders

Commercially available audio processing ICs provide a low-cost solution to
the decoding of compressed audio. They are either dedicated or programmable
DSPs and provide a glueless interface to memory and a host controller (if
needed).
Standards for Audio Compression                                          313




The CS4920 from Crystal Semiconductors is a programmable DSP for either
MPEG-I or AC-2 (precursor to AC-3) audio decoding. It has a 24-bit
architecture and is the only audio decoder with an on-chip programmable PLL
clock generator and dual 16-bit digital to analog converters (DACs) for the
direct generation of stereo audio from a compressed digital stream. Its audio
transmitter is compatible with the SonyfPhilips digital interchange format
(SPDIF).

The L64111 from LSI Logic is a two-channel MPEG audio decoder. It can
decompress both MPEG-i and MPEG-2 (two channels) streams (Layers I
and II). It supports bit rates from 32 (mono) to 384 kbits/s (stereo). Data
can be loaded either bit-serially or in parallel. The L64111 has a 24-bit
architecture and runs at 25 to 30 MHz. The processor uses a serial divider for
the degrouping operation and a two-cycle 24-bit multiplier-accumulator for all
other decoding operations.

Most of the DSPs from Texas Instruments could be used for audio coding
or decoding; however, TI also provides a dedicated MPEG-i audio decoder
(Layers I and II), the TMS320AV110. At 33 MHz it can execute 16.5 M표）S.

Another audio decoder is the ZR38000 programmable DSP from Zoran. This
is a 20-bit processor w姓ia 20 x 20小山仙川plier, a barrel shifter, and a 48小it
accumulator. The processor has a 16-word instruction cache and supports
block floating-point operations. The ZR38000 can execute a radix-2 FFT
butterfly in four cycles. This allows it to compute a 1,024-point radix그 F可
in 0.877 ms (using a 25-MHz clock). Using the ZR38000 core, Zoran plans to
introduce dedicated processors for six channel AC-3 decoding (the ZR38500),
two channel AC-3 decoding (the ZR38501), and two-channel MPEG audio
decoding (the ZR3851i). According to Zoran, the ZR38500 is the only IC that
can decode in real-time a six channel AC-3 stream.




16.7     TO PROBE FURTHER
The G.72x speech coding standards are described in the ITU publications [51],
[501, and [52]. In addition, for the G.722 standard, an extended summary is
given in [130] and a custom hardware implementation is described in [193]. A
314                                                            CHAPTER 16




hardware implementation of the G.728 on a general-purpose DSP is reported
in[6].

The MPEG audio standard is based on the MUSICAM subband coder with
some elements (in Layer III) from the ASPEC transform coder. Musmann
[142] provides details on the early efforts by the International Standards
Organization (ISO) to define an audio compression standard and discusses
similarities and differences between the MUSICAM and ASPEC coding
algorithms. Another description of the MUSICAM algorithm can be found in
[38].

The MPEG-I and MPEG-2 audio standards are described in the third part
of the ISO documents [84] and [86]. In [1501 and [179], Pan and Shlien
provide additional references and details on the polyphase filter bank, the
psychoacoustics models, and the bit-allocation algorithms. Proofs for the
DCT-based matrixing operations in subband coding are given in [151] and
[107]. Lee's fast DCT algorithm is described in [111]. An excellent tutorial on
MPEG audio compression is presented in [152]. For additional details on the
hardware implementation of an MPEG audio decoder, Matun [133] provides
a description of the architecture of the MPEG decoder from LSI Logic. The
final AC-3 standard is still under development; however, Todd et al. from
Dolby give a good overview of the AC-3 system in [185]. For those interested
in how AC-3 is integrated into the Grand Alliance HDTV system, a general
overview of that system is given by Hopkins in [74]. A discussion of the
proposed speech coding standard G.723 can be found in [174].
                                                             17
   NONSTANDARD COMPRESSION
                TECHNIQUES




17.1 INTRODUCTION
Standard compression schemes, such as JPEG and MPEG, have been widely
supported by the industry; however, this has not stopped the development
and marketing of several proprietary image and video compression schemes.
Examples of such schemes include the Kodak Photo-CD compression and
storage format, the QuickTime environment from Apple, and DVI technology
from Intel. There are various reasons for the introduction of proprietary
compression schemes:

    Certain applications are self-contained, and there is no need to exchange
    their data with other platforms (such as a stand-alone image data-base
    system).
    Computational requirements of the standard algorithms are beyond the
    capabilities of a particular platform (such as the software-based video
    playback on low-end personal computers).
    New n垠rket areas 아妃n (such as 小帥카 ph아ography).
    There is dissatisfaction with the capabilities of the standard algorithms
    (such as video teleconferencing).
    There is concern about royalties (such as arithmetic coding in JPEG).

Even though details on proprietary schemes are seldom published, most of
the nonstandard techniques seem to be based either on vector quantization
 316                                                          CHAPTER 17




(VQ) or wavelet-based subband coding. After a short overview of VQ and
subband coding, we briefly present a few of the commercially available and
nonstandard compression techniques.




 17.2 VECTOR QUANTIZATLON
In transform-based coders,such as JPEG and MPEG,blocks of spatial data are
first transformed into the frequency domain. The image energy is now packed
into a few of the frequency components that are carefully quantized to remove
information that is irrelevant to the human visual system. Decompression is
performed by reversing the encoding process. After an inverse quantization,
the dequantized frequency components are translated back to spatial data by
an inverse transform.

 A main characteristic of such transform-based algorithms is that both the
encoder and the decoder have ;similar levels of computational complexity.
However, most multimedia applications are CD-ROM based and require
only real-time decoding of the embedded video clips. Unfortunately, even
with fast transform algorithms, real-time decompression may be beyond the
capabilities of low-end machines. An alternative compression scheme is
vector quantization (VQ) coding. VQ processes image blocks directly in
the spatial domain. It has a far more complex encoder than transform-based
coders, but it allows for very fast decoding.

Figure 17.1 shows a block diagram of a VQ coder for image compression.
An input image is first segmented into nonoverlapping blocks. Each block is
regarded as an M-dimensional vector, where M is the number of pixels in the
block. For example,a 4 x 4 block corresponds to a vector of dimension 16. The
principle of VQ is to match each input vector to a codeword (or reproduction
vector)from a codebook so that the distortion between them is minimized. The
codebook is generated a priori from a collection of representative images and
should be a good representation of all possible image vectors. Compression
is achieved by transmitting the index of the best codeword. For example, if
the input vector has 16 x 8 bits and the codebook has 28 = 256 entries, then
the corresponding compression ratio is 16:1 since each 4 x 4 block can be
represented by an 8-bit codeword index.
Nonstandard Compression Techniques                                                                               317




                Input   Raster to           미없ortion      Index      Codebo아（           Vec佃r           Output
                                                                                                       <>
                                                                                H令
                                                                                       to Raster
                                    -
                                                                                                   H
                         Vector
                 mm令


                                           C계culation                    6
                                                   수                  Address
                                           Codebo아（

                        VO encoder                                VQ decoder


                              Figure 17.1              Block diagram of a VQ image coder.



Decoding in VQ is much simpler than encoding. The decoder, which has
an identical codebook, uses the codeword index and a simple table look-up
operation to reconstruct the original image. The simplicity of the VQ decoder
is the principle reason that VQ is the method of choice for image and video
coding on computing platforms with limited resources, such as PCs and
portable electronic note pads. The complexity of the VQ encoder depends on
the distortion measure and the search algorithm used for determining the best
codeword.



17.2.1 Codebook Search Algorithms

Given an input vector x = x1, x2, · .. , 勾i and a set of N M-dimensional
codewords {c', c2, . . . ,cN}, a commonly used distortion measure in VQ is the
mean square error
                                                           人4
                                        MSE(x, c') =＞二(xk- 4)2,i= 1, 2, · · · ,N.                            (17.1)
                                                          k=1

From (17.1), each evaluation of the MSE requires M data loads, M subtractions,
4'f multiplications, and M - 1 additions, for a total of 4M - 1 operations.


十nalternative                     measure     is   the mean absolute error

                                        入了AE(x, c1)                      ,i= 1, 2, . · · ,N.                 (17.2)
 318                                                               CHAPTER 17




 The MAE criterion requires fewer computations; however, it may compromise
 the fidelity of the reproduced images.

The most straightforward search technique is to compare each input vector
with every entry in the codebook and select the codeword for which the
distortion is minimum. This form of codebook searching is referred to as
full-search and the encoding method is often referred to as full-search VQ.
However, this method can be prohibitively expensive even for coders with
small block sizes and codebooks. For example, using the MSE criterion and a
codebook with 256 entries, this approach requires at least 256 x 63 = 16,128
operations per 4 x 4 block.

The amount of processing can be significantly reduced ifone uses a binary tree-
search vector quantizer(TSVQ). In binary TSVQ, the codebook is organized
in a tree structure. Figure 17.2 shows such a tree with two levels. Starting




              Figure 17.2 Block diagram of a VQ image coder.


from the root, at each level of the tree the input vector is compared with only
two codewords. Based on the comparison, one of the branches is chosen and
an index bit of either 0 or 1 is transmitted, The process continues until a leaf of
the tree is reached. For N codewords, this approach requires the evaluation of
only 2 x log2iV distortions. For a codebook with 256 entries, a TSVQ requires
only 2 x 8 x 63 = 1,008 operations per 4 x 4 block.

TSVQ encoding is much faster than full-search, however, it may also result
in lower image quality. TSVQ is suboptimal because it may lead into a
local minima in the search space, whereas full-search VQ finds the global
minima. These techniques can be further refined or improved by using adaptive
codebooks or pruned tree-search algorithms.
Nonstandard Compression Techniques                                     319




17.2.2   Hardware Considerations

Consider now the hardware implementation of a TSVQ coder. Given an input
vector x, at each level of the tree we need to compute the difference

                      dij = MSE(x. ct) - MSE(x,c).                   (17.3)

From (17.1) and (17.3), after expanding the quadratics and some simplifica-
tions,

                肉＝二［
                   （山' _(c) )2] +>2Xk(Ci -ci).                       (17.4)
                      k=1                    k=1

From (17.4), the first summation is a constant that is independent of x and
it can be precomputed and stored in memory. The differences in the second
summation can also be precomputed. Thus, if ai3 denotes the first summation
in (17.4) and ej = 2(c' - c3), then d13 can be expressed as

                                   勺
                                        MZ   까 Uk          +=
                            d,, = a23 +) : xkek.
                                  O             e                    (17.5)
                                       k=1




Evaluation of (17.5) on a general-purpose RISC-like processor requires M + 1
data loads, M mu川帥cations, and 入I ad小tions, f야 at야키 of 3M+1아氾rations
per level of the tree. For M=16 (such as 4 x 4 blocks), 49 operations are
required per level of the code tree. Table 17.1 shows the MOPS requirements
for real-time TSVQ (30 fps), 4 x 4 blocks, various frame sizes (4:2:2 color
images), and two codebooks: one with 256 entries and one with 1,024 entries.
For comparison, a DSP processor with a multiply-accumulate unit can perform
a data load and a multiply-accumulate operation in one cycle, thus (17.5)
can be computed in M + 1 clock cycles. Assuming again 4 x 4 blocks and
a codebook of only 256 entries, real-time TSVQ encoding of CIF images
on a DSP requires a clock frequency of at least 51 MHz. This assumes no
delays in accessing the memory (approximately 4 Kbytes) and does not take
into consideration any other computations, such as color transformations or
lossless compression of the VQ output using an entropy coder.

One approach to reducing the clock speed is to use multiple processors and
pipelined processing. In TSVQ, only one node is active at each level of the
coding tree. Furthermore, computations at one level do not require codewords
from another level. This localization of operations allows the codeword
memory to be partitioned into separate memories for each level of the tree.
320                                                             CHAPTER 17




                            Codebook s]ize = 256
                           Frame Size MOPS
                           QCIF             37.25
                           CIF             149.02
                           SW              124.19
                           CCIR           508.03
                           Codebook size = 1024
                           Frame Size MOPS
                           QCIF           46.57
                           CIF           186.28
                           SW            155.23
                           CCIR          635.04

      Table 17.1 MOPS re9uirernents.for,TSVQ encoding at 30 fps
      ror '+ x '+ DIOCKS anu airrerent cocieoooK anci rrame sizes.



Figure 17.3 shows the implementation of a TSVQ encoder using a linear
array of L = log2N processors, where each processor is mapped to a level
of the coding tree. An output "Ready" signal from processor P1 resets the




      Figure 17.3 Block diagram of a pipelined TSVQ image coder.


accumulator of P,+i and initiates processing at the next level. Each processor
adds the result of its computation to the index data path. The last processor
returns the index of the best codeword. Note that each processor requires
different sizes of memory. Since each level i (i = 0, 1, ..., L - 1) of the tree
Nonstandard Compression Techniques                                         321




has 22 nodes, and each level is mapped into a single processor, from (17.5),
processor P1 requires (M + 1)21 words of memory. This pipelined scheme
allows the clock frequency of each processor to be reduced by L.




17.3 SUBBAND CODING
The main principle behind transform based coding is that data in the transform
domain have a more compact representation than data in the spatial domain.
The transformation between the two domains can be performed either on a
block by block basis (as in JPEG) or as in the case of a subband coder using a
filter bank.

Figure 17.4 shows a block diagram of a subband coder. In the encoder, the




               Subband                                       Interp이at幻n
        >
               F小ering         Coder                  -
                                                             and Subband
                                              0鈿아
    -
                                       니
             and Decima如n                                     Synthesis

            Subband encoder                Subband decoder


                   Figure 17.4 Block diagram of a subband coder.


image is first divided into multiple frequency bands using a combination of
low-pass and high-pass filters. For example, Figure 17.5 shows a four-band
filter bank and the corresponding partition of the image spectrum in octave
bands. Filtering is followed by a 2 x 2 decimation operation where each
subband output is subsampled by a factor of two in each dimension. In effect,
decimation translates each subband back into a baseband image but with only
one-fourth of the original pixels. Thus, even though there are four output
channels, the output bit rate is the same as the input bit rate. The process of
 frequency subdivision can be iterated on each of these four subbands.

 Subband filtering by itself is a lossless operation. The input data is simply
 decomposed into multiple data streams, without any loss of information. Data
 322                                                                               CHAPTER 17




                                                                         了
                                                                 0)2
                                              yll
                                                                                  It
                                                                 1                         1
                                                            22i          12                1 22
                                                                 +
                                              y12
                                                             4       H   卞    -        -   I-
                                                                                                -




       x                                                         1                         1
                                                            21 1         11                '21
                                              y21
                                                                 刃
                                                                         12                1 22

                                              y22

                            a)                                           b)


           Figure 17.5 (a) Block diagram of a four-band filter bank. (b)
           Partition of the image spectrum.



compression is achieved by discarding subbands that are irrelevant for an
application and by the efficient encoding of the remaining data samples in
each subband. Coding schemes that have been applied to subband coding
include predictive coding and quantization (DPCM), vector quantization,
entropy coding, and arithmetic coding.

The block diagram of a subband synthesis filter is shown in Figure 17.6. After



                     yll



                                     十              h
                                                        '




       Figure 17.6         Block diagram of a four-band synthesis filter bank.


the decoding of the subband data, each subband is upsampled by a 2 x 2
Nonstandard Compression Techniques                                         323




inte叩olator and then filtered by a band-pass filter that eliminates aliasing
                                                                            t
produced by the upsampling. The subbands are finally summed to reconstruc
the original image.

As an example, Figure 17.7 shows the spectrum of a signal at the various
stages of a two-band subband coder. The input signal is first decomposed
into two bands using a low-pass and a high-pass filter. The bandwidth of
these signals is half of the original bandwidth; hence, according to the Nyquist
theorem their sampling rate can also be reduced by half. This is accomplished
by downsampling each signal by a factor of two (in other words by throwing
away every other sample). With downsampling, the aliased output of the
high-pass filter is shifted back into the baseband.

In the receiver, upsampling (a zero is inserted between every two samples)
causes alias spectral signals (shown in gray) that can be suitably filtered with
a low-pass and a band-pass filter. The filtered signals are then added to form
the reconstructed signal.




    A1 b프EmC띤H
                                                               Input
                                                              Spectrum
                               口＞
                                                            Low and 1小gh
                                            \\
                                                             Frequencies



                        V
                                                            Downsampling
                                                               by 2

                                                             Upsan갸)Iing
                                                                by 2




     >m
     m
     뇨 0
       mm工 11lV
                  V
                                                             Band-pass
                                            r>                Filtering



                                    /1                         Output



                      Figure 17.7    Signal spectrum in subband coding.
  324
                                                                   CHAPTER 17




  Subband coding is more computationally expen
                                                  sive than block-based coding;
  however, it has many other advantages, includ
                                                ing the following:

        Since the subband filters operate on the whole
                                                       image, subband coded
        images display fewer artifacts (such as blockiness) than
                                                                 block-coded
        images.

      Subband coding is more robust under transmission or decod
                                                                    ing e口ors
      because errors on a particular subband may be masked by the
                                                                  information
      on the other subbands.

       Subband coders allow for better data rate control
                                                           during encoding or
      decoding by the selective transmission or decompression of subbands.
                                                                            For
      example, to reduce the data rate in a video teleconferen
                                                               cing application,
      the image of the active speaker may be encoded at full resolution,
                                                                          while
      the images of the other participants may be enc어jed and decoded at lower
      resolutions.


Since the coding part of a subband coder uses compression techn
                                                                   iques that we
have already discussed in earlier chapters, in the remaining
                                                             of this chapter we
examine some of the subband filter design and implementation
                                                                 issues.


17.3.1     Subband Filter Design

The analysis and design of the subband filter bank can be
                                                             simplified if we
assume that all two-dimensional (2-D) filters are separable.
                                                             A 2-D filter with
impulse response h(m.,n) is defined as separable if

                             h(m,n) = hi(m)h2 (n),                         (17.6)
 where hi(rn) and h2(ri) are the impulse responses of
                                                            1-D filters. Using
 separable filters, a 2-D filtering operation can be performed
                                                                by filtering first
each row and then each column of the image using the
                                                          1-D filters. Following
this approach, the four-band subband filter of Figure 17.5 can
                                                                be implemented
using a combination of low-pass (h) and high-pass (g) 1-D filters
                                                                    , as shown in
Figure 17.8. Using a similar approach, the corresponding synthe
                                                                   sis filter bank
is shown in Figure 17.9.
Nonstandard Compression Techniques                                         325




                                                          yll


                                                          y12




                                                          y2]


                                                          y22


                 - row
                <H     processingg -+4 ---
                   mVVPr0CeSSin               column -.
                                             미ocessing


       Figure 17.8     Analysis filter bank using row-column filtering.



              yll


              y12




              y21


              y22



       Figure 17.9     Synthesis filter bank using row-column filtering.



Ignoring the effects of coding and decoding on the input signal, we want the
synthesis filters h' and g' to cancel the aliasing effects of the interpolation.
Let h be an L-tap (L is even) finite impulse response (FIR) filter, then the
aliasing can be canceled if h and g form a quadratic minor filter (QMF) pair.
By definition, 九 and g 如rm a（가'IF pair 汗 in the time d이nain

                        g(n)    =   (- 1Y"1h(L- 1- n),

 and in the frequency domain

                               IH(w）尸 늬G（미尸 = 1.
 326                                                             CHAPTER 17




 The corresponding synthesis filters are then given by

                            /2'（미 = 九（乙 - 1 - n)                          (17.9a)
                            叭미 = g(1』小 1- n)                              (17.9b)
 There are many filters that can satisfy the above conditions. In a prac-
 tical implementation we want the filters to have good frequency sepa-
 ration and as few taps as possible. Johnston's QMF filters are used
 quite often in the literature. Johnston's eight-tap QMF filter is given by
 h(n) = {0.00938715, -0.07065183, 0.06942827, 0.48998080, 0.48998080,
 0.06942827, -0.07065183, 0.00938715}.



17.3.2    Subband Coding and Wavelets

A case of particular interest in subband coding is the implementation of the
subband filters using wavelets. Wavelets are families of functions that are
generated from a single function using dilations and translations. They have
been proven to be a useful tool in many different fields, including image
coding. For example, wavelet based coders have been applied successfully for
the compression of still-images and video at very low rates and are now being
proposed for consideration for the MPEG-4 standard.

For discrete signals analysis, if aO > 1 and bO ；三 0 denote the dilation and
translation steps respectively, given a basis (or "mother") wavelet function
砂(t), the family of wavelets of interest is represented by
                        心mn(t) = a,
                                  ,띠知何，까- nhO).                          (17.10)
                                                                         07  l0)
For aO = 2 and bO = 1 one can find mother wavelets so that 砂mn(t) constitute
an orthonormal basis, which allows a given signal f (t) to have a wavelet
decomposition given by

                           f(t) =二二Cm小m),                                (17.11)
                                   7n   n

where
                                                                         (17.12)
                            蜘=
                                   ff
                                        (t)   mn   (t)
                                                         dt.

In intuitive terms, the decomposition of a signal using orthonormal wavelets
yields. a representation/ that lies in-between the spatial and the Fourier repre-
sentations.
Nonstandard Compression Techniques                                              327




Wavelet analysis is also related to multiresolution representation. Under that
context, one can consider that the ae, m term of a wavelet function corresponds
to magnification and that the nbO term corresponds to location. If a, = 2, then
the analysis of a signal is performed octave by octave. In that case, given a
fixed magnification (or scale) m, one can find a "mother" scaling function中(t)
such that the family of functions

                         砂，nn(t) = 才m/2中（丁까 - n)                             (17.13)

forms an orthonormal basis. If fm(t) denotes the value of f (t) at resolution
level m, then fm(t) can be expressed as

                                                                             (17.14)
          凡(t) = ＞二d(m+l).中（m+1)n + ＞二C(m+1).砂（m+1)n
                    n                                    n


In other words, if 砂(t) is considered a low-pass function, and the wavelet
砂(t) is considered a band-pass function, then at a given resolution level m the
function can be expressed as the sum of low and high frequency components.

In 1989, Mallat showed that this multiresolution representation of a signal can
be computed using a pyramidal filter structure of QMF filter pairs, as shown
in Figure 17.10. The filters h and g form again a QMF pair and are related to




                                  H              h                                     J

                         깬 H
                           시H
                            아
                h
                                                                                        /
                                                                                       H



      f(t) +
                                  hdH>
                                                 g                                      +
                g           .->
                                          c1,n




     Figure 17.10 Filter bank for wavelet-based signal decomposition.


the scaling and wavelet functions as follows

                                令（2미 = 月（口)）令（a7),                           (17.15)
                                                                             (17.16)
                                山   (w)
                                                 =   G
                                                         （回）
                                                               西
                                                                   （블）
                                                                         ,



where 令(w) and 山(w) are the Fourier transforms of 中(t) and 砂 (t). As an
example, using the Daubechies 如ur-tap wavelet, h（미 = ｛誌 券 晶小읖｝
328                                                            CHAPTER 17




and g（미 = ｛蟲 券H쀼 拗． In the synthesis band, h'（미 = 九（3 小 n) and
g' (n) = g(3 - n).

The above wavelet decomposition of one-dimensional signals can be general-
ized for 2-D signals. Using row-column filtering, a 2-D wavelet decomposition
of an image can be computed using the filter structure of Figure 17.8. The
2-D wavelet decomposition can be interpreted as an image decomposition in
a set of independent spatially oriented frequency representations: horizontal,
vertical, and diag에al. For a four-band wavelet decomposition, the four output
bands in Figure 17.5(b) can be interpreted as follows. Band 1,1 corresponds to
the lower horizontal and vertical frequencies of the image, band 2,1 gives the
vertical high frequencies and horizontal low frequencies (horizontal edges),
band 1,2 gives the vertical edges, and band 2,2 gives the high frequencies in
both 小recti에s (corners).

Figure 17.11 shows the wavelet decomposition of an image into seven
subbands. After the original image was divided into four bands, the lower
subband was further subdivided into four bands. The h and g filters are the
seven-tap QMF filters with h(n) = {O.00525, -0.05178, -0.25525, 0.60355,
-0.25525, -0.05178, 0.00525} and g(n) = {-0.00525, -0.05178, 0.25525,
0.60355, 0.25525, -0.05 178, -0.00525}.

In summary, from an implementation viewpoint, wavelet decomposition can
be considered as a special case of subband filtering. In a subband coder,
compression efficiency and overall performance depend not only on the
choice of the analysis/synthesis filters but also on the compression method
that will be used on the subband filtered data. Similar considerations apply to
image and video compression methods based on wavelet decompositions.



17.3.3   Computational Requirements for Subband Filtering

The computational requirements of a subband coder may vary widely, depend-
ing on the complexity of the filter bank (number of bands, filter types, and so
on) and the complexity of the coder (such as VQ, DPCM, and Huffman). As an
example, we estimate the number of multiply-accumulate (MAC) operations
in a filter bank where all filters are L-tap FIR filters.
Nonstandard Compression Techniques                                                329




     Figure , 17.11 Example of wavelet decomposition into seven
     suooanas.



Consider an M x N image and the subband filter shown in Figure 17.8. In
the first stage, each of the two filters requires 푤트 MAC operations per row of
data for a total of NML MAC operations for the whole image. The second
stage has twice as many filters; however, the columns are also half as many.
Hence, the number of operations remain the same and the total number of
MAC operations for a four band 2-D filter is 2MNL or 2L operations per
pixel. Assuming we iterate this scheme on the lower band, the number of
MAC operations is still 2L per pixel; however, the input image at this stage has
one-fourth of the pixels in the original image. Hence, for multiple iterations,
 the total nun也er of 入4AC 아氾rations is bounded by

                                     l 玉
                                                                   .     8MNL
                                           l
              tai = 2NML(1 +
          MACt。                                    十               } <    八
                                                                                (17.17)
                                                                          3
                                                       ·   ·   4


                                               示
                                                                   "
330                                                             CHAPTER 17




For example, if L = 6, then the total number of MAC operations is bounded
by 16 operations per pixel. In comparison, in the 8 x 8 fast DCT, the
number of operations can be less than seven operations/pixel. The number of
multiplications can be reduced if the filter coefficients are powers of two or if
the filters are symmetric. When ii is symmetric, g(ri) = (-1)"1i(n). Therefore,
a multiplication with a filter coefficient needs to be performed only once,
and the product can be added or subtracted to the appropriate partial sum of
products.




17.4 VIDEO CODING SCHEMES FOR THE
     DESKTOP
One of the first commercially available techniques for the compression and
storage of digital video is Intel's DVI(Digital Video Interleaved). DVI has two
formats: real-time video (DVI-RTV)and production-level video (DVI-PLV).
Both DVI-RTV and DVI-PLV are based on image color subsampling and
vector quantization. RGB images are first divided into 4 x 4 blocks and
are translated into the YUV color space. The U and V components are then
subsampled by a factor of two in each direction, and the original 24 bits/pixel
image is now compressed down to 9 bits/pixel. The subsampled YUV data are
then further compressed to I to 2 bits/pixel using VQ followed by a lossless
coder.

DVI-RTV operates typically on 128 x 120 pixel images and uses only
intraframe coding. These images are usually scaled up to 256 x 240 during
display. DVI-PLV uses some form of interframe coding and may operate
on larger images (typically 256 x 240 pixels which are scaled up to 512 x
480 during display). DVI processing may be accelerated using Intel's i750
processor.

Indeo is another video coding scheme from Intel. It is based on color
subsampling, pixel differentiation, run-length coding, VQ,and lossless coding.
A typical compression ratio from Indeo is II: I. Using frame sizes of 320 x
240 pixels, Indeo allows software playback on PCs at 15 fps.

In 1991, Apple Computer introduced QuickTime. This is a multimedia
extension to the Macintosh operating system and allows for the manipulation
Nonstandard Compression Techniques                                        331




of dynamic data types, such as sound, video, and animation. QuickTime
supports a variety of compression schemes, including JPEG and a proprietary
(VQ based) algorithm from SuperMac Technology. SuperMac later introduced
Cinepak, a QuickTime compatible algorithm that supports software-only
decompression of 320 x 240 pixels at 15 fps.

Within a year, Apple introduced QuickTime for Windows and Microsoft
introduced Video for Windows. Video for Windows supports both Intel's
Indeo and the Motive algorithm from Media Vision. The Motive algorithm
uses a combination of run-length coding and vector quantization and can be
accelerated using Media Vision's chip set: the MVV2SI image-capture IC and
the MVV35l compression IC.

Wavelets have been used in compression schemes offered by Media Vision
(the Captain Crunch algorithm) and Aware Inc.

An야he叩야川缸 너deo co呻ression sche毗 ism애에－JPEG (M-JPEG). 山der
M-JPEG, each frame of the video is compressed independently using the
standard JPEG algorithm. Real-time compression and decompression is
possible using low-cost video boards with any of the commercially available
JPEG processing ICs. However, there is no standard syntax for M-JPEG coded
streams, and encoded data may not be able to be decoded across different
미atforms.

Table 17.2 summarizes the main coding schemes currently available for
desktop multimedia applications. The column under S/W indicates if software
playback is possible at the given rate, and the WV method denotes a wavelets
based coder.




17.5     TO PROBE FURTHER
Vector quantization for signal compression was first popularized in the 1980s
by Gersho and Gray. Their textbook [57] describes the fundamentals of VQ
theory and various codebook design and search techniques.

 A multiprocessor implementation of a VQ coder is described in [39]. It consists
 of a linear array of multiplier-accumulator ICs terminated by a next-address-
 332                                                           CHAPTER 17




                 Coder           Method      Frame Rate/s      S八V
           DVI-RTV                  VQ       256 x 240@ 15     No
           DVI-PLV                  VQ      引2 )< 480@30       No
           Indeo                    VQ      320 x 240@ 15      Yes
           QuickTime                VQ       160x 120@ 15      Yes
           Cinep出（                  VQ      320 )< 240@ 巧      Yes
           Video for Windows        VQ      160x I20@ 12       Yes
           M-JPEG                  DCT      640 x 480@30       No
                                            (60 fields/s)
           Captain Crunch          WV       320 x 240@30       No
           VideoCube               砥八／      640 x 480@30       No
                                            (60 fields/s)

                  Table 17.2   Video coders for the desktop.



selector processor. A single-chip VQ encoder for pruned tree search was
presented in [129]. This 80-MOPS chip c帥 compute one eight-dimensional
inner product in four clock cycles. The pipelined architecture of the TSVQ
encoder was first introduced by Kolagotla et at. in [105]. A low-power
implementation of the same design is also described in [121]. Another
hardware implementation of a very low-power VQ decoder for real-time
decompression on a portable terminal is presented in [26].

Subband coding was first introduced in 1976 for the efficient coding of speech
signals. Woods and O'Neil [197] were among the first to combine subband
filtering and a DPCM coder for compressing images. A good overview of
wavelet theory and its application to signal processing is given by Rioul and
Vetterli [171]. Mallat [131] was the first to show the relationship between
subband filtering and wavelet decomposition. The book on multiresolution and
signal decomposition by Akansu and Haddad [3] provides a unified coverage
of subband filtering and wavelet transforms and many examples on filter
design for image coding.

There is a variety of wavelet-based coders. In [120], Lewis and Knowles
use the four-tap Daubechies wavelets and a quantization model based on the
human visual system. The subband-filtering operation for this system can
easily be implemented using a multiplier-free architecture [119]. A coding
Nonstandard Compression Techniques                                        333




scheme that combines wavelet decomposition and VQ is described in [8]. In
[119], Lewis et al. describe a low-bit video coder using wavelet transforms
and differential coding. Another architecture for a low-power subband video
decoder using 4-tap wavelet-based filters is described in [63]. At 20 MHz, the
chip can process 10 million color pixels per second while dissipating only 16
mW. A single IC can process images up to 352 pixels wide and performs both
subband decoding and YUV to RGB color transfor伍tions.

Trade magazines are a good source of information for commercially available
video coders. Most of the information on video coders for the desktop appeared
first in various articles in Newmedia [41] and EDN [164]. Intel's i750 system
includes two ICs: the 82750PB pixel processor and the 82750DB display
processor. Both processors are described in [132]. A general overview of
QuickTime is given in [73].
                                                                  A
  ABBREVIATIONS AND SYMBOLS




[xl The smallest integer larger or equal to x.

[xj The largest integer smaller or equal to x.

1-D One-dimensional.

2-D Two-dimensional.

4:2:0 A color subsampling format in which the chrominance components are
    subsampled by a factor of two in both dimensions. Example: If Y is 720
     x 480, then Cb andCr are 360 x 240.

4:2:0 macroblock A 4:2:0 macroblock has four 8 x 8 blocks of luminance
    and two 8 x 8 blocks of chrominance. For example, a 4:2:0 YCbCr
    macroblock has four blocks of Y, one block of Cb, and one block of Cr.

4:2:2 A color subsampling format in which the chrominance components are
    subsampled by a factor of two in the horizontal only dimension. Example:
    If Y is 720 x 480, then Cb and Cr 刻e 360 x 480.

AC component of the DCT Any component of the DCT output except the
   (0,0) (or DC) component.

ADPCM Adaptive differential pulse code modulation.

AGU Address generation unit.

ALU Arithmetic and logic unit.

ANSI American National Standards Institute.
 336                                                         APPENDIX A




 CAM Content-addressable memo口.

 CCIR The International Radio Consultative Committee of the International
    Telecommunications Union (now ITU-R).

 CCIR 601 CCIR recommendation 601 is a specification for digital TV. A
    CCIR 601 image is defined as 720 pixels x 480 lines at 60-Hz interlaced
    (NTSC) or 720 pixels x 576 lines at 50-Hz interlaced (PAL). This
    recommendation is now called ITU-R Recommendation BT.601-4.

CCITT The telecommunication stand町dization sector of the ITU. It is now
   called ITU-T.

CD Compact disc.

CELP Code excited linear prediction.

CISC Complex instruction set computer.

CIF Common intermediate format. In a YCbCr CIF frame, Y is 352 pixels x
   288 lines, and Cb and Cr are 176 pixels x 144 lines.

CPU Central processing unit.

DC component of the DCT The (0,0) component of the DCT output.

DCT, LDCT Discrete cosine transform or inverse discrete cosine transform.

DFT Discrete Fourier transform.

DHT Discrete Hadamard transform.

DMA Direct memory access.

DST Discrete sine transform.

DPCM Differential pulse code modulation.

dpi Dots per inch.

DSP Digital signal processing or digital signal processor.

DVI Digital video interleave.

DVI-PLV DVI production-level video.

DVI-RTV DVI real-time video.
사力revk汀ions and Sy／刃b可S                                             337




EOB End of block.

FFT Fast Fourier transform.

fps Frames per second.

FSM Finite state machine.

GOB Group of blocks.

GOP Group of pictures.

GOPS Giga operations per second. Same as billion operations per second
   (BOPS).

HDTV High-definition TV. Several formats have been chosen for HDTV. For
  instance, MPEG-2 considers two HDTV formats, namely, 1440 pixels x
   1152 lines and 1920 pixels x 1152 lines.

HVS Human visual system.

I/O Input--output.

IC Integrated circuit.

ISDN Integrated services digital network.

ISO International Organization for Standardisation.

ISO/LEC The international Electrotechnical Commission of the ISO.

ITU International Telecommunications Union.

ITU-T The telecommunication standardization sector of ITU, formerly the
     ccrvr.
JBIG Joint Binary Image Experts Group.

 JFIF JPEG file interchange format.

 JPEG Joint Photographic Experts Group.

 KLT Karhunen--Loeve transform.

 MAC Multiply--accumulate.

 MAD Mean absolute difference. Same as MAE.
 338                                                        APPENDIX A




 MAE Mean absolute error.

 MCU Minimum coded unit.

 MOPS Million operations per second.

 MPEG Moving Pictures Expert Group.

 mux Multiplexor.

NTSC A 525-line, 60-Hz television system developed by the National Tele-
   vision Systems Committee of the USA. NTSC is used in North America
   and Japan.

PAL A 625-line, 50-Hz television system developed in Germany. NTSC,
   PAL, and SECAM (from France) are the three main television transmission
   systems in the world.

PCM Pulse code modulation.

PHODS Parallel hierarchical one-dimensional search.

PLA Programmable logic array.

PSNR Peak signal-to-noise ratio.

Px64 Another name for the H.261 video teleconferencing standard.

QCIF Quarter CIF. A QCIF image is defined as 176 pixels x 144 lines.

QMF Quadrature mirror filter.

RAC ROM accumulator.

RISC Reduced instruction set computer.

RLC Run-length coder.

SIF Source input format. In a SW image the luminance component is defined
    as 352 pixels x 240 lines at 30 Hz or 352 pixels x 288 lines at 25 Hz.

SIMD Single input multiple data.

SNR 罰gn키如-n이se ratio.

SPIFF The still-picture interchange file format.
사力revi玎ions口ndSymbols                                                339




TI Texas Instruments.

TLB Translation look-aside buffer.

TSS Three-step-search.
TSVQ Tre已se缸ch ye아야 quantization.

VLC Variable length coder.
VLI Variable length integer.

VLIW Very large instruction word.

VLSI Very large scale integration.

VQ Vector quantization.
YCbCr A color coordinate system used for the transmission and storage of
   image and video signals. Given the primary RGB inputs (R,G, and B in
   [0,1]),
                      Y  = 0.299(R - G) + G + 0.114(B - G),
                      Gb = 0.564(B -y) ,
                      Cr     = 0.713(R - Y).

    Alternatively,


                                                              RGB
                I " 1   I 0.299   0.587  0.114 1 1
                1Cb 1 = 1 -0.169 -0.331  0.500 I 1
                L Cr J  L 0.500 -0.419  -0.081 J L

YUV A color coordinate system used in the PAL TV system. Given the
   primary RGB inputs (R,G, and B in [0,1]),
                      Y      = 0.299(R - G) + G + 0.114(B - G),

                       D V
                             = 0.493(B - y)1
                             = 0.877(R - Y).

     Alternatively,
                 I ' 1  f 0.299   0.587            0.11441 r R 1
                 1U I = 1 -0.148 -0.289            0.437 I I G 1 ·
                 L. V J [. 0.615 -0.515           -0.100 J L B J
                                                                      B
                         INTERNET DIRECTORY




The Internet is a rich source of materials on the image and video corn-
pression standards and their implementation. One can find standards doc-
uments, literature, and software implementations. Most of the discussions
on data compression take place in the news groups comp.compression and
comp.compression.research. A good start to a search for information is
the monthly posted FAQ in these newsgroups. This monthly posting pro-
vides answers to the most frequently asked questions (FAQ)  . You can find
this posting by searching for "comp.compression Frequently Asked Ques-
tions" in the subject lines. This posting is also available via anonymous
ftp from rtfm.mit.edu in the directory usenet/news.answers/-
compression-faq or from other archive sites, such as ftp.uu.net.

In this appendix we provide internet addresses for some of the sites where
literature and software implementations of the compression standards are
currently available. Internet sites are constantly changing,so be sure to consult
the latest "FAQ" postings for the most updated information.


1   ITU and ISO Documents.
     The ITU provides most of the ITU Recommendations in postscript
     format in gopher.itu.ch. You can access the ITU server using the
     command telnet gopher.itu.ch 2000. If you use a graphics-
     based internet browser, such as Mosaic or Netscape, the site location is
     gopher://gopher.itu.ch/. For document searches, it is always
     helpful to know the exact ITU number for a specific standard. For
     example, JPEG is T.81.
342                                                            APPENDIX B




      ISO also has a world-wide web site at
      http: //w사w. iso. ch1'welcorne.html .
      The site allows you to search for ISO documents and provides useful
      information on the ISO activities and ISO members.
      The documents for the proposed ITU-T H.324 standard that will enable
      real-time voice, data, and video over V.34 modems on the general switched
      telephone network (GSTN) can be obtained from the site ftp. std. corn
      and the relevant files are in /vendors/ PictureTel/ h324/. This
      directory contains tiles related to the draft version of the ITU-T H.324
      (formerly known as H.32P) protocol suite.
      If you do not have Internet access, the mailing addresses and telephone
      numbers for the international organizations are given below:

      ITU
      Palais des Nations
      CH-121 1
      Geneva 10, Switzerland
      Tel: (22) 730-5111,

      ISO
      1 Rue de Varembe
      Case Postale 56
      CH-121 I
      Geneva 20, Switzerland
      Tel: (22) 749-01 1 1.

      In the United States, standards documents are also available from the
      American National Standards Institute (ANSI):

      ANSI
      11 West 42nd St.
      New York, NY 10036
      Tel: (212) 642-4900.

      Sources for JPEG.
      Source code for a JPEG coder from the Independent JPEG Group is
      available from
/／玎ernet／가rect아V                                                             343




    ftp. uu.net: /graphics/ jpeg/
    (e.g., version 5 of the program is in the archive file jpegsrc.v5.tar.gz). For
    additional information contact jpeg- info@uunet . uu. net.
    Other sources for JPEG are available from Stanford University at
    havefun. stanford. edu : pub! jpeg.
    This version also supports lossless JPEG. Another program for lossless
    JPEG is available from Cornell University at
    ftp. cs. cornell. edu: /pub/ multimed/ ljpg. tar. Z.

.   Sources for 11.261.
    The IVS video conferencing system from the French research institute
    INRIA is available from
     zenon. inria. fr: !rodeo/ ivs/ last=version/ .
    This is X-windows based and runs on most Unix workstations. Another
    H.261 coder is available from Stanford University at
    havefun. stanford. edu :pub/p641.

.   Sources for MPEG.
    For MPEG-i, sources are available from Stanford University at
    havefun. stanford. edu: !pub/mpeg/
    and from the University of California Berkeley at
    s2k- ftp. cs.berkeley. edu: IpubIinu1timediaImpeg/.
    The Berkeley and Stanford sites include implentations for MPEG-I
    encoder and decoder.
    For Windows and Windows NT, a very fast MPEG player from Stephen
    Eckart is available from
    ftp. netcom. com: /pub/ cf! cfogg!mpeg!vmpegl2a. zip.
    For MPEG-2, the best place to look is
     ftp. netcom. com: /pub/ cf! cfogg!mpeg2/.
     It includes both an MPEG-2 encoder and an MPEG-2 decoder. The
     入玎下G그 encoder and decoder can also encode and decode 入4PEG-1
     bit streams. The software has been developed by the MPEG Software
     Simulation Grouo. which you can contact at MPEG-L@netcom. corn.
     This site also includes files with pointers to other locations where sources
344                                                          APPENDIX B




      or executables for image and video compression programs that are in the
      public-domain.
                                         REFERENCES



[1]
      CCIR Recommendation 601-1. Encoding parameters of digital televi-
      sion for studios.

[2] B. Ackland. The role of VLSI in multimedia. IEEE Journal of Solid-
    State Circuits, 29(4):381--388, April 1994.

[31 A.N. Akansu and R.A. Haddad. Multiresolution Signal Decomposition.
    Transforms, Subbands, and Wavelets. Academic Press, San Diego,
    CA., 1992.

[4]   T. Akiyama et a!. MPEG2 video codec using image compression DSP.
      IE万 가口nsactions on C아玎U刃ier Electronics, 3(40):466--472, Aug.
      1994.

[5] J.D. Allen and S.M. Blonstein. The multiply-free Chen transform - a
    rational approach to JPEG. In Picture Coding Symposium, Japan, pages
    237--240, 1991.

[6] S. Ammon and C. Erskine. Low-delay CELP speech compression and its
    implementation on a fixed-point DSP. DSP & Multimedia Technology,
    May 1994.

[7] P.H. Ang, P.A. Ruetz, and D. Auld. Video compression makes big
    gains. IEEE Spectrum, pages 16--19, Oct. 1991.

[8] M. Antonini, M. Barlaud, P. Mathieu, and I. Daubechies. Image
    coding using vector quantization in the wavelet transform domain. In
    Proceedings IEEE International Conference on Acoustics, Speech, and
    Signal Processing (ICASSP), pages 2297--2300, 1990.

[9] K. Aono et a!. A video digital signal processor with a vector-pipeline
    architecture. IEEE Journal Solid-State Circuits, 27(12):1886--1894,
    Dec. 1992.
346                               IMAGE COMPRESSION STANDARDS




[10] Y. Arai, T. Agui, and M. Nakajima. A fast DCT-SQ scheme for images.
     Transactions of the IEICE, E-7 1(1 1): 1095--1097, Nov. 1988.
[11] R.B. A叩s and T.K. Truong. Comparison of international standards for
     lossless still image compression. Proceedings of the IEEE, 82(6):889--
     899, June 1994.
[12] A. Artieri and O. Colavin. A chip set core for image compression. IEEE
     Transactions on Consumer Electronics, 36(3):395--402, August 1990.
[13] D. Auld. A flexible chip set for intra frame video compression. In
     Digest of Papers, COMCON, pages 330--332, 1991.
[14] D. Bailey et al. Programmable vision processor/controller for flexible
     implementation of current and future image compression standards.
     IEEE Micro, pages 33--39, Oct. 1992.
[15] A. Balkanski, S. Purcell, and J. Kirkpatrick. System for compression
     and decompression of video data using discrete cosine transform and
     coding techniques. U.S. Patent 5341318, Aug. 1994.
[16] l江A. Bayoumi. VI万／Sign口／竹ocessing T匕chn可ogy. Kiuwer Acade而c
     Publishers, Boston, 1994.
[17] T.C. Bell, J.G. Cleary, and I.H. Witten. Text Compression. Prentice
     Hall, Englewood Cliffs, New Jersey, 1990.
[18] T. Berger. Rate Distortion Theor " - A Mathematical Basis for Data
     Compression. Prentice-Hall, Englewood Cliffs, New Jersey, 1971.
[19] V. Bhaskaran, K. Konstantinides. and R. Lee. Real-time MPEG- l
     software decoding on HP workstations. In Proceedings !S& T/SPIE
     Symp. on Electronic Imaging, Vol. 2419, pages 466--473, Feb. 1995.
[20] H. Bheda and P. Srinivasan. A high-performance cross-platform MPEG
     decoder. In Proceedings SPIE, vol. 2187, pages 241--248, San Jose,
     CA, 1994.
[21] M. Bierling. Displacement estimation by hierarchical blockmatching. In
     SPIE Vol. 1001 Visual Communications and Image Processing, pages
     942--951, May 1988.
[22] M. Bolton et al. A complete single-chip implementation of the JPEG
     image compression standard. In Proceedings IEEE Custom Integrated
     Circuits Conference, pages 12.2.l--12.2.4, 1991.
REFERENCES                                                              347




 [23] D. Brinthaupt et al. A video decoder for H.261 video teleconferencing
      and MPEG stored interactive video applications. In Proceedings IEEE
      Internatk刀i口／Solid-State Circu加 Co可計enc巳 pages 34--35, 1993.

 [24] D. Bursky. MPEG silicon puts quality video on PCs. Electronic Design,
      Penton Publishing Inc., Oct. 14 1994.

 [25] M.D. Cam New video coding standard for the 1990s. Electronics and
      Communication Engineering Journal, pages 119--124, June 1990.

 [26] A. Chandrakasan, A. Burstein, and R.W. Brodersen. A low-power
      chipset for a portable multimedia I/O terminal. IEEE Journal of Solid-
      State Circuits, 29(12):1415--1428, Dec. 1994.

 [27] S-F. Chang and D.G. Messerschmitt. Designing high-throughput VLC
      decoder, Part I-concurrent VLSI architectures. IEEE Transactions on
      Circuits and Systems for Video Technology, 2(2): 187--I96, June 1992.

 [28] Chi-Fa Chen and K.K. Pang. Hybrid coders with motion compensation.
      Multidimensional Systems and Signal Processing, 3(I2):241-266, Dec.
      1992.

 [29] C.T. Chen and A. Wong. A self-governing rate buffer control strategy
      for pseudoconstant bit rate video coding. IEEE Transactions on Image
      Processing, 2(1):50--59, Jan. 1993.

 [30] L-G. Chen, W.T. Chen, Y.S. Jehng, and T.D. Chiueh. An efficient
      parallel motion estimation algorithm for digital image processing. IEEE
      Tr口ns口Ct加ns 아i Circuits and Syste刃is for Video T匕chno勿gy, 1(4):378-
      -385, Dec. 1991.

 [31] M-H Chen et al. VLSI implementation of single chip JPEG codec. In
      Proceedings International Symp. on VLSI Technology, Systems, and
      Applications, pages 189--I93, 1993.

 [32] W-H. Chen and C.H. Smith. Adaptive coding of monochrome and color
      images. IEEE Transactions on Communications, COM-25(I1):1285--
      1292, Nov. 1977.

 [33] L. Chiariglione. Development of multi-industry information technology
      standards. the MPEG case. In Proceedings International workshop on
      HDTV '93, Octob. 1993.
348                                 IMAGE COMPRESSION STANDARDS




 [34] N.I. Cho and S.U. Lee. Fast algorithm and implementation of 2-D
      discrete cosine transform. IEEE Transactions on Circuits and Systems,
      38(3):297--305, Mar. 1991.

 [35] O. Colavin, A. Artieri, J-F. Naviner, and R. Pacalet. A dedicated circuit
      for real-time motion estimation. In Proceedings Euro ASIC '91, Paris,
      France, pages 96--99, 1991.
[36] S. Cucchi and M. Fratti. A novel architecture for VLSI implementation
     of the 2-D DCTIIDCT. In Proceedings ICASSP, pages V--693--V--696.
     IEEE, 1992.

[37] R.L. de Queiroz and K.R. Rao. Human visual sensitivity- weighted
     progressive image transmission using the lapped orthogonal transform.
     Journal of Electronic Imaging, 1(3):328--338, July 1992.

[38] Y.F. Dehery, M. Lever, and P. Urcun. A MUSICAM source codec
     for digital audio broadcasting and storage. In Proceedings IEEE
     International Conference on Acoustics, Speech, and Signal Processing
     (JCASSP), pages 3605--3608. IEEE, 1991.

[39] R. Dianysian and R.L. Baker. A VLSI chip set for real time vector
     quantization of image sequences. In Proceedings IEEE International
     Symposium on Circuits and Systems (ISCAS), pages 221--224, 1987.
[40] W. Ding and B. Liu. Rate-quantization modelling for rate control of
     MPEG video coding and recording. In Proceedings SPIE Vol. 2419,
     pages 139--iS0, Feb. 1995.
[41] B. Doyle. Crunch time for digital video. Newmedia, pages 47--S0,
     March 1994.
[42] S. Eckart. High performance software MPEG video player for PCs. In
     Proceedings SPIE, vol. 2419, pages 446--454, San Jose, CA, 1995.

[43] S. Eckhart and C. Fogg. ISO/IEC MPEG-2 software video codec. In
     Proceedings SPIE, volume 2419, pages 100--109, Feb. 1995.
[44] D.F. Elliot and K.R. Rao. Fast Tr口n町or刃is - Algorith刀玎， An끄yses,
     Applications. Academic Press, New York, 1982.
[45] T. Enomoto and M. Yamashina. Video signal processor (VSP) ULSIs
     for video data coding. In Proceedings VLSI Technology, Systems, and
     Applications, pages 184--188, 1993.
REFERENCES                                                               349




[46] E. Feig and S. Winograd. Fast algorithms for the discrete cosine
     transform. IE1万 Tr口nsact加 on＆帥a! Processi似，40（아기74-－기93'
     Sept. 1992.

[47] R.D. Feliman, R.T. Kaneshiro, and K. Konstantinides. Design and
     evaluation of an architecture for a digital signal processor for instru-
     mentation applications. IEEE Transactions on ASSP, 38(3):537--546,
     March 1990.

[48] E.D. Frimout, J. Biemond, and R.L. Lagendijk. Forward rate control for
     MPEG recording. In SPIE Visual Commun. Image Processing, pages
     184--194, May 1993.

[49] H. Fujiwara et at. An all-ASIC implementation of a low bit-rate
     video codec. IEEE Transactions on Circuits and Systems for Video
     Technology, 2(2):123--134, June 1992.

[50] ITU-T Recommendation G.722. 7 kHz audio-c어ing within 64 kbit/s.

[51] CCITT Recommendation G.726. 40, 32, 24, 16 kbit/s adaptive differ-
     ential pulse c어e modulation (ADPCM), 199O.

[52] CdT!' Recommendation G.728. Coding of speech at 16 kbit/s using
     low-delay code excited linear prediction, Sept. 1992.

[53] D. Galbi et al. An MPEG-i audio/video decoder with run-length corn-
     pressed antialiased video overlays. In Proceedings IEEE International
     助妃-Ste町e Circu而 Con肛ence, pages 286--287, Feb. 1995.

[54] D. Le Gall. 入PEG: A video compression standard for multimedia
     applications. Communications of the ACM, 34(4), April 1991.

[55] R.G. Gallager. Information Theory and Reliable Communication. John
     Wiley and Sons, NewYork, 1968.

[56] R.G. Gallager. Variations on a theme by Huffman. IEEE Transactions
     on／可切7nati아i 刀ieory, 24(6):668--674, Nov. 1978.

[57] A. Gersho and R.M. Gray. Vector Quantization and Signal Compres-
     sion. Kiuwer Academic Publishers, Boston, 1992.

[58] M. Ghanbari. The cross-search algorithm for motion-estimation. IEEE
     Transactions on Communications, 38(7):950--953, July 1990.
350                               IMAGE COMPRESSION STANDARDS




 [59] H. Gharavi and卜Vt. 卜느4i11s. 미ockmatchi雎 蜘tion es帥ation 毗orithms
      - new results. 旭EET／   口ns配加ns on Circuits 口nd System옥 37(5):649--
      651, May 1990.

 [60] B. Girod. The efficiency of motion-compensating prediction for hybrid
      coding of video sequences. IEEE Journal on Selected Articles in
      Communications, SAC-5(7):I 140--I 154, Aug. 1987.

[61] B. Girod. Motion-compensating prediction with fractional-pel accuracy.
     IEEE Transactions on Communications, 41(4):604--612, Apr. 1993.

[62] C.A. Gonzales and E. Viscito. Motion video adaptive quantization in
     the transform domain. IEEE Transactions on Circuits and Systems for
     Video Technology, 1(4):374--378, Dec. 1991.

[63] B.M. Gordon and T.H.Y. Meng. A low power subband video decoder
     architecture. In Proceedings IEEE International Conference on Acous-
     tics, Speech, and Signal Processing (ICASSP), pages II--409--412,
     1994.

[64] D. Greenley et al. UltraSPARC: the next generation superscalar 64-bit
     SPARC. In Digest of Papers COMPCONSpring 1995, pages 442--451.
     IEEE, March 1995.

[65] K. Guttag, R.J. Gove, and J.R. Van Aken. A single-chip multiprocessor
     的r 毗岫nedia: the l뇨4VP. lEE万（勿mputer Gr口p厄Cs 口nd App／蜘加ns,
     12(6):53--64, November 1992.

[66] 1TU-T Recommendation H.26 1. Line transmission of non-telephone
     signals. Video codec for audiovisual services at p x 64 kbits, March
     1993.

[67] ITU-T Recommendation H.320. Line transmission of non-telephone
     signals. Narrow-band visual telephone systems and terminal equipment,
     03/93.

[68] E. Hamilton. JPEG file interchange format, Version 1.02. C-Cube
     Microsystems, Literature Department, Sept. 1992.

[69] M. Harrand et al. A single chip videophone video encoder/decoder. In
     Proceedi섕s IEEEI,吐라na加nalS可江訊加 C沇岫sCo蜘rence, pages
     292--293, Feb. 1995.
REFERENCES                                                               351




 [70] R. Hashemian. Design and hardware implementation of a memory effi-
      cient Huffman decoding. IEEE Transactions on Consumer Electronics,
      40(3):345--352, Aug. 1994.

 [71] J. Hennessy, N. Jouppi, F. Baskett, and J. Gill. MIPS: A VLSI processor
      architecture. In Proceedings CMU Conference on VLSi Systems and
      Computations, pages 337--346, Pittsburgh, PA, 1981.

 [12] K. Herrmann et a!. Architecture and VLSI implementation of a RISC
      core for a monolithic video signal processor. In J. Rabaey, P.M. Chau,
      and J. Eldon, editors, VLSI Signal Processing VII, pages 368--377.
      IEEE, New York, 1994.

 f73] E. Hoffert et al. QuickTime: an extensible standard for digital multime-
      dia. In Digest of Papers COMPCON Spring 1992, pages 15--20, Feb.
      1992.

 [74] R. Hopkins. Digital terrestrial HDTV for North America: the Grand
      Alliance HDTV system. IEEE Transactions on Consumer Electronics,
      40(3):185--198, Aug. 1994.

 [75] P.G. Howard and J.S. Vitter. Arithmetic coding for data compression.
      Proceedings of the IEEE, 82(6):857--865, June 1994.

 (76] C-H. Hsieh and T-P. Lin. VLSI architecture for block-matching motion
      estimation algorithm. IEEE Transactions on Circuits and Systems for
      Video Technology, 2(2):169--175, June 1992.

 177] D.A. Huffman. A method for the construction of minimum-redundancy
      codes. Proceedings institute of Electrical and Radio Engineers,
      40(9):1098--1101, Sept. 1952.

 [78] R. Hunter and A.H. Robinson. International digital facsimile coding
      standards. Proceedings of the IEEE, 68(7):854--867, Jul. 1980.

 [79] G. Hutson, P. Shepherd, and J. Brice. Colour Television. System
      Principles, Engineering Practice, and Applied Technology. McGraw-
      Hill, London, second edition, 1990.

 [80] T. Inoue et al. A 300 MHz 16b BiCMOS video signal processor. In
      Proceedings IEEE International Solid-State Circuits Conference, pages
      36--37, 1993.
352                                 IMAGE COMPRESSION STANDARDS




 [81] International Telegraph and Telephone Consulative Committee. Stan-
      dardization of Group 3 facsimile apparatus for document transmission,
      Recommendation T.4. ISO, 1980.

 [821 International Telegraph and Telephone Consulative Committee. Facsim-
      ile coding schemes and coding control functions for Group 4 facsimile
      apparatus, Recommendation T.6. ISO, 1984.

[83] ISO1IEC JTC1 CD 10918. Digital compression and coding of
     continuous-tone still images - part 1: Requirements and guidelines.
     Iso, 1993.

[84] ISO/IEC JTCI CD 11172. Coding of moving pictures and associ-
     ated audio for digital storage media up to 1.5 Mbits/s. International
     Organization for Standardization (ISO), 1992.

[85] ISOfIEC JTC1 CD 1 1544. Coded representation of picture and audio
     information - progressive bi-level image compression. ISO, 1993.

[86] ISOII兀 JTCI CD 13818. Generic coding of moving pictures and
     associated audio. International Organization for Standardization (ISO),
     1994.

[87] ISOfIEC JTCI/SC29IWGI 1/N0400. Test model 5: version 2. ISO,
     1993.

[88] ITU (Q.5/8 Rapporteur). Amendments to ITU-T Rec. T.30 for enabling
     continuous-tone colour and grayscale mode for Group 3, COM 8-43-E.

[89] ITU (Q.5/8 Rapporteur). Amendments to ITU-T Rec. T.4 to enable
     continuous-tone colour and grayscale mode for Group 3, COM 8-44-E.
[90] J.R. Jamn and A.K. Jamn. Displacement measurement and its application in
     interfr카ie coding. 旭月ETr口nsac加ns on C毗unica加ns, 29(12):1799-
     -1808, Dec. 1981.

[91] Y. Jang et al. A 0.8p 100-MHz 2-D DCT core processor. IEEE
     Transactions on Consumer Electronics, 40(3):703--710, August 1994.

[92] N. Jayant. Signal compression: Technology targets and research
     directions. JE万E Journ口／ on Selec肥d Articles in Corn刃iunic玎勿ns,
     10(5):796--818, June 1992.
REFERENCES                                                              353




 [93] N.S. Jayant and P. Noll. I기git口／（勿ding 可 Wave和nfl옥 尸rinc巾／es 口nd
      Applications to Speech and Video. Prentice-Hall, Englewood Cliffs,
      New Jersey, 1984.

 [94] Y-S. Jehng, L-G. Chen, and T-D. Chiueh. A motion estimator for low
      bit-rate codec. IEEE Transactions on Consumer Electronics, 38(2):60-
      -69, May 1992.

 [95] J. Jeong and W. Ahn. Subpixel accuracy motion estimation using a
      model for motion-compensated errors. In Picture coding symposium,
      乙usanne, Switzerland, pages 13.4--13.6, 1993.

 [96] R.A. Vander Kam, P.W. Wong, and R.M. Gray. JPEG compression for
      a grayscale printing pipeline. In Proceedings SPIE Vol. 2418, pages
      229--240, Feb. 1995.

 [97] F.A. Kamangar and K.R. Rao. Fast algorithms for the 2-D discrete cosine
      transform. IEEE Transactions On Computers, C-31(9):899--906, Sept.
      1982.

 [98] S. Kappagantula and K.R. Rao. Motion compensated interframe image
      predict幻n. IEEET／ 口ns口Ct加ns on Communic口ti아玎，33(9):1011--1015,
      Sept. 1985.

 [99] G. Keesman, I. Shah, and R.K. Gunnewiek. Bit-rate control for MPEG
      encoders. Signal Processing: Image Communication, 6(1):545--560,
      March 1995.

[100] J.C. Kieffer. Strong converses in source coding relative to a fidelity
      criterion. IEEE Transactions on Information Theory, IT-37(2):697--
      707, 1991.

[101] D. Kim et al. A real-time MPEG encoder using a programmable
      processor. iEEE Transactions on Consumer Electronics, 40(2):161--
      170, May 1994.

[102] P. Knebel et al. HP's PA7100LC: A low-cost superscalar PA-RISC
      processor. In Digest of Papers COMPCON Spring 1993, pages 441--
      447. IEEE, Feb. 1993.

[103] U. Ko et al. DSP core with parallel module testability. In IEEE ASIC
      '89: 2nd Annual Seminar, pages P6--3.1 -- P6--3.5, 1989.
354                                IMAGE COMPRESSION STANDARDS




[104] L. Kohn et at. The visual inst기ction set (VIS) in UltraSPARC. In
      Digest of Papers COMPCON Spring 1995, pages 462--469. IEEE,
      March 1995.

[105] R.K. Kolagotla, S-S Yu, and J.F. JaJ . VLSI implementation of a tree
      searched vector quantizer. IEEE Transactions on Signal Processing,
      41(2):901--905, Feb. 1993.

[1061 T. Komarek and P. Pirsch. Array architectures for block matching
      algorithms. IEEE Transactions on Circuits and Systems, 36(10):1301--
      1308, October 1989.

[107] K. Konstantinides. Fast subband filtering in MPEG audio coding. IEEE
      Signal Processing Letters, l (2):26--28, Feb. 1994.

[108] Jan L.P. De Lameillieure. A heuristic algorithm for the construction of
      a code with limited word length. IEEE Transactions on Information
      Theory, 33(5):438--443, July 1988.

[1091 Jan L.P. De Lameillieure and I. Bruyland. Comment on algorithm
      for construction of variable length code with limited maximum word
      length. IEEE Transacti아玎 onC이nmunic口玎ons, 34(12):893小894, Dec.
      1986.

[1101 L.L. Larmore and D.S. Hirschberg. A fast algorithm for optimal length-
      limited Huffman codes. Journal of the Association for Computing
      Machinery JACM, 37(3):464--473, July 1990.

[111] B.G. Lee. A new algorithm to compute the discrete cosine transform.
      IEEE Transactions on ASSP, ASSP-32(6):1243--45, Dec. 1984.

[112] D.T. Lee. JPEG: New enhancements and future prospects. In Proceed-
      ings IS&T48-th Annual Conference, pages 58--62, May 1995.

[113] J.C. Lee, E. Cheval, and J. Gergen. The Motorola 16-bit DSP ASIC
      core. In IEEE Proceedings of ICASSP, pages 973--976, 1990.
[114] J.H. Lee, M.K. Doh, and C.W. Lee. A VLSI chip for motion estima-
      tion of HDTV signals. IEEE Transactions on Consumer Electronics,
      40(2):154--160, May 1994.

[115] L-W. 此, J.F. Wang, J.Y. Lee, and J.D. Shie. Dynamic search window
      adjustment and interlaced search for block-matching algorithm. IEEE
      Transactions on Circuits and Systems, 3(1):85--87, Feb. 1993.
REFERENCES                                                               355




[116] R.B. Lee. Realtime MPEG video via software decompression on a
      PA-RISC processor. In Digest of Papers COMPCON Spring 1995,
      pages 186--192, March 1995.
[117] S-M. Lei and M-T. Sun. An entropy coding system for digital HDTV
      applications. IEEE Transactions on Circuits and Systems for Video
      Technology, 1(1):147--155, March 1991.
[118] M. Levy and J.P. Leonard. EDN's DSP-chip directory. EDN, 40(10):40-
      -95, May 11 1995.
[119] A.S. Lewis and G. Knowles. VLSI architecture for 2-D Daubechies
      wavelet transform without multipliers. Electronic Letters, 27(2):171--
      173, Jan. 1991.

[120] A.S. Lewis and G. Knowles. Image compression using the 2-D wavelet
      transform. IEEE Transactions on Image Processing, 1(2):244--250,
      April 1992.
[121] D.B. Lidsky and J.M. Rabaey. Low power design of memory intensive
      functions. case study: vector quantization. In J. Rabaey, P.M. Chau, and
      J. Eldon, editors, VLSI Signal Processing VI!, pages 378--387. IEEE,
      New York, 1994.
[122] E. Linzer and E. Feig. New DCT and scaled-DCT algorithms for
      fused multiply/add architectures. In Proceedings IEEE Intern玎ional
      Conference on Acoustics, Speech, and Signal Processing (ICASSP),
      pages 80--91, 1991.
[123] B. Liu and A. Zaccarin. New fast algorithms for the estimation of
      block motion vectors. IEEE Transactions on Circuits and Systems,
      3(2):148--157, Apr. 1993.
[124] H. Lohscheller. A subjectively adapted image communication sys-
      tern. IEEE Tran요兀ti아玎 onC아nmunications, C（가뇨4-32(12):1316小1322,
      Dec. 1984.
[125] H. Lohscheller and U. Franke. Colour picture coding - algorithm
      optimization and technical realization. Frequenz, 41:291--299, 11/12
      1987.
[126] C.H. Lu. Comment on algorithm for construction of variable length
      code with limited maximum word length. IEEE Transactions on
      Communications, 34(2):373--375, Mar. 1988.
356                                IMAGE COMPRESSION STANDARDS




[127] M-I. Lu and C-F. Chen. A Huffman-type code generator with order-
      N complexity. IEEE Transactions on Acoustics, Speech, and Signal
      Processing, 38(9):1619--1626, Sept. 1990.

[128] A.G. Maclnnis. MPEG systems committee draft, ISO/IEC JTC1/SC2/
      WGI 1. In Digest of Papers COMPCON, Spring '91, pages 338--339.
      IEEE, 1991.

[129] A. Madisetti, R. Jaml, R.L. Baker, and R. Dianysian. Architecture
      and integrated circuits for real time vector quantization of images. In
      Proceedings IEEE Intern口作onal Co／色rence on A口加tics, Speech,（刀id
      Signal Processing (ICASSP), pages V--677--680, 1992.

[130] X. Maitre. 7 kHz audio coding with 64 kbitls. IEEE Journal on Selected
      Areas in Communications, 6(2):283--298, Feb. 1988.

[131] S.G. Mallat. A theory for multiresolution signal decomposition: the
      wavelet representation. IEEE Transactions on Pattern Analysis and
      Machine Intelligence, 1 1(7):674--693, July 1989.

[132] R. Manepally and D. Sprague. Intel's 1750 video processor - the
      programmable solution. In Digest of Papers COMPCON Spring 1991,
      pages 324--329, 1991.

[133] G. Maturi. Single chip MPEG audio decoder. IEEE Transactions on
      Consumer Electronics, 38(3):348--356, Aug. 1992.

[134] J.C. Michalina. Application specific DSP at SGS-Thomson. In IEEE
      Proceedings 可加切na肋nal 鈿叩Os岫i on Circuits and Syste刃is (IS-
      CAS), pages 627--630, 1989.
[135] J.L. Mitchell and W.B. Pennebaker. Optimal hardware and software
      arithmetic coding procedures for the Q-coder. IBM Journal of Research
      and Development, 32(6):727--736, Nov. 1988.

[136] J.W. Modestino and D.G. Daut. Combined source channel coding of
      images. IEEE Transactions on Communications, COM-27:1644--1659,
      Nov. 1979.

[137] J.W. Modestino, D.G. Daut, and A.L. Vickers. Combined source channel
      coding of images using the block cosine transform. IEEE Transactions
      on Communications, COM-29(9):1261--1274, Sept. 1981.
                                                                         357
REFERENCES




                                                 multimedia: JPEG, H.261,
[138] G. Morrison. Video coding standards for
                                                         ort of Multimedia
      MPEG. In lEE Colloquium on Technology Supp
      (Digest No. 088), pages 2.1--2.4, April 1992.
                                                 r, and T. Acharya. MAR-
[1391 A. Mukherjee, N. Ranganathan, J.W. Fliede
                                                         ased codes. IEEE
      VLE: a VLSI chip for data compression using tree-b
                                                         System s, 1(2):203-
      Transactions on Very乙irge Scale Integration (VLSI)
      -214, June 1993.
                                                          Algorithm for con-
[140] H. Murakami, S. Matsumoto, and H. Yamamoto.
                                                                 word length.
      struction of variable length code with limited maximum
                                                    ): 1157--il 59, Oct. 1984.
      IEEE Transactions on Communications, 32(10
                                                       motion video codec. In
[1411 T. Murakami et a!. A DSP architecture for 64Kbs
                                                                    s (ISCAS),
      Proceedings International Conference on Circuits and System
      pages 227--230. IEEE, 1988.
                                                            edings
[142] H.G. Musmann. The ISO audio coding standard. In Proce
      GLOBECOM '90, pages 511--5 17. IEEE, 1990.
                                                              with bit-rate
[143] M. Nakagawaet at. DCT-based still image compression ICs
                                                                     -717,
      contr아．IEEE Tr口ns口c卄ons（가iCo,玎U刃ier Electr이2ics, 38(3):711-
      Aug. 1992.

[144] J.B.O. Neal, Jr. and T.R. Natarajan. Coding isotropic images. IEEE
      Transactions on Information Theory, IT-23:697--707, 1977.
                                                                    based on
 [145] K. Ogawa et at. A single chip compression/decompression LSI
       JPEG. IEEE Transactions on Consumer Electr    onics , 38(3):703--71 0,
       Aug. 1992.
                                                                     h
 [146] N. Ohta. Packet Video - Modeling and Signal Processing. Artec
       House, Norwood, Massachussetts, 1994.
                                                                              e
 [147] S. Okuba. Reference model methodology - a tool for the collaborativ
       creation of video coding standards. Proceedings of the iEEE , 83(2):139-
       -150, Feb. 1995.
                                                                         ts,
 [148] S. Okubo, K. McCann, and A. Lippman. MPEG-2 requiremen
                                                                          al
       profiles, and performance verification. In Proceedings Internation
       Workshop on HDTV '93, Oct. 1993.
 358                                 IMAGE CoNIPREssIoN STANDARDS




 [149] Y. Ooi, A. Taniguchi, and S. Demura. A 162 Mbitis variable length
       decoding circuit using an adaptive tree search technique. In IEEE 1994
       Custom Integrated Circuits Conference, pages 6.5.1--6.5.4, 1994.

 [150] D. Pan. An overview of the MPEG/Audio compression algorithm. In
       Proceedings SPIE, Vol. 2187, San Jose, CA, pages 260--273. SPIE,
       Feb. 1994.

[151] D. Pan. Digital audio compression. Digital Technical Journal,5(2):28-
      -40, Spring 1993.
[152] D. Pan. A tutorial on MPEG/Audio compression. IEEE Multimedia,
      2(2):60--74, Summer 1995.

[153] K.K. Pang and T.K. Tan. Optimum loop filter in hybrid coders. IEEE
      Circuits and Systemsfor Video Technology,4(2):158, April 1994.

[154] H. Park and V.K. Prasanna. Area efficient VLSI architectures for
      Huffman coding. IEEE Transactions on Circuits and Systems-il:
      Analog and Digital Signal Processing,40(9):568--575, Sept. 1993.
[155] P. Patel and D. Douglass. Architectural features of the i860 - micropro-
      cessor RISC core and on-chip caches. In IEEE Proceedings ofICCD,
      pages 385--390, 1989.
[156] D.A. Patterson and J.L. Hennessy. ComputerArchitecture: a Quantita-
      tiPe Approach. Morgan Kaufmann,San Mateo, California, 1990.

[157] A. Peled and B. Liu. A new hardware realization of digital filters. IEEE
      Transactions on ASSP, ASSP-22(6):456--462, December 1974.
[158] W.B. Pennebaker and J.L. Mitchell. JPEG Still Im7iage Data Comnpres-
      sion Standard. Van Nostrand Reinhold, New York, 1993.

[159] H.A. Peterson, H. Peng, J.H. Morgan, and W.B. Pennebaker. Quanti-
      zation of color image components in the DCT domain. In SPIE Vol.
      1453 Hum72an Vision, Visual Processing, and Digital Display II, pages
      210--222, Feb. 1991.

[160] P. Pirsch, N. Demassieux,and W.Gehrke. VLSI architectures for video
      compression - a survey. Proceedings ofthe IEEE,83(2):220--246, Feb.
      1995.
                                                                         359
REFERENCES




                                                      compression processor.
[1611 S.C. Purcell. The C-Cube CL550 JPEG image
                                                 -323, 1991.
      In Digest of Papers COMCON, pages 318-
                                                  nsated video coding with
[1621 A. Puni and R. Aravind. Motion-compe
                                                     actions on Circuits and
      adpative perceptual quantization. IEEE Trans
                                                     Dec. 1991.
      Systems for Video Technology, 1(4):35 I --361,
                                                     efficient block-matching
[163] A. Puni, H.M. Hang, and D.L. Schilling. An
                                                              edings IEEE In-
       algorithm for motion compensated coding. In Proce
                                                                  l Processing
       ternational Conference on Acoustics, Speech, and Signa
       (ICASSP), pages 25.4. 1--25.4.4, 1987.
                                                         Cahners Publishing,
[164] R.A. Quinnell. Image compression, part 3. EDN,
      pages 1 나-120, May 13 1993.
                                                       Symp. on Architec-
[165] G. Radin. The 801 minicomputer. In Proceedings
                                                             39--47, Palo
      tural Support for Prog. Lang. and Oper. Systems, pages
      Alto, CA, 1982.
                                                              ithms, Advan-
[166] K.R. Rao and P. Yip. Discrete Cosine Transform - Algor
                                                             rnia, 1990.
      tages, Applications. Academic Press, San Diego, Califo
                                                                 er chip. In
[167] S.K. Rao et a . A real-time P*641MPEG video encod
                                                                      , pages
      Proceedings IEEE International Solid-State Circuits Conference
      32--33, 1993.
                                                                  encoding of
 [168] V. Ratnakar, E. Feig, E. Viscito, and S. Kalluri. Run妃ngth
                                                                       pages
       quantized DCT coefficients. In Proceedings SPIE, volum 2419,
                                                                e
       398--406, Feb. 1995.
                                                                  thm for op-
 [169] V. Ratnakar and M. Livny. RD-OPT: an efficient algori
                                                                         rence,
       timizing DCT quantization tables. In Data Compression Confe
       Snowbird, Utah, pages 333--339, March 1995.
                                                                       ression
 [170] A. Razavi et al. VLSI implementation of an image comp
                                                         In Proce eding s IEEE
       algorithm with a new bit rate control capability.
                                                                           ssing
       International Conference on Acoustics, Speech, and Signal Proce
       (ICASSP), pages V:669--672, 1992.
                                                                   IEEE Signal
 [171] O. Rioul and M. Vettenli. Wavelets and signal processing.
       Processing Magazine, 8:14--38, Oct. 1991.
 360                               IMAGE COMPRESSION STANDARDS




 [172] P.A. Ruetz et al. A high-performance full-motion video compres-
       sion chip set. IEEE Transactions on Circuits and Systems for Video
       Technology, 2(2):l l卜- 121, June 1992.

 [173] C.P. Sandbank, editor. Digital Television. John Wiley and Sons,
       Chichester, England, 1990.

 [174] R. Schaphorst. Status of H.324 - the videoconferencing standard for
       GSTN and mobile radio. In Desktop Video Conference DVC West,
       pages 457--462, May 1995.
[175] V. Seferidis and M. Ghanbari. Generalized block matching motion
      estimation. In Proceedings of SPIE.' Visual communications and Image
      Processing, pages 80--9 1, 1992.

[176] C.H. Sequin and D.A. Patterson. Design and implementation of RISC-
      I. Technical Report UCB/CSD 82/106, Computer Science Division
      (EECS), Univ. of California, Berkeley, October 1982.

[177] A. Shacham et al. Architectural considerations for SF-core based
      microprocessor. In IEEE Proceedings of ICCD, pages 21--24, 1991.

[178] Y. Shishikui. A study on modeling of the motion compensation
      prediction error signal. fE/CE Transactions on Communications, Japan,
      E75-B(5):368--376, May 1992.

[179] S. Shlien. Guide to MPEG-I audio standard. IEEE Transactions on
      Broadcasting, 40(4):206--2 18, Dec. 1994.

[180] M. Slater, editor. A Guide to RISC Microprocessors. Academic Press,
      San Diego, California, 1992.

[181] M.M. Stojancic and C. Ngai. Architecture and VLSI implementation of
      the MPEG-2:MP,ML video decoding process. SMPTE Journal, pages
      62--72, Feb. 1995.

[182] M.T. Sun, L. Wu, and M.L. Liou. A concurrent architecture for VLSI
      implementation of discrete cosine transform. IEEE Transactions on
      Circuits and Syste,ns, CAS-34(8):992--994, August 1987.

[183] I. Tamitani et a!. An encoder/decoder chip set for the MPEG video
      standard. In Proceedings IEEE International Conference on Acoustics,
      Speech, and Signal Processing (KASSP), pages V--661--664, 1992.
.REFERENCES                                                               361




 [184] Texas Instruments. TM5320 DSP, Product Overview, 1994.

 [185] C.C. Todd et al. AC-3: Flexible perceptual coding for audio transmission
       and storage. In Proceedings AES 96th Convention, Amsterdam, page
       preprint 3796, 1994.

 [186] M. Toyokura et al. A video DSP with macroblock-level-pipeline
       and a SIMD type vector-pipeline architecture for MPEG2 codec. In
       Proceedi叩s IEEE 加ternat加nal 品妃-State C加Cu山 Con／計ence, pages
       74--75, 1994.

 [1871 G. Tziritas and C. Labit. Motion Analysis for Image Sequence Coding.
       Elsevier Science b. V., Amsterdam, The Netherlands, 1994.

 [188] S. Undy et al. A low-cost graphics and multimedia workstation chip-set.
       IEEE Micro, 14(2):10--22, April 1994.

 [189] S. Uramoto et al. A 100-MHz 2-D discrete cosine transform core
       processor. 旭EE Journal of Solid-State Circuits, 27(4):492--499, April
       1992.

 [190] D.C. Van Voorhis. Constructing codes with bounded codeword lengths.
       旭2ETr口ns口C肋ns Infor枷加n Theory, 20(2):288--290, Feb. 1974.

 [191] G.K. Wallace. The JPEG still picture compression standard. IEEE
       Transactions on Consumer Electronics, 38(l):xviii--xxxiv, Feb. 1992.

 [192] N.D. Wells. MPEG: Status of digital coding standardization. In lEE Col-
       loquium on Digital satellite technology and electronic newsgathering,
       Digest No. 006, 1993.

 [193] P.T. Whitcomb and H.M. Ahmed. A VLSI architecture for the CCITT
       G.722 codec. In Proceedings IEEE GLOBECOM '89, pages 1262--
       1266. IEEE, 1989.

 [194] S.A. White. Applications of distributed arithmetic to digital signal
       processing: A tutorial review. IEEE ASSP Magazine, 6(3):4--19, July
       1989.

 [195] I.H. Witten, R.M. Neal, and J.G. Cleary. Arithmetic coding for data
       compression. Communi口2tiOflS 可the Associat油'zfor Co刃zputing 凡I口－
       chinery ACM, 30(6):520--540, June 1987.
362                                IMAGE COMPRESSION STANDARDS




[196] S. Wolter, D. Birreck, and R. Laur. Classification for 2D-DCTs and
      a new architecture with distributed arithmetic. In Proceedings IEEE
      International Symposiumn on Circuits and Systems, pages 2204--2207,
      June 1991.

[197] J.W. Woods and S.D. O'Neil. Subband coding of images. IEEE
      Transactions on Acoustics, Speech, and Signal Processing,34(5):1278-
      -1288, Oct. 1986.

[198] K. Xie, L.V. Eycken, and A. Oosterlinck. A new block-based motion
      estimation algorithm. Signal Processing:Imnage Gommunication,4:507-
      -517, May 1992.

[199] K-M. Yang, H. Fujiwara, T. Sakaguchi, and A. Shimazu. VLSI
      architecture of a versatile variable length decoding chip for real-time
      video codecs. In Proceedings IEEE Region /0 Conference on Gomputer
      and Com,nunication Systems(TENCON '90), IJong Kong, pages 551--
      554, Sept. 1990.

[200] K-M. Yang, M-T. Sun, and L. Wu. A family of VLSI designs for the
      motion compensation block- matching algorithm. IEEE Transactions on
      Circuits and Systems, 36(10):1317--1325, October 1989.

[201] C-G. Zhou et at. MPEG video decoding with the UltraSPARC visual
      instruction set. In Digest of Papers COMPCON Spring 1995, pages
      470--475. IEEE, March 1995.
                                                      INDEX


AC-3 algorithm, 298                Backward-adaptive bit allocation,
AC-3 audio coding, 308                   310
AC-3 decoder, 311                  Barrel shifter, 251, 255
AC-3 decoding, 313                 Baseline JPEG, 139, 258, 263
AC-3 encoder, 310                  Basis functions, 63
Address generation, 221            Bidirectional prediction, 126, 171
ADPCM, 299                         Binary tree, 19
Algorithmic complexity, 208        Binary tree-search vector
Aliasing, 323                            quantizer, 318
Apple Computer, 330                Bit stream scalability, 182, 191
Arithmetic coder, 250              Bit-rate control, 268
Arithmetic coding, 37              Bitonal, 44
 decoding, 40                      Block coding, 62
 encoding, 37                      Block matching algorithms, 108
 implementation issues, 42         Block matching criterion, 108
Array Microsystems, 278            Block matching
Array processor, 239                 full-search, 238
ASPEC transform coder, 314         C-Cube, 263, 284
AT&T, 284                           CL550 and CL560, 266
Audio compact discs, 297             VideoRISC, 275
Audio compression standards, 197   Captain Crunch, 331
Audio                              CCIR 601, 164, 184, 198
 5.1 channels, 308                 CD-ROM, 2
AV4I20A video controller, 284      CELP coder, 299
AV4220 video decoder, 284          Channel coder, 5
AV4引0 미deo encoder, 284            CIF, 198, 208, 238
Average codeword length, 20, 26    Cinepak, 331
AVP Video Codec, 284               CISC, 289
B-pictures, 167                    Closed GOP, 175
 coding, 179                       Coding complexity, 8
Backward motion estimation, 105    Coding delay, 8
                                   Coding efficiency, 7
 364                                IMAGE COMPRESSION STANDARDS




 Color conversion, 265, 285                row-column decomposition,68,
 Color facsimile, 157                          226
 Compression ratio, 4, 21, 55              scaled, 79
 Compression, I                          Decimation. 113
   block-based, 11                       Decorrelation efficiency, 84
   issues, 12                            Differential coding, 17, 47
   tradeoffs, 7--8                       Digital audio, 297
 Computing power                         Digital film, 308
   DSP,211                               Digital telephony, 297
   RISC, 211                             Discrete cosine transform, 63
Concealment motion vectors, 187          Discrete Fourier transform, 63
Constant bit rate coders, 11            Discrete Hadamard transform, 63
Constrained bit stream, 165             Discrete sine transform, 63
Constrained parameter bit stream,       Distributed arithmetic, 226--227
       174                              DMA,221
Content-addressable memory,             Dolby Laboratories, 298, 308
       251, 257                         Downsampling,323
Context modeling, 49                    DPCM vs. DCT-based systems, 85
Covariance function, 54,84              DPCM,61,322
Covariance matrix, 84                   DSP unit, 281
CS4920,313                              DSP
Data interleaving, 134                    core, 215, 219, 271
Data partitioning, 191                    instruction format, 220
Data-driven architecture, 278           Dual-prime mode, 187
Daubechies four-tap wavelet, 327       End of block, 142
Daubechies wavelets, 332               Entropy coder, 249
DC-coded pictures, 167                 Entropy coding, 16, 211
DCT basis functions,66                 Entropy decoder, 253
DCT,208, 226, 330                      Entropy decoding, 16
  3-D,88                               Entropy, 7, 21
  accuracy, 202                        Facsimile, 2,44
  benefits,65                             standards,44
  complexity, 77, 80                   FF1', 221, 303
  definition,66                        Field pictures, 185
  fast algorithms, 77                  Field prediction, 185
  implementation, 231                  Filter bank, 300
  MOPS requirements, 208               Finite-state machine,253
  multiplication-free, 83              Floating-point, 290
                                       Forward motion estimation, 105
Index                                                             365




Forward-adaptive bit allocation,      constrained length, 24
      310                             H.261, 200
Fractals, 54                          JPEG, 48
Frame differencing, 94                properties, 21
  performance, 95                     Voorhis method, 33
Frame pictures, 185                Huffman decoder, 254
Frame prediction, 185              Huffman decoding, 22, 26, 29
Full-search algorithm, 108         Huffman tables, 251
G.72l, 299                         Human perception, 136
G.722, 197, 299, 313               Human visual system, 59
G.726, 197, 299                    Hybrid coding, 91
G.728, 197, 299, 314               Hybrid video coding
GOPS, 238                             performance, 101
Grand Alliance HDTV system,        I-pictures, 167
      298, 引4                         coding, 176
Grayscale, 47                      IBM, 222, 284
Group of pictures, 174             IDCT, 66, 81
H.120, 195                         Integrated Information
H.130, 195                                Technology, 276
H.221, 197                         Intel, 222, 330
H.230, 197                            DVI, 330
H.233, 197                            Indeo, 330
H.242, 197                         Interframe coding, 90, 330
H.261, 196, 211, 235, 260, 272,       performance, 98
      279                          Interframe processing, 272
  GOB, 201                         Interlaced video, 162
  INTER mode, 200                   Interpolation, 243
  INTRA mode, 200                  Intraframe coding, 91, 330
  MOPS requirements, 208            Inverse DCT, 66, 303
 H.262, 161                         Inverse quantization, 73
 H.320, 196                         151가나, 195
 Harvard architecture, 219          ISO standard 11172, 161
 HDTV, 182, 209, 247, 308           ISO standard 13818, 161
 Hewlett-Packard, 289, 291          ITU-T Rec. T.4, 44
 Hierarchical mode, 147             ITU-T Rec. T.6, 45--46
 Huffman coder, 171                  JBIG, 46
 Huffman coding, 18, 250             JFIF, 154
   ad寸田c table design, 31            JPEG processor, 263
   bounds, 26                        JPEG versus JBIG, 50
 366                             IMAGE COMPRESSION STANDARDS




 JPEG, 129, 178, 192, 211, 258       Mean absolute error, 107, 237, 317
    baseline, 132, 150               Mean opinion score, 9
    decoder, 132                     入4ed治 Vis由n
   encoder, 131                        Motive, 331
   entropy coding, 138               Microsoft, 331
   extensions, 155                   Minimum coded unit, 134, 264
   hierarchical, 147                 入4odified Huffn伍n, 44
   Huffman coding, 139               入4od小ed Read, 45
   Huffman tables, 36                MOPS requirements
   implementation issues, 151          subband filtering, 328
   interchange format, 132             H.261, 213
   lossless, 47, 60                    motion estimation, 238
   progressive, 145                    MPEG, 209
   sequential, 145                     TSVQ, 3四
   SPI'下, 156                       MOPS, 8, 208
 Karhunen-Loeve transform, 63       Motion compensation, 91, 170,
Lei-Sun VLC decoder, 255                  211, 237
Lei-Sun VLC encoder, 251            Motion estimation, 91, 211, 237,
Logarithmic search, 109                   295
Loop filter, 201                      comparisons, 120
Loss less compression, 6, 15          full-search, 108, 242
Lossy compression, 8, 11, 53          hierarchical, 116
  video, 87                           logarithmic search, 109
LSI Logic, 235, 247, 284              PHODS, 111
  L64 111, 313                        pixel projections, 115
  L64702, 267                         pixel subsampling, 113
  L64720, 244                         sub-pel, 243
  L64730, 234                         sub-pixel-accurate, 122
  L64735, 234                       Motion estimator, 239--240
  L64745 and L64702, 267             ha作pel, 246
Macroblock stuffing, 175            Motion vector, 106, 237
Macroblock, 90, 175, 184, 200       Motion-estimation error, 97
  MPEG, 165                         Motion-JPEG, 150, 331
Mallat, 327                         Motive, 331
Masking curve, 303                  M아or이a, 222
Matrixing operation, 302, 305       MPEG audio coding, 300
Matsushita, 286, 296                MPEG audio standard, 298
  VDSP2, 274                        MPEG audio
Mean absolute difference, 107        Layers, 307
Index                                                              367




MPEG encoder, 168                   Perceptual model, 59
MPEG vs H.261, 203                  Picture layer, 175
MPEG, 211                           Pixel interpolation, 243
 entropy coding, 177                Polyphase networks, 301
 hardware, 271                      Power spectral density, 56, 59
 layers, 174                        Prediction residual, 18, 47, 91
 motion estimation, 168             Predictive coder, 60, 130, 200
 video decoder, 171                 Predictive coding, 299, 322
MPEG-I, 161, 207                    Prefix-condition code, 21
MPEG-2 audio compression, 308       Probability model, 15, 43
入IPEG그, 161, 182, 298               Processing requirements, 208
 hardware, 274                      Processor array, 244
 levels, 182                        Progressive video, 163
 Main profile, 190                  PSNR, 9
 profiles and levels, 189           Psychoacoustic model, 309
 profiles, 182                      Pulse code modulated, 300
MPEG-4, 161, 326                    Pyramidal filter, 327
Multimedia enhancements, 290,       QCIF, 199, 208
     295                            QMF filters, 325, 327
Multimedia instructions, 291, 293   Quality factor, 137
Multimedia Video Processor, 280     Quantization function, 60
Multimedia-enhanced processors,     Quantization matrix, 135, 174
      289                           Quantization scale factor, 176
Multiresolution representation,     Quantization table, 136
      327                           Quantization, 69, 72, 189, 211
MUSICAM subband coder, 314          QuickTime, 330
National Semiconductors, 222        Rate-distortion function, 55--56,
NEC, 246--247, 260, 286                   93--94
  VSP3, 272                         Rate-distortion theory, 92
NTSC, 164, 195, 198, 276            Reference block, 237
Nyquist theorem, 297, 323           Reference picture, 105
Orthogonal transform, 66            Relative sampling factors, 133
Orthonormal basis, 326              RGB to YCbCr, 265
P x 64, 196                         RISC vs DSP, 221
P-pictures, 167                     RISC, 207, 289
  coding, 178                         architecture, 216
PA7100LC, 291                         core, 215, 271, 296
PAL, 164, 195, 276                    instructions, 216
PCM, 300                            ROM-accumulator, 230
 368                              IMAGE COMPRESSION STANDARDS




   mo小fled, 233                       SPIFF, 156
 Row-column decomposition, 208,       Subband analysis filter, 301
       225                            Subband coding, 321
 Run-length coder, 249                Subsampling, 134
 Run-length coding, 44                  4:2:0, 164, 208, 264
   benefits, 144                        4그2, 164
 Sample-based coding, 60                4:4:4, 184
 Sampling frequency, 297              Successive approximation, 146
 Sampling resolution, 297             Sun Microsystems, 289, 294
 Sanyo Electric, 269                  Temporal correlation, 3
 Saturation arithmetic, 290           Temporal prediction, 91
 Scalable compression, 13             Temporal redundancy, 88
 Scalable extensions, 184             Temporal scalability, 192
 Search window, 237                   Texas Instruments, 222
 Selective refinement, 155             TM5320AV110, 313
 Separable filters, 324                入WP, 280
 Sequence layer, 174                   TMS320IO, 222
 SGS-Thomson, 222, 247, 284            1M532080, 280
  IMSAl21, 234                         TMS320C30, 220
  ST13220, 245                       Three-step search, 109
  5TV3200, 234                       Tiling, 156
  5TV3208, 234                       TLB, 218
Shortened Huffman code, 24           Toshiba, 270
SIF, 164                             Transformation kernels, 63
  definition, 164                    Two's complement, 229
Signal quality, 8                    UltraSPARC, 294
Signal to noise ratio, 9             Uniquely decodable code, 22
Significant pixel area, 165          Upsampling, 323
SIMD, 274, 285                       Variable bit rate coders, 11
SNR Sc기ab小ty, 191                    Variable length integer, 258
SNR, 57                              Variable quantization, 155
Source coder, 4                      Variable-length coder, 170, 249
Source-coding theorem, 56, 62        VCP processor, 276
Spatial correlation, 3               VDSP, 296
Spatial redundancy, 54               VDSP2, 273
Spatial scalability, 192             Vector quantization, 63, 316, 322
Spectral correlation, 3              Video coders, 271
Spectral envelope, 310               Video coding
Spectral selection, 146                model, 94
                              369




Video editing, 13
Video for Windows, 331
Videoconferencing, 109, 195
VideoFlow, 278
VideoRISC, 275
Videoconferencing, 238
Vision controller, 277
Vision processor, 277
VLIW, 219, 221
VP+, 277
Wallace tree-adder, 227
Wavelet decomposition, 326
Wavelets, 326
Wi叱owing 야氾ration, 305
Windowing, 301
YCbCr, 165, 184, 198
Zig- zag order, 141
Zoran
  ZR36040 and ZR36050, 268
  ZR36020, 234
  ZR38000, 313
