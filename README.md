
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rrr.workshop

<!-- badges: start -->

[![R-CMD-check](https://github.com/emptyfield-ds/rrr.workshop/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/emptyfield-ds/rrr.workshop/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of rrr.workshop is to download learning materials for
Reproducible Research in R, as well as to install any required packages.
rrr.workshop also allows you to open a given module in Posit Cloud.

## Installation

You can install the latest version of rrr.workshop with:

``` r
options(repos = c(
  emptyfieldds = "https://emptyfield-ds.r-universe.dev",
  CRAN = "https://cran.rstudio.com/"
))

install.packages("rrr.workshop")
```

## Installing modules

`use_module()` will install the materials for a given module on your
computer. Then, it will open a new RStudio Project containing the files
you’ll need.

``` r
rrr.workshop::use_module("module_name")
```

By default, this package downloads the materials to a conspicuous place
like your Desktop. You can also tell `use_module()` exactly where to put
the materials with `destdir`:

``` r
rrr.workshop::use_module("module_name", destdir = "a/path/on/your/computer")
```

## Opening modules in Posit Cloud

`browse_cloud()` opens a module in Posit Cloud, where the materials and
all necessary tooling will be pre-installed. This requires an Posit
Cloud account.

``` r
rrr.workshop::browse_cloud("module_name")
```
