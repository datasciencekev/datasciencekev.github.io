---
title       : Developing Data Products
subtitle    : 
author      : kts
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Basics

* The goal is to build a shiny app and slidify documentation
* Both need to be publicly published
* shinyapps.io and ph-pages, here we come!

--- 

## The Application

We chose to keep things simple - use the mtcars data set, predict MPG based on weight, and interact with the user via a text box.


```r
data(mtcars)
model <- lm(mpg~wt, data = mtcars)
print (model)
```

```
## 
## Call:
## lm(formula = mpg ~ wt, data = mtcars)
## 
## Coefficients:
## (Intercept)           wt  
##      37.285       -5.344
```
