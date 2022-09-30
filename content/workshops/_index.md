---
header:
  caption: ""
  image: ""
title: 
view: 2
output: 
  html_document: default
    code_folding:hide
---

# Upcoming Workshops:

<!-- <p style="color:red;font-family:courier;"><strong> We have had to postpone our August workshop on ggplot until next term (details to follow very soon!). Instead, we will still be available on Monday for a drop-in help session - details below.</strong></p> --> 

<p style="font-family:courier;">Frustrated with R? Have a problem with your code? Just want help getting started? Come to our relaxed IN PERSON drop-in help sessions where you can sit down with a seasoned R coder and get personal one-on-one help. We all started somewhere, and we know how hard it can be! No registration required, and all are welcome. Feel free to also come along and contribute by helping others in the community!

<strong>Location: [Teaching Lab 3 (Skeleton Lab)](https://studentvip.com.au/unsw/kensington/maps/134111) in Building D26, Ground floor 
Time: 2:30 - 3:30pm </strong>
<!-- <img src="geospatial_flyer_2.png" width=1450 style = "margin-left: 0px; margin-right: 0px; float:right;"> --> 

```{r} 
knitr::opts_chunk$set(echo=FALSE) 
```

```{r echo = FALSE, include = FALSE}
# Create a table for our events
t3 <- data.frame(matrix(nrow = 5, ncol = 3))
colnames(t3) <- c("Date", "Event Description", "Presenter name")

t3[,1] <- c("12 Sept 2022", "26 Sept 2022", "10 Oct 2022", "24 Oct 2022", "07 Nov 2022")

# Drop in help sessions
t3[c(1, 3), 2] <- "Drop In Help Session"
t3[c(1, 3), 3] <- "UNSWcodeRs helpers"

# ggplot
t3[2, 2] <- "It’s all about the aesthetics: dataviz with ggplot2::theme()"
t3[2, 3] <- "PhD candidate Jess Tam"

# Meta-analysis
t3[4, 2] <- "Meta-analysis 101"
t3[4, 3] <- "Prof. Shinichi Nakagawa"

# R Slides
t3[5, 2] <- "Create your presentations in R"
t3[5, 3] <- "PhD candidature Tehilla Mechera-Ostrovsky"
```


```{r}
library(knitr)
knitr::kable(t3, "pipe")
```


# Past Workshops & Resources:
