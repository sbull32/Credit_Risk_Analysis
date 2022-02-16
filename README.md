# Credit_Risk_Analysis
Supervised Machine Learning

## Overview
The purpose of this analysis is to use machine learning models to help predict a loan applicant's credit risk. We will use data from Q1 of 2019 to train and test six different machine learn model methods and determine which one is best suited to predict an applicants credit risk in the future. 

## Results
Below are the results of the six machine learning models we used for this analysis including the balanced accuracy, precision, and recall scores.

### Random Native Oversampling

- Balanced accuracy: 0.62346
- Precision: 0.99
- Recall: 0.62

![Random Oversampling](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/NaiveRandomOS.png)

### SMOTE Oversampling

- Balanced accuracy: 0.62501
- Precision: .99
- Recall: .62

![SMOTE Oversampling](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/SmoteOS.png)

### Undersampling

- Balanced accuracy: 0.49134
- Precision: 0.99
- Recall: 0.42

![Undersampling](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/US.png)

### Combination Sampling

- Balanced accuracy: 0.65447
- Precision: 0.99
- Recall: 0.57

![Combo Sampling](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/ComboS.png)

### Random Forest Classifier

- Balanced accuracy: 0.99816
- Precision: 1.00
- Recall: 1.00

![BRFC](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/BRFC.png)

### Easy Ensemble Classifier with AdaBoost

- Balanced accuracy: 1.00000
- Precision: 1.00
- Recall: 1.00

![EEC](https://github.com/sbull32/Credit_Risk_analysis/blob/main/Credit_Risk_Analysis/EEC.png)

## Summary

In summary, the oversampling methods (both random native and SMOTE) produced relatively high accuracy scores (.62) as well as high recall scores (.62). Our undersampling model had the lowest accuracy (.49) and recall score (.42) amongst the models tested. While the combination method did increase the accuracy score (.65) it did have a lower recall score (.57) than our oversample models. Finally both our Random Forest classifier and Easy Ensemble Classifier with AdaBoost models had extremely high accuracy (.998, 1) and recall scores (1). 

After our six models were evaluated, we determined that we did not have enough informatino to make a recomendation on which model to use for predicting future credit risk. This is because all 4 of the models which involved over or under sampling had relatively low recall scores (.62, .57, .42) which is the most essential score when predicting credit risk. The last two models both had such high accuracy, precision, and recall scores that we were concerned these models possibly were overfitted to the data and might not accurately predict a new set of applicants credit risk correctly.


