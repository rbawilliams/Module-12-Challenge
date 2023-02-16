
# CREDIT RISK ANALYSIS

![Alt text](Images/creditriskanalysis.pnggit )

## Table of Contents:

- Overview of the Analysis
- Results
- Model 1: Logistic Regression Model with the Original Data
- Model 2: Predict a Logistic Regression Model with Resampled Training Data
- Summary

## Overview of the Analysis:
The purpose of my analysis was to develop and compare logistic regression models that could identify the creditworthiness of borrowers. The credit risk posed a classification problem that was inherently imbalanced because healthy loans easily outnumbered risky loans. Therefore, I used various techniques to train and evaluate models with imbalanced classes.

## Results:
I trained two logistic regression models to compare two dataset versions. First, I used the original dataset. Second, I resampled the data using RandomOverSampler module from the imbalanced-learn library. For both cases, I got the count of the target classes, trained a logistic regression classifier, calculated the balanced accuracy score, generated a confusion matrix, and generated a classification report.

## Model 1: Logistic Regression Model with the Original Data
- Balanced Accuracy Score: 0.9520479254722232
- Precision Score:
- Precision for 0: 1.00
- Precision for 1: 0.83
- Recall Score:
- Recall for 0: 0.99
- Recall for 1: 0.91

## Model 2: Predict a Logistic Regression Model with Resampled Training Data
- Balanced Accuracy Score: 0.9936781215845847
- Precision Score:
- Precision for 0: 1.00
- Precision for 1: 0.99
- Recall Score:
- Recall for 0: 0.99
- Recall for 1: 0.99

## Summary:
Both models performed well in identifying the creditworthiness of borrowers. Model 2 that uses resampled data performs better with a higher balanced accuracy score, precision score, and recall score than Model 1 that uses the original data. Model 2 achieved a balanced accuracy score of 0.99, indicating that it has a higher degree of accuracy than Model 1, which achieved a balanced accuracy score of 0.95. In terms of precision, Model 2 has higher precision scores for both 0 and 1. For recall, Model 2 has a higher recall score for 1 but has similar recall score for 0 compared to Model 1.

Therefore, my recommendation is to use Model 2 that uses resampled data as it has a higher degree of accuracy and precision scores for both 0 and 1 labels.



