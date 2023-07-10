
# test.testthat

<!-- badges: start -->
<!-- badges: end -->

Test https://github.com/rstudio/rstudio/issues/11969

To test inside the Windows Sandbox or a fresh Windows Image: Install Git, R, RTools and latest RStudio daily

E.g. with `winget` available:

```
winget install git.git
winget install Rproject.R
winget install Rproject.Rtools
```

Install latest RStudio daily from https://dailies.rstudio.com

clone this repo from within RStudio > File > New Project

Install necessary packages

```r
install.packages("pak")
pak::pak("r-lib/cli")
pak::pak("r-lib/testthat")
pak::pak("devtools")
pak::pak("reprex")
```

Open `tests/testthat/test-testhat.R` in RStudio and click the "Run Tests" button.
