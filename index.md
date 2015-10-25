---
title       : Developing Data Products - Project
subtitle    : 
author      : Kelvin Han
job         : 
framework   : revealjs        # {io2012, html5slides, shower, dzslides, ...}
revealjs    : 
theme       : solarized
transition  : cube
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Interactive NOAA storm data explorer

Kelvin Han

--- .class #id

## The application

The Interactive NOAA data explorer is available at
https://kelvin.shinyapps.io/DevDataProd

This application enables the user to select inputs and presents the output on an interactive map or on a table.

--- .class #id

## The data

The data is from the US National Oceanic and Atmospheric Administration (NOAA) storm database.

The dataset is available at 
https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2

--- 

## A peek at the Post-Processed Data

```r
head(dataFile)
```

```
##    YEAR STATE EventName FATALITIES INJURIES propDmgValue cropDmgValue
## 1: 1950    AL   Tornado          0       15        27500            0
## 2: 1950    AR   Tornado          2       49       860030            0
## 3: 1950    CO   Tornado          0        1        50000            0
## 4: 1950    CT   Tornado          0        3       252500            0
## 5: 1950    FL   Tornado          0        0        82500            0
## 6: 1950    GA   Tornado          0        1        32500            0
```

---

## Leaflet

This application uses Leaflet, an open-source JavaScript library, for the interactive map. More information is available at the link below.

https://rstudio.github.io/leaflet/
