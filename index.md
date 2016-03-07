---
title       : Loan Presentation
subtitle    : 
author      : Sean Chen
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Initialization

Data

```r
loans_tbl <- tbl_df(read_tsv("Loans.csv"))
```

```
## Warning: 643 parsing failures.
##  row     col   expected actual
## 1362 Copy ID an integer    c.1
## 1364 Copy ID an integer    c.1
## 1365 Copy ID an integer    c.1
## 1366 Copy ID an integer    c.1
## 1367 Copy ID an integer    c.1
## .... ....... .......... ......
## .See problems(...) for more details.
```

--- .class #id 

## How many rows?

```r
nrow(loans_tbl)
```

```
## [1] 88781
```

--- .class #id

## How many loans?

```
## Source: local data frame [52 x 2]
## 
##                Collection Desc count
##                          (chr) (int)
## 1                       Stacks 48839
## 2                     Reserves 23334
## 3  Periodicals, Current Issues  4590
## 4                General (III)  1774
## 5          Christie Collection  1695
## 6              Course Reserves  1496
## 7       Library Service Center  1237
## 8               Cox Collection   699
## 9           Faculty Collection   634
## 10        Empirical Collection   606
## ..                         ...   ...
```

