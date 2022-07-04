# Credit Risk Analysis

## Overview 
An analysis of credit risk was done using data from LendingClub. Due to the imbalanced nature of classifying fraud, multiple techniques were used to resample the data before training and evaluating multiple models. The imbalanced-learn and scikit-learn python libraries were used to conduct these analyses. The resampling algorithms used were: RandomOversampler, SMOTE, ClusterCentroids, SMOTEENN. The ensemble learing algorithms used were: BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Results 
### Resampling (Logistic Regression Learning)
#### RandomOverSampler
- Balanced accuracy score: 
- Precision score: 0.64
  - low risk: 1.00
  - high risk: 0.01
- Recall score:
  - low risk: 0.62
  - high risk: 0.66
  
#### SMOTE Oversampling
- Balanced accuracy score: 0.65
- Precision score:
  - low risk: 1.00
  - high risk: 0.01
- Recall score:
  - low risk: 0.69
  - high risk: 0.61
  
#### ClusterCentroids Undersampling
- Balanced accuracy score: 0.54
- Precision score:
  - low risk: 1.00
  - high risk: 0.01
- Recall score:
  - low risk: 0.40
  - high risk: 0.69

#### SMOTEENN (Combination Over and Undersampling)
- Balanced accuracy score:  0.64
- Precision score:
  - low risk: 1.00
  - high risk: 0.01
- Recall score:
  - low risk: 0.57
  - high risk: 0.71

### Ensemble Learning
#### BalancedRandomForestClassifier
- Balanced accuracy score: 0.79
- Precision score:
  - low risk: 1.00
  - high risk: 0.03
- Recall score:
  - low risk: 0.87
  - high risk: 0.70
  
#### EasyEnsembleClassifier
- Balanced accuracy score: 0.93 
- Precision score:
  - low risk: 1.00
  - high risk: 0.09
- Recall score:
  - low risk: 0.94
  - high risk: 0.92
  
## Summary

The EasyEnsembleClassifier had the highest scores for balanced accuracy (0.93), precision (for high risk), and recall (both low and high risk).
