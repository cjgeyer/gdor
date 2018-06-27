R package `gdor` (formerly on CRAN, now archived, hopefully soon to be
on CRAN again)

GDOR stands for "generalized direction of recession", a term introduced by

>  Geyer, Charles J. (2009).
>  Likelihood inference in exponential families and directions of recession.
>  *Electronic Journal of Statistics*, 3, 259-289.
>  http://projecteuclid.org/euclid.ejs/1239716414

which also covers the methodology used in this R package.

This package is "generalized linear models done right" in the sense that
it does the right thing in all cases, not just when the MLE exists in the
conventional sense.  When the MLE does not exist in the conventional sense,
it does exist in the Barndorff-Nielsen completion of the model, which the
package finds.

Tests of model comparison are implemented (by anova.gdor).

Confidence intervals are not yet implemented (no predict.gdor yet).
