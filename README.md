R package `gdor` (formerly on CRAN, now archived, hopefully soon to be
on CRAN again)

GDOR stands for "generalized direction of recession", a term introduced by

>  Geyer, Charles J. (2009).  
>  Likelihood inference in exponential families and directions of recession.  
>  *Electronic Journal of Statistics*, 3, 259-289.  
>  http://projecteuclid.org/euclid.ejs/1239716414

which also covers some of the methodology used in this R package.
The rest is covered in

> Eck, Daniel J., and Geyer, Charles J. (submitted).  
> Computationally efficient likelihood inference
>     in exponential families when the maximum likelihood estimator
>     does not exist.  
> https://arxiv.org/abs/1803.11240

This package is generalized linear models that are exponential families
(logistic regression and Poisson regression) done right in the sense that
it does the right thing in all cases, not just when the MLE exists in the
conventional sense.  When the MLE does not exist in the conventional sense,
it does exist in the Barndorff-Nielsen completion of the model, which the
package finds.

Tests of model comparison are implemented (by the `gdor` method of the
R generic function `anova`).

Confidence intervals are not yet implemented but soon will be (by the `gdor`
method of the R generic function `confint`).

Log-linear models for categorical data analysis are handled by treating
them as Poisson regression (using the well know fact that Poisson sampling,
multinomial sampling, and product multinomial sampling have the same
MLE and the same asymptotic distributions of the likelihood ratio test).
