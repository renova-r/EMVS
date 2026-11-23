# EMVS 1.2.2

- Updated the build configuration and C++ code for compatibility with current R and compilers.
- Compatibility fixes contributed by [Renova](https://github.com/renova-r) (Jing Jia, Guanyang Wang, and Peng Zhang).

# EMVS 1.2.1 (2021-10-12)

- Fixed: PI to M_PI in preparation for Rcpp change.

# EMVS 1.2 (2021-02-15)

- Fixed: errors in vignette build


# EMVS 1.1 (2019-12-13)

- Fixed: EMVS now uses `if(obj, "matrix")` instead of `class(obj) == "matrix"` in preparation for changes in R 4.0.0
