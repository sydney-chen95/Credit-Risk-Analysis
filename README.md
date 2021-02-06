# Credit-Risk-Analysis

## Overview

Credit risk is a challenge that machine learning can help resolve. In this project, we will employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries.


## Results 

The credit card credit dataset is from LendingClub. I oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

#### Naive Random Oversampling
![Naive Random Oversampling](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/Naive%20Random%20Oversampling.png?raw=true)

- The random oversamping method resulted in a balanced accuracy score of: 0.64.
- For high risk applications, this resulted in a precision score of 0.01 and a recall score of 0.66.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.62.

#### SMOTE
![SMOTE Oversampling](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/SMOTE%20Oversampling.png?raw=true)

- The SMOTE oversamping method resulted in a balanced accuracy score of: 0.65.
- For high risk applications, this resulted in a precision score of 0.01 and a recall score of 0.61.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.69.

#### Cluster Centroid
![Cluster Centroid](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/Cluster%20Centroid.png?raw=true)

- The Cluster Centroid method resulted in a balanced accuracy score of: 0.54.
- For high risk applications, this resulted in a precision score of 0.01 and a recall score of 0.68.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.41.

#### Combination (Over and Under)
![SMOTEENN](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/SMOTEENN.png?raw=true)

- The SMOTEENN method resulted in a balanced accuracy score of: 0.64.
- For high risk applications, this resulted in a precision score of 0.01 and a recall score of 0.71.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.57.

#### Balanced Random Forest
![Balanced Random Forest](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/Balanced%20Random%20Forest.png?raw=true)

- The Balanced Random forest Classifier method resulted in a balanced accuracy score of: 0.78.
- For high risk applications, this resulted in a precision score of 0.03 and a recall score of 0.70.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.87.

#### Easy Ensemble Classifier
![Easy Ensemble Classifier](https://github.com/sydney-chen95/Credit-Risk-Analysis/blob/main/images/Easy%20Ensemble%20Classifier.png?raw=true)

- The Easy Ensemble Classifier method resulted in a balanced accuracy score of: 0.93.
- For high risk applications, this resulted in a precision score of 0.09 and a recall score of 0.92.
- For low risk applications, this resulted in a precision score of 1.00 and a recall score of 0.94.


## Summary 

In conclusion, the Easy Ensemble Classifier had the best balanced accuracy score of 0.93. This method also had the best precision and recall scores for both high and low risk applications. I would recommend using this model. 
