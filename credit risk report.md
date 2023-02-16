
# CREDIT RISK ANALYSIS

![Alt text](creditriskanalysis.png)

## Table of Contents:

- Introduction

- Loan Data Description

- Machine Learning Process
    a. Splitting the Data into Training and Testing Datasets
    b. Training Different Machine Learning Models
    c. Model Evaluation

- Results and Recommendations



## Introduction

In this analysis, my goal was to build machine learning models that can predict loan risk based on given financial data. To achieve this goal, I used a loan dataset that includes information on the loan status, annual income, debt-to-income ratio, and others. The task was to predict the loan status, which is binary, either healthy loan or high-risk loan.

## Loan Data Description
The loan status column has two values: 0, which indicates a healthy loan, and 1, which indicates a high-risk loan. The value counts of the loan status column show that 75036 loans are healthy, while 2500 loans are high-risk.

## Machine Learning Process
**Splitting the Data into Training and Testing Datasets**

 I split the data into training and testing datasets to train the models and evaluate their performance.

**Training Different Machine Learning Models**

I trained two different machine learning models, logistic regression and random forest, to predict loan risk.

**Model Evaluation**

To evaluate the performance of the models, I calculated the balanced accuracy, precision, and recall scores, generated a confusion matrix, and printed a classification report for each model. The results of the evaluation are summarized as follows:

## Logistic Regression:
- Balanced accuracy score: 95.2%
- Precision score: 100% for healthy loans (class 0) and 85% for high-risk loans (class 1)
- Recall score: 91% for high-risk loans (class 1)
## Random Forest:
- Balanced accuracy score: 92.2%
- Precision score: 99% for healthy loans (class 0) and 80% for high-risk loans (class 1)
- Recall score: 87% for high-risk loans (class 1)

## Results and Recommendations
Based on the evaluation, the logistic regression model performs better in terms of balanced accuracy and precision scores. It achieved a higher balanced accuracy score and higher precision score for high-risk loans, which is important since the goal is to accurately predict high-risk loans. The performance of the models depends on the problem we are trying to solve. In this case, it is more important to predict high-risk loans accurately, and the logistic regression model seems to perform better in this regard.

Therefore, I **recommend** using the **logistic regression model** to predict loan risk.