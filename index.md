---
title       : Exponential Distribution Simulation
subtitle    : Assignment for Developing Data Products
author      : KP Fong
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction



This application runs interactive simulation of exponential distribution and visualizes the distribution of the mean values. 

The user is able to create simulations by specifying the number of iterations per simulation, the number of random samples to generate and the lambda (rate) parameter.

Based on these parameters, the user can investigate and draw conclusions on the natute of  the distribution of the means for randomly generated exponential values. 

---
## How to Use

# User is able to adjust the following parameters

1. No. of samples to run for each simulation 
2. Lambda - the rate parameter for Poisson-type distribution
3. No. of Iterations to run the simulation


# The results of the simulation is displayed as

1. Histogram that reports the distribution of the means for the simulation.
2. The standard deviation of the mean values
3. The variance of the mean values 

---
## How the code works

The application uses rexp() function to geneate the random exponential values.
The function below creates 30 random values with lambda value of 0.2.


```r
rexp(30, 0.2)
```

```
##  [1]  5.3523  5.1281 11.4165  7.3554  0.7573  7.1172 14.8354  5.3462
##  [9]  4.3916  0.8740  3.7377 26.7516  4.3935 13.7723  1.5945  2.8627
## [17]  2.9136  7.2531  7.5642  9.6401 13.7129  6.0101  8.0870  4.9704
## [25]  3.0698  7.4335  2.6445  2.2067  2.5713  1.7554
```
The user can specify the no. of rounds this simulation generates. The application calculates the means of each iteration and visualizes the results as a histogram.

The user can study and draw their conclusion of the nature of the distribution of the means.

---
## Reference

Application can be assessed at the following URL:

url:http://piewsook.shinyapps.io/shiny1/

Interactive visualization is created with Shiny.

Presentation is prepared with Slidify.



