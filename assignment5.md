Assignment5
================

## Instructions: Please read through this before you begin

## Load packages

To start, load all the required packages with the following code.
Install them if they are not installed yet.

``` r
library(tidyverse)
library(knitr)
```

<p>
 
</p>

## Exercise 1. Tibble and Data Import

Import the data frames listed below into R and parse the columns
appropriately when needed. Watch out for the formatting oddities of each
dataset. Print the results directly, without using kable().

You only need to finish any three out of the five questions in this
exercise in order to get credit.
<p>
 
</p>

##### 1.1 Create the following tibble manually, first using tribble() and then using tibble(). Print both results. \[We didn’t have time to cover this in class, but look up how these functions work here\]

``` r
tribble(
  ~a, ~b, ~c,
  #--|--|----
  1, 2.1, "apple",
  2, 3.2, "orange"
)
```

    ## # A tibble: 2 × 3
    ##       a     b c     
    ##   <dbl> <dbl> <chr> 
    ## 1     1   2.1 apple 
    ## 2     2   3.2 orange

``` r
tribble(
  ~a, ~b, ~c,
  #--|--|----
  integer(1), 2.1, "apple",
  integer(2), 3.2, "orange"
)
```

    ## # A tibble: 2 × 3
    ##   a             b c     
    ##   <list>    <dbl> <chr> 
    ## 1 <int [1]>   2.1 apple 
    ## 2 <int [2]>   3.2 orange
