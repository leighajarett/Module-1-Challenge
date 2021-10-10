# Credit Risk Analysis (Module 1 Challenge)

## Overview
The purpose of this analysis was to predict credit risk for loan applicants for LendingClub, a peer-to-peer lending services company.  Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, to ensure that we are accurately identifying loan applicants who are risky, we tested out several different techniques and evaluated the performance of each. 

## Results
To ensure we were approaching this problem in the best way, we began by exploring the data and understanding the training inputs as well as the class to be predicted. We then tested several methods for sampling and evaluated the accuracy of each using a Logistic Regression classifier. 

- *Oversampling using Naive Random* 
  - Balanced accuracy score of 64%
  - Precision score of 1%
  - Recall score of 59%
- *Oversampling using SMOTE* 
  - Balanced accuracy score of 62%
  - Precision score of 1%
  - Recall score of 59%
- *Undersampling using Cluster Centroids*
  - Balanced accuracy score of 53%
  - Precision score of 1%
  - Recall score of 61%
- *Combination sampling using SMOTEEN*
  - Balanced accuracy score of 61%
  - Precision score of 1%
  - Recall score of 68%

Additionally, we tested two different ensemble learning methods.

- *Balanced Random Forest Classifier*
  - Balanced accuracy score of 79%
  - Precision score of 4%
  - Recall score of 57%
- *Easy Ensemble AdaBoost Classifier*
  - Balanced accuracy score of 93%
  - Precision score of 8%
  - Recall score of 92%

## Summary
Based on these results, the Easy Ensemble AdaBoost classifier performed best in terms of accuracy, precision and recall. I recommend that the team uses the Easy Ensemble AdaBoost classifier as it has a recall of 92% - meaning it will correctly identify about 92% of all high risk loans. In this case, we want to optimize for precision since we would rather flag safe loans as potentially risky than miss risky loans that need further investigation. 
