---
source_url: /run/media/yutae/Data/Numerical_Recipes_Example_Book.pdf (USB, 2026-10-25 확인)
ingested: 2026-10-25
sha256: 9ac5b24bd120d1ccc7ab97608c6a915826c6e8f2232c40bd0b1435235e2562d2
---
# Numerical Recipes Example Book (C), 2nd ed. (raw source)
> text-layer PDF → `pdftotext -layout` 전체 추출 (~682,093 chars). 일부 토큰은 인식 오류로 깨짐 (한/영 혼용 OCR 산출). 원문 PDF(`books/Numerical_Recipes_Example_Book.pdf`, 로컬) 대조 권장.

## Book metadata
- title: Numerical Recipes Example Book (C), Second Edition
- authors: William T. Vetterling (Polaroid), Saul A. Teukolsky (Cornell), William H. Press (Harvard-Smithsonian CfA), Brian P. Flannery (EXXON)
- edition: 2nd (1st 1988, 2nd 1992)
- year: 1988/1992
- publisher: Cambridge University Press
- pages: 336 (pdfinfo)
- isbn: 0-521-43720-2 (example book in C)
- note: companion example book for Numerical Recipes in C (0-521-43108-5); algorithms only (working programs in NRiC)
+ source file: `Numerical_Recipes_Example_Book.pdf` (sha256: `9ac5b24bd120d1cc…`)
+ extract: `pdftotext -layout` @ 2026-10-25, 682,093 chars

## Chapter structure (from TOC)
| # | topic | page |
|---|-------|------|
| 1 | Preliminaries | 1 |
| 2 | Solution of Linear Algebraic Equations | 6 |
| 3 | Interpolation and Extrapolation | 40 |
| 4 | Integration of Functions | 54 |
| 5 | Evaluation of Functions | 68 |
| 6 | Special Functions | 81 |
| 7 | Random Numbers | 125 |
| 8 | Sorting | 139 |
| 9 | Root Finding and Nonlinear Sets of Equations | 153 |
| 10 | Minimization and Maximization of Functions | 171 |
| 11 | Eigensystems | 195 |
| 12 | Fast Fourier Transform | 205 |
| 13 | Fourier and Spectral Applications | 221 |
| 14 | Statistical Description of Data | 227 |
| 15 | Modeling of Data | 259 |
| 16 | Ordinary Differential Equations | 271 |
| 17 | Two-Point Boundary Value Problems | 281 |
| 18 | Integral Equations and Inverse Theory | 283 |
| 19 | Partial Differential Equations | 287 |
| 20 | Less-Numerical Algorithms | ~295 |

## Original text (all 337 pages)

     NUI'너E口I口AL
      口E口作）ES
     Example 日ook ［口］
I       Se口ond Edit；七n
1    WilliamT. Vetterling   SauIA. Teukolsky
     William H. Press       Brian P. Flannery




rH
Numerical Recipes
Example Book (C)
Second Edition



William T. Vetterling
         Polaroid Corporation

Saul A. Teukolsky
         Department of Physics, Cornell University

W川am H. F가ess
         Harvard-Smithsonian Center for Astrophysics

Brian P. Flannery
         EXXON Research and Engineering Company




      CAMBRIDGE
      UNIVERSITY PRESS
Published by the Press Syndicate of the University of Cambridge
The Pitt Building, Trumpington Street, Cambridge CB2 1RP
40 West 20th Street, New York, NY 10011-4211, USA
10 Stamford Road, Oakleigh, Victoria 3166, Australia


Copyright @) Cambridge University Press 1988, 1992
except for computer programs and procedures, which are
Copyright(9 Numerical Recipes Software 1987, 1988, 1992
All Rights Reserved.


First Edition originally published 1988; Second Edition originally published 1992.


Printed in the United States of America
Typeset in TX



        The computer programs in this book are available, in C, in several
   machine-readable formats. There are also versions of this book and
   its software available in the FORTRAN, Pascal, and BASIC programming
   languages.
       To purchase diskettes in IBM PC or Apple Macintosh formats, use
   the order form at the back of the book or write to Cambridge Univer-
   sity Press, 110 Midland Avenue, Port Chester, NY 10573.
        Unlicensed transfer of Numerical Recipes programs from the above-
   mentioned IBM PC or Apple Macintosh diskettes to any other format,
   or to any computer except a single IBM PC or Apple Macintosh or corn-
   patible for each diskette purchased, is strictly prohibited. Licenses for
   authorized transfers to other computers are available from Numerical
   Recipes Software, P.O. Box 243, Cambridge, MA 02238 (FAX 617 863-
   1739). Technical questions, corrections, and requests for information
   on other available formats should also be directed to this address.




 Library of Congress cataloguing in publication data available
 A catalogue record for this book is available from the British Library

ISBN 0 521 43720 2 Example book in C (this book)
 ISBN 0 521 43108 5      Numerical Recipes in C
 ISBN 0 521 43714 8 C diskette (IBM 5.25", 1.2M)
 ISBN 0 521 43724 5 C diskette(IBM 3.5", 1.44M)
 ISBN 0 521 43715 6 C diskette (Mac 3.5",800K)
                           CONTENTS

     Preface                                            V
     A Note on Numerical Recipes Utility Functions      vii
 1. Preliminaries                                       1

 2. Solution of Linear Algebraic Equations               6
 3. Interpolation and Extrapolation                     40
 4. Integration of Functions                            54
 5. Evaluation of Functions                             68
 6. Special Functions                                   81
 7. Random Numbers                                     125

 8. Sorting                                            139
 9. Root Finding and Nonlinear Sets of Equations       153
10. Mm油izat油i and Maximiz毗油i of Functions              168
11. Eigensystems                                       185
12. Fast.Fourier Transform                             195
13. Fourier and Spectral Applications                  209
14. Statistical Description of Data                    222
15. Modeling of Data                                   247
16. Integration of Ordinary Differential Equations     264
17. Two Point Boundary Value Problems                  277
18. Integral Equations and Inverse Theory              280
19. Partial Differential Equations                     284
20. Less-Numerical Algorithms                          290
     Appendix A: Header Files                          300
     Appendix B: Numerical Recipes Utility Functions   313
     Appendix C: Functions for Complex Arithmetic      319
     Index of Demonstrated Routines                    322




                                      泣
F가eface

     This Numerical Recipes Example Book (C) is designed to accompany the text
and reference book Numerical Recipes in C: The Art of Scientific Computing, Second
Edition, by William H. Press, Saul A. Teukolsky, William T. Vetterling, and Brian
P. Flannery (Cambridge University Press, 1992). In that volume, the algorithms
and methods of scientific computation are developed in considerable detail, starting
with basic mathematical analysis and working through to actual implementation in
the form of C routines. The routines in Numerical Recipes in C: The Art of Scien-
tific Computing, numbering more than 300, are meant to be incorporated into user
applications; they are procedures (or functions), not stand-alone (main) programs.
    It often happens, when you want to incorporate somebody else's procedure into
your own application program, that you first want to see the procedure demonstrated
on a simple example. Prose descriptions of how to use a procedure (even those in
Numerical Recipes) can occasionally be inexact. There is no substitute for an actual,
C demonstration program that shows exactly how data are fed to a procedure, how
the procedure is called, and how its results are unloaded and interpreted.
    Another not unusual case occurs when you have, for one seemingly good purpose
or another, modified the source code in a "foreign" procedure. In such circumstances,
you might well 'ant to test the modified procedure on an example known previously
to have worked correctly, before letting it loose on your own data. There is the related
case where procedure source code may have become corrupted, e.g., lost some lines
or characters in editing or customization, and a simple revalidation test is desirable.
     These are the needs addressed by this Numerical Recipes Exflmple Book. Divided
into chapters identically with Numerical Recipes in C: The Art of Scientific Comput-
ing, this book contains C source programs that exercise and demonstrate all of the
Numerical Recipes procedures and functions. The programs are commented, and each
is also prefaced by a short description of w1at it does, and of which Numerical Recipes
routines it exercises. In many cases where the demonstration programs require input
data, that data is also printed in this book. In some cases, where the demonstration
programs are not "self-validating," sample output is also shown.
     Necessarily, in the interests of clarity, the Numerical Recipes procedures and func-
tions are demonstrated in simple ways. A consequence is that the demonstration
programs in this book do not usually test all possible regimes of input data, or even
all lines of procedure source code. The demonstration programs in this book were
by no means the only validating tests that the Numerical Recipes procedures and
functions were required to pass during their development. The programs in this book
were used during the later stages of the production of Numerical Recipes in C: The
Art of Scientific Computing to maintain integrity of the source code, and in this role


                                           V
were found to be invaluable.

                           DISCLAIMER OF WARRANTY

                                     ARE PROVIDED "AS IS" WITHOUT WAR-
   THE PROGRAMS LISTED IN THIS BOOK
              KIND.  WE  MAKE NO  WARRA NTIES, EXPRESS OR IMPLIED, THAT
RANTY OF ANY
                                       E ARE FREE OF ERROR, OR ARE CON-
THE PROGRAMS CONTAINED IN THIS VOLUM
                            STAND ARD OF   MERCHANTABILITY, OR THAT THEY
SISTENT WITH ANY PARTICULAR
                                    ANY PARTICULAR APPLICATION. THEY
WILL MEET YOUR REQUIREMENTS FOR
                                         PROBLEM WHOSE INCORRECT SOLU-
SHOULD NOT BE RELIED ON FOR SOLVING A
                      INJURY TO A  PERSO  N OR LOSS OF PROPERTY. IF YOU
TION COULD RESULT IN
                                      R, IT IS AT YOUR OWN RISK. THE AU-
DO USE THE PROGRAMS IN SUCH A MANNE
                                  LIABIL ITY FOR DIRECT OR CONSEQUENTIAL
THORS AND PUBLISHER DISCLAIM ALL
                    FROM YOUR  USE OF THE   PROGRAMS.
DAMAGES RESULTING




                                       vi
A Note on Numerical Recipes Utility Functions

    The programming conventions used in this book are discussed fully in Chapter
1 of Numerical Recipes in C: The Art of Scientific Computing. You should have a
copy of that book - without it, this one will not be very meaningful. Nevertheless,
we review a few important matters here.
     The Numerical Recipes software collection in C contains about 350 routines. For
the most part the routines are self-contained, making reference only to other routines
in the package, or to standard C library functions. There are some consistent excep-
tions, however. (1) When the Numerical Recipes functions (or the main() programs
in this book) encounter an error, they turn matters over to a function nrerrorQ, not
a standard C function. (2) When vectors and multidimensional matrices are allocated
or deallocated, use is made of a set of utility functions with names like matrixO,
vector 0, free_matrix 0, and free_vector 0. These Numerical Recipes-specific
shared functions are found in a utility file nrutil. c, listed in Appendix B. Example
routines that use any of these utilities include the header file nrutil. h (Appendix
A) along with any of the standard library header files which are required. Similar
remarks apply to routines using complex arithmetic. These make calls to functions
in the file complex. c, which is listed in Appendix C. The appropriate header file is
called complex.h (Appendix A).
     All of the examples in this book call at lea毗 one, and sometimes more than one,
of the Numerical Recipes functions. A prototype declaration must generally be given
for each of the functions used. To spare you the trouble of searching program listings
for the proper declarations, we have compiled an alphabetical list in the form of a
header file nr.h, reproduced in Appendix A. You may, if you wish, simply include the
file nr . h at the beginning of your own application program and use the recipes with
abandon. That is what we have done in the example routines in this book. In some
cases, however, you might want to cull from the file only those declarations which your
programll requires, and to declare them individually. The Numerical Recipes routines
themselves, in which we sought to make the interdependence of routines explicit, are
written in this fashion.
      A final important point about the header file nr.h is that, as furnished on the
diskette, it contains both ANSI C and traditional K&R-style declarations. The ANSI
forms are invoked if any of the following macros are defined: __STDC_ _, ANSI, or
川RANSI. (The purpose of the last name is to give you an invocation that does not
conflict with other possible uses of the first two names.) If you have an ANSI compiler,
it is essential that you invoke it with one or more of these macros defined. The typical
means for doing so is to include a switch like "-DANSI" on the compiler command
line.


                                          vii
    uf course, with an ANSI compiler, you should also be sure to use the ANSI
                                                                               printed
versions of the programs supplied on the Numerical Recipes C Diskette and
in thk Example Book. If you have only a traditional Kernighan and Ritchie(K&R)
C compiler, then you should be sure to use the alternative K&R program versions
that are also supplied on the diskette. These differ slightly from the listings in this
book (and the main book), but the two C dialects are close enough that separate
program listings are not necessary.
Chapter 1: Preliminaries

         The routines in Chapter 1 of Numerical Recipes are introductory and less
    general in purpose than those in the remainder of the book. This chapter 's
    routines serve prim跏加 的 expose t加 切ok눙 notational convention옥 ill哨打ate
    control structures, and perhaps to amuse. You may even find them useful.
    We hope that you will use badluk for no serious purpose.



     Procedure fimoon calculates the phases of the moon, or more exactly, the Julian
 day and fraction thereof on which a given phase will occur or has occurred. The
program xf].moon asks the present date and compiles a list of upcoming phases. We
have compared the predictions to lunar tables, with happy results. Shown are the
results of a test run, which you may replicate as a check. In this program, notice
 that we have set ZON (the time zone) to -5.0 to signify the five hour separation of
the Eastern Standard time zone from Greenwich, England. Our convention requires
you to use negative values of ZON if you are west of Greenwich, as we are. The Julian
day results are converted to calendar dates through the use of caldat, which appears
later in the chapter. The fractional Julian day and time zone combine to form a
correction that can possibly change the calendar date by one day.
    Date          Time (EST)     Phase
 12 9 1992           7 PM     full moon
 12 16 1992          2 PM     last quarter
 12 23 1992         8 PM      new moon
 12 31 1992        10 PM      first quarter
  1 8 1993          8 AM      full moon
  1 14 1993        11 PM      last quarter
  1 22 1993         1 PM      new moon
  1 30 1993         6 PM      first quarter
  2 6 1993          7 PM      full moon
  2 13 1993        10 AM     last quarter
  2 21 1993         8 AM     new moon
  3 1 1993         11 AM      first quarter
  3 8 1993          5 AM     full moon
  3 14 1993        11 PM     last quarter
  3 23 1993         2 AM     new moon
  3 30 1993       11 PM      first quarter
  4 6 1993          2 PM     full moon
  4 13 1993         3 PM     last quarter
  4 21 1993         6 PM     new moon
  4 29 1993         8 AM     first quarter
2      Nu／了ierical／꾸ec徊es Example 80아（

/* Driver for routine fi moon */

#include <stdio.h>
#include "nr. h"

#define Z0N (- 5. 0)

jot main(vojd)
{
     jot j, il, i2, i3, id, im, iy, n,nph=2;
    fl oat tinizon=Z0N/ 24. 0, frac, secs;
    long jl, 32;
    static char *phase[]={"ne므 moon" ,"first          quarter '",
         "full moon", "last quarter ") ;

    printf ( "Date of the next few phases of the moon\n") ;
    printf ( "Enter today\ 's date (e. g. 12 15 1992) : \n") ;
    scanf ( "/.d '/4 /,d", kim,&id,kiy) ;
    1巾 Approximate number of full moons since january 1900 巾/
    n=(int) (12. 37* (jy_1900+( (im-0. 5) /12. 0) ));
    j l= julday (im, jd, iy) ;
    tlinoon(n,nph,kj2, 立frac) ;
    n += (jot) ( (jl- j2) /29. 53 + (ji >= j2 7 0. 5 : -0. 5) );
    printf ( "\ n%los %19s /,9s\n", "date", "tiine (EST) " , 'phase") ;
    for (i '1; i<=20; j++) {
         flmoon(n,nph,kj2, &frac) ;
         frac=24 .0* (frac+timzon) ;
         if (frac < 0. 0) {
             --32;
             frac += 24. 0;
         }
         if  (frac > 12. 0) {
              ++j2;
              frac -= 12. 0;
         } else
              frac += 12. 0;
         j1= (int) frac;
         sec5=3600. 0* (frac- il) ;
         j2= (jnt) (secs/60. 0) ;
         i3=(jnt) (secs-60* j2+0. 5) ;
         caldat (j2, &im,&id,kiy) ;
         printf ( "Y.5d /.3d /,5d 'h7d: 'h2d: 'h2d     %s\n"
              im, id, iy, il, i2, i3, phase[nph] );
         if (nph == 3) {
              nph=0;
              ++n ;
         } else
              ++nph;
    }
    return 0;
}

    The function julday, our exemplar of the if control structure, converts calendar
dates to Julian dates. Not many people know the Julian date of their birthday or
any other convenient reference point, for that matter. To remedy this, we offer a list
of checkpoints, which appears at the end of this chapter as the file datesl. dat. The
                                                                            Gb카丹er I: 尸re加llinaries   3
    program xjulday lists the Julian date for each historic event for comparison. Then
    it allows you to make your own choices for entertainment.
    /卞 Driver for routine ju].day 中/

    #include <stdio.h>
    #include <stdljb. h>
    #include "nr. h"
    #include "nrutil. h"

    #define MAXSTR 80

    mnt main(void)
    {
         mnt i, id, im, iy, n;
         char t工t［甘AXSTR] ，·
         static char 中name[]={",      "j카luary", "tebruary " ,"march",
              "april ", "may ", "june", "july ", "august ", "eepte皿ber ",
              "october ", "novembex-", "deceinber "} ;
        FILE *fp;

        if   ( (fp = fopen( "datesl.dat느 "r ") ) == NULL)
               nrerror ( "Data file datesl.dat not found\n") ;
          fgets (txt, MAXSTrt, fp) ;
          fscanf (fp, "/.d /.*s ", &n) ;
         printf ( "\ n'/.Ss Y.8s /.6s 7.12s Y.9s\n" , "month" , "day " , "year " ,
               "julian day " ,"event ") ;
         for (i= 1; i <=n; i++) {
               fscanf (fp, "%d %d 'IA ", kim,&id,kiy) ;
               fgets (txt, MAXSTR, fp) ;
              printf ( "石los %3d Y.6d %lold '/.58 V.s ", name[i回, id, iy.
                    juldaf (im,id, iy) ," ". txt) ;
         }
         fclose(fp) ;
        printf ( "\ nYour choices: (negative to end) \n") ;
        printf ( "month day year (e.g. 1 13 1905) \n") ;
        for (i=1;i<=20;i+ +) {
              printf ( "\ ninm dd yyyy ?\n") ;
              scanf ( "/,d V.d %d", kim,&id,&iy) ;
              if (us < 0) return 1;
              printf ( "julian day: Y.ld \n", julday(im,id, iy) );
        }
        return 0;
}

    The next program in Numerical Recipes is badluk, an infamous code that com
bines the best and worst instincts of man. We include no demonstration
                                                                            program for
bad].u다．not just because we fear it, but also because it is self-contained, with sample
results appearing in the text.
    Chapter 1 closes with routine caldat, which illustrates no new points, but com-
plements julday by doing conversions from Julian day number to the month, day,
and year on which the given Julian day began. This offers an opportunity, grasped by
the demonstration program xcaldat, to push dates through both julday and caldat
in succession, to see if they survive intact. This, of course, tests only your authors'
ability to make mistakes backwards as well as forwards, but we hope you will share
 4        Numerica/ 尸e아）es日ample Book

our optimism that correct results here speak well for both routines. (We have checked
them a bit more carefully in other ways.)

/中 Driver for routina caldat */

#include <stdio . h>
#include <stdlib. h>
#include "nr.h"
#include "nrutil. h"

#define MAXSTR 80

ml1t main(void)
{
     ml1t i, id, idd,im, imm,iy, iyy, n;
     long j;
     char du工띠sy［片AXSTR] ;
     static char *name口＝{" , "j카luary", "february " ,"ma工ch",
         "april ", "may ", "june", "july ", "august "
         "september ", 'october ", "novembar ", "december"} ;
     FILE *fp;

     /李 Check whether caldat properly undoes the operation of              julday a!
     if ( (fp = fopen( "datesl.dat ", "r ") ) == NULL)
         nrerror ( "Data file datesl.dat not found\n") ;
     fgets (duinmy,MAXSTft, fp) ;
     fscanf (fp, "Y.d %ts ", kn) ;
     printf ("\ n %14s V.435\n", "original date: ", "reconstructed date") ;
     printf ( "h8s 工5s '1.65 Y.15s V.12s '1.55 /.6s\n", "month", "day". "year".
         "julman day " ,"month", "day " ,"year ") ;
     如r (i=1; i<=n; i++) C
           fscanf (fp, "/.d Xci Xd ", kim,kid, &iy) ;
           fgets (dummy,MAXSTR,fp) ;
           j =julday (im,id, iy) ;
           caldat (j ,kimm, &idd,&iyy) ;
           printf ( "%los %3d Y.6d %l3ld '1.165 Y.3d /.6d\n", na皿e[im] ,
             id, iy, j ,name[iui皿] ,idd, iyy) ;
     }
     fclose(fp) ;
     return 0;



                                            Appendix

File datesl. dat:

List of dates for testing routines in Chapter 1
16 entries
12 31   -1 End of millennium
01 01    1 0ne day later
10 14 1582 Day before Gregorian calendar
10 15 1582 Gregorian calendar adopted
01 17 1706 Benjamin Franklin born
04 14 1865 Abraham Lincoln Shot
04 18 1906 San Francisco earthquake
05 07 1915 Sinking of th日 Lu日its끄ia
07 20 1923 Pancho Villa assassinated
                                         Chapter 了： 尸ro加ninaries   5

06 23 1934 Bonnie and Clyde eliminated
07 22 1934 加hn Dillinger shot
04 03 1936 Bruno Hauptman electrocuted
05 06 1937 Mindenburg disaster
07 26 1956 Sinking of the Andrea Doria
06 05 1976 Teton darn collapse
06 23 1968 Julian Day 2440000
Chapter 2: Linear Algebraic Equations

         Numerical Recipes Chapter 2 begins the "true grit " of numerical anal-
    ysis by considering the solution of linear algebraic equations. This is done
    月r就 by Gauss-，兀rdan eliminatio끄 (gaussj上 and then by LU decomposit幻n
     with forward and backsubstitution (ludcmp and lubksb). Several linear sys-
     terns of special form, represented by tridiagonal, band diagonal, cyclic, Van-
    dermonde, and Toeplitz matrices, may be treated with procedures tridag,
    bandec, cyclic, vander, and toeplz respectively. Cholesky decomposition
    (choldc and cholsl) is the preferred method for symmetnic positive definite
    systems. QR decomposition (qrdcmp) is less efficient than LU decomposition
    in general; however, the ease with which it is updated (qrupdt) if the sys-
    tern is changed slightly makes it useful in certain applications. For singular
    or nearly singular matrices the best choice is singular value decomposition
    with backsubstitution (svdcmp and svbksb). Linear systems with relatively
    few non-zero coefficients, so-called "sparse" matrices, are handled by routine
    linbcg. A suite of routines for manipulating general sparse matrices, sprsa兀
    spstx, etc., is provided.



    gaussj performs Gauss-Jordan elimination with full pivoting to find the solution
of a set of linear equations for a collection of right-hand side vectors. The demon-
stration routine xgaussj checks its operation with reference to a group of test input
matrices printed at the end of this chapter asfile matrxl.dat. Each matrix is sub-
jected to inversion by gaussj, and then multiplication by its own inverse to see that
a unit matrix is produced. Then the solution vectors are each checked through multi-
plication by the original matrix and comparison with the right-hand side vectors that
produced them.

／卞 Driver 如r routine gaussj 中／

#include <stdio .h>
#inc].ude <stdlib. h>
#inc]끄de "nr. h1'
#inc].ude "nrutil. h"

#define 甘P 20
#define MP 20
#define MAXSTR 80

ml1t main(void)
{
    ml1t j, k, ].,m,n;
                                             Ch랴升er 2: Linear A勾ebraic Equa加ns   7

float 牛本a, *卞ai, 李本U, 卞卞b, 卞李X144t;
char du工my E!VXSTR] ;
FILE *fp;

a=matrix (1,NP,1,NP) ,
ai=matrix (1,NP,1,NP) ;
u=matrix (1,NF,1,NP) ;
b=matrix(1,NP, 1,MF) ;
x=matrix (1,NP,1,XP) ;
t=matrix (1, 甘F느 1，겨［F) ;
if ( (fp = fopen( "matrxl.dat ", "r ") ) == NULL)
    nrerror ( "Data file matrxl.dat not 如und\n") ;
while (! feof (fp) ) {
     fgets (d山nmy,MAXSTR, fp) ;
     fgets (dummy,MAXSTR, fp) ;
     fscanf (fp, "%d 'hd ", &n,&m) ;
     fgets (dummy,MAXSTR, fp) ;
    for (krl; k<=n;k++)
         for (l=1;l< =n;l+ +) fscanf (fp, "/.f ', &a[k] El] );
     fgets (dummy, MAXSTR , fp) ;
    for (1=1;l<=m; l++)
         for (k=1;k<=n;k++) fscanf (fp, ' 工f ', kbEk] [l] );
     /卞 save matrices for later testing of results 卞/
    for (l=1;l< 'n; l+ +) {
         for (k '1;k<=n;k++) ai[ k] [l] =a[k] [1] ;
         for (k=1;k<=m;k++) xll] [k] =bll] 1k] ;
    }
    ／李 invert matrix 牛／
    iauss1(ai .n. x . nl) :
    printf ( "\ nlnverse of matrix a : \n") ;
    for (k=1;k< 'n;k++) {
         for (1=1;l<=n;l+ +) printf ( " 工12. 6f ", ailk] Cl] );
         printf ( "\ n"') ;
    }
    ／本 check inverse 衣／/
    printf ( "\ na times a-inverse: \n") ;
    for (k=1;k<=n;k++) {
        for (1=1;l<=n;l+ +) {
              u[k] Cl] =0. O;
              for (j=1; j<=n; j++)
                  ulk] [l] += (a[k] 口] *ai[ j] 11] );
         }
         for (l=1;l< =n;l+ +) printf ( "/,12. 6f ", u[k] [l] );
         printf ( "\ n ') ;
    }
    /小 check vector solutions */
    printf ( "\ nCheck the following for equality: \n") ;
    printf ( "'/.21s V.14s\n", "original ", "matrix*sol'n") ;
    for (l=1;l< =m; l++) {
        printf ( "vector %2d: \n", l) ;
        for (k=1;k<=n;k++) {
              t[ k] El] =O. O;
              for (j=1; j<=n; ji-+)
                    珏kl [1] += (aEk] 口］李x[ j] [1] ) ;
              printf ( "/,Ss %12. 6f '/.12. 6f\ n", " "
                    blk] (l] ,t[ k] [1] );
         }
8       N미ne欣：a/ 尸ec枷＄Examp旭 Book

         }
         printf ("                                        \n") ;
         printf ("press RETURN for next problem: \n") ;
         (void) getcharO;
    }
    fclose(fp) ;
    free_matrix(t, 1,NP, 1,MP) ;
    free_matrix (x, 1,NP, 1,MP) ;
    free_matrix (b, 1 ,NP. 1,MP) ;
    free_matrix (u, 1,NP, 1,NP) ;
    free_matrix(ai, 1,NP,1,NP) ;
    free_matrix (a. 1,NP, 1,NP) ;
    return 0;



    The demonstration program for routine ludcmp relies on the same package of
test matrices, but just performs an LU decomposition of each. The performance
is checked by multiplying the lower and upper matrices of the decomposition and
comparing with the original matrix. The array mndx keeps track of the scrambling
done by ludcmp to effect partial pivoting. We had to do the unscrambling here, but
you will normally not be called upon to do so, since ludcmp is used with the routine
lubksb, which knows how to do its own descrambling.
/* Driver for routine ludcmp */

*include <stdio.h>
*include <stdlib. h>
#include "nr. h"
#include "nrutil. h"

#define NP 20
#define MAXSTR 80

ml1t main(void)
{
    mllt j, k, l, m,n,dU皿1卞mnd工14jlld工；,
    float d, 卞中a, 中＋xl, 卞卞工｝1, 卞*工；
    cha工 d山nmy [NAXSTR] ;
    FILE *fp;

    indx=ivector (1,NP) ;
    jndx=ivector (1,NP) ;
    a=matrix( 1, 甘P 'l , 甘P) ;
    xl=inatrix (1,NP, 1,5?);
    xu=matrix(1, 甘P, 1,NP) ;
    x=ntatrix (1,NP,1,NP) ;
    if ( (fp = 如pen( "matrxl.dat ", "r ") ) == NULL)
        nrerror ( "Data file matr工l.dat not found\n") ;
    while (! feof (fp) ) {
         fgets (dummy,MAXSTR,fp) ;
         fgets (du口my，甘A工S丁R, fp) ;
         fscanf (fp, "Y.d Xd ", kn,kin) ;
         fgets (d山口皿y,NAXSTR, fp) ;
         for (k=1;k<=n;k++)
              for (1=1;l<=n;l++) fscanf (fp, "%f ", &a(k] [ll) ;
         fgets (dummy ,MAXSTR,fp) ;
                                         Ch카）ter 2: Linear Algebraic Equations   9

for (1=1;1<=m;l+ +)
     for (k=1;k<=n;k++) fscaiii(fp, "/.f ", &x[k] [l] );
/* Print out a-matrix for comparison with product of
   lower and upper decomposition matrices */
printf ( 'original matrix: \n") ;
for (k=1;k<=n;k++) {
    for (1=1;l< =n;l++) printf ( "/.12.6f ", aEk] [l] );
    printf ( "\ n") ;
}
1京 Perform the decomposition 卞/
ludcmp(a,n,indx,&d) ;
/卞 Compose separately the lower and upper matrices 卞/
for (k=1;k<=n;k++) {
    for (1=1;l<rn; l+ +) {
        if (1 > k) {
            xu[k] [l] =a[k] [1] ;
            xl[ k] [13=0. 0;
        } else if (1 < k) {
            xu[kj [l] =0.0;
            xl[ k] [l] 'a[ k] [1] ;
        } else {
            xu[k] [l] =a[k] [1] ;
            xl[ kJ[l] =1.0;
          }
     }
}
/李 Compute product of lower and upper matrices for
   comparison with original matrix */
for (k=1;k<=n;k++) {
    jndx[k] =k;
    for (1=1;l<=n;l+ +) {
        x[k) [13=0.0;
        for (j=1; j<=n; j++)
             虹k] [1] += 佃1[kj [j］本工u[ j] [1] ) ;
     }
3.
printf ( "\ n%s佃\n" ,"product of lower and upper
      "matrices (rows unscrambled) :") ;
for (k=1;k<'n; k++) {
    dum= jnd虹in缸 [k끄 ;
    jndx[ind玎k끄 =jnd虹幻 ;
    jnd工 [k] =du皿；
3.
for (k=1;k<=n;k++)
     for (j=1; j<=n; j++)
         if (Jndx[ j] == k) {
             for (1=1;l< =n;l+ +)
                  printf ( "%12. 6f ", x[ j] []j) ;
             printf ( "\ n") ;
          3.
printf ( "\ nlower matrix of the decomposition: \n") ;
for (k=1;k<=n;k++) {
    for (l=1; ].<=n;l+ +) printf ( "%12. 6f ", xl[ k] 口] );
    printf ( "\ n") ;
3.
printf ( "\ nupper matrix of the decomposition: \n") ;
for (k=1;k<=n;k++) {
10      Numerical Recipes Example Book

              for (l=1;l< =n;l++) printf ( "%12. 6f ", xu[k] [l] );
              printf ( '\ n") ;
         }
         printf ( "\ n卞京京本中卓李李卞牛卞字中卞卓* 字卞卓李京卞京京卞字方卞本李卞中京卓方＼n') ;
         printf ( "press return for next problem: \n") ;
         (void) getcharO;
     }
     fclose(fp) ;
     free_matrix (x, 1,NP, 1,NP) ;
     free_matrix(xu, 1, 甘P, 1,NP) ;
     free_matrix (xl, 1,NP, 11 NP) ,
     free_matrix (a,1,NP 11,NP) ;
     free_ivector (jndx,1,NP) ;
     free_ivector (indx,11 NP) ;
     return 0;
)

    Our example driver for lubksb makes calls to both ludcmp and lubksb in order
to solve the linear equation problems posed in file matrxl .dat (see discussion of
                                                                                vectors to
gaussj). The original matrix of coe佈cients is applied to the solution
check that the result matches  the right-hand   side vectors posed  for each problem.  We
           for using routine ludcmp   in a test of lubksb,   but ludcmp   has been  tested
apologize
independently, and anyway, lubksb is nothing without this partner program, so a
test of the combination is more to the point.
／京 Driver 如r routine lubksb 卓／

#include <stdio.h>
#include <stdlib. h>
#include "nr.h"
#include "nrutil. h"

#dafine NP 20
#define MAXSTR 80

mnt main(void)
{
     mllt j, k,1,m,n, *indx;
     float p, *X, 方京a, 半卓b1衣巾C;
     char dummy [MAXSTR] ;
     FILE *fp;

     indx=ivector (1,NP) ;
     x 'vector ( 1, NP) ;
     a=matrix (1,NP,1,NP) ;
     b=ma缸ix (1, 甘P .1 , 朴0 ;
     c=matrix (1,NP,1,NP) ;
     if ( (fp = fopen( "matrxl.dat ", "r ") ) == N兀L)
          nrerror ( "Data file matrxl.dat not found\n") ;
     日hile (! feof (fp) ) {
         fgets (du皿my,MAISTR, fp) ;
         fgets (dummy, MAXSTR. fp) ;
         fscanf (fp, "%d%d ", &n,km) ;
         fgeta (duma呵, MAXSTR,缸) ;
         for (k '1;k<=n;k++)
              for (1=1;l<=n;l+ +) fscanf (fp, "%f ", ka[k3[l] );
                                                 Ch카）旭r2: L加ear A勺ebraic Equations   11
            fgets (dummy,MAXSTR,fp) ;
            for (l= 1;l<=m; l++)
                 for (k:rl; k<=n;k++) fscanf (fp, "%f ", kb[k] [l] );
           1中 Save matrix a for later testing */
            for (1=1;l< =n;l++)
                 for (k=1;k<=n;k++) c[k) [l] =a[kj [1] ;
           /卞 Do LU decomposition */
           ludcmp(c, n,indx, &p) ;
           /中 Solve equations for each right- ha끄d vector 中/
           for (k=1;k<"m;k++) {
                for (1=1;l< =n;l++) xtl] 'b[ l] (k] ;
                lubksb(c,n, ind工 , 工） ;
                /中 Te8t results with original matrix 卞1
                printf ( "right- hand side vector: \n") ;
                for (l '1; l<=n;l++)
                     printf ( "%12. 6f ", b[l] [k] );
               printf ( "\ n/.s%s\n" ,"result of matrix applied",
                     " to sol'n vector ") ;
                for (l=1;l<=n;l++) {
                     b[l) [k] =0.0;
                    for (j=1; j<=n; j++)
                        b[l] [kj += (a[l] [j］中工口］) ;
               }
               for (l=1;l<'n; l+ +)
                   printf ( "%12.6f ", b(lj[ kj) ;
               printf ( "\ n                                      \n ') ;
          }
          printf ( "press ItETURN for next problem: \n") ,
          (void) gatcharO;
     }
     fclose(fp) ,
     free_matrix (c, i ',NP, 1,JP) ;
     free4matrix(b, 1,NP, 1,NP) ;
     free. matrix (a,1,NP,1,NP) ;
     frea..vector (x . 1,甘?);
     freemivactor (indx, i, NP) ;
     return 0;
:J

    Procedure tridag solves linear equations with coefficients that form a tridiag-
onal matrix. We provide at the end of this chapter a second file of matrices ma-
trix2 .dat for the demonstration driver. In all other respects, the demonstratio
                                                                                  n
program xtridag operates in the same fashion as xlubksb.
I中 Driver for routine tridag s/

*includa <stdio.h>
#include <stdlib . h>
#includa "nr. h"
#include "nrutil. h"

*define NP 20
*4口fine MA工STR 80

milt main(void)
{
     linsi酊ied long 瓦ll;
12       Numerical Recipes Example Book

     float 牛diag, 本superd1卞subd, *rhs,卓U;
     char dusuny[MAXSTR] ;
     FILE *fp;

     diag=vector (1,NP) ;
     superd=vector (i , 肛) ;
     subd=vector (i ,NP) ;
     rhs=vector (i, NP) ;
     u=vector (1,NP) ;
     if ( (fp = fopen( 'matrx2.dat ", 'r ") ) == NuLL)
         nrerror ( 'Data file matrx2. dat not found\n") ;
     while (! feof (fp) ) {
          fgets (du皿my,MAXSTR, fp) ;
          fgets (duinlny,MAXSTR, fp) ;
         fscanf (fp, "%ld ", &n) ;
         fgets (duituny,MAXSTR,fp) ;
         for (k=1;k<=n;k+i- ) fscanf (fp, "%f ", kdiag[k] );
         fgets (dumnty,MAXSTR, fp) ;
         for (k 'i; k<n;k++) fscanf (fp, "%f ", ksuperd[k] );
         fgets (dummy,MAXSTR, fp) ;
         for (k=2;k<=n;k++) fscanf (fp, "Y.f ' .ksubd[k] );
         fgets (d山my,NAXSTR, fp) ;
         for (k=1;k<=n;ki-+) fscanf (fp, "V.f ', trhs[ k1) ;
         Is carry out solution 中/
         tridag (subd,diag, superd,rhs,u,n) ,
         printf ( "\ nThe solution vector is: \n") ;
         for (k=1;k<=n;k++) printf ( "%12. 6f " , u[k] );
         printf ( "\ n") ;
         ／牛 test solution 卞／
         printf ( "\ n(matrix) *(sol 'n vector) should be: \n") ;
         for (k=1;k<=n;k++) printf ( '%12.6f ", rhs[k] );
         printf ( "\ n") ;
         printf ( "actual result is: \n") ;
         for (k=1;k<=n;k++) {
              if (k == 1)
                   rhs[k] =diag[i] *u[1] +superd[i] 中u[2] ;
              else if (k == n)
                   rh町目=sub町n] 치山i-i] +diag［幻 京町n] ;
              else
                   rhs [k] = subd [k] *u[k- i] +diag [k] 牛u [k]
                        +superd[k] *u[k+i] ;

          。r (k=1;k<=n;k++) printf ( "%12. 6f ", rhs[k] );
         f}
         printf ( "\ n") ;
         printf ( "李卞＋牛中卞京卓李中本卞卞卓本中卓卞中*中中本卞卓中卞方卞京卞卞斗卞衣＼n') ;
         printf ( "press return for next problem: \n") ;
         (void) getcharO;
     }
     fclose(fp) ;
     free4vector (u, i ,NP) ,
     free.= vector (rhs, 1,NP) ;
     free1vector (subd, i , NP) ;
     free_ vector (superd, 1,NP) ;
     free4vector (diag,1,NP) ;
     return 0;
}
                                                  Ch카升cr2: LinearA勺ebra七 Equat幻Us   13

    The demonstration program xban皿ul forms a banded matrix, multiplies if by a
vector using banmul, and compares the answer to the result of carrying out a full
matrix multiplication.
／中 Driver 如r ro1工tine banrnul */

#include <stdio.h>
*include "nr. h"
*include "nrutil. h"

#def ins 甘P 7
#def ins Ml 2
#def ins 片2 1
#define NP (M1+1+M2)

mnt main(void)
{
        1끄lsigned long i, j, k;
        float 字衣a, 卞＋aa, 卞a工1卞b1卞工；

        a=matri工 (1, 丑P .1,MP) ;
        aa=matrix (1, 丑P,1,NP) ;
        a工＝vector (1, 甘P) ;
        b=vector (1, 甘P) ;
        工＝vector (1, 丑P) ;
        for (i=1; i<=N1; i++) for (j=1; j<=NP; j++) a[ j] [i] =10. O* j+i;
        /* Lo日er ba끄d 卞／
        for (i=1; i<=NP; i++) a[i] [M1+1] "i;
        ／卞 Diagonal 卞／
        for (i=1;i<=M2; i++) for (j= 1; j<＝甘P; j++) a[ jl[ 片i+1+i] =O. 1*j+i;
        ／中 Upper ba끄a +/
        如r (i= 1; i<＝且P; i++) {
            for (j=1; j<'NP; j++) {
                k=i- M1-1;
                if (j> =LMAX (1,1+k) U j<=LMIN(M1+M2+1+k, 甘P) )
                 aa[i] [j) =a[i] [j- k] ;
                 else aa[i] [j] =O. O;
             }
        }
        for (i=1; i<=NP; i++) x[i] =i/ 10. O;
        baniaul(a,NP,M1,M2, 工,b) ;
        for (i=1; i<=NP; i++) (
             for (ax[i] =O. O, j=1;J<=NP; j++) a工[i)    += aa[i] [j:]*x[ j] ;
        }
        printf ( "\ t1eference vector\tbamnul vector\n ') ;
        for (i=1; i<=NP; i++) printf ( "\ t%12. 4f\ t/.12.4f\ n", ax[i] ,b[ i] );
        free_ vector (工, 1,NP) ;
        free_ vector (b,1,NP) ;
        f ree_ vector (ax , 1, 甘P) ;
        free_matrix (aa, 1,甘P, 1,NP) ;
        free_matrix (a, 1 ,N?, 1,MP) ;
         retm그L0,
    }

        The sample program xbandec forms a random banded matrix A, a random vector
    x, and calculates b = A · x. It then supplies A and b to bandec and baxibks and
    compares the solution to the saved copy of x.
    14       Num아切／尸ec巾es Exa쨔出Book

/* Driver for routine bandec */

#include <stdio.h>
*include "nr. h"
#include "nruti] . . h "

ml1t mamn(void)
{
         float 미*卞a, 卞卞al,卞b, *x;
         unsigned long i, J, *indx;
         long iduin=(- 1) ;

         a=jsatri工 (1,7,1,幼 ;
         x=vector (1,7) ;
         b=vector (1,7) ;
         al "matrix (i, 7,1,2) ;
         indx"lvector (l ,7) ;
         for (i=1; i<=7;i++) {
              x［幻 =ra끄i (&idum) ;
              for (j=1; j<=4; j++) {
                   aLi] [j] =ran1(kidum) ;
              }
         }
         banmul(a,7,2,1, x,b) ;
         for (i=1;i<=7; i++) printf ( "/.ld 工12. 6f %12. 6f\ a", i, b[ i] ,x[ i] );
         b띠idec(a,7, 之 1,al, in缸 ,&d) ;
         b키ibks(a.乙 긱 1 小l, ind치b) ;
         for (i=1; i<"7; i++) printf ( "%ld 工12. 6f %12. 6f\ n ", i, b(i] ,x[ i] );
         free_lvector (indx,1,7) ;
         fr ee_matrix (al, 1,7,1,2) ;
         free_vector (b,1,7) ;
         f roe_ vector Cx , 1, 7) ;
         free_niatrix (a,1,7,1,4) ;
         return 0,
}

     mprove is a short routine for improving the solution vector for a set of linear
equations, providing that an LU decomposition has been performed on the matrix
of coe佑cients. Our test of this function is to use ludcmp and lubksb to solve a
set of equations specified by the initializations at the beginning of the program. The
solution vector is then corrupted by the addition of random values to each component.
mprove works on the corrupted vector to recover the original. Note the use of the
utility routine convert_matrix () to change a conventionally defined matrix to the
format used in Numerical Recipes.
/t Driver for routine mprove 卞/

#include <stdio.h>
#include "nr. h"
#include "nr比il. h"

#define N S
*define NP N

mnt main(void)
{
                                            Ch랴ter 2: Linear Algebraic Equations    15

    mllt i, j, *indx;
    long idu皿＝（느13) ;
    fl oat 미＋工 1卞＋a, 李牛aa;
    static float ainit[ NP] [NP] =
         (1. 0,2. 0,3.0,4.0,6.0,
         2. 0, 3. 0,4.0,5.0,1.0,
         1.0 'l. o,l. o,l. o,l. o,
         4. 0,5. 0,1.0, 2. 0,3.0,
         6. 0, 1. 0, 2.0,3. 0,4. 0} ;
    static float b[N+1J={0.0,1.0,1.0,1. 0,1.0,1.0} ;

    mlld工＝iv日ctor (1,N) ;
    x=vector (1,N) ;
    a=convert_matrix伍amnit (0J (0] , 1,N, 1,1) ;
    aa=matri工 ( 1, 瓦 1,N) ．·
    for (i= 1; i<=N; i++) {
         玎幻 =b[i] ;
        for (jrl; j<=N; j++)
            aa[i] Ej] =ati] [j] ;
    }
    ].udcmp(aa,N, indx,&d) ;
    lubksb(aa,瓦m d工 , I) ;
    printf ( "\ nSolution vector for the aquation8: \n") ;
    for (i= 1; i<=N; i++) printf ( "/,12.6f ", x[i] );
    printf ( "\ n") ;
    ／中 no므 phoney up 工 카id let mprove 11工 it 字／
    如r (i= 1; i <=!; i++) 工［3.] 卞＝ (1.0+0 . 小ra必（&idu皿）) ;
    printf ( "\ nSolution vector 日ith noise added: \n") ;
    for (i= 1; i<rN; i++) printf ( 'V.12.6f ", x[i] );
    prmntf ( "\ n") ;
    mprove(a,aa, 瓦 in缸巾J) ;
    printf ( "\ nSolution vector recovered by mprove: \n') ;
    for (i= 1;i<=N; i++) printf ( "/.12.6f ". x[i] );
    prmntf ( "\ n") ;
    free_matrix (aa, 1,N, 1,1) ;
    fre하convert_mat工3.工 (a,1, 瓦 1,I) ;
    free_ vector (x, 1,N) ;
    free_ ivector (indx,1,N) ;
    return 0;
}

     The pair svdcmp, svbksb is tested in the same manner as ludcmp, lubksb. That
is, svdcmp is checked independently to see that it yields proper decomposition of
matrices. Then the pair of programs is tested as a unit to see that it provides correct
solutions to some linear sets. (Note: Because of the order of programs in Numerical
Recipes, the test of the pair in this case comes first).
    Driver xsvbksb brings in matrices a and right-hand side vectors b from ma-
trxl. dat. Matrix a, itself, is saved for later use. It is copied into matrix u for
processing by svdcmp. The results of the processing are the three arrays u, w, v which
form the singular value decomposition of a. The right-hand side vectors are fed one
at a time to vector c, and the resulting solution vectors x are checked for accuracy
through application of the saved matrix a.
 16      Numerical Recipes Example Book

/中 Driver for routine svbksb, which calls routine svdcmp */

#include <stdio .h>
#include <stdlib. h>
#include "nr. h"
#inclnde "nrutil. h"

#define NP 20
#defina NP 20
#define MAXSTR 80

ml1t main(void)
{
     jut j, k, l, m,n;
     float wma工1mni兀卓日1中工, *c;
     float; 卞4a 1 字中b,＋中U, 本卞V ;
      char d口awy ENAXSTR] ;
      FILE *fp;

      w=vector (1,NP) ;
      x=vector (1,NP) ;
      c=vector (1,NP) ;
      a=matrix (1,NP, 1,NP) ;
      b=matrix (1,NP, 1, MP) ;
      u=matri工（1,NP,1. 甘P) ;
      v=matrix (1,NP,1,NP) ;
      if ( (fp = fopen( "matrxl.dat ", "r ") ) == NULL)
          nrerror ( "flata file matrxl.dat not found\n") ;
      while (! feof (fp) ) {
           fgets (du皿ay,MAXSTE, fp) ;
          fgets (dmamy,NAXSTR, fp) ;
          fscanf (fp, "I,d %d ' ', &n,&m) ;
          fgets (dunuay,NAXSTR, fp) ;
           for (k=1;k<=n;k++)
               for (lrl; l<rn; l+ +) fscanf (fp, "/.f ", ka[k] [l] );
           fgeta (dumy,MAXSTR, fp) ;
           for (l=1;l<=m; ].++)
               for (k=1;k<'n; k++) fscanf (fp, "/.f ' , kb[k] [l] );
           /* copy a into U 巾／
          for (k=1;k<=n;k++)
               for (1=1;l< =n;l++) ulk] [l] =a[k] [1] ;
          ／中 decompose matri工 a 卓／
           svdcmp(u,n,n,日, v) ;
          ／卓 find ma工mmu皿 singular value s/
          甘ma工＝0. 0;
          for (k=l; k<=n;k++)
               if （口［k] > 日ma幻 wma工＝町k] ．·
           /* define ' 'small ' */
          日mmll＝日ma工卞 ( 1. oe-6) ·,
           /* zero the "small" singular values 巾/
          for (k=1;k< rn;k++)
               if （町k] < 日mmn) 叭k] =0.0·    ．
           /t backsubstitute for each right- hand side vector */
           for (1=1;l< =m; l++) {
               priatf ( "\ nVector nu皿ber X2d\n", l) ;
               for (k=1;k<=n;k++) c[k] "b[k] [l] ;
               svbksb(u,w, v,n,n, c, x) ;
                                             Ch햐ter 2: Linear A勾ebra七 Equat幻ns     17

             printf ( " solution vector is: \n") ;
             for (k=1;k<=n;k++) printf ( "%12.6f ' , x[k] );
             printf ( '\ n original right- hand side vector: \n ') ;
             for (k=1;k<=n;k++) printf ( " 工12. 6f ' , c[kl) ;
             printf ( "\ n (matrix) *(sol 'n vector) :\n ") ;
             for (k=1;k<'n; k++) {
                 c [k] =0. 0;
                  for (j=1; j<=n; j++)
                      c [k] += 町k] Cj］方工［j] ;
             }
             for (k=1;k<=n;k++) printf ( 'Y.12. 6f ", c[k) );
             printf ( "\ n") ;
        }
        printf   ("                                         \n") ;
        printf ( "press RETURN for next problem\n") ;
        (void) getcharO;
    }
    fclose(fp) ;
    free.jnatri工(v, 1,NP, 1,NP) ;
    free_matrix (u. 1,NP, 1,NP) ;
    free..matri工(b, 1,NP, 1,NP) ;
    free_aatrix (a. 1,NP, 1,NP) ;
    freeevect口r (c, 1 ! 甘P) ;
    free_ vector（工 ,1 ! 甘P) ;
    free_ vector (w, 1,NP) ;
    return 0;
}

    Companion driver xsvdcmp takes the matrices a from matrx3 .dat The rather
pathological test matrices for xsvdcmp are given in the Appendix as file matrx3 .dat.
The routine reads each matrix a in and passes a copy of each to svdcmp for singular
value decomposition into u, w, and v. Then 11, w, and the transpose of v are multiplied
together. The result is compared to a saved copy of a.
/* Driver for routine evdcmp */

#include <stdio . h>
#include <etdlib. h>
#include "nr. h'1
#includa "nrutil. h"

#define NP 20
#define NP 20
#def ins N且工STE 80

mnt main(void)
{
    mllt j, k, l, m.n;
    float 中日1卞Ca, 京Cu,＋牛V;
    char dummy [MAXSTR] ;
    FILE *fp;

    w=vector (1,NP) ;
    a=matri工 ( 1,NP, 1,月P) ;
    u=matrix (1,MP,1,JP) ;
    v=matri工 (1,NP,1,月P) ;
    /s read input matrices     巾／
18        Num帥Ca샤？的加＄Examp旭 Book

     if ( (fp = fopen( "matrx3.dat느 "r ") ) == NULL)
         nrerror ( "Data fi le matrx3.dat not 如und\n") ;
     while (! feof (fp) ) {
         fgets (dunuuy,MAXSTR, fp) ;
         fgets (dmnmy,거［AXsTR, fp) ;
         fsc카lf (fp, "%d %d ", km,kn) ;
         fgets (d山uny,MAXSTR,fp) ;
          /s copy original matrix into u 卞1
         for (kr1;k<=m;k++)
              for (l=1;l<=n;l++) {
                   fscanf (fp, "%f ", kaCk] [l] );
                  u[k] [l] =a[k] [1) ;
               }
          /s perform decomposition */
          svdcmp(u,m,n,甘, v) ;
          ／方 日rite results 中／
          printf ( "Decomposition matrices: \n") ;
          printf ( "Matrix u\n") ;
          for (k=1;k<=m;k++) {
              for (1=1,l<=n;l++)
                    printf ( "%12.6f ",u[k3[l] );
              printf ( "\ n") ;
          }
          printf ( "Diagonal of matrix 日\n") ;
          for (k=1;k<=n;k++)
              printf ( '%12. 6f ",町k] );
          printf ( "\ nMatrix v-tr키lspose\n") ;
          for (k=1;k<=n;k++) {
              for (l '1;l<=n;l++)
                    printf ( "Y.12. 6f ", v[l] [k) );
              printf ( "\ n") ;
          }
          printf ( "\ nCheck product against original matrix: \n") ;
          printf ( "Original matrix: \n") ;
          for (k '1;k<'m;k++) {
              for (1=1;l<=n;l++)
                    printf ( "%12. 6f ", a[k3[l] );
              printf ( "\ n") ;
          }
          printf ( "Product usw卓(v-transpose) :\n") ;
          for (k=1;k<=m;k++) {
              for (1'l; l<=n;l++) {
                    aCk] Cl] =0. O;
                    for (j=1; j<=n; j++)
                        缸k] [1] += 町k] [j] sw口］方V口］Ci] ;
              }
              for (1=1;l<=n;l++) printf ( "7.12.6f ", a[k]口] );
              printf ( "\ n") ;
          }
          printf C "＋中卞李＋＋卞卞中卓＋*5中卞＋方卞＋*巾＋字布卞卞中＋中卞＋亡卞＋中＼n,') ;
          printf ( "press RETURN for next problea\n") ;
          (void) getcharO;
     }
     fclose(fp) ;
     free_matrix (v, I ,NP, 1,月P) ;
     free_matrix (u, I, MP, l. 月P) ;
     free느matri工(a, I 1MP 11,甘p) ;
                                              Ch邵）ter2: LinearA勺ebra元 Eq｛坦f幻ns         19

    free_ vector (v, 1,NP) ;
    return 0;
}

    A cyclic tridiagonal matrix is just like a tridia.gonal matrix, but with additiona
nonzero elements in the top right and bottom left corners. Sample program xcyc1i(
generates a random cyclic tridiagonal matrix and right-hand side vector. It then call
cyclic to solve the resulting linear system. The solution is checked by also so1vin!
the system with ludcmp and lubksb and printing out the fractional discrepancy ii
the answer.
/卓 Driver for routine cyclic 李/

#include <stdio . h>
#include "nr. h"
#include "nrutil .h"

#define 甘 20

mllt main(voict)
{
    float alpha,beta,d,*a.*b.*c, 方r,中工1卞＋aa;
    mllt i. j, *indx;
    long idu皿＝(- 23) ;

    mnd工＝ivector (1,助 ;
    a=vector (1,N) ;
    b=vector (1.E;
    c=vector (1,N) ;
    r "vector (i, N) ;
    x=vector (1,N) ;
    aa=ina竹i工（1, 瓦 i. E ;
    如r (i=1;i<＝甘；i++)
        for (j=1; j<=月; j++) aaCi] Cj]=0.0;
    for (i "l; i<=N; i++) {
        t江口 =ran2(kidu미 ;
        aaCi] Ci] =b[i] ;
        r ［幻 =ran2(kidu工）;
    }
    for (i=1; i <N; i++) {
        町i+ j] =ran2(&idu미 ;
        aa[i+1] [i] =a[i+1] ;
        c Ci] "ran2(&idu皿) ;
        aati] [i+ 1] =c[ j] ;
    }
    alpha=ran2(&idu皿) ;
    aa 田］口］=alpha;
    beta=ra끄2 (&idu皿）;
    aa[i] EN] =beta;
    cyclic (a,b, c,alpha,beta,r, x ,N) ;
    ludcmp(aa,N, indx .&4) ;
    lubkeb(aa,瓦 indx,r) ;
    for (i= i; i<=N; i++) printf ( "工4d %12. 6e\n", i, (xEi]-r[ i] )/(xCi] +r[i] ));
    fre乞matri工（aa. 1,瓦 1,N) ;
    free_ v吼如r（工 .1,1) ;
    fre日_ Vect乙r (r, 1, 甘）;
20       Numerica／尸0（和es Examp旭 Book

     free_vector (c, 1,N) ;
     free_vector (b, 1,N) ;
     free_ vect口r (a.1 . 甘）;
     free_ ivector (indx,1,N) ;
     return 0;
}

    Next follow the routines for testing the sparse matrix routines. The first, xsprsin,
takes the matrix defined in Equation (2.7.27) of Numerical Recipes, prints out the
corresponding ij a and sa vectors (which you can check against Equation 2.7.28), and
then reconstructs the matrix from these vectors.
/* Driver for routine sprsin */

#include <stdio . h>
#include "nr. h1'
#inc].ude "nrutil. h"

#define NP 5
#define 표MAX (2半NP本NP+1)

m11t main(void)
{
     unsigned long i, j, msize, *ija;
     float; 京Ca, 半卞aa, 京sa;
     static float ainit [NP] 대P] =(
         3. 0,0.0,1.0,0. 0,0.0,
         0.0,4.0,0.0,0.0,0. 0,
         0. 0,7. 0,5. 0,9. 0,0. 0,
         0. 0,0. 0,0.0,0. 0, 2.0,
         0 . 0,0.0,0.0,6 . 0,5. 0} ;

     幻a=lvector ( 1，且MAX) ;
     sa=vector (1, 甘甘AX) ;
     aa'matrix (l ,NP, 1,1W) ;
     a=convert_inatrix(kainit[ 0] [0] ,1,NP,1,NP) ;
     sprsin(a,NP, 0.5,NMAX 戶a,ija) ; "
     insize=ija[ ija[ 1] -1] -1;
     sa[NP+1] =0.0;
     printf ( "index\tija\ t\ tsa\n") ;
      for (i=1; i<=insize;i++) printf ( "/.lu\ t工lu\t%12.6f\ n", i. ija[ i] ,sa[il) ;
     for (i=1;i<=NP; i++) for (j=1; j<=NP; j++) aa[i] [j] =0.0;
     for (i=1; i<=NP; i++) {
          aa[i] [i] =sa[i] ;
          如r (j= ija[ i] ; j<=ija[ i+1] -1; j++) aa[i] 口戶[ j끄＝8缸3] ;
     }
     printf ( "Original Matrix\n") ;
     for (i "l; i< 'NP; i++) {
         for (j=1; j<"NP; j++) printf ( "%5.2f\ t ", a[i] [j] );
         prmntf ( "\ n") ;
     }
     printf ( "Reconstructed Matrix\n") ;
     for (i= 1; i<=NP; i++) {
         for (j '1; j<=NP; j++) printf ( "/.5.2f\ t ", aa[i] [j] );
         printf ( "\ n") ;
     }
     fre已convert_rn毗rix (a, 1小已 1,NP) ;
                                           Gh카）旭r 2: Linear A勺ebra石 Equal幻ns       21

    free_matrix (aa, 1, 甘P, 1,NP) ;
    free. 叱ctor (ea, 1, 때上X) ;
    free._lvector (ija, 1,NNAX) ;
    return 0;
}

    Program xsprsax takes the same sparse matrix and multiplies it by the vector
(1,2同4,5) using sprsax. It compares the result to that of a full matrix multiplication.
/／中 Driver for routine sprsa工 中／

#include <stdio.h>
#include 1'ni .h"
#include 'nrutil. h"

#define NP 5
#define NMAX (2卓月p卞NP+1)

m1lt main(void)
{
    unsigned long i, 3,msize, *ija;
    float; 中＋a, 中Ba, 卞a工 1 卞b;
    static float ainit [NP] [NP] = {
        3. 0,0. 0,1. 0,0. 0,0. 0,
        0. 0,4. 0,0.0,0.0,0. 0,
        0. 0,7. 0,5.0,9.0,0. 0,
        0. 0,0. 0,0.0,0. 0, 2.0,
        0.0,0 . 0, 0. 0,6.0,5. 0} ;
    static float x[且P+1] = {0. 0,1.0, 2. 0,3. 0,4.0,5.0} ;

    ija= lvector (1,NMAX) ;
    ax=vector (1,NP)..
    b=vector (1,NP) ;
    sa 'vector (l, NMAX) ;
    a=convert_matrix (&ainit[ 0] [0] ,1, NP,1,NP) ;
    sprsin(a,NP, 0.5,N甘AX, sa,ija) ;
    msize=ija[ 1] -2;
    sprsa工佃a. 幻 a, x,b,msize) ;
    for (i=1; i<=msize; j++)
         for (ax[iJ=0. 0, j=1; j<=msize; j++) a工[i] += a[i] [j] sx[ j] ;
    printf ( "\ tReference\tsprsax result\ n") ;
    for (i=1; i<'tssize;i++) printf ( "＼너佰그叭t\t｝侃2f\ n" , a工［i] , 1江ii) ;
    free..convert_matrix (a, 1,NP, 1, 표P) ;
    free_ vector (sa,1, 甘HAX) ;
    free_ vector (b, 1,NP) ;
    free_ vector (a工, 1,NP) ;
    free_lvector (ija, 1,NMAX) ;
    return 0;
}

    Program xsprstx works in exactly the same way as the previous program to test
sprstx by computing the product of the transpose of the sparse matrix with the
vector:
／卞 Driver 如r routine sprst工 卞／

#include <stdio.h>
    22       Numeric酊尸ec加＄ Example Book

#include "nr. h"
#include "nrutil. h"

#d日士inc 甘P 5
#defizte NMAX (2卞且P才NP+1)

ml1t main(void)
{
         unsigned long i, j, maize, *ija;
         float ＋字a, 京Ba, Ca工, *b;
         static float ainit[ NP] [NP] ={
             3. 0,0. 0,1. 0,0. 0,0.0,
             0. 0, 4. 0,0. 0,0. 0,0. 0,
             0. 0,7. 0,5. 0,9. 0,0. 0,
             0.0,0. 0,0. 0,0.0,2. 0,
             0.0,0 . 0,0. 0 ,6. 0,5 . 0} ;
         static float x[NP+1] = {0. 0,1.0,2.0,3.0,4.0,5. 0} ;

         ija=lvector (1, 月片Ax) ;
         ax=vector (1,JP) ;
         b=vector (1, 月P) ;
         sa=vector (1, 甘MAX) ;
         a=convert中matrix (&ainit [0] [0] ,1,NP,1,朴) ;
         sprsin(a,NP, 0. 5,NMAX, sa, ija) ;
         msize"ija[ 1] -2;
         sprstx (sa,ija, x,b,msize) ;
         for (i= 1; i<"msiza; i++)
             for (ax[i] =0.0, j=1; j<=msize; j++) a工[i] += a[ j] [i] *x[ j] ;
         printf ( "\ tfteference\t町）rstx result\ n") ;
         for (i '=l; i<=msize;i++) printf ( "\ t%5. 2f\ t\ t艾5. 2f\ n", ax[i] ,b[ i] );
         free_ convert_matrix (a,1,片P, 1,NP) ;
         free_ v吼tor佃키 1,NMAX) ;
         free_ vector (b, 1,NP) ;
         free_ vector (ax, 1,1?);
         free_lvector (ija, 1,NMAX) ;
         return 0;
}

    Program xsprstp simply prints out the transpose of our sample sparse matrix
after calling sprstp:
/t Driver for routine sprstp */

#include <stdio . h>
#iuclude "nr. h"
*include "nrutil. h"

*define 丑P 5
*define N甘AX (2卞NP卞甘P+1)

jut main(void)
{
         unsigned long i, j, *ija, *ijat;
         float 方卞a,巾卞at , tea, teat;
         static float ajnit[ NP] [yp]={
             3.0,0.0,1.0,0.0,0.0,
             口 이4 力,0 . 이 0 刀,0. 0,
                                                  C/i邵片or 2: Linear A勾ebraic) 日刊計幻ns    23

          0. 0,7. 0,5.0,9. 0,0. 0,
          0. 0,0.0,0.0,0.0,2.0,
          0.0,0 . 0,0 . 0,6.0,5 . 0);

     i: ia=lvector (1,NMAX) ;
     i: iat=lvector (1,NMAX) ;
     sa=vector (1,NMAX) ;
     sat=vector ( 1, NMAX) ;
     at=matrix (1,丑P, 1,聊）;
     a=convert_matrix (&ainit[ 0] [0] , 1,NP, 1,NP) ;
     sprsin(a,NP, 0. 5,NMAX, sa,ija) ;
     sprstp(sa, ija, sat ,ijat) ;
     for (i "l; i<=NP; i++) for (j=1; j<=NP; j++) at[ i] [j] =0. 0;
     如r (i "l ; i <＝引가 j++) {
           at[ i] Ei] =sat[i] ;
          for (jrijat[   i] ;j< =ijat[ i+1] -1; j++) at[ i] [ijat[     j] ]=sat[ j] ;
     }
     printf ( "Original Matrix\n") ;
     for (i= 1; i<'NP;i++) (
         for (j= 1, j<"IiP; j++) printi ( "Y,5. 2f\ t ", a[i] [j] );
         printf ( "\ n") ;
     }
     printf ( "Tr키lspose\n") ;
     for (i=1;i<=NP; i++) {
          for (j "i; j<=NP; j++) printf ( "%5.2f\ t ", at[ i] [j] );
          printf ( "\ n") ;
     J.
     free_ convert_matrix (a,1,NP,1,NP) ;
     free_matrix(at, 1,NP, 1,NP) ;
     free_vector (sat , 1 ,EUX) ;
     free_ v吼tor 佃키 1,NMAX) ;
     free_lvector (ijat , 1,NMAX) ;
     free_lvector (ija, 1,NMAX) ;
     return 0;
3,
     The next program, xsprspm, demonstrates the USe of sprspm. Two sparse ma-
trices A and B are defined, and then the matrix A . B is comnuted. Since sDrsnm
actually calculates A·BT, we first form BT by a call to sprstp. Only a given sparsity
pattern is output by sprspm. In the example, we specify this to be the tridiagonal part
of A . B. As usual, we check the answer by carrying out a full matrix multiplication.
/中 Driver for routine sprspm *1

#incluile <stdio . h>
#include "nr. h"
#include "nruti] ..h"

寸del in白 NP 5
*daf in, 甘MAX (2*NP*MP+1)

mnt main(void)
{
     1끄isi叩led long i, j, 瓦卞ija，巾ijb,巾ijbt,寸1加；
     float *aa, *sb,巾sbt, *ac,**a, *sb,**c, **ab;
     Static float ainit[ NP] [IP] ={
          i. 0,0.5.0.0,0.0.o.0.
24        Numeric串尸ec徊es Example Book

         0 . 5, 2 . 0了0 . 5,0 . 0,0 .0,
         0. 0,0. 5, 3. 0, 0. 5,0. 0,
         0.0,0.0,0. 5,4. 0,0. 5,
         0 . 0,0 . 0,0. 0 , 0 . 5 , 5 .0} ;
     static float binit [NP] [NP] ={
         1. 0,1. 0,0.0,0. 0,0. 0,
         1. 0, 2. 0, 1. 0,0. 0, 0. 0,
         0.0,1. 0,3.0,1.0,0. 0,
         0. 0,0.0,1. 0, 4. 0,1. 0,
         0.0,0. 0,0. 0,1.0,5. 0} ;

     i3a=1vect0r (1,NMAX) ;
     ijb= lvector (1,NMAX) ;
     ijbt= lvector (1,NMAX) ;
     ijc口lvector (1,NMAX) ;
     sa=vector (1,NMAX) ;
     sb=vector (1,NMAX) ;
     sbt=vector (1,NMAX) ;
     scrvector (1,NMAX) ;
     c=matrix (1,NP,1,NP) ;
     ab=matrix (1,NP,1,NP) ;
     a=convert_matrix (kainit[ 0] [0] , 1,NP, 1,NP) ;
     b=convert_matrix (kbinit[ 0] [0] , 1,11? , 1, NP) ;
      sprsin(a,NP, 0. 5,NMAX, sa, ija) ;
      sprsin(b,NP, 0. 5,NMAX, sb, ijb) ;
      sprstp(sb,ijb, sbt,ijbt) ;
                                                                      京/
      /半 specify tridiagonal output, using fact that a is tridiagonal
      for (i=1; i<=ija[ ija[ 1] -1] -1;i+ i) ijc[ i] =ija[ i] ;
      sprspm(sa, ija, sbt,ijbt, sc, ijc) ;
      for (i=1; i<=NP, i++) {
           如r (j '1; j<＝甘P; j++) {
              ab[i] [j] =0.0;
              for (k=1;k<=NP;k++) {
                   ab[i] [j] =ab[i] [j] +a[i] [k] *b[k] [j] ;
                }
           }
      }
     printf ( "Reference matrix: \n') ;
     如r (i=1; i<＝甘P; j++) {
         for (j=1; jc=NP; j++) printf ( "%5. 2f\ t ", ab[i] [j] );
         printf ( "\ n") ;
      }
     printf ( "sprspm matrix (should show only tridiagonals) :\n ") ;
     for (i=1; i<=NP; i++) for (j= 1; j<＝月? ;j+ +) c[i] [j] =0. 0;
     如r (i=1; i<＝甘P; i++) {
          C［幻［幻 =sc[i] ;
          for (3=ijc[ i] ;j< =ijc[ i+1]-1; j++) c[i] [ijc口] ]=sc[ j] ;
      }
      如r (i=1;i<＝甘P; i++) {
         for (j '1; j<=NP; j++) printf ( "%5.2f\ t ", c[i] [j] );
         printf ( "\ n") ;
      }
      free..convert.jsatrix (b, 1,NP, 1,11?);
      free...convert_matri工(a, 1,NP, 1,NP) ;
      free_matrix (ab,1,NP, i, NP) ,
      free_matri工(c, 1,NP,1,NP) ;
      free_ vector (sc, 1, 甘KAX) ;
                                              Ch짜가er 2: 乙near A勺ebraic Eqi旭加ns   25

    free_ vector佃bt 1, 甘MAX) ;
    fr的_ vect口r佃b, 1,NMAX) ;
    free_ vector (sa,l, INAX) ;
    free_lvector (ijc, 1.N片AX)';
    free_lvector (ijbt .1.NMAX) ;
    free_lvector (ijb, 1 , NMAX) ;
    free_lvector (ija, 1.NMAX) ;
    return 0;
}


      ：烈,빠？冒，茄，’們，骨,,？沙，牝：'隘盜IIC
誌：然律恣曜：
test program xsprstm is thus very similar to the previous test program.
/s Driver for routine epretm 卞/

*include <stdio . h>
卄mnci皿de 1뇨r .h"
#include "nr工til.h"

作define NP S
*define 甘MAX (2中NP卞NP+1)
#define THRESH 0.99

jut siain(void)
{
    unsigned long i, j, k, *ija, *ijb, *ijbt, Sijc, msize;
    float 卞Ba, 布sb,*sbt, 字Sc.卓京a, 卞Sb,中卞C1李＋ab;
    static float ainit[ NP] [NP).'{
        1.0,0.5,0.0,0.0,0.0,
        0.S, 2.0,0.5,0.0,0.0,
        0.0,0.5,3.0,0. 5,0.0,
        0. 0,0.0,0. 5,4.0,0. 5,
        0. 0,0.0,0.0,0.5,5. 0} ;
    Static float binit[ NP] ENPJ={
        1. 0,1. 0,0.0,0. 0,0.0,
        1. 0, 2.0,1.0,0.0,0.0,
        0.0.1.0,3.0,1.0,0. 0,
        0.0,0. 0,1. 0,4. 0,1. 0,
        0 . 이0. 0,0.0.1.0,5 . 아；

    ija=lvector (1,NMAX) ;
    幻b=lvector (1,N甘AX) ;
    ijbt= lvector (1,月MAX) ;
    ijc= 1vectOr (1,NMAX) ;
    sa=vector ( 1, 召甘AX) ;
    sb=vector (1,NMAX) ;
    sbt=vector (1,NMAX) ;
    s口＝vector (1,NMAX) ;
    c=iuatri工（1,月P,1,NP) ;
    ab=matrix (1,NP,1,NP) ;
    a"convert_matrix(kajnit [0) [0] , 1,NP, 1, NP) ;
    b=convert_matrix(kbinjt[ 0] [0) , 1,NP, 1,NP) ;
    sprsin(a,NP, 0. 5,N札AX, aa,ija) ;
    aprsin(b,NP, 0.5,NMAX, sb,ijb) ;
    sprstp(sb, ijb, sbt ,ijbt) ;
    msize=ija[ ijaEl] =1] -1;
26       N切net七a／尸ec徊es Ex카까)Ie Book

     sprstm(sa, ija, sbt, ijbt, THRESII,msize, sc,ijc) ;
     for (i=1; i<=NP; i++) {
         for (j=1; j<=NP; j++) {
             ab［刃 口］=0 . 0 ;
             for (k=1;k<=NP; k++) {
                   ab［幻 口］=abEi] [j] +a［刃 [k] 4t江k] Li] ;
               }
          }
     }
     printf ( '떠冶ference matri工：\n.,);
     for (i=1; i<=NP; i++) {
         for (j= 1; j<=NP; j++) printf ( ''%5. 2f\ t ", ab[i] [j] );
         printf ( '\ n") ;
     }
     printf ( "sprstm matrix (off- diag. elements of mag >): %12 . 6f\ n' ,THRESE) ;
     for (i=1; i<=NP; i++) 如r (j= 1; j<=NP; j++) c[i] [j] =0. 0;
     for (i=1; i<=NP; i++) {
         C [i그 [i] =sc［幻 ;
         for (j= ijc[ i] ;j< =ijc[ i+1] -1; j++) c［幻 口3c口끄＝SC［刃 ;
     }
     for (i '1; i<=NP; i++) {
         for (j '1; j<=IP; j++) printf ( "%6. 2f\ t ", c[i] [j] );
         printf ( "\ n") ;
     }
     free_ convert_matrix (b1, NP, 1, NP) ;
     free_ convert_matrix (a, 1, 51', 1,51
                                         ') ;
     free.. matrix (ab, 1.NP,1,NP) ;
     free_matrix (c, I 1 甘F느 1, 且P) ;
     free_ vector (sc,1,NMAX) ;
     freem vector (sbt, 1,NMAX) ;
     free_ vector (sb, 1,NMAX) ;
     free_ v吼如r (sa, 11때AX) ;
     free_lvector (ijc, 1,NMAX) ;
     free_lvector (ijbt, 1 ,NNAX) ;
     free_lvector (ijb, 1,N1(AX) ;
     free_lvactor ( ija, 1, IMAX) ;
     return 0;
}

    Routine liribcg solves linear systems A . x = b with a sparse matrix A. The
matrix A must be specified in sparse matrix format as described in Numerical Recipes.
In our sample program xlinbcg we define A to be the 20 x 20 matrix


                                             2.0
                                                      0        0 0 00
                                                               00n (
                                                    乙
                                                    nl1乙
                                                       n
                                                           4      1
                               [         1.
                                   -0
                                        。0
                                        2.
                                             1.0
                                              .。
                                                           1      1

                                                                   l1
                                        。.。 -2.0           1

                                                               0 000
                                                                  1
                                                                        /]
                                             0.0           1      1




                                                           1      1

                                                           1      t

                                                           1      1




As a right-hand side vector b we have taken (3.0, 1.0, 1.0,. . . ,-1.0), and the solution
is given as x. Notice that the components of x are all initialized to zero. You will set
them to some initial guess of the solution to your own problem, but a zero guess will
usually suffice. The solution in xlinbcg is given the usual checks.
                                                     Ch랴升er 2: Linear A勺ebra厄 Equal幻ns         27
    ／卞 Driver 如r routine linbcg 巾／

    作include <stdio . h>
    #inc].ude <math.h>
    #include "nr. h"
    #include "nrutil. h"

    #define NSIZE 59
    #def ins NP 20
    #define ITOL 1
    #define TOL le- 9
    #def ins 工'r겨AX 75

unsigned 加ng 幻缸邪IZE+1] ={
    0, 22, 23, 25, 27, 29,31, 33,35,37,39,41, 43,45,4
                                                            7,49,51, 53, 55, 57,
    59,60,2,1,3,2, 4,3,5,4,6,5,7,6,8,7,9,8,1
                                                        0,9,11, 10,12,11,13,12,
    14, 13, 15, 14, 16, 15, 17, 16, 18, 17, 19, 18, 20,
                                                        19) ;

double saI'.NSIZE+1] = {
    0.0,3. 0,3. 0, 3. 0,3.0, 3. 0,3.0,3.0,3. 0,3.0,3
                                                           .0,3. 0,3.0,3. 0,3. 0,3.0,3. 0,
   3.0,3.0,3.0,3. 0,0.0,2.0,-2. 0,2.0,-2.0,2.0
                                                           ,-2.0,2.0,-2.0,2.0,-2.0,
    2. 0, -2. 0,2.0, -2 . 0, 2. 0 ,-2. 0, 2.0, -2.0,2. 0,
                                                          -2.0,2. 0, -2.0,2. 0, -2. 0, 2. 0,
   -2. 0, 2.0, -2.0,2. 0, -2.0,2. 0, -2.0, 2.0, -2.0,2.
                                                             0, -2. 0, 2.0, -2.0) ;

ml1t niain(void)
{
          mllt i, ii, iter;
          double 卞b，中bcmp,中工1err;

       b=dvector (1,NP) ;
       bcmp=dvector (1,NP) ;
        x=dvector (1,NP) ; .
       如r (i= 1; i<＝片P; i++) {
            工t:i] "O.O;
            bE:口＝1.0;
       }
      l江1] =3.0;
      t江NP] = 느1. 0;
      linbcg（月P，뉵 치IT0L,T아U工FlU瓦kiter,&err)
                                                      ;
      prmntf ( "/.s /.1&e\n", "Estijsated error: ", err)
                                                           ;
      printf ( "/.s /.6d\n", "Iterations needed: ", iter)
                                                             ;
      printf (' "\ nSolution vector: \n") ;
      for (ii= 1; ii< =NP/5;ii+ +) {
           for (i=5* (ii- 1)+1;i< =5*ij; i++) printf
                                                        ( "7,12.6f ", x[i] );
           printf ( "\ n") ;
      }
      for (i=1; i<=(NP 工 5) ;j+ +)
          printf ( ' 工12. 61", xE5*(NP/S) +i] );
     printf ( "\ n ") ;
     dsprsa工佃미 ija, 치bcmp,NP) ;
     /* this is a double precision version
                                                 of sprsa工 巾/
     printf ( '\ npress RETURN to continue. . .\n ") ;
     (void) getcharO;
     printf ( "test of Solution vector: \n") ;
     prmntf ( "%9s %12s\n", "a*x", "b") ;
     for (i "i; i<=NP;i++)
         printf ( "%12.6f %12. 6f\ n". bcmp[i] ,bEi]
                                                     );
28               Nume力ca／尸ec枷9S Examp旭 Bo아（

            free느dvector（工 ,1 , 川,) ;
            tree_dvector (bcmp,1,NP) ;
            free_dvector (b, 1,NP) ;
            return 0;
}

    Vandermonde matrices of dimension N x N have elements that are entirely integer
powers of N arbitrary numbers x1 . . . xN. (See Numerical Recipes for details). In the
demonstration program xvander we provide five such numbers to specify a 5 x 5
matrix, and five elements of a right-hand side vector Q. Routine vander is used to
find the solution vector W. This vector is tested by applying the matrix to W and
comparing the result to Q.
／字 Driver 如r routine va끄der +/

*include <stdio .h>
#include "nr. h"
*include 1'nrutil. h"

*define N 5

m1lt main(void)
{
            mnt i口 ;
            如uble su皿＝0. 0, 方日 1卞term;
            static double 江[]={0.0,1. 0,1.5, 2.O,2. 5,3.O} ;
            static double q그＝{0. 0, 1. 0,1. 5, 2.0, 2. 5,3. 0);

            日＝dvec如r (1,N) ;
            term=dvector (1,N) ;
            vander (x, 므, q,N) ;
            printf ( "\ nSo].ution vector: \n") ;
            for (i 'l; i<=N; i++)
                printf ( "/,7s%1dX2s 工12f \n", 'w[ ", i, ') =' , w[i] );
            printf ( "\ nTest of solution vector: \n") ;
            prmntf ("%14s '/.lls\ n", "mtrxssol 'n' , "original ") ;
            如r (i=1; i<＝甘；j++) {
               七era［幻＝日Ii] ;
               su皿 += 叭i] ;
             }
            printf ( "%12. 4f /.12. 4f\ n ', sum,q(1] );
            如r (i '2; i<＝且；j++) {
                s1山1=0 . 0 ;
                  如r (j=1; j<＝且；j++) {
                     term[j] 方＝ 玎刃；
                     sum += term[ j] ;
                  }
                  printf ( "/.12. 4f %12. 4f\ n", su皿, q[i] );
             }
             f ree_dvector (t era , 1,N) ;
             free_dvector (v, 1,N) ;
             return 0;
    1
        '




       A very similar test is applied to toeplz, which operates on Toeplitz matrices.
    The N x N Toeplitz matrix is specified by 2N - 1 numbers r, in this case taken
                                                Ch邵加r2: Unear겨勺ebra乞 Equal幻ns    29

to be simply a linear progression of values. A right-hand side yi is chosen likewise.
toeplz finds the solution vector x, and checks it in the usual fashion.
／中 Driver 加r ro1工tine toeplz 巾／

#include <8tdio . h>
#include "nr.h"

*define 月 5
*define TWON (2卞1)

jut main(void)
{
    jut i, j;
    float su皿,r[ TW0N+1] ,xCN+1] .y[N+1] ;

    如r (i:=1; i<=N; i++) 虹i]=0. 1卞i;
    for (i: 1; i<TW0月; i++) r[ iJ=1.o/i;
    toeplz(r, x, y,1) ;
    printf ( "So].ution vactor: \n") ;
    如r (i '1; i<＝甘；i++)
        printf ( "%Ts%ld'/.s %13f\n". "xC", i, "] = " 1工［i] ) ;
    printf ( "\ nTeat of solution: \n") ;
    printf ( "%138 %12c\n", "mtrx卞soln", "original") ;
    for (i=l; i<=1; i++) {
        Cu皿＝0.0;
        for (j 'l; j<"J; j++)
              Cu皿 += (r口＋i- i］卞x [j] );
        printf ( "%12. 4f '/.12.4f\n", su皿, y[i] );
    }
    return 0;
}

    The routines choldc and cholsi are tested together by xcholsl. First we form
a 3 x 3 positive-definite, symmetric matrix. We compute its Cholesky decomposition,
and check the answer by explicitly multiplying back the Cholesky factors. We then
use the decomposition to solve a 3 x 3 system of equations, and check the answer by
substituting back in the original system.
／卞 Driver 如r routine cholal 本／

#include <stdio . h>
#include "nr.h"
#inc끄ide 1'ur1比il.h"

*def inc 月 3

jut main(void)
{
    mnt i, j 小；
    float su且！*方a,卞巾atest, 衣巾chol,卞p. 卞工；
    static float aorig[1+1] [N+1] =
        {0 .0.0.0, 0.0,0.0.
        0. 0,100.0,15. 0,0.01,
        0. 0,16.0,2.3,0. 01,
        0. 0,0.01,0.01,1.0};
    日tatic float 1江J+1]={o.o,0.4,o.02汨且아；
    30       Numerical Recipes Example Book


         amatri工（1,瓦 1,N) ;
         at的1=matrix(1,瓦 1.') ;
         chol=matrix(1,M,1.1) ;
         p'vector(l ,N) ;
         x=vector (1,I) ;
         for (i=1;i<=1;i++)
             for (j=1; j<=1; j++) a(i] 口]=aorigCi] Cj] ;
         choldc(a,I, p) ;
         printf ("Original matrix: \n") ;
         for (j=1;i<=N;i++) (
             for (j=1; j<=1; j++) {
                  cholCi] [j] =( (i > j) ? a[i표j] : Ci == j ? 바i] : 0.0) );
                  if Ci > i) cholCi표刃 aCi끄j] ;
                  else cholCi]日]=(i == j ? pCi] : 0.0) ;
                  printf ( '%16.6e", aorigCi] Cj] );
             }
             printf ("\n") ;
         }
         printf ( '\ n") ;
         printf ( "Product of Cholesky factors: \n') ;
         for (i=1;i<=1;i++) {
             for (j=1; j< "N; j++) {
                   for (sum=0. 0,k=1;k< 1; k++) sum += cholCi표k]*cholCj] C닙;
                   ateetti] [j] =su三;
                   printf ("%16.6e", atestCi] Ci] );
             }
             printf ( "\n") ;
         }
         printf ("\ n") ;
         printf ( "Check solution vector: \u") ;
         cholsi（키瓦p,b，工）;
         for (i=l; i<=1;i++) {
             for (sum=0.0, j=1; j<=J; j++) su += aorigCi] Cj] *x (j] ;
             F止i] "Sum;
             printf ( "%16.6e工16. 6e\n",pCi] , b(i] );
         }
         free_vector (x, I ,N) ;
         free_vector (p,1,$);
         free_matrix(chol. 11瓦 1,1) ;
         free_niatrix(atest , i, 瓦 1,1) ;
         free_皿atri工（a,1.瓦 1,1) ;
         r日tt口n 0;
}

    The QR decomposition routine qrdcmp is tested by a program xqrdcmp that is
very similar to the program1l for testing the LU decomposition. It reads in the same
set of test -matrices from the file matrxl .dat, does the decomposition of each one,
and then checks the result by multiplying the Q and R matrices.
／巾 Driver 如r routine qrdcap 中／

#include <stdio.h>
卄include <stdlib.h>
斗include 1뇨r.h"
#include "nrutil. h"
                                               （가1邵）旭r 2: LinEar A勺ebraic Equa卄ons   31

*def ins NP 20
#def ins MAXSTR 80

m1lt main(void)
(
    mllt i口,k,l, m,n, sing;
    float con, *中a,卞C, 卞d1方中q1中牛qt, 李＋r, 卞*工；
    char dummy［甘A工STRI ;
    FILE *fp;

    a=1natri工（1,甘P,1,NP) ;
    c=vector (1,NP) ;
    d=vector (1,IP) ;
    q=matri工（l ，月P, i, NP) ;
    qt-matrix (1,NP,1,NP) ;
    r=matri工( 1,引', l, 恥）;
    x=inatri工（l , 丑P,1,NP) ;
    if ( (fp = fopen( "matrxl.dat' , "r ') ) == NULL)
        nrerror ( "Data file matrxi.dat not found\n") ;
    while (! feof (fp) ) {
         fgets (dummy,MAXSTR, fp) ;
         fgets (dummy ,MAXSTR, fp) ;
         fsc띠lf (fp, "Y.d %d ", &n,kin) ;
         fgets (dummy ,MAXSTR,fp) ;
         for (k=1;k<=n;k++)
              for (1=1;l< 'n;l++) fscanf (fp, "%f ", ka[k] [lJ) ;
         fg日ts (du皿my，甘AXSTR , fp) ;
         for (1=1;l<=m; l++)
              for (k=1;k<=n;k++) face끄t (fp. "工f " ,t工［k] 口n ;
        ／卓 Print out 十matri工 for comp町ison 日ith product of
             Q and ft decomposition matrices */
        printf ( "Original matrix: \n") ;
         for (k=1;k< 'n;k++) {
              for (l "l; l<=n;l++) printf ( "/.12.6f ", a[k] [l] );
              printf ( "\ n") ;
        }
        /卞 Perform the decomposition 巾/
        qrdcmp(a,n,c,d,ksing) ;
        if (sing) fprintf (stderr, "Singula工ity in Qft decomposition. \n") ;
        /京 find the Q and ft matrices 卞/
        for (k"l; k<=n;k++) {
             for (l=1;l<=n;l++) {
                 if (1 > k) {
                     r[ k] [l] =a[k] [1] ;
                     q[k] [1] =0.0;
                 } else if (1 < k) {
                     r[ k] [l] =qEk] [l] =0.0;
                 } else (
                     r[ k] [lj= d[k] ;
                     q(k] [l] =i. O;
                     }
                }

        f}   。r (i=n-1; i>=1; i- -) {
                for (con=0. 0,k=i; k<=n;k++) con += a[k) [i) *a[kj [i] ,
                con /= 2.0;
                for (k=i; k<=n;k++) {
    32       Nu,加rica! Rec徊es Example Bo｛水

                        for (l= i; l<=n;l+ +) {
                            qt[ k] [l] =O. o;
                            for (j= i; j<=n; j++) {
                                qt[ k] [1] += q[ j) [l] 卞a[k] [ij* a[ j) Ci] /con;
                            }
                        }
                   }
                   for (k=i; k<=n;k++)
                       for (l= i; l<'n; l++) q[k] [l]  中= qt[ k] [l] ;
              }
              /* compute product of Q and ft matrices for compa工ison
                 甘ith original matri工． 串／
              for (k=1;k< 'n; k++) {
                  for (1=1;l< 'n; l++) {
                      x[k] [l] =0. O;
                      for (j=1; j<=n; j++)
                           x[k] [l] += q[k] [j) *r[ j] [l] ;
                   }
              }
              printf ( "\ nProduct of Q and ft matrices: \n") ;
              for (k=1;k<=n;k++) {
                  for (l=1;l<=n;l+ +) printf ( '%12. 6f ", x[k] [l] );
                  printf ( '\ n") ;
              }
              printf ( "\ nQ matrix of the decomposition: \n") .
              for (k'1; k<=n;k++) {
                  for (l=1;l< =n;l++) printf ( "%12. 6f ", q[k) [l] );
                  printf ( "\ n") ;
              }
             printf ( "\ nft matrix of the decomposition: \u") ;
             for (k=1;k<=n;k++) {
                 for (l= 1;l< =n;l+ +) prjntf ( "/,12. 6f ', r[ k] [lj) ;
                 printf ( "\ n' ') ;
             }
             printf ( "\ n. 方*方方中*中卞牛＋字＋*中卓京李字中卞牛中字卞李方字中字卞*卞方字＼O") ;
             printf ( 'press return for next problem: \n") ;
             (void) getcharO;
         }
         fclose(fp) ;
         free_matri工（工 ,1, 恥,1,NP) ;
         free_matrix(r, 1, NP, 1, NP) ;
         free느matrix (qt, 1, 甘P, 1，甘F) ;
         free_matrix (q, I ,NP, 1,NP) ;
         free_ vector (d, 1,NP) ;
         free_ vector (c, 1, 月P) ;
         free_matri工(a, 1, 川：1, 1,NP) ;
         return 0;
}

    Similarly routine qrsolv is tested by a program xqrsolv that is almost the same
as the test program for LU backsubstitution, and uses the same set of test matrices
in the file inatrxl .dat.
/牛 Driver for routine qrdcmp */

#include <stdio . h>
Ninclude <stdlib . h>
                                             Ch카）ter 2: Linear Algebraic Equations   33

#inciude 'nr. h"
#include "nrutil. h"

#deflne NP 20
#define MAISTR 80

mllt main(void)
{
    jut j, k,l, m,n,sing;
    float; 卞X1中巾a, 卞卞ai,中中b, 布C, 卞d;
    char dw皿y [MLXSTR] ;
    FILE *fp;

    x'vector (l, 引：1) ;
    a=matri工（1, 甘P, 1, 甘P) ;
    b=aatrix (i, 甘P,1,NP) ;
    ai=matrix (1,NP,1,NP) ;
    c=vector (1,月P) ;
    d=vector (i ,NP) ;
    if ( (fp = fopen( "matrxl.dat ", "r ") ) == NULL)
        nrerror ( "Data file matrxi.dat not found\n") ;
    while ( 'feof (fp) ) {
        fgets (du띠ny,MAXSTR,fp) ;
        fgete (dummy,MAXSTR,fp) ;
        fsc缸1f (fp, "hd%d ", kn,&m) ;
        fgets(dui皿y,MAXSTIt, fp) ;
        for (k=1;k<=n;k++)
             for (1=1;l<=n;l++) fscanf (fp, "/.f ", &a[k] (l) );
        fgets (du皿my ,MAXSTR,fp) ;
        for (1=1;l< =m;l++)
             for (k=1;k<=n;k++) fsc띠lf (fp, "%f ", &b[k] [l] );
        ／中 Save matri工 a for later testing 巾／
        for (l=1;l< rn;l++)
             for (k=1;k<=n;k++) aiCk] [l] =aEk] [1) ;
         /卞 Do qr decomposition 巾!
        qrdcap(a,n, c,d,1sing) ;
        if (sing) fprintf (stderr, "Singularity in QR decomposition. \n") ;
        ／卞 鈿lye equations 如r each right- hand vector 中／
         for (k=1;k<'m;k++) {
             如r (1=1;l<=n;l++) x[l] =b[1] [k] ;
             qrsolv(a,n,c,d,x) ;
              /s Test results with original matrix 卞!
             printf ( "right- hand side vector: \n") ;
              for (1=1;l<=n;l++)
                  printf ( "/.12.6f ",btl] [k] );
             printf ( "\ n%s%s\n", "result of matrix applied",
                  11 t：乙 sol노 vector") ;
              for (1=1;l<=n;l++) {
                  b[l] [k] =0.0;
                  for (j=1; j<=n; j++)
                        l江1] Ek] += (ai[ l] [j］卞工[ j] );
              }
              for (1=1;l<=n;l++)
                  printf ( "%12.6f ",b[l] Ek] );
             printf   ( "\ n字卞卞巾中中中＋中＋卞中＋＋中*卞卞牛*中巾巾卓＋卞卞卞卞巾衣京卞＼n ") ;
        }
        prmntf ( "press RETURN for next problem: \n") ;
        34       Nume成旨／Re非旭s Examp旭 Book

                  (void) getcharO;
             }
              fclose(fp) ;
             free_ vector (d, 1,1?);
             free_ vector (c 11, NP) ;
             free_matrix (ai, 1,NP,1 1꺄) ;
             free_matrix(b 11,月P 11,IP) ;
             free_matrix(a, 1 ,NP, 1,NP) ;
             free_ vector (x, 1,NP) ;
             return 0;
    }

    The test program for qrupdt once again reads in test matrices from the file
matrxl .dat. However, it uses the solution vectors in the file as vectors defining
                                                                                   the
update to be performed. The solution is checked by explicitly updating the original
matrices and then doing an ab initio QR decomposition.
/* Driver for routine qrdupd */

#inc].ude <stdio .h>
#include <stdlib. h>
#include "nr.h"
#include "nrutil. h"

#define NP 20
#define MAXSTR 80

mnt main(void)
{
         jut i, j, k, l, m1n, sing;
         float con，中方a, *中au1中c1 Cd1 *卞q, 衣中qt, 卞牛rr卞卞8,卞1l14V14＋工；
         cha工 duminy[MA工STK] ;
         FILE *fp;

          a=matrix (1,NP,1,NP) ;
          au=matrix (1,NP,1,NP) ;
          c=vector (1,NP) ;
         d=vector (1,NP) ;
         q'matrix (l, NP, l, NP) ;
         qt=matrix (1,丹P,1,NP) ;
         rrmatrix (1,NP,1,NP) ;
         8=matri工 ( i, NP,1, 甘P) ;
         u=vector (1,NP) ;
         v=vector (1,NP) ;
         工＝matri工（1, 丑P,1,NP) ;
         if ( (fp = 如pen( "matrxl.dat ", "r ") ) == N月．.L)
             nrerror( "Data file matrxl. dat not founcl\n") ;
         while (! feof (fp) ) {
             fgets (dummy ,X1.XSTR,fp) ;
             fgeta (dummy ,MAXSTR, fp) ;
             fecanf (fp, "%d %d ", &n,&m) ;
             fgets (dummy, MAXSTR,fp) ;
             for (k=1;k<=n;k++)
                  for (1=1;l<=n; l+ +) facani(fp, " 加 ", &a[kj[ l] );
             fgets (du1口皿y，片AXSTR , fp) ;
             for (1=1;l< =m;l+ +)
                  for (k "l; k<"n;k++) fscanf (fp. "%f ", k町kJ[l] );
                                      Ch랴升er 2: Linear A勺ebra幻 Equat幻ns   35
  /李 Print out a-matrix for comparison with product of
     Q a끄d ft decomposition matrices */
 printf ( "Original matrix: \n") ;
  for (k=1;k<=n;k++) {
       for (1=1;l<=n;l++) printf ( "%12.6f ", a[k] [l] );
      printf ( "\ n") ;
  }
  /中 updated matrix we 'll use later */
  for (k=1;k<'n; k++)
      for (1=1;l< =n;l++)
           au[k] [l] =aEk] [l] +s[k] 口］京訌1] [2] ;
 /布 Perform the decomposition 中/
 qrdcmp(a,n, c,d,ksing) ;
 if (sing) fprintf (stderr, "Singularity in Qft decoisposition. \n") ;
 ／斗 find the q a끄d ft matrices 卞／
 for (k=1;k<=n;k++) {
      for (1'l; l<"n;l++) {
           if (1 > k) {
               r[ k] [l] =a[k] [1] ;
               아k] 口］=0 . 0;
           } else if (1 < k) {
               r[ k] [l] "qCk] [l] =0. 0;
          } else {
               rtk] [l] =d[k] ;
               q[k] [l] 'l. O;
            }
       3.
 3.
如r (i=n-1; i>=1；卜D {
   for (con=0.0,k=i; k<=n;k++) con += aCk] [i] *a[k] Ei] ;
   con /= 2..0,
   for (k=i; k<=n;k++) {
       for (1=i; l<=n;l++) {
            qt[k] [l] "O.O;
            for (j "i; j<=n; j++) {
                qt [k] [1] += q[ j] Cl］方a[k3［幻卞a[ j] C:L] 八on;
                3.


      for (k=i; k<=n;k++)
          for (l "i; l<=n;l++) qCk] [l]  -= qt[k] Cl] ;
3.
/* compute product of Q and ft matrices for comparison
   日it上 original matrix. 中／
for (k=1;k<=n;k++) {
    for (l=1;l< 'n;l++) {
        x[k] [l] =0.0;
        for (j "l; j<=n; j++)
             x[kj[ l] += qCk] [j] sr[ j] [l] ;
      3.
3.
printf ( "\ nProduct of Q 카ld ft matrices: \n") ;
for (k=1;k<=n;k++) {
    如r (l "i; l<=n;l++) printf ( "工12. 8f ", 址蛇口］) ;
    printf ( "\ n") ;
3.
printf ( "\ nq matrix of the decomposition: \n") ;
36    Numorica/ 尸9（加es Examp旭 Book

       for (k=1;k<=n;k++) {
                                                           );
           for (1=1;1<=n;1++) printf ( "%12.6f ", q[k) [1]
           printf ( "\ n') ;
       )
                                                    \n") ;
       priutf ( "\ nft matrix of the decomposition:
       for (k=1;k<=n; k++) {
                                                            );
           for (1 '1;1<=n;1++) printf ( "%12.6f ", rtk] E1]
           printf ( "\ n") ;
        }
       ／卞 Q transpose 中／
       for (k=1;k<=n;k++)
           for (1=1;1<=n;1++)
                qt[ k] [1]=q[1] [k] ;
       for (k=1;k<=n;k++) {
           v[k] =s[k] [2] ;
                                                                 [1] ;
           for (u[k] =O. O,1=1;1<=n;1++) u[k] += qt[ k] [1]中s[1]
        }
        qrupdt (r, qt, n,u, v) ;
        for (k=1;k<=n;k++)
            for (1=1;1<=n;1++)
                                                                          [k] 卞r[ j] [1] ;
                  for (x[k] [1] =0. O, j=1; j<=n; j++) x[k] [1] += qt[ j]
        printf ( "Updated matrix  : \n") ;
        for (k'l; k<=n;k++) {
                                                                );
            for (1"l; l< "n;l+ +) printf ( "%12.6f ", au[닙口]
               printf ("\ n") ;
           }
                                                           \n") ;
           printf ( "\ nProduct of ne日 Q and ft rnatrices:
           for (k=1;k<=n;k++) {
                                                                 );
               for (] =1;1<=n;1++) printf ( "/.12.6f ", x[k] [1]
               printf ( "\ n") ;
           }
           printf ( "\ nNew Q matri工: \n") ;
           for (k=1;k<=n; k++) {
               for (].=1;1<=n;1++) printf ( "%12. 6f ", qt[ 1] [k] );
               printf ("\ n") ;
           }
           printf ( "\ nNe日 ft matrix: \n") ;
           for (k '1; k<=n;k++) {
                for (1=1;1<'n; l+ +) printf ( "/.12. 6f ", r[ k] [1] );
               printf ( "\ n") ;
            }
                                                                    \n") ;
            printf ( "\
            printf ( "press return for next problern: \n") ;
            (void) getcharO;
     }
     fclose(fp) ;
     free_matrix (x, 1, NP, 1, NP) ;
     free_ vector (v, 1,NP) ;
     free_vector (u, 1,NP) ;
     free_rn批ri工佃 , 1, NP, 1, NP) ;
     free_matrix (r, I ,NP, i, NP) ;
      free_matrix(qt, 1,NP, 1,NP) ;
      free_matrix (q, 1, NP, 1, NP) ;
      free_ vector (d,1, NP) ;
      free_ vector (c, l, 甘P) ;
      free_matrix (au, 1, NP, 1,NP) ;
      free_matrix (a, 1,NP, 1,聊) ;
                                           Ch回口ter 2: Linear Algebra初 Equ카幻ns   37

      return 0;
}
                                        Append奴

File matrxl. dat:
MATRICES FOR INPUT TO TEST ROUTINES
Size of matrix (lx미, lumber of solutions:
32
甘atri工 A:
1.0 0.0 0. 0
0.0 2. 0 0.0
0. 0 0. 0 3. 0
Solution vectors:
1. 0 0. 0 0. 0
1.0 1.0 1.0
丑EXT PROEL目1
Size of matrix (lxi) , lumber of solution月:
32
Matrix A::
1.0 2.0 3,0
2.0 2.0 3. 0
3.0 3.0 3.0
Solution vectors:
1.0 1.0 1.0
1.0 2.0 3.0
且EXT PROBLE甘：
Size of matri工 (I工N) , 小imber of solution月：
52
Matrix A:
1.0 2.0 3.0 4.0 5.0
2. 0 3. 0 4. 0 5. 0 1. 0
3.0 4.0 5.0 1.0 2.0
4. 0 5. 0 1. 0 2. 0 3. 0
5.0 1.0 2.0 3.0 4.0
Solution vectors:
1.0 1.0 1.0 1.0 1.0
1. 0 2, 0 3. 0 4. 0 6. 0
NEXT PROBLEM:
Size of matri工 (I工I) , lumber of solutions:
52
Matrix A:
1.4 2. 1 2, 1 7.4 9.6
1.6 1.5 1.1 0.7 5.0
3.8 8.0 9.6 5.4 8.8
4.6 8. 2 8.4 0.4 8.0
2.6 2.9 0. 1 9.8 7.7
Solution vectors:
1.1 1.6 4.7 9. 1 0. 1
4.0 9. 3 8.4 0.4 4. 1


    File mat rx2 .dat:
    FILE OF TRIDIAGONAL MATRICES FOR PROGRAM 'TRIDAG '
    Di皿en日ion of matri工
    3
    38    N切neri石／Re（加es Example Book

   Diagonal elements (N)
   1. 0 2. 0 3. 0
   Super-diagonal elements (N-I)
   2.0 3.0
   Sub-diagonal elements (N-i)
   2.0 3.0
  Right-hand side vector (N)
  1.0 2.0 3. 0
  甘EXT PROBLE片：
  Dimension of matrix
  S
  Diagonal elements (N)
  1. 0 1. 0 1. 0 1. 0 1. 0
  Super-diagonal elements (N-i)
  1. 0 2. 0 3. 0 4. 0
  Sub-diagonal elements (N-i)
  2.0 3.0 4.0 5.0
 Right寸Land side vector （비
 1. 0 2. 0 3. 0 4.0 5. 0
 丑EXT P}山BLEM:
 Dimension of matrix
 5
 Diagonal elements (N)
 1.0 2.0 3. 0 4. 0 5. 0
 Super-diagonal elements (N-I)
 2. 0 3. 0 4. 0 5. 0
 Sub-diagonal elements (N-I)
 2.0 3.0 4.0 5.0
Right-hand side vector (N)
1. 0 1.0 1. 0 1. 0 1. 0
NEXT PROBLEM:
Dimex田ion of matri工
6
Diagonal elements (N)
9. 7 9.5 5. 2 3. 5 5. 1 6. 0
Super-diagonal elements (N-i)
6.0 1. 2 0.7 3.0 1.6
Sub-diagonal elements (N-i)
2. 1 9. 4 3. 3 7.6 8. 8
Right-hand side vector (N)
2. 0 7. 6 0. 6 7. 4 9. 8 8. 8


File matrx3. dat:

FILE OF MATRICES FOR SVDCMP:
Number of Ro日s, Columns
5 3
Matrix
1. 0 2. 0 3. 0
2.0 3.0 4.0
3.0 4. 0 5. 0
4. 0 5.0 6. 0
6. 0 6. 0 7. 0
月EXT PF山BLEM:
Nu皿ber of Ro日5. Colu口as
55
Matrix
                              Chapter 2: Linear Algebraic Equations   39

1.0 2.0 3. 0 4.0 5.0
2.0 2. 0 3. 0 4.0 5. 0
3.0 3. 0 3. 0 4.0 5. 0
4. 0 4. 0 4. 0 4. 0 5. 0
6. 0 6.0 5. 0 5. 0 5. 0
NEXT PROBLEM:
Number of Ro口S. Co].u皿'S
6 6
Matrix
3.0 6.3 5. 6 3.5 6. 8 5. 7
0. 4 8. 2 8. 7 1.9 2. 2 5.3
7. 8 8. 3 7. 7 3.3 1. 9 4.8
6. 5 8. 8 3. 0 1.0 5.1 6.4
5,1 5.1 3.6 5. 8 6.7 4.9
3.5 2.7 5.7 8. 2 9.6 2.9
Chapter 3: Interpolation and Extrapolation

          Chap扼r 3 of N끄meni口I/ 只ec加es dea加 w元h 加扼叩可atio끄 and e批rap이ation
      (the same routines are usable for both). Three fundamental interpolation
      methods are first discussed,
       1. P이ynom洌 m t針p可ation (polint),
       2. Rational function interpolation (rat int), and
       3. Cubic spline interpolation (spline, splint).
          To 月nd the place in an ordered table at whit出 如 perform an 加扼叩olation,
      two routines are given, locate and hunt. Also, for cases in which the actual
      coefficients of a polynomial interpolation are desired, the routines polcoe
      and polcof are provided (along with important warnings circumscribing their
      usefulness).
          For higher-dimensional interpolations, Numerical Recipes treats only prob-
      lems on a regularly spaced grid. Routine poiin2 does a two-dimensional poly-
      nomial interpolation that aims at accuracy rather than smoothness. When
      smooth interpolation is desired, the methods shown in bcucof and bcuint
      for bicubic interpolation are recommended. In the case of two-dimensional
      spline interpolations, the routines sp1ie2 and sp1in2 are offered.



    Program polint takes two arrays xa and ya of length N that express the known
values of a function, and calculates the value, at a point x, of the unique polynomial of
degree N - 1 passing through all the given values. For the purpose of illustration, in
xpolint we have taken evenly spaced xa[i3 and set yaCi] equal to simple functions
(sines and exponentials) of these xa[i] . For the sine we use an interval of length 冗,
and for the exponential an interval of length 1.0. You may choose the number N of
reference points and observe the improvement of the results as N increases. The test
points x are slightly shifted from the reference points so that you can compare the
estimated error dy with the actual error. By removing the shift, you may check that
the polynomial actually hits all reference points.
／卞 Driver 如r routine 恥lint      */

#include <Ctdio. )l>
*include <ath. h>
*include "nr. h "
斗include "arutil. h "

*detine P1 3. 1415926



 40
                                        Ch카升er 3: 加teip이a加n and Ex甘aP이카幻n          41


milt main(void)
{
     jut i, n,nfunc;
     float dy,f, 工1y1中工a,*ya;

    printf ( 'generation of interpolation tables\n") ;
    printf ( " . . . sin(x)     0<x<PI\n") ;
    printf ( " . . . e工p（工）     0＜工＜1 \n") ;
    printf ( "how many entries go in these tables?\n") ;
    if (scanf ( "%d", 幻l) == EOF) return 1;
    xa=vector (1,n) ;
    ya= vector (1,n) ;
    for (nf nc=i; nfunc<=2;nfunc++) {
         if (nfunc == 1) {
              printf ( "\ nsine function from 0 to PI\n") ;
              for (i=1;i<=n; i++) {
                    工a［幻 =1叩I/n;
                    y缸i] =sin（工a口n ;
             J.
        } else if (ufunc == 2) {
            printf ( "\ nexponential function from 0 to 1\n") ;
            for (i=1;i<=n;i++) {
                 工a［幻 =1巾1. 0/n;
                 y虹i] =e工p伍缸口 ) ;
            }
        } else C
            break;
        }
        printf ( "\ n'/.95 %13s %16s %13s\n",
            "x" ,"f (x) ", "interpolated", "error") ;
        for (jrl; i<=10;i++) {
            if (nfunc == 1) {
                  工＝(m0 . 05+i/ 10.0)sPI;
                  f=sin（工）;
            ) else if (nfunc == 2) C
                  工＝（中0. 05+i/ 10.0) ;
                  f* e工p（工）;
            }
            polmnt (xa,ya,n,x,ky,kdy) ;
            printf ( "%12.6f %12. 6f %12. 6f %4s %lif\ n",
                  x,f, y," ", dy) ;
        }
        printf ( "\n              0                        \n") ;
        printf ( "prees RETUFtI\n") ;
        (void) getcharO;
    }
    free_vector (ya, 1,n) ;
    free_v.ctor (xa,1,n) ;
    retul그10;
}

    ratint is functionally similar to polint in that it also returns a value y for the
function at point x, and an error estimate dy as well. In this case the values are
determined from the unique diagonal rational function that passes through all the
reference points. If you inspect the driver closely, you will find that two of the test
    42       Num帥ca샤？e叩os Exa／까1e Book

points fall directly on top of reference points and should give exact results. The
remainder do not. You can compare the estimated error dyy to the actual error
jyy - yexpi for these cases.
/* Driver for routine ratint */

#include <stdio . h>
#include <math.h>
#inclnde 'nr.h"
#jnclude 11nrutil. h11

#define NPT 6
#define EPS 1. 0

float f (float x,fl oat eps)
{
         return x本exp(- 工）/(S（그ft（工-1. 0) +eps布eps) ;
}

jut main(void)
{
         jut i;
         float dyy，工x, ye工p, yy！卞工1京y;

         x=vector (1,NPT) ;
         y=vector (1,NPT) ;
         for (irl; i<=NPT; i++) {
             x［幻＝1卞2. 0/NPT;
             y[i] =f (x[ i] ,EPS) ;
         }
         printf ( "\ nniagonal rational functjon interpolation\ n") ;
         printf ( '\ n7.Ss %13s %14s Y,12s\n' , "x ', "interp. ", "accuracy", "actual") ;
         for (i=1;i<r10; i++) {
             xx=0 .2* j;
             ratint (x, y,NPT, xx,&yy, &dyy) ;
             yexp=f (xx,EPS) ;
             printf ( "%6. 2f %12. 6f     %llf %13. 6f\ n". xx.yy,dyy,yexp) ;
         }
         free_ vector (y, 1, NPT) ;
         free_ vector (x, 1,NPT) ;
         return 0;
}

    Procedure spline generates a cubic spline. Given an array of x1 and f (xi), and
given values of the first derivative of function f at the two endpoints of the tabulated
region, it returns the second derivative of I at each of the tabulation points. As an
example we chose the function sin x and evaluated it at evenly spaced points x Ci] .
In this case the first derivatives at the end-points are ypi = cos x1 and ypn = cos XN.
The output array of spline is y2Ci] and this is listed along with -sinxi, the second
derivative of sin x2, for comparison.
/中 Driver for routine spline */

#include <stdio . h>
#include <math.h>
*include "nr. h11
                                            Gb카片er3: In旭'p이at幻n and Ex打까）이計幻n      43

#include 'nrutil. h"

#define N 20
#define P1 3. 1415926

mllt main(void)
{
     jot i;
     float ypl, ypn,卞工1中y1卞y2;

    x=vector (1,N) ;
    y "vector (l ,N) ;
    y2=vector (i ,N) ;
    printf ( "\ nsecond-derivatives for sin(x) from 0 to pi\ n") ;
    /卞 Generate array for interpolation s/
    for (i= 1; i<"20; i++) {
         x[i] =i卞PI/N;
         虹口=smn(x[ ij) ;
    }
    /卓 calculate 2nd derivative with spline 京1
    ypl"cos (x[ l] );
    카n=cos 伍 [N] ) ;
    spline(x, y,N, ypl, ypn,y2) ;
    ／京 test result 卞／
    prmntf ( " 工23s Y.168\n", "spline", "actual") ;
    prmntf ( "%lls %14s %16s\n" ,"angle", '2nd deniy' ,"2nd deniy') ;
    for (i=1; 1＜二甘；i++)
         printf ( "%10. 2f 工16. 6f h16. 6f\ n", x[ij, y2[i] ,-sin (x[ i] ));
    f nec_ v ector ( y2 , 1, N) ;
    fre乞加比or (y, 1, 助 ;
    free_ vector (x, 1, 甘) ;
    return 0;
}

     Actual cubic-spline interpolations, however, are carried out by splint. This rou
tine uses the output array from one call to spline to service any subsequent number
of spline interpolations with different x's. The demonstration program xsplint tests
this capability on both sill x and exp X. Tile two are treated ill succession according
to whether nfunc is one or two. In each case tile function is tabulated at equally
spaced points, and tile derivatives are found at the first and last point. A call to
spline then produces an array of second derivatives y2 which is fed to splint. The
interpolated values y are compared with actual function values f at a different set of
equally spaced points.
／卞 Driver 如r routine splint 方／

#include <stdio .h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

#define NP 10
#define P1 3. 1415926

mllt mamn(void)
{
 44       Nume欣：削／拓C徊es Exan冽e Book

      mnt i, nfunc;
      float f, 工, y,ypl, ypn.卓工a,巾ya．京y2;

      xa"vector (l, NP) ;
      ya=vector (1,NP) ;
      y2=vector (1,NP) ;
      for (nfunc=1;nfunc<=2;nfunc++) {
          if (nfunc == 1) {
              printf ( "\ nsine function from 0 to pi\ n") ;
              for (i=1; i<=NP; i++) {
                    xa[i] =i*PI/NP;
                    ya［幻 =sin伍缸ii ) ;
               }
               ypl=cos (xa[1] );
               ypn=cos (xa (NPJ) ;
           } else if (nfunc == 2) {
               printf ( "\ nexponentia]. function from 0 to 1\n") ;
               for (i=1, j<=NP; i++) {
                    工a[i] =1. 0中1／甘F;
                    ya[i] =e工p（工aCi] ) ;
               }
               ypl=exp(xa[1] );
               ypO=exp（工a대키 ) ;
           } else {
               break;
          }
          /卞 Call spline to get second derivatives */
          spline(xa, ya,NP, ypl, ypn.y2) ;
          /字 Call splint for interpolations 卞/
          printf ( "\ nY.9s '1.138 %17s\n", "x", "f (x) ", "mnterpolation") ;
           for (i=1; i<=10; i++) {
               if (nfunc == 1) {
                   x= (- 0.05+i/ 10. 0）町江；
                   f=sin(x) ;
               } else if (nfunc == 2) (
                   x = -0. 05+i/ 10. 0;
                   f=exp（工） ;
               }
               splint (xa, ya, y2,I1P, x,ky) ;
               printf ( " 工12. 6f %12. 6f %12.6f\ n", x,f, y) ;
           }
          printf ( "\ n卞＋卞本卞卞卞卞*＋卞巾卓5*＋方卞巾卞中中*中卞卞＋巾卞卞巾＋5*수＼n,,) ;
          printf ( "Press RETURN\n") ;
          (void) getcharO;
      }
      free_ vector (y2, 1,1
                          (P) ;
      free_ vector (ya, 1,1(P) ;
      free_ vector (xa,1,NP) ;
      return 0;
:j

    The next program, locate, may be used in conjunction with any interpolation
method to bracket the x-position for which f (x) is sought by two adjacent tabulated
positions. That is, given a monotonic array of x, and given a value of x, it finds
the two values xi, n+l that surround x. In x].ocate we chose the array x2 to be
non-uniform, varying exponentially with i. Then we took a uniform series of x-values
                                          Ch햐）旭r 3: Inteipolat幻n and Ex打까）이計幻n       45

and sought their position in the array using locate. For each x, locate finds the
value j for which xx[J] is nearest below x. Then the driver shows j, and the two
bracketing values xxCj] and xxCj+1]. If j isO or N, then xis not within the tabulated
range. The program then flags 'lower tim' if x is below xx[1] or 'upper urn' if x is
above xx [N] .
/* Driver for routine locate */

#include <stdio . h>
卞mnci皿da <math.h>
#include "nr.h"
*include "nrutil .h11

#dafifle N 100

mllt main(void)
{
     山lsigned long i. j;
     float; 치 +x工；

    工工＝vector (1, 助 ;
    /／中 create array to be sea工ched 卞／
    for (i=1; i<=N;i++)
         xx[i] =exp(i/ 20 . 0)-74.0;
    printf ( "\ nrasult of: j=0 indicates x too small\n") ;
    printf ( "/.lls j=100 indicates x too laxge", " ") ;
    printf ( "\ n%lo日 7.6s %ils 工12s \n". "locate ", "j ", 'xx(j) ", "xx(j+1) ') ;
    ／卓 perform test 卞／
    for (i=1;i< '19; i++) {
         x = -100. 0+200.0*i/ 20.0;
         locate（工工，瓦x，幻）;
         if ( (j- < N) U (j >0) )
              printf ( '%10. 4f %61u %12. 6f %12.6f\n",
                   工，j . x工［j]，工x[ j+1] ) ;
         else if (j == N)
              printf ( "%10.4f X6lu %12. 6f 加\n",
                   x, j, xx[ j] ,"  upper lim") ;
         else
              printf ( "Y.10. 4f %61u 加 %12. 6f \n",
                   工，J, "     10日er lim", 工工［j+l] );
    }   .



    free_vector (xx,1,N) ;
    return 0;
}

     Routine hunt serves the same function as locate, but is used when the table
is to be searched many times and the abscissa each time is close to its value on the
previous search. xhunt sets up the array xx[i] and then a series x of points to locate.
The hunt begins with a trial value ji, (which is fed to hunt through variable j) and
hunt returns solution j such that x lies between xxij] and xx[ j+1]. The two cases
j= 0 and j=N have the same meaning as in xlocate and are treated in the same way.
／卞 Driver 如r routine hu끄t 衣／

#inciude <stdio .h>
#include <math.h>
    46       Numerica/ 尸cc徊es Examp旭 Book

#include "nr. h"
*include "nrutil. h"

#define N 100

jut main(void)
{
         unsigned long i, j, ji;
         float; 工1卞xx;

         工工＝vector (1, N) ;
         /* create array to be searched 卞/
         for (i '1; i<=N; i++)
             xx[i] =exp(i/ 20.0) -74.0;
         printf ( "\ n result of:    j=0 indicates x too small\n") ;
         printf ( " 工14s j=100 indicates x too large", " ") ;
         printf ("\ n%12s %85 %4s 工lls %13s \n",
              "locate: ", "guess", "j ", "xx(j) ", "xx(j+ l) ") ;
         /／卞 do test; 李／
         for (ir1; i<=19; i++) {
              x = -100.0+10.0*i;
              ／京 trial pa工ameter 字／
               j= (3i=5*i) ;
              /* begin search */
              hu끄t仕x，瓦x，幻 ) ;
              if ( (j <N) &t (j >0) )
                  printf ( "%12.5f %61u %61u %12.6f 工12. 6f \n",
                       x, ji, j : 工x [j] ，工工 [j+ l] ) ;
              else if (j == N)
                  printf ( "%12. 5f %61u %61u %12. 6f %s \n",
                      x, ji, j, xx[ j] ,"  upper lim") ;
              else
                  printf ( "/.12.5f 工61u X6lu 加 '/.12.6f \n".
                      x, ji, j , "   lo日er ii皿"，工工［j+1] );
         }
         free_vector (xx, 1,N) ;
         return 0;
    }

         The next two demonstration programs, xpolcoe and ipolcof, are so nearly iden-
    tical that they may be discussed together. polcoe and po].cof themselves both find
    coe用cients of interpolating polynomials. In the present instance we have tried both
    a sine function and an exponential function for ya[i] , each tabulated at uniformly
    spaced points xa[11. The validity of the array of polynomial coe岱cients coeff is
    tested by calculating the value su皿 of the polynomials at a series of test points and
    listing these alongside the functions f that they represent.
    ／卞 Driver 如r routine F口lcoe +/

    *include <stdio.h>
    #include <math.h>
    #include "nr. h"
    *include "nrutil .h"

    #define NP 4
    *define P1 3. 1415926
                                          Ch可月er3: Interp이at幻n and E났ra.polat幻n   47


 jilt main(void)
{
     jilt i口. nfunc;
     float f, su丘1工1卞coeff, 京xa,中ya;

    coeff=vector (O ,IP) ;
    xa=vector (O,NP) ;
    ya=vector (O, JP) ;
    如r (nfunc=1;nf띠lC<=2;nfu小＋+) {
        if (nfwic == 1) {
            printf ( "sine function from 0 to PI\n\n") ;
            for (i= O; i<"NP; i++) {
                 工a［口= (i+ j汁PI/ (NP+1) ;
                 ya[i] =sin(xa[i] );
             }
         } else if (nfunc == 2) {
             printf ( "exponential function from 0 to l \n\ n") ;
             for (i= O; i<=JP; j++) {
                  xa[i] =1. Os (j+ 1) /(NP+1) ;
                  ya［口 =0자）(xa[i] ) ;
             }
         } else {
             break;
        )
        polcoe(xa, ya.NP, coeff) ;
        printf ( " coefficients\ n") ;
        for (i= 0; i<=1P; i++) printf ( "Y.12. 6f ", coeff[i] );
        printf ( "\ n\n%9s %13s %1&s\n", "x ' , "f (x)", "polynomial") ;
        for (i=1; i<=10;i++) {
            if (nfunc == 1) {
                  X=（느0. 06+i/ 10. 0）中P1;
                  f=sin（工）;
            } else if (nfunc == 2) {
                  x = -O. 05+i/ 10. O;
                  f=e工p（工） ;
            }
            sum=coeff [IP] ;
             for (j "IP-l; j>=O; j- -)
                 su皿＝coeff [j] +su皿*工 ;
             printf ( "Y.12.6f )12.6f %12. 6f\ n", x,f, sum) ;
        }
        printf ( "\                                              \n") ;
        printf ( "press RETURI\n") ;
        (void) getcharO;
    }
    free_vector (ya,0 , NP) ;
    free..vector (xa,O,NP) ;
    free.-vector (coeff ,0,IP) ;
    return 0;
}

/* Driver for routine polcof *1

甘include <stdio . h>
tjnclude <math.h>
#include "nr. h"
48           N切"9放：a／尸e（巾es Example Book

#include "nrutil. h"

*define NP 4
#define P1 3. 1416926

mnt main(void)
{
        mnt i口, nfunc;
        float f ：日'I工'I '卞coeff ax히＋ya;

        coeff=vector (o,NP) ;
        xa=vector (0, NP) ;
        ya'vector (0,NP) ;
        如r (nfui比＝1; nf山ic<=2 ;nf山lC++) {
            if (nfu끄c == 1) {
                printf ( "sine function from 0 to PI\n\n") ;
                for (i= 0; i<=NP; i++) {
                      工a［幻 = (i+ I 汁PI/ (NP+l) ;
                      ya［幻 =B lfl (工aCi] ) ;
                  }
             } else if (nfunc == 2) {
                 printf ( "exponentia.l function from 0 to 1\n\n") ;
                 for (i= 0; i<=NP; i++) {
                      工a［幻 =1. 0卞 ( i+1) /(IP+1) ;
                      ya［舒 =a工可xa[i] ) ;
                   }
              } else {
                  brea上；
              }
              polcof (xa, ya, NP, coeff) ;
              printf ( " coefficients\ n") ;
              for (i=0; i<=NP; i++) printf ( "%12. 6f ", coeff[il) ;
              printf ( "\ n\n'/.9s V.13s Y,15s\n", "x", "f (x)", "polynomia].") ;
              for (i "l; i<=lO; i++) {
                  if (nfunc == 1) {
                        x=(- 0 .05+i/ 10.0)*PI;
                        f=sin（工） ;
                  } else if (nfunc == 2) {
                        x = -0. 05+i/ 10.0;
                        f=e工P（工）;
                   }
                   sum=coeff [NP] ;
                   如r (j=N肛1; j>=0; j- -)
                       su皿＝coeff (j) +su皿巾工 ;
                   printf ( "V.12.6f %12. 6f %12. 6f\ n", x,f, sum) ;
              }
              prmntf ("\                                                \n") ;
              printf ( "press RETU1N\n") ;
              (void) getcha工O;
         }
         free_ vector (ya, 0, NP) ,
         frae_ vector (xa, 0, NP) ;
         free_ vector (coeff, 0,IP) ;
         return 0;
    }

         For two-dimensional interpolation, polin2 implements a bilinear interpolation.
                                          Ch햐月or 3: Interpolal幻n and Extr邵）이計幻n    49

We feed it coordinates xla,x2a for an M x N array of gridpoints as well as the
function value at each gridpoint. In return it gives the value y of the interpolated
function at a given point xl, x2, and the estimated accuracy dy of the interpolation.
xpo1in2 runs the test on a uniform grid for the function f (x, y) = sin x exp y. Then,
for an offset grid of test points, the interpolated value y is compared to the actual
function value f, and the actual error is compared to the estimated error dy.
/s Driver for routine p011n2 */

#include <stdio.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

*daf in. N &
#define P1 3.1415926

mnt main(void)
{
     mnt i, j;
     float dy,f, 工1, x2, y, *工la！卞工2a1卞卓ya,

    工la=vector (1, 月）;
    x2a=vector (1IN) ;
    ya=matri工（1, 瓦 1.N) ;
    for (i= 1;i<=N; j++) {
        工la［幻 =1朴江／N;
        for (j=1; j<=N; j++) {
             工2a[ j] r1. O中j/N;
             ya［幻 [j] =sin（工la[ij ）巾e工p(x2a[ jj ) ;
        }
    ：卜
    /* test 2-dimensional interpolation */
    pri小f ( "\ nTwo dimensional interpolation of sin(xl) exp(x2) \n") ;
    printf ( "%9s 7.12. %13s 7.16. %lls\n",
        "x1", "x2' . "f (x) ", "interpolated' , "error") ;
    for (i=1;i<=4; i++) {
        工1=（田. 1+i/ 5 . 아中p工；
         for (j=1; j<=4; j++) {
              x2 = -O. 1+ j/ 5. O,
             f=sin(工l汁e工p仕2) ;
             p01in2(xla, x2a. ya，瓦瓦 工1 ,x2，幻小幻）;
             printf (1'%12.6f /.12. 6f %12. 6f %12. 6f %15. 6f\ n",
                  xl, x2, f, y.dy) ;
         }
         printf ( "                                         \n") ;
    }
    free_matri工（ya, 1, 月，1，且）;
    free_ vector (x2a, 1,N) ;
    free...vector (xla. 1.N) ;
    return 0;
}

    Bicubic interpolation in two dimensions is carried out with bcucof and bcuint.
The first supplies interpolating coefficients within a grid square and the second cal-
culates interpolated values. The calculation provides not only interpolated function
50     肌imeric削尸ec徊es Exa쨔1e Book

values, but also interpolated values of two partial derivatives, all of which are guar-
anteed to be smooth. To get thi옥 we are required to supply more information than
we have needed in previous interpolation routines.
     Demonstration program xbcucof works with the function f (x, y) = xy exp(- xy).
                                                                                   func-
The program computes the two first derivatives and the cross derivative of this
tion at the four corners of a rectangular grid cell, in this case  a  2 x 2 unit square
with one corner at the origin. The points are supplied counterclockwise around the
cell. dl and d2 are the dimensions of the cell. A call to bcucof provides the following
sixteen coe佈cients, listed for comparison.
Coeffjcient8 for bicubic interpolation:
   0. 000000    0.000000    0.000000     0.000000
   0.000000     4.000000    0.000000     0.000000
   0.000000     0. 000000 -13.655600     6.095174
   0.000000     0.000000    6.095174    -2. 461486


/s Driver for routine bcncof */

#includa <stdio .h>
#include <math.h>
#include "nr. h"
*include "nrutil. h"

mllt mamn(void)
{
     mit i, j;
     float d11d21ee,工1工2;
     float y[5] ,yl[ 5] ,y2[5] ,y12[S] ,**c;
     Static float x1D={0.0, 0.0,2.0,2.0,0.0} ;
     static float x2口={0.0,0.0,0.012.0,2.0} ;

     c=matrix(1,4,1,4) ;
     dl=xl[ 2]-xlCl] ;
     d2=x2[4] -x2[1] ;
     for (i=1; j<=4; j++) {
         xlx2＝工I [i] 卞工2 Ci] ;
         ee=e工p(＝工1工2) ;
         虹i] ＝工1工2*ee;
         ylCi] =x虹i] * (1.아工1工2汁cc;
         y2[i] ＝工1 Ci] 李（1. 0-工1工2) *ee;
         yl玎i] =(1.0-3. 0卞工1工2＋工1工2巾工1x2汁cc;
     }
     bcucof (y , yl, y2 , y12,dl , d2, c) ;
     prmntf ( "\ nCoefficients for bicubic interpolation: \n\n ") ;
     for (i=1; i<=4; i++) {
         for (j=1; j<=4; j++) printf ( '%12.6f ", cCi] Ej] );
         printf ( "\ n ') ;
     }
     free_matrix(c, 1,4,1 14) ;
     return 0;
 }

     Program xbcuint works with the function f (x, y) = (xy)2, which has derivatives
 Of/Ox = 2工y2, Of/Oy = 2yx2, and 伊1/ t9x야／ = 4xy. These are supplied to bcuint
 along with the locations of the grid points. bcuint calls bcucof internally to deter-
                                                C力아升er 3: Interpolaf幻n and Extr카刃伯r幻n      51
    mine coe佈cients, and then calculates ansy, ansyl, ansy2, the interpolated values
                                                                                      of
    f, Of/ax and Of/Op at the specified test point (xl , x2). These are compared by the
    demonstration program to expected values for the three quantities, which are called
    ey, eyl, and ey2. The test points run along the diagonal of the grid square.
    /卞 Driver for routine bcuint */

    #include <stdio. h>
    #include "nr. h"

    jut main(void)
 {
        jut i;
        float ansy, ansyl,ansy2, ey, eyl, ey2;
        float 工1, xll, 工lu，工1x2, x2, x21，工2u, xxyy;
        float y[5] ,yl[ 5] ,y12[5] ,y2[5] ;
        static float xxD= {O. 0,0. 0, 2. 0, 2.0,0. 0);
        static float yy口＝{0. 0,0. 0,0. 0,2.0, 2. 0} ;

       工11=x工［1] ;
       xlu＝工x［幻 ，·
       x2l'yyE1] ;
       x2u=yy [4] ;
       for (i=1; i<=4; i++) {
            工工yy=x工 [1] 中yy[i] ;
            玎i] ＝工xyy中xx刈；
            戶 Ci] =2. 0中刃 [i] *xxyy;
            y2[i] =2. 0京工x Ci] 中xxyy;
            112[i] =4. 0中x工yy;
       }
       printf ( "\ n%6s 工8s %7s '1.118 /.6s '/,lOs V.6s Y.los \n\ n",
            "xl " ,"x2", "y ", "expect " , "yl " , "expect " ,"y2" ,"expect ") ;
        for (i=1; i<r10; i++) {
            工2=（工1=0. 2卞i) ;
            bcnint (y, yl, y2, y12, xll, xlu, x21, x2u, xl, x2,&ansy, &ansyl,k카lsy2) ;
            工l工2＝工l 中工2;
            ey=xl工2＋工 l工2;
            ey1=2. 0字x2字工 l工2;
            ey2=2 .0卓xl卞工1工2;
            printt ( "%8. 4f %8. 4f %8. 4f '/.8. 4f %8. 4f '/.8. 4t '/.8. 4f %8. 4f\ n",
                 xl, x2,ansy, ey, a工lsyl, eyl, 카lsy2, ey2) ;
       }
       return 0;
}

     Routines splie2 and splin2 work as a pair to perform bicubic spline
                                                                              interpo
lations. splie2 takes a function tabulated on an M x N grid and performs
                                                                                   one
dimensional natural cubic splines along the rows of the grid to generate
                                                                          an array of
second derivatives. These are fodder for splin2 which takes the grid
                                                                     points, function
values, and second derivative values and returns the interpolated function value
                                                                                  for a
desired point in the grid region.
    Demonstration program xsplie2 exercises splie2 on a regular 10 x 10 grid of
points with coordinates xl and x2, for the function y = (x1x2)2. The calculated
second derivative array is compared with the actual second derivative 2x1x2 of
                                                                                the
function. Keep in mind that a natural spline is assumed, so that agreement
                                                                           will not
    52      Numerical Recipes Example Book

be so good near the boundaries of the grid. (This shows that you should not assume
a natural spline if you have better derivative information at the endpoints.)
/* Driver for routine sp1ie2 中/

Ninclude <stdio. h>
#include "nr. h"
#include 'nrutil. h"


#def ins M 10
#define N 10


mnt main(void)
{
         mnt i, j;
         float 工l工2, 5工l 's工2,巾巾y1中* y2;


         xl=vector (1 ,N) ;
         x2=vector (1, N) ;
         y=matrix (1，甘 , 1, 甘） ;
         y2rmatrix (1,M, 1 , 月) ;
         如r (i= 1; i< =M; i++) 工l [i] =0. 2中1;
         如r (i= 1 ; i<＝甘·. i++) 工2［幻＝0. 2卞1;
         for (i= 1; i< =M; i+ +)
              for (j= 1; j<=N; j++) {
                  工l工2=x1 [i] *工2[ j] ;
                  虹口［刃 =xl工2中xl工2;
              1
         sp1ie2 (xl, x2, y,M, 瓦y2) ;
         printf ( "\ nsecond derivatives from SPLIE2\n") ;
         printf ( 'natural spline assumed\n") ;
         for (i= 1; i< =5; i++) {
              for (j= 1; j<=5; j++) prmntf ( "%12. 6f ", y2[i] lj] );
              prmntf ( "\ n ") ;
         }
         pl-intf ( "\ nactual second derivatives\ n") ;
         for (i= 1; i<=5; i++) {
                                                                     中工1[i] );
              for (j= 1; j<=5; j++) printf ( " 工12. 6f ", 2. 0中工1 [1］
              printf ( "\ n ") ;
         }
         fre&.matrix (y2,1,11, 1,N) ;
         free_matrix (y, 1,14,1,N) ;
         free_ vector (x2,1, N) ;
         f re e..vector (工l, 1, N) ;
         return 0;
    }

        The demonstration program xsplin2 establishes a similar 10 x 10 grid for the
    function y = x1x2 exp(- x1x2). It makes a single call to splie2 to produce second
    derivatives y2, and then finds function values f through calls to splin2, comparing
    them to actual function values ft. These values are determined, for no particular
    reason, along a quadratic path x2 = x孑 through the grid region.
    /5 Driver for routine ap1in2 中/

    *include <stdio .h>
    Ninclude <math.h>
                                                 Ch긔oter3: In油加胤幻n and E났r叩叱加n    53
    #include 'nr. h"
    #include 11nrutil. h'1

    #dafina N 10
    #define N 10

    mllt main(void)
    {
         mllt i. j;
         float f, ff, 工l工2,工xl,工工2，卞工i. e工2, *巾y1卞李y2;

         xl 'vector (l .1) ;
         x2=vector (1,J) ;
         y=matrix (l .11,1,N) ;
         y2=matrix (1,N,1, J) ;
         for (i=1; i<=N; i++) xl[ i) =0. 2si;
         for (i=1; i<=N; i++) x2[i] =0. 2中i;
         for (i=1; i<=N; i++) {
              for (j=1; j<=N; j++) {
                  工l工2＝工lCm] 吐缸jJ ;
                  虹ij Eu]＝工1工2中a工pC- 工1工2) ;
              }
        }
        sp1ia2(工l. x2, y,N,N, y2) ;
        priutf ( "%9s V.128 Y.14e Y.12s\n", "xl ", "x2", 'sp1in2", "actual") ;
        for (i=1; i<=10; i++) {
            工工1=0. Isi;
            工工2＝工工l字工工1;
            sp1in2(xi , 工2, y, y2,M, 瓦 工工1 , 工工2, kf) ;
            工l工2＝工工1中x工2;
            tt＝工l工2卞axp (- xl工2) ;
            printf ( '%1216f '/.12. 6f %12. 6f %12. 6f\ n' , xxl, xx2, f, ff) ;
        }
        fras_matri工（y2, l, 瓦 1,助 ;
        frea_matrix (y. 1，瓦 1,助 ;
        free_ vector (工2, 1,N) ,
        f rae_ v act or（工1, 1, 月） ;
        return 0;
}
Chapter 4: Integration of Functions

       Numerical integration, or "quadrature", has been treated with some de-
  gree of detail in Numerical Recipes. Chapter 4 begins with trapzd, a function
  for applying the extended trapezoidal rule. It can be used in successive calls
  for sequentially improving accuracy, and is used as a foundation for several
  other programs. For example qtrap is an integrating routine that makes re-
  peated calls to trapzd until a certain fractional accuracy is achieved. qsimp
  also calls trapzd, and in this case performs integration by Simpson 's rule.
  Hornberg integration, a generalization of Simpson's rule to successively higher
  orders, is performed with qroxnb - this one also calls trapzd. For improper
  integrals a different "workhorse" is used, the procedure midpnt. This rou-
   tine applies the extended midpoint rule to avoid function evaluations at an
  endpoint of the region of integration. It can be used in qtrap or qsimp in
  place of trapzd. Routine qromb can be generalized similarly, and we have im-
  plemented this idea in qromo, a Romberg integrator for open intervals. The
   chapter also offers a number of exact replacements for midpnt, to be used for
   various types of singularity in the integrand:
      1.
         midinf - if one or the other of the limits of integration is infinite.
      2.
         midsql - if there is an inverse square root singularity of the integrand at
         the lower limit of integration.
      3. midsqu - if there is an inverse square root singularity of the integrand at
         the upper limit of integration.
        4. midexp - when the upper limit of integration is infinite and the integrand
           decreases exponentially at infinity.
           The somewhat more subtle method of Gaussian quadrature uses unequally
      spaced abscissas, and weighting coefficients which can be read from tables.
      Routine qgaus computes integrals with a ten-point Gauss-Legendre weight-
      ing using such coefficients. gauleg, gaula.g, gauher and gaujac calculate the
       tables of abscissas and weights for N-point Gauss-Legendre, Gauss-Laguerre,
       Gauss-Hermite and Gauss-Jacobi quadratures, respectively. The routine or-
      thog lets you construct nonclassical orthogonal polynomials, while gaucof lets
      you find the abscissas and weights for the corresponding Gaussian quadrature.



     trapzd applies the extended trapezoidal rule for integration. It is called sequen-
tially for higher and higher stages of refinement of the integral. The sample program



 54
                                                    Ch랴）旭r 4: Integral幻n 可Func抛ns       55
    xtrapzd uses trapzd to perform a numerical integration of the function

                                     tunc = x2(x2 - 2) sin x
    whose indefinite integral is

                       tint = 4x(x2 - 7) sinx -(x4 - 14x2 + 28) cosx.
    The integral is performed from A = 0.0 to B = 冗/2. To demonstrate the increasin{
    accuracy on sequential calls, trapzd is called 14 times with the index i increasing b1.
    one each time. The improving values of the integral are listed for comparison to th(
    actual value fint (B) - fint (A).
    /5 Driver 如r ro끄tine trapzd 卞／

    #include <stdio . h>
    #include <aath.h>
    #include "nr. h"

    作defi五e INA工 14
    甘define P102 1.5707963

    /s Test function */
    float func(float x)
{
       return （工卞工汁（工巾x-2. 0）相in(x) ;
}

／卞 工ntegra]. of test function 卞／
float fint (float 工)
{
       return 4.0卞工K工串x-7. 0）卞sin(x)-(po므（치4. 0)-14. 0*（工＋x)+28 .Q) *cos
                                                                        （功 ;
}

lot maia(void)
{
    ml1t i;
    float a=0.O,b=P102, s;

       printf ( "\ nlntegral of func with 2 (n-1) points\n") ;
       prmntf ( "Actual value of integral is Y.10.6f\ n", fint (b)-fint (a) );
       printf ( "%6s %24s\n". "n" ,"approx. integral ") ;
       for (i= 1;i<=JMAX; i++) (
            s=trapzd(func,a,b, i) ;
            prmntf ( "%6d %20. 6f\ n ", i, s) ;
       }
       ret1｝工且 0;
}

    qtrap carries out the same integration algorithm but allows us to specify th(
accuracy with which we wish the integration done. (It is specified within qtrap
                                                                                a
EPS=1. OE-6.) qtrap itself makes the sequential calls to trapzd until the desire(
accuracy is reached. Then qtrap issues a single result. In sample program
                                                                           xqtraj
we compare this result to the exact value of the integral.
    56       Nume力cal Rec徊es Examp旭 Book

／巾 Driver 如r routine qtrap 卞／

#include <stdio .h>
*include <math.h>
#include "nr. h"

#def ins P102 1. 5707963

／卞 Test function 卞／
float func(float x)
{
          retu工n 工方工KX中工口．0）相in(幻 ;
}

/* Integral of test function 卞/
float fint (float x)
{
          return 4. 0＋工卞（工方x-7. 0）中Bin（工）-(p<）日（工，4.0)-14.0*x＋工＋28. 0）巾COB（工） ;
}

mllt main(void)
{
          float a=0.0,b=P102, e;

          printf ( "Integral of func computed with QTRAP\n\n") ;
          printf ("Actual value of integral is %12. 6f뇨", fint (b)-fint (a) );
          s=qtrap (f끄c. a,b) ;
          printf ( "Result from routine QTRAP is %12. 6f\ n", s) ;
          return 0;
}

    Alternatively, the integral may be handled by qsimp which applies Simpson's rule.
 Sample program xqsimp carries out the same integration as the previous program,
 and reports the result in the same way as well.
／方 Driver 如r routine qsimp 字／

    #include <stdio.h>
    #include <math. h>
    #include "nr. h"

    #define P102 1.5707963

／小 Test function 卓／/
float func(float x)
    {
          return x半x京（工卓x-2.0）衣sin(x) ．·
    }
    /方 Integral of test function */
    float fint (float x)
    {
          ret1工rn 4. 0斗工卓（x巾工-7.0) *sin（工）-(po日（工，4.0) -14. 0卞工＋工＋28. 0）京cos（工） ;
    :1.
    mllt main(void)
    {
                                                      Ch햐ter 4: Integration of Functions   57
         fl oat a=0. O,b=PI02, s;

         printf ( "Integra]. of .I unc computed with QSIMP\n\n,") ;
         printf ( "Actua]. value of integral is '/.12. 61\n", fint (b)-fint (a) );
         s=qsimp(func,a,b) ;
         printf ( "Result from routine QSIMP is %11. 6f\ n", s) ;
         return 0;
    }

     qroinb generalizes Simpson's rule to higher orders. It makes successive calls
 to trapzd and stores the results. Then it uses polint, the polynomial interpo-
later/extrapolator, to project the value of integral that would be obtained were we
to continue indefinitely with trapzd. Sample program xqromb is essentially identical
to the sample programs for qtrap and qsimp.
／巾 Driver 如r routine qromb 卞／

 #include <stdio .h>
 #includa <math.h>
 #include "nr. h"

 #define P102 1.5707963

／中 Teat function 卞／
float fi끄ic (float 工）
{
        return 工中x卞（工京工＝2. 0）李sin(x) ;
}

/卞 Integral of test function func */
float fint (float x)
{
        return 4.0*x卞（x卞工＝7. 0) tsin（工）-(po日（x, 4.0)-14. 0卞工＋工＋28. 0）巾cos (x) ;
}

mnt main(void)
{
        float a=0. 0,b=PI02, s;

        printf ( "Integral of func computed with QRONB\n\n") ;
        printf ( "Actual value of integral is Y.12.6f\ n", fint (b)-fiut (a) );
        e'qromb(func,a,b) ;
        printf ( "Result from routine QROMB is %11. 6f\ n", s) ;
        ret1口그L 0;
}

    Sample program xinidpnt uses the function func = 1/ \/三 which is singular at
the origin. Limits of 'integration are set at A = 0.0 and B = 1.0. midpnt, however,
implements an open formula and does not evaluate the function exactly at x = 0.
In this case the integral is compared to fint (B) - fint (A) where tint = 入／云 the
integral of func.
/s Driver for routine midpnt 斗/

#include <stdio .h>
#include <math.h>
 58       Numerical Recipes Example Book

*include "nr. h'1

#define IHUX 10

／卞 Test function 卞／
fl oat func (float x)
{
      return 1. 0/ sqrt (x) ;
}

/* Integral of test function 字/
float fint (float x)
{
       return 2. 0*aqrt (x) ;
}

ml1t main(void)
{
       float a=0. 0,b=1. 0, s;
       m11t i;

       printf ( "'\ nlntegral of func computed with MIDPNT\n") ;
                                                                       t (a) ));
       printf ( "Actual value of integral is 工7. 4f\ n", (fint (b)=fin
       printf ( "%68 Y.29s \n", "n", "Approx. integral ') ;
       for (i=1; i<=NNAX; i++) {
           s=midpnt (func,a,b,i) ;
           printf ( "Y,6d Y.24.6f\ n", i, s) ;
       }
       return 0;
}

     Various special forms of midpnt (i.e., midsql, midsqu, midinf, midexp) are
                                                                               to infin-
demonstrated by sample program xqromo. For those tests that integrate
ity, we  take infinity to be l.0E20. The following integrations are performed:

  1. Integral of J/ sin x from 0.0 to 丁/2. (This has a l/ .,도 singularity at x = 0, and
       uses midsql.)

    2. hit哨如 V二司鈿如m 귀如 冗· (This h朗 the l/\／三singul町ity at the
       upper limit x = 兀, and uses midsqu.)
    3. Integral of (sin x)/x2 from ir/2 to n工 (This has a region of integration extending
       to no and uses inidiuf. It is quite slowly convergent, as is the next integral.)
    4. Integral of (sin x)/x2 from -아） to -町/2. (Region of integration goes to -no; uses
       midinf.)
    5. Integral of exp(- x)/,三 from 0.0 to no. (This has a singularity at x = 0.0 and
       also integrates up to no. It is performed in two pieces, (0.0 to ir/2) and (ir/2 to
       的) using midsql and inidinf. The two calculations give results real and res2
       respectively, which are added to give the entire integral.)
    6. Same integral as in (5), but with the segment from (ir/2 to no) done using midexp.
 ／斗 Driver 如r routine qromo 中／

    #include <stdio. h>
                                                       C力카升er4: Integrat幻n of Funct幻ns    59
        *include <math.h>
        4inc1ude "nr.h"

    #define Xl 0. 0
    #define X2 1.5707963
    #define 工3 3. 1415926
    #define AIRF 1. 0520
    #define P1 3.1415926

    static float funcl(float x)
    {
           return (float) (sqrt (x)/sin (x) );
    }

    static float funcu(float x)
    {
           return (float) (sqrt (PI-x)/sin(x) );
    }

    static float fncinf (float z)
    {

           return (float) 佃in仕）/（工卞x) );
    }

    static float fncend(float x)
    {
        return (float) Ce工可吐) /叫rt仕）);
    }

    milt main(void)
    {
          float resl, res2,result;

           printf ( "\ nlmproper integrals: \n\n") ;
           result= qrolno(funcl,工1 ,X2,midsql) ;
           printf ( "Function: sqrt (x) /sin(x)       Interval: (0,pi/ 2) \n") ;
           printf ( "Using: MIDSQL                    Result: '/.8. 4f\n\n", resu].t) ;
           result=qro如（funcu,12，工3 皿idsq山 ;
           printf ( "Function: sqrt (pi- x) /sin (x)  Interval: (pi/ 2,pi) \n ') ;
           printf ( "Using: MIOSQU                    Result: %8. 4f\n\n", result) ;
           result=qromo(fncinf ,12 ,AINF,inidinf) ;
          prmntf ( "Function: sin(x)/xs*2            Interval: (pi/ 2』infty) \n") ;
           printf ( "Using: XIDINF                   Result: '/,B.4f\n\n",result) ;
          result=qronto(fncinf ,-AINF,-工2,isidinf) ;
          printf ( "Function: sin仕）／工巾中2             Interval: (- infty, -pi/ 2) \n") ;
          printf ( "Using: MIDINF                    Result: %8. 4f\n\n", result) ;
          resl=qromo(fncend,X1 ,工2,midsql) ;
          res2=groiuo (fncend,12 ,AIMF ,midmnf) ;
          printf ( 'Function: exp(- z) /sqrt (x)     Interval: (0. 0,infty) \n") ;
          prmntf ( "Using: MIDSQL,MIDINF             Result: %8. 4f\n\ n", resl+res2) ;
          res2=qromo (fncend,12, AINF ,midexp) ;
          printf ( "Function: exp(- x) /sqrt (x)     Interval: (0.0,infty) \n") ;
          printf ( "Using: 겨［I0SQL，片IDE工P            Result: '/.8.4f\n\n", resl+res2) ;
          retui口1 0;
)
60                    Numerical F治O戶es Examp旭 Bo아（

    Procedure qgaus performs a Gauss-Legendre integration, using only ten function
                                                                         xexp(- x) whose
evaluations. Sample program xqgaus applies it to the function
integral from x1 to  xis (1+ x)  exp(- xi)  -(1+    x)exp(-  x).  cgaus  returns the value
                                                                                       and
of this integral. The method is used for a series of intervals, as short as (0.0- 0.5)
as long as (0.0 - 5.0). You may observe   how   the  accuracy  depends   on  the interval.

／字 Driver 如r routine qgaus 卞／

#include <stdio .h>
Uinclude <math.h>
#include "nr. h"

#deiine Xl 0.0
#define X2 5. 0
#define NVAL 10

float                 func (iloat   x)
{
              return x卞e자：1(eX) ;
}

mnt main(void)
{
               float d工 1 S8, 工 ;
               m1lt i;

               dx" (X2-X1) /NVAL;
               printf ( "\ n%s V.los %13s\n\n", "0.0 to' , "qgaus", 'expected") ;
               for (i=1; i<'NVAL; i++) {
                    x=X1+i十d工 ;
                    ss=qgaus (func 1X1, x) ;
                    printf ( 'V.5. 2f %12. 6f 工12. 6f\ n", x, ss,
                         (- (1. 0+x汁炚可-x汁（1. 0+X1) 相叩(- Xl) )) ;
               }
               return 0;
 }
                                                                   the same method of
     Sample program xgauleg, which drives gauleg, performs
 quadrature, and on the same function. However,      it chooses  its own abscissas and
 weights for the Gauss-L egendre calculation, and is not  restricted to a ten-point for-
 mula; it can do an N-point calculation for any N. The N abscissas and weights
 appropriate to an interval x = 0.0 to 1.0 are found by sample program xgauleg for
 the case N = 10. The results you should find are listed below. Next the program
                                                                         from a formal
 applies these values to a quadrature and compares the result to that
    integration.
      #                 工［幻              日［幻
          1            0. 013047         0. 033336



            6   8 9
     2 3
                       0. 067468         0.074726
                       0.160295          0. 109543
                       0. 283302         0. 134633



          C  rm

         4V
                       0. 426563         0. 147762




        1
                       0. 574437         0. 147762
                       0. 716698         0. 134633
                       0.839705          0. 109543
                       0. 932532         0. 074726
                                                  Ch邵）伯r4: 幻旭아a加n 可Func加ns          61
     10   0.986953      0.033336

 /s Driver for routine gauleg */

 #include <日tdio .h>
 #include <math.h>
 #include "nr.h"
 #include "nrutil. h"

 #def ins 丑Par月T 10
 #def ins 工i 0. 0
 #define 12 1.0
 #define 工3 10. 0

 float func (float x)
 {
     retur끄 工方e자）(- 工）;
 }

 mllt main(void)
 {
      mnt i;
      float 工工＝0.0;
      float; 卞X1 卞日；

       x=vector (1,NPOINT) ;
       口＝vector (1, NPOI甘T) ;
       gauleg(X1.12 , x ,v,NPOINT) ;
      printf ( "\ n%2s %lOs %12s\n", "*", "x[i] ", "wli] ") ;
       for (inl; i<=NP0INT; i++)
           prmntf ( "Y.2d %12. 6f 艾12. 6f\n", i, xti] ,w[i] );
       /卞 Demonstrate the use of gauleg for integration */
      gauleg(X1,13, x,v,NPOINT) ;
       for (i=1; i<=IP0INT;i++)
           工x += （町i］巾fu恥(x[i] )) ;
      prmntf ( "\nlntegral from GAULEG: X12. 6f\n", xx) ;
      printf ( "Actual value: Y.12.6f\n",
           (1.0＋工1) te工P(＝工1) -(i. 0＋工3）卞e工p(-13) ) ;
      fre包vector佃,1,NPOINT) ;
      iree_vector (x, 1,NPOINT) ;
      retur工1 0;



    The next three sample programs are all similar to the previous one. They
                                                                             compute
abscissas and weights for some form of Gaussian quadrature and print them out. As
a check, each routine sums the weights and compares the sum with
                                                                       an analytically
known value. If the abscissas are not symmetric about the origin, their
                                                                          sum is also
nonzero and can be compared with an analytic value. Next, each
                                                                   program calculates
an appropriate integral using the coefficients just determined.
    The first such sample program, igaulag, exercises gaulag by
                                                                computing coeffi-
cients for an N-point Gauss-Laguerre quadrature. The program fixes
                                                                   the parameter
0= 1. It then calculates the integral

                                /，的
                                      ee ' 而（x)xd工 = 2H3/2
    62       Nume／祀刻／拍C加es Ex可까,!o Book

and compares the answer with the analytic result. As you will find, N of order a
dozen is enough to determine the value to full single precision.
／卞 Driver 如r routine gaulag 卞／

*include <stdio . h>
#include <math.h>
*include "nr. h "
#include "nr끄til. h"

#def ins 1? 64

float func (float x)
{
         return beasjo(x) ;
)

jut main(void)
{
    mnt i, n;
    float alf= l .0 1 check日1 cl田ck工1l工 1卞X 's口；

         x=vector (1,NP) ;
         v=vector (1,NP) ;
         如r (; ;) {
             printf ( "Enter N\n") ;
             if (scanf ( "/.d", 幻l) == EOF) break;
             gaulag(x, v,n,alf) ;
             printf ( "%3s %l0s %14s\u ", "* ", "z(i) ", "w(i) ") ;
             for (i=1;i<=n; i++) printf ( "%3d %14. 6e %14. 6e\n " ,x, z[i] 戶[i] );
             checkx=check日＝0. 0;
             for (i=1; i<=n; i++) {
                 check工 += 工［幻 ;
                 check日 += 日［幻 ;
             }
             printf ( "\ uChack value: %15.7e should be: 工15. 7e\n", checkx,n* (n+alf) );
             printf ( "\ nCheck value: 工15.7e should be: %1& .7e\n", checkw,
                 ezp(ga月mln(1. 0+a].f) ));
             /* demonstrate the use of GAULAG for an integral 卞/
             for （工工＝0.0,i=1;i<=n;i++) 工X += 미.1］字心nc（虹玎）;
             printf ( "\ nlntagra]. from gaulag: %12. 6f\ n ", xx) ;
             printf ( "kctua]. value:          %12. 6f\ u" 小0/ (2.0*sqrt(2.0)));
         }
         free_ vector（口,1, 月P) ;
         free_ vector (x, 1,甘P) ;
         return 0;
}

   The next demonstration program, xgauher, computes coe伍cients for Gauss-
Hermite quadrature by calling gauher. The test integral in this case is

                                    I
                                    J- 。。
                                        em   '
                                                 cosxdx=   /&_h/   4
                                                            Ch콰）旭r4: 加旭7카幻／i of Func力rOflS         63
         /s Driver for routine gauher 中/

     #include <stdio. h>
     甘include <math.h>
     *include "nr. h'1
     #include "nrutil. h1'

     #define NP 64
     甘define SQRTPI 1. 7724539

     float f山ic (float 工）
     {
               return cos (x) ;
     }

     mnt main(void)
     {
               mnt i, n;
               float check, x工1方工1 牛日；

           x=vector (11 NP) ;
           甘＝vector (1, 甘P) ;
           for     , ) {
                   (.
               printf ( "Enter N\n") ;
                if (ecanf ( "7.d", 幻l) == EOF) brea上;
               gai山Ler（工 , v,n) ;
               printf ( "Y.3s Y.los %148\n ', "#' ,"x (i) ", " 口(i) ")
                                                                       ;
               for (i=1; i<=n; i++) printf ( ' 工3d 工14. 8e
                                                                %14. 6e\n", i, x[i] ,v[ i] );
               for (check=0. O, i "1;i<=n;i++) check +=
                                                                町i] ;
               printf ( '\ nCheck value: %15.7e should
                                                                be: Y.1S.7e\n' , check,SQRTPI) ;
               /卞 deswnstrate the use of GAUHER
                                                        for an integral 中I
               for (xx=0. 0,i=1; i<=n;i+ +) 工工 += 町i] 中f山ic
                                                                   （玎1] ) ;
               prmntf ( '\ nlntegra]. frog gauher: %12. 6f\ n"
                                                                    ,xx) ;
               printf ( "Actual value:              %12. 6f\ n". SQRTPI*exp(- 0. 26) );
           }
          free_ vector (v, 1.NP) ;
          free_ vector (x, I 1iP) ;
          reti；
              口兀L0;
 }

   Program Igaujac exercises gaujac by computing the abscissas
                                                                   and weights for
an N-point Gauss- Jacobi quadrature. A convenient
                                                  test integral is


                                  r, V픈？小kz(1* :)/::2K（幻
so we set ( s = /3 = -1/ 2 in the program.
                                                (The integration reduces to Gauss
Chebyshev quadrature for this choice of parame
                                                 ters.) We choose k = 1/2, but you
can easily experiment with other values. A surprisingly
                                                        small value of N will calculate
the integral accurately.
/* Driver for routine gaujac 5/

linclude <stdio. h>
#include <math.h>
斗include "nr. h"
64        Numerical Recipes Example Book

#include "nrutil. h"

#define 甘P 64
#define PIBY2 1. 6707963

float func (float ak, float x)
{
       return 1. O/ sqrt (1. O戶ak本ak卓（1. 0＋工）/2. 0) ;
}

jot main(void)
{
       jot i, n;
       float ak,a1f=(- 0. 5) ,bet= (- 0.S) ,check日1check工1工X1 年工，巾日；

       x=vector (1,NP) ,
       v=vector (1,NP) ,
       如r ( ; ; ) {
           printf ( "Enter N\n") ;
           if (sc띠1f ( "hd" 小n) == EOF) break;
           gaujac (x, w,n, alf, bet) ;
           printf ( "/.35 %los %14s\n", "#", "x (i) " , 노(i) ") ;
           for (i= 1; i< 'n; i++) printf ( "%3d %14. 8e %14. 6e\n", j, x[ i] ,v[ i] );
            checkx=checkw=0 .0;
            for (i=1; i<=n; i++) {
                check工 += 工［1] ;
                checkw += v[ i] ;
            }
            printf ( "\ nCheck value: V.1& .7e should be: %16. 7e\n '",
                     checkx, n* (bet-alf) /(alf+ bet+2中n) );
            printf ( "\ nCheck value: Y.15.7e should be: %15. 7e\n" ,
                     checkw, exp(gammln( 1. 0+alf) +gasiuln(1. 0+bet) -
                     gammln(2. 0+alf+bet) )*pow (2.0,alf+bet+1.0) );
            /* demonstrate the use of GAUJAC for 띠l integral */
            ak=0. 5;
            如r (x工＝0. 0, i=1; i<=n; i++) 工工 += 町i] 巾func (ak，玎ii) ;
            printf ( "\ nlntegral from gaujac: Y.12.6f\ n' , xx) ;
            printf ( "Actual value:          h12. 6f\ n", 2. 0*ellf (PIBY2, ak) );
        )
        free_ vector (w. 1.NP) ;
        free_vector (x, 1,月P) ;
       return 0;
}

        Routine gaucof computes abscissas and weights given the coe佈cients in the re-
    currence relation for the corresponding orthogonal polynomials. We test it in xgaucof
    with Gauss-Hermite quadrature. The results should be the same as from xgauher.
    /* Driver for routine gaucof */

    *include <stdio . h>
    Ninclude "nr. h"
    #include "nrutil. h"

    #def ins NP 64
    *def ins SQRTPI 1. 7724539
                                                                 Ch카片er4: Integrat幻n 아Fun曲'ons   65
    jut main(void)
    {
         /* Test 日ith Gauss느Hermits 卓／
         mnt i, n;
         float 키nuO1 check, 卞a,中b, 李x 's日；

        a=vector (1,NP) ;
        b=vector (1, 且P) ;
        x=vector (1,NP) ;
        v=vector (i, NP) ;
        如r ( ; ; ) {
            printf ( "Enter N: \n") ;
            if (scanf ( " 工d", kn) == EOF) break;
            for (i '1;i<n; i++) {
                  町iJ =0. O;
                  b[ i+1]=it0. 6;
            }
           a[n] =O. O;
           ／卞 t江1] is arbitrary 如r call to tqli 中／
           amuO=SQRTPI;
           gaucof (n,a,b, a皿uO, x, w) ;
           printf ( 工3s 7.lOs 工14s\n' , "#", ''x (i) ", "w(i) ') ;
           for (i=1; i<=n; i++) print ( "V.3d '/.14. 6e V.14. 8e\n", i, x[i] ,w[i] );
           for (check=O. O, i=1; i<=n; i++) check += w[i] ;
           printf ( "\ nCheck value: %15. 7e 計ould be: V.16. 7e\n", check,SqRTPI) ;
        }
        free_ vs比吐 佃,1, 肝')
        free_ vector (x, 1,NP) ;
        frae_ vector (b,1,NP) ;
        free_ vector (a,1,NP) ;
        return 0;
}

    Routine orthog computes abscissas and weights for a nonclassical weight function.
We test it in xorthog with the weight function - log x, as described in Numerical
Recipes. The test integral here is


                                      J。
                                      /,I
                                             (1+
                                             (,
                                                   logx) 2
                                                      x)
                                                           :dx
                                                                   =   1og2
Once again a rather small value of N suffices for good accuracy.
/s Driver for routine orthog 巾/

#include <stdio.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

*def inc NP 64

float func (float x)
{
    ret山rn 1. 0/SQR(1.O+x) ;
}

jut iain (void)
66          Ni仰日切／尸e아殆s Examp旭 Book

{
        jIlt i, n;
        float amu0, check，工工，京a，比，卞工，卞므，卓카1u，中alpha, *beta;

        a=vector (1, 甘?);
        b=vector (1,NP) ;
        工＝vect乙r (1.NP) ·，
        v=vector (1,NP) ;
        카1u=vec如r (1.2*NP) ．·
        alpha=vector (1, 2*NP-1) ;
        beta=vector (1,2*NP-1) ;

        /s Test 日ith 町幻 = -l昭 工 SI
        for (; ;) {
            printf ( 'Enter N\n") ;
            if (scanf ( "%d", kn) == EOF) break;
            alpha口] =O. 5;
            beta [1] = 1. 0;
            for (i= 2; i<=2卞n- 1; i++) {
                 alpha[i] =0. 5;
                 beta[i] =1. 0/ (4.0S (4.0-1.0/ ( (i- 1) $(i- 1) )));
             }
                         ．
            a-flu口］=l . 0·
            a끄U［幻 = -0. 25;
            for (i= 2; i<=2sn-1; i++) anu[ j+1] = -a끄u[i] si* (i- 1) /(2. 0*(i+1)*(2*i- 1) );
            orthog(n,anu, alpha,beta,a,b) ;
            ainuo=l. 0;
            gaucof (n,a,b, a皿uo, x, v) ;
            printf ( "/.3s /.loa /.14s\n", " 井", "x (i) ", "v(i) ") ;
            for (i=1; i<=n; i++) printf ( "%3d Y.14. 6e %14. 6e\n", i, x (i] ,町i] );
            for (check=o. 0, i=1; i<=n;i++) check += vti] ;
                                                                                     ;
            printf ( "\ nCheck value: %15. 7a should be: %15. 7e\n", check,amuo)
            ／京 demonstrate the use of ORT取）G 如r 띠i integral 中／
            如r （工工＝0. 0,i=1; i ＜司i; i++) 工工 += 日［刃卞fundn幻 ) ;
            printf ( "\ nlntegra]. from orthog: /.12. 6f\ n", xx) ;
             printf ( "Actual value:              V.12.6f\ n", log(2.0));
        }
        fre하vec如r (beta,1.2方甘P- i) ;
        freeUvector (alpha, i, 25NP-i) ;
        free4vector (anu, 1, 2*NP) ;
        free_ vector (w, 1, 甘P) ;
        free_ vector (x, i, Np) ;
        free_ vector (b, 1,NP) ;
        free1vector (a, i, NP) ;
        return 0;
    }

         Chapter 4 of Numerical Recipes ends with a short discussion of multidimensional
    integration, exemplified by routine quad3d which does a 3-dimensional integration by
    repeated 1-dimensional integration. The C version of this algorithm is quite simple
    because recursion can be used. Sample program xquad3d applies the method to the
    integration of func = x2 + y2 + z2 over a spherical volume with a radius ima工 which
    is taken successively as 0.1, 0.2,. . . ,1.0. The integral is done in Cartesian rather than
    spherical coordinates, but the result is compared to that easily found in spherical
    coordinates, 4ir(乂max)5/5. Procedure func generates the function. Procedures yyl.
                                                              C力叩椰4: 加旭gra加／i of Funct幻ns   67
        and yy2 supply the two limlits of the y-integration for
                                                                 each value of x. Similarly zi
        and z2 give the limits of z-integration for given
                                                          x and !/.
        ／卓 Driver 如r routine quad3d 中／

        #include <stdio . h>
        甘include <math.h>
        #includ台 1뇨r.h"

        #def ins P1 3.1415927
        #define IVAL 10

        static float 工皿a工；

        float func (float x,f].oat y,float z)
        {
              return ！卞x+y卞y+z巾Z;
    }

    float zl (float x, float y)
    {
              return (float)   -sqrt (xma工中xmax-工卞工-y卞y) ;
    }

    float z2(float        x, float y)
    {
             return (float)    sqrt（工ma工京工flax七工* 工- y中y) ;
    }

    float yyl (float x)
    {
             return (float)    四qrt往ma工4imaX吐杜）;
    }

    float yy2(float x)
    {
        return (float) sqrt (x크a工ax쿄a工＝工ax) ;
}

mnt main(void)
{
            mnt i;
            float x皿in, 8;

             printf ( 'Integral of r2 over a spheric
                                                         al volume\n\n") ;
             printf ( "%13s %los %lls\n' , "radius ",
                                                      "QULD3D", "Actual") ;
             for (i=1;i. Z=NVAL; j++) {
                 x工a工＝0. 1卞1;
                 工ala = 1工ma工 ;
                 s=quad3d(func,工min,工nax) ;
                 printf ( "X12. 2f %12. 6f %11. 61\n",
                       工ma工 , 5.4.야町枉目日（工ma工 , 5.o) /S .o) ;
            }
            return 0;
}
Chapter 5: Ev졔ua如n 아 Functions

                                                                             imation and evaluation
         Chapter 5 of Numerical Recipes treats the approx
   of functio ns,   The   method    s, along     with   a  few   others,   are   applied in Chapter 6
                                                              l" functio  ns.    Polyno    mial or power
   to the calculation of a collection of "specia
                                        s  the   most    often    used   approx    imation    s and a few
   series expansions are perhap
                                                                        some    series.    In  the case of
   tips are given for accelerating the convergence of
                                                 rmation     is  popula   r,   and   is  implem   ented in
   alternating series, Euler's transfo
                                         l polyno     mials,   ddpo].y    demon     strates    the evalua-
   program eulsum. For genera
                                                                             a Ii就 of its coe丹icients.
   tion of both the p이ynom治I and 凡s der加atives 伽m
    The division of one polynomial           into   anothe    r, giving   a   quotient and remainder
                       done   by  poldiv      ,  while   the    evalua  tion    of a rational function
   polynomial, is
                                                               out   by  ratva     l. Ridders' method
   as the ratio of two polynomials is carried
                                        ives,    dfridr    , relies   on  polyno     mial extrapolation
   of finding numerical derivat
    techniq ues  from    Chapte   r  3.
                                                                                      mial series is pre-
         The approximation of functions by Chebyshev polyno
                                  arrivin   g   at  the  approx     imation     of  nearly    smallest de-
    sented as a method of
             from     the  true  functio    n   over   a  given    region     for  a specified order of
    viat ion
                                                                        mials are given by chebft
    approximation. The coefficients for such polyno
                                         s  are    subseq    uently    carried    out by chebev. To
    and function approximation
                                                                                 its   Chebyshev coe伍-
    generate the derivative or integral of a function from
                                                    tively.    To  conver    t  Chebys    hev coefficients
    cients, use chder or chint respec
                             a  polyno    mial    for  the   same    functio    n  (a   danger  ous proce-
    into coefficients of
                                                                                               and pcshft
     dure about which we offer due warning in the text) use chebpc
                                                                          use pccheb, the inverse of
     in succession. Finally, to economize power series,
     chebpc.
                                                                                                      imant
          The chapter concludes with a routine for finding the Padd approx
                                            pade,     and    a routine    ratlsq      for  finding  a ratio-
      from power series coefficients,
     hal  functio n  fit by  a least   squares     method     .
                                                                                                          s.
          Chapter 5 also treats several methods for which we supply no program
                                           s,  comple    x  arithm    etic  (see   Appen     dix  C), recur-
      These are continued fraction
                                                                                              ns.
      rence relations, and the solution of quadratic and cubic equatio



                                                          the summation of an alter-
     Procedure eulsum applies Euler's transformation to
                                                           be summed. Our sample
 nating series. It is called successively for each term to
 program xeu].sum evaluates the approximation


                     ln(l伺= z릉＋루무1···                                       尸 1 ＜二 :r << 1


  68
                                                     Ch叩for 5: Evaluat幻n 可戶mnci幻ns      69
    It asks how many terms mval are to be included in the approximation and then
    makes mval calls to euls끄n. Each time, index j increases and term takes the value
    (- 1)J 'x'/ j. Both this approximation and the function ln(1 + x) itself are evaluated
    across the region -1 to 1 for comparison. If mval is set less than 1 or more than 40,
    the program terminates.
 ／卞 Driver 如r routine eulsu皿 卓／

 #inc].ude <stdio .h>
 #include <math.h>
 #include "nr.h"
 #include "nrutil. h"

 #defiae NVAL 40

 mnt main(void)
 {
     jut i, j, mval;
     fl oat en皿，term. x, xpo甘er,卞wksp;

       日ksp= vector (1,NVAL) ;
       ／卞 evaluate mn(i奴）     ＝工吐n2/2+x3/ 3-x4/ 4 . . . for -1＜工＜1 卞／
       for (; ;) {
           printf ( "\ nRow many terms in polynomial?\n") ;
           printf ( "Enter n between 1 and 7.2d. (n=0 to end) ", NVAL) ;
           scanf ( "Y.d" 小nval) ;
           printf ( "\ n") ;
           if ( (mval <= 0) I I (mval > IVAL) ) break;
           printf ( "7.95 7.148 %14s\n" : "x" ,"actual" ,"poly如mia).") ;
           for (i = -8;i '(=8; j++) {
                工＝i/ 10. 0;
                sum=0 .0;
                工F)0口er = -1;
                for (j=1; j<=mval; j++) {
                     lF山口er 本＝ (-功 ;
                     term＝工F山口er/ j ;
                     eulsuni(&sum, term, j ,wksp) ;
                }
                printf ( "/.12. 6f Y.12. 6f 7.12.6f\ n", x,log(1.0+x) ,sum) ;
           }
      }
      free..vector (口ksp,1,NVAL) ;
      return 0;
}

    ddpoly evaluates a polynomial and its derivatives, given the coefficients of the
polynomial in the form of an input vector. Sample programn xddpoly illustrates this
for the polynomial:

                       (x 卞1)5 = -1+ 5x- 10x2+ 10x3--5上4+ x5

(This is a foolish example, of course. No one would knowingly evaluate
                                                                              (x 叫 i) 5 by
multiplying it out and evaluating terms individually - but it gives us a convenient
way to check the result!). Since this is a fifth order polynomial, we set NC, the
                                                                                   degree
of the polynomial, to 5, and initialize the array c of coefficients, with c [0] being the
constant coefficient and c[5] the highest-order coefficient. There are
                                                                          two ioops, one
70          Numerical Recipes Example Book

of which evaluates for x values from 0.0 to 2.0, and the other of which stores the value
of the function and NC-i derivatives. d[ j] Li] keeps the entire array of values for
printing. In the second part of the program, the polynomial evaluations are compared
with
                  /"'" "              , ,
                                                    n
                                                          n = 1,. .
                                         (
                                     =
                               (7)
                                                                     6_
                                                                0)
                                   5!
                                              -   (x
                                                       -   1.
                             =           (6
／巾 Driver 如r rout in日 ddpoly 卞／

#include <stdio . h>
*include "nr. h11
#include "nrutil. h"

#define NC 5
#define ND NC-i
#defina NP 20

m11t main(void)
{
        jut i, j, k;
        float x,p日r, *pd，卞牛d;
        static float c[NC+1]={-1.0,5.0.-10.0,10.0,-5.0,i. 0} ;
        static char *a[ND+iI= {"polynomial: ", "first deniy: "
            "second deriv: ", "third deriv: ", "fourth deniy: ") ;

        pd= vector (0,ND) ;
        d=matrix (0,ND,1, 甘P) ;
        for (i 'i; i<=NP; i++) {
             工＝0. 卄1;
             ddpoly (c, 丑C, x,pd,ND) ;
             for (j= 0; j<＝月D; j++) dCj]［幻＝pd［刃；
        }
        for (i= 0; i<=ND; i++) {
            printf ( "/.65 加 \n", " ", a[i] );
            printf ( "/.125 %17s %lss\n", "x ", "DDPOLY", "actual") ;
             for (j= i; j <=NP; j++) {
                 工＝0. 1卓3 ;
                 pvr=l. 0;
                 如r (k=1;k<＝표C-i; k++) pwr 字＝卜1. 0;
                 pnintf ( " 工15. 6f X i5. 6f 工15. 6f\ n", x,d[i] [j) ,
                       (factri （甘C) /f actri （甘C-i) ）卞p口r) ;
             }
             printf ( "press ENTER to continue. . .\n ") ;
             (void) getcharO;
        }
        free_rn毗;nix (d,이 吼h L 1P) ;
        free寸vector (pd,0, 표D) ;
        return 0;
    }

        poidiv divides polynomials. Given the coefficients of a numerator and denom-
    inator polynomial, poldiv returns the coefficients of a quotient and a remainder
    polynomial. Sample program xpoldiv takes
               Numerator = U = -1 + 5工 - 10尹 + 10工3_ 5工4 + 工5 = （工 - i) 5
              Denominator = v = 1 + 3丁 + 3r2 + x3 = (x + i) 3
                                                    Ch킥升er 5: Evaluat幻n of向nc加ns    71
    for which we expect

                              Quotient = q = 31 - 8x + x2
                             Remainder = r = -32 - 80x - 80x2

 The program compares these with the output of poldiv.
 ／中 Driver 如r routine poldiv 方／

 *include <stdio.h>
 *inc].ude 'nr.h"
 #include "nrutil. h"

 *define I 5
 社define IV 3

 jut main(void)
 {
     jut i;
     etatic float u[I+1)={-1.0, 5.0,-10. 0,10.0,-5.0,1.0} ;
     static float 吐月V+1卜｛1.0,3 .이3.0,1.0} ;
     float 中q1中r;

       q=vector (0,1) ;
      r=vector (0,I) ;
      poldiv（미 瓦v,IV,q.r) ;
      printf ( "\ n%105 %iOa %l0s Y,los %lOs /.l0s\n\n",
           "r0 '11 "rl " 1 "z2 " , "x3 " , "x4 ", "x '5") ;
      printf ( "quotient polynomial coefficients: \n") ;
       for (i=0; i<=6;i++) printf ( '%10. 2f ", q[i] );
      printf ( "\ nexpected quotient coefficients: \n") ;
      printf ( "%10. 2f %10. 2f %10. 2f %10. 2f %10. 2f %10. 2f\n\n",
           31.0 ,-8 .0,1. 0,0.0,0.0.0.0) ;
      printf ( "re工aind.r polynomial coafficients: \n") ;
      for (i=0;i<=3;i++) printf ( "%10. 2f ", r[ i] );
      printf ( "\ ne工p.ct. d remainder coefficients: \n") ;
      printf ( "%10. 2f %10. 2f %10. 2f %10. 2f\n", -32.0,-80.0,-80. 0,0.0) ;
      free_vector (r, 0,1);
      fr. e_vector(q,0,E;
      return 0;
}

    The next routine in Chapter 5, ratval, does not have its own demonstration
program. Instead, it is used in the demonstration programs for pade and ratlsq at
the end of this chapter.
      Ridders' method for numerical differentiation is carried out by routine dfridr.
In sample program xdfridr we test it on the simple function 1 (x) = tan x, for which
f ' (z) = sec2 x. You might try input values like x = 1.0, h = 0.1, to demonstrate that
h need not (and should not) be very small.

/* Driver for routine dfridr 5/

#include <stdjo.h>
#include <aath.h>
#includ. "nr.h"
*include "nrutil. h"
    72         Nun治nca／尸ecipes Exa／까)Ie Book


float func (float x)
{
         return ta끄（工）;
}

m11t main(void)
{
         float 치瓦d치 err;

         printf ( "input x, h\n" );
         日hule (scanf ( '' 工f 工f ' 1 ,k工,kh) != EOF)
         {
                d工二dfridr (func, 工 ,h,kerr) ;
                prmntf ( "clfridr=%12. 6f Y.12.6f Y.12.6f\ n", dx, l. O/SQR (cos(x) ),err) ;
         }
         return 0;
}

     The next seven programs all deal with Chebyshev polynomials. chebft evaluates
the coe佈cients for a Chebyshev polynomial approximation of a function on a spec-
ified interval and for a maximum degree N of polynomial. Demonstration program
xchebft uses the function func = x2(x2 小 2) sins on the interval (_ir/2, ir/2) with
the maximum degree of NVAL=40. Notice that chebft is called with this maximum
                                                                        Chebyshev
degree specified, even though subsequent evaluations may truncate the
series at much lower terms. After we choose the number mval of terms in the eva卜
uation, the Chebyshev polynomial is evaluated term by term, for x values between
 小O.8兀 and O.8兀 and the result f is compared to the actual function value.
／方 Driver 如r routine chebft 中／

#include <stdio. h>
#include <math.h>
#include "nr. h1'

#def ins NVAL 40
#define P102 1. 5707963

float func (float x)
{
             return 工方工＋（工中x- 2. O）布sin（工）;
 )

    jut main(void)
    {
             float a=(- P102) ,b=P102,dum, f;
             float to, tl, term, x,y, c[JVAL] ;
             jut i, j, mval;

          chebft (a,b, c,WVAL, func) ;
          ／中 test result; 卞／
          如r ( ; ·, ) {
              prmntf ( "\ nsow many terms in Chebyshev evaluation?\n") ;
              printf ( "Enter n between 6 띠1d %2d. (n=0 to end) .\n ", NVAL) ;
              scanf ( 'V.d", kmval) ;
              if ( (aval <= 0) I I (口v且]. > NVAL) ) brea노;
                                                     Ch짜）旭r 5: Eva加a加n 可F｛加Ct幻ns   73
          printf ( "\ n%9e %14s %16s\n ", "x", "actual", "cheby日hev fit ") ;
          for (i = -8; i< '8;i++) {
              x 'j$P工02/10.0;
              y=(x-O. 6* (b+a) )/(O. 5*(b-a) );
              /卞 Evaluate Chebyshev polynomial 口ithout C11EBEV */
              tO=i. O;
              tisy;
              f=c (1] Sti+c[OJ*O. 6;
              for (j= 2; j 'zmval; j++) {
                  du皿＝ti;
                  t1=2. O巾y卞ti-to;
                  t0=dum;
                  term=c[ j] *tl;
                  f += term;
              }
              printf ( "/.12.6f %12. 6f %12. 6f\ n", x, func (x) ,f) ;
          }
     }
     return 0;
}

    chebev is the Chebyshev polynomial evaluator and the next sample program
xchebev uses it for the same problem just discussed. In fact, the program is identical
except that it replaces the internal polynomial summation with chebev, which applies
Clenshaw 's recurrence to find the polynomial values.
／卞 Driver 如r routine ch口bev 巾／

卞include <stdio.h>
#incltide <math.h>
#include "nr. h"

#def in. IVAL 40
年4efine P102 1.6707963

float func (float x)
{
    return 工中x* (好工＝2. 0汁sin仕）;
}

mllt main(void)
{
     mllt i, mval;
     float a=(- P102) ,b=PI02,工, c[NVAL] ;

    chebft (히b 下 ,NVAL 小mc) ;
    /牛 Teat Chebyahev evaluation routine 中!
    如r (; ;) {
        printf ( "\ n且ow many terms in Chebyshev evaluation?\n") ;
        printf ( "Enter it between 6 and %2d. (n"O to end) .\n ", NVAL) ;
        scanf ( "%d" .&aval) ;
        if ( (aval <= 0) I I (mv.). > IVAL) ) break;
        printf ( "\ n%Os %14s %16a \n" , "x" ,"actua工", "chebyshev fit ") ;
        for Ci = -8; i<=8;i++) {
            工＝i巾P102/10.0;
            printf ( "%12. 6f %12. 6f %12. 6f\ n",
                  치 fu恥 仕) ,chebev(a,뇨 디mv.)., 幻 ) ;
74       Numeri口al Re肛1es Example Book

         }
     }
     retui그i 0;
}

    By the same token, the tests for chint and chder needn't be much different.
chint determines Chebyshev coefficients for the integral of the function, and chder
for the derivative of the function, given the Chebyshev coe佈cients for the function
itself (from chebft) and the interval (A, B) of evaluation. When applied to the
function above, the true integral is

                       f jut = 4工（尹 - 7) sin 工 m（工4- 14尹 + 28) cos 工

and the true derivative is

                           fder = 4工（尹 - l) sinx + 工2（尹 -2) cos 工

The code in sample programs xchint and xchder compares the true and Chebyshev-
derived integral and derivative values for a range of x in the interval of evaluation.
Since chint and chder return Chebyshev coefficients, and not the integral and deriva-
tive values themselves, calls to chebev are required for the comparison.
／中 Driver 如r routine chint 京／

#include <stdio . h>
*include <math.h>
#include "nr. h "

#define NVAL 40
#def ins P102 1.5707963

float func (float x)
{
     return 工京工方（工字工-2 . 아卞81fl(工）;
}
float fint (float x)
{
     return 4.0＋工*（工中卜7.아牛Bin仕卜（工巾工卞（工*工-14．아＋28．아*COB（幻；
}

tnt main(void)
{
    mnt i, mval;
    float a=(- P102) 1b=PI02, x;
    float c (IVAL] ,cint[ IVAL] ;

      chebft (a,b. c,NVLL,func) ;
      /t test integral 卞/
      如r (; ;) {
          printf ( "\ nHo甘 many terms in Chebyshev eva].uatiou?뇨l") ;
          printf ( "Enter n between 6 and %24. (n=0 to end) .\n ", IVAL) ;
             scanf ( "/.d" ,kmval) ;
             if ( (mval. <= 0) I I (mvai. > IVAL) ) brea上;
             chint (a,b, c,ci小 1三val加
             printf ( "\ n%9月 %14a %16s\n ", "x", "actua].", "Ch.by. integ. ") ;
                                                     Ch콰升er 5: EvalL石r幻n 아Func甘ons   75

           for (i = -8; i<=8; i++) {
               x=i* P102/10 .0;
               printf ( "%12. 6f %12. 6f /.12.6f\ n",
                    x, fint (x)-fint (- P102) ,chebev (a,b, cint, mval, x) );
          }
      }
      return 0;
:1.

/* Driver for routine chder */

*include <atdio.h>
#include <math.h>
#include "nr. h1'

#def ins 月VAL 40
#def4ne P102 1. 5707963

float func (float x)
{
      return 工卞工*（工中工느2. 0）卞ain(x) ;
}

float fder (float x)
{
      return 4. 0＋工*（工京工-1.0）京sin（工）＋工巾工＋（工字工＝2. 0）中cos（工）．·
}

mllt main(void)
{
      mnt i, mval;
      float a= (- P102) ,b=PI02, x;
      float c[NVAL] ,cder (IVAL] ;

      chebft (a,b, c,NVAL 小nc) ;
      ／卞 Test derivative 卞／
      for C; ;) {
          printf ( "\ n日ow many terms in Chebyshev evaluation?\n") ;
          printf ( "Enter n between 6 and %2d. (n=0 to end) .\n ", NVAL) ;
          scanf ( "%d" ,kmval) ;
          if ( (mval. <= 0) I I (mval > WVAL) ) break;
          chder (a,b, c, cder,mval) ;
          printf ( "\ nV.9a 工14a %16s\n", "x", 'actual", "Cheby. deniy. ") ;
          for Ci = -8; i<=8;i++) {
               工＝1卞P102/10. 0;
               printf ( "%12.6f %12. 6f /.12. 61\n' .
                    x ,fder (x) ,chebev(a.b, cder,mval, x) );
          ).
      }
      return 0;
}

   The next two programs of this chapter turn the coefficients of a Chebyshev ap.
proximation into those of a polynomial approximation in the variable
                                        V H卜 {(B + A)
                                          - '2 '(B- A)
    76       Nun旭nc可 尸ec徊es Exan刃le Book

(routine chebpc), or of a polynomial approximation in x itself (routine chebpc fol-
lowed by pcshft). These procedures are discouraged for reasons discussed in Nu-
merical Recipes, but should they serve some special purpose for you, we have at least
warned that you will be sacrificing accuracy, particularly for polynomials above or-
der 7 or 8. Sample program xchebpc calls chebft and chebpc to find polynomial
coefficients in y for a truncated series. For a set of x values between - 可 and ir it
calculates p and then the terms of the p-polynomial, which are summed in variable
poly. Finally, poly is compared to the true function value. (The function func is
the same used before.)
/中 Driver for routine chebpc */

#include <stdio .b>
#include <math.li>
#include "nr. h"

#define NVAL 40
#define P102 1. 5707963

fl oat func (float x)
{
         return x*x中（工巾x-2 . 0)*sin（工），·
}

mllt main(void)
{
         m11t i口, mval;
         float a= (- P102) ,b=P102,poly,x, y;
         float cENVAL] ,dCNVAL] ;

         chebft (a,b, c, 甘VAL, func) ;
         for (; ;) {
             printf ( "\ nHow many terms in Chebyshev evaluation'\ n ') ;
             printf ( 'Enter ii between 6 and %2d. (n=0 to end) .\n ", NVAL) ;
             scanf ( "V.d", knival) ;
             if ( (mval <= 0) I I (mval > NVAL) ) break;
             chebpc (c. d,mval) ;
             /s Test polynomial 京f
             printf ( "\ n%9s V.14s %14s\n", "x", "actual" , "polynomial") ;
             for (i = -8; i<=8; i++) {
                  x=i* P102/10. 0;
                  y=(x-0. bs (b+a) )/(0. 5*(b-a) );
                 polyrd［皿val小1] ;
                  for (J=mval-2; J>=0; j_ _) poly=poly*y+d[ j] ;
                  printf ( "Y.12. 6f Y.12. 6f 7.12. 6f\ n" , x,func (x) .poly) ;
             }
         }
         return 0;
}

     pcshft shifts the polynomial to be one in variable x. Sample program xpcshft
is like the previous program except that it follows the call to chebpc with a call to
pcshft.
                                                  C/i邵升or 5: EvalL石i幻n 可Func加ns     77

／衣 Driver 如r routine pcshft 卞／

*inc].ude <stdio . h>
#include <math.h>
#include "nr. h"

#define NVAL 40
#define P102 1. 5707963

fl oat f1끄玉c (float x)
{
    return x中x牛（x京工-2. 0）卞sin（工）;
}

mnt main(void)
{
    milt i, j, mval;
    fl oat a= (- P102) ,b=PI02,poly, x;
    fl oat c [IVAL] 1d [NVAL] ;

    chebft (a,b, c,NVAL, func) ;
    for (; ;) (
        printf ( "\ nHow many terms in Chebyshev evaluation'\ n") ;
        printf ( "Enter n between 6 and %2d. (n=0 to end) .\n ", NVAL) ;
        BC띠lf ( " Xd' 느&mval) ;
        if ( (mval <= 0) I I (mva]. > NVAL) ) break;
        chebpc(c, d,mva].);
        pcshft (a,b, d,mval) ;
         /* Test shifted polynomial */
         printf ( "\ n뷰9s %14s %14s\n", "x", "actual", "polynomial") ;
         如r (i = 尸8; i<=8;i++) {
             x=i* P102/10. 0;
             p01y=dEmva1-1] ;
             for (j 'mval-2; j>=0; j- -) po1y=p01y*x+d[ j] ;
             printf ( "%12. 6f %12. 6f X12. 6f\ n", x,func(x) ,poly) ;
         }
    I.
    retu工ii 0;
}

    Program xpccheb shows how to use pccheb to economize a power series. The
example chosen is the series on p. 294 of Numerical Methods That Work, by F.S.
Acton, namely that of cos iry on the interval F-i, ii. The coe佈cients of the series un
to y ' " are computea ano converted to Uflebysliev coetflcients. 'Ihese coefficients are
truncated after the term in y13, and the new power series coefficients are computed.
The answer is checked at selected points in the interval.
/* Driver for routine pccheb */

#include <stdio .h>
#include <math.h>
#include "nr. h"
#include "nrutil. h "

#define NCRECK 15
#define NFEW 13
    78       八加'7冶rica/ 尸ec徊es Example Book

#define 旨MA甘Y 17
#define NMAX 100
#define Fl 3. 14159265

jot main(void)
{
         mllt i, j;
         float a= (- PI) ,b=PI, fac,f, sum, su皿e,py,py2,斗c, *d,*e,*ee;

         c=vector (O,NMAX-1) ;
         d=vector (0,NMAX-1) ,
         e"vector (0,NMAX-1) ;
         ee=vector (0,NMAX-1) ;
         /* put power series of cos (PI巾y) into a 李／
         fac=l. 0;
         e[O] =ee[O] =O. 0;
         for (j= o; J<NMANY; j++) {
               j=j 立 3;     ／巾 tricky 日ay to perform j 工 4 牛／
              if (1. == 1 I I i == 3) e[ j] =0. 0;
              else if (i == 0) e[ j] =1.0/ fac;
             日ise 訌j] = 寸1. 0/ fac;
              fac *= (j+1) ;
              ee 口］=e［刃 ;
         }
         pcshft ( (- 2. 0-b-a) /(b- a) ,(2. 0-b-a) /(b- a) ,e,NMANY) ;
         ／半 i. e. , inverse of pcshft (a,b, . . . ) 日hich 口a do belo口 方／
         pccheb(e, c,NMANY) ;
         printf ( "Index, series, Chebyshev coefficients\ n") ;
         for (j= 0; j<NMANY; j+=2)
             printf ( "/.3d 工15. 6a7.15. 6e\n" , j, e[ j] ,c[ j] );
         chebpc (c, d, NFEW) ;
         pcshft (a,b,d,NFEW) ;
         printf ( "Index, new series, coefficient ratios\ n") ;
         for (j= 0; j<NFEW; j+=2) {
             printf ( "Y.3d '/.15. 6e '/.15. 6e\n",
                        j, d[ j] ,dEj] /(ee[ j] +1. oe-30) );
         }
         printf ( "         Point tested, function value, error power series, error Cheb. \n") ,
         for (i= O; i<=NCHECK; i++) {
             py=a+i* (b-a)! (float) NCHECK;
             py2=py*py;
             sum sume=0 .0;
             fac=l. 0;
             for (j= 0; j<NFEW; j+=2) {
                 so皿 += fac卞d[ j] ;
                 81싸1e += fac中ee [j] ;
                 fac *= py2;
             }
             f=cos (py) ;
             printf ( "check: %15. 6e %15. 6e 工15. 6e '/.15.6e\n", py,f, su皿e-f, sum-f) ;
         }
         free_ vector (ee,0,N甘AX-1) ;
         free_ vector (e,0,N卜1AX-1) ;
         free_ vector (d,0,NMAI-1) ;
         free_ vector (c, 0,NMAX-1) ;
         return 0;
}
                                                  Chac升8八；: Evalual幻n of Funct幻ns   79
    Test program xpade excercises pada by computing the Pade approximation to
ln(1 + x)/x. The Pad6 approximation is accurate for a much larger value of x than
the power series with the same number of terms fromn which it is derived. Note that
this test program and the one following both use ratval, so we do not
                                                                           supply a
separate sample program for it.
／中 Driver 如r routine pade 卞／

*include <stdjo . h>
寸inc:Lude <math. h>
*include "nr . h'1
*inciude "nrutil. h"

double fn(double x)
{
   ret1Urll (X
   return   Cx == 0. 0 ? 1.0 : log(1.0+x) /x) ;
}
#define NMAX 100

mnt main(void)
{
    mllt j, k,n;
    float resid;
    double b,d, fac,工1卞C,字cc;

     c=dvector (0,NMAX) ;
     cc=dvector (0 , NMAX) ;
     加r (; ;) {
         prmntf ( "Enter n for PADE routine: \n") ;
         if (sc카lf ( "%d", kn) == EOP) break;
         fac=l;
         for (j=1; j< '2*n+1; j++) {
             c[ j- 1] =fac/ ( (double) j) ;
             ccCj-1] =cEj-iJ ;
             fac = -fac;
         }
        pade(c,n,tresid) ;
        printf ( "Norm of residual vector= 工16. 8e\n", resid) ;
        printf ( "point, func. value, pade series, power oeries\n") ;
        for (3=1; j<=21; j++) {
            x=(j- 1)*0.2& ;
            for (b=o.0,k=2*n+1;k>=1;k_ _) {
                  b 中＝ X;
                  b Ir cc[k-1] ;
            }
            d=ratval (x,c,n,n) ;
            printf ( "/.16.8f /.16. 8f %16. 8f %16. 8f\n", x ,fn (x) ,d,b) ;
        }
    }
    free_dvector (cc,0,NMAX) ;
    free_dvector (c,0, 甘KAX) ;
    retw口10;



    Sample program xratlsq finds a rational approximation to the function tan니 x
80      Numerica／尸8아）es Examp旭 Book

by the lea就 squares method in ratlsq. You enter a desired interval and the orders
of the numerator and the denominator. The printed result shows the discrepancy
between the fit and the true function value.
／肛 Driver 如r routine ratlsq 本／

#include <stdio.h>
#include <math.h>
#include "ni .h"
*include "nrutil. h"

#define NMAX 100

double fn(double t)
{
     return atan(t) ;
}

jut main(void)
{
       jut j, kk,mm;
       double 키b1卞cof, d的, ee미fit, 工8;

       cof 'dvector (0,NMAX) ;
       如r ( ; ; ) {
            printf ( "enter 미b,min,kk\n") ;
            if (sc카lf ( "Y.lf %lf %d %d", ka,&b, &mm,&kk) ==EOF) break;
            ratlsq (fn, a,b,inm,kk, cof ,&dev) ;
             for (j "O; j<=mm+kk; j++) printf ( "cof (%3d)='/.27. 1&e\n", j, cof[ j] );
            printf ( "maximum absolute deviation= '/.12.6f\ n", dev) ;
            printf ( "     x         error           exact\n") ;
            printf ( "                                     \n") ;
            for (j=1; j<=50; j++) {
                xs'a+(b-a)*(j- 1. 0) /49. 0;
                fit "ratval (xs, cof,znm,kk) ;
                eee=fn仕引 ;
                printf ( "%lO. Sf %15. 7e '/.15. 7e\n", xs, fi七-eee, eee) ;
            }
       }
       free_dvector (cof, 0,NMAX) ;
       return 0;
 }
 Chapter 6: Special Functions

          This chapter on special functions provides illustrations of techniques de-
      veloped in Chapter .5. At the same time, it offers routines for calculating
     many of the functions that arise frequently in analytical work, but which
     are not so common as to be included, for example, as a single keystroke on
     your pocket calculator. In terms of demonstration programs, they represent
     a simple collection. The test routines are all virtually identical, making ref-
     erence to a single file of function values called fncval . dat which is listed in
     the Appendix at the end of this chapter. In this file are accurate values for
     the individual functions for a variety of values for each argument. We have
     缸med to "毗ress月 the routines a bit by throwing i끄 some e玭rerne va加es for
     the arguments.
         Many of the function values came from Abramowitz and Stegun 's Hand-
     知ok of)／毗万em口tic口iF뇨nct加n요 品me others, 加wever, came 介om our library
    of dusty vo加mes 介om j犯針 ma就ers. There is an implic凡 danger 血 a cornpar-
    ison test like this - namely, that our source has used the same algorithms
    as ours to construct the tables. In that case, we test only our mutual corn-
    pet ence at computing, not the correctness of the result. Nevertheless, there
    is some assurance in knowing that the values we calculate are the ones that
    have been used and scrutinized for many years. Moreover, the expressions
    for the functions themselves can be worked out in certain special or limiting
    cases without computer aid, and in these instances the results have proven
    correct.



With few exceptions, the routines that follow work in this fashion:
 1. Open file fncval.dat.
 2. Find the appropriate data table according to its title.
 3. Read the argument list for each table entry and pass it to the routine to be tested.
 4. Print the arguments along with the expected and actual results.
    For the routines in this list, therefore, we forego any further comment, but
                                                                                 simply
identify them by the special function that they evaluate. The exceptions are the test
program for the utility procedure beachb and the test of the hypergeometric function
routine hypgao.
Natural logarithm of the gamma function for positive arguments:




                                                                                    Ri
    82        Nun冶rica/ 尸e아旭s Examp旭 Book

／牛 Driver 如r rout in日 ga工1mln +/

#include <stdio .h>
#include <stcilib . h>
#include <string.b>
#inc].ude <math.h>
#include "nr. h"
#include 1'nrutil. h"

#define MAXSTR 80

ml1t main(void)
{
         char txt [MAXSTR:l,
         jut i, nval;
         fl oat actual, calc, x;
         FILE *fp;

         if ( (fp = 如pen( "fncva]..dat", "r ") ) == NULL)
             nrerror ( "Data file fncval.dat not found\n") ;
         fgets (txt. MAXSTR, fp) ;
         while (strnclnp(txt, "Gan a Function", 14) ) {
             fgets(txt, MA工STR, fp) ;
             if (feof (fp) ) nrerror ( "Data not fou끄d in fncval.dat\n") ;
         }
         fsca끄i(fP, " 工a 工＋5 " ,&nval) ;
         printf ( "\ n'/,s\n" , txt) ;
         printf ( "Y.los 7,21w Y.21s\n", "x", "actua1", "ga   ln (工) ") ;
         for (i "i; i<=nval;i++) {
             fsc키lf (fp, "%f %f ", &x,&actual) ;
             if （工 > 0. 0) {
                  ca1c=(x<1.0 ? ga皿m].n(x+1.0)-log(x) : ganln (工) );
                  printf ( "7.12. 2f %20. 6f %20.6f\ n", 工,
                      log(actual) , caic) ;
             }
         }
         fclose(fp) ,
         return 0;
}

Factorial function N!:
/* Driver for routine factrl          中/

#include <stdio . h>
#include <stdlib. h>
#include <string.h>
#include <math.h>
#include "nr.h"
#include "nrutil. h"

#def joe MAXSTR 80

mnt inain(void)
{
         char t工t［甘A工STR] ;
         float actual;
                                                          Ch可까er 6: 斗：e口洌Func加ns   83
        jut i, n,nval;
        FILE *fp;

         if( (fp = fopen( "fncval. dat ", "r ") ) == N兀L)
            xxerror ( "Data tile tncval.dat not found\n") ;
        tgets (txt ,NAXSTR, fp) ;
        while (strucap(txt, "N-factorial ", ll) ) {
            fgets (txt, MAXSTK, fp) ;
            if (feof (tp) ) nrerror ( "Data not found in tncval.dat\n") ;
        }
        fscanf (fp, "%d %ae " 小lval) ;
        printf ( '\ n%e\n", txt) ;
        printf ("%6s Y.18s Y.20s \n ' ,'n " ,'actual " ,'factrl (n) ") ;
        for (i=1; i<=nva1; j++) {
            fecanf (fp, "%d %f ' ,kn,&actual) ;
            if (actual < 1.oelo)
                 printf ( "%6d t20.Ot t20.of\ n", n,actual,tactrl (n) );
            dlee
                printf ( '%6d %20e %20e \n ' 1n,actua].,factrl (n));
        }
        fclose(fp) ;
        return 0;
}

Binomial coe伍cients:

／卞 Driver 如r routine bico 衣／

#include <etdio.h>
#include <stdlib. h>
#include <string.h>
#include "nr. h"     -
#include "nrutil. h"

#define M工STR 80

jut main(void)
{
    char txt [MAISTR] ;
    jut i, k1n1nval;
    float binco;
    FILE *fp;

    if ( (fp = fop.n( "fncvaLdat", "r ") ) == NULL)
        nrerror ( "Data file fncval.dat not 如und\n") ,
    fgets (txt, XAXSTR, fp) ;
    while (strnc皿p(txt, "Binomjal Coeffjcients", 21) ) {
        fgets (txt ,片AXSTR, fp) ;
        if (feof (fp) ) nrerror ( "Data not found in fncval.dat\u'1) ;
    }
    fscanf (fp, ' 工d %*a ' 小lval) ;
    printf ( '\ n加\n" , txt) ;
    printf ( "%6e Y.6s t12s %12s \n" , 'n " , 'k" ,"actual" ,"bico佃小)") ,
    for (i= 1; i<=nva1;i+ +) {
        tscant (fp, "%d V.4 戈t ", kn,*k. kbinco) ;
        printf ( " 工6d ted %12. Of %12. of \n". n,k, binco,bico(n,k) );
    }
 84          N｛月"9欣：a사？9帥）es Examp旭 Book

        fclose(fp) ;
        return 0;
}

Natural logarithm of N!:
／卞 Driver 如r routine factin 京／/

#include <stdio.h>
#include <stdlib .h>
#include <string.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

#define MAXSTR 80

mnt mamn(void)
{
        char txt[ MAXSTR] ;
        mnt i, n1nval;
        float val;
        FILE *fp;

        if ( (fp = fopen( "fncval. dat " , "'r ') ) == NULL)
            nrerror ( "Data file tncval. dat not found\n') ;
        fgets (txt, MAXSTR, fp) ;
        while (strncmp (txt, ''N-factorial " ,ii) ) {
              tgets (txt, MAXSTR, fp) ;
              if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
        }
        fscanf (fp, ' 力；d }；卓5,,，立nval) ;
        prmntf ( "\ nlog of n..factorial\ n ') ;
        printf ( "\ nY.6s 工198 Y.21s\n"' , 'n" , "actual", "fa亡tln(n) ") ;
        for (i=1; i<=nval; i++) {
            fscanf (fp, "%d %f ", &n, &val) ;
            printf ( "%6d V.20. 7f %20. 7f\ n ', n,log(val) ,factln (n) );
         }
         fclose(fp) ;
         return 0;
 }

    Beta function:
    /* Driver for routine beta */

    #include <stdio . h>
    #include <stdlib. h>
    #include <string. h)
    #include "nr. h"
    #include "nrutil. h"

    *define MAXSTR 80

    mllt main(void)
    {
         char t工t江MAXST瓦1 ;
         mllt i, nval;
                                                                Ch콰가er 6: 印ecial Funet幻ns   85

             float val,口, z;
         FILE *fp;

          if  ( (fp = fopen( "fncval. dat ", "r ") ) == NW工）
               nrerror ( "Data file fncval.dat not found\n") ;
          fgeta (txt, MAXSTR, fp) ;
          while (strncmp(tzt, "Beta Function", 13) ) {
               fgeta(txt. MAXSTR, fp) ;
               if (feof (fp) ) nrerror ( "Data not found in fncval.cLat\n") ;
          }
          fecanf (fp, "%d %*s", knval) ;
         printf ("\ n加＼n" 1t工t) ;
         printf ( "/.Ss /.68 V.16e /.20e\n' ,"w ' ,"z " ,"actual" ,"beta(미z) ") ;
         for (i=1; i<=nva1; i++) {
               fsc카lf (fp, "%f %f %f ", kw,kz,&val) ;
               printf ( "Y.6. 2f Y.6.2f %18. 6e V.18. 6e\n", w,z, val,beta(日, z) );
         }
         fclose(fp) ;
         rett口江i 0;
    }


    Incomplete gamma function P (a, x):

    /* Driver for routine ga皿mp a!

    #include <stdio.h>
    *include <etdlib. h>
    #include <etring·h>
    #include 'nr. h"
    #include 'nrutil. h"

    #define MAXSTR 80          .

    mnt main(void)
    {
        cha工 t工t［甘A工STR] ;
        mllt i, nval;
        float a,val, x;
        FILE *fp;

        if  ( (fp = fopen( "fncval.dat ", "r ") ) == NULL)
             nrerror ( "Data file fncva]..dat not found\n ") ;
         fgets(txt, MAXSTR, fp) ;
         while (strncmp(txt, "Incomplete Ga皿皿a Function' ,25) ) {
             fgete (txt, MAXSTh, fp) ;
             if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n ') ;
         }
        fsca끄f (fp, "%d X*s", &nval) ;
        prmntf ( "\ nY.s\n" ,txt) ;
        printf ( "%4a %lls Y.14s %14a \n", "a", "x", "actual",
                                                               "gammp(a,x) ") ;
        for (i=1;i<=nval; i++) {
             如口anf (fp, "/.f /.f %f ", *a,tx, kval) ;
            printf ( "Y.6.2f Y.12.6f %12.6f 'f.12.6f \n", a,x,val, gaxunp
                                                                          (a,x) );
        }
        fclose(fp) ;
        return 0;
}
    86        Numerica／尸ec徊es Examp旭 Book

Incomplete gamma function Q(a, x) = 1 - P (a, x):
／卞 Driver for routine ga丑mq 卞／

*includa <stdio.h>
#inc].ude <stdlib .h>
#include <string. h>
#include 'nr. h"
#include "nrutil. h'1

#define MAXSTR 80

mnt main(void)
{
         char txt[ MAXSTR] ;
         mnt i, nval;
         float a, val, x;
         FILE *fp;

         if ( (fp = fopen( "fncval. dat ", "r ") ) == NULL)
             nrerror ( 'Data file fncval.dat not 如und\n") ;
         fgets (txt ,MAXSTR, fp) ;
         while (strncmp(txt, 'Incomplete Gamma Function", 25) ) {
              fgets (txt ,MAXSTR, fp) ;
             if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
         }
         fscanf (fp, "Y.d V.*s" , knval) ;
         printt ( "\ nY.s\n' ,txt) ;
         printf ( "%4s Y.lls Y.14s %14s \n' , "a", "x' , "actual", "ga口mq(a,x) ') ;
         for (i '1; i<=nval; i++) {
             fscanf (fp, "%f %f %f ', ka,*x1kval) ;
             printf ( "Y.6. 2f Y.12. 6f %12. 6f %12. 6f\ n". a,x, (l. O-val) ,gammq(a. x) );
         }
         fclose(fp) ;
         return 0;
}

Incomplete gamma function P(a, x) evaluated from series representation:
/卓 Driver for routine gser 卞/

#include <stdio . h>
#include <stdlib. h>
#include <string.h>
#include 1뇨工 . h'1
#include "nrutil. h'1

#define MAXSTR 80

mnt main(void)
{
         char t工t江MAX STR] ;
         mnt i, nval;
         float a,gamser, gln, val, x;
         FILE *fp;

         if   ( (fp = 如pen( "fncval. dat ', "r ") ) == NULL)
               nrerror ( "Data file fncval.dat not fou끄d\n") ;
                                                      （功邵丑& 6: 印ecial Funct幻ns   87

      fgets (txt, MAXSTR, fp) ;
     日hile (strncmp(txt, " Incomplete Ga工ma Function ' 125) ) {
          fgets (txt, MAXSTR. fp) ;
          if (feof (fp) ) nrerror ( 'Data not found in fncval.dat\n') ;
      )
      fscanf (fp, "V.d %*s", &nval) ;
     printf ( "\ n%a\n' .txt) ;
     printf ( '%4s %ils %14s 工148 V.128 V.8s\n". "a", "x ".
          "actual". "gser (a,x) ' , 'gan皿ln(a) ". "gln') ;
     for (i "1;i<=nval; i++) {
          fscanf (fp. '%f /.f %f '. ka.kx,&val) ;
          g88r (kgaJnser.a, x,&gln) ;
          printf ( "V.6.2t V.12.6f 工12.6f %12.6f 工12.6f V.12.6f\ n",
               a, x,val,ga皿ser,gammln(a) ,g].n) ;
     }
     fclo8e(fp) ;
     return 0;
}

Incomplete gamma function Q(a, x) evaluated by continued fraction representation:
/卞 Driver for routine gcf 卞!

#include <stdio.h>
#include <8tdlib . h>
#include <string.h>
#include 11nr. h"
#include nnrutil. h11

#define MAISTIt 80

mllt main(void)
{
     仁har t工t［甘且工STR] ;
     mllt i, nval;
     float 미val. x,ga月mcf,g끄1;
     FILE sip;

    if   ( (fp = fopen( "fncva]..dat ", "r ") ) == NULL)
           nrerror( "Data file fncval.dat not found\n") ;
     fgets (txt. MAXSTR. fp) ;
    口hule 佃trnc叩作工t. "Incomplete Ga皿ma Function" .25) ) {
           fgete (txt, MAXSTR, fp) ;
          if (feof (fp) ) nrerror ( 'Data not found in fncval.dat\n') ;
     )
     fsca끄f (fp. "Y.d 肛s '. knval) ;
    printf ( "\ n%s\n ' .txt) ;
    printf ( '%45 V.118 %14s V.138 %13s %8s\n". "a '. 'x ' .
          'actual". 'gcf (a.x) ". 'gammln(a) ". 'gln") ;
    for (i=1; i<=nva1; i++) {
          fscaiii(fp. "V.f V.f %f ', &a.&工,kval) ;
          if (x >= (a+1.0) ) {
               gcf (*g的1皿cf ,a，工 ,kgln) ;
               printf ( " 兄6. 2f%13.6f%13. 6f%13.6f%12. 6f%13. 6f\n' .
                    a.x. (1.0-val) ,gaa工cf, ga皿1in(a) ,gln) ;
          }
    }
     88        八IL月Tie月ca샤？ec徊es Exam이e Book

          fclose(fp) ;
          ret皿rn 0;
}

Error function:

/* Driver for routine erff 卞/

*include <stdio . h>
*include <8tdlib.h>
#include <string. h>
#include "nr.h"
*ialclude "nrutil , h'1

#define MAXSTR 80

ml1t main(void)
'C
          eke工 t工t [MAXSTR] ．·
          mnt i, nval;
          float val, x;
          FILE *fp;

          if ( (fp = fopen( "fncval.dat ", "r ") ) == NULL)
              nrerror ( "Data file fncval. dat not found\n") ;
          fgets(txt, I4AXSTR, fp) ;
          while (strncmp(txt. 'Error Function", 14) ) 'C
               fgets (txt , MAXSTR , fp) ;
               if (feof (fp) ) nrerror ("Data not found in fncval. dat\n") ;
          }
          fscanf (fp, "%d %*s", tnva] );
          printf ( "\ n加＼n" ,t工tm
          printf ( "%4s %12s %12s\n", "x", "actual", "erf (x) ") ;
          for (i=1; i< 'nval; i++) 'C
              fsc띠f (fp, "%f %f ", kx,&val) ;
              printf ( "%6. 2f '/.12.7f '/.12.lf\ n", x, val, erff (工) );
          }
          tclose(fp) ;
          retux끄 0;
     }

     Complementary error function:
     /* Driver for routine erffc */

     #include <stdio .h>
     #include <stdlib . h>
     #include <string. h>
     #include "nr.h"
     #include "nrutil. h"

     #define XAXSTR 80

     mllt main(void)
     'C
          cha工 t工t［甘AXSTR] ;
          mnt i, nval;
          float 치val;
                                                                 Ch햐升er 6: Special Funct幻ns   89

        FILE *fp;

        if ( (fp = fopen( ''fncval. dat ', "r ") ) == NULL)
            nrerror ( "Data file fncval.dat not found\n") ;
        fgets(txt, MAXSTR, fp) ;
        日hule 佃trnc叩(t心, 'Error Function", 14) ) {
            fgets (txt, MAXSTR. fp) ;
            if (feof (fp) ) nrerror ( 'Data not found in fncval.dat\n") ;
        }
         fscanf (fp, “工d 肛可', knval) ;
        printf ( "\ ncomplementa.ry error function\n") ;
        printf ( '%5s %12s %13s\n" ,"x '", "actual ", '''erfc (x) '") ;
         for (i= 1; i<=nval; i++) {
             fscanf (fp. "%f %f ' , kx,kval) ;
             val=l. 0-va].;
             printf ( '%6. 2f X12. 7f Y.12. 7f\ n' . x, val, erffc (x) );
        )
        fcloee(fp) ;
        return 0;
}

Complementary error function from a Chebyshev fit to a guessed functional form:
/* Driver for routine erfcc */

作include <stdio.h>
#include <atdlib. h>
#include <string.h>
#include '1nr.h"
#include 'nruti] ..h"

#define 甘I工STR 80

mnt main(void)
{
    char txt[ MAXSTtt) ;
    mnt i, nval;
    float x, val;
    FILE *fp;

    if  ( (fp = 如pen( 'fncval. dat ', "r ") ) == NULL)
         nrerror ( "Data file fncval.dat not found\n'') ;
    fgets(t工t，甘且XSTR, fp) ;
    日hi]
       .. 佃trncm可t工t, "Error Function", 14) ) {
          fgete(txt ,MAXSTR, fp) ;
         if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
    }
    fscanf (fp, "工dY.巾8 " ，七｝val) ;
    printf ( "\ ncomplementary error function\n") ;
    printf ( "Z5a 7.128 %13a\n' , ''x ", "actual", 'erfcc (x) ") ;
    for (i=1; i<=nva1; i++) {
         fscanf (fp, "%f 7.f " ,&x,kval) ;
         va].=1. 0-va].;
         printf ( '%6. 2f %12. 7f %12. lf\ n '. x, va]..erfcc (x) );
    }
    fclose(fp) ;
    retuj그l 0;
 90          Numerical Recipes Example Book

}

Exponential integral E, (x) :

／中 Driver 如r routine a工pint 4 /

#inc].ude <stdio. h>
#include <stdlib . h>
#include <string. h>
#include "nr. h'1
#include 11nrutil. h"

#define MAISTR 80

mllt main(void)
{
     cia工 t工t [MAXSTR] ;
     mnt i, nval,n;
     float val, x;
        FILE *fp;

        if ( (fp = 如pen( "fncval. dat ", "r ") ) == lULL)
                                                             ") ;
            nrerror ( "Data file fncval. dat not found\n
        fgets(txt, MAXSTR, fp) ;
                                                       En ', 23) ) {
        while (strncmp (txt, 'Exponential Integral
             fgets (txt ,MAXSTR , fp) ;
                                                        in fncva]..dat\ n") ;
             if (feof (fp) ) nrerror ( "Data not found
        }
        fscanf (fp, "%d %*s ' ,tnya1) ;
        printf ( "\ n%s\n" , txt) ;
                                                      'actual" , 'expint (n, x) ") ;
        printf ( "%4s 工7s %15s Y.21月 \n", "n ' ,'x ",
        for (i=1; i<=nval; i++) {
            fscanf (fp, "%d Y.f V.f ', kn,&x,kval) ;
                                                         x,val, expint (n, x) );
            printf ( 'V.4d %8. 2f 工18. 6e %18. 6e\n", n,
        }
        fclo日e(fp) ;
        return 0;
    }

    Exponential integral Ei(x) :
    /s Driver for routine ei */

    #include <stdio. h>
    #include <stdlib. h>
    #include <string.h>
    甘include 'nr. h'1
    #include 1'nriitil. h"

    #define MAXSTR 80

    jot main(void)
    {
        char t工t [MA工STE] ;
        jOt i 1nval;
        float val 1x;
             FILE *fp;
                                                            Ch카가er 6: Special／七nc加ns   91
            if ( (fp = fopen( "fncval.dat ", "r ") ) == NULL)
                nrerror ( "Data file fncval 4at not found\n") ;
            fgets (txt, MAXSTR, fp) ;
            while (etrncmp(tzt, "Exponential Integral Ei", 23) ) {
                fgets (txt, 甘AXSTE, fp) ;
                if (feofCfp) ) nrerror ( "Data not found in fncval.dat\n") ,
            }
         fscaxtf (fp, "%d %*s", &nval) ;
         priutf ( "\ n%s\n", txt) ;
         printf ( "%Ss Y.12s %lia \n", "x", "actual", "ei(x) ") ;
         for (i "i; i<=nval; i++) {
             fscanf (fp, "%f %f ", kx,kval) ;
             printf ( "%6. 2f %12. 6f %12.6f\n", x,val,ei(x) );
         }
         fclose(fp) ;
         rett口＝n 0;
    }

Incomplete Beta function:
/* Driver for routine betai 中1

#iuclude <stdio.h>
#include <stdlib.h>
#include <etring.h>
#include "nr.h"
#iuclude "nrutil. h"

斗define 出江STR 80

jut main(void)
{
        char I；工t［片AXSTRJ ;
        jut i 1nval;
        float a,b,x,val;
        FILE *fp;

        if ( (fp = fopen( "fucvaLdat ", "r ") ) == NULL)
            nrerror ( "Data file fucval.dat not found\n") ;
        fgets (txt, MAXSTR, fp) ;
        while (strncmp (txt, "Iucomplete Beta Function", 24) ) {
            fgeta (t；工t 1甘A工STR, fp) ;
            if Cf eof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
        }
         fscantCfp, "%d %*s", knval) ;
        printf ("\ n加＼u' ,t工t) ;
        printf ( "%Ss %loa %12e Y.14s %13s \n",
             "a", "b' , "x", "actual", "betaiCx) ") ;
        如r (i=1; i<"uval;i++) {
             fec띠if (fp, "%f 戈f 加 %f " ,&a,*b,k工,kval) ;
             priatfC"%6.2f %12. 6f %12. 6f %12. 6f 兀12. 6f\n",
                  a,b,x,val,betai(a,b, x) );
        }
        fcloee(fp) ;
        return 0;
}
    92         Nurnerica/ 尸ec徊es Examp旭 Book

Bessel function J0:

/卓 Driver for routine besejO */


#includ日 (stdio. h>
#include <stdlib. h>
#include <string. h>
*inclucie '1nr.h"
#includa 'nr比il. h1'

#define MAXSTR 80


mnt main(void)
{
         char txt[ MAXSTR] ;
         mnt i, nval;
         float val, x;
         FILE *fp;


         it ( (fp = fopen( 'fncval. dat ", 'r ") ) 二＝ NULL)
             nrerror ( "Data file fncval. dat not 如imd\n") ;
         tgets (txt, MAXSTR, fp) ;
         日hile (8trncmp(txt, "Bessel Function JO" ,18) ) {
              fgets (txt ,$AXSTR, tp) ;
              if (feof (fp) ) nrerror ( "Data not found in fncval. dat\n ') ;
         }
         fscanf (fp, "%d 肛s ", &nval) ;
         printf ( "\ n%s\n" ,txt) ;
         printf ( "%5s Y.12s Y.13s \n", "x ", 'actual '", ''bessjo (x) ") ;
         for (i '1; i<=nval; i++) {
              fscanf (fp, "%f %f ' , kx,kval) ;
             printf ( "%6. 2f %12. 7f %12. 7f \n", x, val, bessjo (x) );
         }
         fclose (fp) ;
         return 0;
}

Bessel function Y0:

/* Driver for routine bessyo 中1


#include <stdio. h)
#include <stdlib. h)
    #include <string. h>
    #include 'nr. h1'
    #include "nrutil. h"

    #dafine MAXSTR 80


    mnt inain(void)
    {
          char t工t[MAXSTR] ;
          m11t i, nval;
          float val, x;
          FILE *fp;

          if    ( (fp = 如pen( "fncval. dat ", 'r ") ) == NULL)
                 nrerror ( 'Data file fncval. dat not found\n") ;
                                                          Gb카）相r6: 印ecial Functions   93

    fgets(txt ,MAXSTR. fp) ;
    日hule 佃trnc叩作工t, " 加esel Function YO", 18) ) {
        fgeta (txt, MAXSTR, fp) ;
        if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n') ;
     }
    fsca끄f (fp, 'Y.d Y.*s ' ,&nval) ;
    printf ( "\ n%s\n' .txt) ;
    printf ( '%5s Y.12s X13s \n", "x' , "actual", 'bessyo(x) ") ;
    for (i=1; i<=nval;i++) {
        fscanf (fp, "%f %f ", kx,kval) ;
        printf ( "Y.6.2f 7.12.7f /.12. 7f\ n ', x,val, bessyo(x) );
    }
    fclose(fp) ;
    return 0;
}

Bessel function J1:

/卞 Driver for routine beseji */

#include <stdio .h>
*inc].ude <stdlib. Ii>
#include <string. h>
#include 11nr. h"
*jnclude "nrutil. h"

#def ins 片A工STR 80

jut main(void)
{
    char t工t [HAXSTR] ;
    mllt i1nval;
    float val, x;
    FILE *fp;

    if ( (fp = fopen( "fncval.dat", "r ") ) == NULL)
        nrerror ( 'Data file fncval.dat not found\n1') ;
    fgete (txt, MAXSTR, fp) ;
    while (strnciep(txt, "Bessel Function 31 ', 18) ) {
        fgets (txt ,XAXSTR , fp) ;
        if Cf eof (fp) ) nrerror ( "Data not found in fncval.dat\n ") ;
    }
    fscanf (fp. "%d %ss", knval) ;
    printf ( "\ n%s\n" ,txt) ;
    printf ( "Y.Se 7.12a %13a \n", 'x ", "actual". "bessjl (工) ") ;
    for (i=1; i<=uval; i++) {
        fscanf (fp, "%f 工f " ,k工小val) ;
        printf ( "%6.2f %12. 7f %12. 7f\ n ', x,val,besajl(x) );
    }
    fclose(fp) ;
    return 0;
}

Bessel function Yj:

／中 Driver 如r routine bessyl 巾／

tinclude <stdio . h>
    94         Numerica/ 尸ecj戶es Examp旭 Book

#include <stdlib. h>
#include <string.h>
#include "nr. h1'
#include "nruti] ..h1'

#define MAXSTR 80

mllt main(void)
{
         char t工t EMA工STR] ·，
         mllt i 1nval;
         fl oat val, x;
         FILE *fp;

         if ( (fp = fopen( "fncval. dat ", "r ") ) == WULL)
             nrerror ( 'Data file fncval.dat not found\u ') ;
         fgets (txt ,MAXSTE ,fp) ;
         while (strncwp(txt, 'Bessel Function Y1". 18) ) {
                fgets (txt, MAXSTR, fp) ;
                if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
         }
         fsc띠lf (fp, 'Y.d 工*s", &nval) ;
         printf ( "\ n加＼O", t工t) ;
         printf ( " 工ss %12s Y.13s \n", "x " , "actual" , ''bes8yl (x) ") ;
         for (i=1; i<rnval; i++) {
             fscanf (fp, "%f '/.f '' , kx,kval) ;
             printf ( "/.6. 2f %I2. 7f '/.12. 7f\ n", x, val, beesyl(x) );
         }
         fclose(fp) ;
         return 0;
    }

    Bessel function Y1 for n > 1:

／中 Driver 如r routine bessy 卞／

    #include <stdio.h>
    #include <stdlib. h>
    #include <string.h>
    #include "nr. h"
    #include "nrutil. h"

    #define MAXSTR 80

    mllt main(void)
    {
         cha工 t工t [MAXSm] ;
         mnt i, nval,n;
         float val, x;
          FILE Cf p;

          if ( (fp = fopen( "fncva工dat ", 'r ") ) == ULL)
              nrerror ( "Data file fncval .dat not found\n") ;
          fgets (t工t, MAXSTR, fp) ;
          日hule 佃trnc叩(t心，" Bea日a]. Function Yn", 18) ) {
                 fgeta (t工t，겨［A工STh. fp) ;
                 if (faof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
                                                               Ch司가er 6: 印ec洌Func切ns   95

          }
          fscanf (fp, "%d %*s" 小lval) ;
         printf ( "\ n加\n", txt) ;
         printf ( "%4s Xis %lss 工20s \n", 'n". 'x ", 'actual ', "bessy(n, x) ")
                                                                                ;
         for (i=1; i<=nval; i++) {
              fsc띠lf (fp, 'Xd /.f Xf ", kn,&x,kval) ;
              printf ( "X4d X8. 2f %18. 6e X18. 8e\n",n.x, val,beesy(n,x) );
         )
         fclose(fp) ;
         return 0;
    }

    Bessel function J1 for n > 1:

    ／卞 Driver 如r routine bessj 衣／

    #include <stdio . h>
    *include <stdlib.h>
    #include <string.h>
    #include 1뇨r.h"
    #include "nrutil. h"

    #define MAXSTR 80

    mllt uiain(void)
    {
         char txt[ NAXSTR] ;
         mnt i, nval,n;
         float val, x;
         FILE *fp;

        if  ( (fp = fopen( "fncval.dat ' , "r ") ) == NULL)
             nrerror ( "Data file fncval.dat not found\n") ;
         fgets (txt, MAXSTR, fp) ;
         while (strncmp (txt, "Ba月sel Function Jn' , lB) ) {
             fget日(t工t ,MAI＄丁R, fp) ;
             if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
         }
         fsc키f (fp, "%d %*e", knval) ;
        printf ( "\ n加\n", txt) ;
        printf ( "V.4月 工7s Xi$s X20s \n' , "n", "x '. "actua].", 'bessj(n,x)
                                                                             ") ;
        for (i=1; i<=nval;i++) {
             facanf (fp. '%d %f %f ", kn,kx,*val) ;
            printf ( " 工44 X8. 2f 弦18. 6e 戈18. 6e\n' , n，工，val,be日Si (fl，工）) ;
        }
        fclose(fp) ;
        return 0;
}

Bessel function Io
／巾 Driver 如r routine bessio 中／

#include <stdio.h>
#include <atdlib . h>
*include <string.h>
*inc1u4e '1nr.h"
*include "nr끄til.h '
    96        Mime月ca/ 尸ec徊es ExampI9 Book


#def ins MAXSTR 80

mllt iuain(void)
{
         char txt[ MAXSTR] ;
         m1lt i, nval;
         fl oat val, x;
         FILE *fp;

         if ( (fp = f open( "fncval. dat ' , "r ") ) == NULL)
             nrerror ( 'Data fi le t ncval.dat not ound\n") ;
         fgets (txt ,MAXSTR, fp) ;
         while (etrncmp(txt, "Moditied Bessel Function 10 ", 27) ) {
              f gets (txt ,I1AXSTR, fp) ;
              it (feot (fp) ) nrerror ( 'Data not sound in facval.dat\n") ;
         }
         fscanf (fp, 'Y.d '/,*s", &nva].);
         printt ( "\ n%s\n" ,txt) ;
         prmntt ( '/ .5s %12a V,13s \n' , "x ", 'actual " , "bessio(x) ") ;
           or (i=1; i<=nval; i++) {
              fscaitf (fp, "Y.f %V', &x,kval) ;
              printf ( '%6. 2f %i2. 7f %12. 7f\ n", x,val, bessio(x) );
         }
         fclose(fp) ;
         return 0;
}

Bessel function K0:

/方 Driver         or routine besskO *1

#include <stdio . h>
#inc끄lde <stdlib . h>
#include <string. h>
#ittclude "nr. h'1
#include "nrutil. h"

#def ins MAXSTR 80

ml1t main(void)
{
         char txt[ MAXSTR] ;
         mllt i, nval;
         fl oat val, x;
         FILE *fp;

         it ( (tp = topen( "tncval. dat ", "r ") ) == NULL)
             nrerror ( "Data tile tncval.dat not 如und\n") ;
         tgets(txt ,MAXSTR, tp) ;
         while (strncmp(txt, "Modified Bessel Function 1(0 ", 27) ) {
              tgets(txt ,MAXSTR, fp) ;
              it (teot (tp) ) nrerror ( "Data not found in fncval.dat\n") ;
         }
         tscant (tp, "%d 冷s", knval) ;
         printf ( "\ n%s\n" ,txt) ;
         prmntt ( 'V.Ss V.13s 뷰18s \n", "x", "actual", "beseko(x) ') ;
                                                       Ch킥가er 6: 印ec洌 Fundi幻ns   97

    for (i=1, i<=nval; i++) {
        fscanf (fp, '%f %f ", &x,kval) ;
        printf ( "%6. 2f %16. 7e %16. 7e\n", x,val, bessko(x) );
    }
    fclose(fp) ;
    return 0;
}

Bessel function Ii:

/卞 Driver for routine bessil s/

*include <stdio.h>
#include <stdlib . h>
#include <string.h>
#include "nr. h"
#include 'nrutil. h1'

*def ins MAXSTR 80

ml1t iaain(void)
{
    char t工t江XAXSTR] ;
    mllt i, nval;
    float val, x;
    FILE *fp;

    if ( (fp = fopen( "fncval.dat ". "r ") ) == NULL)
        nrerror ( "Data file fncval.dat not found\n") ;
    fgets(txt, MAXSTR, fp) ;
    while (strncmp(txt, "Modified Bessel Function 11", 27) ) {
         fgets (txt ,MAXSTR, fp) ;
        if (feof (fp) ) nrerror ( "Data not found in fncval』dat\n") ;
    }
    fscanf (fp, "%d %ss", knval) ;
    printf ( "\ n%s\n" ,t工t) ;
    printf ( "7,55 %12s 艾13s \n" , "x", "actual", "bessil (幻") ;
    for (i=1; i<'nval; i++) {
        tsca끄f (fp, "/,f %f ", kx,kval) ;
        printf ( "%6. 2f %12. 7f %12.7f\ n", 工, val,bessil(x) );
    }
    fclose(fp) ;
    return 0;
}

Bessel function Kj:

/* Driver for routine besskl */

#include <stdmo . It>
#include <stdlib . h>
*include <string. h>
#include "nr. h"
#include "nrutil. h1'

*def ins MAISTE 80

mnt main(void)
    98            Numerica／尸ec徊es Examp旭 Book

{
         char txt[ MAXSTR] ;
         jut i, nval;
         fl oat val,x;
         FILE *fp;

         if ( (fp = fopen( "fncval.dat ' , "r ") ) == NULL)
             nrerror ( 'Data file fncval.dat not found\n") ;
         fgets(txt, MAXSTR, fp) ;
         while (strncmp (txt, "Modified Bessel Function Ki" .27) ) {
                  fgets (txt, 겨［AXSTR, fp) ;
                  if (feof (fp) ) nrerror ( "Data not found in fncval. dat\n") ;
         }
         fscanf (fp, "%d %*s", &l1val) ;
         printf ( "\ n加\n" .txt) ;
         printf ( "Y.5s %13s Y.17s \n", "x", "actual", 'besskl(x) ") ;
         for (i=i; i<=nval;i++) {
             fscanf (fp, "%f %f ", kx,&val) ;
             printf ( "Y.6.2f Y.16. 7e %16. 7e\n", x,val,besskl(x) );
         }
         fclose(fp) ;
         return 0;
}

Bessel function K。for n > 1:

／卞 Driver 如r routine bessk 卞／

#include <stdjo . h>
#include <atdlib . h>
#include <string.h>
#include "nr.h"
#include "nrutil . h'1

    #define MAXSTR 80

    jut main(void)
    {
          char t工t江MAXSTR] ;
          jut i, uval,n;
          float val, x;
          FIL丘 牛fp;

          if ( (fp = fopen( "fncval. dat", "r ") ) == 吼旺)
              nrerror ( "Data file fncval.dat not 如und\n") ;
          fgets(t工t，거［A工STE. , fp) ;
          while (strncmp (t工t, "겨 ［odified Bessel Function ICn", 27) ) {
                   fgets (t工t,片A工STR,fp) ;
                   if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
          }
          fscanf (fp, "Y.d 加s' , knval) ;
          printf ( "\ n%s\n" ,txt) ;
          print奴 "兄45 工75 工14s 工19s\n" , "n' , "工" ,"actual", "be口ek(u．工）" );
          for (i '1; i<=nval;i++) {
              fecant (fp, "Y.d %f %f ", &n,kx,&val) ;
                                                                            );
              printf ( "%4d %8. 2f %18. 7e %16.7a \n", n,工, val,bessk (n,x)
              }
                                                              Ch킥가er 6: 印ecial Fui兀甘ons   99

          fcloae(fp) ;
          return 0;
    }

    Bessel function I,    for n > 1:

    /* Driver for routine besaj */

    #include <stdio .h>
    #include <stdlib .h>
    #include <string.h>
    #inclucie '1nr.h"
    #include 'nrutil. h"

    #define 甘AXSTR 80

    jilt main(void)
    {
         cha工 txt[ MAXSTR] ;
         mnt i, nval,n;
         float val, x;
         FILE *fp,

         if  ( (fp = fopen( 'fncva]..dat", "r ') ) == 且t工LL)
              nrerror ( "Data file fncval.dat not found\n ") ;
         fgeta (txt , MAXSTE, fp) ;
         while (str如mp(txt, "Modified Beacel Function In ". 27) ) {
              fgets(txt . MAXSTR, fp) ;
              if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n') ;
         }
         fsc띠lf (fp, "/.d 加s", knval) ;
        printf ( '\ n加\n ', txt) ;
        printf ( 'X4s Y.7s Y.lss V.20e\n", "n", "x", "actua1", "beesi(n .x) ") ;
        for (i=1; i<=nval;i++) {
              fscanf (fp, "V.d %f %f ", 幻l,kx,tval) ;
             printf ( "7.4d '/.8.2f %18. 7e %18. 7e\n". n,x, vai,besaj(n, x));
        }
        fclose(fp) ;
        r日t;1U그10;
}

Bessel functions of fractional order, J, and Y:

/* Driver for routine beasjy */

#include <stdio . h>
#include <atdlib. h>
*include <string.h>
社mllci끄de "nr. h'1
#include "nrutil. h"

#define MAXSTR 80

mnt rnain(void)
{
        char t工t [Pu工S丁a] ;
        ml1t inval;
        float rj, ry, rjp. ryp，工1xnu.工rj．工ry，工rjp，工ryp;
100          Numerica사？ec徊es Examp旭 Book

    FILE *fp;

    if   ( (fp = fopen( "fncval. dat ", 'r ") ) == NULL)
          nrerror ( "Data fi le fncval.dat not found\n") ;
      fgets (txt , MAXSTR, fp) ;
      while (strncmp (txt, "Ordinary Bessel Functions ' ,25) ) {
             fgets (txt, MAXSTR, tp) ;
                                                                         ;
             if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n')
    }
    fscanf (fp, "%d %*s " , knval) ;
    printf ( "\ n加\n" ,txt) ;
    printf ("Y.5s V.7s\n/.14s Y.16s Y.17s V.16s\nY.14s Y.16s Y.17s %16s\n",
                                                                                         ;
             "xnu", "x ", "rj ", "ry' , "rjp ' , "ryp", "xrj ", 'xry ", "xrjp ", "xryp")
      for (i=1; i<=nva1; i++) {
          fscanf (fp, "Y.f Y.f %f Y.f 1.f Y.f ", &xnu,&x,krj, kry, 在rjp,kryp) ;
          bessjy (x, xnu,&xrj ,&xry,kxrjp, kxryp) ;
          printf ( "Y.5. 2f Y.5. 2f\ n\ t%16. 6e %16. 6e %16. 6e %16. 6e\n", xnu, x,rj, ry, rjp, ryp) ;
          printf ( "\ t7.16. 6e %i6. 6e 7.16. 6e %16. 6e\n", xrj, xry, xrjp, xryp) ;
      }
      fclose(fp) ;
      return 0;
}

   The routine bessjy calls the utility procedure beschb to calculate the following
quantities:

                                                     :
                                                      1
                 「『카           ,          （,
                                            F- 三 F(1- x)     ),
                                                                  r*
                                                                                           +F* )
                                  三
                                                                            F2
                                      -
                                               (F_
                                                         -             ),
                             F1
                                                                                     （F-
                                                                                 군
                                                                the results obtained
Test program xbeschb compares the result of calling beschb with
by calling gnini1n.
/* Driver for routine beschb */

#include <stdio.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

ml1t main(void)
{
         double gainl,gam2, ga皿pl,ga皿ml，工！xg키Ill，工g쾨n2, 工ga皿p1！工g키mni;

         for (; ;) {
             printf ( 'Enter x: \n") ;
             if (scanf ( "Y.lf ", kx) == BOF) break;
             beschb(x,kxg키ul, &xgam2,&工ga且pl. k工gammi) ;
             printf ( "/.ss\n%17s 7.16s '/.17s V.16s\n%17s Y.16s 7.178 Y.15s\n' ,
                                                                                             ', , "工g키n皿i') ;
                      "x", "gaml", "gam2", "ga呵：江 " , 'ga皿mi ' , " 工ga皿1" , ' 노ga皿2", 'xga皿p1
             gampl=l/ exp  (ga皿mln(  (float) (1+x) ));
             gaimnirl/ exp (g帥口mln( (float) (1-x) ));
              gam1 ' (gammi- gampl) /(2* x) ;
              gain2= (gaxsmi+ga皿pl) /2;
              printf ( "%5. 2f\n\t7.16. 6e Y.16.6e 7.16. 6e 工16. 6e\n", x,gaml, gam2,ga4apl,ga皿ni)
              printf ( "\ t%16. 6e %16. 6e %16.6e %16. 6e\n "，工ga皿I，工ga皿2，工ga皿pl, xgam皿i) ;
         1
                                                       Ch짜ter 6: Special Functions          101

    return 0;
}

Modified Bessel functions of fractional order, I. and K:
/* Driver for routine bessik 中/

#include <stdio . h>
*include <atdlib . h>
#include <string. h>
*include "nr.h"
#include nnrutil. h"

#define MAXSTR 80

jut main(void)
{
    char t工t [Puxs丁83 ;
    mllt i1nval,
    float ri, rk, rip, rkp.x,xnu, xri, xrk,xrip, xrkp;
    FILE *fp;

    if ( (fp = fopen( "fncval.dat ", "r ') ) == NULL)
        n工error ( 'Data file fncval.dat not found\n ') ;
    fgets (txt ,MAXSTR. fp) ;
    while (strncmp(txt, "Modified Bessel Functions ', 2&)) {:
        fgets (txt .甘%XSTR, fp) ;
        if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
    }
    fscanf (fp, "%d %*s", knval) ;
    printf ( "\ n%s\n" ,txt) ;
    printf ( "%ss %7艮\n%14s V.16w 工17w %16a\n%14a 戈16w V.17w %16s\n'1.
             "工1lu '，느" , 'ri " , "rk" . "rip " ,"rkp", "工ni" , 'xrk" , "xrip" . "xrkp") ;
    for (i=l; i<=nval; i++) {
        fscanf (fp, "%f Y.f %f V.f /.f %f ", &xnu,*x,kni,krk,krip, krkp) ;
        bessik(x, xnu,kxri, kxrk.&xrip,kxrkp) ;
        pnintf ( "工5. 2f V.5. 2f\n\t工16. 6e V.16.6e %16. 8e %16. 6e\n", xnu, x,ri, rk, nip,rkp) ;
        pnintf ( "\ t '/.16.6e %16. 6e V.16.6e V.16.6e\n". xri, xrk, xrip, xrkp) ;
    }
    fclose(fp) ;
    return 0;
}

Airy functions:
/李 Driver for routine airy */

#include <stdjo.h>
#include <stdlib . h>
*include <string.h>
#include "nr.h"
#include "nrutil. h"

卄def ins XAXSTR 80

jut main(void)
{
    cha工 t工t [XAXSTR] ;
 102        Numeric別 尸的徊es Examp旭 Book

      mllt i 1nval;
      fl oat ai1bi1aip,bip, x,工ai,工bi,工aip，工bip;
      FILE *fp;

      if ( (fp = 如pen( "fncval. dat ", "r ") ) == NULL)
          nrerror ( "Data file fncval.dat not 如und\n") ;
      fgets (txt , MAXSTR , fp) ;
      while (strncinp(txt, "Airy Functions" ,14) ) {
           fgets (txt, MAXSTR, fp) ;
          if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
      }
      fscanf (fp, "Y.d 小a", &nval) ;
      printf ( "\ nY.s\n" ,txt) ;
      printf ( "%ss\n%14s '/.16s 工17s Y.16s\n%14s %16月 Y.17s %16s\n",
               " X ", "ai ", "bi ' , "aip ' , "bip" ,"xai " , "xbi" , "xaip" ,"xbip") ;
      for (i "l; i<'nval; i++) (
          fscanf (fp, "Y.f /.f V.f %f Y.f ", kx,kai, kbi, &aip,kbip) ;
          airy (x, &xai,&工bi,缸aip,&工bip) ;
          printf ( "Y.5.2f\ n\ t '/.16. 6e Y.16. 6e %16. 6e /.16. 6e\n", x,ai, bi, aip,bip) ;
          printf ( "\ t%16. 6e %16. 6e '/.16. 6e %16. 6e\n", xai, xbi, xaip,xbip) ;
      }
      fclose(fp) ;
      return 0,
:1.

Spherical Bessel functions:
／牛 Driver 如r routine rj               中／

#include <stdio . h>
#include <stdlib. h>
#include <string.h>
#include '뇨r.h"
#include 'nrutil. h"

*define MAXSTR 80

mltt main(void)
{
     char txt[ NAXSTR] ;
     mnt i, n,nval;
      float sj, sy,sjp, syp, x, xsj. xsy, xsjp,xsyp;
      FILE 字fp;

       if ( (fp = fopen( "fncval. dat ", "r ") ) == NULL)
           nrerror ('Data file fncval.dat not found\n ") ;
       fgets(txt ,MAXSTR, fp) ;
       while (strncmp(txt, 'Spherica]. Bessel Functions", 26) ) {
            fgets (txt, MAXSTR, fp) ;
            if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
       }
      fscanf (fp, ' '/.d 小s", &nval) ;
      printf ( '\ n%s\n" .txt) ;
      for (i= i; i<=nval;i++) {
          fec띠if (fp, "%d 工f /.f %f 工f 加" kn, &工，如j ,&sy,&ejp,&町끼；
          prmntf ( "Y.5s %4s\n%14s 工16s %17s %16s\n'/.14a '/.16s %17s %16s\n ",
                    "U,, , " 工" , " 8j " , " 8y " , " 町P" , " 8yF1" , " 工二j " , " 工sy', . " 工ajP " , " 工syp") ;
                                                               Ch콰批9r 6: 印e口a! Func加ns               103
                sphbas (n,x,kxej ,kxsy,kxsjp,&xsyp) ;
                printf ( "%Sd %5. 2f\n\t%16.6e 7.16. 6e %16. 6e 兄16. 6e\n",n,
                                                                                   x,sj, sy,町p, syp) ,
                printf ( "\ t%16. 6e %16. 6e %16. 6e '/.16. 6e\n", xsj, xay,xsj
                                                                                p, xsyp) ;
            }
            fc;lose(fp) ;
            return 0;
    }

    Legendre polynomials:
    /卓 Driver for routine plgndr */

 #include <atdio . h>
 #include <stdlib . h>
 *include <string.h>
 #include <math.h>
 *include "nr.h"
 #include "nrutil. h"

 #def ins )4AXSTR 80

    jot main(void)
{
        char t工t［甘AXSTR] ;
        mllt i, j, m,n,nval;
        float fac, val,x;
        FILE *fp;

        if  ( (fp = 如pen( "fncval.dat ", "r ") ) == MULL)
             nreri'or ( "Data file fncval.dat not found\n") ;
        fgate(txt, MAXST8.fp) ;
        毗ile (strncmp(txt, "Legendre Polynoinials", 20) ) {
             fgets (txt, MAXSTR, fp) ;
             if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
        }
        fscanf (fp, "74 V.*s", knval) ;
        printf ( "\ n加＼n" ,t工t) ;
        printf ( "%4s %4s %los 7.178 뷰24e\n", "n",
             "in", "x" ,"actual", "plgndr(n,m, x) ") ;
        for (i=1; i<=nva1;i++) {
             fscanf (fp, "%d %d %f %f ", &n,&in,kx,&val) ;
             fac=l. 0;
             if (a > 0)
                  for (j=n-m+1; j<=n+rn; j++) fac 才
             fac *= 2.0/ (2.0*n+1.0) ;
             val *= sqrt (fac) ;
            printf ( "%4d %4d X13.6f %19.6e Y.19. 6e\n",
                  n,m, x. val,plgndz(n,m, x) );
        }
        fclose (fp) ;
        return 0;
}

Fresnel integrals:
/／卞 Driver for roi工tine freanel 卞／

#include <atdio.h>
    104         N미nerica/ 尸00衣）es Examp旭 Book

#include <stdlib . h>
#include <string. h>
#include "nr. h"
#include "urutil . h'1

#deflne MAXSTR 80

mllt main(void)
{
          char txt[ MAXSTR) ;
          jut i, nval;
          fl oat C 戶 1 工 1 工C. 工a;
          FILE *fp;

          if ( (fp = topen("fncval. dat ", "r ") ) == 月t兀L)
              nrerror ( "Data file tncval. dat not tound\n") ;
          fgets (txt, MAXSTR, fp) ;
          while (strncmp(txt, "Fresnel Integrals". iT) ) {
                fgets (txt, MAXSTR, fp) ;
                                                                           );
                if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n"
          }
          fscanf (fp, "%d %*s", knval) ;
          pri毗n " \l}X8\n" 1t工t) ;
          prmntf ( "%S日 %12s 7.14s %16a 뷰14s \n",
              "x ", "actual", "c (x) ", "actual", "s(x) ") ;
          如r (i=1; i<=nval; i++) {
              fscanf (fp, "%f Y.f 7.f ", kx,&xs,kxc) ;
                frenel(x, &s,kc) ;
                printf ( "Y.6.2f %15. 6e Y.15. 6e %16. 6e /.1S. 6e\n",
                    X , 工c ,s , xc , c) ;
          }
          tclose(fp) ;
          return 0;
    }

    Cosine and 前ne ii此egra뇨

／卞 Driver 加r routine cisi 中／

    *include <stdio.h>
    #include <stdlib. h>
    #include <string.h>
    #include "nr. h"
    #include "nrutil. h"

    #def ins MIIXSTR 80

    jut main(void)
    {
           char txt (MAXSTR] ;
           mllt i, nval;
           float ci, si, 工1工ci, 工Si;
           FILE *fp;

           if ( (fp = fopen( "fncval.dat", "r ") ) == lULL)
               nrerror ( "Data file fncval.dat not found\n") ;
           fgets (txt, MAXSTR, tp) ;
                                                               Ch카升er 6: S戶ecial Func加ns   105
            while (strncmp(txt, "Coeine 띠1d Sine Integrals", 25) ) {
                fgets(txt, MAXSTR. fp) ;
                if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n') ;
            }
             fscanf (fp, "Y.d %*s", knval) ;
            printf ( '\ n%s\n" .txt) ;
            printf ( "/.ss /.12s Y.12s 7.12s Y.12s \n",
                  'x '', "actual' , "ci (x)", "actual", 'si (x) ") ;
            for (i=1; i<=nval; j++) {
                 fscanf (fp, '%f %f %f ' , kx,&xci,kxsi) ;
                 cisi (x, &ci,ksi) ;
                 printf ( "%6. 2f %12. 6f %12. 6f %12. 6f %12. 6f\ n",
                        工 1工ci, ci, 工si, si) ;
            }
            fclose(fp) ;
            return 0;
    }

 Dawson's integral:
／卞 Driver for routine da日son 卞／

 #includa <stdio . h>
 #include <stdlib . h>
 #include <string .h>
 #include 'nr. h"
 #include "nrutil. h"

#define MAXSTR 80

mnt main(void)
{
        char t工t［甘A工STR] ;
        mllt i, nval;
        float val, x;
        FILE *fp;

        if ( (fp = fopen( "fncval. dat ", "r ") ) == NULL)
            nrerror ( "Data file fncval.dat not found\n") ;
        fgets(txt .MAXSTR. fp) ;
        while (strncmp (txt, "Da日son integral ', 15) ) {
            fgets (txt, MAXSTR, fp) ;
            if (feof (fp) ) nrerror( "Data not found in fncval.dat\n") ;
        }
        fscanf (fp, "Xd %*s", tnval) ;
        printf ( "\ n%s\n ' .txt) ;
        printf ( " 工Ss Y.12s %lls \n", "x ", "actual", 'dawson(x) ") ;
        for (i '1; i<=nval; i++) {
            Zscanf (fp, "%f %f ', &x,kval) ;
            printf ( '%6.2f %12. 6f %12. 6f\ n", x.va].,da日son(x) );
        }
        fclo月e(fp) ;
        return 0;
}

Carison's elliptic integral of the first kind:
    106       Nun治rica사？ec徊es Examp旭 Book

/* Driver for routine rf        中/

#include <stdio.h>
#include <stdlib . ii>
#include <string. h>
#include "nr. h"
#include "nrutil. h1'

#define I4AXSTR 80

mnt main(void)
{
      char txt[ NAXSTR] ;
      jut i, nval;
      fl oat val, x, y,z;
      FILE *fp;

      if ( (fp = fopen( "facval. dat ". 'r ") ) == NULL)
          nrerror ( "Data file fncval.dat not found\n ') ;
      fgets (txt ,MAXSTR, fp) ;
      while (strncmp(txt, 'Elliptic Integral First Kind RF", 31) ) {
              fgets (txt, MAXSTR ,fp) ;
              if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n') ;
      }
      fscanf (fp, '%d 肛s ', &nval) ;
      printf ( "\ n%e\n" ,txt) ;
      printf ( "Y.7s V.8s %8s Y.16s 1.20s\n", "x", "y ', 'z ' , 'actUal", "rf (X, y.z) ") ;
      for (i=1; i<=nva1; i++) {
          fscanf (fp, 'Y.f %f %f %f ", kx,ky,kz,&val) ;
          printf ( "Y.8. 2f h8. 2f %8. 2f %18. 6e V.18. 6e\n' , x.y.z, va].,rf (x. y.z) );
      }
      fclose(fp) ;
      return 0;
}

Carlson's elliptic integral of the second kind:
/* Driver for routine rd 卞/

#include <stdio . h>
#include <atdlib. h>
#include <string.h>
#include "nr. h11
#include 'nrutil. h"

作define MAXSTR 80

mllt main(void)
{
      char t工t [MA工STR] ;
      mnt i, nval;
      float val, x,y,z;
      FILE *fp;

      if     ( (fp = fopen( "fncval. dat ", "r ") ) == NULL)
              nrerror ( "Data file fncval.dat not found\n") ;
          fgets (txt, MAXSTR, fp) ;
                                                        Ch司7ter 6: 印印洌向nc加ns              107

     vhile (strncmp(txt, "Euiptic Integral Second Kind RO", 32) ) {
         fgete (t工t．片A工STR. fp) ;
         if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n ') ;
     }
     i8C띠if (fp. "%d 加B " 小ival) ;
     printf ( "\ n加뇨l" 1t工t) ;
     printf ( '%Ts Y.8s /.8s Y.16a %20a\n", "x", "y' , "z". "actual", "rd(x,y,z) ") ;
     for (i=1;i<=nval; i++) {
         f月canf (fp, "7.f %f 加 加" 'a工,&y,&z.kval) ;
         printf ( "%8.21 %8. 2f %8. 2f %18. 6e %18.6e\n", r, y,z,val,rd(x,y,z) );
     }
     fclose(fp) ;
     r口tu口i 0;
}

Carilson's elliptic integral of the third kind:
／卞 Driver 如r routine rj 中／

#include <stdio.h>
#include <stdlib.h>
寸mllci끄de <etring.h>
#inciude 11nr.h"
#include "urutil. h"

#define MAXSTR 80

mi1t :eain(void)
{
    cha工 t工t [M*xSrRJ ;
    jut i, nval;
    float p,v@,x, y,z;
    FILE CfP;

     if ( (fp = fopen( "fncval.dat ", "r ") ) == NULL)
         nrerror ( "Data file fncval.dat not 如und\n") ;
    :tgets (t工t，甘A工STR, fp) ;
    while (atrucmp(txt, "Elliptic Integral Third Kind RJ", 31) ) {
          fgets(txt ,MAISTR, fp) ;
          if (feof (fp) ) nrerror ( "Data not 如und in fncval.dat\n") ;
    ：卜
     fecanf (fp, "%d %*a", 1vai.);
    printf ( "\ n%B\u" .txt) ;
    prmntf ( "%7e %8a V.88 %8s %16e %20a\n", "x" , "y", "z", "p", "actual", "rj (x,y,z,p) ') ;
    for (i=1; i<=nva1;i++) {
         fsc띠lf (fp, "%f %f '/,f 加 V.f ", kx,ky,kz,kp,*va].);
         prmntf ( "%8.21 %8. 2f %8. 2f 工8. 2f 118.6e %18. 6e\n", x,y,z,p, va].,rj (x,y,z,p) );
    :F
    fciose(fp) ;
    return 0;
}

Carison 's degenerate elliptic integral:
/* Driver 如r roi工ti끄a rc 中／

#inciude <atdio.h>
Sinciude <stdlib.h>
    108      Nu,刀erica／尸ec徊es Exa叫,Ie Book

#include <string. h>
#include "nr. h"
Sinclude 1'nrutil. h"


    define MAXSTR 80

mnt main (void)
{
       cha工 txtEMAXSTRJ;
       jilt i, nval;
       float val 1x 1y;
       FILE *fp;


       if   ( (fp = fopen( 'fncval. dat ", "r ") ) == NULL)
             nrerror ( "Data file fncval. dat not found\n") ;
       fgets (txt ,MAXSTR, tp) ;
       while (strncmp(txt, "Elliptic         Integral Degenerate EC ", 31) ) {
             fgets (txt ,MAXSTR, fp) ;
             if   (feof (fp) ) nrerror ( "Data not found in fncval. dat\n") ;
       }
       fscanf (fp, "%d %*s " , knval) ;
       printf ( "\ nY.s\n" ,txt) ;
       printf ( "%7s V.8s %16s Y.18s\n", '"x '", '"y "", "actual", "rc (x, y) ") ;
       for (i= 1; i< =nval; i++) {
            fscanf (fp, "V.f Y.f /.f ", &x, ty, &val) ;
            printf ( "Y.8. 2f Y.8. 2f Y.18. 6e %18. 6e\n" ,x, y, val, rc (x, y) );
       }
       fclose (fp) ;
       return 0;



Jegendre elliptic integral of the first kind:
r巾 Driver for routine ellf           巾/

1include <stdio. h>
tinclude <stdlib. h>
"include <string. h>
 include <math.h>
    include "nr. h"
    include "nrutil.    h"


    define MAXSTR. 80


    define FPC (3. 1415926535/180. 0)


nt main(void)


       char txt[ MAXSTR] ;
       mnt i, nval;
       float 心；,alpha,phi, val;
       FILE ifp;


       if   ( (fp = fopen( "fncval. dat ", 'r ") ) == NULL)
             nrerror ( "Data file fncval. dat not found\n") ;
       fgets (txt, MAXSTR, fp) ;
       while (strncmp(txt, 兀egendre Elliptic            Integral First      Kind", 37) ) {
                                                             Ch짜ter 6: Special Functions        109

             fgets(txt ,MAXsTR, fp) ;
             if (feof (fp) ) n工error ( "Data not found in fncval. dat\n") ;
    }
    fsc치lf (fp, "%d %中s", kuval) ;
    printf ( "\ n加＼m 't工t) ;
    printf ( "/.5s '/.lOs 工lls Y.22a\n", "phi". "sin(alpha) ", "actual", "ellf (phi, ak) ") ;
    for (i '1; i<=nval; i++) {
         fecanf (fp, "%f %f Y.f ", kphi,kalpha,&val) ;
             alpha=alpha卞FkC;
             ak=sin(alpha) ;
             phi=phi杆沮C;
             printf ( "%6. 2f Y.6. 2f Y.18. 6e %18. 6e\n", phi, ak, val, ellf (phi, ak) );
    }
    fclose(fp) ;
    return 0;
}

Legendre elliptic integral of the second kind:
／中 Driver 如r routine elle 本／

#include <stdio.h>
#include <stdlib. h>
#include <string.h>
#include <math.h>
Ninclude "nr. h"
#jnclude "nrutil. h"

#define MA7STR 80

甘define FAC (3. 1415926535/ 180. 0)

jut main(void)
{
     char txt [NAXSTR] ;
     mnt i, nval;
     float ak, alpha,phi, val;
     FILE ifp;

        if   ( (fp = fopen( "fncval. dat ", "r ") ) == NULL)
              nrerror ( "Data file fncval. dat not found\n") ;
        fgets(txt. MAXSTR, fp) ;
        while (strncmp(txt, "Legendre Elliptic Integral Second Kind' .38) ) {
            fgets(txt ,MAXSTR, fp) ;
            if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
        }
        fscanf (fp, "%d Y.*s ", &nval) ;
        printf ( "\ nV.s\n" ,txt) ;
        printf ( "%ss %l0s %lls Y.22s\n" ,"phi ", 노in(alpha) " ,"actual", "elle (phi, ak) ") ;
        for (i=1; i< 'nval; i++) {
             fscanf (fp, " 工f %f %f ", &phi,kalpha,&val) ;
            alpha=alpha*FAC;
            ak=sin(alpha) ;
            phi=phi*FAC;
            printf ( "Y.6. 2f '/.6. 2f %18. 6e 工18. 6e\n", phi, ak, val, alle (phi, ak) );
        }
        fclose(fp) ;
    110     Numerical Recipes Example Book

      return 0;
}

Legendre elliptic integral of the third kind:
/수 Driver for routine elipi 卞/

Sinclude <stdio.h>
#include <stdlib. h>
Sinclude <string.h>
Sinclude <math.h>
#include "nr. h"
#include "nr此il. h"

#define MAXSTR 80

#defin日 FAC (3. 1415926535/180. 0)

jut main(void)
{
      char txt [MAXSTR] ;
      mnt i, nval;
      float ak,alpha, en1phi, val;
      FILE *fp;

      if  ( (fp = fopen( "fucval.dat ", "r ') ) == NULL)
           nrerror ( ' 'Data file fncval.dat not found\n") ;
      fgets (txt, MAXSTR, fp) ;
      while (strncmp(txt, "Legendr日 Elliptic Integral Third Kind' , 37) ) {
           fgets (txt, MAXSTE, fp) ;
           if (feof (fp) ) nrerror ( ''Data not found in fncval.dat\n') ;
      }
      fscanf (fp, '%d /.*s ", &nval) ;
      printf ( '\ n%s\n" ,txt) ;
      printf ( 'Y.6s %6s 7.6s Y.los 工23s\n",
             ' 'phi", "- en", 'sin (a1pha) " ,'actual ' , "ellpi (phi, ak) ") ;
      for (i=1; i<=nva1; i++) {
          fsc카lf (fp, '%f %f 工f 工f ", kphi,&en,kalpha,&val) ;
          alpha=alpha*FAC;
       '  ak=sin(alpha) ;
          en = -en;
          phi=phi*FAC;
          printf ( "%6. 2f Y.6.2f %6. 2f %18. 6e 工18. 6e\n",
                  phi, en,ak, val, ellpi (phi, en,ak) );

      }
      fclose(fp) ;
      return 0;
}

    Routine sncndn returns Jacobian elliptic functions. The file fncval .dat contains
information only about function an. However, the values of cn and dn satisfy the
relationships
                       sn2+ cn2= 1,        k2sn2+ dn2= 1.
The program xsncndn works exactly as the others in terms of testing an, but for
verifying cn and dii it lists the values of the left sides of the two equations above.
                                                       Ch카가er 6: 印ecial Func加ns   111

Each of them should have the value 1.0 for all choices of arguments.
／卞 Driver for routine sncn山l 卞／

#inc].ude (atdio . h>
*inc].ude <etdlib .h>
#include <string.h>
*inc].ude "nr.h'1
#include "nrutil. h"

#define MAXSTR 80

mllt main(void)
{
     char t工t [MA工STR] ;
     jut 工 ,nva1;
     float em, emmc,uuval, an, cn,dn;
     FILE *fp;

    if ( (fp = fop.n('fncval.dat ", "r ") ) == NULL)
        nrerror ( "Data file t ncval.dat not 如und\n") ;
    fgets(txt, MAXSTIt, fp) ;
    while (strncmp(txt, "Jacobian Elliptic Function", 26) ) 4[
        fgets(txt. MAXSTR, fp) ;
        if (feof (fp) ) nrerror ( "Data not found in fncval.dat\n") ;
    )
    f日canf (fp, "%d 7.*s", knval) ;
    printf ('\ n%a\n' 1 txt) ;
    printf ( "%4s Y.8s V.16e %13s Y.15s %18s\n", "mc ', 'u' . "actua].",
        "en", "snn2+cnn2" , " (mc)*(en2)+dn2") ;
    for (i '1; i<=nval;i++) {
        fec띠if (f p. "加 加 戈f ", &em,&uu,kval) ;
        em皿c=1. 0-em;
        encndn(uu, eamc,ken,kcn,kdn) ;
        printf ( "%5.2f %8.2f '/.i& .&f %IS.6f %12. &f Y.14.5f\n",
              emmc,uu,val,sn,(sn*月n+cnscn) ,(em卞sn卞s小dnsdn) );
    }
    fclose(fp) ;
    ret1口r끄 0;
}                                                                                   f


    The test program xhypgeo tests out the suite hypgeo, hypdrv and hypser by
calculating a hypergeometric function that can be expressed in closed form:

                               2F咐,1烏키        ＝知나는
                             2.F노（{, 1, 릊，_z2)
                                               긍，旽븐는
The program prompts you to enter various values of x and p and compares the results
如rz = 工 + jy.
／中 Driver for routin口 切pgeo 卞／

#iaclude <etdjo.h>
tinclude <工ath.h>
*include "nr.h"
#include "nxutil .h"
    112    Numerical Recipes Example Book

#incl끄de "comple工．h'

fcomplex Clog(fcomplex a)
{
    fcomplex b;

      b.r=log(Cabs (a) );
      b. i 'atan2(a. i, a.r) ;
      return b;
}
int inain(void)
{
      fcomplex a,b, c,z,zi, ql, q2, q3, q4;
      float 工 ,y;

      a 'Complex (0.5,0. 0) ;
      b=Compl日工（1. 0,0. 0) ;
      c=Complex (1. 5,0. 0) ;
      for (; ;) {
           printf ( "INPUT X, Y OF COMPLEX ARGUMENT: \n") ;
           if (scanf ( "%f Y.f ", &x, &y) == EOF) break;
           z=Com아e工伍 ,y) ;
           ql=hypgeo (a,b, c,Cmul(z, z) );
           q2=RCmul(0 .5, Cdiv (Clog(Cdiv (Cadd(b,z) ,Csub(b,z) )) ,z) );
           q3'hypgeo(a,b, c,RCmul (- 1. 0,Cmul(z, z) ));
           zi=Complex (- y, x) ;
           q4=RCmul(0.5,Cdiv (Clog(Cdiv (Cadd(b,zi) ,Csub(b,zi) )) ,zi) );
           printf ( "2F1(0. 5,1.0,1. 5; zn2) = /,12. 8f %12. 6f\ n", ql. r, ql. i) ;
           printf ( "check using log form: Y.12. 6f %12. 6f\ n", q2.r, q2. i) ;
           printf ( "2F1(0.5,1. 0, 1. 5; -z2) =7.12.6f %12. 6f\ n" , q3.r, q3.i) ;
           printf ( "check using log form: %12. 61 %12. 6f\ n", q4.r, q4.i) ;
      }
      return 0;
1

                                               Appendix

File fncval .dat:

Values of Special Functions in format x,F(x) or x,y,F(x, y)
Dawson integral
4 Values
0. 04 0. 0399573606
0.16 0. 1572970920
1.6   0. 3999398943
10. 0 0. 0502538471
0rdinary Bessel Functions          nu,工 , inn（工）1 ynu（工）,jnup（工）1 ynup（工）
20 Val끄es
2.0   1.0    1. 149034849E-01 -1. 6606826075+00 2. 102436159E-01 2. 620152392E+00
2. 0  2.0    3. 528340286E-01 -6. 174081042E-01 2. 238907791E-01 5. 103766726E-01
2.0   6.0    4.656611628E-02 3. 676628826E-01 -3. 4620518415-01 7 .9799034905-04
2. 0 10. 0   2. 646303137E-01 -5. 868082442E-03 -7. 453316&68E-03 2. 501890407E-01
2.0 50. 0 -5. 9712800795-02 9. 579316873E-02 -9. 5123316095-02 -6. 062739531E-02
5.0   1.0    2. 4975773025-04 -2. 604058666E+02 1. 227850313E-03 1. 268760910E+03
6.0   2.0    7. 039629756E-03 -9. 936989128E+00 1. 639664542E-02 2. 207402969E+01
5.0   5. 0   2. 6114064815-01 -4. 636948225E戶01 1. 300918143E-01 2.616626351E-01
                                                             Chapter 6: 助ec洌 Fun아幻ns              나:3

6. 0     10. 0    -2, 340615282E-01 1. 3540304775-01 -1. 025719220E-01 -2. 1265103575-01
5. 0  50. 0       -8. 1400247705-02 -7. 854841391E-02 7. 898 100205E-02 -8. 0203232695-02
10. 0 1. 0         2. 630615124E-10 -1. 216180143E+08 2. 6186350565-09 1. 209399938E+09
10. 0  2. 0        2. 515386283E-07 -1. 2918454225+05 1. 234650294E-06 6. 3136288175+05
10. 0 6. 0         1. 467802647E-03 -2. 512911010E+01 2. 584677845E-03 4. 2494337005+01
10. 0 10. 0        2. 074861066E-01 -3. 5981415225-01 8. 436957863E-02 1. 6051488645-01
10. 0 50. 0       -1. 138478491E-01     5. 723897182E-03 -4. 4228912 14E尸03    1. 116145748E-01
20. 0     1. 0      3. 8735030095-25 -4. 113970315E+22    7. 7377783955-24     8. 2171064665+23
20. 0     2. 0      3. 9189728055-19 -4. 081651389E+16    3. 9002704685-18     4. 060105807E+17
20. 0        2. 770330052E-11 -5. 933965297E+08 1. 0746938215-10 2. 294022549E+09
          5. 0
20. 0 10. 0  1. 151336925E-05 -1. 597483848E+03 2. 011953903E-05 2. 737803151E+03
20. 0 50. 0 -1. 167043528E-01 1 . 644263395E-02 1. 368329398E-02 -1. 07 17 17 1865-01
Modified Bessel Functions          nu, x, inu(x) ,knu(x) ,inup(x) , knup(x)


2.0       0. 2      5. 016687514E-03    4. 951242929E+01    5. 033395889E-02 4. 9990026545+02
2.0       1. 0      1. 357476698E小01    1. 624838899E+00    2. 936637645E-01 -3. 85 1585027E+00
2. 0      2. 0      6. 889484477E-01    2. 537597546E-01    9. 016884069E-01 3. 9362563645-01
2.0       2. 5      1. 276466148E+00    1. 214602063E-01    1. 4955433275+00 1.7105898145-01
2. 0      3. 0      2. 245212441E+00    6. 151045847E-02    2. 456561923E+00 -8. 116340344E-02
2.0       5. 0      1. 75056 1497E+01   5. 308943712E-03    1. 733339616E+01 6. 168190930E-03
2. 0     10. 0      2. 281518968E+03    2. 1509817015-05    2. 214684510E+03 -2. 295073686E-05
2. 0     20. 0      3. 931278522E+07    6. 3295436 12E-10   3. 852369486E+07 -6. 5160123315-10
3. 0      1. 0      2. 216842492E-02    7. 101262825E+00    6. 924239499E-02 2. 292862737E+01
3. 0      2. 0      2. 127399592E-01    6, 473853909E-01    3. 698385088E-01 1. 2248378415+00
3. 0      5.0       1. 033115017E+01    8. 2917684155-03    1. 130692487E+01 -1. 0284004765-02
3. 0     10. 0      1. 758380717E+03    2. 725270026E-05    1. 754004753E+03 -2. 9685627085-05
3. 0     50. 0      2. 677764139E+20    3. 7279367745-23    2. 6557647925+20 -3. 7716080455-23
5. 0      1. 0      2. 714631560E-04    3. 609605896E+02    1. 379804441E-03 -1. 8490353645+03
6. 0      2. 0      9. 825679323E-03    9, 4310491015+00    2. 616437167E-02 -2. 5773538685+01
5. 0      5. 0      2. 157974547E+00    3. 27062737 1E-02   2. 9502602 16E+00 -4. 7965339525-02
5. 0     10. 0      7. 7718828645+02    5. 754184999E-05    8. 378963946E+02 -6. 663236215E-05
6. 0     50. 0      2. 278548308E+20    4. 367 1822545-23   2. 267244113E+20 -4. 4320024775-23
10. 0     1. 0      2. 752948040E-10    1. 807 132899E+08   2. 765437823E-09 -1. 817137940E+09
10. 0     2. 0      3. 016963879E-07    1 .6248240405+05    1. 5357039635-06 -8. 302224962E+05
10. 0     5. 0      4. 580044419E-03    9. 758562829E+00    1.0155629985-02 -2. 202940355E+01
10. 0 10. 0         2. 189170616E+01    1. 614255300E小03    3. 0427586345+01 -2. 324264 134E-03
10. 0 50. 0         1. 0715971595+20    9. 150988210E-23    1.082473779E+20 -9. 419859989E-23
20. 0 1. 0          3. 966835986E-25    6. 294369360E+22    7.943111714E-24 -1. 2605290765+24
20. 0  2. 0         4. 3105605765-19    5.770856853E+16     4. 33 10428085-18 5. 8011415195+ 17
20. 0 5. 0          5. 024239358E- 11   4. 827000521E+08    2. 0687192745-10 -1. 993 195442E+09
20. 0 10. 0         1. 2507997365-04    1. 787442782E+02    2. 7847781185-04 -4. 015325804E+02
                    5. 442008403E+18    1. 706 148380E-21   5. 814242572E+18 -1. 852264589E-21
Spherical Bessel Functions       n, x, sjn (x) ,syn(x) ,sjnp (x) ,synp (x)
11 Values
0   0. 1  9.9833417E-01 -9. 9500417E+00 -3. 3300012E-02           1. 0049875E+02
0   1. 0  8. 4147098E尸01 -5. 4030231E-01 -3. 01168685-01          1. 3817733E+00

0 0
    5. 0 -1. 9178485E-01 -5. 6732437E-02      9. 5089408E-02 -1. 8043837E-01
       50. 0     -5. 24749715-03   -1. 92993215-02     1. 9404271E-02    나4. 8615107E寸03
l
d
        0. 1      3. 3300012E-02   -1. 0049876E+02     3. 3233393E-01     2. 0000250E+03
1       1. 0      3. 0116868E-01   -1. 3817733E+00     2. 3913363E-01     2. 2232443E+00
1       5. 0     -9. 5089408E-02    1. 8043837E-01    -1. 5374909E-01    -1. 2890778E-01
1  50. 0 尸1. 9404271E-02            4. 86 15107E-03   -4. 47 13263E-03    1. 949378 1E中02
20 1. 0   7. 53779575-26           -3. 2395922E+23     1 . 5058053E-24    6. 7948312E+24
20 5. 0   5. 4277268E-12           -9. 26795 14E+08    2. 1071414E-11     3. 7715819E+09
20 50. 0 -1. 5785030E-02            1. 375953 1E-02   -1. 2204181E-02    -1. 4702296E느02
Airy Functions
8 Values
 114     Num아七a／尸e帥始s Exa／까Ie Book

 -3. 5 -0. 37563382 0. 16893984 -0. 34344343 -0. 69311628
 -2. 0   0. 22740743 -0. 41230269 0.61825902 0. 27879617
 -1. 0   0. 53656088 0.10399739 -0. 01016057 0.59237563
 -0. 01 0.35761619 0. 61044364 -0. 25880167 0.44831896
  0. 00 0.35502805 0. 61492663 -0. 25881940 0. 44828836
  0. 01 0. 35243992 0. 61940962 -0. 25880174 0. 44831926
  0. 5   0. 23169361 0. 85427704 -0. 22491053 0.54467256
  1.00 0.13529242 1. 20742359 -0. 15914744 0.93243593
Elliptic Integral First Kind PS
3 Values
   0.1        0. 1      0.1        3. 16227766
   0.0        1.0       2.0       1. 31102878
100. 0     100. 0    100. 0       0.1
Elliptic Integral Second Kind RD
3 Values
   0. 1       0.1       0.1       31. 6227766
   0.0        2.0       1.0       1.79721036
100. 0     100. 0    100. 0       0.001
Elliptic Integral Third Kind 53
3 Values
   0.1        0. 1      0.1         0.1    31. 6227766
   2.0        3. 0      4.0         5. 0   0. 142975797
100. 0     100. 0    100. 0     100. 0      0.001
Elliptic Integral Degenerate SC
S Values
   0.1        0.1         3.16227766
   0. 0       0. 25       3. 14159265
   0. 0625 0. 125         3. 14159265
   2. 25      2. 0        0.69314718
100. 0     100. 0         0.1
Legendre Elliptic Integral First Kind
9 Values
  5. 0   2.0        0. 08726660
  5. 0 30. 0        0.08729413
  5.0 88. 0         0. 08737730
30. 0    2.0        0. 52362636
30.0 30. 0          0.52942863
30. 0 88. 0         0. 54927042
90. 0    2,.0       1.57127496
90. 0 30. 0         1. 68576035
90. 0 88. 0         4. 74271727
Legendre Elliptic Integral Second Kind
9 Values
  5.0    2. 0       0. 08726633
  5. 0 30.0         0. 08723881
  5. 0 88. 0        0.08715588
30. 0    2. 0       0.52357119
30. 0 30. 0         0. 51788193
30. 0 88. 0         0.50003003
90. 0    2. 0       1.57031792
90. 0 30.0          1.46746221
90. 0 88. 0         1.00258409
Legendre Elliptic Integral Third Kind
12 Values
16. 0     0.4       30.0       0. 264953
60. 0     0.6       90. 0      1.71951
90. 0     0.0       30.0       1.68575
                                                  Ch짜）ter 6: 部eciaI Funct幻ns   115

90.0    0.9     75. 0     12.46407
16.0    1. 0    15.0       0. 268156
46. 0   0. 0625 30. 0      0. 813845
45.0    0. 626 30.0        0.921130
46.0    1. 25   30.0       1. 132136
45. 0  -0. 25   30. 0      0. 769872
90. 0   0.0625 30.0        1.743055
90.0    0.626 30. 0        2. 800989
90. 0  -0. 26   30. 0      1. 501762
Fresnel Integrals
6 Values
 0.1   0. 0006236     0.0999975
 1. 0  0. 4382591     0. 7798934
 1.5   0.6975050      0.4452612
 2.0    0. 3434157    0. 4882534
 5.0    0.4991914     0. 5636312
20. 0   0. 4840845    0.4999873
Exponential Integral En             n.工 1 En（工）
13 Values




 0 2 3 4 2 3 4 m 的 2 加 2 加
        1.0      0. 3678794
        0. 0     1.0000000
        0.0      0. 5000000
        0. 0     0. 3333333
        0.5      0.3266439
        0.5      0. 2216044
        0. 5     0.1652428
        0. 5     0. 0634583
        0.5      0. 0310612
        6.0      0. 9964690E-03
        5. 0     0. 2782746E-03
       50. 0     0. 37 11.7836-23
       50. 0     0. 27664236-23
Cosine 카ld Sine Integrals
17 Values
  0. 1  -1. 727868E+00       9.994446E-02
  0. 2  -1. 042206E+00       1.995561E-01
  0.6   -2. 227071E-02       5.8812886-01
  0.7     1.0051476-01       6.8122226-01
  1.8     4.5681116-01       1.5068176+00
  1.9     4. 4工94036-01      1.557775E+00
  2.0     4. 2298086-01      1.6054136+00
  2. 1    4.006120E-01       1.648699E+00
  2. 2    3. 7607465-01      1. 687625E+00
  3.3     2. 467829E-02      1.848081E+00
  6.3    -1. 988822E-02      1.4181746+00
  6. 4   -4. 工81411E-03      1.419223E+00
  6.6     1.1101526-02       1. 4217946+00
  6.6     2.5823146-02       1.425816E+00
 10.0    -4. 5456446-02      1.668348E+00
 12. 5   -1. 140835E-02      1. 4923376+00
 15.0     4. 627868E-02      1.618194E+00
 E자onential 工ntegral Ei
    21 Values
     0.1 -1. 62281
     0. 2 -0. 821761
     0. 3 -0. 302669
     0. 4  0. 104768
                                    116   N切rieric削Re아）es Examp旭 Book

       0.5      0.454220
       0.6      0. 769881
       0. 7     1.06491
      0.8       1. 34740
      0. 9     1.62281
      2. 2     5. 73261
      2. 4     6. 60067
      3. 5     13. 9254
      3.9      18. 3157
      5. 0     40. 1853
      5.4      54. 1935
      12. 5 23565. 1
      13. 0 37197. 7
      13. 5 58827. 0
      14.0 93193. 0
     14. 5 147866.
     15.0 234955.
    Gamma Function
    17 Values
     1.0        1.000000
     1. 2       0. 918169
     1. 4       0.887264
     1.6        0.893515
     1. 8       0. 931384
     2. 0      1. 000000
     0. 2      4. 590845
     0. 4      2. 218160
     0. 6      1. 489192
    0.8        1.164230
   -0. 2       -5. 821149
   -0. 4       -3. 722981
   -0.6        -3.696933
   -0. 8       -5. 738555
   10. 0       3. 6288000E05
   20. 0       1. 2164510E17
   30.0        8. 8417620E30
   뵤叫factorial
   18 Values




                 0
                     2 3
             l




                           5 05 0
             2




l
             6




    3 4 56 7 8 9 l
             24
             120




                   d l l l i 22 3
            720




                  1
            5040




 d八
            40320
            362880
            3628800




                        44
                  1d
            39916800
            479001600
            6227020800
            87178291200
            1. 3076755E12
            2. 4329042E18
            1. 5511222E25
            2. 6525281E32
  Binomial Coefficients
                                                                                                   （沕킥升er 6: Specia사屯nc加ns   117

20 Values
                                                0                           上
                                                                            4
  l 6




                                               l 口U 戶b l aU 5 7
                                                                            6




     5 5 CV 5 5 LU 尸b LU 尸b 尸b 5 nb :U 5 5 5
                                                                            20
                                                                            6
                                                                            16
                                                                            465
                                                                            3003
                                                                            6436




                                                 l 3
                                                                 11 3 5 7
                                                                            5005
                                                                            1365




 6 6 l l l l d1 d上 l n二 n= ni nd 2 2 2 n{ 2
                                                                            105
                                                                            25
                                                                            2300




                                               9 l 4l l 3 5 m/ 9 l l l l
                                                                            53130
                                                                            480700
                                                                            2042975
                                                                            4467400
                                                                            5200300
                                                                            3268760
                                                                            1081575
Beta Function
15 Values
1. 0   1. 0                                                                 1. 000000
0. 2                                           1. 0                         5. 000000
1. 0                                           0. 2                         5. 000000
0. 4                                           1. 0                         2. 500000
1. 0                                           0. 4                         2. 500000
0.6                                            1. 0                         1. 666667
0. 8                                           1. 0                         1. 260000
6. 0                                           6. 0                         3. 607504E-04
6. 0                                           5.0                          7. 936508E-04
6. 0                                           4.0                          1. 984127E-03
6. 0                                           3.0                          6.952381E-03
6. 0                                           2.0                          0. 2380958-01
7. 0                                           7.0                          8.325008E-05
5. 0                                           5.0                          1. 587302E-03
4. 0                                           4. 0                         7. 142867E-03
3. 0                                           3. 0                         0. 333333E-01
2.0    2. 0     1. 666667E-01
工ncomplete Ga皿ma Function
20 Values
0. 1   3.1622777E-02     0.7420263
0. 1   3. 1622777E-01    0.9119763
0. 1   1. 5811388        0. 9898955
0. 5   7. 0710678E-02    0. 2931279
0. 5                                           7. 0710678E卞01                         0. 7666418
0. 5                                           3. 5365339                             0. 9921661
1. 0                                           0. 1000000                             0.0951626
1. 0                                           1. 0000000                             0.6321206
1. 0                                           5. 0000000                             0.9932621
1. 1                                           1. 0488088E-01                         0. 0757471
1. 1                                           1. 0488088                             0. 6076457
1. 1                                           5. 2440442                             0. 9933425
2. 0                                           1. 4142136E-01                         0. 0091054
2. 0                                           1. 4142136                             0. 4130643
2. 0                                           7. 0710878                             0.9931450
  118      N미nerk冶／尸ec刃es Examp旭 Book

6. 0     2. 4494897      0. 0387318
6. 0     12. 247449      0. 9825937
11. 0    16. 583124      0. 9404267
26. 0    25. 495098      0. 4863866
41. 0    44. 821870      0. 7359709
Error Function
20 Values
0. 0     0.000000
0. 1     0. 1124629
0. 2     0. 2227026
0. 3     0. 3286268
0. 4     0. 4283924
0. 5     0. 5204999
0. 6     0. 6038561
0. 7     0. 6778012
0. 8     0. 7421010
0. 9     0. 7969082
1. 0     0. 8427008
1. 1     0. 8802051
1. 2     0. 9103140
1. 3     0. 9340079
1. 4     0. 9522851
1. 5     0. 9661051
1. 6     0. 9763484
1. 7     0. 9837905
1. 8     0. 9890905
1. 9   0. 9927904
Incomplete Beta Function
20 Values
0. 5   0. 5      0. 01   0.0637686
0. 5     0. 5    0. 10   0. 2048328
0. 5     0. 5    1. 00   1. 0000000
1. 0     0. 5    0. 01   0. 0050126
1. 0     0. 6    0. 10   0. 0613167
1. 0     0. 5    1. 00   1. 0000000
1. 0     1. 0    0. 5    0. 5000000
5. 0     5. 0    0. 5    0. 5000000
10. 0    0. 5    0. 9    0. 1516409
10. 0    6. 0    0. 5    0. 0897827
10. 0    5. 0    1. 0    1. 0000000
10. 0    10. 0   0. 5    0. 5000000
20. 0    5.0     0. 8    0. 4598773
20. 0    10. 0   0. 6    0. 2146816
20. 0    10. 0   0. 8    0. 9507366
20. 0    20. 0   0. 5    0. 5000000
20. 0    20. 0   0. 6    0. 8979414
30. 0    10. 0   0. 7    0. 2241297
30. 0    10. 0   0. 8    0. 7586405
40. 0    20. 0   0. 7    0. 7001783
Bessel Function J0
20 Values
-6. 0  -0. 1775968
-4. 0  -0. 3971498
-3. 0    -0. 2600520
＝그 . 0    0. 2238908
 1. 0     0. 7651976
 0. 0     1. 0000000
                       Ch카升er 6: Special Funct幻ns   119

 1. 0    0. 7651977
 2. 0    0. 2238908
 3. 0   -0. 2600520
 4. 0   -0. 3971498
 5. 0   -0. 1775968
 6. 0    0. 1506453
 7. 0    0. 3000793
 8.0     0. 1716508
 9. 0   -0. 0903336
10. 0   -0. 2459368
11. 0   中0. 1711903
12. 0    0. 0476893
13. 0    0. 2069261
14. 0    0. 1710735
15. 0   竹0. 0142245
Besse:L Function Y0
15 Values
 0.1    -1. 5342387
 1. 0    0. 0882670
 2. 0    0. 51037567
 3.0     0. 37685001
 4.0    -0. 0169407
 5. 0   -0. 3085176
 6.0    -0. 2881947
 7.0    -0. 0269497
 8. 0    0. 2235216
 9. 0    0. 2499367
10. 0    0. 0656712
11. 0   -0. 1688473
12. 0   -0. 2252373
13. 0   -0. 0782079
14. 0    0. 1271926
15. 0    0. 2054743
Bessel Function 31
20 V日．ues
-5. 0    0. 3275791
-4. 0    0. 0660433
-3. 0   -0. 3390590
-2. 0   -0. 5767248
-1. 0   -0. 4400606
 0. 0    0.0000000
 1.0     0. 4400506
 2.0     0. 6767248
 3.0     0. 3390590
 4.0    -0. 0660433
 5. 0   尸0. 3275791
 6. 0   -0. 2766839
 7.0    -0. 0046828
 8.0     0. 2346364
 9.0     0. 2453118
10.0     0. 0434728
11.0    -0. 1767863
12.0    -0. 2234471
13.0    -0. 0703181
14.0     0. 1333752
15.0     0. 2051040
Bessel function Yl
            120                            肋m印ca/ 尸e아殆s Example Book

  15 Values
   0.1   -6. 4589511
   1. 0  -0. 7812128
   2. 0  -0. 1070324
   3. 0    0. 3246744
   4. 0    0.3979257
   5. 0    0.1478631
   6.0   -0. 1750103
   7. 0  -0. 3026672
   8.0   -0. 1580605
   9. 0    0. 1043146
  10. 0    0. 2490154
  11.0     0. 1637055
  12. 0  -0. 0570992
  13. 0  -0 '2100814
  14.0   -0. 1666448
  15. 0    0. 0210736
  Bessel Function in, n>=2
  20 Values




                    0 0 00 0 0 000 0
         1. 0       1. 1490348495-01
         2.0        3. 528340286E-01
         5.0        4. 656511628E-02
         10. 0      2. 546303137E-01
         50. 0     -5. 9712800795-02
         1. 0       2. 497577302E-04




2 2 2 2 2   5 5 5 5 i i l l l 2 2 22 2
         2. 0       7. 039629756E-03
         5.0        2. 611405461E-01
         10. 0     -2. 340615282E-01
         50. 0     -8. 1400247705-02
         1.0        2.630615124E-10




         니＝
         2. 0       2. 515386283E-07
         5. 0       1. 467802647E-03
         10. 0      2. 074861066E-01
         50. 0     -1. 138478491E-01
         1. 0       3. 8735030095-25
         2. 0       3. 918972805E-19
         5.0        2. 770330052E-11
         10. 0      1. 151336925E-05
          50. 0    -1. 167043528E-01
  Bessel Function Yn, n> '2
  20 Values




                              0 0 00 0 0
         1. 0      -1. 650682607
         2.0       -6. 1740810425-01
         5. 0       3. 676628826E-01
          10. 0    -5. 868082460E-03
          50. 0     9. 5793168735-02
         1.0       -2. 604058666E02




          2 2 2 2 2 5 5 5 5 5 l i ll l 2
          2.0      -9. 935989128
          5.0      -4. 5369482255-01
          10. 0     1.3640304775-01
          50. 0    -7. 854841391E戶02
         1.0       -1. 216180143E08
          2.0      -1. 291845422E05
          5.0      -2. 512911010E01
          10. 0    -3. 598141522E-01
          50. 0     5. 7238971825-03
          1.0      -4. 113970315522
                                       C/i邵怡r 6: Special Func切／is   121
  20     2. 0      -4. 081651389E16
  20     5. 0       -5. 933965297E08
 20      10. 0     -1. 597483848E03
 20     50. 0    1.644263395E-02
 Modified Bessel Function 10
 20 Values
 0. 0    1. 0000000
 0. 2    1. 0100250
 0. 4    1. 0404018
 0. 6    1. 0920463
 0. 8    1. 1665149
 1. 0    1. 2660658
 1. 2    1. 3937256
 1. 4    1. 5533951
 1. 6    1.7499807
 1. 8    1. 9895593
 2. 0    2. 2795852
 2. 6    3. 2898391
 3. 0    4. 8807925
 3. 5    7. 3782035
 4. 0    11. 301922
 4. 5    17 .481172
 6. 0    27. 239871
 6. 0    67 . 234406
 8. 0  427. 56411
10. 0  2815. 7167
Modified Bessel Function K0
20 Values
 0. 1    2. 4270690
0. 2    1. 7527038
0. 4    1. 1145291
0. 6    0. 77752208
0. 8    0. 56534710
1. 0    0. 42 102445
1. 2    0. 3185082 1
1. 4    0. 24365506
1. 6    0. 18795475
1. 8    0. 14593140
2. 0    0. 11389387
2. 5    6. 2347553E-02
3. 0    3.47395005-02
3. 5    1. 9598897E-02
4. 0    1. 1159676E-02
4. 6    6. 3998572E-03
5. 0    3. 6910983E-03
6.0     I . 2439943E-03
8. 0   1. 464707 1E-04
10. 0  1 . 7780062E-05
Modified Bessel Function Ii
20 Values
0. 0   0. 00000000
0. 2    0. 10050083
0. 4    0. 20402675
0. 6    0. 3 1370403
0.8     0. 43286480
1. 0    0. 565159 12
1. 2    0.71467794
 122        Nun旭nc削 尸8이pes Examp旭 Bo아（

1. 4   0.88609 197
1.6    1. 0848107
1.8    1. 317 1674
2. 0   1.5906369
2. 5    2. 5167 163
3. 0    3. 9533700
3. 5    6. 2058350
4. 0    9. 7594652
4. 5    15. 389221
5. 0    24. 335643
6.0     61. 341937
8. 0    399. 873 13
10.0    2670. 9883
Modified Bessel Function K1
20 Values
0. 1    9. 8538451
0. 2    4. 7759725
0. 4    2. 1843544
0. 6    1. 3028349
0. 8    0. 86178163
1.0     0. 60190724
1. 2    0. 43459241
1. 4    0. 32083589
1. 6    0. 24063392
1. 8    0. 18262309
 2. 0   0. 13986588
 2. 5   7. 3890816E-02
 3. 0   4. 01564315-02
 3. 5   2. 2239393E小02
 4.0    1. 2483499E-02
 4. 5    7. 0780949E-03
 5. 0    4. 04461345-03
 6. 0    1. 3439197E- 03
 8. 0    1. 5536921E-04
 10. 0   1. 8648773E- 05
 Modified Bessel Function Kn, n>=2
 28 Values
 2       0. 2      49. 512430
 d
 n
         1. 0      1. 6248389
 =
 n
         2. 0      2. 53759755-01
 d
 n
         2. 5      1. 2146021E-01
 i
 n
         3. 0      6. 1510459E-02
 {
 n
         5. 0      5. 30894375-03
 i
 n
         10. 0     2. 1509817E-05
 d
 n
         20. 0     6. 3295437E-10
 <U
 n
         1. 0      7. 101262825
 U
 口
         2. 0      6. 4738539095-01
 니
 a
         5.0       8. 291768415E-03
 U
 닥
         10. 0     2.7252700265-05
 U
 口
            50. 0   3. 72793677E-23
 V
 C
            1. 0    3.609605896502
 U
 <
            2. 0    9. 431049101
 U
 k
 戶
            5. 0    3. 270627371E-02
 5
            10. 0   5. 754184999E-05
 U
 C
            50. 0   4. 36718224E-23

      0 0
 1
 d
            1. 0    1. 807132899508
 l
            2.0     1. 624824040E05
                                                                                   Ch司升er 6: Special Fur兀加ns   123
       10     6. 0    9. 758562829
       10     10. 0   1. 614255300E-03
       10     60. 0   9. 15098819E-23
       20     1. 0    6. 294369369E22
       20     2. 0    5. 770856853E16
       20     6.0     4. 827000521E08
       20     10. 0   1. 787442782E02
       20     50. 0  1.70614838E-21
      Xoditied Bessel Function In, n>=2
      28 Values


i
n{ni
   n
              0. 2   5. 0166876E-03
             1. 0    1 .3574767E-01
              2. 0   6. 8894844E-01




                             0 0 0 0 0 0 0 0 0 0
             2.5     1. 2764661
             3. 0    2. 2452126
             5. 0    17. 505615
             10. 0   2281. 5189




2
     2   3 3 3 3 3 5 5 5 5 5 1
             20. 0   3. 9312786E07
             1. 0    2. 216842492E-02




                               l l l
                                       2 2 2 2 2
             2. 0    2. 127399592E-01
             5. 0    1. 033115017601
             10. 0   1. 758380717E01
             50. 0   2. 67776414E20
             1. 0    2. 714631660E-04
             2. 0    9. 825679323E-03
             5. 0    2. 157974547
             10.0    7 .771882864E02




                                    14
             50. 0   2. 27854831E20




 dn1
   n  =n
             1.0     2. 7529480406-10
             2. 0   3. 016963879E-07
             5.0    4.580044419E-03
             10. 0  2. 189170616E01
             50. 0  1.07159716E20
             1. 0   3. 966835986E-25
             2. 0   4.3106605766-19
             6.0    6. 024239358E-11
             10. 0  1. 250799736E-04
            50. 0   5. 44200840E18
     Le5endre Polynomials
     19 Values
     1      0       1. 0              1. 224745




                                                                             0 0
     10     0       1.0               3. 240370
     20     0       1. 0              4.627693
     1      0       0. 7071067        0. 866025




                                                   0 00 0 0 0 0 0
     10     0       0. 7071067




                                                                     2 2 2
                                      0.373006




                                                                             i l
     20     0       0.7071067        -0. 874140
     1      0       0. 0              0. 000000
     10     0       0.0              -0. 797435
     20     0       0.0               0. 797766
     2      2       0.7071067         0.484123
     10     2       0. 7071067       -0. 204789




                                                                  ni
                                                                   n      in
                                                                 i
     20     2       0.7071067         0.910208
     2      2       0.0               0. 968246
     10     2       0.0               0. 804785
     20     2       0.0              -0. 799872
     10     10      0.7071067         0.042505
     20     10      0. 7071067       -0. 707252
124      Numerical Recipes Example Book

10     10       0.0              1.360172
20     10       0. 0            -0. 853705
Jacobian Elliptic    Function
20 Values
0. 0   0. 1      0. 099833
0.0    0. 2      0. 19867
0. 0   0. 5     0. 47943
0. 0   1. 0     0. 84147
0. 0   2. 0     0. 90930
0. 5   0. 1     0.099751
0. 5   0. 2     0. 19802
0. 5   0. 5     0. 47075
0. 5    1. 0    0. 80300
0. 5    2.0      0. 99466
1. 0    0. 1     0. 099668
1. 0    0. 2     0. 19738
1. 0    0. 5     0. 46212
1. 0    1. 0     0. 76159
1. 0    2. 0     0. 96403
1. 0    4. 0     0. 99933
1. 0   -0. 2    竹0. 19738
1. 0   -0. 5    -0. 46212
1. 0   -1. 0    -0. 76159
1. 0   -2. 0    -0. 96403
 Chapter 7: Random Numbers

               Chapter 7 of Numerical Recipes deals with the generation of random num-
           bers drawn from various distributions. The first four procedures produce
           uniform deviates with a range of 0.0 to 1.0. ranO is a procedure that imple-
           ments the Park and Miller "minimal standard" random number generator.
           rani adds a shuffle to the minimal standard. ran2 obtains deviates by the
           L'Ecuyer long period algorithm plus a shuffle. ran3 is Knuth's portable gen-
           erator, based on a subtractive rather than a congruential method.
                 The transformation method is used to generate some non-uniform distri-
            butions. Resulting from this are routines expdev, which gives exponentially
            distributed deviates, and gasdev for Gaussian deviates. The rejection method
            of producing non-uniform deviates is also discussed, and is used in g키ndev
            (deviate with a gamma function distribution), poidev (deviate with a Poisson
            distribution), and bnldev (deviate with a binomial distribution). For gener-
           ating random sequences of zeros and ones, there are two procedures, irbiti
           and irbit2, both based on the 18 lowest significant bits in the seed iseed,
           but each us加ga 小丹erent recurrence 的 proceed I如m 毗ep to 就ep.
                The "pseudo-DES" (Data Encryption Standard) hashing of 64-bit words
           is carried out by psdes. It is used to generate random deviates by ran4.
           sobseq produces Sobol's quasi-random sequence. The routines vegas and
           miser are used for multidimensional Monte-Carlo integration, with different
           strategies for picking points in n-dimensional space.



     Sample program xran tests each random number generator, ranO to ran3, in
 turn. For each one, it first draws four consecutive random numbers Xj,... ,X4 from
 the generator in question. Then it treats the numbers as coordinates of a point. For
example, it takes (X1, X2) as a point in two dimensions, (X1, X2, X3) as a point
in three dimensions, etc. These points are inside boxes of unit dimension in their
respective n-space. They may, however, be either inside or outside of the unit sphere
in that space. For n = 2,3, 4 we seek the probability that a point is inside the unit
n-sphere. This number is easily calculated theoretically. For n = 2 it is ir/4, for
n = 3 it is 冗/6, and for n = 4 it is 冗2/32. If the random number generator is
                                                                                     not
faulty, the points will fall within the unit n-sphere this fraction of the time, and the
result should become increasingly accurate as the number of points increases. In the
program xran we have taken out a factor of 2" for convenience, and used the random
number generators as a statistical means of determining the value of lr, 4ir/3, and
i2/   2.
                                                                                      l乙D
126         Numerical Recipes Example Book

/s Driver for routines ranO, ranl, ran2, ran3 卞/

#include <stdio . h>
#includa <math. h>
#include 'nr. h"

#defina P1 3. 1416926

static u工isigned long t日otoj [16] ={OxlL, 0工2L, 0工4L,0工8L, 0工10L,0工20L.0工40L,0x80L,
     吐1001.. . 吐200L , 缸4001.. , 缸的OL, 0工1000L,0工2000L 戶x4000L,0工8000나 ;

float fnc (float xl, float x2, float x3, float 工4)
{
        return (float)     sqrt（工1*xl＋工2卞x2＋工3方工3＋工4＋工4) ;
}

void integ(float         (* tunc) (long s) )
{
        long idum= (- 1) ,iy[ 4] ,jpower,k;
        mnt i, j;
        float 工1, x2，工3，工4, yprob[4] ;

        /* Calculates pi statistically using volume of unit n-sphere */
        for (i=1; i<=3; i++) iy[ i] =0;
        printf ( "volume of unit n-sphere, n = 2, 3, 4\n") ;
        printf ( "# points       pi       (4/3) *pi   (1/2)*pin2\n\n") ;
        for (j= 1; j<rls; j++) {
            for (k=twotoj[ j- 1] ;k>'O;k--) {
                 xl=（卓func) (&idu皿）;
                 x2=（卞fu工1c) (kid피n) ;
                 x3=（卞func) (&idu皿）;
                 工4= ( 字f1끄tc) (kidu皿）;
                 if (fnc(xl, x2,0.0,0.0) < 1. 0) ++iy[1] ;
                 if (fnc (xl, x2, x3,0.0) < 1.0) ++iy[2] ;
                 if (fnc (xl, x2, x3, x4) < 1. 0) ++iy[3] ;
             }
             Jpo口er= t日otoj 口］;
             for (i= 1; i<=3; i++)
                 ypr아江i] =(float) t日otoj [i+ 1］牛jy [i] /JPO日er;
             printf ( "/.61d Y.12. 6f /,12. 6f %12. 6f\ n",
                  jpower , yprob [i] , yprob [2] , yprob [3] );
        }
        printf ( "\ nactual 工12. 6f /.12. 6f 工12. 6f\ n",
            P1, 4. 0*PI/ 3 .0, 0. 5*pI*pI) ;
    }

    mllt main(void)
    {
        printf ( "\ nTesting rano: \n") ; integ(rano) ;
        printf ( "\ nTesting ranl: \n") ; integ(ranl) ;
        printf ( "\ nTesting ran2: \n") ; mnteg(ran2) ;
        printf ( "\ nTesting ran3: \n") ; integ(ran3) ;
         return 0;
    }

       Routine expdev generates random numbers drawn from an exponential deviate.
                                                                       the results
    Sample program xexpdev makes ten thousand calls to expdev and bins
                                                       Ch카升ar 7: 尸andom Numbers   127

into 21 bins, the contents of which are tallied in array x [1] Then the sum total of
all bins is taken, since some of the numbers will be too large to have fallen in any of
the bins. The x[i] are scaled to total, and then compared to a similarly normalized
exponential which is called expect.
/s Driver 如r routine 日工pdev 卓／

#include <stdio.h>
Sinclude <math.h>
亦끄iclude '1n工 . h'1

#define NPTS 10000
#define ES 2. 718281828

mllt main(void)
{
    long idum' (1) ;
     jot i, j, tota].r0. x[21] ;
    fl oat a工pact，工工，y, trig (21] ;

    如r (i= 0; i< '20;i++) {
       trig [i] = i/ 20 .0;
       玎i] =0;
    }
    for (i= 1; i<=NPTS; i++) {
        y= expdev (&idust) ;
        如r (j=1; j<'20; j++)
             if ( (y < trig[ j] ) U   (y > trig[ j- 1] )) ++r[ j] ;
    }
    for (i=1; i<=20; i++) total += x[ij;
    printf ( "\ nexponential distribution vith 'hid points\n", NPTS) ;
    printf ( "     interval          observed     expected\n\n") ;
    for (i=1; i<=20; i++) {
        xx= (float) x (i] /total,
        expect=exp(- (trigCi- 1] +trigtifl/ 2.0) ;
        e工pact 中＝ (0. 05小EE/ (EE-1) );
        printf ( "Y.6. 2f X6. 21 %12. 6f %12. 6f \n",
               trigEi- 1J ,trig[ i] ,xx,expect) ;
    }
    return 0;
}

    gasdev generates random numbers from a Gaussian deviate. Example xgasdev
takes ten thousand of these and puts them into 21 bins. For the purpose of binning,
the center of the Gaussian is shifted over by NUVER2=10 bins, to put it in the middle
bin. The remainder of the program simply plots the contents of the bins, to illustrate
that they have the characteristic Gaussian bell-shape. This allows a quick, though
superficial, check of the integrity of the routine.
/* Driver for routine gasdev a!

#include <stdio . h>
*include "ni .h"

*def inc 月 20
Idefine I0VER2 (1/2)
    128       N미verica／尸e아）es Examp旭 Book

#define NPTS 10000
#define ISCAL 400
#deflne LLEN 50

jut main(void)
{
        char 口ord訌LLE甘＋1) ;
         jut i. j ,k, klim, dist[ N+1] ;
        long iduin= (- 13) ;
        fl oat dd, x;

        如r (j= 0; j<＝奸；J++) dist日］=0;
        for (i=1; i<=NPTS; i++) {
            x=0. 25*표*gasdev (kidunL) ;
            j=(int) (x > 0 ? x+0.5 : x-0.5) ;
            if ( (j >= -NOVER2) && (j <= N0VER2) ) ++dist[ j+NOVER2] ;
          1
          printf ( "Normally distributed deviate of 兄6d points\n' , NPTS) ;
          printf ( "Y.5s %los %9s\n". "x' , 'p (x) ' ,"graph: ") ;
          for (j= 0; j<=N; j++) {
              dd=(float) dist [j] /NPTS;
              for (k=1;k<=LLEN; k++) words[k)=' ';
               k1im=(int) (ISCAL*dd) ;
               if (klim > LLEN) klim=LLEN;
               for (k"l; k<=klim;k++) wordsEk] ='* ';
               printf ( "Y.8.4f '/.8.4f ". j/ (0. 2S本N) ,dd) ;
               for (k=1;k<=LLEN; k++) printf ( ' 工c ', words[k] );
               printf ( '\ n") ;
          }
          return 0;
    }

        The next three sample programs, xga皿dev, xpoidev and xbnldev, are identical to
    the I)revious one, but each drives a different random number generator and produces
                                                                                     order
    a different graph. xgamdev drives gaiudev and displays a gamma distribution of
    ia specified by the user. xpoidev   drives poidev  and produces a Poisson distribution
    with mean xm specified by the user. xbnldev drives bnldev and produces a binomial
    小stribution) 出so with spec小ed xiii.
    ／卞 Driver 如r rou七mile g如adev 中／

    #unclude <stdio . h>
    #include "nr. h"

    #define N 20
    #define NPTS 10000
    #def ins ISCAL 200
    #define LLEN 50

    jut main(void)
    {
           char words [LLE丑+1] ;
           long idu皿＝(- 13) ;
            jut i, ia, j, k, klim, dist[ N+1] ;
           float dd;
                                                     Ch카가er 7: 尸andom Numbers            129

    for (; ;) {
          for (j= 0; j<=N; j++) dist[ j] =0;
          do {
               printf ( 'Select order of Gasuna distribution (n=1. .Y.d) . -1 to end\n", N) ;
               sc카lf ( "%d", &ia) ;
          } while (ia > N) ;
          if (ia < 0) break;
          for (i= l; i<=NPTS; i++) {
               j=(int) gamdev (ia, &idum) ;
             if ( (j '= 0) U (j <= N) ) ++djst [j] ;
         }
         printf ( "\ nganuna-distribution deviate, order Y.2d of Y.6d points\n",
             ia, NPTS) ;
         printf ( '%65 Y.7s Y.9s \n", "x ", "p(x) ", "graph: '" ) ;
         for (j 'O; j<N; j++) {
             dd= (float) dist[ j] /NPTS;
             for (k=1;k<=50; k++) words[k] =' .
             klim=(int) (ISCAL*dd) ;
             if (klim > LLEN) kliiu=LLEN;
             for (k=1;k<=k1im;k++) words[k] ' 's ' ;
             printf ( "%6d %8. 4f ", j, dd) ;
             for (k=1;k<=klim;k++) printf ( "V.c ' , words[k] );
             printf ( "\ n") ;
          }
    }
    return 0;
}

/* Driver for routine poidev */

#include <stdio.h>
#include "nr. h"

#detine N 20
#def ins NPTS 10000
#def ins ISCAL 200
#define LLE月 50

mnt main(void)
{
    char txt (LLEN+1] ;
    long idwn=(- 13) ;
    ml1t i, j, k,klim, dist[ N+1] ;
    float xm, dd;

    如r ( ,· .· ) {
         for (j= 0; j<=1; j++) dist[ j] =0;
         do {
              printf ( "Me카l of Poisson distribution (0. 0<x<V.d. 0) ", N) ;
              printf ( "- Negative to end: \n") ;
              sca끄f ( "%f ", k工m) ·，
         } 日hile （工In > N) ;
         if (xni < 0. 0) break;
         for (i=1; i<=NPTS; j++) {
              j = C milt) 他5+1：山idev (x皿，Aidu皿）);
              if ( (j >= 0) U (j <= N) ) ++djst[ jJ;
         }
130       Nume月ca/ 尸a야）es Examp旭 Book

         printf ( "Poi日son-dietributed deviate, mean '/.5. 2f of %6d polnts\n"
             xrn, NPTS) ;
         printf ( "Y.5s Y.as Y.lo日\n", "x", "p(x) ", "graph: ") ;
         for (j= 0; J<=N; j++) {
             dd=(float) dist[ j] /且PTS;
             如r (k=0;k<=LLE甘；k++) t工t [k] =J j ;
             klim= (int) (ISCAL*dd) ;
             if (klim > LLEN) klim=LLEN;
             for (k=1;k<=klim;k++) txt[ k] ='卞 ';
              txt[ LLEN] ='\ O ' ;
              printf ( "%6d %8. 4f       %s\n" 口,dd, txt) ;
          }
      }
      return 0;
)

7* Driver for routine bnldev *7

#include <stdio.h>
#include "nr. h"

#define N 20
#def ins NPTS 1000
#def ins ISCAL 200
#define N뵤 100
#daf ins LLEN 50

mnt rnain(void)
{
      char txt[ LLEN+1] ;
      ml1t i口, k,klim, dist[ N+1] ;
      long idurn=(- 133) ;
      float pp, xm, dd;

      for (; ;) {
          for (j= 0; j<rl; j++) disttj] =0;
          do {
               printf ( "Mean of binomial distribution (0.0 to %d. 0) ", N) ;
               printf ( " - Negative to end: \n") ;
              scanf ( "Y.f ", &지n) ;
          J' while (xrn > 20.0) ;
          if (xm < 0. 0) break;
          pp＝工rn/ N甘；
          for (i=1; i<=NPTS; i++) {
               j=bn1dev (pp, NB ,kidu工) ;
              if (j >= 0 Ak j <= N) ++dist[ j) ;
          }
          printf ( "Binomial-distributed deviate, me시l 工5. 21 of %6d points\n",
              xrn,NPTS) ;
          printf ( "%48 '/.8s 工los\n", "x", "p(x) ", "graph: ") ;
          for (j= 0; j<표; j++) {
              for (k=0;k<=LLEN; k++) txttk] =' 1 ;
              dd=(float) dist[ j] /月PTS;
              k1irn=(int) (ISCALsdd+i) ;
               if (klirn > LIEN) klim=LLEN;
              如r (k=1; k<=k1i工；k++) t工t Ek] =1小J ;
                  txt[ LLEN] ='\ O ' ;
                                                                  Ch카升er 7: 尸andom Numbers   131

                    printf ( "%4d /.9. 4f        加\n", j, dd, txt) ;
               }
          }
          return 0;
     }

      Functions irbiti and irb1t2 both generate random series of ones and zeros.
 The sample programs xirbitl and xirb1t2 for the two are the same, and they check
 that the series have correct statistical properties (or more exactly, that they have at
 least one correct property). They look for a 1 in the series and count how many zeros
 follow it before the next 1 appears. The result is stored as a distribution. There
 should be, for example, a 50% chance of no zeros, a 25% chance of exactly one zero,
 and so on.
     /方 Driver for routine irbitl           小/

 #include <stdio.h)
 #include '1nr.h"

 *define NBIN 16
 #define NTRIES 10000

     m1lt main(void)
 {
          mi1t i, iflg, ipts=O, j, n;
          unsigned long iseed=12346;
          float tvoinv,delay[NBIN+1) ;

          /* Calculate distribut ion of runs of zeros 字/
          for (i=1; i<=NBIN; i++) delay[ij= 0.0;
          printf ( "distribution of runs of n zeros\n") ;
          printf ( "%6s 7.22s %18s\n" , "it", "probability " , " expected") ;
          for (i=1; i<=NTRIES; i++) {
              if (irbit1 (kiseed) == i) {
                    ++ipts;
                    if lg=0;
                    for (j=1; j<=NBIN; j++) {
                         if ( (irbitl (kiseed) == 1) k& (ifig == 0) ) {
                              if1gr1;
                             ++delay[ j) ;
                        }
                   }
               }
          }
          t口oinv=0 .5;
          如r (n=1;n<＝月BI月；n++) {
              printf ( "%Gd 工19. 4f %20. 4f\ n".
                  (n-i) ,delay[n] /ipts, tvoinv) ;
              t日oinv /= 2. 0;
          }
          return 0;
}

I.
         Driver for routine irbit2      */

#include <stdio.h>
    132    Numer乞計F相C肛旭s Exam例0 Book

#include "nr. h "

仁define IBIl 15
作dafine ITRIES 10000

static unsigned long tvoton[16] ={0工1L,0工2L,0工4L,0工8L, 0工i0L.O工20L,OX40L,O工80L,
     0x100L,0工200L,0工400L.0工800L,0工1000L,0工2000L,0工4000L,0工8000L} ;

jut main(void)
{
      jut i, jflg, ipt5=0, j, n;
      unsigned long jseed=111;
      float delay[IBII+1] ;

      /* Calculate distribution of runs of zeros 中1
      for (i= 1;i<=NBII; i++) delay[i) =0.0;
      for (i= 1;i<=NTRIES; i++) {
          if (irbit2 (kiseed) == 1) {
               ++ipts;
               if1g=0;
               for (j=1; j<=IBII; j++) {
                   if ( (irbit2 (kiseed) == 1) U     (iflg   == 0) ) {
                        iflg= 1;
                        ++delay[j] ;
                    }
               }
          }
      }
      printf ( "distribntion of runs of n zeros\n") ;
      printf ( "%65 '1.225 工18s \n" ,"n", "probability ", "e工pected") ;
      for (n=1;n<=NBIN;n++)
          printf ( "I.6d 'I,19.4f 工20. 4f\ n",
                (n-I) ,delay[n] /ipts, 1 .0/（如uble汁日otonti口 ) ;
      return O;
}

    The routine psdes uses the logic of the Data Encryption Standard, though with a
simplified nonlinear function, to fully "hash" both of its 4-byte arguments. Since the
routine assumes that unsi因led long integers are 32 bits, it is not strictly portable.
The following test routine simply verifies that the test values suggested in the main
book are in fact obtained.
/* Driver for routine pades */

*include <stdio.h>
*include "nr. h'1

mllt main(void)
{
      static unsigned long lword[&]={0,1,1,99,99} ;
      static unsigned long irword[5]={0.1.99,1,99} ;
      static char *ans[5]={

          ''0x604d1dce 0工509c0c23",
          "0工d97f8571 0xa68cb41a",
          "0x7822309d 0x64300984",
          "0工d7f 376如 0工59ba69eb"} ;
                                                      Ch叩for 7: 尸an由m Num切rs             133

    jilt i;

    for (j=1; j<=4;i++) {
        psdes(klvord[i] ,kirword[i] );
        printf ( "PSDES now calculates:            0工X工 缸狂＼a" ,lword［口 ,ir日ord[i) );
        printf ( "Known correct answers are:       加＼n", ans[i] );
    }
    return 0;
}

    Once psdes is known to work, then the only trick in making the encryption-
based random number generator ran4 functional is to be sure that its hexadecimal
masking values are compatible with your floating point format. The following program
attempts to reproduce the test values given in the main book. If your computer
produces e洌1er the IEEE values, or the VAX values, then you very likely have things
set up correctly. If not, go back and read the discussion in the main book.
    Note that the test program, in resetting the value idu皿 between calls, forces
ran4 to access certain values (the 1st and 99th) in two different random sequences
(sequence -1 and sequence -99). While this random access is an interesting, and
sometimes useful, property, most uses of ran4 would leave idum unchanged between
calls after a single initializing call with a negative value.
/* Driver for routine r띠l4 a!

#include <stdio . h>
#include "nr. h"

jut wain(void)
{
    mnt i;
    static long idu工[5]={0,-i, 99,-99,99} ;
    static char *ansva工[6] ={' " ,"0. 275898", "0. 208204", "0.034307", "0. 838676"} ;
    static char *ansjee[5] ={' " ,"0. 219120" ,"O .849246" ,"0 .375290", "0.467334"} ;
    float rando三[6] ;

    如r (i=1;i<=4; i++) ran如w [i] =ran4仕idu皿[ j] );
    priutf ( "ran4 gets values: ") ;
    for (i=1; i<=4; j++) printf ( "%1&.6f ", randoa[ j] );
    pr幻itf ( "\ n     IEEE a工5日cr5: " );
    for (i=1; i<=4; j++) printf ( "%155", ansiee[ j) );
    prmutf ( "\ n      VA工 키15日cr5: " );
    for (i=1;i<=4;i++) printf ( "%l5s", ansva工[i] );
    printf ( "\ n") ;
    ret,끄：끄 0;
}

    The routine sobseq returns successive values of a multi-dimensional, quasi-random
Sobol' sequence. The following example shows how the routine is initialized via a neg-
ative argument, and then used to obtain the first 32 values of a 3-dimensional sequence
such as might be used to sample points in a 3-dimensional cube. In this example, we
do nothing with the values other than to print them out. You can check your output
against the following:
    0.50000      0.60000      0.50000       1
    0. 25000     0.75000      0. 25000      2
134        Numerical Recipes Example Book




                                                 3 4 5 6 7 8 9 m n n n m 珏 m n 始 四 加 기 力 羽 m 茹 羽 刃 羽 羽 的 釘 的
    0. 75000       0. 25000      0. 75000
    0. 37500       0. 62500      0. 12500
      0. 87500     0. 12500      0.62500
      0. 12500     0. 37500      0. 37500
      0. 62500     0. 87500      0. 87500
      0. 31250     0. 31250      0. 68750
      0. 81250     0. 81250      0. 18750
      0. 06250     0. 56250      0. 93750
      0. 56250     0. 06260      0. 43750
      0. 18760     0. 93750      0. 56250
      0. 68750     0. 43760      0.06250
      0. 43750     0. 18750      0. 81250
      0. 93750     0. 68750      0. 31250
      0. 46875     0. 84375      0. 40625
      0.96875      0. 34375      0. 90625
      0. 21875     0. 09375      0. 16625
      0. 71875     0. 69376      0. 65625
      0. 09375     0. 46875      0. 28125
      0. 69375     0. 96875      0. 78125
      0. 34375     0. 71875      0. 03125
      0. 84375     0. 21875      0. 53125
      0. 15625     0. 53125      0. 84375
      0. 65625     0. 03126      0. 34375
      0. 40625     0. 28125      0. 59375
      0. 90625     0. 78125      0. 09375
      0. 28125     0. 15625      0. 96875
      0. 78125     0. 65625      0. 46875
      0. 03125     0. 90625      0. 71875
      0. 53125     0. 40625      0. 21875
      0. 26562     0. 60938      0. 57812


/* Driver f or routine sobseq 卞/


#inc끄lcie <stdio. h>
#include "nr. h11
#include "nrutil.    h"


ml1t maixi(void)
{
      jot i, nl= (- 1) ,n2=3;
      fl oat CX;


      x=vector (1 ,n2) ;
      sobs eq ( &n1, x) ;
      tor (isl; i< r32; i++) (
          sobseq(kn2, x) ,
          printf ( " 小0. 5f '/.10. 5f %10. sf V.5d\n ", x[1I. 工[2] ,xE3] ,i) ;
      }
      free_ vector (x, 1,n2) ;
      return 0;
}

   We demlonstrate tile adaptive Monte Carlo integration routine vegas on a nar-
rowly peaked, n- dimensional Gaussian function,
                                   /(!          / 10                                                                               XO) 2
                                   f (x)
                                       )=
                                                                                                                        100
                                                                                                               \
                                                                                                                              (X
                                                                                                                   e.
                                            =
                                                                     Gb카升er 7: 尸andom Numbers   135

The function is normalized so that its integral over all space is unity, for any number
of dimensions n.
   After prompting for a (negative) seed for the random number generator, the
demonstration program prompts for several further quantities: First, the number of
dimensions. Second, a scalar offset x0 which is used to construct the vector x0 as

                                 xo =       (x0,
                                                   xo,   .   .   .
                                                                     ,xo)



Third, the maximum number of evaluations of (calls to) the function that are allowed
on each adaptive iteration. Fourth, the number of adaptive iterations. Fifth, a code
that controls how mlluch information is printed out by vegas. The program calls vegas
twice, first from a "cold start", and then a second time, inheriting the adapted grid
from the first call.
    If the five input parameters are entered as

                               4,        0.0,      1000,             4,     0

the answer for the integral ought to come out (1/2)4 = 0.0625. Why not 1? Because
the offset of 0.0 bisects the Gaussian in each dimension with the boundary of the
region.
     The following is typical of the actual output produced. Notice that, with this
random seed, the first pass gets a very unlucky value at iteration no. 2 (a low value
with an unfortunately small error estimate), and the average of all iterations never
fully recovers. You would know that something is wrong, however, from the large
value (6.1) of the x2 per iteration. That is why you might then do a second pass with
the now-adapted grid. By the end of the 4th iteration on the second pass, you have
a good value, a reliable error estimate, and a credible value for the x2.
 Input parameters for Vegas:   ndi皿＝      4 ncall=        768
                               it=       0 itm工＝     4
                               nprn= 0 ALPH= 1. 50
                               口ds= 1 nd= 50



                                                                                        lll l
                                 xl ( l] =           0 xuC i] =
                                 xl [ 幻＝             0 工U[ 幻＝
                                 xl [ 키＝             0 工U[ 幻＝
                                 xl ( 幻＝             0 工U[ 幻＝
 iteration no.    1 : integral =        0.07706088 +1-        0.076
  all iterations:   integral =      0.
                                      07706086+!-      0.076 chi**2/IT n =   0. 00018
 iteration no.    2 : integral =        0.02334202 +1-      0.0075
  all iterations:   integral =      0.02386367+!-    0.0075 chi**2/IT n =         0. 5
 iteration no.    3 : integral =        0.04258667 +1-      0.0066
  all iterations:   integral =       0 .0343241+!-     0.006 chi**2/IT U =           2
  iteration no.   4 : integral =        0.06005678 +1-      0.0048
  all iterations:   integral =     0.04810574+!-     0.0034 chi**2/IT n =         6.1
lumber of iterations performed: 4
Integral, Standard Dcv. , Chi-sq. =         0.048106     0.003386    6.122937
  Input pa工a工eters 如r Vegas: ndia=         4 ncall=       768
                               it=       6 itax "    4
                               nprn      0 ALPH= 1.50
                               is4s= 1 nd= 50
                                 xl[ 1] "            0 xuC i:i=            l
                                 工1[ 幻＝              0 工U[ 幻＝              1
                                 工1[ 釘＝              0 工U[ 幻＝              1
    136      Numerical Recipes Example Book

                                       工1[ 幻＝              0 xu[ 幻＝                1
    iteration    no.    1 : integral =       0. 06294661 +1-       0.0026
    all iterations:       integral =     0. 06294661+/尸    0. 0026 chi方李2/IT n =              0
    iteration no.       2 : integral =       0. 06291871 +1-        0. 002
    all iterations:       integral =     0.06292916+!-     0.0016 chi* *2/IT n =       0.00016
    iteration no.       3 : integral =       0. 06065986 +1-       0. 0014
    all iterations:       integral =     0. 06163905+/-      0. 001 chi* *2/IT n =        0.68
    iteration no.       4 : integral =       0. 06289233 +1-       0. 0013
    all iterations:       integral =     0. 06214162+!-   0.00081 chiC卞2/I丁 n=            0. 68
Additional iterations       performed : 4
Integral,       Standard Dev. , Chi-sq            0. 062142      0. 000810    0. 576426

／半 Driver 如r routine v日gas */


#include <stdio . h>
#include <math. h>
#include "nr. h"
#include "nrutil.       h"


long idum;             ／卞 如rr띠mo 1/

mnt ndim,              /／卞 如r f工n 卞／
float xoff;


float     fxn(float    ptD, float     wgt)
{
       int j;
       float ans 1sum;


      for (suin=0. 0, j=1; j<=ndim; j++) sum += (100. 0*SQR(ptEj] -xoff) );
      an5= (sum < 80. 0 ? exp(- su皿) : 0. 0) ;
      缸1s *= pow (5. 64189, (double)ndim) ;
      return ans;
}

jut main(void)
{
          mnt init, itmax, j ,ncall, nprn;
          float avgi, chi2a, sd, xoff;
          float *regn;


          regn=vector (1, 20) ;
          printf ( "IDUM=\n ') ;
          scanf ( 'Xld ', &idum) ;
          if (id山n > 0) idu皿 = 小id山n;
          for (; ;) {
                printf ( 'E甘TSR 瓦月DI札工OFF,NCALL,IT겨A瓦NPRN\n ") ;
                if (scanf ( "/.d Xf Y.d 工d Y.d", kndim,kxoff. &ncall,kitma工,knprn) == SOF) break;
                avgi=sd=chi2a=0. 0;
                for (j= 1; j<=ndim; j++) {
                    regn[ j] =0. 0;
                    regn[ j+ndim] =1 .0;
                }
                mnit = -1;
                vegas (re酊l,ndim, fxn, mnit,ncall, itma工,nprn,kavgi, tsd, kchi2a) ;
                printf ( "Number of iterations performed: %d\n ", itmax) ;
                printf ( "Integral,   Standard 0ev. , Chi中eq. = %12. 6f %12. 6f工 12.6f\ n "
                                                    Ch카升er 7: 尸andom NL月nbers           137

               .avgi,sd,chi2a) ;
            mnit = 1;
            vegas(regn,ndim,fxn,init, ncall, itmax.nprn,&avgi,ksd,tchi2a) ;
            printf ( 'Additional iterations performed: %d \n", itma工) ;
            printf ( "Integral. Standa工d Dev. , Chi-sq. = %12. 6f Y.12. 6f% 12.6f\n",
               avgi.ad,chi2a) ;
        }
       frea_vector (regn.1,20) ;
       printf ( "如rma]. collpletion\n") ;
       rets口rn 0;
}

    Our demonstration of miser, the routine for multidimensional Monte Carlo inte-
gration with recursive stratified sampling, performs the same integral repeatedly, so
as to test whether miser's claimed standard deviation in fact corresponds (at lea就
roughly) to the actual spread of its answers around the known correct value. The
function being integrated is the samlle narrow Gaussian as was used for vegas. Now,
however, we assume an offset xo that puts the peak of the Gaussian well into the
region of integration, say x0 = 0.33333.
     The program prompts for the number of points to try in each integration, the
number of dimensions, the value for x0, a dithering parameter which can generally be
set to zero (see discussion in main book), and the number of separate times to repeat
the miser integration. A typical run with the input values

                            10000,     4,   0.333333,   0.0,     5

produces output like this:
    Fractional error: actual,indicated=        0.016751        0.022333

    The first number is the average of the actual errors, comparing miser's output
value to the known answer of 1. The second number is the average of the standard
deviations reported by miser, that is, its indicated ermr. In this example, we see
that they are comparable, as expected, and that our Monte Carlo integration is being
performed (each of five times) with an accuracy of about 2%.
    Of course, in most real uses of miser, it would be better to perform the integration
only once, with five times as many points, rather than five times.
/巾 Driver for routine miser */

#include <itdio. h>
#includ. <math.h>
*includ. "nr . t111
*include "nrutil. h11

如ug idum;        /s 如r ranno */

m1it ndi二;       ／小 如r func */
float xoff;

float func(float ptD)
{
    i.nt j;
    float anc1aum;
    138       Numerical Recipes Example Book


      for (sum=O. 0, j=1; j<=ndim; j++) sum += (iOO. 0*SQR(pt[ j] -xoff) );
      ans= (su皿 < 80. 0 ? exp（尸su皿） : 0. 0) ;
      ans 卞＝ pow (5. 64189, (double)ndim) ;
      return ans;
}

mnt main(void)
{
          unsigned long n;
          ml1t j, nt, ntries;
          float ave, dith, sumav, sumsd, var,*regn;

          printf ( 'IDUM= \n") ;
          scanf ( '%ld ", kjdu皿) ;
          if (idum > 0) idum = -idu皿;
          如r ( ·. ·. ) {
              printf ( " 朗TER 瓦月DIM, XOFF,DIT瓦NTRIES\n") ;
              if (scanf ( "Y.ld Xd /.f 1'.f %d' , kn.kndim,kxotf, kdith, kntries) == EOF) break;
              regn=vector (1,2*ndim) ;
               S山5av=s山nsd=0.0;
              for (nt=l; nt<=ntries;nt++) {
                   for (y1; j<=ndim; j++) {
                        regn[ jJ =0. 0;
                        regn[ndim+ j] =1.0;
                   }
                   ntiser (func,regn,ndim,n,dith, kave, &var) ;
                   s山nav += SQR(ave-1. 0) ;
                   su皿sd += sqrt (fabs (var) );
              }
              sumav=sqrt (sumav/ntries) ;
              s山nsd /= ntries;
              printt ( 'Fractional error: actual,indicate4= %12. 6f7. 12.6f\ n", suinav, sumsd) ;
              free_ vector (regn, 1, 2*ndim) ;
          }
          printf ( ''Norinal completion\n") ;
          return 0;
}
Chapter 8: Sorting

        Chapter 8 of Numerical Recipes covers a variety of sorting tasks including
   sorting arrays into numerical order, preparing an index table for the order of
                                                                         element in
   an array, and preparing a rank table showing the rank order of each
   an array. piksrt sorts a single array by  the straight insertion method. piksr2
   sorts by the same method but makes the corresponding rearrangement of a
   second array as well. shell carries out a Shell sort. sort and sort2 both do
   a quicksort, and they are related in the same way as piksrt and piksr2, that
   is, sort sorts a single array, and sort2 sorts an array while correspondingly
   rearranging a second array. hpsort sorts an array by the heapsort algorithm,
    which is not quite as fast (on average) as quicksort, but requires no auxiliary
   storage.
        indexx indexes an array. That is, it produces a second array that con-
    tains pointers to the elements of the original array in the order of their size.
    sort3 uses indexx and illustrates its value by sorting one array while making
                                                                                table
    corresponding rearrangements in two others, rank produces the rank
    for an array of data. The  rank table is a second  array whose  elements list the
   rank order of the corresponding elements of the original array.
       selectfinds the Ntli largest element in an array (e.g., the median). It
   uses the same partitioning idea as quicksort and is very fast. selip performs
   the same function without disturbing the array, and is correspondingly slower.
   hpsel 月iids the M largest 이ements of an array, without （打就urb加g 兀
       Finally, the routines eclass and eclazz deal with equivalence classes.
   eclass gives the equivalence class of each element in an array based on a list
   of equivalent pairs that it is given as input. eclazz gives the same output
   but bases it on a procedure named equiv (j ,k) that tells whether two array
   elements j and k are in the same equivalence class.



    Routine piksrt sorts an array by straight insertion. Sample program xpiksrt
provides it with a 100-element array from file tarray.dat which is listed in the
Appendix to this chapter. The program prints both the original and the sorted array
for comparison.
/巾 Driver for routine pikart */

#include <atdio.h>
#include <stdlib . h>
井include 1뇨r . l111
卄include '1nruti],.h "


                                                                                    139
         140     Numerical Recipes Example Book


        #define NAXSTR 80
        #define NP 100

        mllt main(void)
        {
             char txt[ MAXST1] ;
             jot i, j;
             float 卞a;
            FILE *fp;

            a=vector (1,NP) ;
            if ( (fp = 如pen( "tarray. dat " , "r ") ) == NULL)
                nrerror ( "Data file tarray. dat not 如山ld\n") ;
           tgets (txt, MAXSTR. ,fp) ;
           for (i=1; i <=NP; i++) fscanf (fp, "%f ", &a[i] );
           fclose(fp) ;
           printf ( "original array: \n") ;
           for (i= 0; i<=9; i++) {
                for (j=1; j<=10; j++) prmntf ( "Y.7. 2f ", a[10*i+ j] );
                printf ( "\ n") ;
           }
           piksrt (NP, a) ;
           printf (노orted array: \n") ;
           for (i= 0; i<=9; i++) {
               for (j=1; j <=10; j++) printf ( "Y.7. 2f ", a[10*i+ jfl;
               printf ( "\ n") ;
           }
           free_ vector (a, 1,NP) ;
           return 0;
    }

     piksr2 sorts an array, and simultaneously rearranges a second array (of the same
size) correspondingly. In program xp1ksr2, the first array a[i] is again taken from
tarray.dat. The second is defined by b[l] =i. In other words, b is originally sorted
and a is not. After a call to piksr2, the situation should be reversed. With a second
call, this time with b as the first argument and a as the second, the two arrays should
be returned to their original form.
/s Driver for routine piksr2 */

#inc끄lde <stdio. h>
#include <stdlib .h>
#include "nr. h"
#include "nrutil. h"

#define NP 100
#define MAXSTR 80

lnt main(void)
{
          char txt[ MAXSTR] ;
          jot j口;
          float *a, *b;
          FII厄 李fP;
                                                                   Ch카升er 8: Sorting   141

    a=vector (1,NP) ;
    b=vector (1,NP) ;
    if ( (fp = fopen( "tarray. dat ", "r ") ) == MULL)
        nrerror ( "Data file tarray. dat not found\n") ;
    fgets (txt ,MAXSTR, fp) ;
    for (i '1; i<=MP; i++) fscanf (fp. "/.f ", ka[i] );
    fclose(fp) ;
    /+ gen日rate卜array */
    如r (i=1; i<＝恥느 j++) b［幻＝1;
    ／中 sort a and mix b 中／
    piksr2 (甘P, a,b) ;
    printf ( "\ nAfter sorting a 띠ld mixing b, array a is: \n") ;
    for (i= 0; i<=9; i++) {
        for (j=1; j<=10; j++) printf ( ' 工7. 2f ", a[10*i+ j] );
        printf ( "\ n") ;
    }
    printf ( "\ n. . . and array b is: \n") ;
    for (i= 0; i<=9; i++) {
        for (j=1; j<=10; j++) printf ( "%7. 2f ", b[ 10*i+ j] );
        printf ( "\ n") ;
    }
    print! ( "press return to continue . . .\n " ) ;
    (void) getcharO;
    /+ sort b a工ld mi工 a */
    piksr2(NP,b,a) ;
    printf ( "\ nkftar sorting band mixing a, array a is: \n") ;
    for (i=0; i<=9; i++) {
        for (j= 1; j<'10; j++) print! ( " 工7. 2f ", a(10*i+ j] );
        printf ( "\ n") ;
    }
    printf ( "\ n. . . .and array b is: \n") ;
    for (i=0; i <=9; i++) {
        for (j=1; j<=10; j++) print! ( "%7.2!", b[10*i+ j] );
        print! ( "\ n") ;
    }
    !ree_ vector (b, 1,11?);
    !ree_ vector (a, 1,NP) ;
    return 0;
}

    Procedure shell does a Shell sort of a data array. The calling format is identical
to that of piksrt, and so we use the same sample program, now called xshell.
／卞 Driver 如r routine shell 卞／

#include <stdio.h>
Uinclude <stdlib. h>
#include "nr. h"
#include "nrutil. h"

#de!ine flAXSTft 80
#define NP 100

mnt main(void)
{
    cha工 t工t [MAXSTR] ;
    unsigned long i, j;
    142    Nume月ca／尸ec徊es Example Book

      float Ca;
      FILE *fp;

      a=vector (1,NP) ;
      if  ( (fp = fopen( 'tarray. dat ' , 'r ") ) == NULL)
           nrerror ( "Data file tarray. dat not fo山id\n ') ;
      fgets (txt , MAXSTR, fp) ;
      for (i=1; i<=NP; i++) fsc카lf (fp, ' 工f ' ,ka[i] );
      fclose(fp) ;
      printf ( "\ noriginal array: \n") ;
      for (i= 0; i<=9; i++) {
           for (j=1; j<=10; j++) printf ( "%7. 2f ", atlo* i+ j] );
           printf ( "\ n") ;
      }
      shell (NP, a) ;
      printf ( "\ nSorted array: \n") ;
      for (i= 0; i<=9; i++) {
           for (j=1; j<=10; j++) printf ( "%7. 2f ", a[10*i+ j] );
           printf ( ''\ n") ;
      }
      free_ vector (a, 1, NP) ;
      return 0;
}

    By the same token, routines sort and sort2 employ the same programs as rou-
tines piksrt and piksr2, respectively. (Here they are called xsort and xsort2.)
Both routines use the quicksort algorithm, sort, however, works on a single array.
sort2 sorts one array while making corresponding rearrangements to a second.
／卞 Driver 如r routine sort 中／/

#includo <stdio.h>
#include <stdlib. h>
#inclucle "nr. h1'
#include "nrutil. h"

#def ins MAXSTR 80
#define NP 100

milt nain(void)
1
      cha工 t工t江MAX S Ta] ;
      mnt i, j;
      float 中a;
      FILE *fp;

      a=vector (11 NP) ;
      if  ( (fp = fopen( "tarray. dat ', "r ') ) == NULL)
           nrerror ( "Data file tarray.dat not fou끄d\n') ;
      fgets(txt , MAXSTR, fp) ;
      for (i=1; i<=NP; i++) fscanf (fp, "%f ", &a[i] );
      fcloae(fp) ;
      printf ( "\ noriginal a工ray: \n") ;
      for (i= 0; i<=9; i++) {
            for (j= 1; j<=10; j++) printf ( ' 工7. 2f ", a[10*i+ j] );
           priatf ( "\ n") ;
      }
                                                                   Ch카升or 8: So川ng   143

    sort ( NP , a) ;
    printf ('\ nsorted array: \n ') ;
    for (i=0; i<=9; i++) {
        for (j=1; j<=10; j++) printf ( '%7. 2f ", a[10*i+ j:I) ;
        printf ( '\ n") ;
    ｝·
    free_vector (a, 1, NP) ;
    return 0;
}

/* Driver for routine sort2 */

#inciude <stdio . h>
井include <stdlib.h>
#include 'nr. h1'
#include "nrutil. h'1

#def ins MAXSTR 80
#define NP 100

mnt main(void)
{
    cha工 t工t [MAISTE] ;
    jot j口;
    float; 方a, 卞b;
    FILE *fp;

    a'vector (l ,NP) ;
    b=vector (1,NP) ;
    if ( (fp = fopen( "tarray.dat ", "r ') ) == NULL)
        nrerror ( "Data file tarray.dat not 如und\n ') ;
    fgets(txt, MAXSTR, fp) ;
    for (i=1; i<=NP; i++) fscanf (fp, "/.f ", kaEi] );
    fclose(fp) ;
    /s generate b-ai-ray */
    for (i=i; i<=NP; i++) b[i] =i;
    /5 sort a and mix b */
    sort2(NP,a,b) ;
    printf ( "\ nAfter sorting a and mixing b, array a i8: \n" );
    for (i=0; i<=9; i++) (
        for (j=1; j<'10; j++) printf ( "%7. 2f ", a(10*i+ j] );
        printf ( "\ n") ;
    }
    printf ('\ n. . . and array b is: \n") ;
    for (i '0; i< '9; j++) {
        for (j=1; j<=10; j++) priutf ( "/.7. 2f ' , b[10巾i+j工匕
        printf ( "\ n") ;
    }
    printf ( "press retu口l to continue. . .\n") ;
    (void) getcharO;
    ／卞 sort b and mix a 中／
    sort2(朴,b,a) ;
    printf ( "\ nAfter sorting band mixing a, array a i8: \n" );
    for (i=0; i<=9;i++) {
        for (j=1; j<=i0; j++) printf ( "%7.2f ", a[lo卞i+j] );
        printf ( '\ n") ;
    }
144        肌imerica／尸a加es Examp旭Book

    printf ( "\ n. . . and array b is: \n") ;
    for (i= 0; j<,9; j++) {
        for (j=1; j<=10; j++) printf ( "/.7.2f ", b[ lO杜+ j] );
        printf ( "\ n") ;
    }
    free._vector (b,1,NP) ;
    free_vector(a, I ,NP) ;
    return 0;
}

    hpsort sorts an array by the heapsort algorithm. Its calling sequence is exactly
like that of piksrt and sort, so we again rely on the same sample program, now
called xhpsort.
/* Driver for routine hpsort */

#include <stdio.h>
#include <stdlib . h>
*include "nr. h"
#include "nrutil. h "

#define 甘A工S丁8 80
#define NP 100

ml1t main(void)
{
      char txt[ MAXSTR] ;
      jut i, j;
      float; 方a;
      FILE 卞fp;

      a=vector (1,NP) ;
      if ( (fp = fopen( "tarray. dat", "r ") ) == N口LL)
          nrerror ( "Data file tarray. dat not found\n") ;
      fgets(t工t，甘A工STR, fp) ;
      for (i=1; i<=NP; i++) fecanf (fp, "%f ", ka[i] );
      fclose(fp) ;
      printf ( "\ noriginal a工ray: \n") ;
      for (i= 0;i<'9; i++) {
           for (j=1; j<=10; j++) printf ( "%7.2f ", a[10*i+ j] );
          printf ( "\ n") ;
      }
      hpsort (NP,a) ;
      printf ( "\ nsorted array: \n") ;
      for (i= 0;i<=9; i++) {
          for (j "l; j<=lO; j++) printf ( "%7.2f ", aClo*i+ j) );
          printf ( "\ n") ;
      }
      f ree_vector (a, 1,NP) ;
      ret,玎U 0;
}

    The procedure indeix generates the index array for a given input array. The
index array indx[ j] gives, for each j, the index of the element of the input array
which will assume position j if the array is sorted. That is, for an input array a,
the sorted version of a will be a[indx[ j] ]. To demonstrate this, sample program
                                                             Ch카拍9f 8: Sort加g     145

xindexx produces an index for the array in tarray.dat. It then prints the array in
the order atindx口끄, j=1, . . ,100 for inspection.
/* Driver f or routine ml1dcx工 */

*include <stdio . h>
#include <stdlib. h>
亦include "nr.h"
#include "nrutil. h"

#define NP 100
#define NAXSTR 80

mllt main(void)
{
    char t工t [MA工STE] ;
    unsi肛ed long i, j, 卞mnd工；
    float Ca;
    FILE *fp;

    mlld工＝lvector (1,甘p) ;
    a=vector (1,甘P) ;
    if ( (fp = 如pen( "tarray.dat ", "r ") ) == NULL)
         nrerror ( 'Data file tarray.dat not found\n") ;
    fgets(txt ,MAXSTR, fp) ;
    for (i=1;i<=NP;i++) fscanf (fp, "%f ", ka[i] );
    fclose(fp) ;
    mndcxx佃已키 md工）;
    prmntf ( "\ noriginal array: \n") ;
    for (i=0; i<=9;i++) {
         for (j=1; j<=10; j++) prmntf ( "%7.2f ", a[lO*i+ j] );
         printf ( "\ n") ;
    }
    printf ( "\ nsorted array: \n") ;
    for (i=0; i<=9;i++) {
         如r (j '1; j<=10; j++) printf ( "工7. 2f ", a[indxtlO杜幻끄）;
         printf ( "\ n ') ;
    }
    f ree_vector (a , 1, NP) ;
    free_lvector (indx,1,NP) ;
    return 0;
}

     One use for indexx is the management of more than two arrays. sort3, for exam-
pie, sorts one array while making corresponding reorderings of two other arrays. In
sample program xsort3, the first array is taken as the first 64 elements of tarray .dat
(see Appendix). The second and third arrays are taken to be the numbers 1 to 64
in forward order and reverse order, respectively. When the first array is ordered, the
second and third are scrambled, but scrambled in exactly the same way. To prove
this, a text message is assigned to a character array. Then the letters are scrambled
according to the order of numbers found in the rearranged second array. . They are
subsequently unscrambled according to the order of numbers found in the rearranged
third array. If sort3 works properly, this ought to leave the message reading in the
reverse order.
    146       Numerical Recipes Example Book

/卞 Driver for routine sort3 布/

#include <stdio . h>
#include <stdlib . h>
#include <string. h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

#define NLE奸 64

mnt main(void)
{
      mnt i, j;
      char dummy ENLEN] ,ainsg[NLEN+1] ,bmsg[NLEN+1] ,cmsgtNLEN+1) ;
      float; 卞a, 牛b, 方C;
      FILE *fp;

      a 'vector (1,NLEN) ;
      b=vector (1,NLEN) ;
      c=vector (1,NLEN) ;
      (void) strcpy (amsg, "I 'd rather have a bottle in front of ") ;
      (void) strcat (alnsg, " me than a frontal lobotomy, ") ;
      printf ( "\ noriginal message: \n加\n ', a皿sg) ;
      ／衣 read array of r카ldom nu皿bers +/
      if ( (fp = fopen( "tarray. dat ", "r ") ) == NULL)
          nrerror ( "Data file tarray.dat not fou끄d\n") ;
      fgets (dwnmy , 甘LE瓦 fp) ;
      如r (i=1; i<＝표LE甘；i++) fscanf (fp, "加" ,ka[i] );
          fclose(fp) ;
          /李 create array b and array c 京／
          for (i=1;i<=NLEN; i++) {
              t江i] =i;
              C［幻 =NLE月＋l尸1,
          }
      ／卞 sort a工ray a 口hile mi工ing b and c 方／
      sort3（奸LE且 , a,b, c) ．·
      /卞 scramble message according to array b */
      bmsgENLEN] =axnsg[NLE甘] , /* null terminating character 卓/
      for (i=1; i<＝丑LEN; i++) {
          J=b［幻 ;
          binsg[i- 1] =amsgEj-1] ;
      }
      printf ( "\ nscra皿bled mesaage: \n%s\n", bm月g) ;
      /牛 unscramble according to array c */
      cmsg 대LE비 =a皿S訌吼EN] ;
      for (i 'i; i<＝月LE片; i++) {
           j=c[i] ;
          crnsg[ j- 1] =bmsg[i- 1] ;
          }
      printf ( "\ ninirrored message: \n%s\n", cmeg) ;
      free_ vector (c, 1,月LEN) ;
      free_ vector (b,1,NLE甘) ;
      free_ vector (a,1,NLEN) ;
      return 0;
}
                                                                    Cii짜升er8: Sort加g   147
     rank is a procedure that is similar to indexx. Instead of producing an
                                                                                 indexing
 array, though, it produces a rank table. For an array a[ j] and rank table ira끄k[ j] ,
entry j in irank will tell what index a[ j] will have if a is sorted. irank actually takes
its input information not from the array itself, but from the index array produced by
 indexx. Sample program xrank begins with the array from tarray .dat, and feeds
it to indexx and rank. The table of ranks produced is listed. To check it, the array
a is copied into an array b in the rank order suggested by irank. b should then be
in proper order.
／本 Driver for routine ra끄노 中／

*inc].ude <stdio . h>
#include <atdlib . h>
#include "nr.h'1
#include '1nrutil . h'1

#define NP 100
#define MAXSTR 80

mllt main(void)
{
    char txt [MAXSTR] ;
    U끄sign酊I long i, j, k,l, 中mndx，中ir리lk;
    fl oat *a,b[111;
    FILE *fp;

      indx=lvector (1,NP) ;
      irank=ivector (1,NP) ;
      a=vector (1, 甘P) ;
     if ( (fp = fopen( "tarray.dat ", "r ") ) == NULL)
           nrerror ( "Oati file tarray.dat not found\n") ;
     fgets (txt, MAXsTR, fp) ;
     for (i=1; i<=甘P; i++) fsca끄f (fp, "Y.f ", ka[iJ) ;
     fclose(fp) ;
     mlldc工工 (NP, a, ind工）;
     rank (NP,indx, irank) ;
    printf ( "origmnal array is: \n") ;
     for (i=0; i<'9; i++) .(
           for (j=1; j<=10; j++) printf ( "%7.2f ", a[10*i+ j] );
          printf ( "\ n") ;
     }
    printf ( "table of ranks is: \n") ;
     for (i=0;i< '9;i++) {
           for (3=1; j<=10; j++) printf ( "%7d", irank[10*i+j] );
          printf ( "\ n") ;
    :J
    printf ( "press return to continue. ..\n " ) ;
     (void) getcharO;
    printf ( "array sorted according to rank table: \n") ;
    for (i "0;i<=9; i++) {
          for (j=1; j< 'lO; j++) {
               k=10*i+ j;
               for (l=1;l<=NP;l++)
                    if (iranktl] 二＝ k) b[ j] =a[l] ;
          }
          for (j=1; j<=10; j++) printf ( "%7.2f ", bCj] );
148        Num針元a사？ec徊es Example Book

          printf ( "\ n") ;
      }
       tree_ vector (a, 1,NP) ;
      free.lvector (ir缸lk, 1,NP) ;
      free_lvector (indx, 1,NP) ;
    return 0;
}
                                                                             largest
    Sample program xselect demonstrates the use of select to find the kth
element in tarray .dat. As a cross-check, the answer is compared with that from the
slower routine selip.
/* Driver for routine select */

#include <stdio . h>
#include <stdlib . h>
#include "nr. h"
#include "nrutil. h"

#define MAXSTR 80
#define NP 100

m1lt main(void)
{
      char txt [NAXSTR] ;
      unsigned long i, k;
      float *a, *b,q, s;
      FILE *fp;

      a=vector (i ,NP) ;
      b=vector (1,NP) ;
      if ( (fp = fopen( "tarray. dat ", "r ") ) == NULL)
          nrerror ( "Data file tarray.dat not found\n") ;
      fgets (txt, MAXSTR, fp) ;
      for (i=1; i<=NP; i++) fscanf (fp, 吃f ", la[ i] );
      fclose(fp) ;
      for C; ;) {
          printf ( "Input k\n") ;
          if (sca虹( "%lu ", &k) == EOF) break;
          for (i=1; i<=NP; i++) b[i] =a[i] ;
           s=selip (k, NP, a) ;
           q=se1ect (k, NP,b) ;
           printf ( "Element in sort position Y.lu is %6. 2f\ n", k, q) ;
           printf ("Cross-check from SELl? routine %6. 2f\ n", s) ;
       }
       fr日e_vector (b, I , 卄P) ;
       free_ vector (a, 1,1?);
       printf ( "Normal completion\n") ;
       return 0;
}

    The routine xselip tests selip by selecting the kth largest element of tar-
ray. dat, for each k = 1, . . . , 100. This is a very inefficient way of sorting the array.
As a final check, xselip prints out a user-supplied request for the kth largest element
of the array.
                                                                    Ch따가er 8: Sort幻g   149

1卞 Driver for routine selip *1

#include <stdio. h>
#include <atdlib. h>
#include 'nr. h'1
#include "nrutil. h"

*define MA工STR 80
*define NP 100

mnt main(void)
{
    char txt[ MAXSTR] ;
    unsigned Long i, j, k;
    fl oat 中a！中b,q;
    FILE *fp;

    a=vector (1,NP) ;
    b=vector (11NP) ;
    it ( (fp = fopen( "tarray. dat " , "r ") ) == NULL)
        nrerror ( "Data tile tarray. dat not found\n") ;
    fgets (txt, MAXSTR, fp) ;
    for (i=1; i<=恥）,i+ +) fsc카lt (fp, 'Y.f ", ka[i] );
    fclose (fp) ;
    printf ( '\ noriginal array: \n") ;
    for (i= 0; i<=9; i++) {
        for (3=1; j<=10; j++) printf ( "h7. 2f ', a[10*i+ j] );
        printt ( "\ n") ;
    }
    for (i=1; i<=NP; i++) b[il= aelip(i, 100, a) ;
    printt ( '\ nsorted array: \n") ,
    for (i= 0; i<=9; i++) {
        for (j= 1; j<=10; j++) prmntf ( "Y.7.2f ' , b[10*i+ j] );
        printf ( '\ n") ;
    }
    for (, ;) {
        printf ( "Input k\n' ) ;
        if (scanf ( 'V.lu ' ,kk) == EOP) break;
        qrselip (k, NP, a) ;
        printf ( 'Element in sort position Xlu is V.6. 2f\ n' , k, q) ;
    }
    free_ vector (b. 1.NP) ;
    free卞V日ct or (a1 l . NP) ;
    prmntf ( 'Horisal completion\n") ;
    return 0;
}


sh煮出熬忿然瓷瓷'隘押：:",,"of,,
                  array.
                      an, 뿌 ，峀出畔｝
                                ,"cy),,hcumk
like that for select, except that all k largest elements (not just the 丸th) are printed
out.
/s Driver for routine hpsel *1

#include <stdio . h>
#include <stdlib. h>
#include "nr. h"
 150    Numerical Re가es Example Book

*include "nrutil. h"

#define XAISTR 80
*define NP 100

mlt main(void)
{
    char txt[ MAISTR] ;
    unsigned long i, k;
    float *a,*heap, check;
    FILE *fp;

    a'vector (l, 甘P) ;
    heap=vector (1,NP) ;
    if ( (fp = fopen( "tarray.dat", "r ") ) == NULL)
        nrerror ( "Data file tarray.dat not found\n") ;
    fgets(txt ,MAXSTR, fp) ;
    for (i=1; i<=NP; i++) fscanf (fp, "工f ", kaCi] );
    fcloae(fp) ;
    如r (; ; ) {
        printf ( "Tnput k\n") ;
        if (sc카if ( "%lu ", &k) == EOF) break;
        hpsel(k,NP, a,heap) ;
         check=select (NP+1-노, NP, a) ;
        printf ( "heap[l] . check= 工6. 2f 艾6. 2f\n", h.apti) ,check) ;
        printf ( "heap of numbers of size %lu\u", k) ;
        for (i=1; i<=k;i++) printf ( "工lu      工6. 2f\n" 山heap(i] );
    )
    free_vector (heap. 1,NP) ;
    frea_vector (a,1,JP) ;
    printf ( "Normal completion\n") ;
    return 0;
}

    Procedure eclass generates a list of equivalence classes for the elements of an
input array, based on the arrays lista[ j] and listb[ j] which list equivalent pairs
for each j. In sample program zeclass, these lists are
                        lista:       1, 1, 5, 2, 6, 2, 7, 11, 3, 4, 12
                        list小 :      5, 9, 13, 6, 10, 14, 3, 7, 15, 8, 4

According to these lists, I is equivalent to 5, 1 is equivalent to 9, etc. If you work it
out, you will find the following classes:
                                  classi:        1,5,9, 13
                                  c1ass2:        2, 6, 10, 14
                                  class3:        3, 7, 11, 15
                                  c1ass4:       由8, 12

The sample program prints out the classes and ought to agree with this list.
/* Driver for routine eclass 中/

$include <stdio .h>
#include "nr.h"
#include "nrutil. h"
                                                                   Ch햐升or 8: Sort加g   151

    #define N 11
    #define N 15

    jut main(void)
    {
         jut i, j ,k, ].clas=O,nclass,*nf, *nflag, *nsav;
         static jut lista口={O,1, 1,5,2,6, 2,7,11,3.4,12} ,
                 1istb口={0,6.9,13,6, 10,14,3,7,15, 8,4} ;

        nf=ivector (1,N) ;
        nflag=ivector (1,N) ;
        nsavrivector (1,N) ;
        eclass (nf, 瓦lista, listb, M) ;
        for (i 'l; i<=N; i++) nflag[ i] =1;
        printf ( "\ nNu皿bers from 1-74 divided according to\ n", N) ;
        printf ( "their value modulo 4: \n\ n' ') ;
        for (i=1; i <=N; i++) {
            nclass=nf[ i]
            if (nflag[ nclass) ) {
                  nflag[ nclass] =0;
                  lclas++;
                  k=O;
                  for (j= i; j (=N; j++)
                       if (nf[ j] == nf[ il) nsav[++k] =j;
                  printf ( "Class /.2d:      ", lclas) ;
                  for (j=1; j<=k; j++) printf ( "Y.3d ', nsav[ j] );
                  printf ( '\ n") ;
             }
        )
        free_ ivector (nsav, 1,N) ;
        free_ivector (nf lag, 1,N) ;
        free_ivector (nf, 1,N) ;
        return 0;
}

    eclazz performs the same analysis but figures the equivalences from a boolean
function equiv(i, 刃 that tells whether i and j are in the same equivalence
                                                                            class.
In xeclazz, equiv is defined as true if (i 工 4) and (j % 4) are the same. It is
otherwise false.
/* Driver for routine ecla工z 中1

#include <stdio.h>
#include "nr. h"
#include "nrutil .}i"

#define 甘 15

mnt equiv (mnt i, int j)
{
    return Ci X 4) == (j % 4) ;
}

 jut 皿ain(void)
{
     jut i, j ,k, ].clas=O,nclass, snf, *nflag, *nsav;
152       Numerica/ 尸ec徊es Exa／까,le Book


    nf=ivector (1,N) ;
    of ].ag=ivector ( 1, N) ;
    nsav=ivector (1,N) ;
    eclazz (nf ,N , equiv) ;
    for (i=1; iZ=N; i++) nflag[ i] =1;
    printf ( "\ nNunlber8 from 1-Y.d divided according to\ n", N) ;
    printf ( 'their value modulo 4: \n") ;
      for (irl; i<=N; i++) {
          nclass=nf Li]
          if (nflag[ nclass] ) {
               nflag[ nclass] =0;
               lclas++;
               k=0;
               for (j= i; j<=N; j++)
                   if (of Li] == of Li] ) asav [++k] =J ;
               printf ( 'Class Y.2d:      ", lclas) ;
               for (j= 1; j <=k; j++) printf ( "%3d", nsavEj] );
               printf ( "\ n' ') ;
          }
      I
      free_ ivector (nsav,1,N) ;
      free_ ivector (nflag, 1,N) ;
      free_ ivector (nf , 1,N) ;
      return 0;
I

                                             Appendix

File tarray. dat:

Test data for chapter 8:
  29. 82 71. 51 3. 30 87. 44 53. 42 63. 16 89. 10 26. 75 93. 16 27. 72
  71. 68 48. 34 53. 11 18. 34 27. 13 60. 31 83. 34 22. 81 66. 84 52. 91
  53. 42 15. 22 8. 01 53. 39 76. 12 79. 09 67. 61 38. 39 24. 81 73. 21
  13. 42 62. 10 34. 86 99. 83 38. 46 81. 59 61. 75 79. 62 93. 39 3. 21
  99. 34 92. 22 94. 29 7.03 6. 67 89. 35 83. 14 9. 01 12. 68 62. 22
   2. 95 85. 02 95. 82 73. 96 49. 29 77. 72 36. 65 3. 48 48. 98 71. 83
   1. 41 9. 48 32. 37 89. 95 28. 39 79. 36 54. 05 46. 08 11. 67 37. 78
  77. 17 74. 33 10. 13 4.62 49. 95 68. 40 19. 40 34. 06 4. 11 98. 40
  42. 44 64. 14 89. 41 52. 99 71. 79 3.94 19. 73 44. 91 71. 44 59. 10
  27. 54 15. 67 67. 95 55. 61 26. 05 25. 01 82. 09 89. 67 57. 08 38. 27
 Chapter 9: Root Finding and Sets of Equations

         Chaj元er 9 of Numerical Rec加es deals primari加 w凡h the pr아寸em of 月nd-
    ing roots to equations, and treats the problem in greatest detail in one dimen-
     sion. We begin with a general-purpose routine called scrsho that produces
     a crude graph of a given function on a specified interval. It is used for low-
    resolution plotting to investigate the properties of the function. With this in
    hand, we add bracketing routines zbrac and zbrak. The first of these takes a
    function and an interval, and expands the mnt erval geometrically until it brack-
    ets a root. The second breaks the interval into N subintervals of equal size.
    It then reports any intervals that contain at lea毗 one root. Once bracketed,
    roots can be found by a number of other routines. rtbis finds such roots
    by bisection. rtflsp and rtsec use the method of false position and the
    secant method, respectively. zriddr implements Ridders' method. zbrent
    uses a combination of methods to give assured and relatively efficient con ver-
    gence. rtnewt implemen拓 the 스／e毗on侃叩加on root 月ndii꽁 method, 毗tile
    rtsafe combines it with bisection to correct for its risky global convergence
    properties.
        For finding the roots of polynomials, laguer is handy, and when combined
    with its driver zroots it can find all roots of a polynomial having complex
    coefficients. An alternative to laguer is provided by zrhqr, which finds the
    roots as eigenvalues of the companion matrix. When you have some tentative
    complex roots of a real polynomial, they can be polished by qroot, which
    employs Bairstow's method.
        In multiple dimensions, root-finding requires some foresight. However, if
    you can identi和 thene뇽汕orhood 可a ro야 of a 那tern 可nonlinear equations,
    then mnewt will help you to zero in using Newt on-Raphson. More powerful is
    to use 比明lo比枷 convergent mu九i-dimen加nalNe毗on met加d 加 newt, or
    Broyden 's method broydn, which generalizes the secant method.



    scraho is a primitive graphing routine that will print graphs on virtually any
terminal or printer. Sample program xscrsho demonstrates it by graphing the zer口
order Bessel function J0.
／卞 Driver 如r routine scrsho 京／

finclude <etdio .h>
卞include 1뇨r.h"

static float fx (f] .oat x)



                                                                                  153
    154        Numerical Recipes Example Book

{
      return bessjO(x) ;
}

m1lt main(void)
{
      scrsho (fx) ;
      ret, 心n 0;
}

    zbrac is a root-bracketing routine that works by expanding the range of an in-
terval geometrical!y until it brackets a root. Sample program xzbrac applies it to
the Bessel function J。 . It starts with the ten intervals (1.0, 2.0), (2.0, 3.0), etc.,
and expands each until it contains a root. Then it prints the interval limits, and
the function J。evaluated at these limits. The two values of J0 should have opposite
引gi始1

/s Driver for routine zbrac 卞/


#include <stdio. h>
#include 1'nr. h'1

static       float    fx (float   x)
{
      return bessjo (x) ;
}

mllt main(void)
{
          mllt succes,i;
          float 工1 工2;


      printf ( "Y.21s Y.23s\n" ,"bracketing values: ' , "fu끄ction values: ") ;
      printf ( "%6s 工10s V.21s Y.12s\n' , 'x1 " ,"x2' , "beesj0(x1) ', 'bessj0(x2) ") ;
      for (i= 1; i< '10; i++) 'C
           工1 =i;
          工2＝工1+1.0;
           succes=zbrac (f工 . k工1, k工2) ;
           if (succes) 'C
                     printf ( "%7. 2f 工10. 2f %6s %12. 6f Y.12. 6f \n,'.
                         工1 工2, " " 1f工（工1) ,fx （工2) ) ;
              )
      }
      return 0;
}

    zbrak is much like zbrac except that it takes an interval and subdivides it into
N equal parts. It then identifies any of the subintervals that contain roots. Sample
program xzbrak looks for roots of Jo(x) between Xl = 1.0 and X2 = 50.0 by allowing
zbrak to divide the interval into N = 100 parts. If there are no roots spaced closer
than 스 x = 0.49, then it will find brackets for all roots in this region. The limits of
bracketing intervals, as well as function values at these limits, are printed, and again
the function values at the end of each interval ought to be of opposite sign. There
are 16 roots of Jo between 1 and 50.
                                         Ch킥升er 9: 尸0아Find加g and S이so／日恥石力ons                  155
    /* Driver for routine zbrak */

    #include <stdio.h>
    #include "nr. h"
    #include "nrutil. h"

#define N 100
#def in日 NBNAX 20
幷define Xl 1. 0
仁define 工2 60. 0

    static float fx (float x)
    {
        return bessj0(x) ;
)

mllt main(void)
{
         mnt i, nb＝甘B甘AX;
         float; 中工bl, 卞工b2;

         xbl=vector (1,NBMAX) ;
         xb2=vector (1,NBMAX) ;
        zbrak (fx, X1, X2,N, xb11xb2,&nb) ;
        printf ( '\ nbrackets for roots of bessjO: \n") ;
        printf ( "%215 ZiOs V.16s %los\n", 'lover ", 'upper ", "f (low日r) ", "f (upper)
                                                                                        ") ;
        for (i= 1; i<=nb; i++)
             printf ( "%s %2d %10. 4f V.10. 4f X3s %10. 4f %10. 4f\ n",
                    ' root ", i, xbl[ ij, 工b2Ci] ," "
                   f工（工bl[i] ) ,fx（工b2Ei] )) ;
        free七vector（工b2 .1, 甘SMAX) ;
        free_ vector (xbl , I ,NB甘AX) ;
        return 0;
}

    Routine rtbis begins with the brackets for a root and finds the root itself by
bisection, The accuracy with which the root is found is determined by parameter
xacc. Sample program xrtbis finds all the roots of Bessel function Jo(x) between
Xl = 1.0 and X2 = 50.0. In this case xacc is specified to be about 10_ 6 of the value
of the root itself (actually, 10-6 of the center of the interval being bisected). The
roots root are listed, as well as Jo(root) to verify their accuracy.
/* Driver for routine rtbis */

作include <stdio . h>
#include "nr. h"
Ninclude "nrutil. h"

#define N 100
卞define 甘BMAX 20
斗define Xl 1.0
*define X2 50. 0

static float fx (float        x)
{
        return bessjo(x) ;
    156       N（月nerica/ 尸Sc肛）es Examp旭 Bo아（

}

jut main(void)
{
        jut .i, nb=NBMAX;
        float xacc 1root, 中工bi, *工b2;

        xbl=vector (1,NBMAX) ;
        xb2=vector (1,NBMAX) ;
        zbrak (f工，工1,12,N , 工bi, 工b2 小lb) ;
        printf ( '\ nftoots of bessjo: \n ') ;
        printf ( "%21s '/.16s\n", "x ", "f (x) ") ;
        for (i=1; i<=nb; i++) {
            工acc= (1. 0e田）卞（놔）1[i] ＋工b가幻）/2. 0;
            root=rtbis (f工 1 工bli幻 1 工b기刃 1 工acc) ;
            printf ( 'root Y,3d '/.14. 6f Y,14. 6f\ n", i, root, tx(root) );
          }
          free_ vector（工b2, 1, 甘BMA工）;
          free_ vector (xbl .1 ,NBMAX) ;
          retUrn 0;
}
                                                                               discussed,
     The next six sample programs are essentially identical to the one just
except for the root-finder they employ.   xrtflsp   calls rtflsp,   finding the   root by
                                                                                     uses
"false position". xrtsec calls rtsec and uses the secant method. xzriddr
Ridders' method, zriddr. xzbrent uses zbrent        to  give reliable  and efficient con-
vergence. The Newton-Raphson method implemented in rtnewt is demonstrated by
xrtnewt, and xrtsafe calls rtsafe, which improves upon rtnewt by combining it
with bisection to achieve better global convergence. The latter two programs include
a procedure funcd that returns the value of the function and its derivative at a given
x. In the case of test function Jo(x) the derivative is -Ji (x), and is conveniently in
    our collection of special functions.
    /* Driver for routine rtflsp 中/

    #lnclude <stdio.b>
    #include "nr. h1'
    #include "nrutil. h"

    #define N 100
    #defjne NBMAX 20
    #def in. Xl 1. 0
    #define 12 60. 0

    static float fx (float x)
    {
          return bessjo(x) ;
    }

    jut main(void)
    {
        ml1t i, nb=NBNAX;
        float 工acc ,root, 中工bi , 方xb2;

           xbl=vector (1,NBMAX) ;
           工b2=vector (1,NB片A工）;
                                      Ch카升or 9: 尸O야月nding and S이S可Eq石r幻ns   157

      zbrak (f工 'xl ' 工2, J, 工bi,工b之ktb) ;
      printf ( "\ nftoots of bessj0: \n") ;
      printf ( "%218 %16s\n", "x", "f (x) ") ;
      for (i=1; i<=nb; i++) {
          工acc=(1. oe-6) 卞（工bl[i] ＋工b2 [.i] )/2. 0;
          root=rtflsp (f工 , 工bl[i] . 工b2[i] ．工acc) ;
          printf ( "root 工3d %14. 6f '/,14.6f\ n", i, root, fx(root) );
      }
      free_ vector (xb2,1,NBMAX) ;
      free_ vector (xbl, 1,NBMAX) ;
      return 0;
}

／李
     Driver for routine rtsec 中1

#include <stdio.h>
*include "nr. h"
#include 'nrutil. h"

卄define N 100
#d日fine NBMAX 20
#define Xl 1. 0
#define X2 60. 0

static float fx (f] .oat x)
{
     return bessjo(x) ;
}

mnt main(void)
{
      jut i, nb＝甘BMAX:
      float 工acc ,root 1 卞工bi,＋工b2;

     工bl=vector (1,NB甘AX) ;
     工b2=vector (l ,NBMA工）;
     zbrak(f치 X1, X2, 瓦 工bi, 工t泣 小ub) ;
     printf ( "\ nRoots of bessj0: \n") ;
     printf ( "/,21s '/.l5s\n", "x", "f (z) ") ;
     for (i=1;i<=nb; i++) {
         工acc ' (1.oe-6汁 往bi［幻＋工b2 口］)/2. 0;
         root"rtsec (fx，工bi［幻 , 工b2[i] ,工acc) ．·
         printf ( 'root 工3d '/.14.6f %14. 6f\ n", i, root, fx (root) );
     1
     free_ vector (xb2, 1,NBMAX) ;
     free_ vector（工bi, 1, 甘B겨［A工）．·
     return 0;
}

/t Driver for routine zriddr 中1

#include <stdio.h>
#include "nr. h"
#include "nrutil. h"

#define N 100
#define NBMAX 20
     158    Numerical Recipes Example Book

#deflne Xl 1. 0
#define X2 50. 0


static     float   fx (float   x)
{
       return bessjO(x) ;
}

mllt main(void)
'C
       m1lt i 1nb=NBMAX;
       float xacc,root, *工bl,中工b2;


       xbl=vector (l ,HBMAX) ;
       工b2=vector (1 , 甘BMA工） ;
       zbrak (f工，X1, X2 , 瓦工bi, 如기h山）·，
       printf ( "\ n} oots of bessjO: \n' ) ;
       printf ( 'Y.21s 工15s\n ', "x ", 'f (x) ") ;
       for (i= 1; i<=nb; i++) {
           xacc= (1. oe-6) s (xbl[ i] +xb2[i] )/2. 0;
            root=zridd工（fx , xbl Ci]，工b2［幻 , 工acc) ;
            printf ( "root %3d 7.14. 6f %14. 6f\ n ", i, root, fx (root) );
       }
       free_ vector (xb2, 1,NBMAX) ;
       free小vector (xbl 1 I ,NBMAX) ;
       return 0;
}

/／京 Driver 如r routine zbrent 卞／/


#include <stdio . li>
#include "nr. h"
#include 'nrutil.       h"


#define N 100
#define NBMAX 20
#define Xl 1. 0
#define X2 50. 0

static     float   fx (float   x)
'C
       return bessjo(x) ;
1

ml1t main(void)
{
       mllt i, nb=NBMAX;
       float; 如1,root, 卓xbl, 卞工b2;


       xbl=vector (1, 甘BMAX) ;
       xb2=vector (1 ,NBPUX) ;
       zbra) (fx, Xl, X2, W, xb1. xb2.knb) ;
       printf ( "\ n!toots of bessjo: \n") ;
       printf ( "?.21s %15s\n' , 'x ' , "f (x) ") ;
       for (i= 1; i<=nb; i++) 'C
            to1=(1. oe-6)$(xbl[ i] +xb2[i] )/2. 0;
           root=zbrent (fx, 工bl幻 ,xb2[i] ,tol) ;
                                             Ch콰月er 9: 尸0야月nding and Sc台可Equ카幻ns   159
                printf ( "root %3d 玄14. 6f %14. 6f\ n", i, root, fx (root) );
            }
            free_ vector (xb2, 1,NBXAX) ;
            free_ vector (xbl, 1 ,NBMAX) ;
            return 0;
    }

    ／巾 Driver 如r routine rtfle日t; 卞／

    linclude <stdio.h>
    #include "nr. h"
    #include "nrutil. h"

    #define N 100
    #def ins NBMAI 20
    Idefine 工l 1. 0
    #define 工2 50. 0

    static fl oat fx (float x)
    {
        return bessjo(x) ;
    }

    static void funcd(float x, float *fn, float *df)
    {
        卞fn=bessj 0（工） ;
        卞df = 小essj I仕）;
}

milt main(void)
{
        mnt i, nb=NBMAX;
        float xacc,root, 卞工bl,中xb2;

        xbl=vector (1,NBMAX) ;
        xb2=vector (1,JBMAX) ;
        zbrak (！工 , 工1,工2,1 . 工bl, xb2,knb) ;
        printf ( "\ nRoots of bessjo: \n") ;
        printf ( "Y.21s '/.15s\n", "x". "f (x) ") ;
        for (i= 1; i<=nb;i++) (
            工acc=(1.oe-8)*(xbl [ij+ xb2[i] )/2. 0;
            root=rtnewt (funcd,xbltj) ,xb2[ij ,xacc) ;
            printf ( "root 工3d %14. 6f %14. 8f\ n", i, root, fx (root) );
        }
        free나vector（工b2, 1,NBXA工）;
        free_ vector (xbl, 1,IBMAI) ;
        return 0;
)

/* Driver for routine rtsafe */

#include <stdio.h>
#include "n工.h"
*include 1'nruti] ..h"

#define N 100
#define IBMAX 20
 160       Numerica/ 尸eci戶os Examp旭 Bo아（

#define 工l 1. 0
#define X2 50. 0

static float fx (float x)
{
       return bessjo(x) ;
1

static void funcd(float 工, float *fn, float *df)
{
       巾f0=be58j0（工） ;
       卓df = -bessj 1（工）;
}

mnt main(void)
{
       mllt i, nb=NBXA工;
       float 工acc ,root, 巾工bi, 字工b2;

       工bl=vector (1 ,NBML工）;
       xb2=vector (1,NBMAX) ;
       zbrak (！工 ,XI, X2,N, xbl , 工b기缸b) ;
       printf ( "\ nRoots of bessjo: \n") ;
       prmntf ( "%218 %15s\n'', "x " , "f (x) ") ;
       for (i= l; i<=nb; i++) {
           工acc=(1. 0e戶6) *(xbl口］+x泣口1) /2. 0;
           root=rtsafe (funcd, xbl ti] ,xb2[i] ,xacc) ;
           printf ( "root %3d Y.14.6f V.14.6f\ n" , i, root, fx (root) );
       1
       free_ vector (xb2, 1,NBMAX) ;
       free_ vector (xbl , 1 ,NBMAX) ;
       return 0;
}

    Routine laguer finds the roots of a polynomial with complex coefficients. The
polynomial of degree M is specified by M + 1 coefficients which, in sample program
xlaguer, are specified in the complex array a of dimension M + 1. The polynomial
in this case is
                            F (s) = T4 - (1 + 2i)x2 + 2i

    The four roots of this polynomial are x = 1.0, s = -1.0, x = i + i, and x = -(1 + i).
    laguer proceeds on the basis of a trial root, and attempts to converge to true roots.
    The root to which it converges depends on the trial value. The program tries a series
                                                                                    1.0 + i.
    of complex trial values along the line in the imaginary plane from -1.0- ito
    The actual roots   to which  it converges are compared  to all previously found values,
    and if different, are printed.
    ／中 Driver 如r routine laguer 中／

    *include <stdio .h>
    #include <math.h>
    *include "nr. h "
    #include "complex.h"

    *define M 4     /s degree of polynomial */
    #define MP1 (M+1)   /中 no. of polynomial coefficients */
                                     Ch邵珀9r 9: 尸O아尸nding and S이$ of Equat幻ns   161

#define NTRY 21
#def mne 甘TRY1 月TRY+1
#define EPS 1. e-6

mnt main(void)
{
    fcomple工 虹NTRY1] ,x;
    static fcomplex a[MPI] = {{0. 0,2.0} ,
                     {o.o,o. o}.
                   {-1 .이 -2 . 아 1
                   {o. o.o.o} ,
                   {1.o1o. o} };
    milt 치iflag its. j 1n=0;

    printf ( "\ nRoots of polynomial x4- (1+2i) *x2+2i\n") ;
    printf ( "\ n工lss V.158 V.7s\n' , "Real", "Co口plex", "#iter ") ;
    for (i=1; i<=NTRY; i++) {
        x=Complex ( (i- 11.0) /10. 0, (i- 11.0) /10.0) ;
        laguer (a,M.&x.kits) ;
        if (a == 0) {
              n=1;
              y[1] =x;
              printf ( "工5d %12. 6f %12. 6f %5d\n", n,x.r, x.i, its) ;
        } else {
              if 1ag=0;
              如r (j=1; j<=n; j++)
                   if (Cabs (Csub(x,y[ j] )) <= EPS*Cabs(x) ) iflag=1;
              if (iflag == 0) (
                   虹＋＋미＝工；
                   printf ("%sd %12. 6f %12. 6f V.5d\n", n.x.r. x. i. its) ;
             }
        }
    }
    reti끄工 0;
}

    zroots is a driver for laguer. Sample program xzroots exercises zroots, using
the same polynomial as the previous routine. First it finds the four roots. Then it
corrupts each one by multiplying by 1 + .Oli. Finally it uses zroots again to polish
the corrupted roots by setting the boolean variable polish to TRUE.
／卞 Driver 如r routine zroots 小／

#include <stdio .h>
*inclucle "nr.h"
#includo "complex.h"

#define N 4
#define NP1 04+1)
#define TRUE 1
#def ins FALSE 0

jut main(void)
{
     jut 치po:1.i日h;
    f complex roots [MPI] ;
    static fcomplex a[NP1] = {{O.0,2.O} ,
    162     Numerical Recipes Example Book

                        {Q. o,o.o},
                        {-i .이 -2 .아 1
                        {o.o,o.o}.
                        {1.o,o. o} };

      printf ( "\ nRoots of the polynomial x4- (1+2i) *x2+ 2i\ n") ;
      polish=FALSE;
      zroots (a,M.roots,polish) ;
      printf ( '\ nUnpolished roots: \n") ;
      printf ( "%14s %13月 V.13s\n", "root #", "real ", 'imag. ") ;
      for (i= 1;i<=M; i++)
          printf ( 'Y.lld %18. 6f 工12. 6f\ n", i, roots[i] .r, roots[i] .i) ;
      printf ( '\ nCorrupted roots: \n ') ;
      for (i=1; i<=M; i++)
           roots [i] =RCmul(1+O .01*i 1roots[i] );
      printf ( "%148 %13s %13s\n", "root 1 ", "real " ,"imag. ") ;
      for (i=1; i<=M; i++)
          printf ( "%lld %18. 6f %12. 6f\ n", i, roots[i] .r, roots[i] .i) ;
      polish=TftUE;
      zroots(a,M,roots,polish) ;
      printf ( "\ nPolished roots: \n") ;
      printf ( "Y.14s Y.13s %13s\n", "root #" ,"real " ,"imag. ') ;
      for (i=1; i<=M; i++)
          printf ( "Xlld 工18. 6f 工12. 6f \n", i, roots[ i] .r, rootsCi] .i) ;
      return 0;
}

   Routine zrhqr is an alternative to laguer for polynomials with real coe任icients.
Sample program xzrhqr tries it out on the polynomial x4 - 1.
／本 Driver 如r routine zrhqr 卞／

#include <stdio.h>
#include 'nr. h"
#include "nrutil. h"

#def ins N 4    /卞 degree of polynomial 中/
#define MP1 (M+1)   /s no. of polynomial coefficients 5/

mllt main(void)
{
      static float aEMP1] = {-1. 0,0.0,O刀,0刀,1刀} ;
      float 巾rti,牛rtr;
      mnt i;

      rti= vector (11M) ;
      rtr= vector (1,X) ;
      printf ( '\ nRoots of polynomial x4- 1\n ') ;
      printf ( '\ n%lSs %155\n' , "Real' , "Complex") ;
           zrhqr (a,M,rtr, rti) ;
           如r (i=1; i<＝甘；j++) {
                printf ( "%5d %12. 61 %12. 6f\ n", i, rtr[ i] 1rti[ i] );
           }
      free_ vector (rtr, 1,N) ;
      free_ vector (rti, 1,N) ;
      return 0;
}
                                        C/i邵片ar 9: 尸oot月nd加g and S이$ 可Equa加ns        163
        qroot is used for finding quadratic factors of polynomials with real coefficients.
    In the case of sample program xqroot, the polynomial is

                       P（끼 = 工6 e6工5 + 16x4 - 24x3 + 25x2 卞 18x + 10.

The program proceeds like that of laguer. Successive trial values for quadratic factors
x2 + Bx + C (in the form of guesses for B and C) are made, and for each trial, qroot
converges on correct values. If the B and C which are found are unlike any previous
values, then they are printed. By this means, all three quadratic factors are located.
The answer should be

                            P(x) = (x2 + 1)(x2 - 4x + 5)(x2 - 2x + 2)

／卞 Driv日r for routine qroot; 李／/

#include <stdio . It>
#include <inath.h>
#include "nr. h"
#include "nrutil. h"

#define N 6 /* degree of polynomial */
#define EPS 1. 0e-6
#define NTRY 10
#define TINY i. 0e-5

mnt main(void)
{
       mllt i 3 ,nflag, nr00t=0;
       static float pEN+1) ={10.0, -18.0,25. O, -24.0,16.0,-6. O,1.0} ;
       float *b, *c;

       b=vector (1,NTRY) ;
       c=vector (1,NTRY) ;
       printf ( '\ nP(x)=xm6-6x小5+16xm4-24xn3+25xn2-18x+10\n') ;
       printf ( 'Quadratic factors x2+bx+c\n\n") ;
       printf ( '%6s Y.los 工12s \n\n", 'factor ", 'b", 'c ") ;
       for (i=1;i<=NTRY; i++) {
           C 口］=0. 5杜 ;
           bCil = -0. 5*i;
           qroot (p,N,&b[i] ,&cli] ,EPS) ;
           if (nroot == 0) {
                 printf ( "工4d %15. 6f %12. 6f\ n", nroot,b[i] ,c[ i] );
                 nroot=1;
           } else {
                nflag=o;
                for (j= 1; j<=nroot; j++)
                    if ( (fabs (b[i] -b[ j] ) < TINY)
                         k& (fabs (c[ i] -c[ j] ) < TINY) )
                         nflag=l;
                if (nflag == 0) {
                    printf ( '%4d %16. 6f X12. 6f\ n ', nroot,b[i] ,c[ i] );
                    ++flroot;
                }
           }
      }
      free_ vector (c 1 I, 甘TRY) ;
164          Numerica/ 尸e帥始s Example Book

        trae_vector (b, 1 1NTRY) ;
        rett口:n 0;
}
                                                              In order to run the sample
    mnewt looks for roots of multiple nonlinear equations.
                                            usrfun    that returns  the matrix alpha of
program xmnewt we supply a procedure
                                                    to each of the variables, and vector
partial derivatives of the functions with respect
                                                           The sample program tries to
beta, containing ihe negatives of the function values.
find sets of variables that solve the four equatio ns

                                       H工｝H 哮 中 哮 + m      =
                                                                   0
                                     T! + 哮 + 堵 + 工：-l     =
                                                                   0
                                                工1 H 工2    =
                                                                   0
                                                ;r2- ;r3       =
                                                                   0

                                                      s to this set even without mnewt,
You will probably be able to find the two solution
                           x2  = X3.   If not, simply  take the output from mnewt and
noting that x1 = x2 and
                                               The output from mnewt should convince
plug it into these equations for verification.
you of the need for good starting values   (or that you should use newt instead!).
／卓 Driver 如r routine mite日t +/

 #include <stdio . h>
 *include <math.h>
 #include "nr. h "
 *inc].ude "nrutil. h11

                                                 **fjac)
    void usrfun(tloat 李x,int n1f1oat *fvec,float
    {
         mnt i;

         tjac口］[1] = -2. 0枉口］;
         fjac[ 1] [2] = -2.0*x[2] ;
         幻ac[1] [3] = -2. 0本x [3] ;
         ijac[ 1] [4] =1. 0;
         Thr (i=1; i<=n; i++) fjac[ 2] [i] =2.0*x[ i] ;
         f j ac [3] [ 1] =1.0 ;
          tjac[ 3] [2] = -1. 0;
          fjac[ 3] [3] =0.0,
          幻ac [3]［幻 =0. 0;
          fjac[ 4] [1] =0.0;
          fjac[ 4] [2] =1. 0;
          fjac[ 4] [3] = -1. 0;
          fjac[ 4] [4] =0. 0;
                                                         ;
           fvec［幻 = -SQR(x[ 1]卜S餌(x[ 2] )田qa（虹幻）＋工[4]
                                                        幻卜1. 0;
          fvec[2] =SQR(x[ 1] )+sqa（虹幻 ) +SQa(x口］)+SQa(虹
           fvec[3] 玎1]-虹2] ;
           fvec［幻 =x［그卜玎3] ;
    }

     #define NTRIAL 5
     #define TOLl 1.0e-6
     #define 뀨 4
     #define TOLF 1. 0e-6
                                     Ch랴升er 9: 尸0이同ndi四and Sets可Equa加ns         165

jut main(void)
{
    jut i, j, k, kk;
    float x工1卞工，中fvec, *卞fjac;

    fjac=matri工 ( 1, 瓦 1,N) ;
    fvec=vector (1,N) ;
    x'vector (1,N) ;
    for (kk'1; kk<=2;kk++) {
        for (k=1;k<=3;k++) {
             x工＝0. 2001本k方 (2李kk-3) ;
            printf ( 'Starting vector nu皿ber Y.2d\n", k) ;
            for (i '1; i<=4; i++) {
                 玎j] ＝工工＋0. 2中1．·
                 printf ( "%7s/.ld加 Y.5. 2f\ n".
                       " 工［." ,1, "] = " 1工［j] ) ;
             )
             printf ( ''\ n") ;
             for (j=1; j<=NTKXAL; j++) {
                 mne口t{1,工 1瓦TOLX1TOLF) ;
                 usrfun(x,N, fvec,fjac) ;
                 printf ("%5s '/.13a %13s\n ', "i ", "x[ i] ', "f ") ;
                 for (i=1; i<=N; i++)
                     printf ( "V.Sd Y.14.6f %16. 61\n",
                           i, x[il ,fvec[ i] );
                 printf ( "\ npreaa RETURN to continua. . .\n ") ;
                 (void) getcharO;
             }
         }
    }
    free..vector (x, 1,N) ;
    free..vector (f寸ec, 1,N) ;
    free_matrix (fjac, 1, 瓦 1,1) ;
    return 0;
}

    Sample program xnewt tries out routine newt on the nonlinear system

                                     11 = 工｝ + 哮 叫 2
                                                                O乙
                                     12=   (
                                           e    +
                                               '1_   1)
                                                          工二H
which has a root at (x1, x2) = (1, 1). It attempts to find the root starting from the
initial guess (2, .5). (This is Example 6.5.1 in Numerical Methods for Unconstrained
Optimization and Nonlinear Equations by Dennis and Schnabel.) mnewt, which ap-
plies Newton's method blindly without a globally convergent strategy, fails on this
example. (Note that newt is also used in the solution of two point boundary value
problems in Chapter 17.)
/* Driver for routine newt 卞/

#include <atdio .h>
#include <math.h>
#include "nr. h"
#include "nrutil . h'1

void funcv(int 끼float 工［그 , float f ［가
    166        N切nerica/ 尸ec徊es Example Book

{
        玎1] =SQR（工 [j] )+SQR(x[幻卜2. 0;
        f [2卜exp伍 [i] -i. 아仕口] *SQR（玎2]卜2. 0;
}

#define N 2

jOt main(void)
{
          jot i, check;
          float 巾x ' 卞f ;

          x=vector (1,N) ;
          f=vect0r (1, 표) ;
          工 [1] =2. 0;
          x [2] =0.5;
          newt Cx , N , &check , f uncv) ·，
          fui比V（瓦 치 f ) ;
          if (check) printf ( "Convergence prob].ems. \n") ;
          prxntf ( "%7s Y.3s %12s\n", "Index ", "x ", "f ") ;
          for (i=1; i<"N; i++) printf ( "%5d 工12. 6f V.12.6f\ n", j, x[i] ,f[ i] );
          free_ vector (f, 1,N) ;
          free_ vector (x, 1,N) ;
          return 0;
}

     The sample program for broydn, which implements a multidimensional general-
ization of the secant method, is identical to the one for newt:
／卞 Driver 如r routine broydn 巾／

#include <stdio.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

void fnncv (int n, float x (J, float tO)
    {
          f[ 1] =SQR(x[ 1] )+SQR(x[ 2] )-2. 0;
          玎기 相印伍 [1卜1. 0）奴 [2] *叩M工 [2] )口. 0;
}

    #define N 2

    jot main(void)
    {
           jot j, chack;
           float 卞工1卞f ;

           工＝vector (1, 甘） ;
            f'voctor (1JN) ;
                      ，
           工［l] =2 . 0·
           工［幻 =0.5;
           broydn(x,N, kcheck,tuncv) ;
           funcv(N, x,f) ;
           if (check) printt ( "Convergence problems. \n") ;
           printt ( "/.7s %3s 工12s\n", "Index", "x", "f ") ;
                                      Ch랴가er 9: 尸0야月ndi四and Se台可的嵋加ns                167

      or (i= 1; i< =N; i++) printf ( "Y.Sd V.12. 6f %12. 6f\ n", i, x[ i] ,fEi] );
    free_ vector (f, 1.11) ;
    fr日8-ye毗町 (x, 1 , 助 ;
    return 0;
}
Chapter 10: Minimization and Maximization of
            Functions

        Chapter 10 of Numerical Recipes deals with finding the maxima and mmn-
   ima of functions. The task has two parts, first the discovery of one or more
   bracketing intervals, and then the convergence to an extremum. mnbrak be-
   gins w凡h 如Os꺄ci月ed abscissas of a 血nc加n and searches 加 the "而wn川11"
   direction for brackets of a minimum, golden can then take a bracketing
   triplet and perform a golden section search to a specified precision, for the
   minimum itself. When you are not concerned with worst-case examples, but
   only very efficient average-case performance, Brent 's method (routine brent)
   is recommended. In the event that means are at hand for calculating the
   function's der加毗加e as w三11 as its va加e, consider dbrent.
       Most multidimensional minimization strategies are based on the above
   one-dimensional algorithms. Our single example of an algorithm that is not so
   based is a皿oeba, which utilizes the downhill simplex method. Among the ones
   that do use one-dimensional methods are powell, frprmn, and dfpmin. The
   月r毗 two make calls 的 uin皿in, a procedure that m加im物es a function along a
   given direction in space. lin皿in in turn uses the one-dimensional algorithm
   brent, if derivatives are not known, or dbr이lt if they are. powell uses
   only function values and minimizes along an artfully chosen set of favorable
   directions. frprmn uses a Fleicher-Reeves-Polak-Ribiere minimization and
   requires the calculation of derivatives for the function. dfpmin uses a globally
   convergent variant of the Davidon-'Fletcher-Powell variable metric method.
   This, too, requires calculation of derivatives, but the routine uses lnsrch for
   approximate one-dimensional minimizations.
            The chapter ends with two topics of somewhat different nature. The
       月r毗 is linear prog了amming, which dea加 w凡h the maxim初ation of a linear
       comb加ation of variables, subject to linear co끄straints. 끄山 pr이沅m is dea凡
        with by the simplex method in routine simplx. The second topic is the
       subject of large scale optimization, which is illustrated with the method of
       simulated annealing. One application of this is a combinatorial minimization
       problem, the "travelling salesman" problem in routine an如al. The second
       is the use of s加川吼ed annealing 的 find the d的aIm加imum in a continuous
       space, procedure amebsa.



    mnbrak searches a given function for a minimum. Given two values ax and bx
of abscissa, it searches in the downward direction until it can find three new values

1 尸n
                          Ch따升or 10: 人刃nimizat幻n and Max力nizat幻n of Funct幻ns       169

a工,bx,cx that bracket a minimum. fa,fb,fc are the values of the function at these
points. Sample program xmnbrak is a simple application of mnbrak applied to the
Bessel function J0. It tries a series of starting values ax,bx each encompassing an
interval of length 1.0. mnbrak then finds several bracketing intervals of various minima
of J0.
／卓 Driver 如r routine mnbra노 巾／

#includa <etdio . h>
tinclude "nr. h"

fl oat func (float x)
{
     return beeejo(x) ;
}

mnt main(void)
{
    float a工1b工 'C工, fa, fb, fc;
    mllt i;

    for (i=1; i<=10; i++) {
        a工＝i10 . 5 ;
        b工＝(i+ i. 0)中0. 6;
        口nbrak (&a工 ,kb工 1tC工 ,&fa,kfb, tfc, func) ;
        printf ( "%14e %12s '/.12s\n" , "a", 'b" , "c') ;
        prmntf ( "%3s X14.6f %12. 6f V.12.6f\ n", "x", a工,bx,cx) ;
        printf ( "%3s 工14. 6f 工12. 6f %12. 6f\ n", "f ", fa, fb, fc) ;
    }
    rett口rn 0;
}

    Routine golden continues the minimization process by taking a bracketing triplet
ax,bx,cx and performing a golden section search to isolate the contained minimum
to a stated precision TOL. Sample program xgolden again uses 70 as the test function.
Using intervals (ax,bx) of length 1.0 it uses mnbrak to bracket all minima between
x = 0.0 and x = 100.0. Some minima are bracketed more than once. On each pass, the
bracketed solution is tracked down by golden. It is then compared to all previously
located minima, and if different it is added to the collection by incrementing nmin
(number of minima found) and adding the location xmin of the minima to the list
in array amin. As a check of golden, the routine prints out the value of J0 at the
minimum, and also the value of J1, which ought to be zero at extrema of Jo.
/* Driver for routine golden */

tinclude <stdio .h>
#includa <aath.h>
tinclude "nr. h"

*def in. TOL i. Oe-6
*def in. EqL 1.0.-3

float fu끄c (float x)
{
    ret山rn be.町0(幼 ;
}
    170    Numerical Recipes Example Book


mllt main(void)
{
      mllt i, iflag, j, nmin=O;
      float ax,bx, cx, fa, fb, fc, 工min,gold,anin[21] ;

      printf ( "Minima of the function bessjO\n") ;
      printf ( "V.lOs %8s %17s 工12s\n", "min. #", "x ", "bessjO (x) '", "bessjl (x) ") ;
      for (i=1; i<=100, i++) {
          a工＝1;
          bx=i+1. O;
          mnbrak (&a工 , tb工 , tC工 , tt키 虹b,kfc, f山IC) ;
          g01d=go1den(a工 ,b工 , c工 ,fu끄c, TOL, *工mm1) ;
          if (nain == 0) {
                aminti] = xmln;
                nmln=1;
                printf ( "%7d %1& .6f 'I.12. 6f Y.12. 6f\ n",
                     xunin, xmin,bessjo(工皿in) .bessjl (xmin) );
          ) else {
                if lag=0;
               for (jrl; j<=n皿in; j++)
                   if (fabs (工min-amin[ j] ) <= EQL*xmin) iflag= 1;
               if (iflag == 0) {
                   amin [++n皿in]＝工mill;
                   printf ( "/.7d X15. 6f 工12. 6f Y.12.6f\ n",
                        nmin, xmin,besejO(xmin) ,bessj 1(l꾜in) );
               }
          }
      }
      return 0,
}

    There are two other routines presented that also take the bracketing triplet
ax, bx ,cx from mnbrak and find the contained minimum. They are brent and dbrent.
The sample programs for these two, xbrent and xdbrent, are virtually identical to
that used on golden. Note that dbrent is only used when the derivative can be
calculated conveniently.
／李 Driver 如r routine brent 卞／/

#include <stdio.h>
#include <math.h>
#include "nr. h11

#define TOL 1. Oe-6
#define EqL 1. 0e-4

float f山ic (float 工）
{
      return bessjo(x) ;
}

jot main(void)
{
      mnt i, iflag, j, nmin=0;
      float ax,bx, cx, fa, fb, fc, 工min,bren,amin[21] ;
                         C力랴升or 10: 凡仰功깨zat幻n and Maxi,끼za切n 可 Fun아幻ns                  171

    printf ( "\ nMinima of the function bessjo\n') ;
    printf ( "%lOs Y.8s /.17s %12s\n", 'min. #' , "z ', 'bessjO(x) ", 'bessji(x) ') ;
    for (i=1; i<=100; i++) {
        ax=1;
        뇨＝i+1. O;
        mu뇨ak (&a工 小b工 , tC치kfa, kfb, 缸디 func) ;
        bren=brent (a工 , b工 ! c工 ,func,TOL,&工皿in) ;
        if (nmin == 0) {
              a皿in[1]＝工皿in;
            n皿l11= l ;
            printf ( "Y.7d X15. 6f V.12. 6f %12. 6f\ n",
                 iunin, xmin ,bessjO(xmin) ,bessj1(xmin) );
        } else {
            if lag=0;
            for (j=1; j<=nmin; j++)
                 if (fabs（工皿in-a皿in [ji) <= (EQI片I皿in) ) iflag= l;
            if (iflag == 0) {
                 amin [++nmjn]＝工min;
                 printf ( 'Y.7d /.15. 6f V.12. 6f Y.12.6f\ n".
                       nmin, xmin,bessjo(xmin) ,bessj 1(xmin) );
             }
        }
    }
    return 0;
}

/* Driver for routine dbrent */

#include <stdio . h>
#include <math.h>
#include nnr. h"

#define TOL 1. 0e-6
#define EQL 1.0e-4

float dfunc (float x)
{
    ret山그l 小es町1（妨 ;
}

float func (float x)
{
    return bessjo(x) ;
}

jut inain(void)
{
    jut i iflag口 1n皿in=0;
    float a工1b工 'C工, fa, fb, fc, 工皿in,dbr,a且in[21] ·，

    printf ( '\ nNininta of the function bessjo\n ') ;
    printf ( "Y.los %8s Y.16s %12s /.lls\ n' ,
        'mmn. #", "x", "bessjo(x) ", "bessjl(x) ", "DBREJT") ;
    for (i= 1;i< 'lOO; i++) {
        a工＝l ;
        bx=i+1.0;
        mnbra노 (ta工 .kb工 ,kc工,kfa, &fb,&fc,func) ;
     172    Numerica／尸a非）es Examp旭 Book

           cibr=dbrent (a工 .bx 1 cx.func,dfunc.TOL,&工min) ;
           if (n皿jn == 0) {
                a皿in[1]＝工皿in;
                nmin=1;
                printf ( "%7d %1& .6f %12. 6f %12. 6f %12.6f\ n",
                     n皿in,工皿in, fl끄'C（工工in) ,dfunc伍min) .dbr) ;
           } else {
                if lag=0;
                for (j= 1; j (=nmin; j++)
                     if (faba（工皿in-a皿in[j] ) <= EqI片工mmn) iflag= 1;
                if (iflag == 0) {
                     a皿in [++nmin]＝工工in;
                     printf ( "%7d %15. 6f '/.12.6f %12.6f %12. 6f\ n",
                          nmin,工皿in, func (xmin) ,dfiuic (工ain) ,dbr) ;
                }
           }
       }
       return 0;
 }

    Numerical Recipes presents several methods for minimization in multiple dimen-
sions. Among these, the downhill simplex method carried out by amoeba is the only
one that does not treat the problem as a series of one-dimensional minimizations.
As input, 키noeba requires the coordinates of N + 1 vertices of a starting simplex
in N-dimensional space, and the values y of the function at each of these vertices.
Sample program xamoeba tries the method out on the exotic function
                    fa皿oeb = 0.6 - Jo[(x - 0.5)2 + (y - 0.6)2 + (z - 0.7)2]

which has a minimum at (x, y, z) = (0.5, 0.6, 0.7). As vertices of the starting simplex,
specified by the array p, we used (0,0, 0), (1, 0, 0), (0, 1, 0), and (0, 0, 1). A vector
xli] is set successively to each vertex to allow the evaluation of function values y.
This data is submitted to amoeba along with FTOL=1. OE-6 to specify the tolerance
on the function value. The vertices and corresponding function values of the final
simplex are printed out, and you can easily check whether the specified tolerance is
met.
/+ Driver 如r routine a皿oeba 中／

#include <stdio .h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

*define NP 4
#define JP 3
#define FTOL 1.0e-6

float func(float 工［가
{
       ratu]口1 0.6小的幻o(sQR仕口卜0. 旬＋sQR(玎幻-0.6)+SQR仕臼卜口7) );
}

mnt main(void)
'C
       m11t 치nfunc, j ,ndi且＝IP;
                             Ch카月er 10: M加沕仁刻幻n and Maximiza加n of Fun이幻ns                173

        float ＋工1中y, 卓＋P;

        x=vector (1,NP) ;
        y=vector (1,N?);
        p=Inatri工（1,NP,1，甘P) ;
        for (i=1;i<=MP; i++) {
             for (j=1; j<=NP; j++)
                  x[ j] =p[i] [j] =(i == (j+1) ? 1. 0 : 0.0) ;
             y[i] =func(x) ;
        }
        a皿oeba(p,y,ndim,F且兀func，缸func) ;
        printf ( "\ nNu皿ber of function evaluations: '/.3d\n" ,nfu끄c) ;
        printf ( "Vertices of final 3-d simplex and\n") ;
        printf ( "function values at the vertices: \n\n") ;
        printf ( "%38 7.108 '/.12s %12s Y.14s\n\n",
            " i " , " 虹i] " 1 " 虹i] " 1 "玎i] " , " fnl1Cti0ll" );
        如r (i=1; i<＝甘P; j++) {
            printf ( "%3d ", i) ;
            for (j=1; j<=NP; j++) printf ("%12.6f " mn] [j] ) ;
            printf ( "%12.6f\n", y[ij) ;
        1'
        printf ( "\ nTrue minimu皿 is at (0.S,0.6,0.7) \n") ;
        free_matrix(p,1,MP,1,甘P) ;
        free_vector (y,1,MP) ;
        free_vector (x, 1,NP) ;
        return 0;
}

   powell carries out one-dimensional minimizations along favorable directions in
N-dimensional space. The function minimized in sample program xpowell is defined
as
              func（乙 !/，기 =卜 川 (x 口尸 + (y - 기2 + (z - 旬可
The program provides powell with a starting point P of (3/2, 3/2, 5/2) and a set of
initial directions, here chosen to be the unit directions (1, 0, 0), (0, 1, 0), and (0, 0, 1).
powell performs its one-dimensional minimizations with linmin, which is discussed
next.
/方 Driver for routine powell */

#include <stdio .h>
#include <math.h>
#include "nr.h"
#include "nrutil. h"

#define NDIM 3
#define FTOL 1. Oe-6

float func (float xD)
{
    ret1lJ:
    returnll 0石小essjo
              .5-be8BjC (SQR(x口］-1. 0) +SQR(x[幻-2. 0) +SQR（虹引-3.0) );
1   '




mnt main(void)
{
    mnt i, iter, j;
    float fret, 中*工1;
    174            Numerica／尸ec徊es Examp旭 Book

           static float p[]={O. O,1. 5,1. 5, 2.5} ;

           工i=matri工 ( 1, 丑DIM,1，川：)IM) ;
           如r (i=1 ·, i<＝甘DIM; i++)
               for (j=1; j<=NDI긔［; j++)
                     xi[ i] [j] =(i == j ? 1.0 : 0. 0) ;
           povell(p, xi, NDIM,FrOL,&iter, &fret, func) ;
           printf ( "Iterations: %3d\n\n", iter) ;
           printf ( "Minimuln found at: \n") ;
           for (i 'l; i< 'NDIM; i++) printf ( "%12.6f ", p[ i] );
           printf ( "\ n\nMinimum f山lction value = %12. 6f \n\n", fret) ;
           printf ( "True minimum of function is at: \n") ;
           printf ( "Y.12. 6f Y.12.6f %12. 6f\ n", 1.0.2.0,3.0) ;
           free_matrix (xi, 1,甘DIM 1 1, NDIM) ;
           return 0;
}

    linmin, as we have said, finds the minimum of a function func along a direction
in N-dimensional space. To use it we specify a point P and a direction vector xi,
both in N-space. linmin then does the bookkeeping required to treat the function as
a function of position along this line, and minimizes the function with a conventional
one-dimensional minimization routine. Sample program xlin皿in feeds linmin the
function
                     func(x, y, 力 = （工 H 寸 + (y- 1)2 + (z 小 1)2
which has a minimum at (x, y, z) = (1, 1, 1). It also chooses point P to be the origin
(0, 0, 0), and tries a series of directions


                           (V5cos（즐命）, '/ sin（증命）, 1.0)
For each pass, tile location of the minimum, and the value of the function at the
minimum, are printed. Among the directions searched is the direction (1, 1, 1). Along
this direction, of course, the minimum function value should be zero and should occur
at   (1,     1,   1)   .




／卞 Driver for routine lin皿in 卞／

#include <stdio.lt>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

#define NDIM 3
#define P102 1. 5707963

float tunc (float xl] )
{
    mnt 1;
    float f=0. 0;

           for (i=1; i<=3; i++) f += (x (i] -1.0)*(x[ i] -1.0) ;
           return f;
1

mnt main(void)
                                 Ch카升er 10: M加沕仁a加n and Maximiza加n 아劤nc加ns      175

{
            jut i, j;
            float fret, 8r2,z, *p,*xi;

            p= vector (1,NDIM) ;
            xi=vector (1,NDIM) ;
            printf ( "\ nflinimu皿 of a 3-d quadratic centered\n'O;
            printf ( "at (1.0,1.0,1. 0) . Minimu皿 is found\n") ;
            printf ( "along a series of radials. \n\ n") ;
            printf ( "%9日 %128 Y.12s 7.14s \n", "x ", "y", "z", "minimu皿") ;
            for (1=0;i<=10; i+ +) {
                工＝P102中i/10. 0;
                sr2=sqrt (2.0) ;
                工i[1] =sr2中cos（기 ;
                工i [2卜sr2中sin仕）;
                xi[ 3] =1. 0;
                可:1] =p[2] 叩 臼1=o.o;
                liiusin (p, xi, NDI$,kfret, func) ;
                for (jr1; j<=3; j++) printf ( "%12. 6f ", p[ j] );
                printf ( "%12. 6f\ n", fret) ;
            }
            free_vector (xi, 1,甘DIM) ;
            free_ vector (p,1,NDIM) ;
            return 0;
:1  .




    fidirn accompanies linmin and is the routine that makes the N-dimensional
function func effectively a one-dimensional function along a given line in N-space.
There is little to check here, and our perfunctory demonstration of its use, in sample
program xfldim, simply plots fidim as a one dimensional function, given the function

                              func(x, y, z) = (x - 1)2 + (y 小 1)2 +(z - 1)2.

You get to choose the direction; then scrsho plots the function along this direction.
Try the direction (1, 1, 1) along which you should find a minimum value of funcrO at
position (1, 1, 1).
 /* Driver for routine fldim */

#include <stdio . h>
#include "nr. h"
#include "nrutil. h"

    float fi끄lc (float 工口 )
    {
             jut i;
             float f=0. 0;

             如r (i=1; i<"3; i++) f += 仕[i卜1. 0汁（虹口-1. 0) ．·
             return f;
    :1  ,




        #define WDIM 3

        jut ucom;    /李 defining declarations 卞/
        float 方Pcolu，京工icom, (*i江f iii比乂float 口）;
        176    N切lie庇洌尸ec加es Exam例a Book

    mnt inain(void)
    {
          ncoin=JDIM;
          pcoa= vector(1.ncois) ;
           xicois=vactor (1,ncom) ;
          nrfunc=func;
          pcom [1] =pcoin[2] =pcomC3] =0.0;
          pri毗f ( "\ nEnter vector direction along which to\n ') ;
          printf ( "plot the function. Minimua is in the\n") ;
          printf ( "direction 1.0 1.0 1.0 - enter x y z: \n") ;
          scanf ( " I.f '1.1 加" 11工icom口］'a工icomt2] ,k工icoin[3) ) ;
          scr帥LO(fldi皿）;
          free_vector (xicom,1,ncom) ;
          frea_vector(pcom.1,ncom) ;
          return 0;
    }

      frprinxt is another multidimensional minimizer that relies on the one-dimensional
 minimizations of linxnin. It works, however, via the Fletcher-Reeves-Polak-Ribiere
 method and requires that routines be supplied for calculating both the function and
 its gradient. Sample program xfrprmn, for example, uses

                        func(工, y, z) = 1.0 - Jo(x - { )Jo(y - { )Jo(z
                                                                          吉）
 and
                             Ofunc -J,'（卜加如
                                     寸 ,' \n - 2 )JOUI -극\   7- (：극）
                                                         2 /VU\  m - 2/
                              Ox
etc. A number of trial starting vectors are used, and each time, frprmn manages to
find the minimum at (1/2, 1/2, 1/2).
/* Driver for routine frprmn 求/

#include <stdio . K>
#jnclude <math.h>
#include 'nr. h"
#include "nrutil. h"

#def inc NDIM 3
#define FTOL 1.0e-6
#define P102 1.5707963

float func(float x[])
{
    return 1.아的朗叩仕口卜0.旬札essjo(虹幻-0. 5) *bes町0(玎引'-0.5) ;
}

void dfunc (float xD, float df口)
{
    df 口］=bessj I 仕口卜0.6汁bessjo（虹幻 -0 石汁besej0（江幻 七. 5) ;
    缸［幻 =bee町0（虹1] -0 石汁bessjl（虹幻山石汁bee町0（江키 -0.5) ;
    d玎幻 =bes町0(x[1]山. S汁bee月jO仕 [2卜0 石汁比sej 1仕口卜0.5) ;
}

mnt lnain(void)
{
    mnt iter, k;
                          Ch킥가er 10: Mm印1기zat幻n and Ma刃／nizat幻n of Funct幻ns    177

    fl oat angl. fret, 巾p;

    p=vector (1,NDIM) ;
    printf ( "Program finds the minimu皿 of a function\n") ;
    printf ( "with different trial sta工ting vectors. \n") ;
    printf ( "True minimum is (0. 5,0.5,0.5) \n") ;
    for (k'0; k<=4;k++) {
        angl=PI02*k/ 4. 0;
        p[1] =2. 0* cos (angl) ;
        아幻 =2. 0中sin(angl) ;
        p［幻 =0. 0;
        printf ( "\ nStarting vector: (Y.6. 4f. Y.6. 4f, V.6. 4f) \n",
             pCi] ,p[ 2] ,p[ 31) ;
        frprn (p,NDIM,FTDL,&iter, &fret, func,dfu恥) ;
        printf ( "Iterations: V.3d\n", iter) ;
        printf ( "Solution vector: (V.6. 4f, %6. 4f, %6. 4f) \n",
            pCi] ,p[ 2] ,pC3] );
        printf ( "Func. value at solution Y.14f\n", fret) ;
    }
    free_ vector (p. i, NDIM) ;
    return 0;
}

    The routine dlinmin is an alternative to linmin for minimization routines that
use derivative information as well as function values. The sample program for dlinmin
is essentially the same as for linmin, given above.
/s Driver for routine dlin皿jn */

#include <stdio . h>
#inc].ude <math.h>
#include "ni .h'1
#include "nrutil. h"

#def ins 吼）IM 3
#define P102 1. 6707963

float func (float 工口 )
{
    mnt i;
    float f=0. 0;

    for (j=1; j<=3; i++) f += (x[ i] -1.0) s(xCi] -1. 0) ;
    return f;
}

void dfunc (float 工口 ,float df ［그 )
{
    jot i;

    for (i=1; i<=3; i++) df[ i] r2. 0*(x[ i] -1. 0) ;
}

jot majn(void)
{
    mllt i, j;
    float fret, sr2，工，中p.中工1;
    178    Numerical Recipes Example Book


      p=vector (1,NDIM) ;
      工i=vector (11 甘DIM) ;
      printf ( "\ nMinimu皿 of a 3-d quadratic centered\n") ;
      printf ( "at (1. 0,1. 0, 1. 0) . Minimum is found\n") ;
      printf ( 'along a series of radials. \n\ n") ;
      pr].ntf ( "%95 %125 V.12s V.14s \n", "x ", "y " , "z", "minimum") ;
      for (i '0; i<=10; i++) {
           工＝P102卞i/10. 0;
           sr2=sqrt (2. 0) ;
           工i[1] =sr2中cos (x) ，·
           工i [2] =sr2京sin(x) ·，
           工i [3] =1.0;
           可1] =p[2]＝可幻 =0. 0;
           dlin皿in(p , 工i,NDIM,&fret, fun디dfui比）;
           for (j=1; j<=3; j++) printf ( "%12. 6f ", p[ j] );
          printf ( "%12. 6f\ n", fret) ;
      }
      free_ vector (xi, 1, 甘DIM) ;
      free_ vector (p, 1,110111) ;
      return 0;
}

     Completeness requires that we provide a sample program for dfldim, which is
presented in Numerical Recipes as a routine for converting the N-dimensional gradient
procedure to one that provides the first derivative of the function along a specified line
in N-dimensional space. It is exactly analogous to fidim and the program xdfldim
is the same.
/* Driver for routine dfldim */

#include <stdio.h>
#include "nr. h"
#include 1느｝工util. h"

#define NDIM 3

m1lt ncom;  /* defining decla工ations */
float *pco皿，＋工icom;
void (*nrdfun) (float 0, float 0) ;

void dfunc (float xD, float dfD)
{
      jot i;

      for (i=1; i<=3; i++) df[ i] =(x[i] -1. 0)*(x[ i] -1. O) ;
}

jot main(void)
{
     ncom=NDIM;
     pcom=vector (1,ncom) ;
     xicors=vector (1,ncom) ;
     nrdf山i=dfu끄C;
     printf ( "\ n目lter vector direction along which to\ n") ;
     printf ( "plot the function. Minim三 is in the\n") ;
     printf ( "direction 1.0 1.0 1.0 - enter x y z: \n\n") ;
                           Ch랴升er 10: M亦irr庇카幻n and Maximiza加n of Func的ns                179

    pcom[1] =pcom[2] =pcom[3] =0. 0;
    scanf ( " 工f 艾f /.V' ,kxicom[1] , 缸icom［幻 , k工icomE3] ) ，·
    scr毗o(dfldim) ;
    free尸vect乙r（工icom, 1.nc（가U) ·，
    free_ vector (pcom, 1,ncom) ;
    return 0;
}

    dfpmin implements the Broyden-Fletcher-Goldfarb-Shanno variant of the David-
on-Fletcher-Powell minimization by variable metric methods. It requires somewhat
more intermediate storage than the preceding routine, but it works well with a glob-
ally convergent strategy that requires only approximate line minimizations, and can
therefore be more e佈cient. Sample program xdfpmin works just as did the pro-
gram for frprmn, including the fact that it requires a procedure for calculation of the
derivative. The approximate line minimizations are carried out by lnsrch. In this
case we try it on the somewhat harder problem (Stoer and Bulirsch, Introduction to
Numertcal Analysis, p. 308):


                                                             + xi) ]2
                                                                        +,  + x i ,2
                   f             (3
                           10[ (x弓
                                                                                     )
                                                                           (2
                       =                  x1)
                                                                          1+ + x1)2
                                      -         -   x   (3
                                                                                (2
which has a minimum at (x1, x2) = (- 2, 士0.89442719). We take the initial guess to
be (0.1, 4.2). (The original problem in Stoer and Bulirsch has 100 in the first term
instead of 10. We have changed it because some machines may have trouble in single
precision. Even this easier problem requires double precision if you try to solve it
with powell.)
/* Driver for routine dfpmin */

#include <etdio . h>
*includa "nr. h'1
#include "nrutil. h"

static mnt 心1끄lC1ndf Ui比；

float func (float 工口 )
{
      float 工1p2sqr=SQR (2 .0＋工口1) ;

      ntnnC++ ;
      return 10. 0中
           SQR (SQh(x[ 2] )s (3.0-x[1] )-SQit(x[ 11) s(3. 0+x[1] ))+
           xlp2sqr/ (1. 0+xlp2sqr) ;
}

void df1끄ic (float 工［그 ,float df口 )
{
    float 工1sqr=SQR(x[ 1] )，工2sqr'SQR(x [21)，工lF口＝工[11+2. 0;
    float x1p2sqr=SQR(xlp2) ;

    ndf山lC++ ;
    df [1] =20. o* (x2sqr*(3.0吐 [1] )吐lsqr* (3 .0＋玎11) )*(吐2sqr田.0枉口卜3.야xl sqr) +
         2. 0中工1p2/ (l. O＋工lp2sqr) -2. 0巾工1p2*xlp2sqr/SQR( (1.0＋工lp2sqr) ) ;
    df 口卜40. o* (心sqr*(3. 0吐 [1] )吐始qr* (3. 아工 口］) ) 枉 [2] *(3. Ox口n ;
}
 180       Nume月ca／尸ec徊es Exa쨔,Ie Book


#define NDIM 2
#define GTOL 1. oe-4

mnt main(void)
{
    jilt iter;
    float *p, frst;

    p=vector (1,NDII4) ;
    printf ( "True minimum is at (- 2. O十O. 89442719) \n") ;
    nflnc=ndfunc=O;
    p［幻 =O.1;
    可幻＝4. 2;
    printf ( "Sta工ting vector: ('/.7. 4f, Y.7. 4f) \n", p[1] ,p[2] );
    dfpmin(p, NDIM, GTOL,&iter, &fret, func,dfunc) ;
       printf ( "Iterations: Y.3d\n", iter) ;
       printf ( "Func. evals: %3d\n", nfunc) ;
       printf ( "Deriv. evals: 'I,3d\n", ndfunc) ;
       printf ( "Solution vector: (Y.9. 6f, '/.9.6f) \n", p[1] ,p[2fl;
       printf ( 'Fu끄c. value at solution h14. 6g\n", fret) ;
       free_ vector (p,1,NDIM) ;
       return O;
}

    simpix is a procedure for dealing with problems in linear programming. In these
                                                                            subject to
problems the goal is to maximize a linear combination of N variables,
the constraint that none   be  negative, and that  as a  group they satisfy a number
of other constraints. In order to clarify the subject, Numerical Recipes presents
                                                                         problem into
a sample problem in equations (10.8.6) and (10.8.7), translating the
tableau format  in (10.8.18), and presenting a solution in equation (10.8.19). Sample
program xsimplx carries out the calculations that lead to this solution.
／本 Driver 如r routine simpl工 京／

 #include <stdio .h>
 #include "nr. h"
 #include "nrutil. Ii"

 #def ins 甘 4
 #define 14 4
 #def ins NP 5       ／京 NP >= N+1 巾／
 #define MP 6        ／卓 NP >= 14+2 本／
 #def ins 甘l 2       ／卞 141+142+143 = 甘 京／/
 #define 142 1
 #def ins 143 1
 #define NMIM2 (N+MI+142)

 mnt main(void)
 {
     ml1t i, icas티3 '卞izrov,卞iposv;
     static float c[MP] [NP] =
          {o .0,1.0,1.0,3. 0, -O.5,
          740. 0,-1. 0,0. 0, -2. 0, 0. 0,
          0.0,0 .O, -2. 0,0.0,7 .O,
          0. 5,O. 0,-1. 0,1. 0,-2. 0,
                              Ch叩旭r 10: 凡仰切iizat幻n and Maximiza加n of Fundi幻ns       181

        9.0,-1.0,-1.0,-1.0,-1.0,
        0.0,0.0,0.0,0.010. 0} ;
    float 巾Ca;
    static char *txt (IM1N2+1]=
        { " " , " 工1" 1 " 工2" 1 " 工3", " 工4" , " yl " 1" y2" , " y3" };

    虹rOv=ivec如r (1,I) ;
    iposv=ivector ( 1,긔) ;
    a=convert_日atrix(kc[0] [0] ,1,MP,1,JP) ;
    si叩lx(a,N,J,M1,M2,N3,kicase,izrov,ipoav) ;
    if (ic心a == 1)
        printf ( "\ n띠lbo띠lded objective function\n") ;
    else if (icase == -1)
        printf ( "\ nno solutions satisfy constraints given\n") ;
    else (
        printf ( "\ n工lls", " ") ;
        for (i=1;i<=1;i++)
            if (izrov[i] <= IM1M2) printf ( "工los", t工t[izrov[i] ]);
        printf ( "\ n") ;
        for (i=1;i<=fl+1;i++) {
            it (i == 1 I I iposv[i- 1] <= 1M1M2) {
                  if Ci > 1)
                       priatf ( "%s" ,txt[ iposv[i- 1]]);
                  else
                       printf ( " ") ;
                  printf ( "%10.2f ", a[i] [1] );
                  for (j=2; j<'N+l; j++)
                       if (izrovtj- 1] <= 5甘1)12)
                            pri小f ( "%10. 2f ", a[i] 口] );
                  printf ( "\ n") ;
                }
          }
    }
    fr. e_convert_Natrix(a,1,MP, 1,1?);
    free_ivector (iposv,1,fl) ;
    fr ee_ivector(izrov,1,1) ;
    return 0;
}

     anneal is a procedure for solving the travelling salesman problem - a problem
that is included as a demonstration of the use of simulated annealing. Sample program
xannea]. has the function of setting up the initial route for the salesman and printing
final results. For each of NCITY=10 cities, it chooses random coordinates x[i] ,y[i]
using routine ran3, and puts an entry for each city in the array ip'tr Ci]. The array
indicates the order in which the cities will be visited. On the originally specified path,
the cities are in the order i=1, . . ,loso the sample program initially takes iptr Ci] =i.
(It is assumed that the salesman will return to the first city after visiting the last.)
A call is then made to anneal, which attempts to find the shortest alternative route,
which is recorded in the array. After finding a path that resists further improvement,
the driver lists the modified itinerary.
/s Driver for routine anneal 中/

#include <stdio.h>
*include "nr . h"
*include "nrutil . l111
182       肌加｝eric可 尸ec肛）es Examp旭 Book


#define ICITY 10

mllt main(void)
{
    mnt i, ii, *iorder;
    long idu皿＝（中111) ;
    float 卞工1卞y;

    iorder=ivector (1,JCITY) ;
    x=vector (1,ICITY) ;
    y=vector (i. JCITY) ;
    for (i=1; i<=JCI丁Y;i++) {
        虹i] =ran3（缸du皿）;
        虹ij "ra必（缸du크）;
        iord日r［幻 =1;
      }
    aniieal(x, y,iorder,NCITY) ;
    printf ( "*** System Frozen ***\n") ;
    printf ( 'Fina]. path: \n") ;
    printf ( "%8s X 9s %128\n", "city ", "x". "y") ;
    for (irl; i<=JCITY;i++) {
         ii 'iorder[ i] ;
        printf ( "%44 %10. 4f %10. 41\n", ii, x[ii) ,y (ii] );
    }
    free_vector (y.1.JCITY) ;
    free_vector (x, 1,NCITY) ;
    free_ivector ( iorder 11.ICITY) ;
    return 0;
}

     If you have any doubts about the effectiveness of simulated annealing in dealing
with otherwise intractable minimization problems with continuous control variables,
the next example, using routine amebsa, ought to convince you of the merits of
the technique. The 4-dimensional test function to be minimized, tfunk, is quite
diabolical: It is bounded below by a parabolic function whose principal axes are in
the ratio 1 : 3 : 10 : 30, and bounded above by 3 (or more generally 1+AUG) times
the lower bound. At most points, the function in fact takes on its upper bound; but
within a radius 0.3 (that is, RAD) of any integer lattice point, it dives down to its lower
bound in a narrow parabola. The narrow parabolas, in other words, form an infinite
lattice of local minimum "traps," trying to capture the test point. The "surface" of
this function would look like a piece of 4-dimensional Swiss cheese, scooped out into a
paraboloid. Any minimization algorithm that goes strictly downhill will get captured
by the holes, virtually always. Let's see how well simulated annealing does at finding
the true minimum, located at the origin.
     The program prompts for a starting temperature, t, and for the number of amoeba
iterations, iter, that it should perform before reducing the temperature by 20%.
The latter number, therefore, controls the annealing schedule. The test point is
aiway started at a position p = (10, 10, 10, 10), down at the bottom of a steep local
minimum. Note how the program sets up the initial simplex and its function values,
as required by the routine a皿ebsa.
    Try running the program first with t=1000, iter= 20. For this low a value of
                         Ch햐）旭r 10: M加沕仁카幻na耐Max加zat幻n of Functions              183

t, the routine never gets out of its original local minimllum, and it ends up with a
function value of 101001. Next try the input values t= l x 106, iter= 20. For most
random seeds, the program now finds its way to the origin, with a final function value
of 1, the true global minimum.
    To see the effect of too rapid quenching, try t=1 x 106, iter= 2. For many random
seeds, the program now gets part of the way towards the origin but then freezes into
a local minimum. For other seeds, the program does find the true global minimum.
You might enjoy experimenting with other input values to map out the regions of
relatively secure and insecure global convergence.
/中 Driver for routine amebsa */

#include <stdio.h>
#include "or .b"
*include "nrutil. h"

*def ins NP 4
#def ins 甘P S
#define F丁OL 1. OE-6
#def ins 甘 4
#defina RAD 0. 3
#define AUG 2.0

long idum= (- 64) ;

float tfunk(float p口)
{
      m1lt 3;
      float q,r, sU皿d=0.0, sumr=0.0;
      static float wid[N+1] ={0. 0, 1. 0,3.0,10. 0,30.0);

       for (j= 1; j<=N; j++) {
           q=p[ j] 李日id[ j] ;
           r=(float) (q >= 0 ? (int) (q+0. 5) : -(int) (0.5-q) );
           su口r += 中q;
           sn皿d += (q-r) *(q-r) ;
       }
       return 1+suisrs(j+ (sujd > fiJ.汁R1D ? AUG : AUG*su皿d/ (R.AD*LtAD) ));
)

mnt main(void)
{
    mllt i, iiter, iter, j, jiter, ndi皿=JP,nit;
    float temptr, yb, ybb;
    float; 年卞p '李工，sy．卞pb;
    static float xoff[ NP+1]={0. 0,10. 0, 10. 0,10.0,10.0) ;

    p=matrix(1,MP,1,NP) ;
    工＝vect口r (1,NP) ;
    y=vector (1,MP) ;
    pb=vector (i, NP) ;
    for (i= 1; i<=MP; i++)
        如r (j=1; j<=IP; j++) 이口 [jI= 0. 0;
    for (; ;) {
         for (3=2; j<"XP; j++) p[ j] [j- 13=1.0;
         for (i= 1;i<=MP; i++) {
184       Numerical Recipes Example Book

              如r (j=1; j<=NP; j++) 工［j]=(p[i] ［刃 += 工ofl口］);
              虹i] =tf山lk（工） ;
          }
          yb=l. 0e30;
          printf ( "Input t, iiter: \n'') ;
          if (scanf ( "V.t Y.d ', kteinptr,kiiter) == EOF) break;
          ybb=1. 0e30;
          nit 0;
          for (jiter= l; jiter< =100; jiter+ +) {
               iter= iiter;
               七emptr 中＝ 0. 8;
               amebsa(p, y,ndim,pb, kyb,FTOL, tfunk,&itar, temptr) ;
              nit   += iiter- iter;
               if   (yb < ybb) {
                     ybb=yb;
                     printf ( "%6d /.10. 3e ", nit, temptr) ;
                     for (j=1; j<=NP; j++) printf ( "Y.10. 5f ". pb[ j] );
                     printf ( "Y.15. 7e\n" , yb) ;
               }
               if   (iter   > 0) break;
          }
          printf ( 'Vertices of final 3-0 simplex and\n' ) ;
          printf ( "float values at the vertices: \n") ;
          printf ( "Y.3s Y.l0s %12s %12s %14s\n\n ',
              "l ", ''X ［工］" , " y [口“ , ' 2 [l ] " ,"f 1lnCtiOn" ) ;
          for (i=1; i<=MP; i++) {
              printf ( ''V.3d ", i) ;
              for (j=1; j<=NP; j++) printf ( "Y.12. 6f " ,p[ i] 口] );
              printf ( "%15. 7e\n", y[i] );
          }
          printf ( "X3d ' , 99) ;
          for (j=1; j<=NP; j++) printf ( "%12.6f ", pbtj] );
          printf ( "%1S. 7e\n'", yb) ;
      }
      free_ vector (pb, 1,NP) ;
      f re s_ v ector (y , 1,NP) ;
      free_ vector (x, I , HP) ;
      free. matrix (p, i ,MP, i, NP) ;
      printf ( "Normal completion\n") ;
      return 0;
}
     Chapter 11: Eigensystems

             In Chapter II of Numerical Recipes, we deal with the problem of finding
       eigen vectors and eigen values of matrices, first dealing with symmetric ma-
        trices, and then with more general cases. For real symmetric matrices of
       small-to-moderate size, the routine jacobi is recommended as a simple and
       foolproof scheme of finding eigenvalues and eigenvectors. Routine eigsrt may
       be used to reorder the output of jacobi into descending order of eigenvalue.
       A more efficient (but operationally more complicated) procedure is to reduce
       the symmetric matrix to tridiagonal form before doing the eigen value analy-
       sis. tred2 uses the Householder scheme to perform this reduction and is used
       in conjunction with tqli. tqli determines the eigenvalues and eigenvectors
       of a real, symmetric, tridiagonal matrix.
          For nonsymmetric matrices, we offer only routines for finding eigen values,
      and not eigenvectors. To ameliorate problems with roundoff error, balanc
      makes the corr司）onding rows and columns of the matrix have comparable
      norms while leaving eigen values unchanged. Then the matrix is reduced to
      Hessenberg form by Gaussian elimination using elmhes. Finally hqr applies
      the QR algorjthm to find the eigenva加es of the Hessenberg matrix.



    jacobi is a reliable scheme for finding both the eigenvalues and eigenvectors of a
symmetric matrix. It is not the most e伍cient scheme available, but it is simple and
trustworthy, and it is recommended for problems of small-to-moderate order. Sample
program xjacobi defines three matrices a,b,c for use by jacobi. They are of order
3, 5, and 10 respectively and are, each in turn, sent to jacobi. For each matrix, the
eigenvalues and eigenvectors are reported. Then, an eigenvector test takes place in
which the original matrix is applied to the purported eigenvector, and the ratio of
the result to the vector itself is found. The ratio should, of course, be the eigenvalue.
／卞 Driver 如r routine jacobi 卞／

#include <stdio.h>
#include "nr.h"
*include "nxutil. h"

#deXine NP 10
Idefine hUT 3

ml1t main(vojd)
-C
      jilt i. j, k,kk,1,1].,nrot;
      Btatic float a[3] [3)=


                                                                                   185
186       Numerical Recipes Example Book

      (1. 0, 2. 0,3. 0,
      2. 0, 2. 0, 3. 0,
      3. 0,3 . 0,3. 0} ;
  static float bCS] [53=
      {-2 .0, -1. 0,0. 0, 1.0,2. 0,
      -1.0,-i .0, 0. 0,1. 0, 2.0,
      0.0,0.0,0. 0,1. 0, 2. 0,
      1. 0, 1. 0, 1. 0, 1. 0, 2. 0,
      2. 0, 2. 0, 2. 0, 2. 0, 2. 0} ;
  static fl oat c[NP] [NP] =
       {5. 0,4. 3,3. o,2. o, i. o,o. o, -1. o,-2. o,-3.o,-4..0,
       4. 3,5. 1, 4. 0,3. 0, 2. 0, 1.0,0. 0, -1.0, -2.0 ,-3 .0,
       3 . 0,4. 0 , 5. 0 , 4. 0, 3. 0, 2 . 0 , I . 0,0. 0,-i . 0, -2 . 0,
       2. 0, 3. 0, 4. 0,5. 0, 4.0,3. 0,2.0, i. 0, 0.0, -i. 0,
       1. 0, 2. 0, 3. 0, 4. 0, 5. 0, 4.0,3. 0, 2. 0,1.0,0.0,
       0. 0, i. 0, 2. 0,3. 0,4. 0,5.0,4. 0,3. 0, 2.0, 1.0,
       -1. 이 0. 0, 1. 0, 2 . 이 3. 0, 4 . 이 5. 0, 4 . 이 3 . 이 2. 0,
       -2. 0,-i. 0,0. 0,1.0, 2. 0,3.0,4.0,5.0,4. 0,3. 0,
       -3.0, -2. 0, -i. 0,0. 0,1.0, 2. 0,3.0,4. 0,5. 0, 4. 0,
       -4. 0, -3. 0, -2. 0, -i. 0,0. 0,1. 0,2.0,3.0,4.0,5. 0} ;
      fl oat 抑1, 卞r 1 中本v 1 卞卞日 ;
      static m1lt num[4] =(0, 3, 5,10} ;

      d=vector (i ,MP) ;
      r=vector (1,NP) ;
      v=matrix (i, NP, 1,NP) ;
      for (i=1; i<=NMAT; i++) {
          if (i == 1) a=convert_matrix (&a[0] [0] ,i, num[i] , i, n山n[i] );
          else if (i == 2) a=convert_matrix (&bto] [0] ,i, nu皿[i] ,1,n끄n[i] );
          else if (i == 3) e=convert_matrix (Ac[0] [0] ,i, num[i] ,1,num[ij) ;
          jacobi(e,num[i] ,d, v,&nrot) ;
          printf ( "matrix number %24\n", i) ;
          printf ( "n山nber of JACOBI rotations: '/.3d\n", arot) ;
          printf ( "eigenvalues: \n") ;
          for (j=1; j<=num[i] ;j++) {
              printf ( "/.12.6f ", d[ j] );
              if ( (j % 5) == 0) printf ( "\ si") ;
           }
           prmntf ( "\ neigenvectors: \n") ;
           for (j '1; j<=num[i] ;j+ 4) {
               prmntf (叫（gs %34 \n", "nuinber ", j) ;
               for (k=1;k< 'nu皿[i] ;k++) {
                     printf ( "%12.6f ", v[k] [j] );
                     if ( (k 7. 5) == 0) printf ( "\ n") ;
                }
                printf ( "\ n") ;
           }
           /* eigenvector test */
           printf ( "eigenvector tast\ n") ;
           for (j= 1; j (=num[i] ;j+ +) {
               for (l= i; l<=num[i] ;l+ +) {
                     r [1] =0.0;
                     for (k=1;k<=nu可幻 ;k++) {
                           if (h > 1) {
                               kk=1;
                               11=k;
                           } els日 {
                                                                        Ch可升er 11: E勺ensyst日ns   187
                                       kk=k;
                                       11=1;
                               )
                               r[ l]    += (etll]   [kk] sv[k] [j] );
                          )
                    }
                    printf ( "vector number %3d\n", j) ;
                    printf ( ' '/.lls Y.14s Y.10s\n",
                         "vector ", "mtrx*vec. ", 'ratjo ") ;
                    for (].=1; l< =numfi] ;l+ +)
                         printf ( "%12. 6f %12. 6f Y,12. 6f\ n ",
                              v[l) Cu] ,r[ ].J ,r[ l] /v[ l] 口] );
              }
              printf ( "press RETURN to continue. . .\n ") ;
              (void) getcharO;
              Zree_ convert_matrix (e, 1,nu.m[ j] 1 1,num[i] );
         }
         fr ee，皿atri工（v. 1．甘P. 1 . 甘P) ;
         free_ vector (r, l, NP) ;
         free_ vector (d, 1, 月P) ;
         return 0;
    )

     eigsrt reorders the output of jacobi so that the eigenvectors are in the order
 of decreasing eigenvalue. Sample program xeigsrt uses matrix c from the previous
program to illustrate. This l0x 10 matrix is passed to jacobi and the ten cigenvectors
 are found. They are printed, along with their eigenvalues, in the order that jacobi
returns them. Then the matrices d and v from jacobi, which contain the eigenvalues
and eigenvectors, are passed to eigsrt, and ought to return in descending order of
eigenvalue. The result is printed for inspection.
,'中 Driver for routine eigsrt */

#include <stdio. h>
*include 1'nr. h "
#iacluda "nrutil.         h"

#def in. NP 10


mnt main(void)
{
        mllt i, j, nrot;
        static fl oat 吐月P1 [N円＝
             {5 .0, 4. 3,3.0, 2. 0,1.0 0. 0.-I. 0, -2. 0 , -3. 01-4. 0,
             4. 3, 5. 1,4. 0,3. 0, 2.0,1. 0,0. 0, -1. 0, -2. 0 ,-3. 0,
             3. 0, 4. 0, 6. 0, 4. 0,3.0, 2. 0,I. 0,0.0, -1. 0, -2. 0,
             2.0, 3 . 이 4 刀 丙 . 이4 刀,3. 0,2.0, 1 .0, 0.0, -I .0,
             1. O, 2.0, 3. 0, 4. 0,5.0,4. 0,3. 0, 2. 0,1.0, 0.0,
             0. 0, l. 0, 2. 0, 3. 0, 4.0,5. 0,4.0, 3. 0, 2.0,1.0,
             -1. 0,0.0,1.0, 2. 0,3.0, 4. 0,6. 0,4.0, 3.0,2.0,
             -2. 0, -I. 0,0. 0,1.0,2. 0,3.0, 4. 0,5.0,4. 0,3. 0,
             -3. 0, -2. 0. -1. 0,0.0,1. 0,2. 0,3.0, 4. 0, 6. 0, 4.0,
             -4. 0, -3. 0, -2. 0. - 1.0,0. 0,1. 0 , 2. 0,3.0, 4.0, 6.0) ;
        float 卞d, *中V. 中卞e;

        d=vector (1,NP) ;
188       Nume比a! R比加＄Exa끼均 Book

    v=aatrix (l, iP, 1,JP) ;
    e=convert_matrix(kc [0] [0] ,l 1JP, l 1IP) ;
    printf ( "         Findi垠 Eigenvectore **卞京卞中＼n') ;
    jacobi（이月P,d, v,幻irot) ;
    printf ( "unsorted eigenvectora: \n") ;
    for (j=l; j<=IP; j++) .(
        printf ( "eigenvalue %34 = %12.6f\a" 山d[ i] );
        printf ( "eigenvector: \n") ;
        for (j=l; j<=IP; j++) {
               printf ( "茗12. 6f ", v[ j] [i] );
               if ( (j % 5) == 0) printf ( "\ n") ;
          }
          printf ( "\ n") ;
    }
    printf ( "\        Sorting Eigenvectors *s*s**\n\n") ;
    eigsrt (d.v,NP) ;
    printf ( "sorted eigenvectora: \n") ;
    for (i=1;i<=NP;i++) {
        printf ( "eigenvalue 工3d = %12.6f\n", i, d[i] );
        printf ( "eigenvector: \n") ;
          for (j=l; j<=IP; j++) {
              printf ("%12.6f ", v[ j] [i] );
              if ( (j % 5) == 0) printf ( "\ n") ;
          }
          printf ( "\ n") ;
      }
      free_ convert_matrix(e,1,1? , 1,IP) ;
      frea_matrix (v, 1,NP, 1,NP) ;
      free_vec如r (c%,1,I기 ;
      return 0;
}

    tred2 reduces a real symmetric matrix to tridiagonal form. Sample program
xtred2 again uses matrix c from the earlier programs, and copies it into matrix a.
Matrix a is sent to tred2, while c is saved for a check of the transformation matrix
that tred2 returns in a. The program prints the diagonal and off-diagonal elements of
the reduced matrix. It then forms the matrix f defined by F = ATCA to prove that
f is tridiagonal and that the listed diagonal and off-diagonal elements are correct.
/s Driver for routine tred2 s/

甘include <stdio . h>
#include "nr.h"
#include "nr比il. h"

*define NP 10

mnt main(void)
{
    mnt i, j, k,l, m;
    float Cd,巾e1卞中a14卞t ;
    static float c[NP] [NP] =
        { 5.0, 4. 3, 3.0, 2.0, 1.0, 0.0,-l. 0,-2.0,-3.0,-4.0,
           4.3, 5.1, 4.0, 3.0, 2.0, 1.0, 0.0,-l. 0,-2.0,-3.0,
           3.0, 4.0, 5.0, 4.0, 3.0, 2.0, 1.0, 0.0,-1.0,-2.0,
           2. 0, 3. 0, 4. 0, 5. 0, 4. 0, 3. 0, 2.0, 1. 0, 0.0, -1.0,
                                                              Cha,t升er 11: 日gensyst이17S   189

             1.0, 2. 0, 3. 0, 4. 0, 5. 0, 4.0, 3. 0, 2. 0, 1. 0, 0.0,
             0. 0, 1. 0, 2. 0, 3. 0, 4. 0, 5. 0, 4.0, 3. 0, 2. 0, 1.0,
            -1. 0, 0. 0, 1. 0, 2. 0, 3. 0, 4. 0, 5.0, 4. 0, 3. 0, 2. 0,
            -2. O, -1.0, 0. 0, 1. 0, 2. 0, 3. 0, 4. 0, 5. 0, 4. 0, 3. 0,
            -3. O, -2. O, -1. 0, 0. 0, 1. 0, 2.0, 3. 0, 4. 0, 5.0, 4. 0,
            -4. O, -3. 0, -2. O, -1. 0, 0. 0, 1.0, 2. 0, 3. 0, 4. 0, S. 0} ;

    d=vector (1,NP) ;
    e=vector (1,NP) ;
    a=matri工 ( 1,NP, 1, 卯）;
    f=matrix (1,NP,1,NP) ;
    如r (i=1; i<＝川느j++)
        for (j= 1; j<=NP; j++) a[i] 口]=c[i- 1] [j- 1] ;
    tred2(a,NP,d, e) ;
    printf ( "diagonal elements\n") ;
    for (i=1; i<=NP; i++) (
        printf ( "/.12. 6f ", d[i] );
        if ( (ix 5) == 0) printf ( "\ n") ;
    }
    printf ( "off尸diagonal elements\n") ;
    for (i=2; i<=NP; i++) (
        printf ( "/,12. 6f ", e[i] );
        if ( (iX 5) == 0) printf ( "\ n") ;
    }
    /* Check transformation matrix */
    for (j=1; j<=NP; 3++) {
        for (k=1;k<"NP;k++) {
            玎刃 [k] =0. 0;
            for (1=1; ].<=NP; l++) {
                 for (m=1;m<"NP;m++)
                         f[ ji[ k] += a[l] [j] *c[l- 1] [m-1] *a[m] Ek] ;
               }
        }
    }
    ／中 Ho口 does it look? 京／
    printf ( "tridiagonaJ. matrix\n") ;
    for (irl; i<=NP; i++) {
        for (j "l; j<=NP; j++) printf ( "Y.7. 2f ", f[ il[ j] );
        printf ( "\ n") ;
    }
    free_aatrix (f, 1,NP,1, WP) ;
    free_matrix(a, 1,NP, 1,1(P) ;
    free1vector (e, 1,1 (P) ;
    fre日_ vector (d, 1, 甘P) ;
    retui그i0;
}

    tqll finds the eigenvectors and eigenvalues for a real, symmetric, tridiagonal
matrix. Sample program xtqli operates with matrix c again, and uses tred2 to
reduce it to tridiagonal form as before. More specifically, c is copied into matrix a,
which is sent to tred2. From tred2 come two vectors d, e which are the diagonal
and subdiagonal elements of the tridiagonal matrix. d and e are made arguments
of tqli, as is a, the returned transformation matrix from tred2. On output from
tqli, d is replaced with eigenvalues, and a with corresponding eigenvectors. These
are checked as in the program for Jacobi. That is, the original matrix c is applied to
 190       Numerical Recipes Example Book

each eigenvector, and the result is divided (element by element) by the eigenvector.
Look for a result equal to the eigenvalue. (Note: in some cases, the vector element is
zero or nearly so. These cases are flagged with the words "div. by zero".)
/中 Driver 如r routine tqli */

#include <stdio.h>
#include <math.h>
#include "or .b"
#include "nruti] ..h"

#define NP 10
#define TINY 1.Oe-6

mllt main(void)
{
       jut i 口 1k;
       float 字d 1 4e 1中f 1 卞李a;
       static float c[NP] [NP] =
           { 5. 0, 4. 3, 3. 0, 2.0, 1.0, 0. 0, -1.0,-2.0,-3. 0,-4. 0,
              4. 3, 5. 1, 4. 0, 3. 0, 2. 0, 1. 0, 0. 0,-1. 0,-2. 0,-3.0,
              3. 0, 4. 0, 5. 0, 4. 0, 3. 0, 2. 0, 1.0, 0.0,-1. 0,-2.0,
              2. 0, 3. 0, 4. 0, 5. 0, 4. 0, 3. 0, 2.0, 1.0, 0.0,-1. 0,
              1. 0, 2. 0, 3. 0, 4. 0, 5. 0, 4. 0, 3. 0, 2.0, 1. 0, 0.0,
              0. 0, 1. 0, 2. 0, 3. 0, 4.0, 5. 0, 4. 0, 3.0, 2. 0, 1. 0,
             -1. 0, 0. 0, 1. 0, 2. 0, 3. 0, 4. 0, 5. 0, 4. 0, 3. 0, 2. 0,
             -2. 0,-j .O, 0.0, 1. 0, 2. 0, 3.0, 4. 0, 5. 0, 4.0, 3. 0,
             -3. 0,-2. 0,-1. 0, 0.0, 1 . 0, 2. 0, 3.0, 4.0, 5. 0, 4. 0,
             -4. 0,-3. 0,-2. 0,-i. 0, 0.0, 1. 0, 2.0, 3.0, 4.0, 5.0);

       d=vector (1,NP) ;
       e=vector (1, 甘P) ;
       f=vector (1,NP) ;
       a=matrix (1, 甘P,1,NP) ;
       for (i "1; i<=NP; i++)
            for (j=1; j<=NP; j++) a[i] [j] =c[i- 1J[ j- i) ;
       tred2(a,NP,d, e) ;
       tqli (d, e,NP, a) ;
       printf ( "\ nEigenvectors for a real symmetric matrix\n") ;
       for (i= 1; i<=NP; i++) {
            如r (3=1; j<＝月P; j++) {
               f[ j] =0. 0;
               for (k=1;kz=NP;k++)
                      f[ j] += (c[ j- 1] [k--1) *a[k] [i] );
            }
            printf ( "/.s %3d '1,8 '/,10. 6f\ n", "eigenvalue", i, " =", d[i] );
            printf ( "%lls V.14s Y.9s\n", "vector ", "mtrx*vect. ", "ratio ") ;
            for (j= 1; j<"NP; j++) {
                if (fabs (a[ j] [i] ) < TINY)
                      printf ( "%12.6f '/.12.6f 工12s\n",
                           缸刃［幻 ,f口］,"div. by o") ;
                 else
                     priutf ( "%12.61 'I.12. 6f '/.12.6f\ n",
                         缸3] [ii ,f[ j] ，玎刃／a[ j끄i] ) ;
            }
            printf ( "Press ENTER to continue. . .\n " );
            (void) getcharO;
                                                                          Ch카丑or 11: E勺ensysten四   191
      }
     free_matrix(a,1,NP,1,NP) ;
     free_vector (f 11,1?);
     fr. e_vector (e,1,NP) ;
     free_vector (d,1,NP) ;
     retul：且 0;
}

    bal띠lc reduces error in eigenvalue problems involving non-symmetric matrices.
It does this by adjusting corresponding rows and columns to have comparable norms,
without changing eigenvalues. Sample program xbalanc prepares the following array
a 白r ba].anc


                                               0 0 0

                                      ll lll
                                                              l ll ll
                                                         ll
                                                                      /
                                               0 l0 l0        0
                                                         上
                                                         1
                                                                 0 0
                                               l  l l
                                                              0 l0
                                                                 l ll
                                                                    0
                                                         ll
                                                                  1
                                                              l
                                                              \
The norms of the five rows and five columns are printed out. It is clear from the
array that three of the rows and two of the columns have much larger norms than
the others. After balancing with balanc, the norms are recalculated, and this time
the row, column pairs should be much more nearly equ孔

/中 Driver for routine balanc */

#include <stdio .h>
*include <math.h>
#include "nr.h"
#include "nrutil. t111

#define NP 5

mnt main(void)
{
    mlt i, j;
    float; 卞C1+r1＋卞a;

     c=vector (1,NP) ;
    r=vector (1,NP) ;
    a=matrix(1,NP,1,IP) ;
    for (i=1;i<=NP;i++)
         for (j=1; j<=JP; j++)
              aCi] Cj] = ( ( (1 & 1) U     ' (j & 1) ) ? 100.0 : 1.0) ;
    ／小 Write norma 卞／
    for (i=1;i<=1P;i++) (
        r Ci] =c Ci] =0.0;
         for (j=1; j<=IP; j++) {
             rti] += fabs(a[i] [j] );
              cCi] += fabs(aEj] [i] );
          }
    }
    printf ( "rova: \n") ;
    for (i=1;i<=1P;i++) printf ( " 工12.2f ", rCi] );
    printf ( "\ ncolumns: \n") ;
    for (i=1;i<=1P;i++) pri毗f ( "%12.21", c[i) );
192          肌imerica／尸9'亦治$ Examp旭 Book

    priatf ( "\ n\n斗卞中卞＋ Balancing zatri工 亡*中中＋\n\n") ;
    bal띠lc(a 1NP) ;
    ／中 Write norm月 中／
    for (i=1; i<=NP; i++) {
        r Ci] =c Ci] =0.0;
        for (j=1; j<=IP; j++) {
              r[ i] += fabs(a[i) [j] );
              c[i] += fabs(atj] Ei] );
             }
      }
      printf ( "rows: \n") ;
      for (i=1; i<=5P;i++) printf ( '%12. 2f ", r[ i] );
      prjntf ( "\ ncolumns: \n") ;
      如r (i=1;i<=IP;i++) printf ( '%12.2f ", c[i] );
      printf ( "\ n") ;
      free_matrix (a,1,甘P11,NP) ;
      free_vector (r, 11NP) ;
      free_vector (c, 1, 甘P) ;
      return 0;
}

     elmhes reduces a general matrix to Hessenberg form using Gaussian elimination.
It is particularly valuable for real, non-symmetric matrices. Sample program xelmhes
employs balanc and elmhes to get a non-symmetric and grossly unbalanced matrix
into Hessenberg form. The matrix a is




                                                       mm5mm
                                                             n0    8
                                       4e
                                       l
                                                   3 4
                                              O
                                              乙

                                          n
                                         9J
                                                                                     1
                                               3
                                                           =
                                                           U    n
                                                                r    0
                                                                     U
                                        4U
                                        1 =bn                        8
                                                      n0   4 <U n0
                                          4
                                            <
                                            U     n
                                                  1                n
                                                                   r
                                                                                         \
After printing the original matrix, the program feeds it to bal카lc and prints the
balanced version. This is submitted to elmhes and the result is printed. Notice that
the elements of a with i>j+1 are all set to zero by the program, because elmhes
returns random values in this part of the matrix. Therefore, the output of the test
program is guaranteed to look Hessenberg. To check that it is the cor毛ct Hessenberg
matrix, one has to go further and compute its eigenvalues, as will be done in the
example program after this one. We include here the expected results for comparison.
Balanced Matrix:
              1.00        2.00         37.50                4.00             6.00
              2.00        3.00         50.00                6.00             6.00
             24.00       32.00          5.00               48.00            56.00
              4.00        6.00         75.00                7.00             8.00
              6.00        6.00         87.60                8.00             9.00


Reduced to Hessenberg Form:

          1.00e+00    3.94e+01      9.62e+00        3.33a+00              4.ooe+00
          2.40e+01    2.73a+01      1.16e+02        4.80e+01              4.80e+01
          0.00e+00    8.55e+01     -4.78e+00       -1.33e+00             -2.oOe+00
          0. ooe+00   0.00e+00      5.19e+00        1.45e+00              2.17e+00
          0.00e+00    0.00e+00      0. oOe+00       6.95e-08              4.77e-07
                                                                   Ch邵）旭r 11: E也ensyst이ns   193
 ／卞 Driver 如r routine .1口he8 +/

    #include <stdio . a>
    斗includa "nr.h"
    卞include "nrutil. h"

    #define Np 5

 mi1t main(void)
 {
      mlit i, j;
      atatic float b[NP] [NP] =
           {1.이2.이300. 0,4.0丙 . 0,
           2. 0,3.0,400.0,5.0 16.0,
           3.0,4.0,5.0,6. 0,7.0,
           4.0,5.0,600.0,7.0,8. 0,
           5.0,6.0,700.0,8.0,9. 0} ;
      float; 卞中a;

         a=convert_matrix(*b[0] [0] ,1,NP, 1,NP) ;
        printf ( "S卞卞牛＋ original matri工 卞卞卞中卞＼n" );
         for (i=1; i<=NP;i++) {
              for (j=1; j<=NP; j++) printf ( "%12. 2f ", a[i] [j] );
             printf ( "\ n") ;
        }
        pri小n "           balance matrix 牛李卞卞李＼It,,);
        ba].anc(a,NP) ;
        for (i=1;i<=NP;i++) {
             for (j=1; j<=NP; j++) prmntf ( "%12. 2f ", a[i] [j] );
             printf ( "\ n") ;
        }
       prmntf C " 卞巾卞*5 reduce to hessenberg 如rm               \ll " ) ;
        e加hoe（피 NP) ;
        for (j=i; j<=NP-2; j++)
             for (i "j+2;i<=NP;i++)
                  缸i] [j] =0.o;
       for (i=1;i< 'NP;i++) {
             for (j=i; j<=1P; j++) printf ( "%12. 2e", a[i] 日) );
            printf ( "\ n") ;
       }
       free_convert_matrix (a, 1,NP, 1,NP) ;
       ret1口그i 0;
}

    hqr, finally, is a routine for finding the eigenvalues of a Hessenberg matrix using
the QR algorithm. The 5 x 5 matrix a specified in the array a is treated just as you
would expect to treat any general real non-symmetric matrix. It is fed to balanc
for balancing, to elmhes for reduction to Hessenberg form, and to hqr for eigenvalue
determination. The eigenvalues may be complex-valued, and both real and imaginary
parts are given. The original matrix has enough strategically placed zeros in it that
you should have no trouble finding the eigenvalues by hand. Alternatively, you may
check them against the list below:
Matrix:
           1.00            2.00             .00            .00             .00
194         Numerical Recipes Exa까le Book

          -2. 00          3. 00           .00       .00             .00
           3.00           4. 00         60. 00      .00             .00
          -4. 00          5. 00        -60. 00     7.00             .00
          -5. 00          6. 00        -70.00      8.00           -9. 00


Eigenvalues:
           real                imag.
          60. 000000          0. 000000
           2. 000000         -1. 732062
           2. 000000          1.732062
           6. 999999          0. 000000
          -9. 000000          0.000000

/* Driver for routine bqr 字1

#incl끄de <stdio .h>
#iuclude "nr. ii"
#include "nrutil. h"

#def ins NP 5

mllt main(void)
{
      mllt i, j;
      static float cENP) [NP] =
           {i . 이2 . 이0. 0,0 . 이0.0,
           -2. 0,3.0,0. 0,0.0,0.0,
           3.0,4. 0,50. 0,0.0,0.0,
           -4. 0,5. 0, -60. 0,7.0,0. 0,
           -5. 0,6. 0, -70. 0,8.0 ,-9 . 0} ;
      float; 卞日r , *wi, 本卞a;

      wr=vector (1,NP) ;
      vi=vector (1,NP) ;
      a=convert. matrix (&c[0) [0] ,1,NP, 1,NP) ;
      printf ("matrix: \n") ;
      for (i "l ; i<＝표F느 i++) {
          for (j=1; j<=NP; j++) printf ( "%12. 2f ", a[i] 日] );
          printf ( "\ n") ;
      }
      bal카lc (a,NP) ;
      elmhes (a,NP) ;
      hqr (a, 甘P 戶r 1日i) ;
      printf ("eigenvalues: \n") ;
      printf ( "%lls %16s \n", "real ", "imag. ") ;
      for (i=1; i<=NP; i++) printf ( "/.lsf %14f\n", wr[i] ,wi[ i] );
      free..convert...matrix(a. 1,甘P, 1,NP) ;
      free. vector (vi, 1,NP) ;
      free..vector (wr, 1, NP) ;
      return 0;
}
Chapter 12: Fast Fourier Transform

        Chapter 12 of Numerical Recipes deals with the fast Fourier transform
    (FFT). Routine fourl performs the FFT on a complex data array. twofft
    does the same transform on two real-valued data arrays (at the same time)
    and returns two complex-valued transforms. Finally, realft finds the Fourier
    transform of a single real-valued array. Two related transforms are the sine
    transform and the cosine transform, which comes in two incarnations. The
    corresponding routines are sinft, cosftl and cosft2. For FFTs in two or
    more dimensions the routine fourn is supplied. Real data in two or three
    dimensions is more efficiently handled by r1ft3, while huge data sets on
    external media can be FFT'd by fourTh.



    Routine fourl performs the fast Fourier transform on a complex-valued array
of data points. Example program xfourl has five tests for this transform. First,
it checks the following four symmetries (where h(t) is the data and H (n) is the
transform):
 1. If h(t) is real-valued and even, then H (n) = H (N - n) and H is real.
 2. If h(t) is imaginary-valued and even, then H (n) = H (N - n) and H is imaginary.
 3. If h(t) is real-valued and odd, then H (n) = -H (N - n) and H is imaginary.
 4. If h(t) is imaginary-valued and odd, then H (n) = -H (N - ii) and H is real.
    The fifth test is that if a data array is Fourier transformed twice in succession,
the resulting array should be identical to the original.
/* Driver for routine fourl .1

tinclude <atdio.h>
*include <math.h>
tincludo "ni . h"
linclud. "nrutil . h11

void prntft (float dataO ,uneign.d long nn)
{
    Un月igned 如ng a;

    printf ( "%4i %13s %13e %12e 工13s\n",
        "a", "real(n)" . "inag. (a)", "real(I- n) " , "iag. (卜n)") ;
    printf ( "   0 %14. 61 %12.6f %12. 6f %12.6f\n",
        data[1] ,data[2] ,data[1] ,data(2] );
    for (n=3;n<=nn+1;n+=2) {
        printf ( "X4lu 茗14.ef %12.61 %12.6f %12.6f\n",

                                                                                 fl:rn
    196       Numerica/ 尸ec仁冶＄ Example Book

                 ( (n-1) /2) ,dataEn] ,dataEn+1] ,
                 data [2snn+2-n] ,data [2snn+3-n] );
      }
      printf ( " press return to continue . . .\n ") ;
      (void) getcharO;
      return;
}

#define NN 32
#define NN2 (2SNN)

mnt main(void)
{
      long i;
      mnt isign;
      float 牛data, 卓dcmp;

      data=vector (1,NN2) ;
      dcmp=vactor ( I ,NN2) ;
      printf ( "h(t) =real-valued aven-function\n') ;
      printf ( "h(n) =h(N-n) and real?\n") ;
      for (i二l; i<NN2; i+=2) {
          data [i] =1. 0/ (S（그R ( (float) (j- 甘N口1)／표丑）+1. 0) ;
          data[i+1] 二0. 0;
      }
      isign=l;
      fourl (data,NN, isign) ;
      prntft (data, N甘) ;
      prmntf ( "h(t) rimaginary-valued 日ven-function\n"') ;
      printf ( "h(n) 'h(N-n) and imagmnary7\n") ;
      for (i: t; i<NN2; i+=2) {
          data[i+1] =1. 0/ (SQR ( (float) (i巾NN-1) /NN) +1. 0) ;
          data[i] =0.0;
      }
      is ign=1;
      如unl (data, 甘N, isign) ;
      prntft (data,NN) ;
      printf ( "h(t) =real-valued odd-function\n') ;
      printf ( "h(n) = -h(N-n) and imaginary?\n") ;
      如r (i '1 ·, i<N甘2; i+=2) {
           data［刃＝( (float) (i- 甘N-1) /NN) /(S아t( (float)         (i- 甘甘-1) /N甘）+1.0) ;
           data[i+1] =0.0;
      }
      data[1] =0 .0;
      isign=l;
      founl (data, NN, isign) ;
      prntft (data,NN) ;
      printf ( "h(t) =imaginary-valued odd-function\n") ;
      printf ( "h(n) = -h(N-n) and real?\n ') ;
      如r (i=1; i<N甘2; i+=2) {
          data[i+1] =( (float) (i- NN-1) /NN) /(SQR ( (float)       (i尸NN-1) /N뵤)+1. 0) ;
          data[i] =0. 0;
          }
      data[2] =0. 0;
      is ign=1;
      fourl (data,N片, isign) ;
      prntft (data,N비;
                                                   Ch카가or 12: Fast I七ur旭r Transform   197
       /* transform, inverse-transform test 牛/
       for (i= 1; i<NN2; i+=2) {
           da七a［幻 =1. o/ (sQR(0.5本 ( i- N甘-1.0) /NN)+1 .0) ;
           dcmp[i] =data(i] ;
           data[i+1] =(0. 25* (i느甘甘-1.0) /NN）卞exp(- SQR(0. 6卞 (1-甘N小1)／甘甘）) ;
           dcnip[i+1J=data[i+1] ;
      :1-
      isign=1;
      fo丑rl (data,NN, isign) ;
      isign = -1;
      fourl (data,甘N, isign) ;
     printf ( "%23s Y.33s \n", "original data: ' , "double fourier transform: ") ;
     printf ( "\ n %3s '/.155 7.12s Y.12s %12s \n",
           "k ', "real h(k) "', "imag h(k) ", "real h(k) " , "imag h(k) ") ;
     for (i=1; i<N月; i+=2)
           printf ( "%41u %14. 6f 7.12. 6f %12. 6f %12. 6f\ n" ,
                 (i+1) /2, dcmp[i] ,dcmp[i+1J ,data[i] /甘N,data[i+1] /NN) ;
     free_ vector (dcmp, 1,NN2) ;
     free_ vector (data, 1,NN2) ;
     return 0;
}

    twofft is a routine that performs an efficient FFT of two real arrays at once by
packing them into a complex array and transforming with fourl. Sample program
xtwof ft generates two periodic data sets, out of phase with one another, and performs
a transform and an inverse transform on each. It will be difficult to judge whether
the transform itself gives the right answer, but if the inverse transform gets you back
to the easily recognized original, you may be fairly confident that the routine works.
／卞 Driver for rout缸te t口offt 卞／

#include <stdio .h>
#include <math. h>
#include 'nr. h"
#include "nrutil. h"

#define 月 32
#define 甘2 (2卞甘）
#define PER 8
幷define P1 3.1415926

void prntft (float dataD,unsigned long on)
{
    unsigned long n;

    printf ( "%45 %13s '/.13s %12s '/.13s\n' .
         "n", "real (n) ", "imag. (n) ", "real(N-n) ", "imag. (N-n) ") ;
    printf ( "     0 %14. 6f '1.12.6f 7.12. 6f 7.12.6f\ n",  '
        dataCi] ,data[2] ,data[1] ,data[2] );
    for (n=3;n<=on+1;n+ '2) {
        printf ( ' 工41u 7.14.6f 7.12.6r '1.12. 8! %12. 6f\ n".
               ( (n-1) /2) ,data[n] ,data[n+1:l,
              data [2snn+2-n] ,data [2*nn+3-n] );
    }
    printf ( " press return to continue . . .\n 'D;
    (void) getcharO;
    198    Nume月ca/ 尸ec徊es Examp旭 Book

      return;
}

mllt majn(void)
{
      unsigned long i;
      mllt isign;
      float 半datal, 卞data2,中fftl, 中fft2;


      datal=vector (1 ,N) ;
      data2=v ect or ( I ,目) ;
      fftl= vector (1 . 片2) ;
      fft2= vector ( 1,1(2) ;
      for (i= 1; i< =N; i++) {
           datal [i] = f1oor (O. 5+cos (j方2. O*PI/ PER) );
           data2[i) =floor (0. 5+sin (i* 2. O*PI/ PEP.));
      }
      twofft (datal ,data2 1 fftl , fft2 , N) ;
      printf ( "Fourier transform of first           function: \n") ;
      prntft (fftl, N) ;
      printf ( "Fourier transform of second function: \n') ;
      prntft (fft2, 甘) ;
      ／卞 Invert tra끄Sf ora 小／
      isign = -1;
      fourl (fftl. ,N, isign) ;
      printf ( " inverted transform          first     function: \n') ;
      prntft (fftl. N) ;
      如url (fft2 , 甘 isign) ;
      printf ( "inverted transform           second function: \n") ;
      prntft (fft2, N) ;
      free_ vector (fft2, 1,1(2) ;
      free_ vector (fftl .1. (
                             12) ;
      free_ vector (data2, 1,1) ;
      free v吼t,江（datal , 1 . 助 ;
      return 0;
}

    realft performs the Fourier transform of a single real-valued data array. Sample
routine xrealft takes this function to be sinusoidal, and allows you to choose the
period. After transforming, it simply plots the magnitude of each element of the
transform. If the period you choose is a power of two, the transform will be nonzero
in a single bin; otherwise there will be leakage to adjacent channels. xrealft fol-
lows every transform by an inverse transform to make sure the original function is
recovered.
/方 Driver for routine realft         *7

#include <stdio. h>
#include <math.h>
#include "nr. h "
#include "nrutil.      h"

#define EPS 1. 0e-3
#define NP 32
#define WIDTH 50. 0
#define P1 3. 1415926
                                                 Ch司가er 12: Fast Fou月er Trans幻rm   199


jut main(void)
{
    jut i. j 1n=NP/2,nhiin;
    float big, per, scal, small, tdata, *size;

    data=vector ( 1,NP) ;
    size=vector (1,NP/ 2+1) ;
    for (; ;) {
        printf ( "Period of sinusoid in channels (2-V.2d) \n", NP) ;
        scanf ( "Y.f ' , kper) ;
        if (per <= 0. 0) break;
        for (i=1; ic.=NP; i++)
             data[i] =cos (2. 0*PI* (i- 1) /per) ;
        realft (data,NP, 1) ;
        big = -1. 0e10;
        for (i= 2; i<=n; i++) {
             sizeti] =sqrt (SQR(data[2*i- 1] )+SQR(data[2中i] ));
             if (sizeti) > big) big=size (x] ;
        }
        size[1] =fabs (data[1] );
        if (sizeEl) > big) big=sizaCl] ;
        size[n+1)=fabs (data[2] );
        if (size[n+i] > big) big=size[n+1] ;
        日cal= WIDTE/big;
        for (i=1; i<=n; i++) {
            nlim= (int) (0. 5+scal*size[i] +EPS) ;
            pr].ntf ( ' 工4d ", i) ;
             for (j=1; j<=n1im+1; j++) printt ( "*") ;
             printf ( '\ n") ;
        }
        printf ( ''press RETURN to continue . . , \1ln) ;
        (void) getcharO;
        realft (dataNP - 1) ;
        big = -1.0elO;
        small=1. 0e10;
        for (i=1; i<=NP; i++) {
            if (dataCi] < small) sma11=data[i] ;
            if (dataCi] > big) big=data[i] ;
        }
        scal=wloTll/ (big- small) ;
        for (i=1; i<=NP; i++) {
            nlim=(int) (0. 6+scal* (data[i] -small)+EPS) ·，
            printf ( "%4d ", i) ;
            for (j=1; j<=nlim+1; j++) printf ( '* ") ;
            printf ( '\ n ') ;
        }
    }
    free_ vector 佃iz미 1, 且하2+1) ;
    free_ vector (data, 1,NP) ;
    return 0;
}

    sinft performs a sine-transform of a real-valued array. The necessity for such
a transform arises in solution methods for partial differential equations with certain
kinds of boundary conditions (see Chapter 19). The sample program xsinft works
    200             Numerical Recipes Example Book

exactly as the previous program. Notice that in this program no distinction needs to
be made between the transform and its inverse. They are identical.
/中 Driver for routine sinft           */

#include <stdio .h>
#include <math.h>
#include "nr. h"
#include 'nrutil. h"

#define EPS 1. 0e-3
#define NP 16
#define WIDTH 30. 0
#define P1 3. 1416926

jot main(vojd)
{
      float big,per, scal,small, *data;
      jot i口, nlim;

     data=vector (j ,NP) ;
     如r      ;) {
               (;
         printf ( "\ nPeriod of sinusoid in ch띠lnels (3-Y.2d) \n", IP) ,
          scanf ( "%f ", &per) ;
          if (per <= 0.0) brea1 ;
          for (lrl; i<=NP; i++)
               data[i] =sin(2. 0*PX* (i- 1) /per) ;
         sinft (data. NP) ，·
         big = -1. 0elO;
         small=l. 0e10;
         for (i=1; i<=NP; i++) {
               if   (data[i] < small) sma].l=data[ij;
               if   (data[i] > big) big=data[ii;
         }
         scal=WIDTH/ (big- small) ;
         for (i=1; i<=NP; i++) {
               n1ia=(int) (scals (dataCi] -small)+EPS+0.5) ;
               printf ( "%4d ", i) ;
               for (j=1; j<=nhim+1; j++) printf ( "* ") .
               printf ( '\ n") ;
          J.
          printf ( "prose RETURN to continue . . .\ll " ) ;
          (void) getcha工O;
          sinft (data, 且P) ;
          big = -1. 0e10;
          saall=l .Oelo;
          for (i=1; i<＝甘P, i++) {
              if (data[i) < small) small=dataCi] ,
              if (dataCi] > big) big=data[i] ;
          }
          scal=WIDTH/ (big-suiall) ;
          如r (i= 1; l <＝甘P; i++) {
              n1im=(int) 佃cal中（data［幻田mall) +EPS+0．旬 ;
              printf ( "%4d ", i) ;
              for (j=1; j<=n1im+1; j++) printf ( "* ") ;
              printf ( "\ n") ;
          }
                                               Ch카）ter 12: Fasr Four旭r Trans幻rm   201
    )
    free_vector (data11, NP) ·．
    retur끄 0;
}

    cosftl is a companion procedure to sinft that does the cosine transform. It
also plays a role in partial differential equation solutions. Program xcosftl is again
the same as xrealft.
/／中 Driver 如r routine cosftl 中／

#include <stdio.h>
#include <math.h>
*includa ' 'nr.h'1
Ninclude 'nr此il. h'1

#define EPS 1. Oe-3
#define NP 17
#define WIDTH 30. 0
#define P1 3.1416928

jut ntain(void)
{
    milt i j. nhim;
    float big1per1scal, small, sdata;

    data=vector (1,NP) ;
    for (; ;) {
          printf ( "Period of cosine in ch카nels (2-%2d) \n ", 目P) ;
          scanf ( 'V.f ', kper) ;
          if (per <= 0. 0) break;
          for (i=1; i<=NP; j++)
               data[i] =cos(2. 0sPI*(i- 1) /per) ;
         cosftl (data,NP-1) ;
         big = -1. oelO;
         Bmall=1. oelo;
         for (i=1; i<=1P; i++) {
              if (data[i] < small) small=data[i] ;
              if (data[i] > big) big=data[i] ;
         }
         scal=WIDTH/ (big- saall) ;
        for (i=1;i<=JP;i+ +) {
              n].im=(int) (0.&+ecals (data[i] -siaall)+EpS) ;
              pri小f ( '%4d 兀6. 2f ", i, data[i] );
              for (j= 1; j<=n1im+1; j++) printf ( "* ") ;
             printf ( "\ n') ;
        }
       printf ( "presa RETURN to continue . . .\n ") ;
        (void) getcharO;
       cosftl (data,JP-1) ;
       big = -1. 0110;
       small=l. oelO;
       for (i=1; i<=IP;i++) {
             if (data[i) < small) amall=data[i] ;
             if (data[i] > big) big=data[i) ;
       }
       scal=WIDTH/ (big- smail) ;
202        Numerica/ 尸eci戶es Examp旭 Bo아（

           for (i= 1; i< =NP; i++) {
               n1im=(int) (0. 5+ scal巾(data[ i] -small)+EPS) ;
               printf ( "%4d ", i) ;
               for (j= 1; j<=nhim+1; j++) printf ( "* ") ;
               printf ( "\ n") ;
           }
    }
    f ree_ ve ctor (data , 1, NP) ．·
    return 0;
}

    cosft2 carries out a cosine transform on a "staggered" grid. Its demonstration
                                                                              filled
program, xcosft2, is again the same as xrealft, except that the data array is
on the staggered grid points.
／卞 Driver 如r routine cosft그 +/

#include <stdio. h>
#include <math.h>
#include 'nr. h1'
#include '1nrutil. h "

#define EPS 1. 0e- 3
#define NP 16
#define WIDTH 30. 0
#define P1 3. 1415926

mi1t main(void)
{
      mnt i, j, nliin;
      float big, per, scal, small,中data;

      data=vector (1,NP) ;
      如r  ( ; ;) {
          printf ( "Period of cosine in ch띠l끄els (2-%2d) \n ', NP) ;
          scanf ( "/.f ", tper) ;
          if (per <= 0. 0) break;
          如r (i= 1 ; i<＝月P; i++)
                data［幻 =cos (2. 0中PI* (i- 0. 旬／per) ;
          co8f t2 (data, NP , 1) ;
           big = -1. 0al0;
           small=l. 0e10;
           for (i= 1; i< =NP; i++) {
               if (data[i] < small) small=data[i] ;
               if (data [ii > big) big=data[i] ,
            }
            scal=WIDTH/ (big- small) ;
            for (i= 1; i<=NP; i++) {
                n1im=(int) (0. 6+sca].*(data[ i] -small)+EPS) ;
                prmntf ( "%4d V.6. 2f ", i, data(i] );
                for (j= 1; j<=n1im+1; j++) printf ( "* ") ;
                prmntf ( ''\ n") ;
            }
            printf ( 'press RETURN to continua . . .\n ") ;
            (void) getcha工O,
            cosft2(data,且P, -1) ;
            big = -1. oelo;
                                                    Ch카）ter 12: Fast Fourier Transform   203
             smallrl. Oelo;
             如r (i= 1;i<＝月P; i++) {
                 if (dataCi] < small) small=dataCiJ;
                 if (dataLi] > big) big=data[i] ;
             }
             scal=WIDTH/ (big- small) ;
             for (i=1;i<=NP; i++) {
                 nhim=(int) (0. 5+scal* (dataCi] -small)+EPS) ,
                 printf ( "Y.4d ", i) ;
                 for (j=1; j<=nlim+1; j++) printf ( "*") ;
                 printf ( '\ n") ;
             }
         }
        tree_ vector (data, 11NP) ;
        return 0,
    }

     fourn is a routine for performing N-dimensional Fourier transforms. We have
used it in sample program xfourn to transform a 3-dimensional complex data array
of dimensions 4 x 8 x 16. The function analyzed is simply an array of random
                                                                               values.
The test conducted here is to perform a 3-dimensional transform and inverse transform
in succession, and to compare the result with the original array. Ratios are provided
for convenience. In the program, the 3-dimensional complex array is stored in a 1-
dimensional real array data2 as described in Numerical Recipes. The array datal is
a saved copy of data2 for the comparison at the end.
／中 Driver 如r routine tow口l 中／

#include <stdio . h>
#include "nr. h"
#include "nrutil. h"

#define NDIM 3
#define NDAT2 1024

mnt main(void)
{
        milt isign,
        long idu皿=(- 23) ;
        u끄signed long i, j, k, l, ndum'2, *nn;
        float *datal, *data2;

        nn=lvector ( 1 1 NDIM) ;
        datal=vector (1,NDAT2) ;
        data2=vector (1,NDAT2) ;
        for (i 'l; i<=WDIM; i++) nn[i] =(ndum <<= 1) ;
        for (i=1; i<=nn[3] ;i+ +)
            for (j=1; j<=nn[2] ;j+ +)
                  for (k"l; k<=nn[l] ;k++) {
                      1=k+(j- 1) *nn[1]+(i- 1)*nn[2J*nn[1] ;
                      l= (l <<l ) =l ;
                      /c real part of component */
                      data2 [1] =datal [1] =2*ranl (kidu皿)-1;
                      ／中 imaginary part of co工ponent 卞／
                      l+ + ;
                      data2 El] =datal [1] =2中ra끄1(* idu且）느1;
 204     Numerical Recipes Example Book

             }
    isign=l;
    fourn(data2 ,nn , NDIM, isign) ;
    ／本 h日ra 日ould be 카iy processing to be done in Fourier 아：1ace 中／
    isign = -1;
    fourn(data2,nn, NDIM, isign) ;
    printf ( "Double 3-dimensional tra끄sform\n\n") ;
    printf ( "%22s '/.24s Y.20s\n",
         'Double transf. ", "original data", "Ratio") ;
    printf ( "Y.lOs Y.13s '1.128 V.13s Y.lls %13s\n\n",
        "real " ,"lmag. " , "'r eal "' , "'i inag. ", ' 'r eal", "imag. ' ' ) ;
    for (irl; i<=4; i++) 'C
         k=2卓 (j =2卞i) ，·
         l=k+(j- 1汁nnll] + ( 느1) 卞nfl［幻 *nn[ j] ;
         1=(l<<1) -1;
         printf ( 'Y.12. 2f Y.12. 2f %10. 2f %12. 2f %14. 2f Y.12. 2f\ n",
             data2[l] ,data2[l+1] ,datal[ l] ,datal[ l+1] ,
              data2 [1] /datal Cl] , data2 [1+1] /datal [1+1] );
    }
    printf ( "\ nThe product of transform lengths is:         /.41u\n" ,nnCl] *im[2] *nn[3] );
    free1vector (data2, t, NDAT2) ;
    free_ vector (datal, i, NDAT2) ;
    free_lvector (nn, I 1NDIM) ;
    return 0;
}

     When your multidimensional data consists of real, rather than complex, values, it
is faster (and more e佈cient in memory use) to use an FFT routine that is optimized
for real data. rlft3 is such a routine. The main book already gives, at least in
outline, three sample programs using this routine. Here we content ourselves with an
example that simply fills a three dimensional real array with random values, performs
the Fourier transform followed by its inverse, and then verifies that (up to a known
constant multiplicative constant) the original matrix is recovered.
    The function compare is a simple utility for comparing all the values of an array
for equality with another array to within a certain tolerance (allowing for roundoff
errors). If the tolerance 0.0008 looks large to you, it is because we are comparing
numbers whose magnitude is as large as '-. 2 x iO3, so the fractional tolerance is
actually parts in iOd
/* Driver for routine r1ft3 巾/

#include <stdio.h>
#lnclude (math.h>
#include "nr. h"
#include "nrutil. h'1
#define IPRNT 20

static unsigned long compare (char *string, float ***arrl, float 牛**arr2,
    unsigned long leni, 山1signed long 1en2, 山lsigned long 1an3, float eps)
'C
    unsigned long err=0, i1, i2, i3;
    float al, a2;

    printf ( "I.s\n", string) ;
    for (i1=1; ii< =lenl; ii+ +)
                                               Cha아er 12: Fast Fourier Transform         205

        for (i2 "1; i2(=1en2; i2++)
            for (i3=1; i3< rlen3; i3++) {
                 al=a工rl [ii] [i2] [i3] .,
                 a2"arr2[ il] [i2] [i3] ;
                 if ( (a2 == 0. 0 && fabs (al- a2) > epa) I I (tabs ( (al- a2) /a2) > epa) ) {
                      if (++err <= IPRNT)
                          printf ( "Y.d Y.d %d Y.12.6f X12. 6f\ n",
                                   i1 1i2, i3, a1, a2) ;
                   }
             :1.
    retu그L err;
}

#define NX 32
#def mne 甘Y8
*define NZ 16

#define EPS 0. 0008

mnt main(void)
{
    long idum=(- 3) ;
    山lsigned long err, i, j, k1l, rm1=NX,nn2=NY,nn3=NZ;
    float fnorm, 卞卞中datal,＋卞李data2 1＋牛speql ;

    fnorm= (float) nnl* (f loat) nn2*(float) n沼/2 .0;
    datal=f3tensor (1,nnl, 1,nn2,1,nn3) ;
    data2=f3tensor (1,nnl, 1,nn2, 1,nn3) ;
    apeq1 'matrix(1,nn1,1,nn2<<1) ;
    如r (i=1; i<"I끄ii; i++)
         for (j=1; j<=nn2; j++)
              for (k=1;k<=nn3;k++)
                   data2[i] [j] [kj=fnorm*(datal[ i] 口] [k] =2*ranl (kidum) -1) ;
    r1ft3 (datal , speqi ,nnl, nn2,nn3, 1) ;
    /中 here would be any processing in Fourier space 卓/
    r1ft3 (datal, speql,nnl, nn2,nn3, -1) ;
    err=compare ( 'data", datal, data2,nnl, nn2,mi3,EPs) ;
    if (err) {
        printf ( "Comparison error at tolerance X12. 6f\ n", EPS) ;
        printf ( "Tota]. number of errors is 7.d\n", err) ;
    }
    else {
        printf ( "Data compares OK to tolerance V.12.6f\ n", EPS) ;
    }
    free_matrix (speql , 1,nnl , 1,nn2<<1) ;
    free_f 3tensor (data2, 1,nnl, 1,nn2, 1,nn3) ;
    free_ f 3tensor (datal, 1,nnl, 1,nn2, 1,n沼) ;
    return (err > 0) ;
}

    If your need to take the Fourier transform of a data set that is simply too long
to hold in your computer's memory, but which can be read from an external medium
such as a tape or disk, then the routine fourf S can be used. The following example
program creates a "pretend" such data set correspon小旽 的 a corn미炚月小m印前onal
array (it actually fits perfectly well into the arrays datal and data2), writes its first
half to one sequential file and its second half to another. fourfs is then called to
    206    八lume力C削尸ec徊es Examp旭 Book

take the the Fourier transform of the sequential files. To demonstrate that the correct
answer is obtained, we use the in-memory routine fourn to take the same transform,
and compare the answers.
    Note that, for multidimensional arrays, the output of fourf s is the transpose of
that from fourn. This is taken into account when the comparison is made.
     The example program then inverts the Fourier transform. Since we are starting
with the transpose of the inverse, the components of the array idim must be reversed
for fourfs, but restored for fourn. A final comparison of values is made.
／卞 Driver 如r routine 如urfs 方／/

#include <stdio.h>
#include <math. h>
#include "nr. h"
#include '1nrutil. h'1

#dafine SWAP (a,b) {iswap=(a) ; (a) =(b) ; (b)=iswap. }
#define FSWAP (a,b) {flswap= (a) ; (a)=(b) ;(b) =flswap; }

#define NX 8
#define NY 32
#define NZ 4
#define NDAT (2*NX*NY*NZ)

#define TEMPFILE1 'frfstmpl '
#define TEMPFILE2 "frfstmp2"
#define TENPFILE3 "frfstmp3"
#define TENPFILE4 "frfstmp4"

#if defined(MSDOS) I 1 defined(_MSDOS) I 1 defined(_MSDOS_ ) I I defined(_ .MSDOS_ _)
#define BINFtEADWRITE "wb+11
#else
#def ins BINREAD닙RITE "w+1'
#endif

char *fnames[4J= {TEMPFILE1 ,TEMPFILE2, TEMPFILE3,TE片PFILE4} ;

jot main(void)
{
      m1lt cc,nnv=3,nwrite;
      long idum= (- 23) ;
      unsigned long dim[4] .j, j, k, l, ll, jsvap;
      float diff, smax, s1m, sU皿1=o. o, sum2=O. o 1tot 1sdata1, *data2, *data1p, *data2p;
      FILE *f1swap1*file[ 5] ;

      data1=vector (1, 甘DAT) ;
      data2=vector (1,NDAT) ;
      dim[1] =NX;
      dim[2J=NY;
      diin[3J =NZ;
      如t= (float) NX卞 (float) N恥 (float 川Z;
      for (j '1; j<=4; j++)
          if ( (file Ej] =fopen(fnames[ j- 1] ,BINREADWRITE) ) == NULL)
               nrerror ( ''Conld끄 't open temporary file ') ;
      for (i=1; i<=dimC3] ; j++)
                                             C力a,pter j2: Fast Fourier 刀ans幻rm         207
      for (j= 1; j<=dim[ 2) ;j+ +)
          for (k=1;k<=dim[1) ;k++) {
               1=k+(j- 1) *dim[1]+(i- 1) *dimE2] *dim[1] ．·
               l= (1<<1) -1;
               data2 [1] =datal [1] =2*ranl (kidum) -1;
               1++;
               data2 [1] =datal [1] = 2*ra.n1(tidu皿) -1;
           }
 U日rite＝吼）AT >> I ;
  cc= fwrite (kdatal[1] ,sizeof (float) ,n口rite, file[ I] );
  if (cc != n日rite) nrerror ( "write error in xfourfs") ;
  cc=f日rite (&datal[nwrite+1J ,sizeof (float) ,n口rite, file[ 2] );
 if (cc != nvrite) nrerror ( "vrite error in xfourfs ") ;
 re日ind(file 口n ;
 re日ind(file ［刃 ) ;
 printf ( "                           doing fourfs 卞*卞卞卞中京卞卞＼n' ) ;
 fourfs (file, dim,nnv, 1) ;
 for (j= 1; j<=4; j++) rewind(file[ j] );
 cc=fread(kdatal[l] ,sizeof (float) ,n日rite, file[ 3J) ;
 if (cc != nwrite) nrerror ( "read error in xfourfs '') ;
 cc=fread(kdatal[nwrite+lJ ,sizeof (float) ,n日rite, file[ 4] );
 if (cc != nwrite) nrerror ( "read error in xfourfs") ;
printf ( "                            如ing 如urn 卞*卞方卞中卞卞卞＼n') ．·
 fourn(data2,dim,nnv,1) ;
 sum=smax=0 .0;
如r (i '1 ; i<=dim［幻 ; i++)
       for (j '1; j<=dim[2] 口++)
            for (k=I; k<=dim[lJ; k++) (
                l=k+(j 叫1) 妃im口J+(j- i) 妃im[2J*虹mCi] ;
                l= (l <<l )1l ;
                ll= i+ (j- 1) 中dim[3] +(k-1) 中di皿［3]巾dim[2] ;
                11=(ll< <i) -i;
                diff= sqrt (SQR(data2[ll] -datal[ l] )+SQR(data2[ll+ 1卜datal口+i] ));
                sum2 += SQR(datal Cl] )+SQR(datal [1+1] );
                so皿 += diff;
                if (diff > smax) smax=diff;
           }
su皿2=sqrt (su皿2/tc't) ;
sum=sum/tot;
 printf ( " (r. m. s. ) value, (ma工, ave) discrepancy= V.12.7f 工12.7f Y.12.7f\
                                                                               n",
      su皿2 , sma工 , sum) ;
 /* now check the inverse transforms */
 SWAP (dim[1] ,dimC3] );
 /s This step swap step is conceptually a reversal, but for
 three dimensions a swap accomplishes that. */
FSWAP(file[ 1] ,fi1eE3] )
FSWAP (file ［幻 . file ［幻 )
for (j= 1; j<=4; j++) re日ind(fileCj] );
printf ( " 字京中卓字*卞李卞*5卒* 巾卞卓 now doing fourfs               \n") ;
如町如 (file, dim,nnv, -1)
                              ..
for (j= l; j<=4; j++) revind(fileCj] ),
cc=fread (kdatal[1] ,sizeof (float) ,n日rite, file[ 3] );
if (cc != n日rite) nrerror ( "read error in xfourfs ") ;
cc=fread(&datalfn日rjt日+i] ,sizeof (float) ,n日rite, fi1eE4] );
if (cc != n日rite) nrerror ( 'read error in xfourfs") ;
SWAP (dim［幻 , d끄5 [3] ) ;
printf ( '                         doing fourn            \n") ;
208        Numerical Recipes Example Book

    如urn(data2, dim,nnv, -1) ;
    swn= sma工＝0 .0 ;
      datalp=datal;
      data2p=data2;
      for (j=1; j<=NDAT; j+=2) {
          8O皿l += S叭（data2p[1] )据叭（data2아幻 ) ;
          diff= sqrt (SQR (data2p [1] -dataip [1] )+SQR(data2p [2] -dataip [2] ));
          sum += diff;
          if (diff > sma幻 smax=diff;
          dataip += 2;
          data2p += 2;
      }
    8Om= sum/tot;
    s山nl=sqrt (suml/tot) ;
    printf ( " (r. m. s. ) value, (max, ave) discrepancy= %12. 7f %12. 7f 工12. 7f\ n",
         8山iii , sma工 , su皿）;
    printf ( "ratio of r. m. s. values, expected ratio= '/.12. 6f '/.12.6f\ n"",
         suxnl/ sum2, sqrt (tot) );
    for (j=1; j<=4; j++)
        if (fclose (file[ j] ) == EOF) nrerror ( "Couldm't close temporary file ") ;
    free_ vector (data2, 1,NDAT) ;
    free_ vector (datal, 1 ,NDAT) ;
    for (j=1; j<=4; j++)
         if (remova (fnames[ j- 1] )) nrerror ( "Couldn 't delete temporary file ') ;
    reti丘n 0;
}
 Chapter 13: Fourier and Spectral Applications

         Chapter 13 of Numerical Recipes covers mainly Fourier transform spec-
     tral methods, particularly the transform of discretely sampled data. Two
     common uses of the Fourier transform are the convolution of data with a
    response function, and the computation of the correlation of two data sets.
     These operations are carried out by convlv and correl respectively. Other
    ap可ications of Fouri町 method釘n the ma加 boo뉘nc加de data 月九en碼 p아ver
    spectrum estimation (spctrm, or evlmem with memcof), and linear prediction
    (predic with fixrts and memcof). For power spectrum estimation of un-
    evenly sampled data, you can use period, or its "fa就" cousin for large data
    sets, fasper. An application with a somewhat different flavor is the high
    accuracy computation of Fourier integrals with dftint. Finall.y, we provide
    routines for wavelet transformns: wt 1 for a one-dimensional wavelet transform,
    vtn for a multidimensional wavelet transform, and (in daub4, pwtset, and
    pwt) a small selection of wavelet filters, out of which the wavelets themselves
    are constructed.



    Procedure convlv performs the convolution of a data set with a response function
using an FFT. Sample program xconvlv uses two functions that take on only the
values 0.0 and 1.0. The data array data[ij has sixteen values, and is zero everywhere
except between i=6 and i=10 where it is 1.0. The response function respns[i] has
nine values and is zero except between i=3 and i=6 where it is 1.0. The expected
value of the convolution is determined simply by flipping the response function
                                                                                 end-
to-end, moving it to the left by the desired shift, and counting how many non-zero
channels of respns fall on non-zero channels of data. In this way, you should be able
to verify the result from the program. The sample program, incidentally, does the
calculation by this direct method for the purpose of comparison.
/s Driver for routine convlv */

#include <stdio . h>
#include "ni .h"
#include "nrutil. h"

#define N 16           ／卞 data array size 卞／
*define M 9            /* response function dimension - must be odd *1
#def ins 月2 (2卞月）

mnt main(void)
{
    unsigned long i, j;



                                                                                 209
    210    Numerical Recipes Example Book

      mllt isign;
      fl oat cap,卞dat키Cr86恥is,巾re町I.卞帥a;

      data=vector (1, 甘) ;
      re町'I田＝vec切r (1,N) ;
      resp=vector (1,1) ;
      ans=vector ( 1,1(2) ;
      for (i=1; i<=N; i++)
          if ( (i >= 三/2-1/ 8) && (i <= 1/ 2+1/ 8) )
               data[i] =1.0;
           else
               data[i] =0.0;
      for (i= 1; i<=M; i++) .(
          if ( (i > 2) && (i < 7))
               re町n8［幻 =1.0;
          else
               respns[i) =0.0;
          resp[i] =respns[ij ;
      }
      isign=l;
      convlv(data,N.resp,M, isign, ans) ;
      /* compare with a direct convolution 수/
      printf ( '%3s %14s %13s\n", "i ", "CONVLV ', "Expected") ;
      for (i=1; i<=N; i++) {
          cmp=0 .0;
          for (j=1; j<=1/2; j++) {
              cap += data( ( (i- j- 1+N) Y, N)+1] *respns[ j+1] ;
              cap += data[ ( (i+ j- 1) % 丑) +1] *respns[M- j+1] ;
          }
          cmp += dat缸口수respns口L
          printf ( "%31d 工15. 6f %12. 6f\ n", i, ans[i] ,cmp) ;
      }
      free_ vector (ans,1,12) ;
      free_ vector (resp,1,1) ;
      free..vector (respns, 1,月) ;
      free_vector (data,1, 月) ;
      return 0;
}

    correl calculates the correlation function of two data sets. Sample program
xcorrel defines datal Li] as an array of 64 values that are all zero except from
i=25 to 1=39, where they are one. data2 Li] is defined in the same way. Therefore,
the correlation being performed is an autocorrelation. The sample routine compares
the result of the calculation as performed by correl with that found by a direct
calculation. In this case the calculation may be done manually simply by successively
shifting data2 with respect to datal and counting the number of nonzero channels
of the two that overlap.

／方 Driver for routine corr缸 卞／

#include <stdio.h>
#include "nr. h"
linclude "nrutil. h1'

*define 奸 64
#define (
        12 (2*1)
                                          Ch叩旭r 13: Fourier and S／그ectral k刃／'cat幻／iS   211

    mllt 1 ain(void)
    {
         unsigned long i, j;
         float cmp *datal, *data2, *uns;

         data1'vector (1,N) ;
         data2"vector (l ,N) ;
         ans=vector (1,N2) ;
         for (i= 1;i<=N; i++) {
             if ( (i > 丑／2-月／8) kk (i < N/2＋月／8) )
                  dataltj] =1. O;
             else
                 datal[ i] =0. O;
             data2 [i卜datal［幻 ;
         }
         correl(data1.data2 1N, ans) ;
         /巾 Calculate directly 卞/
         printf ( "%3s %14s 7.18s\n", 'n", "CORREL' , 'direct calc. ") ;
         for (i= 0; i<=16;i+ +) {
             clsp=O. O;
             for (j=1; j<=N; j++)
                   cap += datal[ ( (i+ j- 1) % N)+1] *data2 (jl;
             printf ( '%31d 工15. 6i %1S. 6f\ n". i, ans (i+l] ,cmp) ;
         }
        free_va比or (ans 1 1 小2) ;
        free_ vector (data2,1IN) ;
        free_ vector (datal 11,N) ;
        rett口：
             n 0;
}

    spctrm does a spectral estimate of a data set by reading it in as segments, win
dowing, Fourier transforming, and accumulating the power spectrum. Data segments
may or may not be overlapped at the decision of the user. In sample program xspctrin
the spectral data is read in from a file called spctrl .dat containing 1200 numbers
and included on the diskette. It is analyzed first with overlap and then without. The
results are tabulated side by side for comparison.
/* Driver for routine spctrm 卞/

#include <stdio .h>
#include <stdlib. h>
#include 'nr. h1'
#include "nrutil. h"

#define M 16
#define TRUE 1
#define FALSE 0

mllt main(void)
{
        jut j. k, ovrlap;
        float; 柱hm;
        FILE *fp;

        p=vector (1,N) ;
    212              Numerica/ 尸ec徊es Examp旭 Book

          q=vector (1,N) ;
          if ( (fp = fopen( "spctr1.dat ' , 'r ') ) == NULL)
               nrerror ( "Data file spctrl. dat not found\n") ;
          k=8;
          ovrlap=TRUE;
          spctrm(fp,p,fl, k, ovrlap) ;
          revind(fp) ;
          k=16;
          ovrlap=FALSE;
          spctrm(fp ,q,M,k, ovrlap) ;
          fclose(fp) ;
          printf ( "\ nSpectrum of data in file spctrl. dat\n') ,
          printf ( "7.13s %s %55 %s\n", " " , "overlapped ", " ", "non-overlapped') ;
          for (j=1; j<=M; j++)
               printf ( 'Y.3d %ss Y.13f %5s %13f\n", j ," " ,p[ j] ," ", q[ j] );
          free_ vector (q, 1,M) ;
          free_ vactor (p. 1,M) ;
          return 0;
}

    memcof is used in two different capacities in Numerical Recipes. In combination
with evlmem it is used to perform spectral analysis by the maximum entropy method.
memcof finds the coefficients for a model spectrum, the magnitude squared of the in
verse of a polynomial series. Sample program xmemcof determines the coefficients for
1000 numbers from the file spctrl .dat and simply prints the results for comparison
to the following table:
Coefficients for spectral estimation of spctrl. dat
 a[ 1] =    1. 261539
 a[ 2] =   -0. 007696
 a[ 3] =   -0. 646778
 a[ 4] =   -0. 280603

    J m
    m
    1 J mJ m J 1
           J m 1
               J 0
            0. 163693                                                                   =




    5 6 n/ 8 9 0 a
                                                                                        =
            0. 347674
                                                                                        =
            0. 111247
               l
                                                                                        =
           -0. 337141
    [ [ PL [ [ [
                                                                                        =
           -0. 358043

    a a a a a a
                                                                                        =
            0.378774
                                                                                        =
            0. 003511

／卞 Driver 如r routine m日mcof 卓／

#incl工de <stdio.h>
#include <stdlib.h>
#include 'nr. h"
#include "nrutil. h"

#define N 1000
#define M 10

ml1t main(void)
{
     mllt i;
     float pm.卞cof, 本data;
     FILE *fp;
                                        Ch카）旭r 13: Four旭rand Spec打可Ap川C카幻ns       213

      cof=vector (1,M) ;
      data=vector (1,N) ;
      if ( (fp = fopen( "spctrl. dat ", "r ") ) == NULL)
          nrerror ( "Data file spctrl. dat not found\n") ;
      for (i= 1; i<=甘; i++) fscaitf (fp, " 工f ", tdata[i] );
      fclose(fp) ;
      memcof (data,N,M 小pm, cof) ;
      printf ( 'Coefficients for spectral estimation of spctrl. dat\n\n") ;
      for (i=1; i<=M; i++) printf ( "a[Y.2d] = 工12. 6f \n", i, cof[i] );
      printf ( "\ nao =%12. 6f\ n", pm) ;
      f ree_vector (data11,N) ;
      free_v吼如r (cof, 1,M) ;
      return 0;
}

    Although evimem appears later in Chapter 13, we show its sample program here,
because it is so closely tied to the previous program. evl皿ein uses coefficients from
memcof to generate a spectral estimate. The example xevlmem uses the data from
spctrl.    dat and prints the spectral estimate. You may compare the result to:

    Power spectru皿 estimate of data in spctrl. dat
        f巾delta         po日er
        0. 000000    0.026023
        0. 031250    0. 029266
        0. 062500    0.193087
        0. 093750    0. 139241
        0. 125000  29. 915518
        0.156250     0.003878
        0. 187500    0.000633
        0. 218750    0.000334
        0. 250000  - 0.000437
        0. 281250    0.001331
        0.312500     0.000780
        0.343750     0. 000451
        0. 375000    0. 000784
        0. 406250    0. 001381
        0.437500     0. 000649
        0.468750     0.000775
        0.500000     0.001716

／卞 Driver 如r roi工tine ev].mem 卞／

#include <stdio . h>
#include <stdlib. h>
#include "nr. h"
#include "nrutil. h "

*define N 1000
#define K 10
#define NFDT 16

mllt main(void)
{
       mnt i;
       float fdt, pm, *cof, *data;
       町LE 字fP;
    214     Numerical／相（加es Exa／까,le Book

      cof=vector (1,M) ;
      data=vector (1,N) ;
      if  ( (fp = fopen( 'spctrl. dat ", 'r ') ) == NULL)
           nrerror ( "Data file spctrl. dat not found\n") ;
      for (i 'l; i<=N; i++) fscanf (fp, "%f ", &data[i] );
      fclose(fp) ,
      memcof (data，瓦瓦缸si, cot) ;
      printf ( "Power spectusi estimate of data in spctrl. dat\n") ;
      printf ( "       f* delta        pover\n") ;
      for (tdt=O. O; fdt<=O. 5; fdt+=O. 5/甘p1.)T)
           printt ( "Y.12. 6f X12. 6t\ n", fdt, evlm이n(fdt, cof,M,psi) );
      f ree_ vector (data 1 1, N) ;
      free_ vector (cof .1,10;
      return 0;
}

    Notice that once memcof ha.s determined coe佈cients, we may evaluate the estimate
at any intervals we wish. Notice also that we have built a spectral peas into the noisy
data in spctrl.dat.
    The second use of memcof is to perform linear prediction in combination with
predic and fixrts. memcof produces the linear prediction coe佈cients from the
data set. fixrts massages the coefficients so that all roots of the characteristic
polynomial fall inside the unit circle of the complex domain, thus insuring stability
of the prediction algorithm. Finally, predic predicts future data points based on
the modified coefficients. Sample program xfixrts demonstrates the operation of
fixrts. The coefficients provided in the array d[i] are those appropriate to the
polynomial (z - 1)6 = 1. This equation has six roots on a circle of radius one,
centered at (1.0, 0.0) in the complex plane. Some of these lie within the unit circle
and some outside. The ones ou-tside are moved by fixrts according to zi -* 1/z .
You can easily figure these out by hand and check the results. Also, the sample
routine calculates (z - 1)6 for each of the adjusted roots, and thereby shows which
have been changed and which have not.
1卞 Driver for routine fixrts          *1

#include <stdio .h>
#include "nr. h"
#inclnde "complex.h'

#define NPOLES 6
#detine NPI (NPOLES+1)
#def ins ONE Complex(1.O,0. O)
#def ins TRUE 1

mllt main(void)
{
      ml1t i ,polish=TRUE;
      static float 虹甘Pi] =
           {o . O, 6.O, -15.0,20 . 0, -1S.0,6.0,0 . 0} ;
      fcomplex zcoaf[NPI] ,zeros[NP1] ,zl, z2;

      /* finding roots of (z-1.0Y6=1. O */
      ／中 first 日rite roots 巾／
      zcoef DIPOLES] =ONE;
                                         Ch햐ter 13: Fourier arid Spectral Applications   215
        for (i=NP0LES-1; i>=0; i- -)
            zcoef[i] = Complex (卞dENPOLES-i) ,0.0) ;
        zroo出（zcoef ,NPO比S ,zeros ,poli帥口 ;
        printf ( 'ftoots of (z-i. 0) 6 = l. 0\n" ) ;
        printf ( "Y.24s Y.27s \n". "1oot ", ' (z-1.0Y6 ") ;
        for (i=1; i<=NP0LES; i++) {
            zl=Csub(zeros[i] ,ONE) ;
            z2=Cmul(zl 1z1) ;
            zi=Cmul(zl, z2) ;
            zl=Cmul(zi, zl) ;
            printf ( "Y.6d %12. 6f %12. 6f %12. 6f %12. 6f\ n' ,
                  i, zeros[i] .r, zeros[i] .i, zi. r, zi. i) ;
        }
         /* now fix them to lie within u끄it circle */
         fixrts (d,NPOLES) ;
        ／京 check results 本／
         zcoef [NPOLES] =ONE;
         for (i 'NP0LES-1; i>=0; i- -)
              zcoefCi] = Comple工(- d[NPOLES-i:l ,O. O) ;
         zroots(zcoef ,NPOLES, zeros ,polish) ;
        printf ( "\ nRoots reflected in unit circle\ n") ;
        printf ( "%24s %27s \n", "Root ", " (z-1. 0Y6") ;
        如r (i=1; i<＝朴口LES; i++) {
              z1=Csub (zeros[i) ,DNE) ;
              z2=Cmul(z1,z1) ;
              zl=Cmul(zl, z2) ;
              z1=Cmul(zl, zl) ;
             printf ( "%6d %12. 6f 工12. 6f Y.12.6f Y.12.6f\ n",
                  i, zeros[i] .r, zeros[i] .i, zl. r, zl. i) ,
        }
        return 0;
    }

        predic carries out the job of performing the prediction. The function chosen for
    investigation in sample program xpredic is

             F (n) = exp(- n/npts) sin(2irn/50) + exp(小2n/npts) sin(2.2兀n/50)

the sum of two sine waves of similar period and exponentially decaying
                                                                          amplitudes.
On the basis of 500 data points, and working with coefficients representing
                                                                            ten poles,
the routine predicts 20 future points. The quality of this prediction may be
                                                                               judged
by comparing these 20 points with the evaluations of F (미 that are provided.
1* Driver for routine predic */

#include <stdio . h>
#include <math.h>
#include "nr. h'1
*include 11nrutil. h"

#define NPTS 500
#define NPOLES 10
*define NFUT 20
#define P1 3.1415926

float f (int n, int npts)
{
216        Numerica／尸BC徊es Examp旭 Book

      return exp(- (1.O*n) /npts)*sin(2. osPlsn/50.0)
          +exp(- (2.0*n) /npts)*sin(2. 2*PI*n/50.0) ;
}

jut main(void)
{
    mllt i;
    float du皿14d1卞future1京data;

      d=vector (1. 1POLES) ;
      ！吼ure=vector (1 WFL月）;
      data=vector (1,NPTS) ;
      for (i=1; i<=NPTS; i++)
            data[i] =f (i, NPTS) ;
      memcof (data,NPTS ,1P0LES小iui , d) ;
       fixrts (d,NPOLES) ;
      predic(data,N?TS,d,NPOLES, future,NFUT) ;
                                                       1IC") ;
      printf ( "%6s Y.lls %12s\n", "I ", "Lctual" ,"PR日：
       for (i=1; i<=NFUT; i++)
            printf ( "Y.6d %12. 6f %12.6f\n" 山f (i+IPTS,IPTS) ,future[i] );
       free_vector (data, 1,WPTS) ;
       free_vector(future,11NFUT) ;
       free_vector (d,1,NPOLES) ;
       return 0;
}
                                                                                 miss-
     Spectral analysis of unevenly sampled data, or of evenly sampled data with
                                                                 constructs the Lomb
ing values, can be performed by the routine period, which
                                                                                    of
normalized periodogram. In the following example, we construct a data array
length 90 that consists of a regular sampling of length 100 with 10 (random) dele-
tions. The sampled function is a pure cosine, plus Gaussian white noise of somewhat
                                                                                signal
larger amplitude. A call to period yields the significance level with which the
is found to be non-Gaussian (very significant in this case!), and the output spectrum.
 We print out a few values in the neighborhood of the largest peak found. You can
 verify that the peak is indeed nicely centered on the frequency of the input cosine.
 /巾 Driver for routine period */

    #include <stdio. h>
    *include <math.h>
    #include "nr.h'1
    #include '1nrutil.h"

    #define 甘P 90
    #define NPR 11
    #defina TWOPI 6.2831853

    jut main(void)
    {
        如ng idu皿＝(- 4) ;
        jut j=0, jmax,n,nout;
        float prob,卞P工1卞py. 卞X1中y;

        x=vector (1,NP) ;
        y=vector (1,MP) ;
        P工＝vector (1,2卞甘P) ;
                                     Ch카가er 13: Fou片針and Spec打削Ap;川ca打이iS       217
     py=vector (1,2*NP) ;
     for (n=1; n<=NP+10;n++) {
         if Co ' = 3 k立n ! = 4 &kn ! = 6 &&n ! = 21 &在
             n != 38 kk n ! = 51 &k ii ! = 67 立& n ! = 68 &&
             n '= 83 && fl ! = 93) {
              X +J][+
                      ;       =1l
              叭刃 =0. 75卞cos (0. 6卓工口] )+gasdev（缸dun) ;
         }
     }
    period(x, y, j, 4. 0,1. 0,px,py, 2*NP,立nout,立jniax,kprob) ;
    printf ( 'period results for test signal (cos (0. 6x) + noise) :\n ") ;
    printf ( "nout, jmax,prob=/.d Y.d V.12. 6g\n' , nout, jmax,prob) ;
    for (n=LMAX (1, jmax-NPR/2) ;n<=LMIN(nout jmax+NPR/ 2) ;n++)
        printf ( ' /.d %12. 6f %12. 6f\ n", n, TWOPI*px[n] ,py[n] );
    free_ vector (py, 1, 2*NP) ;
    free_ vector (px, 11 2*NP) ;
    free_ vector (y, 1 ,NP) ;
    free_ vector (x, 1, NP) ;
    return 0;
}

     The routine fasper has the same capabilities as period, but performs its under-
lying calculations using FFT routines. For large data arrays, fasper is very much
faster than period. Here, we give a demonstration program that is closely equivalent
to tile one given for the previous routine. About the only difference is that fasper
requires a larger workspace, here 4096, onto which it "extirpolates" the given data,
as described in the main book.
／中 Driver 如r rout in日 fasper +/

#include <stdjo.h>
#include <math. h>
#include "nr. h"
#include "nrutil. h1'

#define NP 90
#define MP 4096
#define NPR 11
#define TWOPI 6. 2831853

mllt main(void)
{
    long id山n=(- 4) ;
    unsigned long y0, jmax,n,nout;
    float prob，싸）x *py，京X1京y;

    x=vector (1,NP) ;
    y=vector ( 1, NP) ;
    px=vector (1,NP) ;
    py=vector (1,MP) ;
    for (n=1;n< =NP+10; n++) {
        if (n ! = 3 立立 n ! = 4 立立 n ! = 6 立立 n 1 = 21 &立
            n 1 = 38 立立 n ! = 51 && n 1 = 67 &在 n ! = 68 &&
            n 1= 83 && ll 1 = 93) {
             X +J]
              [+
                        ;
                        =1l
             y Ci그 =0. 75牛cos (O. 6卒x 口］)+gasdev（立idum) ;
 218         Numerica／月e뎨7es Examp旭Book

             }
    }
    fasper (x, y, j, 4.0,1.0,px,py,MP,&nout,kjma工,&prob) ;
    printf ( "fasper results for test signal (cos (O. 6x) + noise) :\n ") ;
    printf ( 'noutjma工,prob=/.ld %ld %12. 6g\n" , nout, jmax,prob) ;
    for (n=LMAX (1, jma工-NPR/2) ;n<=LMIN(nout, jmax+NPR/2) ;n++)
        printf ( "%ld X12. 6f 工i2. 6f\ n" ,n, TWOPI*pxEn] ,py[nl) ;
    free_ vector (py,1,川P) ;
    free_vector (px.1 1MP) ;
    free. vector (y. 1,NP) ;
    free_ vector (x, 1 1NP) ;
    retm口l0;
}

    We test dftint on the integrals


        f6
                 cos(cx『d) coswx』       ，)’吼 ""[（붊，‘: ),: ' 可］,“
                               ：寸'"[（늙，“少
        尸s(cx+d)s［岫＝[- ""'[（旨’
                            ，c)x‘미 """[（，‘
                                        늙:):, ' 끼‘，
                                               2((i- c)            2(w+ c)      j,

where W / 士c. Sample program xdftint prompts for values of c, d, a, b and w. It
then compares the results of dft jut with the analytic values of the integrals.
／方 Driver 如r routine dftint     卞／

#include <stdio . h>
#include <math.h>
#inclnde "nr. h11

static float c,d;

float cosc工d(float 工）
{
    return cos (c卓工＋d) ;
}

#def in日 ci (x) 佃in( (w尸C汁卜키八2. 0*（十c) )+sin(佃妃汁工＋d) /(2. 0京（小c) ))
#define si (x) (- cos( (w-c)枉크）/(2. 0字（日-c) )-cos(（日＋c) *工＋d) /(2. 0s（口＋c) ))

void getans(float w, float a,float b, float *c띠ls, float S sans)
{
    卞ca끄5=ci (b)-ci (a) ;
    卞sans=si（功-Si佃）;
}

ml1t iuain(void)
{
    float a,b, c카is ,cosiflt, safl티Sinint,日；

    printf ( " Omega Integral cosiue*test func Err ") ;
    printf ("      Integral sine字test func       Err\ n") ;
    for C; ;) {
        printf ( 'input c,d: \n") ;
        if (sc키lf ( ' '/,f %f ", kc,kd) == EOF) break;
        如r (; ; ) {
                                        Cha拍9r 13: Fourier and Spectral Applications   219
                printf ( "input a,b: \n') ;
                if (scanf ( "Y.f Y.f ", &a,&b) == EOF) break;
                if (a == b) break;
                    for C; ;) {
                          printf ( 'input w: \n') ;
                          if (scanf ( "Y.f ", &w) == EOF) break;
                          i f (w < 0.0) break;
                          dftint (coscxd, a,b, w,kcosint,&sinint) ;
                          gets工田佃 , a巾，Ac카is,ksans) ;
                          printf ( 'Y.15. 6e 7,15.6e V.15.6e Y.15. 6e V.15.6e\n' ,
                               w, cans, cosint小cans, sans, sinint- sans) ;
                    }
           J.
       }
       printf ( "normal completion\n") ;
       return 0;
:1,

     The wavelet transform routine uti can be used either with the lowest-order
 wavelet filter, as provided by daub4, or else with the higher-order filters provided
 by the combination of pwtset and pwt. The following sample program allows
                                                                                    for
 both possibilities by prompting for the input order as k. For k = -4 the program
 uses daub4, while for k positive it uses pwtset (k). Also prompted for is a quantity
 frac: The program computes the wavelet transform of a function consisting of a
parabolic "bump" on an otherwise zero background. It then truncates the wavelet
transform to zeros, except for a fraction frac of the components. After reconstructing
 the function from the truncated data with an inverse wavelet transform, it finds the
maximum deviation between the original function and its approximate reconstruc
tion. One finds that with a comparatively small number of wavelet components, one
is able to reconstruct the original bump to very good approximatio
                                                                    n.
/s Driver for routine wtl */
#include <stdio . h>
#include <math.h>
#include "nr. h'1
#include "nrutil. h"

#define 月甘AX 512
#def ins NCEN 333
#define NVID 33

ml1t main(void)

      unsigned long i, nused;
      mllt itest, k;
      float 中U, *V, 京日，frac, thr日sh, tmp;

      u=vector (1,NMAX) ;
      v'vector (1,NMAX) ;
      日＝vector (1,N甘Ax) ;
      如r ( ; ;) {
          printf ( 'Enter k (4, -4, 12, or 20) and frac (0.0 to 1.0) :\n ') ;
          if (scanf ( '%d 工f " ,kk,kfrac) == EOF) break;
          frac=FMIN (1. 0,FMAX (0.0,frac) );
          1如引＝住 == -4 ? 1 : 0) ;
220       Numerica／尸e아）es Examp旭 Book

          if (k < 0) k = -k;
          if (k != 4 U k != 12 && k != 20) continue;
          for (i=1; i<=NMAX; i++)
              日［幻＝V［幻=(i > 甘CEN-NWID U i < 丑CEN+NWID ?
                                                                               0. 0) ;
                     ( (float乂卜恥EN＋甘WXD) *(float) （甘CE片＋뀨WI小i) )/(NWID京NWID) :
          if (! itest) pwtset (k) ;
          vtl (v. NMAX,1,itest 9 daub4 : pwt) ;
          for (i=1; i<=NMAX; i++) u[ i] =fabs (v[ ij) ;
          thresh=select ( (int) ( (1.0-frac) *NMAX) ,NMAX,u) ;
          nused=0;
          for (i=1;i<＝甘MAX; i++) {
              if (fabM吐幻 ) <= thresh)
                   v[i] =0. 0;
               else
                   nused++;
         }
         日tl(v, 甘MAX, -1,itest ? daub4 : pvt) ;
         for (thresh=0 .01i=1; i<=甘MAX; i++)
             if ( (tmp=fabs (v[ i] -w (i] )) > thresh) thresh=tmp;
         printf ( 'k, NMAX,nused= %d V.d %d\n", k, NMAX,nused) ;
          printf ( "discrepancy= %12. 6f\ n", thresh) ;
      }
      free_ vector (v, 1,NMAX) ;
      free나vector (v, 1,NMAX) ;
      free_ vector (u, 11NMAX) ;
      return 0;
}
                                                                                    set
     As an example of using wtn, the n-dimensional wavelet transform routine, we
up the two-dimensional matrix   described in the caption to Figure 13.10.5 of Numerical
Recipes, then take its wavelet transform (using the DAUB12 wavelet), then undo the
transform and show that the original matrix is recovered. In real applications, of
course, what matters is what we have left out: processes that would be applied
to the matrix while it is in wavelet space. The simplest such process would be
truncation, encoding, and transmission of the matrix in a wavelet-compressed form,
for reconstruction at another location. Another kind of process would be truncation
followed by some operations of linear algebra optimized for the now-sparse form.
／卓 Driver for routine 日tn 中／
Ninclude <stdlo . h>
#inc].ude <math.h>
#include "nr. h"
#include "nrutil. h11

#define EPS 1. oe-06
#define NX 8
#define NY 16

mnt rnain(void)
{
      unsigned long i口 ,l. nerr0r=0,ntot=NX*甘Y;
      float 卓a, 中aorg;
      static unsigned long ndim[]={0,NX, NY} ;

       aorg=vector (1,ntot) ;
       a"vector (l ,ntot) ;
                                   Chapter 13: Fourier and Spectral Applications    221
    pwtset (12) ;
    for (i=1; i<'NX; i++)
         for (j=1; j< rNY; j++) {
             lri+ (j- 1) *NX;
             aorg[1J=a[1] =(i == J ? -1. 0 : 1. 0/四rt (fabs ( (float) (i- j) )));
         }
    wtn(a,ndim, 2, 1,pvt) ;
    7* here, one might set the smallest components to zero, encode 카ld transmit
    the remaining components as a compressed form of the "image " */
    wtn(a,ndim, 2, -1,pwt) ;
    for (lr1 ;l< =ntot;l+ +) {
        if (fabs (aorgEl] -a[1] ) >= EPS) {
            printf ( "Compare Error at element '/.ld\ n", l) ;
            nerror++;
        }
    }
    if (nerror) printf ( "Nuinber of comparision errors: '/.ld\ n", nerror) ;
    else printf ( "transform-inverse transform check OK\n"') ;
    free_ vector (a, 1,ntot) ;
    free尸vector (aorg, 1,ntot) ;
    return nerror;
}
Chapter 14: Statistical Description of Data

       Chapter 14 of Numerical Recipes covers the subject of descriptive statis-
  tics, the representation of data in terms of its statistical properties, and the
  use of such properties to compare data sets. We start with a procedure to
  characterize data sets: moment returns the average, average deviation, stan-
  dard deviation, variance, skewness, and kurtosis of a data array.
      Most of the remaining procedures compare data sets. ttest i:ompares
  the means of two data sets having the same variance; tutest does the same
  for two sets having different variance; and tptest does it for paired samples,
  correcting for covariance. ttest is a test of whether two data arrays have
  significantly different variance. The question of whether two distributions
  are different is treated by four procedures (pertaining to whether the data is
  binned or continuous, and whether data is compared to a model distribution
  or to other data). Specifically,
        7.
             chsone comnpares binned data to a model distribution.
   2.
             chstwo compares two binned data sets.
   3.
       ksone compares the cumulative distribution function of an unbinned data
       set to a g加en funct幻n.
    4. kstwo compares the cumnulative distribution functions of two unbinned
             data sets.
       The next set of procedures tests for associations between nominal vani-
   ables. cntabl and cntab2 both check for associations in a two-dimensional
   contingency table, the first calculating on the basis of x2, and the second
   by evaluating entropies. Linear correlation is represented by Pearson's r, or
   the linear correlation coe伍cient, which is calculated with routine pearsn.
   Alternatively, the data can be investigated with a nonparametric or rank con-
                                                                               r
   relation, using spear to find Spearman 's rank correlation r8. Kendall's
   uses rank  ordering of ordinal data to test for monotonic correlations. kendil
   does this for two data arrays of the same size, while kendl2 applies it to
   contingency tables.
                                                                           ks2dls
        We provide two procedures for testing two-dimensional data sets.
                                                                                 n
   per forn招 a)白加mogorov-鈿小nov te就 of data toag加en mo（伺 (gener키切atio
   ofksone), while ks2d2s does  the same  for testing one data set against another
   (generalization of kstwo).
       One final routine savgol makes no attempt to describe or compare data
   statistically. It calculates Savitzky-Golay smoothing coefficients that can be
   used to smooth out statistical fluctuations, usually for the purpose of visual

 272
                                            Gb햐升er 14: Stat台tical Description 可Da治            223
        presentation.




         Procedure moment calculates successive moments of a given distribution of data.
    The example program xmoment creates an unusual distribution, one that has a sinu
    soidal distribution of values (over a half-period of the sine, so the distribution is a
    symmetrical peak). We have worked out the moments of such a distribution theoret
    ically and recorded them in the program for comparison. The data is discrete and
    will only approximate these values.
    /* Driver for routine moment */

 #include <stdio . h>
 #include <math.h>
 #include "nr. h"
 #incl끄de "on比il . l111

 #define PT 3. 14159265
 #define NPTS 5000
 #define 甘BI甘 100
 #define NPP月B （川,TS＋丑町甘）

 mllt main(void)
 {
       mllt i=0,k,nhim;
       float adev,ave,curt ,sdev, skew, vrnce, x,*data;

       data=vector (1,NPPNB) ;
       for (x=PI/ NBIN; x<=PI; x+'PI/ NBIN) {
           n1im=(int) (0.5+sin(x) *PI/2. 0*NPTS/NBIN) ;
           for (k=1;k<"nlim;k++) data[++i] =x;
       }
      printf ( "moments of a sinusoidal distribution\ n\n") ;
      moment (data,i, &ave, 在adev,ksdev,&vrnce,kskew,&curt) ;
      printf ( "%39s %lls\n\n", "calculated". "expected") ;
      printf ( "Y.s %17s %12. 4f %12. 4f\ n", "Me카l :", " ", ave,PI/ 2.0) ;
      printf ( "%s %4s %12. 4f Y.12. 4f\ n".
           "Average Deviation :", " ", adev, (PI/ 2.0) -1.0) ;
      printf ( "%s V.35 %12. 4f 工12. 4f\ n",
            'Standard Deviation :", " ", sdev,0. 683667) ;
      printf ( "%s %13s 7.12.4f /.12. 4f\ n",
           "Variance :", " ", vrnce,0. 467401) ;
      printf ( "%s 工13s 工12.4f 7.12.4f\ n",
           "Skewness :' , " ", skew,O. O) ;
      printf ( "%s 工13s '/.12.4f %12. 4f\ n",
           "Kurtosis :", " ", curt, -0. 806249) ;
      free_ vector (data, 1,NPPNB) ;
      return 0;
}

   Student 's i-test is a test of two data sets for significantly different means. It is
applied by xttest to two Gaussian data sets datal and data2 that are generated by
gasdev. data2 is originally given an artificial shift of its mean to the right of that of
datal, by NSHFT/2 units of EPS. Then datal is successively shifted NSHFT times to
the right by EPS and rnmnarPd to r1n＋功 h,, +.nn+              A4 hLn..1 -' ,,, " n" nm /n "
 224       N切1)9欣汨／尸e이pes Examp旭 Book

distributions should superpose and indicate populations with the same mean. Notice
that the two populations have the same variance (i.e. 1.0), as required by ttest.
／卞 Driver 如r routine ttest 卞／

#inclucie <stdio . h>
#include "nr. h"
*include "nrutil. h'1

*define )IPTS 1024
#define MPTS 512
*dof ins EPS 0.02
*define NSHFT 10

mllt main(void)
{
       如ng idu皿＝(- 5) ;
       mllt i, j;
       fl oat prob1t1 *datal1*4ata2;

       datal=vector (1,WPTS) ;
       data2=vector (1,MPTS) ;
       /卞 Generate gaussi카k distributed data */
       printf ( "7.6s Y.8s X16s\n", "shift ', "t ", 'probability ") ;
       如r (i=1; i<=NPTS; i++) datal[ i] =gasdev (kidum) ;
       for (i=1;i<=MPTS; i++) data2[i] =(NSHFT/2.0) 李EPS+gasdev (&idum) ;
       for (i=1; i<=NSHFT+1; i++) {
           ttest (data1,NPTS,data2.MPTS,kt ,kprob) ;
           printf ( '%6. 2f %10. 2f %10. 2f\ n", (i- 1) sEPS, t, prob) ;
           for (j= 1; j<=NPTS; j++) datalEj] += EPS;
       }
       free_ vector (data2,1,MPTS) ;
       fraa..vector (datal , 1,NPTS) ;
       return 0;
 }
                                                                                       of a
     avevar is an auxiliary routine for ttest. It finds the average and variance
                                                                          distributions for
 data set. Sample program xavevar generates a series of Gaussian
 1=1, . . ,11, and gives each a shift of (i 나 1)EPs and a variance of i2. This progression
 allows you easily to check the operation of avevar "by eye".
 ／卞 Driver for routine aveva工 卞／

 #include <stdio . h>
 #include 11nr. h"
 #include nnrutil. h'1

 #def ins NPTS 1000
 #def ins EPS 0.1

    mllt main(void)
    {
         mllt i, j;
         long idu皿＝(- 5) ;
         float ave. shift ,vrnce 1*data;

        dat牛vector ( 1, 川玎s) ;
                                                Ch카까er 14: 針카店tical De＄口衣가／on 可Data   225

        /s generate gaussian distributed data 京/
        printf ( "\ n%9s Y.lls Y.12s\n", ''shift ", "average ", ' 'v ari키lce ") ;
        for (i= 1; i< =11; i+ +) {
             shiftr (i叫 1 ) 卓EPS;
             for (j= 1; j<=NPTS; j++)
                  data[ jJ =shift+ i* gasdev (&idust) ;
             avevar (data, NPTS,kave,立vrnce) ;
             printf ( '7.8. 2f V.11. 2f %12. 2f\ n", shjft ,ave, vrnce) ;
        }
        free_ vector (data, 1,NPTS) ;
        return 0;
)

    tutest also does Student's t-test, but applies to the comparison of means of two
distributions with different variance. The example xtutest employs the comparison
method used in ttest but gives the two distributions datal and data2 variances of
1.0 and 4.0 resr氾cti比竝
/卞 Driver for routine tutest */

#include <stdio .h>
#include <math. h>
#include "nr. h1'
#include 'nrutil. hr '

#define NPTS 5000
#define 4PTS 1000
#define EPS 0. 02
#def ins VAR1 1. 0
#define VAR2 4. 0
#def ins NSHFT 10


m1lt main(void)
{
    long id山5=（小51773) ;
    m1lt i, j;
    float fctr1, fctr2 1prob,t, *data1, *data2;

    datal=vector (1 ,NPTS) ．·
    data2=vector (1 ,MPTS) ;
    /京 Generate two gaussian distributions of different variance 5/
    fctrl= sqrt (VAR1) ;
    for (i= 1; i <=NPTS; i++) datal[ i] =fctrlsgasdev (&idum) ;
    fctr2= sqrt (VAR2) ;
    for (irl; i< =MPTS; i++)
         data2［幻 =NSHFT/ 2 刀扼PS+ fctr2枳asdev（虹如5) ;
    printf ( "\ nDistribution #1 : variance = %6. 2f\ n", VAFU) ;
    printf ( "Distribution #2 : variance = Y.6. 2f\ n\ n". VAR2) ;
    printf ( "%7s /.8s %16s\n", "shift ' ' , "t ", 'probability ") ;
    for (i= 1; i< =NSHFT+1; i++) {
         tutest (datal , NPTS,data2,MPTS,立t,&prob) ;
            printf ( '%6. 2f %10. 2f %11. 2f\ n ', (i- l) sEPS, t, prob) ;
            for (j= 1; j<=NPTS; j++) datal[ j] += EPS;
    }
    free_ vector (data2,1,MPTS) ．·
    free_ vector (datal .1, NPTS) ;
    reb江it 0;
     226      N미neri冶／尸a加es Examp旭 Book

J.
    tptest goes a step further, and compares two distributions not only having dii-
ferent variances, but also perhaps having point by point correlations. The example
xtptest creates two situations, one with correlated and one with uncorrelated dis-
tributions. It does this by way of three data sets. datal is a simple Gaussian
distribution of zero mean and unit variance. data2 is datal plus some additional
Gaussian fluctuations of smaller amplitude. data3 is similar to data2 but generated
with independent calls to gasdev so that its fluctuations ought not to have any cor-
relation with those of datal. datal is then given an offset with respect to the others
and they are successively shifted as in previous routines. At each step of the shift
tptest was applied. Our results are given below:
                      Correlated:                    Uncorrelated:
      Shift           t      Probability              t    Probability
      0.01         3. 1199      0.0019             0.6287      0. 5298
      0.02         2. 3399      0.0197             0. 4716     0.6374
      0. 03        1. 5600      0. 1194            0. 3144     0.7534
      0.04         0. 7800      0. 4358            0.1572      0.8751
      0. 05        0. 0000      1. 0000            0. 0000     1. 0000
      0.06        -0. 7800      0. 4358           -0. 1572     0. 8751
      0.07        -1. 5600      0. 1194           -0. 3144     0. 7534
      0. 08       -2. 3399      0. 0197           -0. 4716     0.6374
      0. 09       -3. 1199      0. 0019           -0. 6287     0.5298
      0. 10       -3. 8999      0. 0001           -0. 7859     0.4323
      0. 11       -4. 6799      0. 0000           -0. 9431     0.3460

／卞 Driver 如r routine tptest 字／

#include <stdio . h>
#include 'ni .h"
#include "nrutil. h"

#define NPTS 500
*define EPS 0.01
甘define 月SEFT 11
#define ANOISE 0. 3

mllt main(void)
{
       long idu皿=(- 5) ;
       mllt i, j;
       float avel,ave2, ave3;
       float offset, prob1,prob2,shift, tl, t2;
       float varl, var2, va工3,*datal ,*data2, *data3;

       datal=vector (1,NPTS) ;
       data2=vector (1,NPTS) ;
       data3=vector (1,NPTS) ;
       printf ( "%29s 7.31e\n" ,"Correlated:", "Uncorrelated: ") ;
       printf ( "%7s 工lls 工17s %lle %17s\n ".
           "Shift ", "t ", 'Probability", "t ", "Probability") ;
       offee卜(NSHFT/2汁EPS;
       for (j=1; j< 'NPTS; j++) {
           datal [j] =gasdev (kidun) ;
           data2 [ji =datal [j] +AIOISE*gasdev(kidua) ;
                                          Chapter 14.' 夕帥S加削 Descnp打on 아Da治        227
          data3 [j] =gasdev (&id山n) ;
          data缸口 += ANOISE半gasdev（立iduin) ;
     )
     avevar (datal ,NPTS,&avel, 立varl) ;
     avevar (data2, NPTS,&ave2, &var2) ;
     avevar (data3 ,NPTS ,kave3,立var3) ;
     for (j= 1; j<=NPTS; j++) {
         datalEj] -= avel小offset;
         data2[3] -= ave2;
         data3[ j] -= ave3;
     }
     for (i=1;i<=NSHFT; i++) {
         ehift= i$EPS;
         for (j= 1; j<=WPTS; j++) {
              data2[ j] += EPS;
              data3Ej] += EPS;
         }
         tptest (datal, data2.IPTS,ktl, &probl) ;
         tptest (datal, data3 ,NPTS,&t2 .勾rob2) ;
         printf ( "%6.2f '/.14.4f %12. 4f %16. 4f %12. 4f\ n",
              shift, tl, probl.t2, prob2) ;
     }
     free_ vector (4ata3 11,IPTS) ;
     free_ vector(data2,1,NPTS) ;
     free_vector(datal 11,NPTS) ;
     return 0;
}

    The F-test (routine ftest) is a test for differing variances between two distribu-
tions. For demonstration purposes, sample program xftest generates two distribu-
tions datal and data2 having Gaussian distributions of unit variance. The values
of a third array data3 are then set by multiplying data2 by a series of values factr
which takes its variance from 1.0 to 1.1 in ten equal steps.. The effect of this on the
F-test can be evaluated from the probabilities prob.
／中 Driver 如r routine fteet 卞／

*inc].ude <stdio.h>
*include <iiath.h>
#include "nr. h"
#includa "nrutil. h'1

#define RPTS 1000
#define MPTS 500
#define El'S 0.01
#define IVAL 11

m1lt main(void)
{
     long idwn=(- 13) ;
     lnt i, j;
     float f ,factor, prob, vrnce, *data1, *data2, *data3;

    datal=vector (1,NPTS) ;
    data2rvector (1 1 MPTS) ;
    data3=vector (1,MPTS) ;
    228    Numerica／尸e아）es Examp旭 Book

      /* Generate two gaussian distributions with different varia工lces          卞／
      printf ( "\ n%165 V.5.2f\ n", "Variance 1 = " ,l1 (D;
      printf ( "%13s %lls Y.16s\n" , 'Variance 2", "Ratio", "Probability ") ;
      for (j=1; j<=NPTS; j++) datal[ j] =gasdev (&idu皿) ;
      for (j=1; j<=I4PTS; j++) data2[ j] =gasdev (kiduin) ;
      for (i=1; i<=NVAL; i++) {
          vrnca=l .0+(i- 1) *EPS;
          factor=sqrt (ymnca) ;
          for (3=1, j<=MPTS; j++) data3[ j] =factor*data2[ j] ;
          ftest (datal, NPTS,data3,MPTS,&f,kprob) ;
          printf ( "/,11. 4f '/,13. 4f %13. 4f\ n", vrnce,f, prob) ;
      }
      free..vector (data3,1,MPTS) ;
      free_ vector (data2,1,MPTS) ;
      free_ vector (datal ,i, NPTS) ;
      return 0;
}

    chsone and chstwo compare two distributions on the basis of a x2 test to see if
they are different. chsone, specifically, compares a data distribution to an expected
distribution. Sample program xchsone generates an exponential distribution bins Li]
of data using routine expdev. It then creates an array ebins Li] which is the expected
result (a smooth exponential decay in the absence of statistical fluctuations). ebins
and bins are compared by chsone to give x2 and a probability that they represent
the same distribution.
/* Driver for routine chsone */

#include <stdio.h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

#define NBINS 10
#define NPTS 2000

mnt main(void)
{
      long idum=(- 15) ;
      mnt i, ibin, j;
      float chsq,df, prob, x, *bins,*ebins;

      bins=vector (1,NBINS) ;
      ebins=vector (i ,NBINS) ;
      for (j= l; j<=NBINS; j++) bins[ j] =0.0;
      for (i '1; i<=NPTS; i++) {
          x=expdev (kidu皿) ;
          ibin= (int) (x*NBINS/3. 0)+1;
          if (ibmn <= NBTNS) ++bins (ibmn] ;
      }
      for (i=1; i <rNBINS; i++)
          ebins[i] =3.0*NPTS/NBINS*exp(- 3. 0*(i- 0.5) /NBINS) ;
      chsone(bins, ebins,NBINS,0.&df,&chsq.幻）rob) ;
      printf ( "hlSs Y,lss\ n", "expected", "observed") ;
      for (i "l; i<=NBINS; i++)
          printf ( "/.14. 2f 工1S. 2f\ n", ebins[i] ,bins[i] );
                                                 Ch. 아er 14: S治i恕f允al Descri;升幻n 可Da治   229
          printf ( "\ n%19s %10'. 4f\ n", "chi- squared: ", chsq) ;
          printf ( "%19s 工10. 4f\ n ", 'probability: ", prob) ;
           free..vector (ebins 11,NBINS) ;
          free_ vector (bins,1,NBINS) ;
          return 0;
    :1
     '




        chstwo compares two binned distributions bins1 and bins2, again using
                                                                                  a x2
    test. Sample program xchst日o prepares these distributions both in the same way.
    Each is composed of 2000 random numbers, drawn from an exponential deviate, and
    placed into 10 bins. The two data sets are then analyzed by chstwo to calculate x2
    and probability prob.
／李 Driver for routine chst；
                          日0 卞／

    #inclucte <stdio .h>
    #include <math. h>
    #include "nr. h"
    #include "nrutjl . h1'

 #define 甘BI甘S 10
 #define NPTS 2000

    jut main(void)
{
         long idum=(- 17) ;
         mllt i, ibin, j;
         float chsq, df, prob, x,卓binsl ,*bins2;

         binsl=vector (1,NBINS) ;
         bins2=vector(1 ,NBINS) ;
         for (j=1; j<=NBINS; j++) {
              bmns1[ j] =0. 0;
              bins2[ j] =0. 0;
         }
         如r (i '1 ; i <＝甘PTS; i++) {
              x=expdev (ftithnn) ;
               jbin=(int) (x本甘BI甘S/3.0+1) ;
              if (ibmn <= NBINS) ++binsl[ibin] ;
              x= expdev (kidum) ;
              ibin=(int) (x*NBINS/3. 0+1) ;
              if (ibmn <= 뵤B工甘S) ++bjns2[ jbjn] ;
         }
          chst日o(binsl ,bins2,NBINS, 0 小df，立ch叫．匈江ob) ;
         printf ( "\ nXlss %15s\n", "dataset 1" , "dataset 2") ;
         for (i=1; i<=NBINS; i++)
              printf ( "Y.13. 2f %15. 2f\ n", binslti] ,bins2 (i] );
         printf ( "\ n%18s '/.12. 4f\ n", "chi- squazed: ", chsq) ;
         printf ( "Y.18s Y.12.4f\ n", 'probability: ' ,prob) ;
         free_ vector (bins2,1,NBINS) ;
         free_ vector (binsl , 1, NBTNS) ;
         return 0;
}

    The Kolmogorov- Srnirnov test used in ksone and kstwo applies to unbinned dis-
tributions with a single independent variable. ksone uses the K-S criterion to compare
230       Numerical Re枷s Example Book

a single data set to an expected distribution, and kstwo uses it to compare two data
                                                                                  with
sets. Sample program xksone creates data sets with Gaussian distributions and
          increasing variance, and compares  their cumulative distribution function to
stepwise
the expected result for a Gaussian distribution of unit variance. This result is the
error function and is generated by routine erff. Increasing variance in the test de-
stribution should reduce the likelihood that it was drawn from the same distribution
represented by the comparison function.
／中 Driver 如r routine keone 卞／

#include <stdio . h>
#include <math.h>
#include "nr. h'1
#include nnrutil. h11

#define NPTS 1000
#define EPS 0. 1

float func (float x)
{
      return 1. 0 - erfcc (x/ sqrt (2.0) );
}

mllt main(void)
{
      long idu皿 ' (- 5) ;
      mllt i, j;
      float d,factr, prob, varnce. *data;

      datarvector (1,NPTS) ;
      printf ( "工19s Y.16s %15s\n\n".
          "variance ratio " ,"k- s statistic " , 'probability") ;
      for (i= l; i<"11;i++) {
          varnca=1. 0+(i- 1) *EPS;
           factr=sqrt (varnce) ;
           for (j=1; j<' 'NPTS; j++)
               data Lj] =factr*fabs (gasdev (&idum) );
           ksone(data,NPTS, fu끄c,&d,&prob) ;
           printf ( "%16.6f %16. 6f %16. 6f \n", va口lce,d,prob) ;
      }
      free_ vector (data, 1,NPTS) ;
      return 0;
 }

    kstwo compares the cumulative distribution functions of two unbinned data sets,
 datal and data2. In sample program xkstwo, they are both Gaussian distributions,
 but data2 is given a stepwise increase of variance. In other respects, xkstwo is like
 xksone.
 /+ Driver 如r routine kst日O 中／

 #include <stdio . h>
 #include <math.h>
 #include "nr. h"
 #include "nrutil. h"
                                         Ch콰升er 14: St카台打cal Desc꺄刈on 可Da治      231

#define Ni 2000
#define N2 1000
#define EPS 0. 1

mnt main(void)
{
    long id피n= (- 1357) ;
    ].nt i, j;
    float d, factr, prob, varnce, *datal, sdata2;

    datal=vector (1,N1) ;
    data2=vector (1,N2) ;
    for (i= 1; i<=NI; i++) data1Ei] 'gasdev (&iduin) ;
    printf ( "%18s Y.15s Y.14s\n",
        'variance ratio " , "k-s statistic " ,"probability '" ) ;
    for (i= 1; i< rll; i++) {
        varnce=i. 0+(i- i) *EPS;
        factr=sqrt (varnce) ;
        for (j= 1; j<=N2; j++)
                  data2[ j] = factrtgasdev (&idum) ;
        kstwo (datal,NI,data2,N2,&d, &prob) ;
        printf ( "/.15. 6f /.15. 6f Y.1S. 6f\ n", varnce,d,prob) ;
    }
    free_ vector (data2,1,N2) ;
    free_ vector (datal ,1,Ni) ;
    return 0;
I

    probks is an auxiliary routine for ksone and kstwo which calculates the function
Qk8(시 used to evaluate the probability that the two distributions being compared
are the same. There is no independent means of producing this function, so in sample
program xprobks we have chosen simply to graph it. Our output is reproduced below.
／京 Driver 如r routine probks 卞／

#include <stdio .h>
#include "nr. h"

#define NPTS 20
#define EPS 0. 1
#d日fine ISCAL 40

mnt main(void)
{
    jot i, j, jmax;
    ch缸 t工t [iscAL+i] ;
    fl oat ala皿, aval;

    printf ( "probability function for kolmogorov-smirnov statist ic\ n\n") ;
    printf ( "%75 V.ios Y.135\n", "lambda", "value: ", "graph: ") ;
    for (i=1; i 'c=甘PTS; i++) {
        alajn=i* EPS;
        aval=probks (alam) ;
         jlnax= (int) (0. S+ (ISCAL-1) *aval) ;
        for (j= 0; j<ISCAL; j++) {
              if (j < jmax)
                   txtEj] ='* ' ;
    232    Ni加erica／尸e아始$ Examp伯 Book

                 else
                    txt[ j] =' ';
           }
           txt (ISCALJ= '\ O ';
           printf ( " 工8. 6f %10. 6f          加＼n ' ,ala皿1aval , t工t) ;
      }
      return 0;
}

 Probability      func. for Kolmogorov-Smirnov statistic
   lambda          value:        graph:
  0. 100000       1. 000000
  0. 200000       1. 000000
    0. 300000     0.999991       卞 中 卞 卞 卞＋卞 小 卞 + 中 + * 卞 卞巾＋中中中* 中中中李字 小 巾卞 本卞* 卓 中卞卞＋+ + 中

    0. 400000     0.997192
    0. 500000     0.963945
    0. 600000     0. 864283
    0. 700000     0.711235
    0. 800000     0.544142
    0. 900000     0. 392731
    1. 000000     0. 270000
    1 . 100000    0. 177718      *卞卞＋卞＋卞
    1. 200000     0. 112250      李牛卞*
    1. 300000     0.068092       **中
    1. 400000     0.039682       李字
    1. 500000     0.022218       *
    1. 600000     0.011952
    1. 700000     0. 006177
    1. 800000     0. 003068
    1. 900000     0.001464
    2. 000000     0. 000671


    Procedure cntabl analyzes a two-dimensional contingency table and returns sev-
era! parameters describing any association between its nominal variables. Sample
program xcntabl supplies a table from a file table1.dat that is listed in the Ap-
pendix to this chapter. The table shows the rate of certain accidents, tabulated on
a monthly basis. These data are listed, as well as their statistical properties, by
xcntabl. We found the results to be:
                     chi- squared                               5026. 29
                     degrees of freedom                           88. 00
                     probability                                 0.0000
                     cramer-v                                    0.0772
                     contingency coeff.                          0. 2134


／牛 Driver 如r routine cutabl 卞／


#include <stdio .h>
*include <stdlib. h>
#include "nr. h "
#include "nrutil.       h"

*define 月DAT 9
#define N甘0丑 12
社define MAXST且 80
                                                Ch햐）旭r 14: 匐計M七削Descr肛川on 可Da相   233
    mnt main(void)
    {
         mllt i口，京卞nmbr;
         float ccc, chisq1cramrv ,df ,prob;
         char d山口my[MAXSTR] ,fate[ NDAT+1] [16] ,rnon[NMON+1] [6] ,txt[ 16] ;
         FILE 卞fp;

         nil巾r=ima缸ix (1,NDAT, 1,Nlq0肋 ;
         if   ( (fp = fopen( "tablel. dat " , 'r ") ) == NULL)
                nrerror ( 'Data file tablel. dat not found\n") ;
          fgets (du皿皿y，甘AXSTR, fp) ;
          fgets (d山usy,MAXSTR, fp) ;
          fscanf (fp, "7.16c ", txt) ;
          txt[ 15]='\ O ';
          for (i=1; i<=12; i++) fscanf (fp, " Xs ", mon[i] );
         fgets (dus皿y,MAXSTR,fp) ;
         fgets (dummy,MAXSTIt, fp) ;
         如r (i=1; i<＝甘DAT; i++) {
               fscanf (fp, "Y.16[m0123456789] ", fate[ i] );
               fate[ i] [is] ='\ o ' ;
               for (j=1; j<=12; j+i-)
                    fscanf (fp, "Xd ", &nrnbr[i] [j] );
         }
         fclose(fp) ;
        printf ( '\ n'/.s", txt) ;
         for (i= 1; i<=12; i++) printf ( 'V.ss ', mon[i] );
        printf ( "\ n\n") ;
         for (i=1; i< rNDAT; i++) {
              printf ( "%s", fate[ i] );
               for (j=1; j<=12; j++) printf (叫.5d", nmbr[i] [jj) ;
              printf ( "\ n") ;
        }
        cntabl (nmbr ,NDAT ,NMON ,&chisq,kdf ,却rob,kcramrv ,&ccc) ;
        printf ( "\ n%lSs chi- squared             X20. 2f\ n", " ", chisq) ;
        printf ( "XlSs degrees of freedoinY.20. 2f\ n", " ", df) ;
        printf ( '%iSs probability             Y.20. 4f\ n", " ", prob) ;
        printf ( "V.lSs cramner-v              V.20. 4f\ n'1, " ", cramrv) ;
        printf ( "Y.lSs contingency coeff.工20. 4f\ n" ," ', ccc) ;
        free_ irnatrix (nmnbr, 1, NDAT, 1, NMON) ;
        return 0;
}


th.忿：'二然읖忿忿烈：熙：烈，de
                 ng戈叫杰，까艸，?,'，客｝
忿就罵노群黨ca。f恣趾黑各걺業各鼎，‘竄謐豁斗，琵
entropies for the table:
              entropy of table                     4. 0368
              entropy of x-distribution            1. 5781
              entr야孑 of 少distribution              2.4820
              entropy of y given x                 2.4588
              entropy of x given y                 1.5548
              dependency of y on x                 0. 0094
              dependency of x on y                 0. 0147
              syssnetrical dependency              0. 0114
 234         Numerical Recipes Example Book

/字 Driver for routine cntab2 中/

#include <stdio.h>
#include <stdlib. h>
#include "nr. h"
#include 11nrutil. h11

#define NI 9
#define NMDN 12
#define MAXSTR. 80

mllt main(void)
{
        fl oat h,hx ,hxgy ,hy ,hygx,uxgy,uxy ,uygx;
        mllt i, j, *Snmbr;
        char dulnxny[MAXSTR] ,fate대I+1] [16] ,mon대MON+1] [6] ,txt[ 16) ;
        FILE *fp;

        nmbr=imatrix (1. NI,1,NMON) ;
        if ( (fp = fopen( "tablel. dat ", "r ") ) == NULL)
            nrerror ( "Data file tablel. dat not fo山1d\n' ') ;
        fgets (dummy, MAXSTR, fp) ;
        fgets (duminy,NAXSTR, fp) ;
        fsca끄f (fp, "Y.16c ", txt) ;
        txt[ 15] ='\ O ';
        for (i=1; i<=12; i++) fscanf (fp, ' %s ' , mon[ifl;
        fgets (dununy,NAXSTR, fp) ;
        fgets (d山iny,MAXSTR, fp) ;
        for (irl; i<=NI; i++) {
             fscanf (fp, "V.16[八01234S6789] ", fate[ i] );
             fate[ i] [15] ='\ o ' ·，
             for (j=1; j<=12; j++)
                 fscanf (fp, "Y.d " ,knmbr[i] [j] );
        }
        fclose(fp) ;
        printf ( "\ n/.s" ,txt) ;
        for (i=1; i<=12; i++) printf ( " 工5a' , mon[i] );
        prmntf ( "\ n\n") ;
        for (i=1; i<=N1; i++) {
            printf ( "%s", fate[ i] );
            for (j=1; j<=12; j++) printf ( "V.sd", nmbr[i] (j] );
            printf ( "\ n") ;
        }
        cntab2(nmbr, NI, NMO瓦 &h,khx, *hy,khyg工 , &뇨gy, &uy肛小lxgy,ku工y) ;
        printf ( "\ n      entropy of table              工10. 4f\ n ', h) ;
        printf ( "       entropy of x-distribution %10. 4f\ n", hx) ;
        printf ( '       entropy of y-distribution Y.10. 4f\ n", hy) ;
        printf ( "       entropy of y given x         V.10. 4f\ n" , hygx) ;
        prmntf ( ''      entropy of x given y         Y.10. 4f\ n", hxgy) ;
        printf ( '       dependency of y on x         %10. 4f\ n", uygx) ,
        prmntf ( '       dependency of x on y         %10. 4f\ n ', uxgy) ;
        printf ( '       symmetrical dependency       工10. 41\n", u工y) ;
        free_ imatrix (nmbr , 1,NI , 1,NMON) ;
        return 0;
    }

        The dependencies of x on y and y on x indicate the degree to which the type of
                                        Ch카升er 14: 匐a卄到叱a! Descr材幻nof Data           235
 accident can be predicted by knowing the month, or vice-versa.
     pearsn makes an examination of two ordinal or continuous variables to find linear
 correlations. It returns a linear correlation coefficient r, a probability of correlation
 prob, and Fisher's z. Sample program xpearsn sets up data pairs in arrays dose
 and spore which show hypothetical data for the spore count from plants exposed to
 various levels of 7-rays. The results of applying pearsn to this data set are compared
 with the correct results by the program.
 /s Driver for routine pearsu */

#include <stdio.h>
#include "ar .k"

#defina 1 10

 jut main(void)
{
    mnt i;
    float prob,r, z;
    static float 如se［甘＋1] =
        {0. 0,56.1,64. 1,70. 0 戶已 已 82 . 이아 .3, 90 . 이 99 .乙 115.3,110.0);
    static float spore[N+1] =
        {o. o,0. 11,0. 40,0.37,0. 48,0. 75,0.66,0.71, 1. 20,1.01,0. 95) ;

    printf ( "\ nEffect of Gamma Rays on Man-in- the-Moon Marigolds\n") ;
    printf ( " 工16s %23s\n ", "Count Rate (cpm) ". "Pollen Index ") ;
    for (i= 1;i<"I; i++)
        printf ( "%10. 2f 工25. 2f \n", dose[i] ,spore[i] );
    pearsu(dose, spore,月,kr, &prob,kz) ;
    printf ( "\ n'/.30s '/.16s\n ", "PEARSN", "Expected") ;
    printf ( "%s %8s %9f %16f\n ", "Corr. Coeff. ", " ", r, 0. 9069586) ;
    printf ( "/.s 水s '/.9f %lsf\n", "Probability", " ", prob,0. 2926505e-3) ;
    printf ( "/.s 工los 工9f '/.lSf\ n", "Fisher 's z", " ", z, l. SlOllO) ;
    return 0;
}

    Rank order correlation may be done with spear to compare two distributions
datal and data2 for correlation. Correlations are reported both in terms of d, the
sum-squared difference in ranks, and rs, Spearman's rank correlation parameter.
Sample program xspear applies the calculation to the data in table tab1e2 .dat
(see Appendix) which shows the solar flux incident on various cities during different
months of the year. It then checks for correlations between columns of the table,
considering each column as a separate data set. In this fa計lion it looks for correla-
tions between the July solar flux and that of other months. The probability of such
correlations are shown by probd and probrs. Our results are:
Check correlation of sampled U. S. solar radiation (july with
                                                              other months)
month         d      St. dcv.        probd      spearman-r    probrs
 jul         0.00   -4. 358899    0.000013       1.000000    0.000000
 aug       122. 00  -3. 958458    0.000075       0.908132    0. 000000
 sep       218. 00  -3. 643898    0.000269       0. 835967   0.000004
 0ct       384. 00  -3. 098495    0.001945       0.710843    0.000443
 nov      390. 50   -3. 077642    0.002086       0.706060    0.000503
 dec      622. 00   -2. 318075    0.020445       0.531803    0.015806
 jan      644.50    -2. 244251    0.024816       0.514866    0.020181
    236    八加me力ca사？ec徊es Exan冽e Book

    feb        483. 50    -2. 772503      0.005563            0. 636056   0. 002573
    mar        497. 00    -2. 728208      0. 006368           0. 625894   0.003158
    apr        405. 50    -3. 027925      0. 002462           0. 694654   0.000677
    may        264. 00    -3. 492371      0. 000479           0. 801205   0.000022
    jun        121. 50    -3. 960099      0. 000075           0. 908509   0. 000000

/* Driver for routine spear */

#include <stdio.h>
#include <stdlib. h>
#include "nr. h"
#include "nrutil. h1'

#define NDAT 20
#def ins NMON 12
#def ins MAXSTR 80

mnt main(void)
{
      mllt i 口 ;
      float d,probd,probrs,rs, zd, *ave, *datal, *data2,卓zlat, *Srays;
      cha工 duimny[MAXSTR] ,txt[ MAXSTR] ,city[ NDAT+1] [17] ,mon[NMO甘+1] [5] ;
      FILE *fp;

      ave=vector ( 1, NDAT) ;
      datal=vector (1,NDAT) ;
      data2=vector (1,NDAT) ;
      zlat=vector (1,NDAT) ;
      rays=matrix (1,NDAT,1,NMON) ;
      if ( (fp = fopen( "table2. dat ", "r ") ) == NULL)
          nrerror ( "Data file tab1e2. dat not found\n") ;
      fgets (dummy,MAXSTIt, fp) ;
      fgets (txt ,MAXSTR. , fp) ;
      fscanf (fp , 叫伊 l5c ") ;
      for (i=1; i<=NM0N; i++) fscanf (fp, " Y.s", mon[i] );
      fgets (duinmy,MAXSTh, fp) ;
      fgets (dul띠ny, MAXSTR, fp) ;
      for (i=1; i<=NDAT; i++) {
           fscanf (fp, "% V0123456789] ", city[ i] );
           city[ i] E16] ='\ o ' ;
           for (j= 1; j <=NM0N; j++) fscanf (fp, "%f ", krays[i] [j] );
           fsc키if (f p, 叫仕 };f " .&ave[i] 小zlat 口］) ;
      }
      fclose (fp) ;
      prmntf ( "%s\n" , txt) ;
      printf ( "%165 " , " ' ') ;
      for (i=1; i<=12; i++) printf ( "%4s ", mon[i] );
      printf ( "\ n") ;
      for (i=1; i<=NDAT; i++) {
          printf ( "%s ", city[ i] );
          for (j= 1; j<=12; j++)
                prmntf ( "%4d", (int) (0. S+rays[i] [j] ));
          printf ( "\ n") ;
      }
      /巾 Check temperature correlations between different months 卞/
      printf ( "\ nAre sunny summer places also s山lny winter places?\n") ;
      printf ( "Check correlation of sampled U. S. solar radiation\ n") ;
                                          Ch카升er 丁4: 針카旭伉：a江)esc꺄川on of Data      237


    printf ( " (july with other months) \n\ n") ;
    printf ( "Y.s %95 V.14s %lls Y.l6s Y.los\n" ,"month", "d",
        "at. dev. ", "probd", "spearman-r ", "probrs") ;
    for (i=1; i<=甘DAT; j++) datal [i] =rays [ii [1] ;
    for (j=1; j<=12; j++) {
        for (i=1; i<=NDAT; j++) data2[i] 'rays[i] [j] ;
        spear (datal, data2，川DAT,kd，幻d，幻江obd,&rs，却robr引 ;
        printf ( "/.45 V.12. 2f %12. 6f V.12. 6f /.13. 6f %12. 6f\ n",
             mon[ j] ,d, zd,probd,rs, probrs) ;
    }
    free_matrix (rays, 1,NDAT, 1,NMON) ;
    free_ veCtOr (Z].at , 1, NDAT) ;
    free. veCtor (data2,1,甘DAT) ;
    free_ vector (datal ,1,NDAT) ;
    free_ vector (aVe, 1,NDAT) ;
    return 0;
}

     crank is an auxiliary routine for spear and is used in conjunction with sort2. The
latter sorts an array, and crank then assigns ranks to each data entry, including the
midranking of ties. Sample program xcrank uses the solar flux data of table2 .dat
(see Appendix) to illustrate. Each column of the solar flux table is replaced by the
rank order of its entries. You can check the rank order chart against the chart of
original values to verify the ordering.
／巾 Driver for routine cra끄k 布／

#iflc].ude <stdio .h>
#include "nr. h"
#include "urutil . h'1

#define NDAT 20
#define NMON 12
#define I4AXSTR 80

mllt main(void)
{
    mllt i, j;
    float 牛data, 京order, 李5, 卞巾rays;
    cha工 dummy[MAXSTR] ,txt[ MAXSTR] ,city[ NDAT+1] [17] ,mon[NMON+1] [5] ;
    FILE *fp;

    data=vector (1,NDAT) ;
    order=vector (1,NDAT) ;
    s=vector (1,NMON) ;
    rays=matrix(1,NDAT, 1,NMON) ;
    if ( (fp = fopen( "tab1e2. dat ", "r ") ) == NULL)
        nrerror ( "Data file table2.dat not fonnd\n") ;
    fgets (dummy,MAXSTR, fp) ;
    fgets (txt , MAXSTR ,iP) ;
    fscanf (fp, " 加lsc") ;
    for (i '1; i<=NM0甘; i++) fscanf (fp, " V.s", mon[i] );
    fgets (dui띠ny,NAXST!t, fp) ;
    fgets (dummy,MAXSTR, fp) ;
    for (i=1; i<'甘DAT; i++) {
         fsc카lf (fp, "V. V0123456789] ", city[ i] );
    238    Nun甘元a/ 尸e야石S Examp旭 Bo아（

           city[ i] [16] ='\ O ' ;
           for (j=1; j<=NMOM; j++) fscanf (fp, "IJ ', &rays[il[ j] );
           fgets (duismy,MAXSTR, fp) ;
      }
      fclose(fp) ;
      printf ( "Y.s\n%16s ", txt, " " );
      for (i= l; i<=12; i++) printf ( " 加", luon[i] );
      printf ( "\ n ') ;
      for (i=1; i<=NDAT; i++) {
          printf ( ' '%s", cjty[ i] );
          for (j=1; j<=12; j++)
              printf ( "%4d", (int)        (O. S+rays[i] [j] ));
          printf ( "\ n") ;
      }
      printf ( " press return to continue . . .\n ') ;
      getcharO;
      /* Replace solar flux in each column by rank order */
      如r (j= l口＜=12; j++) {
          for (i= 1; i<=NDAT; i++) {
                dat缸ii =rays［幻 Li] ;
                order Li] =i;
          }
          sort2(NDAT,data, order) ;
          cr카1k (NDAT , data, &s [j] ) ;
          for (i=1; i<=NDAT; i++)
                rays[(int) (O. 5+order[i] )] [j] =data[i] ;
      }
      printf ( "'/.16s ' , ' ') ;
      for (i=1; i<=12; i++) printf ( " /.s", mon[i] );
      printf ( "\ n") ;
      for (i=1; i<=NDAT; i++) {
          printf ( "%s", city[ i] ),
          for (j=1; j<=12; jl+ )
              printf ( 'V.4d", (int)       (O. 5+rays[i] [j] ));
          printf ( "\ n') ;
      }
      freejnatrix (rays, 1,NDAT, 1,NMON) ;
      free_ vector (s * 1, NMOIJ) ;
      free_ vector (order, 1,NDAT) ;
      free_ vector (data,1,NDAT) ;
      return 0;
}

    kendli and kendl2 test for monotonic correlations of ordinal data. They differ
in that kendil compares two data sets of the same rank, while kendl2 operates on
a contingency table. Sample program xkendll, for example, uses kendil to look
for pair correlations in our five random number routines. That is to say, it tests for
randomi瑯s by seeing if two consec毗汁e nun小ers from the ger此r毗야 have a mon야onic
correlation. It uses the randomn number generators ranG, . . ., ran4, one at a time, to
generate 200 pairs of random numbers each. Then kendil tests for correlation of the
pairs, and a chart is made showing Kendall's r, the standard deviation from the null
hypotheses, and the probability. For a better test of the generators, you may wish
to increase the number of pairs NDAT. It would also be a good idea to see how your
result depends on the value of the seed idum.
                                          cm카）旭r 14: Sta打＄加a! Descril刈on of Data   239

1李 Driver for routine kendli */

#include <stdio . h>
#inc].ude nnr. h11
#include "nrutil. h"

#define NDAT 200

m11t main(void)
{
     jut i, j;
    long idu皿；
    float prob, tau,z, 京datal, *data2;
    static char *txt[ 5] ={ "RANO" ."RANI". "RAN2 ". "RA甘3 " , "RAN4"} ;

    data1 'vector (1,NDAT) ;
    data2=vector (1,NDAT) ;
    /* Look for correlations in RANO, RAN1, RAN2, RAN3 카1d RAN4 */
    printf ( "\ nPair correlations of RAND . . . RAN4\n\n") ;
    printf ( "V.9s %17s Y.16s %18s\n ',
        "Progra皿", "Kendall tau", "Std. Dev. ". "Probability ') ;
    for (i=1;i<=5;i++) {
        iduin ' (- 1357) ;
         for (j= 1; j<=NDAT; j++) {
             if (i == 1) {
                  datal[ jl= rano (&idum) ;
                  data2[ j] =rano (&idum) ;
             } else if (i == 2) {
                  datal[ j] =ranl (&idum) ;
                  data2[ j] =rani(kidum) ;
             } else if (i == 3) {
                  data1[ j] 'ran2 (&idum) ,
                  data2[ jJ'ran2(&idum) ;
             } else if (i == 4) {
                  datal [j] =r카i3 (tidu皿）;
                  data2[ j] =ran3(kiduiu) ;
             } else if (i == 5) {
                  data1Cj] =ran4(idum) ;
                  data2[ j] =ran4(&idum) ;
             }
        }
        kendli (datal, data2,NDAT,&tau,&z,kprob) ;
        printf ( "%8s '/.17.6f %17. 6f Y.17. 6f\ n", txt[ i- lI, tau,z,prob) ;
    }
    fre乞V毗h江（data2,1,NDAT) ;
    free_ vector (datal , 1,NDAT) ;
    return 0;



    Here is the output from the above test:
Pair correlations of RANO             RAN4
Program      Kendall tau               Std. 0ev.         Probability
  RAND        -0. 010452               -0. 219801          0.826026
  RAIl        -0. 023719               -0. 498780         0. 617934
  RAN2         0.130251                 2.739064          0.006161
  RAN3        -0. 062814               -1. 320922         0. 186527
    240     Numerical Recipes Example Book

     RAN4           0. 023016          0.483986             0.628396


    Sample program xkendl2, for routine kendl2, prepares a contingency table based
on the routines irbiti and irbit2. You may recall that these routines generate
random binary sequences. The program checks the sequences by breaking them into
groups of three bits. Each group is treated as a three-bit binary number. Two
consecutive groups then act as indices into an 8 x 8 contingency table that records
how many times each possible sequence of six bits (two groups) occurs. For each
random bit generator, NDAT=1000 samples are taken. Then the contingency table
tab[k] [1] is analyzed by kendl2 to find Kendall's r, the standard deviation, and
the probability. Notice that Kendall's r can only be applied when both variables are
ordinal (here, the numbers 0 to 7), and that the test is specifically for monotonic
correlations. In this case we are actually testing whether the larger 3-bit binary
numbers tend to be followed by others of their own kind. Within the program, we
have expressed this roughly as a test of whether ones or zeros tend to come in groups
more than they should.
／卞 Driver 如r routine kend12 方／

#include <stdio . h>
#include "nr. h"
#include "nrutil. h'1

#define NDAT 1000
#def ins IP 8
#define JP 8

mnt raain(void)
{
      mllt ifunc, i=IP, j=JP,k. l, m,n,t口oton;
      unsigned long iseed;
      float prob,tau, z, **tab;
      static char 巾t工t [8] =
           {"000", "001", "010", "011", "100", "101", '110", "111"} ;

      /* Look for 'ones-after- zeros ' in IRBITI and IRBIT2 sequences */
      tab=matrix (1,IP, 1, JP) ;
      printf ( "Are ones followed by zeros and vice-versa'\ n") ;
      for (ifunc=l; ifunc<==2; ifunc++) (
          iseed=2468;
          if (ifunc == 1)
                printf ( "test of irbitl: \n") ;
          else
                printf ( "test of irbit2: \n") ;
            for (k=1;k<=i; k++)
                for (1=1;l<=j; l+ +) tab[k] [l] =0.0;
            for (m=1;m<=NDAT;m++) {
                k=1,
                t日oton=l ;
                for (n=0;n< '2;n++) {
                     if (ifu工1c == 1)
                         k += (irbiti伍iseed汁t日0的n) ;
                     else
                          k += (irbit2 (&iseed)方t日oton) ;
                     twoton *= 2;
                                      C/i카升or 14: Statis加a! Desc꺄月幻n 可Da治   241

            }
            l=1;
            t日oton=1;
            for (n=0;n<=2;n++) {
                 if (ifunc == 1)
                      1 += (irbitl (&iseed）牛t日Ot(玎l) ;
                 el月e
                      1 += (irbit그伍iseed汁的毗on) ;
                 t；日oton 卞＝ 2;
            }
            ++tab[k] [1] ;
       }
       kendl2(tab, i ,j ,&tau,tz ,&prob) ;
       printf ( "    ") ;
       for (n=0;n<=7;n++) printf ( " 工6s ", txt[ n] );
       printf ( "\ n") ;
       for (n=1;n<=8;n++) {
           printf ( "%3s", txt[ n-1] );
           for (m=1;m<=8;m++)
                 printf ( "工6d", (int) (0.5+tab[n] [m1) );
           printf ( "\ n") ;
       }
       printf ( "\ n%17s 工14s %165\n' .
           "kendall tau", "std. dev. ", "probability ") ;
       printf ( "Y.15.6f X15. 6f Y.15.6f\ n\n", tau,z,prob) ;
   }
   free_matrix(tab, 1,IP, 1, JP) ;
   return 0;



   The output of xkendl2 looks like this:
Are ones followed by zeros and vice-versa?
test of irbiti:       l
                      0    0
       000     001 010     011   100  101    110         111
                        그
                        U
000    17      15   3      14    14   18     10          15
                        8
001    18      14   8      16    14   22     17          10
                        6
010    18      15   6      14    14   16     13          15
                        8
011    17      13   8      18    21   26     17          13
                      n
                      d LU 5
100    15      16  12      11    18   18     18          18

                      d
                      1 d1 2
101    14      10  15      17    18   16     25          15
110    16      12  25      16    23   16     13          22
111    17      15  16      18    16   15     23          14
      kendall tan      std. dev.     probability
       0. 011227       0.531589       0. 595010
test of irbit2:
       000     001 010     011   100  101    110         111
000    21      12  21      16    17    9     14          15
001    14      17  15      18    10   17     20          16
010    19      17  15      16    17   17      9          14
011    12      18   9      16    13   26     13          13
100    16      18  14      16    12   19     16          11
101    12       21 20      16    17   13      8          15
110    14      18  20      17    12   17     12          19
111    19      16  15      22    19    9     19          13
      kendall tan      std. dev.     probability
      -0. 003014      -0. 142716      0. 886516
    242      Numerica사？ec徊es Examp旭 Book

    The routine ks2dls tests a single sample (hence "is") of a two-dimensional dis-
tribution (hence "2d") against a theoretical model distribution, returning the signif-
icance level with which the distribution can be said to differ from the model. The
model, supplied by the user, is contained in the routine quadvi. The main book
supplies a sample quadvi where the model is a distribution that is uniform inside the
square xj < 1, I!/I < 1, so we will use that quadvi in our example program.
    We generate a sample that is made nonuniform by "warping" the output of the
uniform random number generator by a quadratic function of adjustable amplitude
(factor). Then, the program invokes ks2dls and prints the significance of the result.
This is repeated some number of times, so that you can get an idea of how variable
the test is from run to run.
    If you run the program, you will see that factor as large as 0.1 is easily detectable
in a 500 point sample (i.e., it gives very small values for PROB), but not detectable
in 100 points. In a 100 point sample, factor must be on the order of 0.5 before it
becomes easily detectable.
/s Driver for routine ks2dls */

#include <stdio.h>
#include 11nr. h"
#include '1nrutil. h11

#define NMAX 1000

mllt ntain(void)
{
          long idu皿；
          unsigned long j, jtrial, nl, ntrial;
          float d.factor. prob,u1v,中x1, sy1;

          xl=vector (1.NMAX) ;
          yl=vector (1,NMAX) ;
          for (; ;) {
              printf ( "How many points?\n'O,
              if (scanf ( "%lu ' , &nl) == EOF) break;
              if (ni > NMAX) {
                  printf ( "nl too large. \n") ;
                  continue;
              }
              printf ( "What factor nonlinearity (0 to 1) ?\n") ;
              for (; ;) (
                        if (scanf ( "%f ' , &factor) == EOF) {
                                   factor = -1. 0;
                                  break;
                       }
                       if   (factor < 0. 0) {
                                 printf ( "factor less than 0\n") ;
                                 continue;
                       }
                       if   (factor > 1.0) {
                                 printf ( 'factor greater than 1\n") ;
                                 continue;
                       }
                       break;
                                         Gb카가or 14: 針計台依：a! Descr(c川on 可Data    243
            }
            if (factor == -1. 0) break;
            printf ( "How many trials? \n") ;
            if (scanf ( "Y.lu ", &ntrial) == EOF) break;
            iduni = -289-ntrial- nl;
            for (jtrial= 1;jtrial< =ntrial; jtrial+ +) {
                 for (3=1; j< 'n1; j++) {
                      u=ranl (&idum) ;
                      u=u*( (1.0-factor) +u*f actor) ;
                      xl [j] =2 . 0*u-1.0;
                      v=ranl (&iduin) ;
                      v=v*( (1.0-f actor)+v*f actor) ;
                      yl[ j] =2.0*v-1.0;
                }
                ks2dls (xl ,yl ,nl, quadvl,kd, &prob) ;
                printf ( "d, prob= %12. 6f %12. 6f\ n", d,prob) ;
            )
       }
       free_ vector (yl, 1,NMAX) ;
       free_vector (xl 山NMAX) ;
       printf ( "Normal completion\n") ;
       return 0;
}

    The routine ks2d2s performs a similar statistical test, but on two samples and
without the necessity of a model. The example program is quite similar to that for
ks2dls. Now, however, we generate two samples, drawn from 2-dimensional Gaussian
distributions of slightly different shape (as controlled by the variable shrink).
    Running the program, one finds that with, e.g., sample sizes of 100 points for
the first sample and 80 points for the second sample, a value shrink = 0.5 is easily
detectable as a low value for prob, while shrink = 0.8 is not.

／斗 Driver 如r routine ks2d2$ 牛／/

#inc].ude <stdio.h>
#include "nr. h"
#include "nrutil .li "

#define NMAX 1000

mnt main(void)
{
      Long idum;
      unsigned long j ,jtrial, nl, n2,ntrial;
      float d,prob, shrink,u,v;
      flo毗 求xl Jyl, 卞x2, 京y2;

      xl=vector (1 ,NMAX) ;
      yl=vector (1 ,NMAX) ;
      x2=vector (1,NMAX) ;
      y2=vector (1,NMAX) ;
      for (; ;) {
          prmntf ( " 工uput 甘1,甘2\n') ;
          if (scanf ( "%lu '/.lu", &nl,kn2) == EOF) break;
          if (ni > NNAX) {
               printf ( "nl too laxge. \n") ;
244       Nume月ca/ 尸ecipes Examp旭 Book

                 Cont mnu日 ;

            }if (n2 > NMAX) {
                 printf ( 'n2 too large. \n") ;
                 continue;
            }
            printf ( "What shrinkage?\n') ;
            if (scanf ( "/.f " ,&shrink) == EDF) break;
            printf ( "How many trials? \n') ;
            if (scanf ( "V.lu ', tntrial) == EOF) break;
            if   (ntrial > NMAX) {
                  printf ( "Too many trials. \n") ;
                  continue;
            }
            iduin = -287-ntrial- nl- n2;
            for (jtrial= 1; jtrial< =ntrial; jtrial+ +) {
                 for (j=1; 3< 'ni; j++) {
                     u=gasdev (kidu皿) ;
                     v=gasdev (kidum) *shrink;
                       xl[ j] =u+v;
                       yl [j] 'u- v;

                  f。
                  J.r (3=1; j<=n2; j++) {
                      u=6asdev (tidum) *shrink;
                      v=gasdev (kidum) ;
                       x缸刃m+V;
                       y2[ j] 'u- v;
                 }
                 ks2d2s(xl, yl, nl, x2, y2,n2,&d,幻：1rob) ;
                 printf ( 'd, prob= 工12. 6f 7.12. 6f\ n", d,prob) ;



        free_ vector (y2 ,1,NMAX) ;
        free_ vector (x2 ,1,NMAX) ;
        free_ vector (yl 11,NI4AX) ;
        free_ vector (xl .1,NMAX) ;
        printf C "Normal completion\n ") ;
        return 0;
}

     Sample program xsavgol tests savgol by computing Savitzky-Golay smoothing
coefficients for various values of M, 7iL and n足 It then compares the answers with
pre- saved values.
/* Driver for routine savgol */

#include <stdio.h>
#include '1nr.h'1
#include "nrutil . h'1

#define NMAX 1000
#defjne NTEST 6

mllt main(void)
{
      mnt i, j, m,nl, np.nr;
      float *c, swfl;
                                                 Chapter 14: 針a打S比a! Descn乍가幻／7of Da治                       245

      static        mnt mtest[NTEST+1] = (0, 2, 2, 2, 2, 4,4) ;
      static        mllt nltest[ NTEST+1] = (0, 2,3, 4, 5, 4,5) ;
      static        mllt nrtest[ NTEST+1] = (0, 2, 1, 0, 5, 4, 5) ;
      static        char *카ls[NTEST+1] = {1111 1
                                -0. 086 0. 343        0. 486     0. 343 -0. 086"
11
                         -0. 143 0. 171 0. 343        0. 371     0. 257",
                0. 086 -0. 143 -0. 086       0. 257   0. 886",
11 - 0. 084     0. 021 0. 103 0. 161         0. 196    0. 207    0. 196   0. 161   0. 103   0. 021 -0. 084",
             0. 035 -0. 128         0. 070   0. 315    0. 417    0. 315   0. 070 -0. 128    0. 035",
     0. 042 -0. 105 -0. 023         0. 140   0. 280    0. 333    0. 280   0. 140 -0. 023 -0. 105     0. 042"]';


     c=vector (1, NMAX) ;
     printf ( "M iii nr\ n") ;
     printf ( "\ t\ t\ tSample Savitzky-Golay Coefficients\ n") ;
     for (i= 1; i< =NTEST; i++) {
          m=mtest Ii] ;
          nl=nltest 1刃
          nr=nrtest [i] ;
          np=n1+nr+1;
          savgol(c, np,nl, nr, 0,m) ;
          for (sum'0. 0, j=1; j<=np; j++) sum += ctj] ;
          printf ( "/.ld %ld Y.ld\ n"", m,nl, nr) ;
          for (j= nl; j<5; j++) printf (叫.7s", " ") ;
               (j= nl+1; j>=1; j- -) printf ( "%7. 3f ", c[J] );
              for
          for (yro; j<nr; j++) printf ( "Y.7. 3f ", c[叩- j] );
          printf ( "\ n") ;
          printf ( "Sum = Y.7. 3f\ n", s山s) ;
          printf ( "Compare answer: \n'/.s\n"' , ans[i] );
      }
      free1vector (c, 1,NMAX) ;
      return 0;
}

                                                      Appendix

File table 1 .dat:

Accidental Deaths by Month and Type (1979)
Month:                     jan feb mar apr may jun jul        aug sep oct nov dec
Motor Vehicle             3298 3304 4241 4291 4594 4710 4914 4942 4861 4914 4563 4892
Falls                     1150 1034 1089 1126 1142 1100 1112 1099 1114 1079 999 1181
Drowning                   180 190 370 530 800 1130 1320 990 580 320 250 212
Fires                      874 768 630 516 385 324 277 272 271 381 533 760
Choking                    299 264 258 247 273 269 251 269 271 279 297 266
Fire- arms                 168  142 122 140 153 142 147 160 162 172 266 230
Poisons                    298 277 346 263 253 239 268 228 240 260 252 241
Gas-poison                 267 193 144 127      70   63   55   53   60 118 150 172
0ther                     1264 1234 1172 1220 1547 1339 1419 1453 1359 1308 1264 1246


File tab1e2 .dat:
Average solar radiation (watts/ square meter) for selected cities
Month:          jul aug sep oct nov dec jan feb mar apr may jun                             ave     lat
Atlai比a, GA     257 246 201 166 30 102 106 140 184 236 258 271                              192    34. 0
Barro日1 AK      208 123 56 20      0   0   0 18 87 184 248 256                              100    71. 0
Bisma工k, ND     296 251 185 132 78 60 76 121 170 217 267 284                                178    47. 0
Boise, ID       324 275 221 152 88 60 69 113 164 235 284 309                                191    43. 5
246     Numerical Recipes Example Book

Boston. MA       240 206 165 115   70   58   67 96 142 176 228 242     150   42.5
Caribou, MX      246 218 161 102   53   51   66 111 178 194 229 232    153   47.0
Cleveland, OH    267 239 182 127 68 56 60 87 151 182 253 271           162   41.5
Dodge City, KS   311 287 239 184 138 113 123 153 202 2S6 275 315       216   38.0
El Paso, TX      324 309 278 224 178 151 160 209 266 317 346 353       260   32.0
Fresno, CA       323 293 243 182 117 77 90 143 212 264 308 337         216   37.0
Greensboro, NC 263 235 197 1S6 118 95 97 134 171 227 257 273           185   36.0
Honolulu, HI    305 293 271 245 208 176 175 200 234 262 300 297        247   21.0
Little Rock, AR 270 250 214 167 118 91 96 127 173 220 256 272          188   35.0
Miami, FL        260 246 216 188 171 154 166 201 238 263 267 257       219   26.0
New York, NY     251 238 175 127 77 62 71 102 151 183 220 255          159   41.0
0maha, NE        275 252 192 142 96 80 99 134 172 224 248 272          182   21.0
Rapid City, SD   288 262 208 152   99   76   90 135 193 235 259 287    190   44.0
Seattle, WA      242 209 150 84    44   29   34   60 118 174 216 228   132   47.5
Tucson, AZ       304 286 281 216 172 144 151 195 264 322 358 343       253   41.0
Washington, DC   267 190 196 145 75 64 101 124 153 182 215 247         163   39.0
 Chapter 15: Modeling of Data

         Chapter 15 of Numerical Recipes deals with the fitting of a model func-
    tion to a set of data, in order to summarize the data in terms of a few model
    parameters. Both traditional least-squares fitting and robust fitting are con-
    sidered. Fits to a straight line are carried out by routine fit. When there
    are errors in both x and y, straight-line fitting is done by fitexy. More gen-
    eral linear least-squares fits are handled by if it and covsrt. (Remember
    that the term "linear" here refers not to a linear dependence of the fitting
    function on its argument, but rather to the fact that a linear combination of
    the functions is fit to the data.) In cases where if it fails, owing probably to
    near degeneracy of some basis functions, the answer may still be found using
    svdf it and svdvar. In fact, these are generally recommended in preference
    to if it because they never (?) fail. For nonlinear least-squares fits, the
    Levenberg-Marquardt method is discussed, and is implemented in mrqmin夕
    which makes use also of covsrt and mrqcof.
        Robust estimation is discussed in several forms, and illustrated by routine
    niedf it which fits a straight line to data points based on the criterion of
    least absolute deviations rather than least-squared deviations. rofunc is aul
    auxiliary function for medf it.



     Routine fit fits a set of N data points (x[ij ,y[i] ), with standard deviations
 sigCi] , to the linear model y = A + Bx. It uses x2 as the criterion for goodness-
of-fit. To demonstrate fit, we generate some noisy data in sample program xf
                                                                                 it.
For NPT values of i we take x = O.li and y = -2x + 1 plus some values drawn
from a Gaussian distribution to represent noise. Then we make two calls to fit, first
performing the fit without allowance for standard deviations sig[i] , and then with
such allowance. Since sig[i] has been set to the constant value spread, it should
not affect the resulting parameter values. The values output from this routine are:
Ignoring standard deviation:
               1. 079573        uncertainty:   0. 099821
      b   =   -2. 006663        uncertainty:   0. 017161
      chi- squared:        24. 047955
      goodness-of- fit:     1. 000000


Including standard deviation:
     a   =     1. 079573        uncertainty:   0. 100755
     b   =    -2. 006663        uncertainty:   0.017321
      chi- squared:        96. 191818



                                                                                  '47
 248          N切nerica／尸ec徊es Examp旭 Book

            goodness-of- fit:      0.532772


／方 Driver 如r routine fit           中／


*include <stdio.h>
#include "nr. h"
#include "nrutil. h'1

*define NPT 100
#define SPREAD 0. 5

mnt main(void)
{
        long idum=(- 117) ;
        mnt i, mwt;
        float a,b, chi2,q,siga.sigb, 方工，中y1巾sig;

        x=vector (1.IPT) ;
        y= vector (1,NPT) ;
        sig 'vector (1. NPT) ;
        for (i=1; i<=NPT; i++) {
             工［刃 =0. 1京1;
             此ii = -2. 0中工［i] +1. 0+SPREAD中gasdev (kidu皿）;
             Big [i] =SPREAD;
        }
        如r (a日t=0;m日t<=1;m日t++) {
           lit (x, y.NPT, sig. mwt,&a,kb,ksiga,ksigb,kchi2,kq) ;
               if (mwt == 0)
                   printf ( "\ nignoring st띠ldard deviations\n") ;
               else
                   prmntf ( "\ nlncluding sta끄dard deviations\n") ;
               prmntl( "V.125 V.9.61 V.18s V.9.61 \n".
                   "a = ", a, "uncertainty: ' . siga) ;
               prmntf ( "%12s V.9. 61 %18s V.9.61 \n",
                    'b = ". b, "uncertainty: ". sigb) ;
               printf ( "V.19s V.14. 61 \n". "chi- squared: ", chi2) ;
               printf ( "V.235 V.10.61 \n". "goodness느ol-fit:    ', q) ;
        }
        freeevector (sig. 1,NPT) ;
        free느vector (y. 1,NPT) ;
        free. vector (x, 1,月PT) ;
        return 0;
    }

        Here is a program that puts the routine fitexy, which fits a straight line to data
    with error bars in both x and y, through its paces. The underlying straight line is
    taken to be
                                         y = 2x -5

         We generate a synthetic data set that has errors in both x and y, with the errors
                                                                                         then
    having a magnitude that is highly variable (but known) from point to point. We
         fitexy   and print its result. As a comparison,  we  set the x errors to zero and do
    call
    the fit both with fitexy and with the simpler routine fit. Similarly, interchanging
    the roles of x and y, we can do this setting the y errors to zero. (We have to transform
    the answers, however, so as to be able to interpret x and y in their true roles.)
                                                         Ch햐가or 15: Mode／加g 아Da治   249

       0utput from this program looks like this:
    Values of a,b,siga, sigb, chi2,q:
    Fit with x and y errors gives:
      -5. 058980   2. 022800   0. 274571    0. 020892   42. 586609    0. 038141
    Setting x errors to zero gives:
      -5. 538356   2.008888    0. 110675    0.009360 277. 534546      0. 000000
    . . .to be compared with fit result:
      -5. 538357   2. 008888   0. 104930    0.008537 277. 534424      0. 000000
    Setting y errors to zero gives:
      -5. 477018   2. 043204   0. 184778    0. 012426 105. 700729     0. 000000
    . . .to be compared with fit result:
      -5. 494896   2. 044625   0. 160466    0. 012380 105. 687660     0. 000000


    Notice that the intercept and slope are obtained correctly, notwithstanding a
somewhat unlucky value for the x2 probability. (This demonstrates that you should
not reject a hypothesis just because its x2 probability is as small as a few percent:
that happens a few percent of the time for correct models!)
    Setting either the x or y errors to zero, however, produces significantly wrong
results for the intercept, as well as misleading formal errors on the parameters and
unacceptable x2 probabilities.
／巾 Driver 如r routine fitexy 牛／

#include <stdio.h>
#include <math.h>
#include 'nr. h"
#include 1'nrutil. h"

#define NPT 30

mllt main(void)
{
      long idwn ' (- 1) ;
      ml1t j;
      float a,b, chi2.q,sa,的.siga,sigb;
      float *x, 卞y，李d工，卓dy！中dz;

       x=vector (i, NPT) ;
      y=vector (1,NPT) ;
      d工＝vector (1, 甘PT) ·，
      dy=vector (1,NPT) ;
      dz=vector (1,NPT) ;
      for (j=1; j<=NPT; j++) {
           d址刃 =0. 1+ranl仕idwu) ;
           dyEj] =0. 1+ranl (kidum) ;
           d玎j] =0. 0;
           xEj] =10. 0+10. 0*gasdev (&idum) ;
           虹刃 =2. Ocx 口卜瓦 0+dy口h率sdev (&idu皿）;
           x[ j] += dx (j] *gasdev (&idum) ;
      }
      printf ( "Values of a,b, siga,sigb,chi2,q: \n") ;
      printf ( "Fit with x andy errors gives: \n") ;
      fitexy (x, y,NPT,dx,dy,ka,&b.&siga,&的gb,kchi2,kq) ;
      printf ( " 工11. 6f 7.11.6f Y.11.6f %11. 6f V.11.6f Y.11.6f\ n\n",
               a,b, siga.sigb. chi2,q) ;
    250    Numerica/ 尸ec：肛）es Examp旭 Book

      printf ( "Setting x errors to zero gives: \n") ;
      fitexy (x, y,NPT,dz,dy,ka,&b,ksiga,ksigb,&chi2,&q) ,
      printf ( "V.11. 6f/ .11.6f %11. 6f /.11. 6f %11. 6f %11. 6f\ n",
              a,b, siga, sigb, chi2,q) ;
      printf ( ". . . to be compared with fit resuit: \n") ;
      fit (x, y.RPT,dy,1,ka,kb,ksiga,&sigb,&chi2,kq) ;
      printf ( "%11. 6f 工11. 6f %11. 6f %11. 6f V.11.6f V.11. 6f\ n\n",
               a,b, siga,sigb, chi2,q) ;
      printf ( "Setting y errors to zero gives: \n") ;
      fitexy (x, y,NPT,dx,dz,&a,&b,ksiga,&sigb,kchi2,&q) ;
      printf ( "Y.11. 6f Y.11. 6f %11. 6f %11. 6f /.11. 6f %11. 6f\ n",
               a,b, siga,sigb,chi2,q) ;
      printf ( ". . .to be compared with fit resuit: \n") ;
      fit (y, x,NPT,dx,1, 立a,&b,&siga,&sigb,kchi2,tq) ;
      sa=sqrt (sigassiga+SQR(sigb* (a/b) ) )/b;
      sb=sigb/ (b*b) ;
      printf ( "/.11.6f Y.11.6f %11. 6f %11. 6f Y.11.6f '/.11. 6f\ u",
               -a/b,1. 0/b, sa, sb,chi2,q) ;
      freemvector (dz,1,NPT) ;
      free_ vector (dy,1,NPT) ;
      free_ vector (dx,1,NPT) ,
      free_ vector (y, 1,NPT) ;
      free_ vector (x, 1,NPT) ;
      return 0;
}

     if it carries out the same sort of fit as fit but this time does a linear least-
squares fit to a more general function. In sample program xif it the chosen function
is a linear sum of powers of x, generated by routine funcs. For convenience in checking
the result we have generated data according to y = 1 + 2x + 3x2 + · . .. This series
is truncated depending on the choice of NTERN, and some Gaussian noise is added
to simulate realistic data. The sig[i] are taken as constant errors. ifit is called
twice to fit the same data. The first time ia[i] is set to 1, so that ifit fits for all
the parameters: a[1] 勺 1.0, a[2] 勺 2.0, a[3] 勺 3.0.... .Then, as a test of the ia
feature, which determines which parameters are to be fit, the fit is restricted to odd-
numbered parameters, while even-numbered parameters are fixed. In this case the
elements of the covariance matrix associated with fixed parameters should be zero.
In xifit, we have set NTER11=5 to fit a 5th degree polynomial.
／卓 Driver 如r routine if it        布／

#inciude <stdio . h>
#inciude <math.h>
#inciude "nr. h"
#inciude "nrutii. h"

#define NPT 100
#define SPREAD 0.1
#defina NTER甘 5

void funcs(fioat x, fioat afuncD,int ma)
{
      mnt i;

      afunc[1] =1.0;
                                                           Cha,加r 15: Mod帥ng of I治Ia   251
      afuncL2] =x;
      for (i "3; i <=ma; i++) afuncLi] =sin(i* x) ;
}

jot main(void)
{
     long id피n ' (- 911) ;
     lot ].,j, *ia;
     float chisq, 卞a，中工，卓y，京sig，卓卞covar;

     larlvector (1, NTERM) ;
     a= ve Ct or ( 1, NTERM )
     x= vector (1,NPT) ;
     y=vector (1,NPT) ;
     sig=vector (1,NPT) ;
     covarrmatrix (1 ,NTERM, iNTERN) ;

     for (i=1; i<=NPT; i++) {
         x［幻 =0. 卄1;
         funcs (x［幻 , a, 町ERN) ·，
         y Li] = 0 .0;
         for (j= i; j<=NTERM; j++) 虹口 += 伊缸刃 ;
         y［口 += SPREAD卓gasdev（立idu皿）;
         sig[ i] =SPREAD;
     }
      for (i= i; i <=NTERN; i++) iaLj] =1;
      lfit (x, y, sig, NPT, a, ia, 甘TERM, covar,&chisq, funcs) ;
      printf ( "\ n'/.iis %21s\n", "pazameter" , "'uncertainty") ;
      for (i= i ; i<=NTERM; i++)
            printf ( " a[7.ld] = 7.8. 6f %12. 6f\ n",
                i, aLi] ,sqrt (covar[i] Li] ));
     printf ( "chi- squared = %12f\n" , chisq) ;
     printf ( "full covariance matrix\n") ;
      for (i= i; i<rNTERM; i++) {
            for (j= 1; j<=NTERN; j++) printf ( "Y.12f ", covarLi그[ j] );
           prixitf ( "\ n") ;
     }
     printf ( "\ npress RETURN to continue. . .\n ") ;
     (void) getcharO;
     /* Now check results of restricting fit paraneters
                                                                    *1
     for (i= 2; i<=NTERM; i+=2) ia[ i] 'O;
     lfit (x, y, sig, NPT, a, ia, NTERM, covar,&chisq, f山1cs) ;
    printf ( "\ n%iis Y.21s\n" , "parameter " ,"uncertainty ") ;
     for (i= 1; i< 'NTERM; i++)
           printf ( " aL'/.ld] = %8. 6f '/.12. 6f\ n",
               l , a［幻 , sqrt (cova工 [i] ［刃 ) ) ,·
    printf ( "chi- squared = Y.12f\n", chisq) ;
    printf ( "full covari띠lce matrix\n") ;
    for (i "i; i< 'NTERN; i++) {
           for (j 'i; j<"甘TERM; j++) printf ( "%12f ", covarLi] 口] );
          printf ( "\ n") ;
    }
    printf ( "\ n") ;
    free..matrix (covar, 1,NTERN, 1,NTERN) ;
    free_ vector (sig, 1,뀨PT) ;
    free_ vector (y, i, NPT) ;
    free_ vector (x, i, NPT) ;
 252        Numerica／尸e（加es Examp旭Book

      free_vector (a, 1,ITERM) ;
      free_ivector (ia, 1,ITER3() ;
      return 0;
}

     covsrt is used in conjunction with ifit (and later with the routine svdfit)
to redistribute the covariance matrix covar so that it represents the true order of
coe佈cients, rather than the order in which they were fit. In sample routine xcovsrt
an artificial l0x 10 covariance matrix covar[i] Ci] is created, which is all zeros except
for the upper left 5 x 5 section, for which the elements are covar[i] [j] =i+j- 1. Then
two tests are performed:
 1. By setting ia[i] = I for i = 1,.. . ,10 and MFIT=5, we simulate a fit where the
    first 5 out of 10 parameters are fit. covarCi] Ci] should be returned unchanged.
    2. By setting the even elements of the ia array to 1 and the odd elements to zero,
       we simulate a fit where parameters 2,4,6,8 and 10 have been fit. The elements of
       covar[i] Ci] should be spread so that alternate elements are zero.
/卞 Driver for routine covert 小/

#inc].ude <stdio . h>
#include "nr.h'1
#include "nrutil. h"

#defina MA 10
*define MFIT 5

mnt main(void)
{
    jut i, j, sia;
    float **covar;

       ia=ivector (1,MA) ;
       covar=matri工(1,MA, 1,MA) ;
       for (i=1; i<=MA; i++)
           for (j=1; j<=MA; j++) {
               cova工(i] [j] =0.0;
               if ( (i <= MFIT) ft (j <= 片FIT) )
                    covarlil [j] =i+ j- 1;
           I.
       printf ('\ noriginal matrix\n") ,
       for (i=1; i<=MA; i++) {
           for (j=1; j<=MA; j++) printf ( "%4. 1f ' 1covarCi] [j] );
           printf ( '\ n") ;
       }
       printf ( "press RETURI to continue. ..\n ") ;
       (void) getcharO;
       printf ( "\ nTest *1 - full fitting\ n ') ;
       for (i=1; i<=MA; i++) ia[ i] =1;
       covert (covar,MA, ia1MA) ;
       for (i=1; i<=MA; i++) {
           for (j=1; j<=MA; j++) printf ( "%4. 1f ', covar (i] [j) );
           printf ( '\ n') ;
       }
       printf ( "prese RETURI to continue. . .\ll " );
       (void) getcharO;
                                                          Ch카亥er 15: 凡fodeling 可Data   253

    printf ( "\ nTest #2 - spread\n ') ;
    for (i=1; i<=MA; i++)
        for (3=1; j<=NA; j++) {
            covar[ij [j] =0. 0;
            if ( (i <= M1IT) U      (j <= MFIT) ) covar[i] [j] =i+ j- 1;
        }
    for (i=1; i<=MA; i+=2) ia[ i] =0;
    covsrt (cova.r, MA, ia, MFIT) ;
    for (i=1;i<=MA; i++) {
        for (j=1; j<=MA; j++) printf ( "Y.4.lf ", covar[i] CJ] );
        printf ( "\ n") ;
    }
    free_matrix (cova工, 1,NA. 1 ,NA) ;
    free_ivector (ia, 1,MA) ;
    ret；山그L 0;
}

   Routine svdf it is recommended in preference to if it for performing linear least-
squares fits. The sample program xsvdf it puts svdf it to work on the data generated
according to

                  F (x) = 1 + 2x + 3x2 + 4x3 + 5x4 + Gaussian noise.

This data is fit first to a five-term polynomial sum, and then to a five-term Legendre
polynomial sum. In each case sig[i] , the measurement fluctuation in y, is taken to
be constant. For the polynomial fit, the resul4ng coefficients should clearly have the
values aui] 치 i. For Legendre polynomials the expected results are:

                                           a[ 1] 穴二 3.0

                                           a［幻 公二 4.4

                                           a[ 3] 穴二 4.9

                                           缸4] 二뇝 1.6

                                           缸5] 二뇹 1.1

/s Driver for routine avdfit 中/

#include <etdio .h>
卄I工c].ude <math.h>
#include "nr. h"
#include 'nrutil. h"

#define NPT 100
#define SPREAD 0.02
#define NPOL 6

mlit main(void)
{
    long idu皿＝(- 911) ;
    ml1t i;
    float chisq,牛工1+y1卞eig,*a.字日1中*cvm, 牛卞U, 卞卓V;

    x=vector (1,NPT) ;
    y=vector (1,NPT) ;
 254     Num可乞可 F相（加es Examp旭 Book

    sig=vector (1, 甘PT) ;
    a=vector (1,NPOL) ;
    w=vector (1,NP0L) ;
    cva=matrix (i ,NPOL, 1,NPOL) ;
    u=matrix (1,NPT, i, NPOL) ;
    v=matrix(1,NP0L, 1,IP0L) ;
    for (i=1; i<=NPT; i++) {
        工［幻 =0.02杜 ;
        叭j] =1. 0＋玎j] *(2. 0＋工[i] s(3.0+江j] *(4. 0+妊j] 帖 . 0) )) ;
        y[i] 巾= (1.0+SPREADsgasdev (kidum) );
        sig Ci] = y [j] *SPREAD;
    }
    svdfit (x, y, sig, NPT, a,NPOL,u,v.w,kchisq,fpoly) ;
    svdvar (v, NPOL, v, cvui) ;
    printf ( "\ npolynomial fit: \n\ n") ;
    如r (i=1; i <＝且POL; i++)
        printf ( "Y.12. 6f %s %10. 6f\ n", a[i] ," +-", sqrt (cvm[i] Ci] ));
    printf ( "\ nChi-squared '/.12.6f\ n", chisq) ;
    svdfit (x, y, sig, 月PT,a,NPOL,u,v,w,&chisq, fleg) ;
    svdvar (v, NPDL, w, cvm) ;
    printf ( "\ nLegendre polynomial fit: \n\n") ;
    for (i= 1; i<=NPOL; i++)
        printf ( "/.12. 6f 加 %10. 6f\ n", a[i] ,'   +-",sqrt (cvm[i] Ci] ));
    printf ( "\ nChi-squared Y.12. 6f\ n' , chisq) ;
    free_matrix (v, 1,甘POL, 1,NPOL) ;
    free_matrix (u, 1,NPT,1,NPOL) ;
    free_matrix (cvm, 1,NPOL, 1,NPOL) ;
    free_的ctor（吼 1 ,NPOL) ;
    free_ vector (a, 1,NPOL) ;
    fre乞四ctor佃ig, 1，甘PT) ;
    free_ vector (y, 1, NPT) ;
    free_ vector (x, 1 ,NPT) ;
    return 0;
}

    svdvar is used with svdf it to evaluate the covariance matrix cvm of a fit with
MA parameters. Iii program xsvdvar, we provide input vector w and array v for this
routine via two data statements, and calculate the covariance matrix cvm determined
from them. We have also done the calculation by hand and recorded the correct
results in array tru for comparison.
／卞 Driver 如r routine svdv缸 卞／

#inclucie <stdio . h>
*include "nr. h"
#include "nrutil. h'1

#define NP 6
#define MA 3

mnt main(void)
{
    mnt i, j;
    float; 牛字cvm, 卞字V;
    static float vtemp[IP] [NP] =
        {1. 0.1. 0,1.0,1.0,1.0,1.0,
        2.0,2.0,2.0,2.0, 2.0,2.0,
                                                           Ch햐升or 15: Mode片ng 可Data   255
         3.0,3.0,3.0,3. 0,3.0,3.0,
         4. 0,4.0,4.0,4.0,4. 0,4.0,
          5.0,5. 0,5. 0,5.0,6.0,6.0,
         6.0,6. 0,6.0 , 6. 0,6. 0,6. 0);
     static float 日[NP+1] =
         {0 .0,0.0,1.0,2. 0,3.0,4.0,5.0);
     static float tru[ MA] [MA] =
         {1. 25, 2.s, 3.75,
         2.5,5.0,7.5,
         3. 75,7.5,11. 25) ;

      cvmrinatri工(1, HA,1,MA) ;
      v'convert_matrix(kvt이p[O] [0] ,1, NP,1,NP) ;
     printf ( "\ n皿atrix v\n") ;
      for (i=1; i<=WP; i++) {
          for (j= 1; j<=NP; j++) printf ( "/.12.6f ", v[i] [j] );
          printf ( "\ n") ;
      }
     printf ( "\ nvector w\n ") ;
     如r (i=1; i<＝月I'; i++) printf ( "%12.6f " 戶口］) ;
    printf ( "\ n") ;
     svdvar (v,MA, v, cvm) ;
    printf ( "\ ncovariance matrix from svdva.r\ n") ;
     for (i=1; i<'MA; i++) {
          for (j=1; j<=MA; j++) priutf ( "%12.6f ", cvm[i] [j] );
          printf ( "\ n") ;
     }
    printf ( "\ nexpected covariance matrix\n") ;
    for (ir1; i<=NA; i++) {
          for (j=1; j<=MA; j++) printf ( "%12. 6f ", tru[ i- 1] [j- 1] );
          printf ( "\ xi") ;
    }
    free_的nvert_m毗工ix (v, 1,甘p,1, 川）) ;
    free_matri工 (cvm,1,MA,1,片幻 ;
    return 0;
}

   Routines fpoly and f leg were used above with sample program xsvdf it to
generate the powers of x and the Legendre polynomials, respectively. In the case of
fpoly, sample program xfpoly below is used to list the powers of x generated by
fpoly so that they may be checked "by eye". For f leg, the generated polynomials
in program xf leg are compared to values from routine plgndr.
/卓 Driver for routine fpoly */

#include <stdio.h>
#include "nr. h"
#include "nrutil. h"

#define NVAL 15
#define DX 0.1
#def ins NPOLY 5

mllt main(void)
1
    mlit i, j;
    float x, *afunc;
256       Numerical Recipes Example Book


    afunc=vector (1,NPOLY) ;
    printf ( "\ &/.38s\n", "powers of x") ;
    printf ( "%88 %10s %9日 %9日 %9s %9s\n",
        1' 工 " 1 " 工＋卞0", " 工卞卞1", "工中卞2", " X中中3" ' " 工牛京4, );
    for (i=1;i<rIVAL;i++) {
        工＝1方DX;
        fpoly(x, afunc ,NPOLY) ;
        printf ( "%1D. 4f ", x) ;
        for (j=1; j<=NPOLY; j++) printf ( "%10. 4f ", afunc[ j] );
        printf ( "\ n") ;
      }
      free_vector (afunc,1,NPOLY) ;
      return 0;
}
/* Driver for routine fleg */

*include <stdio . h>
#include "nr.h"
#include "nrntil. h"

#define NVAL S
#define DX 0. 2
#define NPOLY S

jut main(void)
{
    jut i, j;
    float x,*afunc;

    afunc=vector ( 1, NPOLY) ;
    printf ( "\ n%3s\n" ,"Legendre polynomials") ;
    printf ( "%9s '/.gs %9s 工9s 工9s\u", "n=1", "n=2", "n=3", "a=4", "n=5") ;
    for (i=1; i<=NVAL;i++) {
        工＝1.求DX;
        fleg(x,afunc,月P0LY) ;
        printf ( "x =工5. 2f\n", x) ;
        for (j=1; j<=IP0LY; j++) printf ( "%10.4f ", afuncCj] );
        prjntf ( " routine FLEG\n") ;
        for (j=1; j<=NPOLY; j++) printf ( "%10. 4f ", plgndr (j- i, 0, x) );
        printf ( " routine PLG且DR\n\n") ;
      }
      free_vector (afunc,1, IPOLY) ;
      return 0;
}

   mrqmin is used along with mrqcof to perform nonlinear least-squares fits with the
Levenberg-Marquardt method. The artificial data used to try it in sample program
xmrqmin is computed as the sum of two Gaussians plus noise:

                 y同 = a[1] exp{ -[(xEi] - a[2])/a[3] ]2}
                       +a[4] exp{-[(x[ i] -a[ 5] )/a[6] ]2) + noise.

The a[i] are assigned at the beginning of the program, as are the initial guesses
gues Ei] for these parameters to be used in initiating the fit. Also initialized for the
                                                       Ch카가er 15: Mode初g 可Da伯           257

fit are ia[ iJ=i for i=1, . . ,mf it to specify that all six of the parameters are to be fit.
On the first call to mrqmin, alamda=-1 to initialize. Then a loop is entered in which
mrqmln is iterated while monitoring successive values of chi-squared chisq. When
chisq changes by less than 0.1 on two consecutive iterations, the fit is considered
complete, and Inrqmin is called one final time with al키nda=0 .0 so that array covar
will return the covariance matrix. Uncertainties are derived from the square roots of
the diagonal elements of covar. Expected results for the parameters are, of course,
the values used to generate the "data" in the first place. As a test of the ia feature,
the fit is redone holding fixed a[2] =2 and a[5] =5.
/* Driver for routine mrqmin */

#include <stdio.h>
#include <math. h>
#include "nr. h"
#include 'nrutil. h"

#define NPT 100
#define 片A 6
#define SPREAD 0. 001

m1lt inain(void)
{
    long iduin= (- 911) ;
    mnt i, *ia, iter, itst, j, k,mfit=MA;
    float aiamda, chisq, ochisq，卞x，中y，半518，中卞covar,＋中alpha;
    static float a[MA+13 =
        {o .0, 5. 0, 2. 0,3. 0, 2.0,5. 0, 3. 0} ;
    static float gues[NA+1] =
        {0 .0, 4. 6,2. 2, 2. 8, 2.5,4. 9, 2. 8} ;

    ia=ivector (1,MA) ;
    工＝vect or C I , 甘PT) ;
    y=vector (1,NPT) ;
    sig=vector (1,NPT) ;
    cova.r=matrix (1,MA, l, MA) ;
    alpha=matrix (1,MA,1,MA) ;
    /中 First try a sum of two Gaussians */
    for (i=1; i< rNPT; i++) {
         址i] =0. 1卞i ;
         y[i] =0. 0;
        for (j=1; j<=MA; j+=3) {
             姓i] += a口] *exp（占餌（（虹i] -a口+1] )/a口+2] )) ;
        ).
        y［幻 卞＝ (1. 0+SPREAD中gasdev (Aidu皿）);
        sig[ i그 =SPREAD卞y Ii] ;
    }
    for (i=1; i<=mfit; i++) ia[ i] =1;
    如r (i=1; i<=MA; i++) a［幻＝8的5［幻 ;
    for (iter= 1;iter< =2; jter++) {
        alanda = -1;
        mrqmin(x ,y , sig,NPT, a, ia, XA, covar .aipha,kchisq, fgauss 潼aiamda) ;
        k=1;
        itst= 0;
        如r (; ; ) {
             printf (八n%s '/.2d 7.17s %10. 4f '/,lOs %9. 2e\n' , " Iteration 8" ,k,
258       Numerica사？e야仍 Exa쨔兆 Book

                   "chi- squa工ad: ", chisq,"a].ainda: ", alalsda) ;
               printf ( "%8s %8s %8s %8s %8s %85\n",
                   " a[l] " , " 缸2] " , "a[3] "1" a[4] " , " a[5] " , " 缸6] " );
               for (i=1; i<=6;i++) printf ( "%9.4f ", aEi] );
               printf ( "\ n") ;
               k++ ;
               ochisq=chisq;
                                                                                   a) ;
               mrqmin(x, y, sig,NPT,a, ia, 札1, cova工, alpha,kchisq, fgauss,&ala皿d
               if (chisq > ochisq)
                     itst= 0;
               else if (fabs(ochisq-chisq) < 0.1)
                     itst+ +;
               if (itst < 4) continue;
               al깁nda'0. 0;
                                                                                       ;
               inrqinin(x, y, sig,NPT,a,ia, MA, covar, alpha,&chisq, fgauss, kala皿da)
               printf ( "\ nUncertainties: \n") ;
                for (i=1; i<=6; i++) printf ( "%9. 4f ", sqrt (covar[il[ i] ));
               printf ( "\ n") ;
               printf ( '\ nExpected results: \n") ;
               printf ( " %7. 2f %8. 2f 工8. 2f %8. 2f %8. 2f '/,8.2i\ n",
                        5.0,2.0,3.0, 2.0,5.0,3.0) ;
               break;
          }
          if   (iter == 1) {
               printf ( "press return to continue 日ith constraint\n") ;
               (void) getcha工O;
               printf ( 'holding a[2] 띠ld a[5] constant\n") ;
               for (j=1; j<=MA; j++) a[ j] += 0. 1;
                a［幻＝2.0;
                ia［幻 =0;
                缸旬＝5. 0;
                ia[ 5) =0;
          }
      }
      free_matrix(alpha,1,MA, 1,MA) ;
      free_matrix (covar,1,NA, 1,MA) ;
      free_ vector (sig, 1,NPT) ;
      free_ vector (y, 1,NPT) ;
      free_ vector (x, 1,NPT) ;
      free_ ivector (ia, 1,MA) ;
      return 0;
}

    The nonlinear least-squares fit makes use of a vector /3k (the gradient of x2 in
parameter-space) and cs,a (the Hessian of x2 in the same space). These quantities are
produced by mrqcof, as demonstrated by sample program xmrqcof. The function is
a sum of two Gaussians with noise added (the same function as in xmrqmin) and it is
used twice. In the first call, ia[ i] =1 and mfit=6 so all six parameters are used. In
the second call, ia[ i] =0 for i=1, 2,3 and mfit=3 so the first three parameters are
fixed and the last three, a[4] .. . af6] are fit. Here is the output you should get:
matrix alpha
    137. 2021           60. 6572       148. 2204        147. 7027       -12. 6093     90. 9625
     60. 6572          500. 8828       366. 9686        448. 3022       287. 4484    257.7019
    148. 2204          366. 9686       583. 6553        659. 6396       553. 0109    612. 6782
    147. 7027          448. 3022       659. 6396        971. 0057      1131. 7701   1410. 9380
                                                        Chapter 15: Modeling of Data   259
     -12. 6093      287. 4484     553. 0109    1131. 7701    1911. 5935   2409. 3484
      90. 9625      257. 7019     612. 6782    1410. 9380    2409. 3484   3341. 0002
vector beta
     -24. 7629    -118. 2998      -76. 5074    -124. 1268    -104. 8776   -145. 4018
chi- squared:       147. 9271
matri工 alpha
     971. 0057    1131. 7701    1410. 9380
   1131. 7701     1911. 5935    2409. 3484
   1410. 9380     2409. 3484    3341. 0002
vector beta
   -124. 1268     -104. 8776    -145. 4018
chi- squared:       147. 9271

/t Driver for routine mrqcof */

#includa <stdio. h>
#include <math. h>
#include "nr. h"
#include "nrutil. h"

#define NPT 100
#define MA 6
#clefine SPREAD 0. 1

mnt main(void)
{
    long idujn" (- 911) ;
    m1lt i, j, mfit14A. *ia;
    float chisq, 京beta, 本x！卞y，卞sig，京卞covar，李taipha;
    static float 缸MA+1] =
         {o .0, 5. 0, 2. 0,3. 0, 2. 0, 5. 0, 3. 0);
    static float gues[MA+1] =
         {0. 0, 4. 9, 2. 1, 2. 9, 2. 1,4. 9,3. 1);

    ia=ivector (1 , 片A) ;
    beta=vect or C 1, MA) ，·
    x=vector (1,NPT) ;
    y= vector (1,NPT) ;
    sig=vector (1,NPT) ;
    covar=matrix (1,MA, 1 小A) ;
    alpha=matrix (1,MA, 1,MA) ;
    /* First try sum of two gaussians */
    for (i=1; i<'NPT; i++) {
         x［刃 =0. 1卞1;
         y［幻 =0 刀;
         虹i] += aEl] 卞exp（占畔（  （江1.卜M幻 )/a[ 3] )) ;
         y[i] += 缸4］京exp（田QR ( (xli卜缸旬）/a臼n) ．·
         y［幻 卞＝ (1. 0+SPREAD*gasdev（立id山a) );
         sig［幻 =SPREA먀虹ii ;
    }
    for (i=1; i<=mfit; i++) ia[ i] =1;
    for (i 'l; i<=mfit; i++) ali] =gues[i] ;
    mrqcof (x, y, sig, NPT, a, ia, MA, alpha,beta,kchisq, fgauss) ;
    printf ( "\ nmatrix alpha\n") ;
    for (i=1; i<=MA; i+ -i) {
        for (J=1; j<=MA; J++) printf (叫.12.4f ", alphali] [j] );
        printf ( "\ n") ;
260      N切加nc別尸6뺘）es Example Book

    }
    printf ( "vector beta\n") ;
    for (i '1; i<=MA; i++) printf ( "%12. 4f ", beta[i] );
    printf ( "\ nchi-squared: %12. 4f\n\n" ,chiaq) ;
    /京 Next fix one line and improve the other 卞/
    mfit=3;
    for (i=1; i<=mfit;i++) ia[ i] =0;
    for (i=1; i<=MA; i++) 缸i] =g的町i] ;
    mrqcof (x,y,aig,NPT, a,ia, MA, alpha,beta,kchisq,fgausa) ;
    printf ( "matrix aJ.pha\n") ;
    for (i=1; i<=mfit;i++) {
        for (j=1; j<=mfit; j++) printf ( "%12.4f ", alphaCi] [j] );
        printf ( "\ n") ;
    }
    printf ( "vector beta\n") ;
    for (i "l; i (=mfit; i++) printf ( "工12. 4f ", beta[i] );
    printf ("\ nchi-squared: %12. 4f\n\n", chiaq) ;
    free_matri工(alpha,1,片A,1,MA) ;
    free_matrix(covax,1,MA 11,NA) ;
    free_vector (sig, 1,IPT) ;
    free_vector (y, 1,NPT) ;
    free_vector (x,1,NPT) ;
    f ree_vector (beta,1,NA) ;
    free_ivector (ia, 1,XA) ;
    return 0;
}

    fgauss is an example of the type of procedure that must be supplied to mrqf it
in order to fit a user-defined function, in this case the sum of Gaussians. fgauss
calculates both the function, and its derivative with respect to each adjustable pa-
rameter in a fairly compact fashion. The sample program xfgauss calculates the
same quantities in a more pedantic fashion, just to be sure we got everything right.
／卞 Driver 如r routine fgausa 卞／

#include <stdio .h>
#include <math.h>
#include 'nr.h"
#include "nrutil. h"

#def ins NPT 3
#def ins ILIN 2
#def ins NA 3中月LII

mnt main(void)
{
    mllt i, j;
    float el, e2,f, x,y;
    static float a[NA+1] {O. O, 3. 0,0. 2,O. 5,1. O,0. 7,O. 3};
    float dyda[NA+1] ,df [NA+i] ;

      printf ( "\ n工6s %8a V.8s %7a %7s %7s %7s %7s\n",
          "x", "y", "dydal", "dyda2", "dydas", "dyda4", "dyda5", "dyda6") ;
      如r (i "l; i<:＝甘PT; i++) {
          工＝0,3*i;
          fgausa (x,a,&y,dyda,IA) ;
          el=exp(- SQIt( (x-a[2] )/aC3] ));
                                                        C/i카升er 15: Mo旭加g 可Data      261

        e2=exp(- SQR( (x-a[5] )/a[ 6] )),
        f=a口］卞el+a［幻 卞e2;
        df[ 1] =e1;
        df[ 4] =e2;
        df[ 2J =a口］卞el中2. 0卓 仕-a[2] )/(a臼Js町키 ) ;
        diEs] a［幻 中e깐2. 0CC戶缸旬 ) /（缸旬 卓a［幻 ) ;
        di [3] =a[1] *el* 2 . 0*SQR(x-a[2] )/(a[ 3] *a[3] aa[3] );
        di [6] =a[4] 卓e2卞2. 0卞SQR（工-a [5] )/(a[ 6] 卓a[6] 卓a[8] ) ;
        printi ( "irom FGAUSS\n') ;
        printi ( "7.8. 4f Y.8. 4i ", x, y) ;
        for (y1; jc=6; j++) printf ( '%8. 4i ' , dyda[ j] );
        printf ( '\ nindependent calc. \n") ;
        printf ( "%8. 4f %8. 4i ", x,i) ;
        for (j=1; j< '6; j++) printf ( "%8. 4f ", di[ j] );
        printi ( '\ n\n") ;
    }
    return 0;
}

     medf it is a routine illustrating a more "robust" way of fitting. It performs a fit
of data to a straight line, but instead of using the least-squares criterion for figuring
the merit of a fit, it uses the least-absolute-deviation. For comparison, sample routine
치nedf it fits lines to a noisy linear data set. using first the Ieast-souares routine fit.
anu tnen tne ieast-aosoiute-aeviation routine meanl-c. You may De interesteo to see
if you can figure out what mean value of absolute deviation you expect for data with
gaussian noise of amplitude SPREAD.
／衣 Driver 如r routine mediit 中／

#include <stdio . h>
*include 'nr. h"
#include "nrutil. h"

#deiine IPT 100
#deiine SPREAD 0. 1
*deiine IDATA NPT

milt main(void)
{
    long i4um=(- 1984) ;
    mllt 치m日t=1;
    float a,abdev,b, chi2,q,siga,sigb;
    float 卞l1+y1衣sig;

    x=vector (11NDATA) ;
    y=vector (11NDATA) ;
    日ig=vector (1,NDATA) ;
    for (i=1; i<=NPT; i++) {
         虹i] =0. lsi;
         y[i] = -2. 0*x[i] +1. 0+SPREADsgasdev(kiduia) ;
         sig Ci] =SPREAD;
    }
    iit (x, y ,IPT,sig, m日t,ka,*b,k叭甲,k的gb,kchi2,&q) ;
    printf ( "\ nAccording to routine FIT the result is: \n") ,
    printf ( "    a = %8. 4f    uncertainty: X8. 4f\ n ', a,siga) ;
    printi ( "    b = XS. 4f    uncertainty: %8. 4i\ n", b. sigb) ;
    262       Numeric削／羽帥）es Exam工1e Book

      printf ( '    chi- squared: %8. 4f for h4d points\n", chi2,NPT) ;
      printf ( "    goodness-of- fit:     7.8.4f\ n", q) ;
      printf ( "\ nAccording to routine MEDFIT the result is: \n") ;
      medfit (x, y.NPT,ka,&b,&abdev) ;
      printf ( "    a = Y.8.4f\ n", a) ;
      printf ( "    b = V.8.4f\ n' , b) ;
      printf ( "    absolute deviation (per data point) : %8. 4f\ n", abdev) ;
      printf ( '    (note: gaussian SPREAD is %8. 4f) \n' , SPREAD) ;
      Ire乞的ctor佃ig. 1.NDATA) ;
      free_ vector (y, 1,RDATA) ;
      free_ vector (x, 1.NDATA) ;
      return 0;
}
      rofunc is an auxiliary function for medf it. It evaluates the quantity
                                    N
                                   Z 小恥（yi卜 (z- bxi)
                                   i=1

given arrays x2 and !/ j. Data are communicated to and from rot unc primarily through
global variables, but the value of the sum above is returned as the value of rofunc (b).
abdev is the summed absolute deviation, and aa (listed below as a) is given the value
that minimizes abdev. Our results for these quantities are:
              b        a      ROFUNC       ABDEVT
          -2.10     1.51      249.80        25.17
          -2.08     1. 40     247. 40       20. 20
          -2.06     1.30      247. 40       15. 25
          -2. 04    1.21      231. 20       10. 36
          -2. 02    1.11      193.60         5. 92
          -2.00     1. 00     -15.60         3. 75
          -1.98     0. 89    -199.20         6.00
          -1.96     0.80     -234. 40       10.40
          -1. 94    0.71     -247.20        15. 25
          -1. 92    0.60     -247.20        20. 19
          -1. 90    0. 51    -247.20        25. 14

/本 Driver for routine rofunc 卞/

#include <stdio.h>
#inc].ude "nr. h"
#include "nrutil. h"

#define SPREAD 0.05
#define NOATA 100

m11t ndatat; /卞 defining declaration */
float *xt, *yt. aa,abdevt;   /s defining declaration */

m1lt main(void)
{
      long iduni=(- 11) ;
      ml1t i;
      float b,rf, sx,*y;

      工＝vector (1,NDA丁A) ;
      y=vector (1,NDATA) ;
                                                       Ch랴ter 15: Modeling of Data   263
    ndatat=NDATA;
    xt =x;
    yt =y;
    for (i= 1; i<rNDATA; i++) {
         x［幻 =0. 什i．·
         虹ii = -2. 0卞x [i] +1. 0+SPREAD卞gasdev（立idu皿）;
    }
    printf (叫.9s %9s V.12s %los\n' , "b '", "a", "ROFUNC", "A BDEVT") ;
    for (i = -5; i <=5; j++) {
         b = m 2. 0+0. 02* j;
        rf= rofunc (b) ;
        printf ( "Y.10. 2f %9. 2f %11. 2f %10. 2f\ n",
             b, aa,rf, abdevt) ;
    }
    fre&.vector (y, 1,NDATA) ;
    free. VeCtor (X,1,NDATA) ，·
    retUrn 0;
}
Chapter 16: Ordinary Differential Equations

           Chapter 16 of Numerical Recipes deals with the integration of ordinary
      differential equations, restricting its attention specifically to initial-value prob-
      lems. Three practical methods are introduced: 1) Runge-Kutta methods (rk4,
      rkdumb, rkqs, and odeint), 2) Richardson extrapolation and the Bulirsch-
      Stoer method (bsstep, mmid, stoerm, rzextr, pzextr), 3) predictor-corrector
      methods. In general, for applications not demanding high precision, and
       where convenience is paramount, Runge-Kutta with adaptive step-size con-
       trol is recommended. For higher precision applications, the Bulirsch-Stoer
      method dominates. The predictor-corrector methods are covered because of
       their history of widespread use.
          Stiff differential equations require special methods. Routine stiff uses
      a generalization of Runge-Kutta, known as a Rosenbrock method. The semi-
      implicit midpoint extrapolation method is a Bulirsch-Stoer method designed
      for stiff equations, and implemented in stifbs.
                                         士   士    女   女



    Routine rk4 advances the solution vector yEn] of a set of ordinary differential
equations over a single small interval h in x using the fourth-order Runge-Kutta
method. The operation is shown by sample program xrk4 for an array of four vani-
ables yEt],... , y [4]. The first-order differential equations satisfied by these variables
are specified by the accompanying routine derivs, and are simply the equations de-
scribing the first four Bessel functions Jo(x),.. . , Ja(x). The y's are initialized to the
values of these functions at x = 1.0. Note that the values of dydx are also initialized
at x = 1.0, because rk4 uses the values of dydx before its first call to derivs. The
reason for this is discussed in the text. The sample program calls rk4 with h (the
step-size) set to various values from 0.2 to 1.0, so that you can see how well rk4 can
do even with quite sizeable steps.
/s Driver for routine rk4 *1

*include <stdio . h>
#include "nr. h11
#include "nrutil. h"

#define N 4

void derivs(float 치float y口 ,float dyd工口）
{
      dydx[i] = -y[ 2] ;
      dyd虹幻카[1卜(1.0八汁叭幻 ;
      dyd虹幻 斗[2卜但 . 0/x汁外3] ;


    264
                                       Ch카）旭r 16: Ordinary D肝eren卄削Equ副幻ns          265

     dyd虹幻 斗臼卜四. 0/x汁虹4] ;
 }

 jut main(void)
 {
     mnt i, j;
     float h，工＝1.0Jy '卞dyd工Jyout;

     y=vector (1,N) ;
     dydxrvector (1,N) ;
     yout=vector (1,N) ;
     y 口］=bes町0（幻 ;
     y[2] =bes町l(x) ;
     虹키 =bes町 侄x) ;
     叭幻 =bes幻 (3, x) ;
     derive（工，y,dyd工）;
     printf ( "\ n'/,16s '1.55 /.12s Y,12s '/.12s\xt",
          "Bessel function: ", "jo ", "jl ", "j3 ", "j4 ") ;
     for (i=1; i (=5;i++) {
         h=0. 2*i;
         rk4臼，dydx,瓦x,h, yo끄t,（如rivs) ;
         printf ( "\ nfor a step size of: Y,6.2f\n", h) ;
         printf ( '%125", "rk4: ") ;
         for (j=1; j<=4; j++) printf (" /.12. 6f ", yout[ j] );
         printf ( "\ n%128 %12. 6f %12. 6f %12. 6f %12. 6f\n", "actual: ',
               bessjo(x+h) ,bessjl (x+h) ,bessj (2,x+h) ,bessj (3,x+h) );
     }
     free_vector (yout, 1,月）;
     free_vector (dydx. 1,N) ;
     free中vector (y, 1，甘）;
     return 0;
J.
     rkdumb is an extension of rk4 that allows you to integrate over larger intervals. It
is "dumb" in the sense that it has no adaptive step-size determination, and no code to
estimate errors. Sample program xrkdumb works with the same functions and deriva-
tives as the previous program, but integrates from x1=1.0 to x2=20 .0, breaking the
interval into NSTEP=150 equal steps. The variables vstart [1], . . . , vstart [4] which
become the starting values of the y's, are initialized as before, but their derivatives
this time are not initialized; rkdumb takes care of that. This time only the results for
the fourth variable 兀(x) are listed, and only every tenth value is given.
/* Driver for routine rkduinb */

#include <stdio . h>
#include "nr.h"
#include "nrutil. h"

*define NVAR 4
#define NSTEP 150

void derivs (float x,float yD, f].oat dydx[])
{
   dydx[1] = -y[ 2] ;
   dyd址幻 카 [1卜(1.0八汁虹2] ;
   dyd玎幻카 [2卜但 . olx汁虹3] ;
    266       Numerica／尸ec徊es Examp旭 Book

      dy缸[4] =y同m侮.0八汁虹幻 ;
}

8工tern fl oat 卞卞y，卞xx;          ／卞 referencing declaration 卞／

mllt main(void)
{
          mllt j,
          float x1=1.0,x2=20.0,*vstart;

      vstart=vector (11 NVAR) ;
      ／卞 如te: The arrays 工工 and y must have indices up to 甘STEP+1     卓／
      xx=vector (1,NSTEP+1) ;
      yosatrix (1,NVAft, 1,NSTEP+1) ;
      vstart 口] =bessj0(x1) ;
      vstart[ 2) =bessjl (xl) ;
      vstart [3) =bessj (2，工i) ;
      vstart[ 41=be8sj (3 ,xl) ;
      rkdumb(vstart, WVkR, x11x2,NSTEP,derivs) ;
      printf ( '%8s %17a %los\n", "x", "integrated", "bessj3") ;
      for (j= 10; j<=NSTEP; j+=10)
          printf ( "%10. 4f X14. 6f %12. 6f\ n' ,
               xx[ j] ,y[ 4] Ej) ,bessj (3,xx[ j3) );
      free_matrix (y, 1,NVAR, 1, NSTEP+1) ;
      free_ vector (xx,1 NSTEP+1) ;
      free. vector (vstart, 1 ,NVAR) ;
      return 0;
}

    rkqs performs a single step of fifth-order Runge-Kutta integration, this time
with monitoring of local truncation error and corresponding step-size adjustment. Its
sample program xrkqs is similar to that for routine rk4, using four Bessel functions
as the example, and starting the integration at x = 1.0. However, on each pass a
value is set for eps, the desired accuracy, and the trial value htry for the interval size
is set to 0.6. For the first few passes, eps is not too demanding and htry may be
perfectly adequate. As eps becomes smaller, the routine will be forced to diminish h
and return smaller values of lidid and hnext. Our results (in single precision) are:
              eps       htry           hdid               hnext
           0. 367879    0. 60        0.600000           3.000000
           0. 135335    0. 60        0.600000           2.542155
           0. 049787    0.60         0.600000           2.081340
           0. 018316    0.60         0.600000           1.704057
           0.006738     0.60         0.600000           1. 395164
           0.002479     0.60         0.600000           1. 142264
           0.000912     0.60         0. 600000          0. 935206
           0.000335     0. 60        0. 600000          0. 765682
           0. 000123    0. 60        0. 600000          0. 626888
           0.000045     0. 60        0. 506775          0. 513415
           0. 000017    0. 60        0. 394677          0. 421229
           0. 000006    0. 60        0. 307374          0.346002
           0. 000002    0. 60        0. 239383          0. 284358
           0.000001     0.60         0.186432           0. 233682
           0.000000     0. 60        0.145193           0.191925
                                      Gb햐升er 16: Ord加ary D肝erent洌Equaf幻ns         267

／本 Driver for ro끄tine rkqs 卓／

#include <stdio . h>
#include <math.h>
#include 1'nr. h"
#include "nrutil. h"

#define N 4

void derivs (float x,float yD, tloat dydxD)
{
    dydx[1] = -y[ 2] ;
    dyd工［2] =y [1] 寸（1. 0／工）字y [2] ;
    dydx[3]=y[2] -(2. 0/x)*y[3] ;
    dycix[4]=y[3:l- (3. 0/x)*y[ 4] ;
}

m1lt inain(void)
{
    mnt i, j;
    float eps ,hdid,linext小缸y, x=1 刀Jy1京dydx, *dysav, 水ysav, *恥cal;

    yrvector (1, 甘) ;
    dydx=vector (1,N) ;
    dysav=vector (1,N) ;
    ysav= vector (1,N) ;
    yscal=vector (1,N) ;
    邪av [1卜bess叩佃）;
    ysa吐기 =bessjl(x) ;
    ysav[3] =bessj (2, x) ;
    ysav[4] =bessj (3, x) ;
    derivs (x, ysav,dysav) ;
    for (i=1; i<=N; i++) yscalEi]=1.0;
    htry=0.6;
    printf ( "%los Y.lls %12s /.13s\n" ,"eps", "htry", 'hdid", "hnext") ;
    for (i=1; i<=15; i++) {
        eps=exp( (double) -i) ;
        x=1.0;
        for (j=1; j<＝甘; j++) {
              虹刃카距吐ii;
              dydxEj] =dysavtj] ;
        }
        rkqs(y, dydx ,N ,&x,htry, eps,yscal.khdid,&뇨lext,derivs) ;
        printf ( '%13f %8. 2f %14. 6f 7.12.6f \n", eps,htry, hdid,hnext) ;
    }
    free_ vector (yscal,1.N) ;
    free_ vector (ysav,1,N) ;
    free_ vector (dysav11, 且) ;
    free_vector (dydx,1,N) ;
    free_ vector (y, 1.N) ;
    return 0;
}

    The full driver routine for rkqs, which provides Runge-Kutta integration over
large intervals with adaptive step-size control, is odeint. It plays the same role for
rkqs that rkdumb plays for rk4. Integration is performed on four Bessel functions
    268    Numerical Recipes Example Book

from xl=1. O to x2=10. O, with an accuracy eps=1. Oe-4. Independent of the values
of step-size actually used by odeint, intermllediate values will be recorded only at
intervals greater than dxsav. The sample program returns values of .13(x) for checking
against actual values produced by bessj. It also records the number of function
evaluations used, how many steps were successful, and how many were "bad". Bad
steps are redone, and indicate no extra loss in accuracy. At the same time, they do
represent a loss in e佈ciency, so that an excessive number of bad steps should initiate
an investigation.

/希 Driver for routine odeint */

#include <stdio . h>
#include "nr. h"
#include "nrutil. h"

#define N 4

float dxsav，卞xP，京卞yp;        ／本 defining declarations 衣／
jut kniax,k叫毗 ;

mnt nrhs;       /中 counts function evaluations 卞/

void derivs (float 工，float y口 ,float        dyd工口）
{
    nrhs++;
      dydx [1] = 1y [2] ;
      dydxE2] =y[1] -(1. 0/ x)*y[ 2] ;
      dyd玎引카 [2卜(2. 0/x汁虹幻 ;
      dyd虹幻 斗臼卜臼. 0/x汁虹4] ;
}

jut main(vojd)
{
      jut i, nbad,nok;
      float eps=1.oe-4,hl=0.1,hmin=0.0,xl=1.0,工2=10. 0,*ystart;

      ystart=vector (1,N) ;
      xp=vector (1,200) ;
      yp=matr ix (1, 10,1, 200) ;
      ystart[ 1] =bessjo(xl) ;
      ystart[ 2] =bessjl(xl) ;
      恥tart 口] bess叭之xl) ;
      ystart [4] =bessj (3 ,xl) ;
      nrhs=0;
      kmax= 100;
      dxsav=(x2-xl) /20 .0;
      odeint (ystart, N, xl, x2, eps,hl, hmin,knok,&nbad,derivs,rkqs) ;
      printf ( "\ n%s 7.13s Y,3d\n", "successful steps: ", " ", nok) ;
      printf ( "%s Y.20s Y.3d\n", "bad steps: ", " ", nbad) ;
      printf ( "Y.s Y.9s Y.3d\n", "function evaluations: ", " ", nrh的;
      printf ( "\ n加 %3d\n", "stored intermediate values:           ", kount) ;
      printf ("\ nY.8s Y.18s %l5s\n", "x", "integral ", "bessj (3, x) ") ;
      for (j=1; j<=kount; j++)
          prjntf ( "/.10.4f '/.16.6f 工14. 6f\ n",
             xp[i] ,yp[4] Ci] ,bessj (3,工p[i] ));
      free_matrix (yp,1,10,1, 200) ;
                                             Gb邵）旭r 16: Ord加ary 0肝erent洌Equa的(is    269
         free_ vector (xp, 1, 200) ;
         free_ vector (ystart, 1, N) ;
         return 0;
    }

     The modified midpoint routine minid is presented in Numerical Recipes
                                                                                primarily
 as a component of the more powerful Bulirsch- Stoer routine. It integrates variables
over an interval htot through a sequence of much smaller steps. Sample routine xm皿id
takes the number of subintervals i to be 5, 10, 15, . . . ,50 so that we can witness
                                                                                     any
improvements in accuracy that may occur. The values of the four Bessel functions
are compared with the results of the integrations.
／卞 Driver 如r routine maid 卓／

#include <stdio.h>
#include 'nr. h"
#include "nrutil. h"

#define NVAR 4
#define Xl 1.0
#define HTOT 0.5

void derivs (float x, float y[],float         dydxD)
{
        dydx [1] = -y [2] ;
        dyd虹기 카 [1卜(1.0八）切[2] ;
        dyd虹引斗 m卜仁 .0八汁虹3] ;
        dy缸［幻 =y [3] -侮 . 0/x汁虹幻 ;
}

ml1t main(void)         '
{
        mnt i;
        float bl, b2,b3,b4, xf＝工1+HTOT，求y．卞yout，卞dyd工；

         y"vector (l, NVAR) ;
         yout=vector (1,NVAit) ;
        dydx=vector (1,NVAR) ;
        y[1] 'bessjO(Xl) ;
        址幻 =bes町 lOu) ;
        虹幻 =bess叭之 Xl) ;
        吐幻 =bee幻 (3, XI) ;
        derivs (X1, y,dydx) ;
        bl=bessjO(xf) ;
        b2=bessj1(xf) ;
        b3=bes8j (2, xf) ;
        b4=be55j (3, xf) ;
        printf ( "First four Bessel functions: \n") ;
        for (i=5; i<=50; j+=6) {
            mmid(y, dydx,NVAft, XI,HTOT, i, yout,deriv的;
            printf ( "\ n加 Z5. 2f 加 %5. 2f 加 %2d 加 \U",
                  "x=", XI," to ", Xl+HTOT, " in ", i, " steps") ;
            printf ( "/.14s V.95\n", "integration" ,"bessj ") ;
            printf ( "/.12. 6f 7.12. 6f\ n", yout[l] ,bl) ;
            printf ( "%12.6f %12. 6f\ n", yout[2] ,b2) ;
            printf ( "Y.12.6f Y.12.6f\ n", youtl3] 小3) ;
    270        Numerica／尸e아）es Example Bo아（

              printf ( '%12. 6f V.12. 6f\ n' , yout[4] , b4) ;
              printf ( '\ nPress ItETUaN to continue. . .\n ') ;
              (void) getcharO;
      }
      free_ vector (dydx, 1 , NVAR) ;
      free_ vector (yout, 1, NVAR) ;
      free_ vector (y, 1,NVAR) ;
      return 0;
}

    The Bulirsch-Stoer method, carried out by routine bsstep, is the integrator of
choice for higher accuracy calculations on smooth functions. An interval h is broken
into finer and finer steps, and the results of integration are extrapolated to zero step-
size. The extrapolation is via a polynomial with pzextr. bsstep monitors local
truncation erior and adjusts the step-size appropriately, to keep errors below eps.
From an external point of view, bsstep operates exactly as does rkqs: it has the
same arguments and in the same order. Consequently it can be used in place of rkqs
in routine odeint. allowing more efficient integration over large regions of x. For this
reason, the sample program xbsstep is of the same form used to demonstrate rkqs.
You will notice that bsstep integrates the test problem in far fewer steps than rkqs,
which is typical. Because of the low accuracy requirement, however, rkqs makes
fewer function evaluations.
/方 Driver for routine bsstep 卓/

#include <stdio.h>
#include "nr. h"
#include 'nrutil. h'1

#define 甘 4

float dxsav,ixp, **yp;             7* defining declarations *7
mnt kmax,kount;

mnt nrhs;          7* counts function evaluations *7

void derivs (float x, float y[],float          dydxD)
{
      nrhs++;
      dydx[1] = 1y [2] ;
      dydx[2) =y[1] -(1. 0/ x) *yC2] ;
      dydx[3] =y[21-(2.0/x)半y[3] ;
      dydxE4] =y[3) -(3. 0/ x) *y[ 4] ;
}

m11t main(void)
{
          ml1t i, nbad1nok;
          float eps= l. 0e-4,h1=0. 1, tdnin=O. 0, x1=i. 0,x2=10. 0,*ystart;

          ystart=vector (1'N) ;
          xp= vector (1,200) ;
          yp=matrix (1, 10 1 1. 200) ;
          ystart[ 1] =bessj0(xl) ;
          ystart12] =bessjl (xl) ;
                                               Chapter 16: Ord加ary D肝erent河E（刊帥ons   271

    ystart [3] =bessj (2,xl) ;
    ystart [4] =bessj (3,xl) ;
    nrhs=0;
    kmax=100;
    d工5av=（工2寸xl) /20 .0;
    od毗小臼毗art , 瓦 工1, x2, e外 ,hl, hntin,knok,&的ad,derivs ,bsste미 ;
    printf ( "\ n%s Y.13s %3d\n", "successful steps: ", " ", nok) ;
    printf ( "Y,s %20s 工3d\n", "bad steps: ", " ", nbad) ;
    printf ( " 工s %9s %3d\n", "function evaluations: ", " ", nrhs) ;
    printf ( "\ n%s %3d\n", "stored intermediate values:          ", kouut) ;
    printf ( "\ n%8s V,18s Y.155\n", "x", "integral ", "bessj (3,x) ") ;
    如r (i: 1; i<=kount; i++)
        printf ( "/.10. 4f /.16. 6f %14. 6f\ n",
            工p[il ,yp[4]［幻 ,bessj 伯 , xp［幻 ) ) ;
    free_matrix (yp,1, 10,1, 200) ;
    free_ vector (xp, i, 200) ;
    free_ vector (ystart, 1, N) ;
    return 0;
}

    pzextr performs a polynomial extrapolation for bsstep. It takes a sequence of
interval lengths and corresponding integrated values, and extrapolates to the value
the integral would have if the interval length were zero. Sample routine xpzextr
works with a known function
                                             1 - r -4- r3

                                          凡＝ 佃n)
                                              + 1);         n= 1 ..,4
We extrap이ate the vect야 yest = （夙 , 尻，尻，尻）given a sequence of ten va노es. The
ten values are labelled iest=1, ... , 10 and are evaluated at xest=l .0/ jest. A call
to pzextr produces extrapolated values yz, and estimated errors dy, and compares
to the true values (1.0, 1.0, 1.0, 1.0) at xest=0.0.
／牛 Driver 如r routine pzextr 斗／

#include <stdio . h>
#include "nr. h"
#include "nrutil. h"

#define NV 4
#define IMAXX 10

float **d, *x;         1* defining declaration */

mllt main(void)
{
    mllt i, iest, J;
    float du꾜11X多Ct, 卞dy, 卞yest, 本yz;

    dy=vector (1,NV) ;
    yest 'vector (l ,NV) ;
    yz=vector (1,NV) ;
    x=vector ( 1, IMAXX) ;
    d"matrix ( 1, INAXX, 1, IMAXX) ;
    /* Feed values from a rational function *1
    /／卞 fn(x)=(1-x＋工＋相）/（工＋1汁＋n 牛／
    .fn, 口 (4 =1. i /= T甘aYY · -,.,..,.
    272    N切nerica／尸9帥）es Examp旭 Book

          iest=i;
          xest=1.0/i;
          du皿＝1.0＝工eat＋工est；卞工eat京工eat;
          如r (j=1; j<＝月V; j++) {
             dun /= (xest+1.0) ;
             yest [j] =dum;
          }
          pzextr (iest, xest, yest,yz,dy,NV) ;
          printf ( "\ ni = 7;2d" .i) ;
          printf ( "\ nExtrap. function: ") ;
          for (j=1; j<=NV; j++) printf ( "/.12.6f ", yz[ j] );
          printf ( "\ nEstimated error: " );
          如r (j=1; j<=NV; j++) printf ( "/.12.6f ", dy[ j] );
          printf ( "\ n") ;
      }
      printf ( "\ nactual values: %14. 6f '/,11.6f %11. 6f 戈11.6f\ n",
          1 .0, 1.0, 1 .0, 1 . o) ;
      free_matrix (d,1,INflX, 1,IMAXX) ;
      free_ vector (x, 1,IMAXX) ;
      free_ vector (yz,1,NV) ;
      free. vector (yest, 1,NV) ;
      free_ vector (dy,1,NV) ;
      return 0;
}

    rzextr performs a diagonal rational function extrapolation for bsstep. It is
usually a less e佈cient standby for rzextr, to be used primarily when some problem
crops up with the extrapolation. The sample program xrzextr is identical to that
for pzextr.
／卞 Driver 如r routine rze工t工 +/

#include <stdio . h>
#include "nr. h"
*include "nrutil. h"

#define 月V4
*define IMAXI 10

float 布水d，卞工；      ／本 defining declaration 字／

mnt inain(void)
{
      mnt i, iest, j;
      float dum, xest,*dy,*yest,*yz;

      dy"vector (l, NV) ;
      yest=vector (1,NV) ;
      yz=vector (1,NV) ;
      x 'vector (1,IMAXX) ;
      d=matrix (1,IMAXX,1,IMAXX) ;
      /* Feed values from a rational function 卞/
      ／卓 fn伍) = (1-好x卞卞3) /(x+1）牛卞n 李／
      for (i=1;i< 'IMAXX; i++) {
           iest=i;
           xest=1.0/i;
           dum=1. 0-工est+xest涍Zest；卞工est;
                                         Ch랴ter 16: Ordinary Differential Equations   273
          for (j=1; j<=NV; j+i-) {
              dum /= (xest+1. 0) ;
              yest[ j) =dum;
          }
         rzextr (iest, xest, yest, yz,dy,NV) ;
         printf ( "\ n%s Y.2d 工8 7.8.4f\ n",
              "iest = ", i, "      lest = ", xest) ;
         printf ( "Extrap. function: ') ;
         for (j=1; j<=NV; j++) printf ( "%12.6f ", yz[ j] );
         printf ( "\ nEstimated error: " ) ．·
         for (j=1; j.c=NV; j++) printf ( "Y.12.6f ", dy[ j] );
         printf ( "\ n") ;
     }
     printf ( "\ nActual values: %15. 6f %11. 6f 7.11. 6f %11. 6f \n",
         1. 0,1. 0, 1. 0,1. 0) ;
     free_matrix (d,1,IMAXX,1, Ii4AXX) ;
     free_ vector (x, I ,IMAXX) ;
     free_ v吼如r (yz,1, 川t) ;
     free_ vector (ye日t, 1,NV) ;
     free_ vector (dy, 1,NV) ;
     return 0;
}

    Stoermer's method is a special-purpose integration method for second-order ODEs
in which the first derivative term is absent. It replaces minid in the Bulirsch-Stoer
method. Sample program xstoerm tests it out on the system
                                        nl n2
                                            V = S 小 Yi
                                        VU    =
                                                工2
                                                    -    !/2
The system is integrated from x = 0 to x = ir/2 with initial conditions

                          111= 0,     112 = i,          y; =2,         16= 0

The program compares the result of integrating with varying number of substeps to
the exact solution
                                     y1 = x + sins

                                     112 =   T2 + cos 工        -
                                                                   2
Of course, in real life you would use stoerin as a replacement for nunid in a modified
version of bsstep, as described in Numerical Recipes.
/卓 Driver for routine stoerm */

#include <stdio . h>
#include <inath.h>
#include "nr. h"
#include "nrutil. h"

#ciefine NVAft 4
#define Xl 0.0
#define HTOT 1. 570796

float d2yl(float x)
{
    return sin(x)+x;
    274    Nt玎nerica／尸e帥始s Example Book

}

float d2y2(float x)
{
    return cos(x)+x*x-2;
}

void derivs(float x, float yD, float dydx[])
{
      dyd工口］=Xmy [l] ;
      dyd址기＝工*卜y［幻 ;
}

mnt main(void)
{
      mnt i;
      float al, a2, xf, *y, *yout,*d2y;

      y=vector (1,NVAR) ;
      yout=vector (1,NVkR) ;
      d2y=vector (1,NVAR) ;
      y 口］=0 . 0;
      y［幻 = -1. 0;
      虹引=2. 0;
      y [4] =0. 0;
      derive (XI, y,d2y) ;
      xf 'X1+HT0T;
      al=d2yl (xf) ;
      a2=d2y2(xf) ;
      printf ( 'Stoermer 's Rule: \n ') ;
      for (i= 5;i<=45;i+=10) {
           stoerm(y, d2y,NVAR, XI,HTOT. i, yout,derivs) ;
           printf ( "\ n加 工5. 2f 加 工5. 2f 加 %2d 加 \U".
                "x=", Xl, ' to ", X1+HTOT, " in "4, " steps") ;
           printf ( "/.14s /.95\n", "intagration", "ansvers") ;
           printf ("%12.6f %12. 6f\ n", yout[l] ,al) ;
           printf ( "X12. 6f %12. 6f\ n", yout[2] ,a2) ;
      }
      free_vector (d2y,1,NVAR) ;
      free_vector (yout.1, NVAR) ;
      free_ vector (y, 1,NVAR) ;
      return 0;
}

    Numerical Recipes provides two routines for stiff systems. The first, stiff, is a
fourth-order Rosenbrock method. We try it out on the sample problem described in
g16.6. Note that for best results one should change the line
           yscal[i] =fabs(y[ i] )+fabs (dyd工[i] 中h) +TIWY;

in odeint to

           yscal[i] =FMAX (1.0,fabs(yli] ));

/中 Driver for routine stiff      */

*includa <stdio .h>
                                            Chapter 16: Ordinary Differential Equations   275
 #include "nr. h'1
 #include "nrutil. h"

 ml1t kmax,kount;             /* defining declarations */
 float 卞xp，卞卞yp, dxsav;

 jut nain(void)
 {
      float eps,hstart, xl=0. 0, x2=50. 0, y[4] ;
      m1lt nbad,nok;

      for (; ;) {
          printf ( "Enter eps,hstart\ n") ;
          if (scanf ( "Y.f V.f "，立叩S，砒田tart) == EOF) break;
          kmax=0;
          y 口］=y［幻 =1. 0;
          y [3] =0. 0;
          odeint (y, 3, xl, x2, eps,hstart, 0. 0,&nok,立nbad, derivs, stiff) ;
          printf ( "\ n'相 %13g Y.3d\n", "successful steps: ' , " ", nok) ;
          printf ( "Y.s Y.20s V.3d\n", "bad steps: ", " " , nbad) ;
          printf ( "Y (END) = 工12.6f %12. 6f %12. 6f\ n", y[1] ,y[ 2] ,y[ 3] );
      }
      printf ( "Normal complation\n") ;
      return 0;
}

    The second method for stiff equations is a version of Bulirsch- Stoer integration
that uses the semi-implicit midpoint rule simpr instead of tumid. Demonstration
program xsimpr tries it out on the same test problem as above, exploring the effect
of different stepsizes.
／半 Driver 如r rqutine simpr 卞／

#include <stdio .h>
#include "nr. h"
#include "nrutil. h"

#define NVAR 3
#define Xl 0. 0
#define HTOT 50. 0

 jut main(void)
{
     mnt i;
     f:Loat al=0. 5976, a2=1. 4023, a3=0. 0 , 卞y , 半yont , 卞df dx, 卞卞dfdy , 孝dydx;

     y=vector (1,NVAR) ;
     yout=vector (1,NVAR) ;
     dfdx=vector (1,NVAR) ;
     dfdy=matrix (1,NVAR, 1,NVAR) ;
     dydx=vector (1,NVAR) ;
     y口］=y［幻 =1.0;
     姓引＝0.0;
     derivs(X1 ,y, dydx) ;
     jacobn(XI ,y, dfdx,dfdy,芹VAR) ;
     printf ( "Test Problem: \n") ;
     for (i= 5; i<=50; i+=5) {
    276    Numerical／相帥旭s Exa／까!e Book

          simpr (y, dydx,dfdx,dfdy,甘VAK, Xi,HTOT,i, yout,derivs) ;
          printf ( "\ n%s %5. 2f %s %5. 2f '/.s 工2d %s \n",
              "x=", Xl, " to ", Xl+HTOT, " in ", 1, " steps") ;
          printf ( "%145 Y.9s\n", "integration", "bessj ") ;
          printf ( "%12.6f %12. 6f\ n" ,yout[1) ,al) ;
          printf ( "%12. 6f %12. 6f\ n", yout[21, a2) ;
          printf ( "%12. 6f '/.12.6f\ n", yout[3] ,a3) ;
      }
      free_ vector (dydx, 1,NVAR) ;
      free_matrix (dfdy, 1,NVAR, 1,WVAR) ;
      free_vector (dfdx,1,NVAR) ;
      free_ vector (yout, 1,NVAYt) ;
      free_ vector (y, 1,NVAR) ;
      return 0;
}

    Finally, sample program xstifbs solves the same problem with the full machinery
of the Bulirsch-Stoer method via routine stifbs. Once again you should modify the
scaling in odeint as in xstiff for best results.
/* Driver for routine stifbs */

#include <stdio.h>
#inc]끄de "nr. h"
#include "nrut ii. h'1

mnt kmax,kount;             /方 defining declarations */
float 卞xp, 半卓yp, dxsav;

mnt main(void)
{
      float eps,hstart, x1=0.0, x2=50. 0,yE4] ;
      mnt nbad,nok;

      for (; ;) {
          printf ( "Enter eps,hstaxt\n") ;
          if (scanf ( "%f %f ", &eps,&hstart) == EOF) break;
          kmax=0;
          y［幻 =y m卜1. 0;
          y[3] =0. 0;
          odeint (y, 3, xl, x2, eps,hstart, 0. 0,knok,&nbad,derivs, stifbs) ;
          printf ( "\ n'/.s %13s 'h3d\n", "successful steps: ", " ", nok) ;
          printf ( "/.s 工20s '/.3d\n", "bad steps: ", " ", nbad) ;
          prmntf ( "Y (END) = %12. 6f %12. 6f %12. 6f\ n", y[1] ,y[ 2) ,y[ 3] );
      }
      printf ( "Norinal completion\n") ;
      return 0;
:1,
    Chapter 17: Two-Point Boundary Value Problems

          Two-point 加undary川妃 problems, and their 北erat加e so加tion, are the
      sub就ance of Chaj元er 17 of Numerical Rec加es. The first 就ep 加 so加加g them
     is to cast the problem as a set of N coupled first-order ordinary differential
     equations, satisfying n1 conditions at one boundary point, and n2 = N 中 ni
     conditions at the other boundary point. We apply two general methods to
      the soli此ions. 川r就 are the shooting met加小j typ沂ed by routines shoot and
     shootf, which enforce the n1 conditions at one boundary and set n2 con-
     ditions freely. Then they integrate across the interval to find discrepancies
     with the n2 conditions to be enforced at the other end. The Newt on-Raphson
     method is used to reduce these discrepancies by adjusting the variable pa-
     rameters.
         The other approach is the relaxation method in which the differential
     equations are replaced by finite difference equations on a grid that covers the
     range of interest. Ron tine solvde demonstrates this method, and is demon
     strated "in action" by program sfroid, which uses it to compute eigen values
     of spheroidal harmonics. The programs sphoot and sphfpt in Numerical
     Recipes similarly demonstrate the use of shoot and shootf on the same
     problem. Since these three programs are essentially self-contained, we do
     not need separate demonstration programs here. The file xsphfpt . c on the
     diskette merely contains a copy of the routine derivs needed by sphfpt. We
     reproduce it here, along with typical output from the three test programs.



／卞 A끄xiliary routine for sphfpt 半／

extern jut m,n;
extern float c2,dx,gnuna;

void derivs (float x,float yD, float dydx[])
{
     dyd虹11=y m] ;
     dy缸 [2] =但 . 0*x卞（小1. 0) 押[2卜臼口卜口卞x卞x汁址n V (l . 0吐竹）;
     dyd虹引 =0.0;



     In the following sample output, note that 入 (lamda) and i (mu) are merely two
different conventions for expressing the same result, related by

                            尸(7兀미 = 入（m, n) - rn(m+ 1)

     Typical output for sfroid.c:
 278        Num아切／尸e아旭s Examp旭 Bo아（

enter in n
35
Enter c**2 or 999 to end.
16. 0
   Iter.       Error         FAC
      1      0. 271212    1. 000000
   Iter.       Error        FAC
      2      0.080674     1. 000000
   Iter.       Error        FAC
       3     0. 006255    1. 000000
   Iter.       Error         FAC
      4      0.000039     1. 000000
   Iter.       Error        FAC
      &      0. 000000    1. 000000
 in = 3   n = 5     c**2 = 16. 000      lainda =   35. 461006
Enter c**2 or 999 to end.
20. 0
    Iter.    Error         FAC
       1   0. 075860    1. 000000
    Iter.     Error        FAC
       2   0.004998     1. 000000
   Iter.        Error        FAC
      3       0. 000025   1. 000000
   Iter.        Error       FAC
       4      0. 000000    1. 000000
 a = 3       n = 5     c**2 = 20. 000   lamda =    36. 771168
Enter c**2 or 999 to end.
-16. 0
   Iter.     Error        FAC
       1   0. 517707   1. 000000
   Iter.        Error       FAC
      2       0. 835383   1. 000000
   Iter.        Error        FAC
      3       0. 375960   1. 000000
   Iter.         Error      FAC
      4       0. 172314   1. 000000
   Iter.         Error       FAC
      5       0. 020227   1. 000000
   Iter.         Error       FAC
      6       0. 000824   1. 000000
   Iter.      Error        FAC
      7    0.000001     1. 000000
 m = 3    n ;= 5    c字卞2 二 尸16. 000     la皿da =    24. 310978
Enter c**2 or 999 to end.
-20.0
    Iter.       Error       FAC
       1      0. 052214   1. 000000
    Iter.        Error       FAC
       2      0. 003544   1. 000000
    Iter.       Error       FAC
       3   0. 000022     1. 000000
    Iter.     Error         FAC
       4   0. 000000     1. 000000
 in = 3   n = 5      c**2 = -20. 000    lanida =   22. 893074
Enter c京$2 or 999 to end.
999
                               C力可升er 17: 了녀／o-I七亦卄 Bound計y Va加e 尸rob/ems   279
    Typical output from sphoot . C:
 input In,n, c- squared (999 to end)
3 5 1.5
     mu (m1n)
    18. 524508
 input m,n, c- squared (999 to end)
3 5 0. 0
     mu (rn 1n)
    18. 000002
 input m,n. c-squa工ed (999 to end)
3 5 999


    Typical output from sphfpt . C:

 input m,n, c- squared (999 to end)
3 5 1. 5
     mu (m .n)
    18 . 524508
 input m.n, c-squared (999 to end)
3 5 -1. 5
     mu(m,n)
    17. 473288
 input m,n, c-squared (999 to end)
3 5 0, 0
     mu (m,n)
    18. 000004
 input m,n, c-squared (999 to end)
3, 5, 999
Chapter 18: Integral Equations and Inverse Theory

        Linear Fredholm equations of the second kind can be solved with the
    routine fred2. The accompanying routine fredin interpolates the solution
    returned by fred2 on the quadrature points to arbitrary abscissas. voltra
    handles linear Volterra equations of the second kind. Routine wwghts con-
    structs quadrature weights for an arbitrarily singular kernel. In Numerical
    Recipes a sample program demonstrating its use is given in fredex, so we do
    not give another sample program here.
        Fredholm equations of the 月rst kind are closely related to so-called inverse
    problems. While no general-purpose routines are given in Numerical Recipes
    for such problems, there is an extensive discussion in Chapter 18.



    Our test problem for routine fred2 is Example 4.2.5b from Computational Meth-
ods for Integral Equations by Delves and Mohamed:

                                                                  쓰叭
                   /(0크
                   1(t)            s)3If(s)
                        = fJ。"'(t.伽）        ds『+！ti/2
                                     3/4/(3)43            )9/4
                                                  1/2. (1즐）
with exact solution
                                      f (t) = ti! 2

Using only an 8-point Gaussian quadrature gives reasonable accuracy in the solution.
／方 Driver 如r routine fred2 卞／

#include <atdio . h>
#include <math.h>
#include "nr. h"
*include "nrutil. h"

#def in. N 8
*define P1 3.1415927

float g(float t)
{
                                       （t,O.75) /2. 25;
      return sqrt (t）中0日（1江／2．이2. 25汁P0日
}

float ak(float t, float a)
{
       return pov(t* a.O.75) ;
}
                                        C/
                                         i랴玎er 18: Integral Equ카幻ns and 加verse 了/
                                                                                ieory                    281
      mnt main(void)
      {
           jut 1,
           fl oat a=O. O,b=PI/ 2.O, *f;
           fl oat 巾t; 1 4日;

            t=vector (1,N) ;
            f=vector (1,N) ;
           口＝vector (1, 肋 ;
            fred2(N, a,b,t, f, w,g,ak) ;
           ／中 Compare 口ith exact solution 牛／
           printf ( "Abscissa, Calc soin, True soln\n") ;
            for (i "l; i<=N; i++) printf ( "/,10. 6f '/,10.6f '/.iO.Gf\n", t[ i] ,fEi]
                                                                                       ,sqrt (tCi] ));
           free_ v吼如H口,1小）;
           free_ vector (f, 1,N) ;
           free_ vector (t, 1,N) ;
           return 0;
  }

     Routine fredin interpolates the solution obtained with fred2 onto an arbitrary
 point t using Nystrom interpolation. Sample program xfredin demonstrates its use
 on the same problem solved in xfred2.
 ／卞 Driver 如r routine fredin 卓／

 #include <stdio . h>
 作include <math.h>
 #include "nr. h"
 #include "nrutil. h"

 #define II 8
 #define Pt 3. 1415927

float g(float          t)
{
            return sqrt (t) -pow (Px/2. 0,2. 25) *pow(t, O.75) /2. 25;
}

float ak(float t, float s)
{
            return pow(tss, O. 75) ;
:1,

jut main(void)
{
          float a=O. O,ans ,b=PI/ 2.O, x,*f;
          float; 京t, 卞日；

          t=vector (1,M) ;
          f=vector (1,N) ;
          日＝vector (1, 肋 ;
          fred2(N,a,b, t, f, w,g,·aic) ;
          如r (; ; ) {
              printf ( "自lter T between 0 and PI/ 2\n") ;
              if (sc旬lf ( " Xf " 小工） == EOF) break;
              ans=f redin（工，瓦a,b,t, f ．吼g, a上）;
              printf ( "T, Calculated a끄swer, True answer\n") ;
    282    Nu／加成：a／尸0아始＄ Exa／까1e Book

           printf ( " 工10. 6f %10. 6f 工10. 6f\ n", x.카ls,sqrt (x) );
      }
      fr ee느vector（日, 1,표）;
      free_ vector (f, 1, N) ;
      fr ee_ ye比吐（t,1, 助 ;
      return 0;
}

   Our test system of Volterra equations comes from p. 151 of Delves and Mohamed's
book:


           f1(t) = _j'e 'fi(s)ds- j 'cos(t- s)fz(s)ds+ cosht+ tsint
          12(t) = - f' e"'f1(s) ds- j' tcossfz(s)da+ 2sint + t(5in2t + e')
with exact solution
                                           月（t) = e1i
                                           丘(i) = 2sint

／字 Driver 如r routine voltra 卞／
#include <stdio . h>
#include <math.h>
#include "nr. h"
#include "nrutil. h"

float g(int k, float t)
{
      return (k == I ? cosh(t) +t卞sin(t)          : 2.0*sin(t) +t* (SQR(sin(t) )+exp(t) ));
)
float a.k (int k, int l, float t    float s)
{
      return ( (k == 1) ?
          (1 == 1 ? -e자：1(t- s) : -cos(t- s) ) :
          (1 == 1 ? 小e工p(t+s) : -t* cos佃）)) ;
}
*define 甘 30
#define H 0. 05
#define 甘 2

ml1t main(void)
{
      mllt nn;
      float t0=0.0,*t 1*卞f;

      t=vector (1,N) ;
      f=ma缸ix(1,瓦 1,N) ;
      voltra（甘，甘，t0 1月［, t ,t, g,ak) ;
      ／布 exact coin is fE1] =exp(- t) , 玎기＝2sia(t) 小／
      printf ( '  abscissa, voltra 缸1sverl, rca]. answerl, ") ;
      printf ( " voitra answer2, real a끄swer2\n") ;
      for (nn=1;nn<＝甘;nn++)
          prmntf ( "%12.6f '/.12.6f '/.12.6f 工12. 6f '/.12.6f\ n".
                   t[ nn) ,fCl] [un] ,e印(- t[ nn] ),f [2] [nn] ,2.0*smn(t[ nn] ));
                                  Chapter 18: Integral Equations and Inverse Theory   283
    tree_ vector (t, 1 IN) ;
    free_matrix(f .1 ,M, 1,N) ;
    return 0;
}
Chapter 19: Partial Differential Equations

        Several methods for solving partial differential equations by numerical
   means are treated in Chapter 19 of Numerical Recipes. All are finite differ-
   encing mllethods, including forward time centered space differencing, the Lax
   method, staggered leapfrog differencing, the two-step Lax- Wendroff scheme,
   the Crank-Nicholson method, Fourier analysis and cyclic reduction (FACH),
   Jacobi눙 method, the Gauss-Seidel method, successive over-relaxation (SOR)
   with and without Chebyshev acceleration, operator splitting methods as ex-
   emplified by the alternating direction implicit (ADI,) method, and multigrid
   methods. There are so many methods, in fact, that we have not provided each
   topic with a routine of its own. In many cases the nature of such routines
   follows naturally from the description. In some cases, you will have to consult
   other references. The routines that do appear in the chapter, sor, mglin and
   nigf as, show two of the more useful and efficient methods for elliptic equations
   in application.



    Procedure sor incorporates successive over-relaxation with Chebyshev accelera-
tion to solve an elliptic partial differential equation. As input it accepts six arrays of
coe佑cients, an estimate of the spectral radius of Jacobi iteration, and a trial solution
which is often just set to zero over the solution grid. In program xsor the method is
applied to the model problem
                                      ,32u 02u
                                      === + 二＝;      p
                                       a工｛ 아／1
                                                 =
which is treated as the relaxation problem
                                 Ou   02u 02u
                                  e = ;;= + ;;= 小 p
                                 二；
                                 or   ox口 ('1尸

Using FTCS differencing, this becomes

                   u슈1.I + u｝尸1 .1 + 畔，1+1 + 畔，iel- 4u芥l = Pui스2
(The notation is explained in Chapter 19 of Numeric口l Recipes.) This is a simple
form of the general difference equation to which sor may be applied, with

                     A,, = B,, = C,, = D,, = 1.0 and E,, = -4.0

for all j and 1. The starting guess for u is u,1 = 0.0 for all j, 1. We choose the density
p to be zero everywhere except directly in the center of the grid where p = 2. For
a 32 x 32 grid, 스 = 1/32 and so F,,, = 0.0 except in the center of the grid where

 284
                                              Ch카刃er 19: 尸am削O肝eren打計Equa加ns             285

                                                 bi, which is called rjac, is taken
F (midl,midl) = 2/322 勺 0.0020. The value of Pjac。
from equation (19.5.24) of Numerical Recipes,



                                              呻｝唯加S三
                                                    （匍
                                  PJacobi =

                                                 1+
                                                            "

In this case, j=1=JMAX and 스x = 스9 so rjac = cos(ir/ JMAX). A call to sor leads to
the solution shown below. To fit the output on the page, the solution at only every
fourth grid point is printed out. As a test that this is indeed a solution to the finite
difference equation, the program plugs the result back into that equation, calculating

                         斗 = 啞1.1 + U知,1+ 畔,l+1 + 呼- 1 中 4畦｝l

The test is whether F,,1 is almost everywhere zero, but equal to 0.0020 at the very
centerpoint of the grid.
SOR solution:
  0.0000 0. 0000 0. 0000 0.0000 0. 0000 0.0000 0. 0000 0.0000                  0. 0000
  0.0000 0.0000 -0. 0001 -0. 0001 -0. 0001 -0. 0001 -0. 0001 0.0000            0. 0000
  0.0000 -0. 0001 -0. 0001 -0. 0002 -0. 0002 -0. 0002 -0. 0001 -0. 0001        0. 0000
    0.0000 -0. 0001 -0. 0002 -0. 0003 -0. 0005 -0. 0003 -0. 0002 -0. 0001      0. 0000
    0.0000 -0. 0001 -0. 0002 -0. 0005 -0. 0014 -0. 0005 -0. 0002 -0. 0001      0.0000
    0. 0000 -0. 0001 -0. 0002 -0. 0003 -0. 0006 -0. 0003 -0. 0002 -0. 0001     0.0000
    0. 0000 -0. 0001 -0. 0001 -0. 0002 -0. 0002 -0. 0002 -0. 0001 -0. 0001     0.0000
    0. 0000     0.0000 -0. 0001 -0. 0001 -0. 0001 -0. 0001 -0. 0001   0.0000   0.0000
    0. 0000     0.0000 0.0000 0. 0000 0.0000 0.0000 0. 0000           0.0000   0.0000


/* Driver for routine sor */


#iaclude <stdio . h>
#include <math.h>
#include "nr. h"
#include "nrutil. h "


#define NSTEP 4
#define JMAX 33
#define P1 3.1415926


jot main(void)
{
      jot i, j, midl;
      double 中＋a，半卓b1牛Sc：卞中d1卞＋C，李牛f1＋牛u.rjac;


      a=dmatrix (1, JMAX, 1, JMAX) ;
      b=dmatrix (1 , .IMAX, 1, JMAX) ;
      c=dmatrix (11iMkX,1, JMAX) ;
      d=dmatrix (1 ,JMAX, 1, JMAX) ;
      e=dmatrix ( 1, JMAX , 1. JMAX) ;
      f=dmatrix (1 1JMkX, 1 ,JMAX) ;
      u＝山natrix (1 JMAX, 1, .IflAX) ;
      for (i= 1; i< =JMAX; i++)
              for (j= 1; j<=JMAX; j++) {
                  缸ij [j] =b[i] ［刃 =c [i표刃 dli] Cj] =1.0;
    286    八／umei七削 尸e아治s Example Book

                eEi] [j] =(-4. 0) ;
                玎i] [j] =u[ij [j3=0.0;
            }
      midl=JI4AX/2+1;
      玎midl] [midl卜2. 0/ ( (JMAX-1汁（Jilt.    卜1) ) ;
      rjac=cos(PI/ JMAX) ;
      sor (a,b, c,d, e, f, u, JMAX,rjac) ;
      printf ( "SOR solution: \n") ;
      如r (ir1; i<=JMAX; i+=NSTEP) {
           for (j. 1; j<=JMAX; j+=NSTEP) printf ( "%8. 4f '. u[i] (j] );
           print f ( '\ n ') ;
      }
      printf ( "\ n Test that solution satisfies difference aquations: \n") ;
      for (i=NSTEP+1; i< JMAX; i+=NSTEP) {
           for (j=NSTEP+1; j<JMAX; j+=NsTEP)
                玎i] [j] =uC1+i] Ci] +u[ j- j] [j] +u Ci] [j+ 1] +u[i] Cj-1]
                      -4. 0希u[i] 口］;
           printf (叫（75", " ") ;
           for (j=NSTEP+1; j<JMAX; j+=NsTEP) printf ( "%8.4f ", fCi] Cj] );
           printf ( '\ n") ;
      }
      free_dinatrix (u, 1, uMAX, 1, J甘AX) ;
     free..dmatrix(f , 1, JMAX, 1, JNAX) ;
     free4dmatrix (e,1, JMAX,1, JMAX) ;
     free느dinatrix (d, 1, JMAX, 1, JMAX) ;
     free_dinatrix (c 11, JMAX , 1, JMAX) ;
     free-－山natrix (b, 1, JMAX, 1, JMAX) ;
     freeedniatrix (a, 1, JMAX, 1, uMAX) ;
     return 0;
}

    Multigrid methods are generally much more efficient than SOR. Routine mglin
solves linear elliptic equations using the full multigrid method. Program xmg].in
solves the same model problem as xsor and prints out the solution, which may be
compared with the copy listed above. However, because of the way mglin is set up,
when the solution is substituted into the difference equations, it should give back p
and not p스2. Here is the output on a 32 x 32 grid:

 Test that solution satisfies difference equations:
         0. 0001 -0. 0001 -0. 0004 0. 0008 -0. 0004 -0. 0001 0.0001
        -0. 0001 -0. 0002 -0. 0008 0.0028 -0. 0008 -0. 0002 -0. 0001
        -0. 0004 -0. 0008 -0. 0027 0.0048 -0. 0027 -0. 0008 -0. 0004
         0.0008 0. 0028 0.0048 2.0171 0.0048 0.0028 0.0008
        -0. 0004 -0. 0008 -0. 0027 0. 0048 -0. 0027 -0. 0008 -0. 0004
        -0. 0001 -0. 0002 -0. 0008 0.0028 -0. 0008 -0. 0002 -0. 0001
         0.0001 -0. 0001 -0. 0004 0.0008 -0. 0004 -0. 0001 0.0001

/* Driver for routine mglin */

#include <stdio . h>
#include <math.h>
#include 'nr. h"
#include "nrutil . h'1

#define NSTEP 4
#define uMAX 33
                                              Chapter 了9: Part洌D肝erenti削白ua加ns               287

 mllt main(void)
 {
     mnt i j ,midl=JMAX/2+1;
     如uble 卞卓f. 牛卓U;


     f=dmatrix (1, JMAX 11, JMAX) ;
     u=dmatrix (1 1JMAX, 1, JMAX) ;
     for (i= 1; i< =JMAX; i++)
         for (j= 1; j<=JMAX; j++)
              町i] [j] =0.0;
     u[midl] [iuidl] =2.0;
     mglin(u, JMAX, 2) ;
     printf ( 'MGLIN solution: \n") ;
     for (i= 1; i< =JMAX; i+ =NSTEP) {
          for (j= 1; j<=JMAX; j+=NSTEP) prmntf ( "7.8.4f ", u[ i] [jj)    ;
          printf ( "\ n ") ;
     }
     printf ( "\ n Test that solution satisfies        difference equations: \n") ;
     for (i= NSTEP+1; i< JHAX; i+=NSTEP) {
          for (j= NSTEP+1; j<JNAX; j+tNSTEP)
              f[ i] [jl= u[ i+1] [jj+ u[ i- 1] Cj] +uCi] [j+ 1]+u[i] [j- 1]
                    -4. 0*u[ i] [jJ;
         printf ( '%7s ", " ") ;
         for (j= NSTEP+1; j<JMAI; j+=NSTEP) printf ( "%8.4f ", f[ i] [J] *(JMAX-1) *(J거［AX-1) );
         printf ( "\ n ") ;
     }
     free_dmatrix (u, 1, JMAX, 1, JMAX) ;
     free_dntatrix(f 11, JMAX 11, JMAX) ;
     return 0;
}

    Numerical Recipes provides mgf as as a prototype for solving nonlinear
                                                                           elliptic
problems with the Full Approximation Storage (FAS) scheme. Program xmgf as
                                                                            solves
the simple problem
                                    V2u + u2 = p
as described in Numerical Recipes with the same choice of p made in xsor and
                                                                              xmglin.
The solution is checked once again by substituting into the difference equation. Here
is the output for the 32 x 32 grid:
MGFAS solution:
  0.0000 0. 0000 0. 0000 0. 0000 0.0000 0.0000 0. 0000                   0.0000    0.0000
  0. 0000 0.0000 -0. 0001 -0. 0001 -0. 0001 -0. 0001 -0. 0001            0. 0000   0. 0000
 0.0000 -0. 0001 -0. 0001 -0. 0002 -0. 0002 -0. 0002 -0. 0001 -0.
                                                                   0001            0. 0000
 0.0000 -0. 0001 -0. 0002 -0. 0004 -0. 0004 -0. 0004 -0. 0002 -0.
                                                                   0001            0.0000
 0. 0000 -0. 0001 -0. 0002 -0. 0004 -0. 0013 -0. 0004 -0. 0002 -0.
                                                                   0001            0.0000
 0.0000 -0. 0001 -0. 0002 -0. 0004 -0. 0004 -0. 0004 -0. 0002 -0.
                                                                   0001            0. 0000
 0. 0000 -0. 0001 -0. 0001 -0. 0002 -0. 0002 -0. 0002 -0. 0001 -0.
                                                                   0001            0.0000
 0. 0000 0.0000 -0. 0001 -0. 0001 -0. 0001 -0. 0001 -0. 0001 0. 0000
                                                                                   0.0000
 0.0000 0.0000 0.0000 0.0000 0. 0000 0. 0000 0.0000 0.
                                                                   0000            0. 0000
Test that solution satisfies difference equations:
         0. 0000 0. 0008 -0. 0009 0.0000 -0. 0009 0. 0008 0.0000
         0.0008 0.0033 0.0007 -0. 0035 0. 0007 0.0033 0.0008
        -0. 0009 0. 0007 0. 0051 -0. 0328 0.0051 0.0007 -0. 0009
         0.0000 -0. 0035 -0. 0328 1. 8660 -0. 0328 -0. 0035 0.0000
        -n rnno n flflA7 A nnci =r1 nnn11 r\ nr\ 11 4 n r1八八m n r1J1r1r1
288      Nume川口a／尸9아）es Examp旭Book

          0. 0008   0. 0033 0. 0007 -0. 0035 0.0007       0.0033    0.0008
          0. 0000   0.0008 -0. 0009 0.0000 -0. 0009       0. 0008   0.0000


    You might be a little puzzled by this output at first., For example, the center
value of V2u + u2 for the solution is 1.8660, while the true value is 2. Both sor
and mglin get closer, with 2.0171, yet the nonlinear correction u2 is only (_ .0013)2.
                                                                              than the
Here's what's going on: mgf as iterates until the iteration error is smaller
truncation error. These errors   are r.m.s. errors, computed  with routine anorm2.   To
check the  performance   of mgf as, we did a run with the parameter  ALPHA  set to 10小
and with maxcyc = 6. This high accuracy solution is essentially the exact solution of
the finite difference equations, and is in fact very close to the solution obtained by
sor and mglin. We next computed the truncation error by applying the routine lop
to this accurate solution and then finding the difference between the answer and the
                                                                                 applied
original right-hand side, p. The norm of this error was 6 x 10丑 Next, we
lop to the solution obtained in the demonstration program. (This gives the quantity
printed above as "Test that solution satisfies difference equations:".) The difference
between this quantity and lop of the "exact" finite difference solution is the iteration
 error. Its norm is 6 x i03. Thus mgf as is solving the problem to better than the
 truncation error, as advertised. Since in this problem p is so sharply peaked, the
 r.m.s. error is perhaps not the best measure of the error - the maximum deviation
 might be better. For a smoother p, these error measures are not that different and
                                                                                    need
 mgf as would give more intuitive looking results. For this problem, however, you
 a smaller value of ALPHA if you want the maximum deviation below the truncation
error; ALPHA = 0.1 will do the trick.
/* Driver for routine mgfas */

#include <stdio.h>
#include (math.h>
#include "nr. h"
#include "nrutil. h"

 #define NSTEP 4
 #define .)MAX 33

 m11t main(void)
 {
      ml1t i口 mid1'JMAI/2+1;
      double 半中f 1卞＋U;

      f=dxnatrix (1, JMAX, 11 JNAX) ;
      u=daatrix (1, JMAX, 1, JI4AX) ;
      for (i=1; i<=JMAX; i++)
           for (j=1; j<=JI4AX; j++)
                uCi) [j1=0. 0;
      u[inidl] [midl] =2 .0;
      mgf as (u, JMAX, 2) ;
      printf ( 'MGFAS solution: \n") ;
      for (i "l; i<=JMAX; i+=NSTEP) {
           for (j=1; j<=JMAI; j+ 'NSTEP) printf ( "V.8.4f ", u[ i] Ej3) ;
           printf ( "\ n") ;
      }
      printf ("\ n Test that solution satisfies difference equations: \n") ;
      for (i "NSTEP+i; i<JMAX; i+=NSTEP) 1
                                            Ch司升er 19: 尸art河O肝eren打削Equa加ns             289

        for (j=NSTEP+1;j< JKAX; j+=NSTEP)
            玎i] [j] =uti+1] Ej] +u[i- 1] [j] +uEi] Ej+1] +u[i] [j- 1] -
                  4. 0字u[i] [j] +u[i] [j] 卞uci] 口］/( (JMAX-1汁（JMA卜1) ) ;
        printf ( 'V.78", " ") ;
        for (3=NSTEP+1; j<JMAX; j+=NSTEP) printf ( "%8. 4f "f[ i] [j] *(JMAX-1) *(JMAX-1) );
        printf ( "\ n') ;
    }
    free_dmatrix (u, 1. JMAX, 1, J11AX) ;
    free_dmatrix (f 1 1, JMAX, 1, JMAX) ;
    return 0;
}
    Chapter 20: Less-Numerical Algorithms

               Chapter 20 of Numerical Recipes collects together an idiosyncratic group
          of "less-numerical" algorithms whose usefulness lies either in tasks peripheral
          切 numerica/ 的rk, or in eluci而ting some less 的vious applic毗ions 可numeri-
          cal techn匈配5 在計 examp厄 the use ofF뇨就 Fourier I노ansforms for performing
          extended precision arithmetic).
               The routine machar is a useful aid in understanding the limits of floating
          point arithmetic on your particular computer. igray is a simple function that
          converts integers into their Gray code, or back again. The combination of icrc
          and its captive routine icrcl is used to construct cyclic redundancy check-
          sums, in some standard conventions. The main book discusses two rather
          different methods for compressing information, Huffman coding, realized in
          the routines hufmak, huf app, hufenc, and hufdec, and arithmetic coding,
          realized as arcmak, arcode, and arcsum. Finally, a whole group of routines
          for multiple precision arithmetic are given, with names of the form nip. . . j
          culminating in the program mppi which is used to compute 冗 to as many as
          several thousand decimal digits.



    The sample program for machar does nothing more than run the routine and print
the results. machar, by some fairly subtle arithmetic processes, feels out the floating
point characteristics of your computer. The main book explains the meaning of- the
parameters that are reported. The most important ones are epa, xmin, and mmax,
which give respectively the floating point precision, and the smallest and largest (in
magnitude) numbers that are representable at full precision. (Most ANSI C compilers
already provide values for these quantities, under different names, in the standard
header file fl oat. h.)

／衣 Driver 如r routine mach町 卞／

#include <stdio.h>
*inc].ude "nr.h"

mnt main(void)
{
      mnt ibeta,iexp, irnd, it, inachep,maxexp,minexp,negep,
                                                             ngrd;
      float epa, epsneg , xmax , xinin;

      machar (立ibeta,&it, &irnd,&ngrd,kmachep, knegep,kiaxp,也ininexp,&maxe
                                                                             xp,
          立epa , 立epsneg , &xmin，在xma工）;
      printf ( "ibeta = %d\n", ibeta) ;
      prmntf ( "it = 工d\n" :it) ;


    290
                                           Ch카）旭r 20: Less-Nun旭月cal A勾or丹加71S         291
     printf ( "irnd = ?.d\n", irnd) ;
     printf ( "ngrd = %d\n' , ngrd) ;
     printf ( "machep = Y.d\n", machep) ;
     printf ( "negep = 工d\n", negep) ;
     printf ( "iexp = Xd\n", iexp) ;
     priatf ( "mixiexp = Xd\n", minexp) ;
     printf ( "maxexp = %d\n", maxexp) ;
     printf ( "eps = %12. 6g\n", eps) ;
     printf ( "epsneg = Y.12.6g\n", epsneg) ;
     printf ( "xmin = %12. 6g\n ', xmin) ;
     printf ( "xmax = %12. 6g\n", xmax) ;
     return 0;



     The function igray returns the Gray code of its first argument, or else the inverse
Gray code (if the second argument is -1). The following example program
                                                                                  verifies,
for some range of integers, that the function, followed by its inverse, does in fact
produce the original input value. It also prints out a few values within the chosen
range, and verifies, for those values, that the Gray code of two consecutive integers
differ in only one bit: the last column printed should always be a power of 2; half the
time it will simply be the value 1, since the results differ only in the least significant
bit.
／字 Driver 如r routine igray 卞／/

#include <stdio .h>
#inc].ude "nr.h"

 jut main(void)
{
    unsigned long jp,n,ng,nmax, iunin,nni,nxor;

    如r (; ;) {
       printf ( "input nmin,n皿ax: \n") ,
       if (scanf ( "兄in %iu" ,tn皿1끼如ma幻 == EOF) break;
        jp=(n皿ax-I｝皿in) /11;
       if (jp < 1) jp=i;
       priutfC 'n, Gray[n] , Gray (Gray[nj) , Gray[n] - Gray[n+i] \n") ;
       for (n=nmin;n<=nmax;n++) {
            ng 'igray (n,1) ;
            Iuii 'igray(ng,-1) ;
            if (nni != n) printfC 'WRONG 1 AT %d Y.d %d\n", n,ng,nni)
                                                                       ;
            if ( ' ( (n-nmin) % jp) ) {
                       nxor=ng m lgray(n+1,1) ;
                       printf ( "%iu %lu Y.lu %lu\n",n,ng,nni,n工or) ;
             }
        }
    }
    prlntf ( "Normal completion\n") ;
    return 0;



    Cyclic redundancy checksums are constructed, according to any one of several
standard conventions, by the routine icrc. The following test
                                                              program, with the
input lines
292      Numerica/ 尸e아治s Exam下,le Book

i T
17 CatMouse987654321


will reproduce the test values that are given in the Table in the main book. Notice
how some conventions (e.g., X.25), require that the packet (message and checksum
together) be made from the bitwise complement of the CRC bytesj while others use
the bytes themselves. Note also that the desired checksum of the full packet is zero
in some conventions, but some particular value (here hexadecimal FOB8) in others.
/* Driver for routine icrc 卓/

#include <stdio.h>
#include "nr. h"

#define LOBYTE(x) ( (unsigned char) ( (x) & OxFF) )
#define HIBYTE(x) ( (u끄signed char) ( (x) >> 8) )

mlit inain(void)
{
      unsigned char lin[ 256] ;
      unsigned short il, i2;
      unsigned long n;

      如r ( ; ;) {
         printf ( 'Enter length and string: \n") ;
         if (scanf ( "%lu 工s", &n,&lin[ l] ) == EOF) break;
           linEn+i] =0;
           printf ( " 加＼n" ,&lin 口n ;
           i1=icrc (0,lin, n, (short)0,1) ;
           lin[ n+1] =HI8YTE(i1) ;
           lin[ n+2] =LOBYTE(ii) ;
           i2=icrc (il ,lin, n+2, (short) 0, 1) ;
           printf ( "      XMODEM: String CRC, Packet CRC=    oxV.x    ox7,x\n", ii, i2) ;
            i1=icrc (i2, lin, n, (short)0xff, -1) ;
           lin[ n+1] = = LOBYTE(il) ;
           lin[ n+2] = = HIBYTE(il) ;
           i2=icrc (il, lin, n+2, (short)oxff ,-i) ;
           printf ( "        X. 25: String CRC, Packet CRC=   0뇌.x     ox%x\n", il, i2) ;
           il= icrc (i2, lin, n , 佃如此 ) 0, -i) ;
           lin[ n+1] =LOBYTE(il) ;
           lin[ n+2]=NIBYTE(ii) ;
           i2=icrc (il, lin, n+2, (short) 0,-1) ;
           printf ( " CRC-CCITT: String CRC, Packet CRC=      0x'/.x   0xV.x\n", il, i2) ;
       }
       printf ( "Normal completion\n") ;
       return 0;
 }
                                                                                verifies
     The example program for the decimal check digit routine decchk first
 the claim in the main book that the method finds about 95% of jump transpositions
 (acb -+ bca). (The exact answer is that it finds all but 52 out of 900.) The program
 then prompts the user for test strings (terminated by "x") and prints out the string
 with a following check digit, and verification that the augmented string passes the
 check-digit test. You might test this program with, e.g., telephone numbers in various
 formats, such as '1-800-433- 7300" or "1 (800) 241-6522," to verify that decchk in fact
                                             Ch카升er 20: Less-Numeric刻A／如nt!갸71$                   293

ignores all input characters except decimal digits in computing its check digit.
7* Driver for routine decchk */

#include <stdio.h>
#include "nr. h'1

#define MAXL工甘E 128

ml1t main(void)
{
    jut j, k, l, n,nbad'"O,ntot=O;
    mllt iok, jok;
    char lin[ MAXLINE+2] ,ch, chh;

    /* test all jump transpositions of the form 86j1k41 *7
    lin[ O] ='8 ';
    uin口］" '6 ' ;
    linES] = '4 ' ，·
    lmn[6] ='l ';
    for (j "'48; j<"'57; j++) {
        for (k=48;k<=57;k++) {
              for (l= 48;l ( '57; l+ +) {
                   1inE3] =1;
                   if (j != k) {
                        ntot++;
                        lin[ 2] =j;
                        lmn[．幻 =k;
                        iok=decchk (lin, 7,立ch) ;
                        lin[ 7kch;
                        如k=decchk (lin, 已立chh) ;
                        'in ［幻 =k ;
                        lin ［幻 =3 ;
                         jok=decchk (lmn,8,&chh) ;
                        if (! iok I I jok) nbad++;
                   }
              }
         }
    }
    printf ( "佃 '/,14s V.3d\n", "Total tries: ", " ", ntot) ;
    printf ( "Y.s %16s '/,3d\n", "8ad tries: ", " ' , nbad) ;
    printf ( 'Y.s '/.lls '/.4.2f\ n", "Fraction good: ' , " ", ( (float) (ntot- nbad) )/ntot) ;
    for (; ;) C
        printf ( "enter string terminated by x: \n") ;
        if (gets (lin) == NULL) break,
        for (j= O; j<MAXLINE; j++)
               if (uin[ j] == 'x ') break;
         n= j ;
         if (! n) break;
         如k"decc岫(lin, n 4ch) ;
         linEn] = ch;
          jok=decchk(lin, n+1,&chh) ;
         lin [n+1] =O;
         printf ( "/.s checks as %c\n", lin, jok ? 'T ' : 'F') ;
    }
    printf ( "Normal completion\n") ;
    return 0;
        294    肌im아ica／尸e印es Example Book

    }

     The example program that demonstrates Huffman compression of alphabetic text
has several separate tasks to perform. First, it must construct a statistical profile of
the kind of text to be compressed, in the form of a table of letter frequencies. It does
this using the file text .dat which, as supplied on the diskette, contains a particularly
racy passage from Thomas Hardy's Far from the Madding Crowd (New York: Harper,
1895).
   Next, the Hu卄man code itself is constructed from the frequency count. The
demonstration program prints out the entire code, allowing you to see how more
common letters are encoded in fewer bits than less common ones.
    The program then prompts repeatedly for an input line of text, compresses that
line, decompresses it, and prints out the result (hopefully the same as you input)
and the lengths of the line in uncompressed and compressed forms. Notice how a
compressed line is terminated by encoding a (spurious) rare character, while not
incrementing the message byte count. This ensures that on decoding, the spurious
character will not be fully decoded. In addition to trying ordinary text as input to
the program, you might try a line of all lower case e's, or all upper case X's.
/卓 Driver for routines hufmak, hufenc, hufdec */

#include <stdio . h>
#include <stdlib . h>
#include (string. h>
#include "nr. h"
#include 'nrutil. h"

#define 片C 512
#define MQ (2牛甘C- i)

#define MAXLINE 256

mnt inain(void)
{
         jot k;
         unsigned long i, j ,ilong, n,nb,nh,nlong,nt, lcode=片AXLI甘E,nch,nfreq[257J;
         unsigned char *code,mess[MAXLINEJ ,ness[MAXLINE) ;
         huff code hcode;
         FILE *fp;

          code=cvector (0.MAXLINE) ;
         hcode. icod=lvector(1,MQ) ;
         hcode .ncodrlvector ( 1,MQ) ;
         hcode.1eft=1vect0r(i ,MQ) ;
         hcode.right=lvector (1,MQ) ;
         for (j=1; j<=MQ; j++) hcode.icod[ j] =hcode.ncod[j] =0;
         /卞 construct a Letter frequency table from the file       text. dat 卞/
         if ( (fp = fopen( "text. dat ", 'r ") ) == NULL)
              nrerror ( "Input file text. dat not found. \n") ;
         for (j=1; j<=256; j++) nfreqEjj=O;
         while ( (k=getc (fp) ) != EOF) {
              if ( (k -= 31) >= 1) nfreq[k] ++;
         }
         fclose(fp) ;
                                            Chap旭r 20: Less小加／Tie放：a/ A勺orit加us         295
     nch'96;
     /* here is the initialization       that constructs the code */
     hufmak(nfreq,nch ,&ilong,立nlong ,立hcode) ;
     printf ( "ind char nfreq ncod icod\n") ;
     for (j=1; j<'nch; j++)
         if (nfreq[ j] ) printf ( "/,31u Y.c %61u '/.61u /,61u\n",
               j ,(char) (j+31) ,nfreq[ j] ,hcode.ncod[ j] ,hcode.icod[ j] );
     for C; ;)
                 {
         ／李 no日 ready to prompt 如r lines to encode 衣／
         printf ( "Enter a line: \n") ;
         if (gets ( (char *)亡messCl] ) == NULL) break;
         n=strlen ( (char *)&mess[1] );
         /中 shift from 256 character alphabet to 96 printing characters */
         for (j=1; j<=n; j++) messEji -= 32;
         /* here we Huffman encode mess[1. . nj */
         nb=0;
          for (j=1; j<=n; j++) hufenc ( (unsigned long)mess[ j] ,&code,klcode,立nb,立hcode) ;
          nh=(nb>>3)+1;
           /卞 message termination (encode a single long character) 方/
          hufenc(ilong ,&code,&lcode ,&nb,&hcode) ;
          /* here we decode the message, hopefully to get the original back 本/
          nb=0;
          for (j=1; j< 'MAXLINE; j++) {
               hufdec (立i, code,nh,&nb,&hcode) ;
               if Ci == nch) break;
               else ness口] =(unsigned char)i;
          }
         if (3 > icode) nrerror ( "Huffman coding: Never get here") ;
         nt= j- 1;
         printf ( "Length of line input, coded= /.lu /.lu\n", n,nh) ;
         printf ( "Decoded output: \n") ;
         for (j=1; j<=nt; j++) printf ( "/.c", (char) (ness[ j] +32) );
         printf ( "\ n") ;
         if (nt != n) printf ( "Error! : n decoded != n input\n") ;
         if (nt- n == 1) printf ( "May be harmless spurious character. \n") ;
    }
    free_ cvector (code ,O ,MAXLINE) ;
    free_lvector (hcode . right, 1 ,MQ) ;
    free_lvector (hcode . left, 1, MQ) ;
    free_lvector (hcode . ncod, 1,MQ) ;
    free_lvector (hcode. icod,1,MQ) ;
    printf ( "Normal completion\n") ;
    return 0;
}

     The demonstration program for arithmetic compression is very similar to that
for Huffinan compression. As before, we construct a letter frequency table from a
corpus that is statistically similar to the text that we are expecting to compress, then
initialize the code, and finally encode/ decode messages.
    There are several characters' worth of output associated with message initializa-
tion and message termination in arithmetic coding, so one would not normally begin
a new compression for each input line (as is done in the following demonstration).
Rather, a whole file would normally be compressed in a single pass.
    296       N미nerica/ 尸ec徊es Example Book

/* Driver for routines arcmak and arcode 中/


#include <stdio. h>
#include < stdlib . h>
#include <string, h>
#include "nr. h1'
#include "nrutil. h11


#define MC 512


#def ins NWK 20


#def ins MAXLINE 256


mnt main(void)
{
          jut k;
      unsigned long i, j ,lc, lcode=MAXLtNE,n,nch,nrad,nt, nfreqE257] ,tmp, zero=0;
      unsigned char *code,mess[MAXLINE] ,ness[MAXLINE] ;
      arithcode acode;
      町LE 卞fp;


      code=cvector (0, MAXLINE) ;
      acode. ilob=lvector (1 1 NWK) ;
      acode. iupb=lvector (1, N可K) ;
      acode. ncumfq=lvector (1, MC+2) ;
      if ( (fp = fopen( "text. dat ", "r ") ) == NULL)
          nrerror ( "Input file text. dat not found. \n") ;
      for (j= 1; j<=256; j++) nfreq[ j] =0;
      while ( (k=getc (fp) ) != EOF) (
          if ( (k -= 31) >= 1) nfreq[ k) ++;
      }
      fclose (fp) ;
      nch=96 ;
      nrad=256;
          /* here is the initialization    that constructs the code 方/
      arcmak (nfreq, (int) nch, (int) n工ad,立acode) ;
      ／卞 no日 ready to prompt 如r lines to encode 卞／
      如r （·. ·, ) {
          printf ( "Enter a line: \n ") ;
          if (gets ( (char *)kmess[1) ) == NULL) break;
              n=strlen ( (char s)如ness[1] );
              /半 shift from 256 character alphabet to 96 printing      characters 卓/
              for (j= 1; j<=n; j++) mes訌刃 口＝ 32;
              /幸 message initialization    */
              lcrl;
              arcode (立zero,&code,klcode,&lc, 0,&acode) ;
             ／卞 here 日a arith皿etically encode mess (1:n) 牛／
              for (j= 1; jc=n; j++) {
                   tmp=mess[ j] ;
                   arcode (&tmp, &code,&lcode,klc, 1, &acode) ;
              }
              /本 message termination */
              arcode（立uch , 立code小lcode,&lc 1,立acode) ;
              printf ( 'Length of line input, coded= %lu %l끄\n", n, lc- l) ;
              /半 here we decode the message, hopefully to get the original      back */
              lc 'l;
                                                     Ch햐ter 20: Less-Numerical Algorithms   297
          arcode (&zero,kcode,&lcode, &lc 1O,&acode) ;
          for (j '1; j<=lcode; j++) {
              arcode(ki, tcode,klcode,klc, -1,&acode) ;
              if (i == ach) break;
              else ness[ j] =(unsigned char)i;
          }
          if (j > lcode) nrerror ( "Arith. coding: Never get here ") ;
          nt= j- 1;
          printf ( "Decoded output: \n') ;
          for (j 'l; j<=nt; J++) printf ( '/.c ', (char) (ness[ j] +32) );
          printf ( "\ n") ;
          if (nt != n) printf ( "Error ! j decoded != n input. \n') ;
     }
     fzee_ cvec如r (cod이이NAXLI甘E) ;
     free_lvector (acode . ncu皿fq, 1,MC+2) ;
     free_lvector (acode. iupb,1,NWK) ;
     free_lvector (acode. ilob, I ,NWK) ;
     printf ( " 如rinal coinpletion\n") ;
     return 0,
 }

     The Numerical Recipes book ends on a note of numerical denouement with the
calculation of 7r to some 2398 decimal places. The following demonstration program,
and its one additional function, repeats that calculation, and also uses the various
mul뺘脆 prec油on routin田 的 calcula扼 a couple 可 simpler qua的ties at high precision,
 \／牙and 2 - \／牙. You might wonder why bother with the latter quantity. The answer
is that the multiple precision integer divide routine mpdiv happens not to be used at
all in the calculation of 冗 (although the routine for reciprocals, mpinv, is used). To
give it some exercise, we therefore calculate 2卜 v牙 by the following nutty scheme
that does make use of the integer divide:

                          2 x
                                          ]                              V5)
                                2M
                                     2,
                                              =   1 remainder                       "
                              x
                                                                (2
                                                                               X2
                                                                     -
at least to the same approximation that ＼厄 is computed. Here square brackets
indicate integer part, and M is the number of binary digits in the precision that you
supply when prompted.
    Before you go off and compute a million digits of 兀, be sure to read the main book's
note about the routine mp2dfr for converting from base 256 to decimal fractions.
Unless you are satisfied with knowing 冗 in base 256 (or binary, octal, or hexadecimal),
you will need to rewrite that routine to make it faster.
/s Driver 如r 叫：1routines 卞／

#include <stdio.h>
#include <math.h>
#include 'nr. h"
#include "nrutil . h'1

#detine IA0FF 46
#define 月MAX 1024

void mpsqr2(int n)
{
298         肌imericai 肋印的 Examp旭 Book

    milt j, m;
    unsigned char 卓工．卞y, 中t1中q，中r, 卓8;

    x=cvector (1,NMAX) ;
    y=cvactor (1,NMAX) ;
    trcvector ( 1,NXAX) ;
    q=cvector (1,NMAX) ;
    r=cvector (1,NMAX) ;
    s=cvector (1.3*NMAX) ;
      t ［幻 =2;
      for (j '2; j<=n; j++) tEjirO;
      mpsqrt (x, x,t ,n,n) ;
      mpmov (y, x,n) ;
      printf ( "sqrt (2)=\n") ;
       5 口］=y 口］+IAOFF;
      s[2:J= ' . J ;
                                                           N */
      /年 caution: next step is 1卞*2! omit it for large
      mp2dfr仕y[1] ,&町幻 md ,tm) ;
      町In＋引＝0;
      printf ( " %64s\n", ks[l] );
                                                 6 place: \n") ;
      printf ( 'Result rounded to 1 less base-26
       /* use s as scratch space */
      mpsad(s, x.n, 128) ;
      mpmov (y,ks[1] ,n-1) ;
       s [i] =y [1] +IA0FF;
      訌기 = } . } ;
      /s caution: next step is 1*卞2 ' omit it    for la工ge N */
      mp2dfr仕y 口］,t町2] ,n尸2.km) ;
      町m＋幻＝0;
      printf (" %64s\n", ks口) ;
      printf ( "2-sqrt (2)=\n") ;
                                                e the mpdiv function 巾/
      /* Calculate this the hard way to exercis
      mpdiv (q,r, t, x,n,n) ;
      s[1] =r[ 1] +I40FF;
      訌기 = J . J ;
                                                        N 卞／
      ／卞 caution: ne工t step is N小卞2 ' omit it 如r large
      mp2dfr (krEl] ,&s[2] ,n-1,km) ;
       町m＋刃 =0;
       printf ( " Y.64s\n", ks[l] );
       free_ cvector (s, 1,3*月MAX) ;
       free_ cvector (r, 1,NXLI) ;
       free_ cvector (q,1.NMAX) ;
       free_ cvector (t. 1,11111) ;
       free_ cvactor (y, 1,NMAX) ;
       free_cvector (x 11, NXAX) ;
}

mllt main(void)
{
     mnt n;

       如r (; ; ) {
          printf ( "Input n\n") ;
          if (scanf ("%d", kn) == EOF) break;
          a恥qr2佃）;
          mppi(n) ;
        }
                                    Ch카升or 20: Less小加／nerical Algorit／가us   299

printf ( "Normal completion\n") ;
return 0;
Appendix A: Header Files

        The Numerical Recipes functions, and the example routines in this book,
    make use of the following header files. The files listed here are abbreviated
    forms of those found on the Numerical Recipes diskettes, in that they do not
    show the alternative constructions for use with compilers that do not support
    the full prototype specifications of the ANSI C standard. We list the full
    ANSI prototypes because they are more helpful in checking the data types
    expected by each function. They can easily be abbreviated to the traditional
    K也R 兀rm.



    File nrutil. h contains a number of macros and utility routines, which are dis
cussed in Chapter 1 of the main book. The macros are used for common mathematical
operations such as squaring a quantity, finding the maximum of a pair of numbers,
and so on. The utility functions are used for error reporting, dynamic allocation and
deallocation of memory for vectors and matrices, and the creation of references to
submatrices. Source code for the utility functions is in the file nrutil . c, listed in
Appendix B. Note that nrut ii. h and nrutil . c are not copyrighted, and you may
copy them freely for any purpose.
#ifndef _NR_UTILS_H_
#define .J1R_UTILS_H_

static float sqrarg;
#define SQR(a) ( (sqrarg=(a) ) == 0.0 ? 0.0 : sqrarg*sqrarg)

static double dsqrarg,
#define DSQR(a) ( (dsqrarg=(a) ) == 0. 0 ? 0.0 : dsqrarg*dsqrarg)

static double dmaxarg11dma工arg2;
#defiue DMAX (a,b) (山maxargl=(a) ,dmaxarg2=(b) ,(dmaxargl) > (dmaxarg2) ?\
        (dma工argi) : (dma工a工g2) )

Static double dminargl,dminarg2;
#define DMIN(a,b) (dminarg1=(a) ,dminar82=(b) , (dminargl) < (dminarg2) ?\
        (dminargl) : (dminarg2) )

static float maxargl,maxarg2;
#define FMAX (a,b) (ma工argl=(a) ,ma工arg2=(b) ,(maxaxgl) > (maxarg2) ?\
         (maxargi) : (maxarg2) )

static float ininargl.minarg2;
#def ins FMIN(a,b) (minarg1' (a) ,minarg2=(b) , (minargi) < (ininarg2) ?\
        (minargi) : (minarg2) )


 300
                                                        Appendix A: Header Files         301

 static long lmaxargl,1maxarg2;
 #define LMAX (a,b) (lmaxargl= (a) ,lmaxarg2= (b) ,(lmaxargl) > (1maxarg2)
                                                                           ?\
          (lmaxargl) : (1maxar82) )

 static long lmina工gl,1minarg2;
 #define LMIN(a, b) (lininargl=(a) ,lminarg2=(b) ,(lminargl) < (1minarg2)
                                                                          7\
         (lainargi) : (1minarg2) )

 static mllt mrnaxargl, imaxarg2;
 #define IMAX (a,b) (imaxargl= (a) ,iaaxarg2= (b) ,(imaxargl)
                                                                > (imaxarg2) ?\
          (imaxargi) : (imaxarg2) )

 static mllt iminargl, iminarg2;
 #define IMIN(a,b) (iminargl=(a) ,ixnina工g2= (b) ,(iminargl)
                                                                < (iminarg2) ?\
         (iminargi) : (iminarg2) )

 #defmne SIGN(a,b) ( (b) >= 0. 0 ? fabs (a) : -fabs(a) )

 #if defined (_ _STDC_ _) I 1 defined(ANSI) 1 1 defined(NRANSI) /牛 ANSI */

 void nrerror (char error_ text[ fl ;                               .
 float *vector (long nl, long nh) ;
 mnt *ivector (long ni, long nh) ;
unsigned char *cvector (long nl, long nh) ;
unsigned long 中lvector (long ni, long nh) ;
double *dvector (long nl, long nh) ;
float **matrix (long nrl, long nrh, long ndl, long
                                                         nch) ;
double **dinatrix (long nrl, long nrh, long ndl, long
                                                           nch) ;
mllt **imatrix (long nrl, long nrh, long ndl, long
                                                        nch) ;
float **submatrix (float **a, long oldrl, long oldrh, long
                                                                  oldcl, long oldch,
         long newrl, long newcl) ;
float s*convert卞matrjx (float Ca, long nrl, long
                                                       nrh, long ndl, long nch) ;
float ***f3tensor (long nrl, long nrh, long ndl, long
                                                            nch, long ndl, long ndh) ;
void free_ vector (float 京v, long nl, long nh)
                                                 ;
void free_ ivector (int 卓v, long nl, long nh) ;
void free_ cvector (unsigned char iv, long nl, long
                                                         nh) ;
void free_lvector (unsigned long 李v, long nl,
                                                   long nh) ;
void free_dvector (double 本v, long nl, long nit) ;
void free_matrix (float 本斗a, long nrl, long nrh,
                                                      long ndl, long nch) ;
void free_disatrix (double 中半a, long nrl, long
                                                   nrh, long ndl, long nch) ;
void free_ imatrmx (int urn, long nrl, long nrh,
                                                     long ndl, long nch) ;
void free_ submatrmx (float 卞＋t, long nrl, long
                                                    nrh, long ndl, long nch) ;
void free_ convert_isatrix (float 京ib, long nrl,
                                                    long nrh, long ndl, long nch) ;
void free_ f 3tensor (float ii中t, long nrl, long
                                                    nrh, long ndl, long nch,
        long ndl, long ndh) ;

#elsa ／李 ANSI 才／/
／李 traditional - K立a 半／

void nrerrorQ;



void free_ f3tens0rO;

#endif 1本 ANSI *7
 302     N切rnerica／尸e帥殆S Examp旭 Book

＃이dif ／卞 ＝甘R_UTILS尸Hm +/


    The complex. h header file contains prototypes for a set of routines that perform
arithmetic functions with complex variables. Complex data types, and predefined
arithmetic operations on complex numbers, are not part of the ANSI C standard.
However, if your C library provides such facilities, you may use them in place of the
ones we provide. Source code for these functions may be found in Appendix C.

*ifndef _FCOMPLEX. DECLAaE_T_
typedef struct FCOMPLEX {float r, i, } f complex;
#def mne _FCOMPLEX_DECLARE_T_
#endif /* _FCOMPLEX_DECLAftE_T_ 卞/

#if defined(_ _STDC_ _) I I defjned(ANSI) I I defined(NRANSI) /* ANSI */

fcomplex Cadd(fcomplex a, fcomplex b) ;
fcomplex Csub(fcomplex a, fcomplex b) ;
fcomplex Cmul(f complex a, fcomplex b) ;
f complex Complex (float re, float im) ;
f complex Conjg(fconlplex z) ;
fcomple工 Cdiv (fcomple工 a, fcompl日工 b) ;
 float Cabs (f complex z) ;
 fcomplex Csqrt (fcomplex z) ;
 fcomplex RCmul(float x, fcomplex a) ;

 *else ／字 A甘SI 卓／/

 f complex CaddO;



 fcomplex RCmnlO;

 #endif /卞 ANSI */


      The following is a list of prototypes for all functions in the Numerical Recipes
 software collection. This is a section of the file nr .h, a header file included in virtually
 all of the example routines in this book. As an alternative to including nr.h in your
                                                                                     that you
 programs, you may cuii from this file the references to the specific Recipes
 will be using, and incorporate them as individual      declarations.
 #ifndef _NR_H_
 *define _NR_H_

 #ifndef _FCOMPLEX_DECLARE. .T_
 typedef struct FCOMPLEX {float r, i; } f complex;
 *def mne _FCOMPLEX_DECLAB.E_T_
 #endjf /半 .FCOMPLEX...DECLARE_T_ */

 #ifndef _ARITHCODE_DECLARE. .T_
 typedef struct {
          unsigned long *ilob, 牛iupb, *ncumfq, jdif, nc,minint,ach,ncu皿,nrad;
 } arithcode;
 #def inc _ARITHCODE_DECLARE_T...
 #endif ／方 =ARITHCODE_DECLAR.民T= 方／

 #ifndef _HUFFCODL.DECLARE_T_
                                                      Appendix A: Header Files        303

typedef struct {
        unsigned long *icod, *ncod, *left, *right, nch,nodemax;
} huffcode;
#define _HUFFCODE_DECLARE_ T_
#endif /半 _HUFFCODE_DECLARE_T. */

#include <stdio.h>

#jf defined（小STD口_ ) I 1 defined(ANSI) I I defined（甘RA甘SI) /／半 ANSI 牛／

 void addint (double 本字uf , double 卞卞uc, 面uble 李牛res, ml1t nf) ;
 void airy (float x, float *aj, float *bi, float *aip, float *bip) ;
 void amebsa(float 半*p, float yD, milt ndim, float pbD,              float *yb,
         float ftol, float (* funk) (float 口) , mnt *iter, float tamptr) ;
 void 三moeba(float **p, float yE] , mltt ndim, float ftol,
         float (* funk) (float 0) , m11t *iter) ;
 float aslotry (float 牛卞p, float y口 , float PS끄itt口 , mnt ndim,
         float (* funk) (float 口) , m1lt ihi, float fac) ;
float amotsa(float 木*p, float yE] , float psum口, mllt ndim, float pb口 1
         float *yb, float (*funk) (float 0) , mllt ihi, float *yhi, float fec) ;
void anneal(float x[], float yE] , mllt iorder口, mllt ncity) ;
double a工lorm2 (double **a, ml1t n) ;
void arcmak (unsigned long nfreq[J, unsigned long nchh, unsigned long nradd,
         arithcode *acode) ;
void arcode (unsigned long *ich, u꾜signed char **codep, unsigned long *lcode,
         unsigned long 卞lcd, mnt isign, arithcode *acode) ;
void arcsum(unsigned long iin[ ], unsigned long mont口, unsigned long ja,
         mllt nwk, unsigned long nrad, u工lsigned long nc) ;
void asolve (unsigned long n, double bD, double x[], mnt itrnsp) ;
void atimes (unsigned long n, double x[], double rE] , m1lt itrnsp) ;
void avevar (float dataE] , unsigned long n, float 本ave, float 半var) ;
void balanc (float **a, mllt n) ;
void banbks (float **a, unsigned long n, mllt ml, ml1t m2, float **al,
         unsigned long indx[], float bE] );
void bandec (float *牛a, unsigned long n, m1lt ml, m1lt m2, float **al,
         unsigned long indx口, float *d) ;
void banxnul (float **a, unsigned long n, mnt ml, ml1t m2, float xE] , float bE] );
void bcucof (float yE] , float ylD, float y2E] , float yl2E] , float dl,
         float d2, float 牛卞c) ;
void bcuint (float yE] , float ylD, float y2E] , float yl2E] ,
         float xll, float xlu, float x21, float x2u, float xl,
         float x2, float *ansy, float *aimsyl, float *ansy2) ;
void beschb (double x, double *gainl, double *g쾨n2, double *gainpl,
         double *gamnti) ;
float bessi(mnt n, float x) ;
float bessiO (float x) ;
float bessil(float x) ;
void bessik (float x, float xnu, float 字ri, float *rk, float *rip,
         float *rkp) ;
float bessj (int n, float x) ;
float bessjO(float x) ;
float bessjl (float x) ;
void bessjy (float x, float xnu, float *rj, float *ry, float
                                                                 *rjp,
         float *ryp) ;
float bessk (int n, float x) ,
float besskO(float x) ;
float besskl (float x) ;
 :304       八加merica/ 尸ec刃es Example Book

fl oat bessy (int     n, float     x) ;
float    bessyo (float    x) ;
float    bassyl (float
                    x) ;
float beta(float z, float w) ;
float betacf (float a, float b, float x) ;
float betai (float a, float b, float x) ;
float    bico (int   n, jut k) ;
void bksub (int      ne, jut nb, mnt jf,           m1lt ki,    mllt k2, float      ***c) ;
float bnldev (float pp, jut n, long 卞idwu) ;
float brent (float ax. float bx, float cx,
        float (sf) (float) , float tol, float                   *xmjn) ;
void broydn(float xD, mnt n, jut *check,
           vojd (* vecfunc) (lnt,         float    [3, float  [3) );
 void bsstep(float       yE] , float      dydx[],     jut uv, float *xx, float           htry,
           float epa, float yscal[ ],             float *hdid, float *hnext,
           void (* derivs) (float, float            口, float      []));
 void caldat (loug julian,      jut *mm, jut *id, jut *iyyy) ;
void chder (float      a, float b, float cC] , float cder[], ml1t n) ;
float    chebev (float    a, float b, float cO, m11tm, float x) ;
 void chebft (float      a, float b, float cC] , m1lt n, float (* func) (float) );
'void chebpc (float cC] , float dE] , lot n) ;
 void chint (float a, float b, float cC] , float                  cjutD,     jut u) ;
 float chixy (float      b카lg) ;
 void choldc (float      **a, jut n, float p[ ]);
 void cholsl (float      **a, jut n, float p[ ], float b[ ], float x口) ;
 void chsone (float      bins[ ], float ebius[], jut ubins, mllt knstrn,
         float *df, float Schsq, float sprob) ;
 void chstwo (float binsl[ ], float bins2[], jut nbjns, jut knstrn,
         float *df, float *chsq, float *prob) ;
 void cisi (float     x, float     *Cj, float       ssj) ;
 void cntabl (iut **Im, jut ui, jut nj,               float *chisq,
         float 半df, float 卞prob, float                本cra皿rv, float        *ccc) ;
 void cutab2 (mut **nn, jut uj,            jut uj,     float    *h, float    *hx, float       *hy,
         float *hygx, float *hxgy, float *uygx, float *uxgy, float 本uxy) ;
 void convlv (float data口, unsigned long n, float respns[], unsigned long m,
         jut isign, float ansO) ;
 void copy (double **aout, double x*ain, jut n) ;
 void correl (float datal[ ], float data2[], unsigned long n, float ans[]);
 void cosft (float yE] , jut n, m1lt isign) ;
 void cosftl (float yE] , jut n) ;
 void cosft2(float       yE] , jut n, jut isign) ;
 void covsrt (float      **covar, m1lt ma, jut ia[ ],            jut mfit) ;
 void crank (uusigned long n, float wE] , float *s) ;
 void cyclic (float a口, float bE] , float c口, float alpha, float beta,
         float r口, float xD, unsigned long n) ;
 void daub4(float aD, unsigned long n, jut isign) ;
 float dawson(float x) ;
 float   dbrent (float ax, float bx, float cx,
           float (* f) (float) , float (* df) (float) , float               tol,    float    *xmin) ;
 void ddpoly (float c[ ], jut nc, float x, float pdD,                      jut ud) ;
 jut decchk (char striug[ ], jut n, char *ch) ;
 void derivs (float x, float yE] , float dydx口) ;
 float dfldmm(float x) ;
 void dfourl (double data口, unsigned long nn, m1lt isigu) ;
 void dfpmiu(float P口, jut n, float gtol, jut *iter,      float *fret,
          float （半func) (floa七 口 ) , void （京dfunc) (float 口 , float 口 )) ;
 float dfridr (float (* func) (float) , float x, float h, float *err) ;
                                                            Appendix A: Header Files      305
   void dftcor (float   w, float delta, float a, float b, float
                                                                       endpts[],
              float *corre, float *corim, float *corfac
                                                              );
    void dftint (float (* func) (float) , float
                                                   a, float b, float w,
             float 本cosint, float *sjnlnt) ;
    void difeq (int k, jot ki, mnt k2, lot
                                               jsf, mnt jal, jot isf,
              jot indexv口 , jot me, float 牛本s, float
                                                           牛卞y) ;
   void dlixunin (float p口 , float xi[ ] , jot
                                                  n, float *fret,
             float (* func) (float []), void (* dfunc)
                                                          (float [3, floatO) );
   double dpythag(double a, double b) ;
   void drealft (double data[], unsigne
                                           d long n, lot isign) ;
   void dsprsax (double sa口, unsigned long
                                                  ija[ ], double x[ ], double b[ ],
            unsigned long n) ;
   void dsprstx (double sa[], unsigne
                                        d long 幻aC] , 山＞uble x口 1 double b［그 1
            unsigned long n) ;
   void dsvbk計)(如uble 本牛u, double w口 , double
                                                       卞本v, m1lt m, jot n, double b口 ,
            double x[ ]);
   void dsvdcmp (double **a, jot a, jot
                                            n, double wD, double **v) ;
  void eclass (int nf[ ], jot n, lot lista[
                                               ], jot listbD,      jot in) ;
  void eclazz (iot nf 口, jot n, jot (*
                                          equjv) (int, jot) );
  float ei (float x) ;
  vojd eigsrt (float d[ ], float **v, m1lt n)
                                                 ;
  float elle (float phi, float ak) ;
  float ellf (float phi, float ak) ;
 float ellpi (float   phi, float en, float ak) ;
 void elahes (float   **a, mllt n) ;
  float erfcc (float x) ;
  float erff (float x) ;
  float erffc (float x) ;
  void eulsuni (float *suln, float term,
                                          jot Jterrn, float 日ksp[]);
 float evlrnem (float fdt, float d[ ],
                                         mnt in, float xms) ;
 float expdev (long *jdujn) ;
 float expmnt (iot n, float x) ;
 float fl (float x) ;
 float fldjrn (float x) ;
 float f2 (float y) ;
 float   f3 (float z) ;
 float   factlo ( jot n) ;
 float   factrl (iot n) ;
 vojd fasper (float   x口, float y[ ], unsigned long n, float
                                                                  ofac, float hjfac,
           float wkl口, float wk2[], 山lsjgned long
                                                         nwk, unsigned long *nout,
           unsigned long 幻max, float 싸江ob) ;
 void fdjac (int n, float x[ ] , float
                                         fvec口 , float **df,
           void (* vecfunc) (jnt, float O, float
                                                     []));
 vojd fgauss (float x, float a[], float
                                             ty, float dydafl 1 jut oa) ;
 void fillO (double **u, mnt o) ;
 vojd fit (float x口 , float y[] , m1lt
                                         ndata, float sig[ ]    jot mwt,
          float *a, float *b, float *siga,
                                                float *zigb, float *chj2, float
 void fitexy (float xD, float y[ ],                                               *q) ;
                                        jot ndat, float sigx[ ], float sigy[
                                                                              ],
          float *a, float *b, float *siga,
                                                float *sigb, float *chi2, float
vojd fjxrts (float d[ ], lot in) ;                                                *q) ;
void fleg (float x, float pl口, m1lt nl)
                                             ;
void flmoon (jnt n, mllt nph, long
                                      *jd, float *frac) ;
float fmjn(float x口) ;
vojd fourl (float data口, unsjgne
                                     d long on. jot isigo) ;
Void fourew (FILE *file[ 5] , jot *na,
                                          jot ml1b, jot *oc, jot mod) ;
void fourfs (FILE *fjle[ 5J, unsigne
                                       d long n1l口, mlit ndjm, jut isign)
void fouro(float data口, unsigned                                            ;
                                       long nn[], jot ndiin, m1lt isign) ;
 306    Numerical Recipes Example Book

void fpoly (float x, float p口, jot np) ;
void fred2 (int n, float a, float b, float t口, float fO, float 口［] ,
         float (sg) (float) , float (*ak) (float, float) );
                                                                          float w[],
float fredin(float x, jot n, float a, float b, float t[ ], float f[ ],
         float (* g) (float) , float (*ak) (float, float) );
void frenel(float x, float 京s, float cc) ;
                                                                *fret,
void frprmn(float p[ ], mllt n, float ftol, mllt *iter, float
         float （非fu끄c) (float 口 ) , void （牛dfunc) (float 口 j float 口 )) ;
void ftest (float datal[ ], unsigned long ni, float data2口, unsigned long n2,
         float 卞f, float 本prob) ;
float gaisdev (int ia, long *id山n) ;
float g缸usln(float xx) ;
float gaxnmp (float a, float x) ;
float gasmiq(float a, float x) ;
float gasdev (long Sidun) ;
                                                                x[], float 町］) ·，
void gaucof (int n, float aC] , float b口, float ainuO, float
void gauher (float x[], float wE] , m1lt n) ;
void gaujac (float x[], float wE] , into,     float alf, float bet) ;
void gaulag(float x[], float w[J, into,       float alf) ;
void gauleg(float xl, float x2, float xE] , float wE] , mnt n) ;
void gaussj (float **a, m1lt n, float **b, jot xn) ;
void gcf (float *ga工uncf, float a, float x, float *gln) ;
                                                                          tol,
 float golden(float ax, float bx, float cx, float (*f) (float) , float
          float exam1l) ;
 void gser (float *gamser, float a, float x, float *gln) ;
                                                                      heap口) ;
 void hpsel(unsigned long a, unsigned long n, float arr[ ], float
 void hpsort (unsigned long n, float ra口) ;
 void hqr (float 京本a, mllt n, float 日r口 , float 日1口）;
 void hufapp (unsigned long index口, unsigned long nprob[], unsigned long n,
        unsigned long i) ;
void hufdec (unsigned long *ich, unsigned char *code, unsigned long lcode,
        unsigned long 方ob, huffcode *hcode) ;
void hufenc (unsigned long ich, unsigned char **codep, unsigned long *lcode,
        unsigned long 本ob, huffcode *hcode) ;
void hufmak (unsigned long nfreq口, unsigned long nchin, unsigned long 本ilong,
        unsigned long 本nlong, huffcode Ihcode) ;
void hunt (float xx[], unsigned long n, float x, unsigned long *jlo) ;
 void hypdrv (float s, float yy[], float dyyds口) ;
 fcomplex hypgeo (fcornplex a, fcomplex b, fcomplex c, fcoiuplex z) ;
 void hypser (fcomplex a, fcomplex b, fcomplex c, fcomplex z,
         fcomplex Sseries, fcomplex *deriv) ;
 unsigned short icrc (unsigned short crc, unsigned char 半bufptr,
         unsigned long len, short uinit, mnt jrev) ;
 unsigned short icrcl (unsigned short crc, unsigned char onech) ;
 unsigned long igray (unsigned long n, mllt is) ;
 void imndexx (unsigned long n, long arr[ ], unsigned long mndx[]);
 void mndexx (unsigned long n, float arr口, unsigned long indx[]);
 void interp (double 李半uf, double **uc, mnt nf) ;
 mnt irbitl (unsigned long *iseed) ;
 m1lt irbit2 (unsigned long *iseed) ;
 void jacobi(float **a, mllt n, float dE] , float 木* v, mllt *nrot) ;
 void jacobn(float x, float yE] , float dfdx[], float **dfdy, m11t n) ;
 long julday (int isis, m1lt id, mnt iyyy) ;
 void kendll (float datalD, float data2E] , unsigned long n, float *tau, float 卞a,
         float *prob) ;
 void kend12 (float **tab, m1lt m, mllt j, float 京tau, float *z, float 京prob) ;
 void kermom(double wE] , double y, mllt a) ;
                                                          Appendix A: Header Files                307

void ks2dls (float  x1D, float yl[ ], unsigned long ni,
         void (* quadvl) (float, float, float *, float 卞, float         京, float      *),
         floa七 京dl, float 京prob) ;
void ks2d2s (float xl 口, float yl[ ], unsigned long 01, float x2口, float y2[],
        unsigned long 02, float 中d, float 枉rob) ;
void ksone (float data口, unsigned long n, float (* func) (float) , float 卞d,
        float 卞prob) ;
void kstwo (float datal 口, unsigned long ni, float data2[], u工lsigned long n2,
        float 卞d, float 京prob) ;
void laguer (fcomplex aD, jot m, fcomplex *x, m11t 卒its) ;
void lfit (float x口, float y[ ], float sig口, mnt ndat, float          a[ ],     jot ia[ I1 ,
         jot ma, float    半卓covar, float   *chisq, void (* funcs) (float,       float 口, lot) );
void linbcg (unsigned long n, double b口, double xi] , mnt itol,              double tol,
           mllt itmax, mnt Siter, double *err) ;
void lioinio (float p1] , float xi口, jot n, float 卓fret,
         float （本f1끄ic) (float 口 ))
                                    ,,
void lnsrch (int n, float xold[ ], float fold, float g口, float p[ ], float                  x口,
           float 卞f, float stpniax, jot 本check, float (xfunc) (float 口) );
void load(float xl, float vi] . float yE] );
void loadl (float xl, float vi 口, float yD) ;
void 10ad2 (float x2, float v2[], float y[ ]);
void locate(float xx[], unsigned long n, float x, unsigned long *j) ;
void lop (double 衣Sout, double 本本u, mnt n) ;
void lubksb(float **a, mnt n, jot *indx, float b[ ]);
void ludcrnp (float 卄a, jot n, jot 中iodx, float 本d) ;
void machar ( jot 卞ibeta, jot 卞it, jot *irnd, jot *ngrd,
        jot *machep, m1lt *oegep, m11t *iexp, mllt *minexp. jot 抑naxexp,
        float 卞eps. float 李epsoeg, float 卞xmin, float *xmax) ;
void matadd(double 卓本a, double 牛卞b, double 卓卓c, jot n) ，·
void matsub (double 半京a, double 卞本b, double 卞京c, m1lt o) ;
void medfit (float xi] , float yE] , jot ndata, float 牛a, float Sb, float             卓abdee) ;
void memcof (float    data口, jot n, jot m, float     *xms, float   d[ fl ;
jot metrop(float     de, float t) ;
void mgfas (double *卓u, jot n, jot maxcyc) ;
void mglin(double 牛*u, mnt o, jot ncycle) ;
float midexp (float (卞funk) (float) , float aa, float bb, lot o) ;
float inidiof (float (京funk) (float) , float aa, float bb, jot n) ;
float midpot (float (* func) (float) , float a, float b, jot n) ;
float midsql(float (京tunk) (float) , float aa, float bb, jot n) ;
float midsqu(float (* funk) (float) , float aa, float bb, jot 0) ;
void mjser (float (* func) (float 口) , float rego口, jot odim, unsigned long opts,
         float dith, float Save, float 卓var) ;
void sunid(float yE] , float dydx[], int nvar, float xc, float htot,
         jot ostep, float yout그, void (* derivs) (float, floati] , floatED) ;
void mnbrak (float 京ax, float 卞bx, float *cx, float 本fa, float *fb,
         float 本fc, float (* fuoc) (float) );
void mnewt (iot ntrial,   float x[], jot o, float toix, float tolf) ;
void momeot (float datal] , mllt n, float 宰ave, float 中adev, float           Ssdev,
        float; 本var, float 方ske日 1 float; 卞curt) ，·
void mp2dfr (uosigned char a口, unsigned char si] , jot o, jot Sin) ;
void mpadd(uosigoed char wE] , unsigned char ui] , unsigned char vi] ,            jot n) ;
void inpdiv (uosigned char q口, uosigoed char n [j,      unsigned char u[ ],
        unsigned char vi] , jot o, mllt a) ;
void mpiov (unsigoed char u口, unsigned char 吐] ,        jot n, jot a) ;
void mplsh(山lsigned char u[ ], m11t o) ;
void mpmov (unsigned char u口, unsigned char v口, jot o) ;
void inpmul(unsigned char v口, 山lsigned char ui] , unsigned char vi] , int              o,
 308     Numerical Recipes Example Book

          jot in) :
 void mpneg(unsigned char uD, ml1t n) ;
void mppi(int n) ;
void mprove (float 肛李a, float 卞京alud, mllt n, in七 mndx口 , float b口 ,
         float xD) ;
void mpsad(unsigned char wD, unsigned char u[J, jot n, m1lt iv) ;
void mpsdv (unsigned char wCJ, unsigned char u[J, mnt zl, jot iv, jot *ir) ;
void mpsmu(unsigned char w[], unsigned char uC] , jot n, m1lt iv) ;
void inpsqrt (uosigned char wD, unsigned char u[], unsigned char yE] , jot o,
         mnt in) ;
void rnpsub(int *is, 山lsigned char wE] , unsigned char u[ ], unsigned char v口,
          jot o) ;
void mrqcof (float x口, float yE] , float sig[ ], mnt odata, float a[],
          jot ia口 , jut ma, float 卞京alpha, float beta口 , float 李chisq,
         void （京funcs乂float, float 口 , float 卞， float 口 , int) ) ;
void inrqmmn(float xLI , float y口, float sig口, m1lt ndata, float aD,
          jot iah] , m1lt ma, float **covar, float **alpha, float *chisq,
         void (* funcs) (float, float [], float 宰, float LI , int) , float talainda) ;
void newt (float x[] , m1lt n, m1lt *check,
         void (* vecfunc) (int. float 口, float LI ) );
void odeint (float ystartE] , m1lt nvar, float xl, float x2,
         float epa, float hi, float 노nin, jot *nok, jot *nbad,
         void (*derivs) (float, float [], float 口) ,
         void (*rkqs) (float 口, float [1, int, float *, float, float,
         float [], float 京, float 中, void (s) (float, float 口, float 口) ));
void orthog(int n, float anuD, float alpha口, float beta[], float a口,
         float b口 ) ;
void pade (double cof口, mllt n, float *resid) ;
void pccheb(float dE] , float cE] , m11t n) ;
void pcshft (float a, float b, float d口, m11t n) ;
void pearsn(float x[], float yE] , unsigned long n, float 半r, float *prob,
         float *z) ,·
void period(float x[], float yE] , jot n, float ofac, float hifac,
         float pxD. float pyE] , jot up, jot *nout, mllt *jmax, float *prob) ;
void piksr2(int o, float arr口, float brr口) ;
void piksrt (iot n, float arr[ ]);
void pinvs (mnt idl, jot je2, m1lt jel, mnt jsf, m1lt jcl, mnt k,
         float. 本李半c, float; 李卓s) ·，
float plgndr (int 1, jot in, float x) ;
float poidev (float xm, long 卞idum) ;
void polcoe(float xD, float yE] , jot o, float cofD) ;
void polcof (float xaE] , float yaD, jot n, float cof[]);
void poldiv (float uD, jot n, float v口, jot nv, float qD, float rED;
void p01102(float xiat] , float x2a口 , float **ya, mnt m, mllt n,
         float xl, float x2, float *y, float *dy) ;
void polint (float xa[], float yat] , jot n, float x, float *y, float *dy) ;
void powell(float p口, float 衣京xi, jot n, float ftol, jot *jter, float *fret,
         float (* func) (tloat E] ));
void predic (float dataD, jut ndata, float aD, jot m, float futureE] , jut nfut) ;
float probks (float alain) ;
void psdes (unsigned long tiword, unsigned long *irword) ;
void pwt (float aD, unsigned long n, jot isign) ;
void pwtset (mnt n) ;
float pythag(float a, float b) ;
void pzextr (mnt jest, float xest, float yestE] , float yzh] , float dyE] ,
         jot ov) ;
float qgaus (float (* func) (float) , float a, float b) ;
                                                   Appendix A: Header Files    309

void qrdcmp(float **a, jut n, float *c, float *d, jut *siug) ;
float qromb(float (* func) (float) , float a, float b) ;
float qromo(float (* func) (float) , float a, float b,
         float (* choose) (float (* )(float) , float, float, jut) );
void qroot (float p[], jut u, float *b, float *c, float eps) ;
void qrsolv (float **a, jut n, float cD, float d口, float b[ ]);
void qrupdt (float **r, float **qt, jut n, float u[ ], float yE] );
float qsimp(float (* func) (float) , float a, float b) ;
float qtrap(float (* func) (float) , float a, float b) ;
float quad3d(float (* func) (float, float, float) , float xl, float x2) ;
void quadct (float x, float y, float xx[], float yy[], unsigned long on,
         float 李fa, float; 本fb, float 本fc, float 京fd) ;
void quadxnx (float **a, jOt n) ;
void quadvl(float x, float y, float *fa, float *fb, float *fc, float *fd) ;
float ranO(long *jdum) ;
float ranl (loug *idun) ;
float r카l2(loug *jdum) ;
float ran3(loug *idwn) ;
float r카i4(long *idwn) ;
void rank (unsigued long n, unsigned long iudx口, unsigned b0ug jrank口) ;
void ranpt (float ptD, float regn口, jut n) ;
void ratint (float xaD, float ya[], jut n, float x, float *y, float *dy) ;
void ratlsq (double (* fn) (double) , double a, double b, jut nun, mllt kk,
         double cof口, double *dev) ;
double ratval (double x, double cof[], jut mm, jut kk) ;
float rc (float x, float y) ,
float rd(float x, float y, float z) ;
void realft (float dataD, unsigned long u, jut isign) ;
void rebiu(float rc, jut ud, float r口, float xin口, float xi[ ]);
void red(int izi, jut iz2, jut jzl, ml1t jz2, jut Jml, mllt jm2, mllt jmf,
         mllt idl, 뇨lt jcl, jnt jcf, mnt kc, float 斗＋李c, float 卞孝8) ;
void r日lax (double 非半u, double 卞卞rhs, jut u) ;
void relax2(double **u, double **rhs, ml1t n) ;
void resid(double 卞肛res, double 京卞u, double 水卞rhs, jut n) ;
float revcst (float xE] , float yD, jnt jorderD, mllt ucity, jnt n[]);
vojd revarse(int morderD, jut ucjty, mllt nO) ;
float rf (float x, float y, float z) ;
float rj (float x, float y, float z, float p) ;
void rk4(float yE] , float dydx[], jut u, floatx,       float ii, float youtD,
         void (*derivs) (float, float 口, float []));
void rkck(float yE] , float dydx[], jut n, float x, float h,
         float yout口, float yerrD, void (*deriys) (float, float [], float C] ));
void rkdumb(float vstaxt口, jut uvar, float xl, float x2, ml1t nstep,
         void (*derivs) (float, float 口, float 0) );
void rkqs (float yE] , float dydxD, jut n, float *x,
         float htry, float eps, float yscalD, float *hdjd, float *hnext,
         vojd (*derjvs) (float, float 口, float 0) );
vojd rlft3 (float ***data, float **speq, u工isjgued long nfl,
         unsjgued long un2, unsigned long nn3, jut isi目l) ;
float rofunc (float b) ;
vojd rotate (float **r, float **qt, jut n, jut i, float a, float b) ;
void rsolv (float **a, jnt n, float d口, float b口) ;
void rstrct (double **uc, double **uf, jut uc) ;
float rtbis (float (* func) (float) , float xl, float x2, float xacc) ;
float rtflsp (float (* func) (float) , float 工i, float x2, float xacc) ;
float rtnewt (void (* funcd) (float, float *, float *), float 工l, float x2,
         float xacc) ;
 310     Numerical Recipes Example Book

float rtsafe (vojd (* funcd) (float, float 本, float *), float xl, float x2,
         float xacc)
                     ..
float rtsec (float (卓func) (float) , float xl, float x2, float xacc) ;
void rzextr (int lest, float xest, float yestE] , float yzE] , float dy[], m1lt fly) ;
void savgol(float c[ ], jut np, milt nl, mllt nr, jut id, jut in) ;
void score(float xf, float y[], float f[ ]);
void scrsho (float (* fx) (float) );
float select (unsigned long k, unsigned long n, float arr[ ]);
float sellp (unsigued long k, 山lsigned long n, float             arr口) ;
void shell (unsigned long n, float a[ ]);
void shoot (int n, float v[ ], float f[ ]);
void shootf (int n, float yE] , float fE] );
void smmpl (float   **a, mnt isis, jut liE] ,   jut nil,    jut iabf,      jut *kp,
         float   *bmax) ;
void simp2 (float 京本a, jut u, jut l2口, jut n12, jut *ip, 工l1t kp, float 半ql) ;
void simp3(float 卞水a, m1lt ii,    jut ki, mllt ip, mllt kp) ;
void simplx (float 本*a, m1lt in , jut n, jut ml, jut xn2, jut m3, jut *icase,
        m1lt lzrov[ ], m1lt iposv[]);
void siinpr (float yE] , float dydxE] , float dfdx[ ], float **dfdy,
         m1lt n, float xs, float htot, jut nstep, float yout[],
        void (* derivs) (float, float [],       float   E] ));
void siuft (float yD, jut n) ;
void s1vsm2 (double 年京u, double 卞牛rh引 .,
void slvsml(double **u, double **rhs) ;
void sncndn(float uu, float emmc, float *sn, float *cn, float 半dim) ;
double snrxn(unsigned long is, double sx E] , jut itol) ;
void sobseq(int Sn, float xE] );
void solvde (mnt itmax, float cony, float slowc, float scalvO,
         jut jndexv口 , jut ne, jut ub, jut in, float 京京y, float 卞卓卞c, float               半卞S) ;
void sor (double 李本a, double 半斗b, double 方本c, double 本本d, double 京本e,
        如uble 卓李f, double 卓卞u, jut Jmax, doubi月 rjac) ;
void sort (unsigned long n, float mirE] );
void sort2 (unsigned long n, float arr[ ], float brrE] );
void sort3 (unsigned long n, float ra口, float rb[ ], float ic口) ;
void spctrin(FILE *fp, float p口, jut in, jut k, jut ovrlap) ;
void spear (fioat datal[ ], float data2[], unsigned long n, float 京d, float *zd,
        float 卓probd, float; 牛is, float 本probr的 ;
void sphbes (mnt n, float x, float *sj, float *sy, float *sjp, float *syp) ;
void splme2 (float xlaEj, float x2aE] , float **ya, jut is, jut u, float **y2a) ;
void splln2 (float xlaE] , float x2aE] , float *Sya, float **y2a, jut m, mnt 1l,
        float xl, float x2, float *y) ;
void splmne (float xE] , float yE] , jut n, float ypl, float ypn, float y2E] );
void splint (float   xaD, float   ya[], float y2aE] , jut n, float x, float           *y) ;
void spread(float    y, float  yyE] , unsigned long n, float x, jut m) ;
vojd sprsax (float   saE] , unsigned long ijaE] , float xE] , float bE] ,
        unsigned long n) ;
void sprsin(floa七 **a, jnt n, float   thresh, unsigned long umax, float sa[],
        unsigned long 幻a口 ) ;
void sprspm(float sa口 , unsigued long ijaD , float sbD, unsigned long jjbD,
        float scE] , unsigned long ijc口) ;
void sprstm(float sa口 , unsigued long ijaE] , float abE] , unsjgned long ijb[ ]
        float thresh, unsigned long umax, float scE] , unsigued long ijcE] );
void sprstp(float sa口, unsigned long ija口 , float sb[] , unsigned long ijb[ ]);
void sprstx (float sa口, unsigued long ijaL] , float x口, float bE] ,
         unsigned long u) ;
void stjfbs (float yD, float dydxL] , m1lt fly, float *xx,
         float htry, float eps, float yscal口, float *hdid, float                本hnext,
                                                     却pendix A: Header日es           311

         void (*derivs) (float, float [], float 口) );
void stiff (float y[], float dydxD, jOt n, float 卞x,
         float htry, float epa, float yscal[], float *hdid, float *hnext,
         void (*derivs) (float, float 口, float []));
void stoerm(float y[], float d2y 口, ml1t nv, float xs,
         float htot, jot nstep, float youtD,
         void (sderivs) (float, float [], float C] ));
void svbk引）(float **u, float 口[], float *卞v, jot in, ml1t n, float b[],
         float 工口 ) ;
void svdcmp(float **a, mllt m, jot n, float w[], float **v) ;
void svdfit (float x[], float y[], float sigE] , mllt ndata, float aD,
         mnt isa, float *Su, float 本京v, float w[], float *chisq,
         void (* funcs) (float, float C] , jot) );
void svdvar (float 方* V, mnt ma, float w[], float **cvm) ;
void toeplz (float r[ ], float xC] , float y[], mnt n) ;
void tptest (float datal[ ], float data2口, unsigned long n, float *t, float *prob) ;
void tqli (float d[], float e[], mnt l1, float ssz) ;
float trapzd(float (* func) (float) , float a, float b, jot ii) ;
void tred2(float t卞a, mnt n, float d[], float e[]);
void tridag(float a[], float bE] , float cC] , float r口, float u[ ],
        unsigned long n) ;
float trncst (float xC] , float yE] , mnt iorder[ ], jot ncity, ml1t n口) ;
void trnspt (int iorder[ ], mnt ncity, mnt n口) ;
void ttest (float datal口, unsigned long ni, float data2口, unsigned long n2,
        float *t, float 싸江ob) ;
void tutest (float datalE] , unsigned long ni, float data2[], unsigned long n2,
        float 小t, float 卞prob) ;
void tvofft (float datal口, float data2口, float fftl口,        float fft2口,
        unsigned long n) ;
void vander (double x[], double wE] , double q[], mnt n) ;
void vegas(float regn[], m11t ndim, float (* fxn) (float [], float) , m1lt m11it,
        unsigned long ncall, mnt itmx, ml1t nprn, float *tgral, float tsd,
        float *chi2a) ;
void voltra (int n, mllt m, float to, float h, float Ct, float **f,
        float (*g) (mnt, float) , float (*ak) (int, jot, float, float) );
void 日tl(float aD, unsigned long n, mnt isign,
        void (* wtstep) (float [], unsigned long, int) );
void 日tn(float aD, unsigned long iui口, mnt odin, mnt isign,
        void (* wtstep) (float C] , unsigned long, int) );
void 日日ghts(float 日ghts口 , iint n, float h,
        void (*kermom) (double 口, double ,int) );
mnt zbrac (float (* func) (float) , float 卞xl, float *x2) ;
void zbrak (float (* f工) (float) , float xl, float x2, mnt n, float xbl口,
        float 工b2口 1 mllt *nb) ;
float zbrent (float (sfunc) (float) , float xi, float x2, float tol) ;
void zrhqr (float a[]. mllt in, float rtr[ ], float rtiE] );
float zriddx (float (* func) (float) , float xl, float x2, float xacc) ;
void zroots (fcomplex a[], mntm, fcomplex rootsE] , mnt polish) ;

#else ／中 ANS工 卓／
／字 traditional - K&R 中／

void addintO;



void zrootsO;
312      Numerical Recipes Example Book

#endif ／京 ANSI 卓／


#endif /／本 _NFt_E_ 李／
    Appendix B: Numerical Recipes Utility Functions

          The utility functions listed below are used by many Recipes and Exam-
      pies in the Numerical Recipes collection. Along with the short error-reporting
      function, there are functions that we have found indispensable in the handling
      of vectors and matrices of different data types. A full discussion of the use of
      matrices and vectors within the Numerical Recipes collection may he found
      in Chapter 1 of Numerical Recipes, along with a description of ot her program
      milig standards adopted for the use of C in scientific programming.



#include <stdio . h>
#include <stddef.h>
#inc].ude <stdlib .h>
#defirie NR_END 1
#define FREE_ ARC char*

void nrerror (char error_text[ ])
/卞 Ntunerical Recipes standard error handler *1
{
        fprintf (stderr, 'Nwnerical Recipes run-time error. . .\n " ) ，·
        fprintf (stderr, " 加\n" 1 error_text) ;
        fprintf (stderr, ". . .now exiting to system. . .\n ") ;
        exit (1) ;
}

float *vector (long ul, long nh)
/卓 allocate a float vector with subscript range vCnl.
                                                      .nh] *1
{
        float; 卞V ;

         v=(float *)malloc ( (sjze_t) ( (nh-nl+ 1+NR_END) *sizeof (float) ));
         if ( 'v) nrerror ( 'allocatjon failure in vectorO ") ;
         return卜nl+ NR小E甘D;
}

 jot *ivector (long ol, long oh)
Is allocate an m11t vector with subscript range vEnl. . nh)
                                                            */
{
         jut; 布V ;

         v==(int *)malloc ( (size_t) ( (nh-ul+1+NR_END) *sizeof (mnt) ));
         if (! v) nrerror ( "allocatjon failure in ivectorQ1') ;
         return v-nl+NR_END;
}


                                                                                   313
    314   Nun冶rica／尸e아殆S Examp旭 Book

unsigned cha.r *cvector (long nl, long nh)
/* allocate an unsigned char vector with subscript range vEni. 1 n口 */
{
        unsigned char Cv;

          v=(unsigned char *)malloc ( (size_t) ( (nh-nl+1+NR_E甘D) *sizeof (unsigned char) ));
          if (! v) nrerror ('allocation failure in cvectorO ") ;
          return 中nl＋甘ft_END;
}

unsigned long *lvector (long nl, long nh)
/s allocate an unsigned long vector with subscript range v[nl. 1 nh] 卞/
{
        1끄isigned long 牛1r;

          v=(unsigned long *)malloc ( (size_t) ( (nh-nl+1+NR_END) *sizeof (long) ));
          if (! v) nrerror ("allocation failure in ivectorO ") ;
          return v-nl+NR_END;
}

double *dvector (long ni, long nh)
/卞 allocate a double vector with subscript range 吐nl. . nh] 京/
{
        double Cv;

          v=(double *)malloc ( (size_t) ( (nh-nl+1+NR_END) *sizeof (double) ));
          if (! v) nrerror ("allocation failure in dvectorO ") ;
          return v-nl+NR_END;
}

float *水matrix (long nrl, long nrh, long ndl, long nch)
I卓 allocate a float matrix with subscript range m[nrl. .nrh] [ndl. .nch] 卞/
{
          long i, nrow=nrh-nrl+1 ,ncol=nch-ncl+1;
          float 方中in;

           /卞 allocate pointers to rows */
          m=(float **) malloc ( (size_t) ( (nro日+甘R_END) *sizeof (floats) ));
          if (! m) nrerror ( "allocation failure 1 in matrixO ") ;
          in += NR_END;
          in -= nrl;

          /* allocate rows and set pointers to them */
          m[nrl] =(float 中） inalloc（佃皿乞n ( (1口0日抑tcol＋甘RUE川力相izeof仕b0at) ));
          if (! m[nrl] ) nrerror ( "albocation failure 2 in matrixO ") ;
          虹虹1] += NR_E甘D;
          可nrl] 戶＝ ndl;

          for (i "nrl+ l; i<=nrh;i++) m[i] =m[i- 1] +ncol;

          /* return pointer to array of pointers to rows 字/
          return in;
}

double 卞*dinatrix(long nrl, long nrh, long ndl, long nch)
/卞 allocate a double matrix with subscript range m[nrl. .nrh] [ndl. .nch] */
{
                                 Appendix B: Numerical Recipes Utility Functions        315

        long i, nrow=nrh-nrl+11 nco1=nch-ncl+1;
        doubi月 本＋m;

        /* allocate pointers to rows 肛1
        m= (double *s) malloc ( (size_t) ( (nrow+甘R_ END) ssizeof (double*)));
        if (! m) nrerror ( "allocation failure 1 in siatrixO ") ;
        m += MR_END;
        m -= nrl;

        /* allocate rows and set pointers to them *1
        m[nrl] =(double *) malloc ( (size_t) ( (nrow*ncol+NR_END)半sizeof (double) ));
        if (! m[nrl] ) nrerror ( "allocation failure 2 in matrixO ") ;
        mlnrl] += 甘a小END;
        m[nrl] -= ndl;

        for (i=nr1+1; i<=nrh;i++) mEi] =mCi-1] +ncol;

        /* return pointer to array of pointers to rows */
        return m;
}

m11t 半* imatrix (long nrl, long nrh, long ndl, long nch)
/本 allocate a mllt matrix with subscript range m[nrl. .nrh그 [ndl. .nch] 卞/
{
        long i, nrow=nrh-nrl+1,ncol=nch-ncl+1;
        tnt 才李1n;

        /幸 allocate pointers to rows *1
        m= (int 本本） malloc ( (size_ t) ( (nro日＋NR_E甘D）卞sizecf (int；京）)) ．·
        if ( 'm) nrerror ( "allocation failure 1 in matrixO ") ;
        m += HR_END;
        a -= nrl;



        /* allocate rows and set pointers to them 中/
        m[nrl] =(int *) malloc ( (size_t) ( (nrow*ncol+NR_END) *sizeof (int) ));
        if (! m[nrl] ) nrerror ( "allocation failure 2 in matrixO ") ;
        m[nrl] += HR_END;
        m[nrl] -= ndl;

        for (i=nrl+1;i< =nrh; i++) m[i] =m[i_ 1] +ncol;

        /卞 return pointer to array of pointers to rows */
        return m;
}

float 卓半submatrix (float 卞ea, long oldrl, long oldrh, long oldcl, long oldch,
        long ne口rl, long nawcl)
/5 point a submatrix [newrl. .]Cne日cl. .] to a[oldrl. .oldrh) [oldcl. .oldch] */
{
        long i ,] , nro日=oldrh-oldrl+1, ncolroldcl-ne日cl;
        float; 卓卞nl;

        /* allocate array of pointers to rows */
        m= (float 李中) malloc ( (size_t) ( (nrow+NR_END) 京sizeof (float中) ));
        if (! m) nrerror ( "allocation failure in submatrixO ") ;
        m += NR_END;
    316   Num이七a/ 尸e帥旭s Examp旭 Book

          In -= ne日rl;

          /* set pointers to rows 巾／
          如r ( i=oldrl，尸newrl; i<=o1drh; i++,j卄） m口］=a［幻＋ncol;

          /* return pointer to array of pointers to rows 京/
          return a;
}

float **convert_matrix(float 巾a, long nrl, long nrh, long ndl, long nch)
/* allocate a float matrix mCnrl. .nrh) [ndl. .nch] that points to the matrix
declared in the st카1dard C manner as a[心ow) Incol] , where n工ow=nrh-nrl+1
and ncol=nch-ncl+1. The routine should be called with the address
ka[O] [0] as the first argument. 字/
{
          long i, j ,nrow=nrh-nrl+1,ncol=nch-ncl+1;
          float 京巾11l;

          ／卞 allocate pointers to ro日S 卞／
          m=(float 卞卓） malloc ( (size.-t) ( (nr이卄NR_E肛D相izeof (float昑）) ;
          if (! m) nrerror ( "allocation failure in convert_matrixO ") ,
          m += Nit_END;
          m 七＝ nrl;

          1* set pointers to rows 수/
          a [nrl] =a-ncl;
          如r (i '1, j=nrl+ i; i<nro日；i++,j ++) 可刃m口-1] +ncol;
          /* return pointer to array of pointers to rows 衣／
          return m;
}

float ***f3tensor (long nrl, long nrh, long ndl, long nch, long ndl, long ndh)
/* allocate a float 3tensor with range t[ nrl. .nrh] [ncl. .nch] [ndl. .ndh] */
{
          long i口 ,nrow=nrh-nrl+1,ncol=nch甘ncl+1,ndep=ndh-ndl+1;
          float ***t;

          /* allocate pointers to pointers to rows 수/
          t=(float; 卓李京） malloc (佃1z乞tKO江ow+NR_E吼D相izeof (float* 幻）) ;
          if (! t) nrerror ( "allocation failure 1 in 13ten80rO ") ;
          t += Nit_END;
          t -= nrl;

          ／本 allocate pointers to ro口s a끄d set 恥1小ers to them 方／
          t江虹l]=(float *卞） malloc（佃汪e_t) ( (nro日＋ncol+N艮E札汁sizeof (float* )));
          if ( 't[ nrl] ) nrerror ( "allocation failure 2 in f3tens0rO ") ;
          町虹1] += 甘R. END;
          t[ nrl] -= ndl;

          /* allocate rows and set pointers to them */
          t[ nrl] [ncl] =(float *) malloc( (size_t) ( (n工o日*ncol*ndep+NR_END) *sizeof (float) ));
          if ( 't[ nrl] [ncl] ) nrerror ( "allocation failure 3 in f3tens0rO ") ;
          t[ nrl] [ndl] += Nit_END;
          t[ nrl] [ndl] -= ndl;

          for (j=nc1+1; j<"nch; j++) t[ nrl] [j] =t[nrl] [j- 1] +ndep;
          for (i=nrl+1; i<=nrh; i++) {
                                 쟈汐end灰 B: Numerica/ 尸ec徊es (／甘片ty F切7C打ons   317

                 t [i] =t (i- i] +ncol;
                 t[ ij [nc1] rt [i- i] [ncli+ncol*ndep;
                 for (j=ncl+1; j<=nch; j++) t[ i] [jJ=t[ i:1 [j- 1] +ndep;
         }

        /* return pointer to array of pointers to rows */
        return t;
}
void free_ vector (float *v, long nl, long idi)
/* free a float vector allocated with vector () */
{
        free( (FaEE_ ARG) (v+nl- NR_END) );
}

void free_ ivector (int 李V, long nl, long nh)
/* free 키l mllt vector allocated with ivector () */
{
        free( (FREE_ ARG) (v+nl- NR_END) );
}

void free_ cvector (unsigned char 布v, long ni, long nh)
/卞 free an unsigned char vector allocated with cvector () 卞/
{
        free( (FREE.1ARG) (v+nl- Nft_END) );
}

void free_lvector (unsigned long 卞v, long ni, long nh)
/字 free an unsigned long vector allocated with lvector () */
{
        free( (FREE:ARG) (v+nl- NR_END) );
}

void free_dvector (double 本v, long nl, long nh)
/卞 free a double vector allocated with dvector () */
{
        free( (F1EE_ ARG) (v+nl- NR_END) );
}

void free_matrix(float 京京m, long nrl, long nrh, long ndl, long nch)
/s free a float matrix allocated by matrixO 京/
{
        free( (FREE1ARG) (m[nrl] +ucl-NR_END) );
        free( (FItEE_ARG) (m+nrl寸凡E肛D) ;
}

void free_dinatrix (double 卞*m, long nrl, long nrh, long ndl, long nch)
／中 free a 如uble matri工 allocated by dmatri工（) 中／
{
        free( (FREE_ARG) (m[nrl] +ncl-NR_END) );
        free( (FREE_ARG) (m+nrl- NR_END) );
}

void free_imatrix (int 方卞m, long nrl, long nrh, long ndl, long nch)
/中 free an mllt matrix allocated by imatrix() 中/
{
        free( (FIEE_ ARG) (m[nrlj+ ncl- Nft_END) );
318     肌ime比a／尸a加es Exa쨔抛 Book

        free( (FREE_ ARG) (m+nrl- NR_END) );
}

void tree_ submatrix (float **b, long nrl, long nrh. long ndl, long nch)
/* free a submatrix allocated by submatrix() */
{
        free( (FREE_ AItG) (b+nrl- NR_END) ),
}

void free..convert_matrix(float **b, long nrl, long nrh. long ndl, long rich)
/本 free a matrix allocated by convert1matrix() s/
{
        free( (FREE_ARG) (b+nrl- NR_END) );
}

void free_f3tensor (float ***t, long nrl, long nrh, long ndl, long nch,
        long ndl, long ndh)
/卞 free a float f3tensor allocated by f3tensor () 卞1
{
        free( (FREE_ ARG) (t[ nrlj [ncl] +ndl-NR_END) );
        free ( (FftEE_ ARG) (t [nrl] +ncj-月ft_END) );
        free( (FREE. ARG) (t+nrl- NR_END) );
}
Appendix C: Functions for Complex Arithmetic

    Complex data types, and arithmetic operations on complex numbers, are not
    a standard part of C. We have therefore included the following functions for
    use with the small number of Numerical Recipes routines that use complex
    variables. When using C libraries that support the use of complex numbers,
    references to these routines may be replaced by equivalent library functions.



#include <math.h>

typedef struct FCOMPLEX {f] .oat r, i; } fcoutplex;

f complex Cadd(f complex a, f complex b)
{
        fcomplex c;
        c.r=a.r+b.r;
        c. i=a.i+b. i;
        return C;
}

fcomplex Csub(fcomplex a, fcomplex b)
{
        f complex C;
        c.r=a.r- b.r;
        c. i=a. i- b.i;
        return C;
}


fcomplex Cmul(f complex a, fcomplex b)
{
        fcomplex C;
        c.r=a.r싸）.r- a. i卄）.1;
        c . i=a. i* b . r+a.r* b. i;
        return c,
}

f complex Complex (float re, fl oat im)
{
         f complex c;
         C. r=re;
         C. l= lm ;
         return C;
}

f complex Conjg(f complex z)

                                                                                3] q
    320   Numerica/ 尸ec戶es Examp旭 Book

{
          f complex C;
          C . r=z . r;
          c. i = 1Z . l ;
          return C;
}

fcomple工 Cdiv (fcomplex a, fco끼江e工 b)
{
          f complex C;
          float r, den;
          if (fabs(b.r) >= fab叭b. i) ) (
                   r=b. i/ b.r;
                   den=b.r+r* b.i;
                   c.r=(a.r+r* a. i) /den;
                   c. j=(a. i- r* a.r) /den,
          } else {
                   r=b.r/ b. i;
                   den=b. i+r싸.r;
                   c.r=(a.r* r+a. i) /den;
                   c. i= (a. i* r- a.r) /den;
          }
          return c,
}

float Cabs (fcomplex z)
{
          float x,y,ans, temp;
          x=fabs (z. r) ;
          y= fabs (z. i) ;
          if (x == 0. 0)
                     ans=y;
          else if    (y == 0.0)
                     ans=x;
          else if    Cx > y) {
                     temp=y／工；
                     ans＝工中sqrt (1. 0+tamp卞temp) ;
          } else {
                     temp=x/y;
                     카1s=y*sqrt (1. 0+tempatemp) ;
          }
          return 카1$ ;
}

fcomplex Csqrt (fcomplex z)
{
        fcoxnplex C;
        float 치y,吼r;
        if ( (z. r == 0. 0) k& (z. i        0.0) ) {
                  c.r=0. 0;
                  c. i=0. 0;
                  return c;
        } else {
                  x=fabs (z.r) ;
                  y= fabs(z. i) ;
                  if （工 >= y) {
                              r=y/ x;
                                         Append灰 C: Funct幻ns for（力mp旭xA片thme加            321

                               w=sqrt ( x) *sqrt (0 . 5* (1. 0+sqrt ( 1. 0+r* r) ) ) ;
                 } else {
                               r＝工／y;
                               w=5qrt (y) ssqrt (0. 5牛(r+sqrt (1 .0+r* r) ));
                  lJ


                 if    (z. r   >= 0. 0) C
                               c.r＝口 ;
                               c. i= z. i/ (2. 0sw) ;
                 } else {
                               c. j=(z. j >= 0) ? v : -V·．
                               C .r=z. i/ (2 . 0*c. i) ;
                 }
                 return C;
        }
}

fcomplex RCieul(float    x, fcomplex a)
{
        fcomplex C;
        C. r=x李a .r;
        C. i＝工＋a.i;
        return C;
}
Index of Demonstrated Routines
airy      101             chebev   68, 73-74
키nebsa    168, 182-183    chebft   68, 72, 74-75
a皿oeba    168, 172        chebpc   68, 75-76
anneal    168, 181        chint    68, 74
anorm2    288             choldc   6, 29
arcmak    290             cholsl   6, 29
arcode    290, 295        chsone   222, 228
arcs띠n    290             chstwo   222, 228-229
avevar    224             cisi     104
badluk    1, 3            cntabl   222, 232
balaiic   185, 191-193    cntab2   222, 233
banbks    13              convlv   209
bandec    6, 13           correl   209-210
banmul    12-13           cosftl   195, 201
bcucof    40, 49-50       cosft2   195, 202
bcuint    40, 49-51       covsrt   247, 252
beschb    81, 100         crank    237
bessi     99              cyclic   6, 19
bessi0    95              daub4    209, 219
bessil    97              dawson   105
bessik    101             dbrent   168, 170-171
bessj     95, 267         ddpoly   68-70
bessj0    91              decchk   292
bessjl    93              dfldim   178
bessjy    99-100          dfpmin   168, 179
bessk     98              dfridr   68, 71
bessk0    96              dftint   209, 218
besskl    97              eclass   139, 150
bessy     94              eclazz   139, 151
bessyo    92              ei       90
bessyl    93              eigsrt   185, 187
beta      84, 164         elle     109
betai     91              elif     108
bico      83              ellpi    110
bnldev    125, 128, 130   elmhes   185, 192-193
brent     168, 170        erfcc    89
broydn    153, 166        eulsum   68-69
bsstep    264, 270-273    evimem   209, 212-213
caldat    1, 3-4          expdev   125-127, 228
chder     68, 74-75       expint   90



322
                                 Index 可Demonstra旭d /：初Ut加es      323
fidim     175, 178             indexx     139, 144-146
factin    84                   irbiti     125, 131, 240
factrl    82                   irbit2     125, 131, 240
fasper    209, 217              jacobi    185, 187, 189
fgauss    260                   julday    2-3
fit       247-248, 250, 261    kendli     222, 238
fitexy    247-249              kendl2     222, 238, 240-241
fixrts    209, 214             ks2dls     222, 241-243
fieg      255-256              ks2d2s     222, 243
fimoon    1                    ksone      222, 229-231
fourl     195, 197             kstwo      222, 229-231
fourfs    195, 205-206         laguer     153, 160-163
fourn     195, 203, 205-206    if it      247, 250, 252-253
fpoly     255                  linbcg     6, 26
fred2     280-281              linmin     168, 173-177
fredex    280                  lnsrch     168, 179
fredin    280-281              locate     40, 44-45
frenel    103                  lop        288
frprmn    168, 176, 179        iubksb     6, 8, 10-11, 14-15, 19
ftest     222, 227             ludcmp     6, 8, 10, 14-15, 19
gaindev   125, 128             machar     290
ganinin   81, 100              medfit     247, 261-262
gainmp    85                   memcof     209, 212-214
gain皿q    85                   mgfas      284, 287-288
gasdev    125, 127, 223, 226   mglin      284, 286-288
gaucof    54, 64               midexp     54, 58
gauher    54, 62, 64           midinf     54, 58
gaujac    54, 63               midpnt     54, 57-58
gaulag    54, 61-62            midsqi     54, 58
gauleg    54, 60-61            midsqu     54, 58
gaussj    6, 10                miser      125, 137
gcf       87                   mmid       264, 269, 273, 275
golden    168-170              mnbrak     168-170
gser      86                   mnewt      153, 164-165
hpsel     139, 149             moment     222-223
hpsort    139, 144             mp2dfr     297
hqr       185, 193-194         mpdiv      297
hufapp    290                  mpinv      297
hufdec    290                  mppi       290, 297
hufenc    290                  mprove     14
hufmak    290                  mrqcof     247, 256, 258-259
hunt      40, 45               mrqmin     247, 256-258
hypdrv    111                  newt       153, 164-166
hypgeo    81, 111              odeint     264, 267-268, 270, 274, 276
hypser    111                  orthog     54, 65
icrc      290-292              pade       68, 71, 78-79
icrcl     290                  pccheb     68, 77
igray     290-291              pcshft     68, 75-76
324         Numerical Recipes Example Book

pearsn          222, 235                     rtbis      153, 155
period          209, 216-217                 rtflsp     153, 156
piksr2          139-140, 142                 rtnewt     153, 156, 159
piksrt          139, 141-142, 144            rtsafe     153, 156, 159
plgndr          103, 255                     rtsec      153, 156-157
poidev          125, 128-129                 rzextr     264, 272
polcoe          40, 46                       savgol     222, 244
polcof          40, 46-47                    scrsho     153, 175
poldiv          68, 70-71                    select     139, 148- 149
p011n2          40, 48-49                    selip      139, 148
polint          40-41, 57                    sfroid     277
powell          168, 173, 179                shell      139, 141
predic          209, 214-215                 shoot      277
probks          231                           shootf    277
psdes           125, 132- 133                 simplx    168, 180
pwt             209, 219                      simpr     275
pwtset          209, 219                      sinft     195, 199-201
pzextr          264, 270-272                  sncndn    110
qgaus           54, 59-60                     sobseq    125, 133-134
qrdcmp          6, 30                         solvde    277
qromb           54, 57                        sor       284-288
qromo           54, 58                        sort      139, 142, 144
qroot           153, 162-163                  sort2     139, 142-143, 237
qrsolv          32                            sort3     139, 145
qropdt          6, 34                         spctrm    209, 211
 qsimp          54, 56-57                     spear      222, 235-237
qtrap           54-55, 57                     sphbes     102
 quad3d         66-67                         sphfpt     277
 quadvl          241                          sphoot     277
 ra끄0            125, 238                     5p1ie2     40, 51-52
 rani            125                          5p1in2     40, 51-52
 ran2            125                          spline     40, 42-43
 ran3            125, 181                     splint     40, 43
 ran4            125, 133, 238                spread     247
 rank            139, 146-147                 sprsax     6, 21
 rat m1lt        40-42                        sprsin     20
 ratlsq          68, 71, 79-80                sprspm     23, 25
 ratval          68, 71, 78                   sprstm     25
                 107                          sprstp     22-23
 rd              106                          sprstx     6, 21
 realft          195, 198, 201-202            stifbs     264, 276
 rf              105                           stiff     264, 274, 276
 rj              107                           stoerm    264, 273
 rk4             264-267                       svbksb    6, 15
 rkdumb          264-265, 267                  svdcmp    6, 15, 17
 rkqs            264, 266-267, 270             svdfit    247, 252-255
 r1ft3           195, 204                      svdvar     247, 254
 rofunc          247, 262                      toeplz     6, 28-29
                         Index 可Demons却ated 尸outines   3앞i

tptest   222, 226
tqli     185, 189-190
trapzd   54-55, 57
tred2    185, 188-189
tridag   6, 11
ttest    222-225
tutest   222, 225
twofft   195, 197
vander   6, 28
vegas    125, 134-137
voltra   280, 282
wtl      209, 219
wtn      209, 220
wwghts   280
zbrac    153-154
zbrak    153-154
zbrent   153, 156, 158
zrhqr    153, 162
zriddr   153, 156-157
zroots   153, 161
Following is a brief explanation of each NumericalRecipes product, plus two order fonns (one
幻rNorth Ame如anre針dents, one缸all야her), which may be used to order these沁msd汰씨y
from the publisher if you cannot obtain them from your local bookstore.

  Numerical Recipes in FORTRAN, Second Edition and Numnerical Recipes in C, Second
Edition represent the main text and reference component of the Numerical Recipes package.
Each book contains over 300 programs, in the language of the reader's choice, and constitutes
a complete subroutine library for scientific computation. Both versions contain equivalent
tutorial, mathematical, and practical discussions.
   There are two example bo炚s containing FORTRAN or C source progr缸lls respectively that
exercise and demonstrate all of the Numerical Recipes, Second Edition programs. Each
exa끄［lple program contains comments and is prefaced by a short description. Input and output
data are supplied in many cases. The example books are designed to help readers inco叩orate
procedures and subroutines and conduct simple validation tests.
   The programs contained in both the second edition main books and the example books are
available in several machine-readable fonnats that will save users hours of tedious keyboard-
ing. Diskettes for IBM PC compatible machines are available in either .너 inch high density
or 3'/2 inch format and operate on DOS 2.0 or later. Diskettes for the Apple Macintosh are 3!4
inch single-sided disks.
   Some selected first edition products are also still available:
   NumnericaiRecipes inPascalcontains the original 200Nu刃iericalRec巾es routines translated
into Pascal along with the tutorial text. The Pascal example book contains the example pro-
grams for these routines. Diskettes foreach book are available in 5% inch double-sided, double-
density IBM and 314 inch Apple Macintosh format.
   NumericalRecipes Routines andExamples inBASIC contains all the routines from the orig-
inal Numerical Recipes plus the exercise programs from the example book, all translated into
BASIC, along with the text from the example book. TheB ASIC routines and programs are also
available on 5 14 inch diskette for IBM PC compatible machines.

Instruct沁ns
To obtain the books or the latest version of the disks, please order from your bookstore or
complete the information on the order form in this book and mail it to Cambridge University
Press in Port Chester, New York or C町llbridge, England. Please note that there is a separate
order form for each location. All orders must be prepaid. Ordinary postage for shipping is paid
by the publisher.

NB: Technical question욕 corrections, and requests for information on mainframe and
workstation licenses should be directed to Numerical Recipes Software, P.O. Box 243,
Cambridge, MA 02238, U.S.A. Please do not write the publisher.

I万ere 口re no cash 爬／unds for diskette工 Only diskettes with mani｛和（?turing 叱加Is 刃a口y be
returned to the publisher for replacement.
ORDER FORM (United States and Canada)
Order from your bookstore or mail to
Cambridge University Press, Order Department, 110 Midland Avenue, Port Chester,
New York 10573
Califor current prices: 1-800-431-1580
        43064-X       Numerical Recipes in FORTRAN: The Art of Scientific Computing,
                      Second Edition
        43717-2       FORTRAN Diskette (IBM, 5% inchul.2M), second edition
        437 19-9      FORTRAN Diskette (IBM, 3!4 inch/720K), second edition
        43716-4       FORTR사나 Diskette (Macintosh), second edition
        43721-0       FORTRAN Example Book, second edition
        43 108-5      Numerical Recipes in C: The Art of Scientific Computing, Second Edition
        437 14-8      C Diskette (IBM. 5泊 inch/1.2M), second edition
        43724-5       C Diskette (IBM, 3!4 inch/720K), second edition
        43715-6       C Diskette (Macintosh), second edition
        43720-2       C Example Book, second edition
The following first edition products are still available:

        375 16-9      Numerical Recipes in Pascal: The Art of Scientific Computing
        37532-0       Pascal Diskette (IBM)
        38766-3       Pascal I거skette 小4a曲如sh)
        37675-0       Pascal Example Book
        37533-9       Pascal Example Diskette (IBM)
        38767-1       Pascal Example Diskette (Macintosh)
        40689-7       Numerical Recipes Routines and Examples in BASIC
        40688-9       BASIC Diskette (IBM)

Please indicate method of payment: check              , Mastercard          or Visa
Name

A山Iress




Card No.                                                Expiration date
Signature

       Please indicate the total number of items ordered.

       total price,

       ta兀 if applicable (NY and CA residen四)

       total enclosed
OR!死R FORM 田Ut前de North America)
Order from your bookstore or mail to
Customer Services Department. Cambridge University Press, Edinburgh Building,
Shaftesbury Road, Cambridge CB2 2RU, U.K.
       43064-X     Numencal Recipes in FORTRAN: The Art of Scientific Computing,
                   Second Edition f 35.00
       43717-2     FORTRAN Diskette (IBM, 54 inch/1.2M), second edition f 24.95
       43719-9     FORTRAN Diskette (IBM, 3'/2 inch/720K), second edition f 24.95
       437 16-4    FORTR사나 Diskette (Macintosh), second edition f 24.95
       43721-0     FORTRA나 Example Book, second edition f 19.95
       43 108-5    Numerical Recipes in C: The Art of Scientific Computing, Second Edition
                   f 35.00
       43714-8     C Diskette (IBM, 5났 inch/1.2M), second edition f 24.95
       43724-5     C Diskette (IBM, 3'/2 inchfl20K), second edition f 24.95
       437 15-6    C Diskette (Macintosh), second edition f 24.95
       43720-2     C Example Book, second edition f 19.95

The following first edition pr에ucts are still available:
        375 16-9   Numerical Recipes in Pascal: The Art of Scientific Computing f 30.00
        37532-0    Pascal Diskette (IBM) f 21.50
        38766-3    Pascal Diskette (Macintosh) f 26.50
        37675-0    Pascal Example Book f 19.50
        37533-9    Pascal Example Diskette (IBM) f 21.50
        38767-1    Pascal Example Diskette (Macintosh) f 26.50
        40689-7    Numerical Recipes Routines and Examples in BASIC f 19.50
        40688-9    BASIC Diskette (IBM) f 21.50

Name                                                                (Block capitals please)

 A山Iress




 Please accept my payment by cheque or money order in pounds sterling:
 I enclose (circle one) a Cheque (made payable to Cambridge University Press)IUK Postal
 Order/International Money Order/Bank Draft/Post Office Giro.

 Please accept my payment by credit card:
                                                                         Americ毗
 Charge my (circle one) Barclaycard/VISA/Eurocard/Access/Mastercard/Bank
 any other credit card bearing the interbank symbol (please specify).
 Card No.                                                    Expiry date:

 Signature                                                         Date:

 Ad如ess as registered by card company:




 Prices 可毗kettes do n아 加C加de V.A工，which should be 口dded to 口11 U.兀 깬rchases.
