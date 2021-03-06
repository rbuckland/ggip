
<!-- README.md is generated from README.Rmd. Please edit that file -->

# ggip

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN
status](https://www.r-pkg.org/badges/version/ggip)](https://CRAN.R-project.org/package=ggip)
[![R build
status](https://github.com/davidchall/ggip/workflows/R-CMD-check/badge.svg)](https://github.com/davidchall/ggip/actions)
[![Coverage
status](https://codecov.io/gh/davidchall/ggip/branch/master/graph/badge.svg)](https://codecov.io/gh/davidchall/ggip?branch=master)
<!-- badges: end -->

**WARNING:** This package is in very early stages of development\!

## Installation

You can install the development version from GitHub:

``` r
# install.packages("remotes")
remotes::install_github("davidchall/ggip")
```

## Quick start

`coord_ip()` forms the basis of any ggip plot. It determines which
region of address space is displayed and also the resolution of the
pixels in terms of network sizes. It also translates `ip_address()` and
`ip_network()` vectors into Cartesian coordinates that can be used by
ggplot2 layers.

With ggip, it is easy to quickly produce visualizations like this:

<img src="man/figures/ipv4-heatmap.png" alt="IPv4 heatmap" width="100%" />
