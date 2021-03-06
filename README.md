
<!-- README.md is generated from README.Rmd. Please edit that file -->

# `{covid19ita}` <img src='man/figures/logo.png' align="right" height="120" />

<!-- badges: start -->

[![Lifecycle:
maturing](https://img.shields.io/badge/lifecycle-maturing-blue.svg)](https://www.tidyverse.org/lifecycle/#maturing)
[![CRAN
status](https://www.r-pkg.org/badges/version/covid19ita)](https://CRAN.R-project.org/package=covid19ita)
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/UBESP-DCTV/covid19ita?branch=master&svg=true)](https://ci.appveyor.com/project/CorradoLanera/covid19ita)
[![Travis Build
Status](https://travis-ci.com/UBESP-DCTV/covid19ita.svg?branch=master)](https://travis-ci.com/UBESP-DCTV/covid19ita)
[![Codecov test
coverage](https://codecov.io/gh/UBESP-DCTV/covid19ita/branch/master/graph/badge.svg)](https://codecov.io/gh/UBESP-DCTV/covid19ita?branch=master)
<!-- badges: end -->

The goal of `{covid19ita}` is to provide a platform for the monitoring
of COVID-19 infection diffusion in Italy.

## Installation

You can install the development version of `{covid19ita}` from
[GitHub](https://github.com/) with:

``` r
# install.packages("remotes")
remotes::install_github("UBESP-DCTV/covid19ita")
```

## Shiny App

<img src='inst/app/www/covid19ita_screen.png' align="center"/>

**Last app update**: 2020-03-12 14:19:54.

You can visit the `covid19ita` Shiny App running on the UBEP servers
[here](https://r-ubesp.dctv.unipd.it/shiny/covid19ita/).

You can also run a local version of the app from your computer with:

``` r
library(covid19ita)
run_app()
```

## Data

The package provide R versions of the three [official Italian COVID-19
datasets](https://github.com/pcm-dpc/COVID-19/) at national, regional
and provincial level of detail.

**Last data update**: 2020-03-12 13:04:54.

Access the data with:

``` r
library(covid19ita)
data(dpc_covid19_ita_andamento_nazionale) # national level data
data(dpc_covid19_ita_regioni)             # regional level data
data(dpc_covid19_ita_andamento_province)  # provincial level data
```

You can access to the data documentation with any of:

``` r
?dpc_covid19_ita_andamento_nazionale
?dpc_covid19_ita_regioni
?dpc_covid19_ita_province

?dpc_covid19_ita
```

## Data attribution

**License**:
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.en) -
[Visualizza
licenza](https://github.com/pcm-dpc/COVID-19/blob/master/LICENSE)

**Dataset author/editor**: [Dipartimento della Protezione
Civile](http://www.protezionecivile.it/)

**Data provided by**: [Ministero della
Salute](http://www.salute.gov.it/)

**Original data processing and management by**: [Dipartimento della
Protezione Civile](http://www.protezionecivile.it/)

## Code of Conduct

Please note that the ‘covid19ita’ project is released with a
[Contributor Code of Conduct](CODE_OF_CONDUCT.md). By contributing to
this project, you agree to abide by its terms.
