# mgof
Stata module to perform goodness-of-fit tests for multinomial data

`mgof` computes goodness-of-fit tests for the distribution of a discrete
(categorical, multinomial) variable. The default is to perform classical large
sample chi-squared approximation tests based on Pearson's X2 statistic and the
log likelihood ratio (G2) statistic or a statistic from the Cressie-Read
family. Alternatively, `mgof` computes exact tests using Monte Carlo methods or
exhaustive enumeration. A Kolmogorov-Smirnov test for discrete data is also
provided.

To install `mgof` from the SSC Archive, type

    . ssc install mgof, replace

in Stata. Stata version 9.2 or newer is required. Furthermore, the `moremata`
package is required. To install `moremata` from the SSC Archive, type

    . ssc install moremata, replace

---

Installation from GitHub:

    . net install mgof, replace from(https://raw.githubusercontent.com/benjann/mgof/main/)
    . net install moremata, replace from(https://raw.githubusercontent.com/benjann/moremata/master/)


---

Main changes:

    07jul2008 (version 1.0.5)
    - -nolabel- added to -proportion- call

    14jan2008 (version 1.0.4)
    - svy support added (Rao&Scott correction): -svy[()]- option
    - pweights now allowed (-approx- method only) (Rao&Scott correction)
    - -expected()- option
    - does no longer break if input variable has noninteger values
    - matrix() => error if varname, if, in, or weights specified

    28jun2007 (version 1.0.0)
    - published on SSC

