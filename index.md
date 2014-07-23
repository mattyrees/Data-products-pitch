---
title       : Temperature converter
subtitle    : Farenheit to Celsius and all the way back again!
author      : Matthew Rees
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Tool Description

This tool is able to convert temperature to either Celsius or Farenheit. 

The calculation is performed using a the established conversion formula for temperature in degrees. 

User enters the parameters via numeric box 

The tool is hosted at the link listed below:
https://mattyreesy.shinyapps.io/Developing-data-product-course-project/

--- .class #id 

## Tool Layout


The tool has an input panel


The tool has a single output tab with 4 components 
 - The entered temperature in Farenheit
 - The entered temperature in Celsius
 - The temperature converted to Celsius
 - The temperature converted to Farenheit
 

By default, the tool hides ui.R and server.R code from user view. 

--- .class #id 

## Farenheit-Celsius Calculation


This is the exact model used in the application




```r
Farenheit = (Celsius * (9/5)) + 32


Celsius = (Farenheit - 32) * (5/9)
```

i.e. What is the temperature in Farenheit when the temperature in Celsius is 29 degrees. 

```r
Celsius<-29
Farenheit = (Celsius * (9/5)) + 32
Farenheit
```

```
## [1] 84.2
```

--- .class #id 

## Tool interactive console

Temperature Farenheit: range(-500, 500), default = 0, step = 1

Temperature Celsius: range(-500, 500), default = 0, step = 1

Submit

--- .class #id 
