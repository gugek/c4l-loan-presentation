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
## 
## 
##            Collection Desc             count 
## ------------------------------------- -------
##                Stacks                  48839 
##               Reserves                 23334 
##      Periodicals, Current Issues       4590  
##             General (III)              1774  
##          Christie Collection           1695  
##            Course Reserves             1496  
##        Library Service Center          1237  
##            Cox Collection               699  
##          Faculty Collection             634  
##         Empirical Collection            606  
##              Periodicals                462  
##               Documents                 406  
##            NC Alcove (III)              398  
##      Superseded Looseleaf (III)         328  
##   Law School Academic Technologies      319  
##     Regional Reporters (Level 1)        297  
##               Reference                 238  
##         Superseded Reference            207  
##            Alumni Authors               165  
##         Leisure Reading (III)           132  
##            Leisure Reading              122  
##               NC Alcove                 116  
##        Professional Collection          106  
## Federal Reporters & Digests (Level 3)   75   
##            Documents (III)              59   
##        Unclassified Collection          58   
##               Archives                  53   
##           Superseded Codes              51   
##            Tax Collection               35   
##              Rare Books                 22   
##            Superseded Tax               22   
##          Rare Books, Level 1            19   
##      Federal Reporters & Digests        18   
##           Records & Briefs              17   
##         Practice & Procedure            16   
##          Regional Reporters             16   
##              State Codes                16   
##                 Media                   15   
##         Superseded Looseleaf            15   
##             S.J.D. Theses               13   
##         Tax Collection (III)            12   
##            Federal Alcove               11   
##     Professional Collection (III)       11   
##               Oversize                   8   
##         Federal Alcove (III)             6   
##         Rare Books, Oversize             4   
##                Thesis                    4   
##     Rare Books, Level 1 Oversize         1   
##                Riddick                   1   
##          Riddick Senatorial              1   
##         State Codes (Level 3)            1   
##             UnKnown-LAW,-                1
```

