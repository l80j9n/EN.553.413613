java c
Applied   Stats   and   Data   Analysis
EN.553.413-613
Practice   Midterm   2
Question   1.   Consider   the   linear   model
Y   = Xβ +   ε   ,where Y is an-by-1 vector of   response variables, X is ann-by-p design matrix,   β   is   a   p-by-1   vector   of   coefficients,   ε   is   a   multivariate   normal   Nn   (0,σ2In   ).   Denote   by   b   the   least-squares   estimate   of β   .
(a)   Write   down   the   formula   for   the   least-squares   estimate   for   the   regression   vector   b   in   terms   of matrices   X,   Y.   You   don’t   need   to   derive   it.
(b)   What   is the   distribution   of b?    Specify the   corresponding   mean   and vari-   ance   covariance   matrix.   You   don’t   need   to   derive   it.
(c)   Write   down   normal   equations   in   the   matrix   form.   You   don’t   need   to   de-   rive   them.
(d)   Write   SSE   ,    SSR,    SSTo   in   the   matrix   form,    using   matrices   Y   ,   H,   J.   Specify   degrees   of   freedom   for   each   sum   of   squares.    You    don’t   need   to   derive   anything   here.
(e)   What   are   the   conditions   on   matrix   X   such   that   XTX   is   invertible?   You don’t   need   to   prove   anything   here.(f)   Compute   the   covariance   matrix   Cov(b,   Y(ˆ)).      Show   your   steps   and   sim-plify.   Your   answer   should   be   expressed   in terms   of X   and   σ   2    only.    What are   the   dimensions   of the   matrix   Cov(b,   Y(ˆ))?Question   2.   Consider   the   following   plots   of   data   points   in   the   XY   plane,   where   X    is   the   predictor   variable   and   Y   is   the   response   variable.       Points   in   the   parallelogram   (slanted   box)   represent   evenly   distributed   data   points.   The   ‘o’   represent   unusual   observations.
(i)   For each of the plots   (A),   (B),   (C) and   (D) describe whether the unusual   observation/s is   an   ‘outlier   with   respect   to   X   ’, or   an   ‘outlier   with   respect   to   Y   ’,   or   an   ‘outlier   with   respect   to   X   and   Y   ’,   or   none   of   the   above.
(ii)   Internally   studentized   residuals   (ISR),   externally   studentized   residuals   (ESR),   and   leverage   are   common   diagnostic   tools   to   idenify   unusual   observations.   Which of   the three tools are more likely to identify unusual   observation   in   each   of   the   four   cases   (A),   (B),   (C)   and   (D).   List   best   two   diagnostic   tools   for   each   case.
Question   3.   Suppose   Yi      follows   the   model
Yi   = β1Xi1   +   β2Xi2   +   εiwhere   εi    is   independent,   identically   distributed   and   normal   with   mean   zero   and variance   σ   2   .   There is   NO   INTERCEPT TERM.   The   graph   below   shows   the individual 95% CI for β1      (horizontal   axis)   and   the   95%   CI   for   β2      (vertical   axis),   and   the   95%   confidence   region   for   the   overall   model   fit   F-test    (the   ellipse).    Locations   A,   B   and   C   are   possible   locations   where   the   origin   (0,   0)   could   be   located.   

(a)   For   each   of the   points   A,   B,   C   state   whether
●   β1    is   significant   OR   nonsignificant,
●   β2    is   significant   OR   nonsignificant,
●   overall   model   fit   is   significant   OR   nonsignificant.
You   need   to   write   three   statements   for   each   point   A,   B   and   C!
(b)   What   should   be   the   conditions   on   predictors   X1    and   X2    such   that   case   B   is   much   more   common   than   case   A.   Briefly   explain.

Question   4.   Suppose   we   wish   to   understand   how   blood   pressure,   Y   ,   in   a   certain   population   depends   on   the   patient   age   and   patient   asthma   status   (asthmatic   or   nonasthmatic).      Let   X1      be   a   patient’s   age   in   years,   and   X2   the   asthma   status.   Note   that   X2    is   a   qualitative   variable,   and   X2    is   1   if the   patient   is   asthmatic   and X2    is   0 if the patient   is   nonasthmatic.    Consider the   second-order interaction   model
Y = β0   +   β1X1   +   β2X2   +   β3X1(2)   +   β4X1X2   +   β5X1(2)X2   +   ε
where,   again,   ε   is   a   normally   distributed   random   variable   with   mean   0   and   constant   variance   σ   2   .
(a)   Compute   the   blood   pressure   for   non-asthmatics   in   terms   of   X1   ,   the   age   in   years,   and   some   or   all   of   the   coefficients   β0   ,β1   ,β2   ,β3   ,β4      and   β5   .   Your   answer   to   this   part   should   NOT   have   any   numbers   in   it–it   should   be   entirely   in   terms   of X1    and   the   coefficients   βi.(b)   Suppose   we   are   given   the   following   regression   output   (note:    x1       :   x2      de-
no代 写EN.553.413-613 Applied Stats and Data Analysis Practice Midterm 2
代做程序编程语言tes   the   product   term   X1X2   ;   similarly   (x1   )2    : x2      stands   for   X1(2)X2   ):
Coefficients:


                                Estimate Std. Error t value Pr(>|t|)
(Intercept) 4.5094 42.2371 0.107 0.9155
x_1 6.3940 5.7774 1.107 0.2752
x_2 -50.8539 56.2080 -0.905 0.3712
x_1^2 0.1318 0.1687 0.781 0.4394
x_1:x_2 17.0645 7.1011 2.403 0.0211
(x_1)^2:x_2 -0.5025 0.1992 -2.522 0.0158
---

Residual      standard      error:      71   . 69    on      39    degrees      of      freedom Multiple   R-squared:          0   .7682,Adjusted      R-squared:            0   .7385   F-statistic:      25.85      on      5      and      39   DF,         p-value:      0   . 0000
How   many   data   points   there?    How   many   parameters   are   in   the   model?   I.e.,   find   n   and p.


(c)   Based   on this   output,   state   hypotheses   and   conduct   a   level   α   = 0.05 test   of whether or not the interaction   term   between   asthma   and   the   square   of   age   is   associated   with   the   response.   Find   the   t*    and   the   p-value.    Deter-   mine   your   conclusion   based   on   this   data.
(d)   Based   on   this   output,   find   the   interval   where   the   blood   pressure   in   a   35-   year-old   asthmatic   would   be   with   95%   probability.
(e)   Based on the R output, can you conclude that the only appropriate model   for   the   data   is
Y = β4X1X2   +   β5X1(2)X2   +   ε   ?
Explain   why   yes,   or   why   no.
(f)   Do   you   think   there   is   evidence   of   multicollinearity   in   the   provided   out-   put?   Briefly   explain   why   yes   or   why   no.

Question   5.   Consider the following data seton the calories   (Ci   )   and   sodium   level   (Si   )   of   several   types   (Ti   )   of   sausages.    The   categorical    (or   qualitative)   variable   type    (Ti   )   can   take   on   three   values:       “chicken”,    “beef”    or    “pork”   .   First   six   rows   of the   dataset   is   as   follows.   There   are   n   observations   in   total.
type,   Ti
calories   Ci
sodium   Si
pork
172
496
chicken
87
359
chicken
143
581
chicken
132
375
pork
190
545
pork
173
458
Consider   the   following   regression   output.
g1      <-    lm(calories      ~    sodium,    sausage)
g2      <-      lm(calories    ~      sodium      +      factor(type),      sausage)
#factor(type)      is   the   way   R   treats      qualitative    (or      categorical)   variables
summary(g1)$r   . squared
##      [1]    0   . 218
summary(g2)$r   . squared   ##      [1]    0   .793   




Model   g1   is   obtained   by   fitting   the   linear   model
g1:                     Ci   = β0   + β1   Si   +   εi
to   the   data.
Model   g2   is   obtained   by   fitting   the   linear   model
g2:                     Ci   = β0   + β1   Si   + β2Xi2   +   β3Xi3   +   εi
to   the   data.
From   the   above   output,   answer   the   following   questions.
(a)   Explicitly   define   Xi2    and   Xi3   .   Hint:   dummy   coding.
(b)   Write   down the first   six rows of   the   two   design   matrices   X   for   models   g1   and   g2   based   on   the   provided   data   table.
(c)   The   above   plot   displays   the   calories   count   against   the   sodium   predictor variable   for   the   model   g1.    The   square,   triangle,   and   circle   points   corre-   spond   to   sausages   of   type    “chicken”,    “beef”,    and    “pork”,    respectively.   Explain   why   based   only   on   this   plot   we   can   suggest   that   model   g2   should   be   preferred   over   model   g1?
(d)   Explain   why   this   plot   also   suggests   that   the   following   model
Ci   = β0   +   β1   Si   +   β2Xi2   +   β3Xi3   +   β4Xi2Si   +   β5Xi3Si   +   εi
is   unnecessarily   complicated   for   this   dataset.
(e)   Consider   model   g2.    Assuming   independent   normal   errors   and   constant   variances,   write   down   the   null   and   alternative   hypotheses   that   the   type   of sausage   is   not   associated   with   calories,   in the   presence   of other vari-   ables   in   the   model   g2.


(f)   Continuing   part   (e).   Write   down   the   exact   form   of the   test   statistic   and   specify   the   distribution   of this   test   statistic   under   the   null   hypothesis   of   no   association   between   type   of   sausage   and   calories   (in   the   presence   of   other   variables).    Note   that   the   test   statistic   can   be   computed   from   the   quantities   given   above.    Your   final   answer   will   depend   only   on   n.    Hint:   General   Linear   Test   and   R2    =   1 − SSE/SSTO.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
