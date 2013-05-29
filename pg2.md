---
title       : My First Test
subtitle    : HTML5 slides
author      : JPN
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]     # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
  
--- .class #id 

## Plot Eg

![plot of chunk unnamed-chunk-1](figure/unnamed-chunk-1.png) 


---

You can use Latex's typesetting
$$\sum_{i=0}^n x_i$$

---

### A Simple Plot

Let us create a simple scatterplot. 


```r
require(ggplot2)
qplot(wt, mpg, data = mtcars)
```

![plot of chunk simple-plot](figure/simple-plot.png) 


--- 

### A Table


```r
library(xtable)
```

```
Error: there is no package called 'xtable'
```

```r
options(xtable.type = "html")
xtable(head(mtcars))
```

```
Error: could not find function "xtable"
```


---

## Animated List

> 1. Point 1
> 2. Point 2


<!-- Do it once to install needed packages:
# library(devtools)
# install_github('slidify', 'ramnathv')
# install_github('slidifyLibraries', 'ramnathv')
-->

<!-- need to execute:
library(slidify)
author("slidifyEg")  # create a new slidify project
slidify("index.Rmd") # can be made at RStudio with the 'Knit HTML'

publish('slidifyFolder', host = 'dropbox')  # to post at dbox's Public folder

# replace USER and REPO with your username and reponame
# publish(user = "USER", repo = "REPO", host = 'github')
------------------------------------------------------------ -->
