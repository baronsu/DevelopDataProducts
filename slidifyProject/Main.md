Course Project of Developing Data Products
========================================================
author: BaronSu
date: 2016-10-14
autosize: true

Introduction
========================================================

This presentation is about the course project of Developing Data Products
of Data Science Specialization program of John Hopkins University. In this
presenation, we will show you

- Purpose of this application
- How we get data
- Related Links of source code and online shiny apps

Purpuse of the Application
========================================================
We devlope a simple application for users to navigate economic and population impacts
of natural disasters happened in U.S. by choosing interacive input conditions like the
following:

- State
- Year
- Event Type

Users can download data from interactive filter

How We Get Data
========================================================
The Data is obtained from U.S. National Oceanic and Atmospheric Administration's (NOAA)
database. Here is sample data:


```r
library(data.table)
dt <- fread('events.agg.csv')
head(dt)
```

```
   YEAR   STATE  EVTYPE COUNT FATALITIES INJURIES PROPDMG CROPDMG
1: 1950 alabama TORNADO     2          0       15 0.02750       0
2: 1951 alabama TORNADO     5          0       13 0.03500       0
3: 1952 alabama TORNADO    13          6      116 5.45250       0
4: 1953 alabama TORNADO    22         16      248 3.07000       0
5: 1954 alabama TORNADO    10          0       36 0.60753       0
6: 1955 alabama TORNADO     8          5       27 7.58000       0
```

Related Links
====
[GitHub] (https://github.com/baronsu/DevelopDataProducts)

[Download Data](https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2FStormData.csv.bz2)

[Shiny online App](https://baronsu.shinyapps.io/shinyProject/)
