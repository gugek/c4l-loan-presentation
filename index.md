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



