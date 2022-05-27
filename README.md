# Credit Risk Analysis

## Overview of the analysis.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Python was used in order to build and evaluate different machine learning models to predict credit risk. A credit card dataset from LendingClub was used for this analysis. We oversampled the data using RandomOverSampler and SMOTE algorithms and undersampled the data using ClusterCentroids algorithm. SMOTEENN algorithm was used to do oversampling and undersampling. Finally in order to predict credit risk, we compared BalancedRandomForestClassifier and EasyEnsembleClassifier.


## Results.

### Naive RandomOverSampling

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/NaiveRandomOverSampling.png)

* The balanced accuracy score is 65%.
* The high risk precision is 1% with 62% sensitivity.
* the low risk precision is 100% with 68% sensitivity.


### SMOTE 

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/SMOTEOversampling.png)

* The balanced accuracy score is 64%.
* The high risk precision is 1% with 63% sensitivity.
* the low risk precision is 100% with 66% sensitivity.


### ClusterCentroid 

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/ClusterCentroids%20Undersampling.png)

* The balanced accuracy score is 53%.
* The high risk precision is 1% with 61% sensitivity.
* the low risk precision is 100% with 45% sensitivity.


### SMOTEENN 

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/SMOTEENNOver_and_Under_SAMPLING.png)

* The balanced accuracy score is 62%.
* The high risk precision is 1% with 68% sensitivity.
* the low risk precision is 100% with 57% sensitivity.


### BalancedRandomForestClassifier 

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/BalancedRandomForestClassifier.png)

* The balanced accuracy score is 79%.
* The high risk precision is 4% with 67% sensitivity.
* the low risk precision is 100% with 91% sensitivity.


### EasyEnsembleClassifier 

![](https://github.com/EnoVaqari/Credit_Risk_Analysis/blob/main/IMG/EasyEnsembleClassifier.png)

* The balanced accuracy score is 93%.
* The high risk precision is 7% with 91% sensitivity.
* the low risk precision is 100% with 94% sensitivity.



## Summary.
While analyzing the credit card dataset from LendingClub, EasyEnsembleClassifier model generated the highest balanced accuracy score of 93%. All the other models had balanced accuracy scores under 80%. The EasyEnsembleClassifier model is the best option given the data and the results, but keeping in mind that due to low precision, many of the low risk credits will be inaccurately detected as high risk credits, which might be misleading for the banks.
