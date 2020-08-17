---
output: github_document
---

<!-- README.md is generated from README.Rmd. Please edit that file -->



# ggip

<!-- badges: start -->
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![CRAN status](https://www.r-pkg.org/badges/version/ggip)](https://CRAN.R-project.org/package=ggip)
[![R build status](https://github.com/davidchall/ggip/workflows/R-CMD-check/badge.svg)](https://github.com/davidchall/ggip/actions)
[![Coverage status](https://codecov.io/gh/davidchall/ggip/branch/master/graph/badge.svg)](https://codecov.io/gh/davidchall/ggip?branch=master)
<!-- badges: end -->

**WARNING:** This package is in very early stages of development!

## Installation

You can install the development version from GitHub:

``` r
# install.packages("remotes")
remotes::install_github("davidchall/ggip")
```

Example usage:
```r
ip_data %>%
  ggplot() +
  stat_ip_heatmap(aes(ip = ip)) +
  scale_fill_viridis_c(trans = "log2", na.value = "black") +
  coord_ip(pixel_prefix = 20) +
  theme_ip_dark()
#> Warning: Transformation introduced infinite values in discrete y-axis
```

<img src="man/figures/README-ipv4_heatmap-1.png" title="plot of chunk ipv4_heatmap" alt="plot of chunk ipv4_heatmap" width="100%" />
