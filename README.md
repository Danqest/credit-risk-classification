# credit-risk-classification

## Overview of the Analysis

- The purpose of this analysis is to use supervised machine learning to predict high-risk loans from a cross-sectional dataset of features. The data is first modeled using Logistic Regression using an unbalanced dataset with substantially different figures for the two labeles, and then modeled again with Logistic Regression using Random Oversampling to have a more balanced label-set.
- Features in the dataset include loan size, interest rate, borrower income, debt-to-income ratios, number of accounts, and delinquencies, with over 75k rows of data; classification for healthy and high-risk loans is binary between 0 (75,036 labels) and 1 (2500 labels) respectively.

## Results

- Machine Learning Model 1:

  - Accuracy: 0.9520
  - Precision: 0 Label - 1.00, 1 Label - 0.85
  - Recall: 0 Label - 0.99, 1 Label - 0.91

- Machine Learning Model 2:
  - Accuracy: 0.9937
  - Precision: 0 Label - 1.00, 1 Label - 0.99
  - Recall: 0 Label - 0.84, 1 Label - 0.99

## Summary

- Both models have good accuracy scores but overall the 2nd model performs better with an accuracy of 0.9937 and a recall (true positives) for the at-risk loan classification of 0.99.
- It is more important to accuractely identify true-positive labels for at-risk loans; though model 2 tends to label more false positives than model 1 we would rather be more cautious and overall more conservative in our assessment of credit risk to avoid defaults.
