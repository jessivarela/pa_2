Pa\_2
================

Programming Assignment 2
========================

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────── tidyverse 1.2.1 ──

    ## ✔ ggplot2 3.1.1       ✔ purrr   0.3.3  
    ## ✔ tibble  2.1.1       ✔ dplyr   0.8.0.1
    ## ✔ tidyr   0.8.3       ✔ stringr 1.4.0  
    ## ✔ readr   1.3.1       ✔ forcats 0.4.0

    ## ── Conflicts ────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

``` r
data <- read_csv("data/data.csv")
```

    ## Parsed with column specification:
    ## cols(
    ##   info = col_character(),
    ##   durationV = col_double(),
    ##   f0 = col_double(),
    ##   int = col_double()
    ## )

``` r
print(data)
```

    ## # A tibble: 10 x 4
    ##    info    durationV    f0   int
    ##    <chr>       <dbl> <dbl> <dbl>
    ##  1 capo_1       0.15  196.  78.5
    ##  2 capo_2       0.16  173.  78.1
    ##  3 pinto_1      0.13  239.  68.3
    ##  4 pinto_2      0.1   199.  73.4
    ##  5 pujo_1       0.13  241.  79.4
    ##  6 pujo_2       0.13  202.  80.2
    ##  7 quemo_1      0.14  198.  76.4
    ##  8 quemo_2      0.13  189.  75.5
    ##  9 testo_1      0.13  220.  76.1
    ## 10 testo_2      0.12  180.  75.2

``` r
f0_1 <- c(196,239,241,198,220)

mean(f0_1)
```

    ## [1] 218.8

``` r
f0_2 <- c(173, 199, 202, 189, 180)

mean(f0_2)
```

    ## [1] 188.6

``` r
durationV_1 <- c(.15, .13, .13, .13, .13)

mean(durationV_1)
```

    ## [1] 0.134

``` r
durationV_2 <- c(.16, .1, .13, .13, .12)

mean(durationV_2)
```

    ## [1] 0.128

``` r
int_1 <-c(78.5, 68.3, 79.4, 76.4, 76.1)

mean(int_1)
```

    ## [1] 75.74

``` r
int_2 <- c(78.1, 73.4, 80.2, 75.5, 75.2)

mean(int_2)
```

    ## [1] 76.48
