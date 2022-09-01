# Credit_Risk_Analysis

## Overview of the analysis
In this project, we use Python to build and evaluate several machine learning models to predict credit risk.Basic the libraries for imbalanced-learn & scikit-learn we use the the model below

1. imbalanced-learn 
2. scikit-learn
3. RandomOverSampler
4. SMOTE algorithms
5. ClusterCentroids algorithm
6. SMOTEENN algorithm
7. BalancedRandomForestClassifier (bias reduction model)
8. EasyEnsembleClassifier (bias reduction model)


We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results

### RandomOverSampler
<img width="828" alt="image" src="https://user-images.githubusercontent.com/104603177/187822196-ca0e7a04-1ab7-4ce9-a805-a2aa7a192923.png">

The results are pretty similar to the previous model.
The balanced accuracy score is 65%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 59%. 

### SMOTEENN
<img width="881" alt="image" src="https://user-images.githubusercontent.com/104603177/187822710-c0fb7f8d-de55-47b0-9425-09e1a5080f04.png">

The balanced accuracy score is about 65%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 64%. 

### Balanced Random Forest Classifier
<img width="940" alt="image" src="https://user-images.githubusercontent.com/104603177/187823427-13d977d9-f6d2-4e6c-a6a0-70f3a610bdaf.png">
The balanced accuracy score is about 79%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 7%.
Due to the high number of false positives, the low_risk sensitivity is 91%. 



## Summary

When working with balanced accuracy, the highest compared accuracy between 0 and 1 and is closest to 1 is the best machine learning model.  For the credit card data set, the Easy Ensemble AdaBoost Classifier is the best model to choose with its .93 balanced accuracy.  The other models were below .80 balanced accuracy.  The precision for all models were similar and within an appropriate range.  The recall score also needs to fall within 0 and 1, with numbers closer to 1 being the better model.  The Easy Ensemble AdaBoost Classifier had the highest recall score, making it the final best machine learning model to choose for further credit card analysis.   
