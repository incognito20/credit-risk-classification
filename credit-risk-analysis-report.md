Credit Risk Classification

## Overview of the Analysis

Machine learning techniques were used to train and evalute a model based on loan risk. The dataset was based on
historical lending activity from a peer-to-peer lending services company. The goal of the model was to identify the
creditworthiness of the borrower.

The financial data in the dataset was as follows:

* The loan size.
* The interest rate.
* The borrower income.
* The debt to income ratio of the borrower.
* The number of accounts.
* The number of derogatory marks.
* The borrower's total debt.
* The loan status.

The dataset was split into training and testing datasets. The training set was used to perform a logistic regression
model. The data was then resampled in order to generate an equal number of data for both types of loans. The resampled
data was modeled in order to compare the results of the first iteration.


## Results

* Machine Learning Model 1:
  * Accuracy Score: 0.9520479254722232
  * Precision 0: 1.00 Precision 1: 0.85
  * Recall 0: 0.99 Recall 1: 0.91
  * F1 Score 0: 1.00 F1 Score 1: 0.88
  * Support 0: 18765 Support 1: 619

* Machine Learning Model 2:
  * Accuracy Score: 0.9936781215845847
  * Precision 0: 1.00 Precision 1: 0.84
  * Recall 0: 0.99 Recall 1: 0.99
  * F1 Score 0: 1.00 F1 Score 1: 0.91
  * Support 0: 18765 Support 1: 619


## Summary

The logistic regression model predicts healthy loans well very. It has a precision of 100% with a large number of support. High-risk
loans on the other had only have an 85% precision rate, however, there is a significant imbalance in the data between healthy and
high-risk loans as there are only 619 high-risk loans in the model. Without additional high-risk loan data I would not use the 85% 
precision rate in making decisions as that value could very well change with additional support.

The second model is less likely to produce incorrect results given the increased number of data points used in the model. Model
2 would be the recommended model to use in order to help determine creditworthiness.
