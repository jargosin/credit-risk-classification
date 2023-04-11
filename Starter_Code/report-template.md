# Module 12 Report

## Overview of the Analysis

* The purpose of the analysis is to create a regression model that can accutately predict whether a loan is healthy (0) or high-risk (1).

* The data contains various account details that factor into credit risk. This includes loan size, income, total debt and number of accounts. Using these factors, we will be able to determine whether or not any given account is suitable for a loan or deemed high-risk

* There are 75,036 healthy loans, and 2,500 high-risk loans in this dataset.

* First, we split the data into training and testing datasets. We then fit the logistic regression model to predict and compare the results. After, we perform a classification report to evaluate the precision of the model. We do these steps again but with the RandomOverSampler module to see if the model performance improves.

* Logistic regression utilizes financial account variables to predict wheather a loan is considered healthy or high-risk. 

## Results

* Machine Learning Model 1:
  * Model 1 accuracy was 95.20%, with a precision score of 100% for healthy loans and 85% for high-risk loans.
  
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

* Machine Learning Model 2:
  * Model 2 accuracy was 99.36%, with a precision score of 100% for healthy loans and 84% for high-risk loans. 
  
               precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

## Summary

* Both models preformed with excellent precision, and differences between them are marginal but are definetly worth comparing. When trying to achieve higher overall accuracy model 2 is favorable, but for slightly higher precision for high-risk loans, model 1 performs better.
