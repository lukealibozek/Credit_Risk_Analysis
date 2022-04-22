# Overview

This project tests numerous supervised machine learning models for their ability to predict credit risk when evaluating loan applications. 

The following algorithms were used:
- **Oversampling**: 
  - Naive Random Oversampling
  - SMOTE
- **Undersampling**: 
  - Cluster Centroids
- **Combination Sampling**: 
  - SMOTEENN
- **Ensemble Learners**: 
  - Balanced Random Forest Classifier
  - Easy Ensemble AdaBoost Classifier

# Results

## Naive Random Oversampling

![](resources/naive_BAS.png)
![](resources/naive_CM.png)
![](resources/naive_ICM.png)

- **Balanced Accuracy Score**: 61%
- **Precision**: 1% (High) 100% (Low)
- **Sensitivity**: 56% (High) 66% (Low)
- **F1**: 2% (High) 80% (Low)

## SMOTE

![](resources/smote_BAS.png)
![](resources/smote_CM.png)
![](resources/smote_ICM.png)

- **Balanced Accuracy Score**: 64%
- **Precision**: 1% (High) 100% (Low)
- **Sensitivity**: 59% (High) 70% (Low)
- **F1**: 2% (High) 82% (Low)

## Cluster Centroids

![](resources/under_BAS.png)
![](resources/under_CM.png)
![](resources/under_ICM.png)

- **Balanced Accuracy Score**: 50%
- **Precision**: 1% (High) 99% (Low)
- **Sensitivity**: 52% (High) 49% (Low)
- **F1**: 1% (High) 65% (Low)

## SMOTEENN
![](resources/comb_BAS.png)
![](resources/comb_CM.png)
![](resources/comb_ICM.png)

|           |Naive ROS|SMOTE|Cluster|SMOTEENN|
|-----------|---------|-----|-------|--------| 
|BAS        |61%      |64%  |50%    |63%     | 
|Pre (High) |1%       |1%   |1%     |1%      | 
|Pre (Low)  |100%     |100% |99%    |100%    | 
|Rec (High) |56%      |59%  |52%    |66%     | 
|Rec (Low)  |66%      |70%  |49%    |62%     | 
|F1 (High)  |2%       |2%   |1%     |2%      |
|F1 (Low)   |80%      |82%  |65%    |76%     | 