## Introduction

In this project , we will be using financial ratios data for stock price and shares price ratios data to analyze and project If the stock prices will change. First, pulled multiple stock prices for different industries and joined with ratio analysis data for quarterly results. and then calculate the percent change. We only keep adjusted close prices for shares. 

Datas were pulled from simfin.com

## Technical 
will be using random forest and logistic regression model for the project. 

Logistic regression falls under the category of supervised learning; it measures the relationship between the categorical dependent variable and one or more independent variables by estimating probabilities using a logistic/sigmoid function.
The logistic regression model computes a weighted sum of the input variables similar to the linear regression, but it runs the result through a special non-linear function, the logistic function or sigmoid function to produce the output y.

Random forest is a Supervised Machine Learning Algorithm that is used widely in Classification and Regression problems. It builds decision trees on different samples and takes their majority vote for classification and average in case of regression.
One of the most important features of the Random Forest Algorithm is that it can handle the data set containing continuous variables as in the case of regression and categorical variables as in the case of classification. It performs better results for classification problems.


## Installation Guide
Simfin
pip install simfin

Numpy
pip install numpy


## Built with 
simfin
pandas
numpy
standardscaler
traintestsplit
randomforestclassifier
counter