---
title: "Project_2_Storm_Data"
author: "Benjamin Sila"
date: "Friday, August 21, 2015"
output: html_document
---

Impact of Storms and other severe weather events can cause both public health and economic problems for communities and municipalities.

This project analyzes the effects of Storms and other severe weather events which cause both public health and economic problems for communities and municipalities. Many severe events can result in fatalities, injuries, and property damage, and preventing such outcomes to the extent possible is a key concern.

- The data for this assignment comes in the form of a comma-separated-value file compressed via the bzip2 algorithm to reduce its size and downloaded herein:

- Read the data from the working dir:

```{r}
rawdata <- read.csv(bzfile("data/repdata_data_StormData.csv.bz2"), header = TRUE, stringsAsFactors = FALSE)
```

```{r echo=FALSE}
dim(rawdata)
```

There are 902297 rows and 37 columns in total


### Questions

Your data analysis must address the following questions:

1.Across the United States, which types of events (as indicated in the EVTYPE variable) are most harmful with respect to population health?

2.Across the United States, which types of events have the greatest economic consequences?

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.