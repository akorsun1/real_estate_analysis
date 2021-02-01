## Predicting House Prices in King County, WA

## Problem Statement:

This is a project for a real estate agency that helps homeowners sell their homes. I have been tasked to analyze King County housing data set to provide the agency with advice about which home renovations might increase the estimated value of a home so seller can decide which renovations to make. Therefore, in my data analysis, I will explore the most impactful features in terms of pricing.

## Approach and methodology:

1. Import the data
2. Clean the data
3. Explore the data
4. Model 
5. Interpret
6. Recommendations
7. Conclusions
8. Future work

## Diagonal correlation matrix

Diagonal correlation matrix answers an important question for my analysis : "Which features are the most impactful in terms of pricing?."

According to this correlation matrix, I can assume that bulding grade impacts price significantly due to the high correlation level (0.68). Also, I can state that the next features are the most impactful in terms of pricing: sqft_living,grade, bathrooms.

However, my analysis will be more valuable if I will use other methods to answer my research question.

![download](https://user-images.githubusercontent.com/68250383/106407954-43369300-640b-11eb-8371-7158a1b80687.png)

## Models Training

The Linear Regression model may be a good option to show a dependency between price and features, however, I have decided to use Lasso and Ridge models too. Also, I will use log of target in my models training. 

Therefore, to make my final conclusions more reliable, I will be comparing Linear Regression, Ridge and Lasso prediction models with original target and with log of target to find the best model based on R2 score. Then, I will use additional metrics (Mean Squared Error, Mean Absolute Error and Root Mean Square Error) to measure the errors of a chosen model.

In the result of comparison of 6 models I have decided to proceed with Linear Regression with original target because this model has the highest R2 score (0.633414).

## Linear Regression with Original Target

In this section I compare weights to define the most important features.

![download (1)](https://user-images.githubusercontent.com/68250383/106408546-affe5d00-640c-11eb-89e1-e973245eb9d0.png)

















