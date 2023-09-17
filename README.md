
<!-- README.md is generated from README.Rmd. Please edit that file -->

This is a package that counts and tells you the sizes of libraries in
your RStudio. \# libminer

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer is to …

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("melimore86/libminer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer)
## basic example code

lib_summary()
```

    ##                                                                                        Library
    ## 1                         /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
    ## 2 /private/var/folders/j9/85xxvzw144d_4vbn_cp0rrm40000gn/T/RtmplNsS5Q/temp_libpathb02a46a3c2ae
    ##   n_packages
    ## 1        232
    ## 2          1

``` r
lib_summary(sizes = TRUE)
```

    ##                                                                                        Library
    ## 1                         /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
    ## 2 /private/var/folders/j9/85xxvzw144d_4vbn_cp0rrm40000gn/T/RtmplNsS5Q/temp_libpathb02a46a3c2ae
    ##   n_packages   lib_size
    ## 1        232 1126636916
    ## 2          1      14195

