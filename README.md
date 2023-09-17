
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

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

![](README_files/figure-gfm/pressure-1.png)<!-- -->

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
