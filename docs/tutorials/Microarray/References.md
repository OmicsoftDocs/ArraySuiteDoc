# References

## MAS5

Hubbell, E. et al. (2002) Robust estimation for expression analysis. Bioinformatics, 18, 1585-1592
[^link^](http://www.affymetrix.com/support/technical/whitepapers/sadd_whitepaper.pdf )

## RMA

Irizarry, R. A. et al., (2003) Exploration, normalization, and summaries of high density oligonucleotide array probe level data. Biostatistics, 4, 249-264
[^link^](http://www.biostat.jhsph.edu/~ririzarr/papers/affy1.pdf )

## GCRMA

A Model-Based Background Adjustment for Oligonucleotide Expression Arrays

Zhijin Wu , Rafael A. Irizarry , Robert Gentleman , Francisco Martinez-Murillo , Forrest Spencer

Journal of the American Statistical Association, 2004 vol 99 page 909
[^link^](http://biostats.bepress.com/cgi/viewcontent.cgi?article=1001&context=jhubiostat )

## GCRMA 2

GCRMA2 is newer implementation of GCRMA which fixes a bug in original GCRMA implementation that introduces artifacts that can lead to the overestimation of pair wise correlation
[^link^](http://www.bioconductor.org/packages/2.12/bioc/vignettes/gcrma/inst/doc/gcrma2.0.pdf )

## Moderated t-test (Limma Package in R)

The moderated t-test is used to rank genes in order of evidence for differential expression. They use an empirical Bayes method to shrink the probe-wise sample variances towards a common value and to augment the degrees of freedom for the individual variances (Smyth, 2004).
The empirical Bayes moderated t-statistics test each individual contrast equal to zero. For each probe (row), the moderated F-statistic tests whether all the contrasts are zero. The F-statistic is an overall test computed from the set of t-statistics for that probe. This is exactly analogous to the relationship between t-tests and F-statistics in conventional anova, except that the residual mean squares and residual degrees of freedom have been moderated between probes.
[^link^](http://rss.acs.unt.edu/Rdoc/library/limma/html/ebayes.html )
