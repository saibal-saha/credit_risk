# Module 12 Credit Risk Analysis Report

## Overview of the Analysis

* Explain the purpose of the analysis.

### We were provided a set of data consisting of multiple independent variables or X variables and y variable also known as dependent variable. Here the y variable is a binary classifier where '0' indicates healthy loan and '1' indicates high risk loans. The purpose of this analysis is to create Logistic Regression model with the original data and predict a logistic regression model with resampled training data, and compare how each of these models perform against each other to accurately classify whether a loan is 'healthy' or 'high-risk'.


* Explain what financial information the data was on, and what you needed to predict.

### The financial information given was various individuals financial data like loan size, interest rate, borrower's income, total debt, debt to income ratio, total accounts and deragatory marks. Using these financial data we are supposed to predict whether a given loan is healthy or at high risk.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

### We were trying to predict the y variable also known as the dependent variable. '0' being healthy loan and '1' being high risk loan. using value_counts we could analyze in the given data set what percentage of the loans were healthy and what percentage of the loans were at high risk.  

* Describe the stages of the machine learning process you went through as part of this analysis.

### At first the data were seperated into X variables and y variables. The data was then split into training and testing data sets. Then a machine learning model was fitted for the training data. Then based on that predictions were made on the test data and the performance of the machine learning model was evaluated in terms of accuracy precision and recall.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

### Logistic Regression is a type of supervised machine learning algorithm used for classification problems. It is a statistical method that is used to fit a regression model when the response variable is binary. The goal of logistic regression is to find the best parameters for the model that maximizes the likelihood of correctly classifying the training data. The model uses a logistic function (also called sigmoid function) to predict the probability of the dependent variable being of a certain class. Once the model is trained, it can be used to make predictions on new, unseen data.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
        -Accuracy : 0.9520479254722232
        -Precision: '0' - 1.00 , '1' - 0.85
        -Recall   : '0' - 0.99 , '1' - 0.91


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
         -Accuracy : 0.9936781215845847
         -Precision: '0' - 1.00 , '1' - 0.84
         -Recall   : '0' - 0.99 , '1' - 0.99
  
  notes

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

### Comaparatively, the Model 2 performs better than the Model 1. It has higher accuracy score and although it has slightly lower precision score compared to Model 1 while comparing risky loans, it has much better recall score of 0.99 comared to 0.91. 

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

### Performance does depend on the problem we are trying to solve. Given the current problem although both the models can very accurately predict the healthy loans but while trying to predict the unhealthy loans both the models perform very poorly. and given the problem it is much more desirable to predict unhealthy loans accurately than the healthy loans, as the financial ramafications are much more dire if an unhealthy loan is classified as healthy loan. Hence in this scenario it would be recommended to avoid both these models.

If you do not recommend any of the models, please justify your reasoning.
