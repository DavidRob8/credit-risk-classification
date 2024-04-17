# Module 12 Report

## Analysis Overview

In this module, I used various techniques to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers. More specifically, I trained the model to predict the loan status as "healthy" or "high-risk". The data included information such as loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt, and loan status.

I first split the data into training and testing datasets by using train_test_split from sklearn. Then I created a logistic regression model with the training data (X_train and y_train), made a prediction using the testing data (X_test), evaluated the model's performance by generating a confusion matrix that displays true positives, true negatives, false positives, and false negatives, and produced a classification report for the model.

## Results

- Overall Accuracy: 99%
- Precision
    - Healthy loans: 100%
    - High-risk loans: 87%
 - Recall
    - Healthy loans: 100%
    - High-risk loans: 89%


## Summary

The logistic regression model predicts both the healthy loans and the high-risk loans with great accuracy at 99%. For the healthy loans in particular, precision and recall are at 100% and the F1-score is at 1 which is an almost flawless model. The sample size was much larger for healthy loans, 18,679, and there were only 67 false negatives. For high-risk loans, precision was at 87%, recall was at 89%, and the F1-core was at .88. This model did not perform as well for the high-risk loan perhaps due to the much smaller sample size, 563, but it would still be considered to be a very solid model. Overall, the model performed very well for both types of loans. The lending services company would definitely want to avoid false negatives in which a loan is deemed to be healthy when it's actually high-risk. I would recommend this model to the lending services company because this model boasts very strong results in accuracy, precision, and recall.
