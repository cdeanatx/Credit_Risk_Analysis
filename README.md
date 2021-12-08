# Credit Risk Analysis

## Overview of Analysis

The purpose of this project is to create a model that will identify high-risk credit applications. We will assess the differences between different supervised machine learning techniques and determine which strategy yields the best results.

------

## Results of Analysis

For our analysis, we used six different machine learning techniques. The pros and cons of which will be discussed below.

|                                             |                   Balanced Accuracy Score                    |                    Classification Report                     |
| :-----------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|        **Naive Random Oversampling**        | ![NRBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/naive_random_balanced_accuracy.png) | ![NRCR](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/naive_random_classification.png) |
|           **SMOTE Oversampling**            | ![SMOTEBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/smote_balanced_accuracy.png) | ![SMOTEBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/smote_classification.png) |
|    **Clustered Centroids Undersampling**    | ![CCBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/cluster_balanced_accuracy.png) | ![CCBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/cluster_classification.png) |
|      **SMOTEEN Combination Sampling**       | ![SMOTEENBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/smoteen_balanced_accuracy.png) | ![SMOTEENBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/smoteen_classification.png) |
|    **Balanced Random Forest Classifier**    | ![RFBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/random_forest_balanced_accuracy.png) | ![RFBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/random_forest_classification.png) |
| **Easy Ensemble Adaptive Boost Classifier** | ![AdaboostBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/ada_boost_balanced_accuracy.png) | ![AdaboostBAS](https://github.com/cdeanatx/Credit_Risk_Analysis/blob/main/images/ada_boost_classification.png) |

**Naive Random Oversampling**

- Balanced Accuracy Score: 64.5%
- Precision
  - High risk: 0.01
  - Low risk: 1.00
- Recall
  - High risk: 0.70
  - Low risk: 0.59

**SMOTE Oversampling**

- Balanced Accuracy Score: 
- Precision
  - High risk: 0.01
  - Low risk: 1.00
- Recall
  - High risk: 0.63
  - Low risk: 0.69

**Clustered Centroids Undersampling**

- Balanced Accuracy Score: 
- Precision
  - High risk: 0.01
  - Low risk: 1.00
- Recall
  - High risk: 0.69
  - Low risk: 0.40

**SMOTEEN Combination Sampling**

- Balanced Accuracy Score: 
- Precision
  - High risk: 0.01
  - Low risk: 1.00
- Recall
  - High risk: 0.69
  - Low risk: 0.58

**Balanced Random Forest Classifier**

- Balanced Accuracy Score: 
- Precision
  - High risk: 0.03
  - Low risk: 1.00
- Recall
  - High risk: 0.70
  - Low risk: 0.07

**Easy Ensemble Adaptive Boost Classifier**

- Balanced Accuracy Score: 
- Precision
  - High risk: 0.09
  - Low risk: 1.00
- Recall
  - High risk: 0.92
  - Low risk: 0.94

------

## Summary of Analysis

Accurate identification of high-risk credit applications is our primary concern and models will be evaluated on this criterion. In this model, we want to avoid false negatives, i.e. we don't want the model to tell us an application is low risk when it is actually high risk. Therefore, the best model will have a **high recall** for high risk.

Based on this criteria, the **Easy Ensemble Adaptive Boost Classifier** model gives us the best results by a large margin. Its recall is 0.92, with the closest competiors being Naive Random Oversampling and Balanced Random Forest Classifier, which both come in at a 0.70 recall.

