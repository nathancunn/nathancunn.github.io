---
layout: post
title:  The decline of Katrinas after Hurricane Katrina
date: "2017-09-10 14:00:00"
image: /figure/source/hurricane_katrina/katrina.png
share-img: http://www.nathancunn.com/figure/source/hurricane_katrina/katrina.png
---

With a series of large hurricanes hitting the US recently, I wondered what impact their names have on people's opinion of those names for their children: do people try avoid the new negative connotations of the name or is that even a factor in their decision process?

For some superficial exploration of this I looked at the single case of Hurricane Katrina because it had the useful combination of being both a hugely devastating hurricane and being given a reasonably common name. As you can see below, the name Katrina underwent a massive decrease in popularity in the years immediately following the hurricane, with a drop of just under 90% in girls named Katrina ten years after the hurricane, compared to ten years prior.

![No. of babies born named Katrina 1995 - 2015](https://raw.githubusercontent.com/nathancunn/nathancunn.github.io/master/figure/source/hurricane_katrina/katrina.png)

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

<p style="width: 100%; height: 0px; padding-bottom: 56.25%; position: relative;">
	<iframe style="width: 100%; height: 100%; position: absolute; left: 0px; top: 0px;" src="https://www.youtube-nocookie.com/embed/mc2_zYDuHC4" frameborder="0" allowfullscreen="">
	</iframe>
</p>


With that done, plotting the data is straightforward using `ggplot2`. The annotated arrows were added after in Inkscape.

``` r
library(ggplot2)
year = 2005
name = "Katrina"
sex = "F"
ggplot(names_dat[names_dat$name == name & names_dat$sex == sex & names_dat$year %in% seq(year - 10, year + 10), ], 
       aes(x = year, y = count)) +
       geom_line() +
       geom_vline(xintercept = 2005)
```

