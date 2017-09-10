---
layout: post
title:  Hurricane Katrina led to a sharp fall in the number of babies born named Katrina
date: "2017-07-16 08:30:10"
image: /figure/source/simpsons-characters/all_seasons.png
share-img: http://www.nathancunn.com/figure/source/hurricane-katrina/katrina.png
---

![No. of babies born named Katrina 1995 - 2015](http://www.nathancunn.com/figure/source/hurricane-katrina/katrina.png)

The data for this plot are all freely available on the site for the US government's open data, specifically [here](https://catalog.data.gov/dataset/baby-names-from-social-security-card-applications-national-level-data). If you'd like to recreate this plot yourself you'll need to download and unzip the data. The data come in individual files for each year from 1880-2016, listing the most popular names for boys and girls born in that year. Due to privacy restrictions, only names which were used at least five times in the specified year are included. The first step is to concatenate these datafiles into a single dataset, which we can do with the following R code.

``` r
setwd("/directory/containing/only/unzipped/data/")
names_files <- list.files()

for(file in names_files) {
  tmp <- read.csv(file, header = FALSE)
  # We need to create a year variable in the data
  tmp <- cbind(tmp, as.numeric(substr(file, start = nchar(file) - 7, nchar(file) - 3)))
  names(tmp) <- c("name", "sex", "count", "year")
  if(exists("names_dat")) {
    names_dat <- rbind(names_dat, tmp)
  } else {
    names_dat <- tmp
  }
}

```

With that done, plotting the data is straightforward using `ggplot2`. The annotated arrows were added after in Inkscape.

``` r
library(ggplot2)
year = 2005
name = "Katrina"
sex = "F"
ggplot(names_dat[names_dat$name == name & names_dat$sex == sex & names_dat$year %in% seq(year - 10, year + 10), ], 
       aes(x = year, y = count)) +
       geom_line()
```
