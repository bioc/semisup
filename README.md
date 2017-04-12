
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![Travis-CI Build Status](https://travis-ci.org/rauschenberger/semisup.svg?branch=master)](https://travis-ci.org/rauschenberger/semisup) [![Coverage Status](https://codecov.io/github/rauschenberger/semisup/coverage.svg?branch=master)](https://codecov.io/github/rauschenberger/semisup?branch=master) <!-- [![Platforms](http://www.bioconductor.org/shields/availability/release/semisup.svg)](http://bioconductor.org/packages/devel/bioc/html/semisup.html#archives)
 [![Downloads](http://www.bioconductor.org/shields/downloads/semisup.svg)](http://bioconductor.org/packages/stats/bioc/semisup/)
[![Posts](http://www.bioconductor.org/shields/posts/semisup.svg)](https://support.bioconductor.org/t/semisup/)
[![in Bioc](http://www.bioconductor.org/shields/years-in-bioc/semisup.svg)](http://bioconductor.org/packages/devel/bioc/html/semisup.html#since)
[![Build](http://www.bioconductor.org/shields/build/devel/bioc/semisup.svg)](http://bioconductor.org/checkResults/devel/bioc-LATEST/semisup/)
[![Commits](http://www.bioconductor.org/shields/commits/bioc/semisup.svg)](http://bioconductor.org/packages/devel/bioc/html/semisup.html#svn_source)
[![Coverage Status](http://www.bioconductor.org/shields/coverage/devel/semisup.svg)](https://codecov.io/github/Bioconductor-mirror/semisup/branch/master) -->

Scope
-----

When testing for association between a quantitative trait and single nucleotide polymorphisms (SNPs), researchers often detect significant SNPs, but seldom detect significant SNP-SNP interactions. This is partly due to the massive amount of SNP-SNP combinations. We propose to move away from testing interaction terms, and move towards testing whether an individual SNP is involved in any interaction. This reduces the multiple testing burden to one test per SNP, and allows for interactions with unobserved factors. Analysing one SNP at a time, we split the individuals into two groups, based on the number of minor alleles. If the quantitative trait differs in mean between the two groups, the SNP has a main effect. If the quantitative trait differs in distribution between some individuals in one group and all other individuals, it possibly has an interaction effect. We propose a test to detect both types of effects. Implicitly, the posterior probabilities may suggest potential interacting variables. Analysing simulated and experimental data, we show that the proposed test is statistically powerful, maintains the type I error rate, and detects meaningful signals.

Installation
------------

The package semisup depends on [R &gt;= 3.4.0](https://cran.r-project.org/), and is available from [Bioconductor](http://bioconductor.org/packages/semisup/):

``` r
source("https://bioconductor.org/biocLite.R")
BiocInstaller::biocLite("semisup")
```

Alternatively, it can be installed from [GitHub](https://github.com/rauschenberger/semisup). This requires the package [devtools](https://cran.r-project.org/web/packages/devtools/README.html):

``` r
devtools::install_github("rauschenberger/semisup",build_vignettes=TRUE)
devtools::install_github("Bioconductor-mirror/semisup",build_vignettes=TRUE)
```

Please restart R before loading the package and its documentation:

``` r
library(semisup)
utils::help(semisup)
utils::vignette("semisup")
```

Reference
---------

A Rauschenberger, RX Menezes, MA van de Wiel, NM van Schoor, and MA Jonker (2017). Detecting SNPs with interactive effects on a quantitative trait. Manuscript in preparation. <!-- [html](http://dx.doi.org/) [pdf](http://) -->
