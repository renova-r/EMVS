# EMVS

An expectation-maximization algorithm for fitting Bayesian spike-and-slab regularization paths for linear regression.

Compatibility updates by Renova.

Version 1.2.1.9001: the C++ build no longer calls `Rcpp:::LdFlags()` from `src/Makevars` and `src/Makevars.win` (Rcpp needs no extra link flags), `src/functions.cpp` uses `std::isfinite()` in place of the unqualified `is_finite()`, and the author records are normalized so that `Author`, `Authors@R` and `Maintainer` agree (both authors retained; Gemma Moran as sole maintainer).

## Install

```r
install.packages("EMVS", repos = c(
  Renova = "https://renova-r.r-universe.dev",
  CRAN = "https://cloud.r-project.org"
))
```

See the [R-universe package page](https://renova-r.r-universe.dev/EMVS) for builds and installation. This release is tagged on GitHub as `renova-1.2.1.9001`:

```r
remotes::install_github("renova-r/EMVS@renova-1.2.1.9001")
```

[Release notes](NEWS.md) · [Renova package directory](https://github.com/renova-r/revival-catalog)

EMVS is by Veronika Rockova and Gemma Moran (maintainer); the original CRAN package is at <https://CRAN.R-project.org/package=EMVS>. License: GPL-3; see [COPYING](COPYING).
