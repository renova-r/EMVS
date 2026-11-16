# EMVS 1.2.1.9001

Renova release, based on CRAN EMVS 1.2.1 (archived on CRAN 2022-12-05).

- `src/Makevars`, `src/Makevars.win`: `PKG_LIBS` no longer runs `Rcpp:::LdFlags()`; it keeps `$(LAPACK_LIBS) $(BLAS_LIBS) $(FLIBS)` (build configuration).
- `src/functions.cpp`: one finiteness test uses `std::isfinite(res)` instead of `is_finite(res)` (C++; same test).
- `DESCRIPTION`: author records normalized - `Authors@R` added and `Author` rewritten to list Veronika Rockova (aut) and Gemma Moran (aut, cre), matching the existing `Maintainer`; the original `Author` field listed Veronika Rockova as `aut,cre`, so the roles are not identical to that field (metadata only).
- `DESCRIPTION`: stale optional `Date` field removed (metadata only).

Release preparation:

- `DESCRIPTION`: `Version` set to `1.2.1.9001`; "Compatibility updates by Renova." appended to `Description`.
- The stale `MD5` file was removed.
- `COPYING` (GNU GPL version 3 text) was added; the `License` field is unchanged.
- `README.md` was added and is excluded from the R build.
- This entry was added above the existing `NEWS.md` content.

# EMVS 1.2.1 (2021-10-12)

- Fixed: PI to M_PI in preparation for Rcpp change.

# EMVS 1.2 (2021-02-15)

- Fixed: errors in vignette build


# EMVS 1.1 (2019-12-13)

- Fixed: EMVS now uses `if(obj, "matrix")` instead of `class(obj) == "matrix"` in preparation for changes in R 4.0.0
