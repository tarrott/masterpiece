---
title: "Recipes"
date: 2021-02-27T15:33:16-05:00
draft: false
---


## Linear Regression
- goal: fitting a line to a data set
- many different methods
- use residuals to determine if linear regression is appropriate for the data set
    - seeing a "random" residual plot is a good sign for linear regression
    - if a pattern exists, then another method would most likely be a better fit
- if a curve would fit the data better then a polynomial would be more appropriate than linear regression

#### Ordinary Least Squares
- fit a line to the data set that minimizes the distances between all of the data points

#### Gradient Descent
- calculate the error of a guess (cost) by subtracting what the output should be by the estimate of the output
- move the estimate in the direction that minimizes the error (cost) by making small adjustments to the parameters (weights) affecting the estimate by using a learning rate
- stochastic gradient descent is adjusting the weights by each data point, opposed to batch gradient descent by adjusting all the weights at the same time