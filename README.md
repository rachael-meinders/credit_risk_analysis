# Credit Risk Analysis

## Overview
This analysis examines a credit card dataset from LendingClub, a peer-to-peer lending services company. Due to the inherent imbalance of low- vs high-risk lending, a variety of resampling and ensembling techniques are used as part of a logistic regression. Each technique is then evaluated and compared for best performance.

## Results
- The undersampling model was the least accurate overall, with an accuracy score of 0.544.
- The Easy Ensemble AdaBoost Classifier was the most accurate, with an accuracy score of 0.925.
- The remaining four models were all moderately accurate, with accuracy scores in the range of 0.6 - 0.7.
- All 6 models had a considerably higher precision than recall, indicating that these are all somewhat conservative models with a higher reliability of positive classification. 
- The recall for the ensembling models were much higher than the resampling models, indicating that were more aggressive models in flagging high-risk loans.


## Summary
While resampling models were mildly accurate and effective in compensating for the imbalance of low- vs high-risk loans, the ensembling methods were overall better performing. 

To best enhance the overall accuracy of the model, the Easy Ensemble AdaBoost Classifier would be the best choice due to the accuracy score of 0.925. This model also had a high recall for high risk loans, leading to a high number of high-risk loans being flagged. However, if an analysis values a high degree of accuracy for flagged loans, the Balanced RAndom Forest Classifier would be most successful due to its high precision. The four resampling methods are in no way bad or inaccurate models, but their performance do not match the success of the ensemble methods.