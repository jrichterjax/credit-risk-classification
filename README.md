# Credit Risk Analysis Report

## Overview of the Analysis

The purpose of this analysis is to identify the creditworthiness of borrowers. To accomplish this, two logistic regression models were created.


## Results

* Logistic Regression Model with the Original Data:
  * Accuracy - high level of overall accuracy at 95%
  * Precision - higher precision for healthy loans (100%) than high-risk loans (85%) 
  * Recall scores - higher recall scores for healthy loans (99%) than high-risk loans (91%) 


* Logistic Regression Model with Resampled Training Data:
  * Accuracy - high level of overall accuracy at 99%
  * Precision - higher precision for healthy loans (100%) than high-risk loans (84%) 
  * Recall scores - similar recall scores for healthy loans (99%) and high-risk loans (99%) 

## Summary

Due to higher precision and recall percentages, the logistic regression model with the original data better predicts healthy loans than high-risk loans. On the other hand, fit with oversampled data the logistic regression model's recall precentage is significantly higher for high-risk loans. This indicates that more loans are predicted as high-risk using the oversampled data than without which catches more true negatives but also results in slightly more false negatives. Additionally, the model using oversampled data has a higher accuracy rate (99%) compared to the original data model (95%).

From a lender perspective, it would be more important to predict the 1's, or the high-risk loans. In that case, the logistic regression model with resampled training data would be the better model to use. Since the recall score for high-risk loans is significantly higher using this model, then we know that more loans will be flagged as high-risk, therefore significantly decreasing the number of loans that are defaulted on, presumably outweighing the loss in profit from slightly fewer healthy loans provided.

