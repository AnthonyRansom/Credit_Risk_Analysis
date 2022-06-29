# Credit_Risk_Analysis
 
## Overview of Analysis

### Purpose

This analysis will look at various machine learning models that can be used to predict credit risk in order and compare the performance of each model in order to determine which machine learning model is best suited to predict credit risk.

## Results

The following provide a summary of the results of each machine learning model

### RandomOverSampler
![RandomOverSampler](/analysis/naive_random_oversampling.PNG)
 - The Naive Random oversampling model indicates an accuracy score of 65%
 - The Naive Random oversampling model indicates an average precision rate of  99%
 - The Naive Random oversampling model indicates an average recall rate of 58%

### SMOTE
![SMOTE](/analysis/SMOTE.PNG)

 - The SMOTE model indicates an accuracy score of 66%
 - The SMOTE model indicates an average precision rate of 99% 
 - The SMOTE model indicates an average recall rate of 68%

### ClusterCentroids
![ClusterCentroids](/analysis/cluster_centroids.PNG)

 - The Cluster Centroids model indicates an accuracy score of 54%
 - The Cluster Centroids model indicates an average precision rate of 99%
 - The Cluster Centroids model indicates an average recall rate of 40%

### SMOTEENN
![SMOTEENN](/analysis/SMOTENN.PNG)

 - The SMOTEENN oversampling model indicates an accuracy score of 64%
 - The SMOTEENN Random oversampling model indicates an average precision rate of 99% 
 - The SMOTEENN Random oversampling model indicates an average recall rate 59%
 
### BalancedRandomForestClassifier
![BalancedRandomForestClassifier](/analysis/balanced_random_forest.PNG)

 - The Balanced Random Forest Classifier model indicates an accuracy score of 79%
 - The Balanced Random Forest Classifier indicates an average precision rate of 99% 
 - The Balanced Random Forest Classifier indicates an average recall rate 87%
 
### EasyEnsembleClassifier
![EasyEnsembleClassifier](/analysis/Easy_Ensembler.PNG)

 - The Easy Ensemble AdaBoost Classifier model indicates an accuracy score of 93%
 - The Easy Ensemble AdaBoost Classifier model indicates an average precision rate of 99%
 - The Easy Ensemble AdaBoost Classifier model indicates an average recall rate 94%
 
## Results

### Summary of results - Accuracy
when comparing the various machine learning models the Easy Ensemble Classifier model showed the highest accuracy at a rate of 93% indicating 93% of the time the predictions the model made were correct when compared to the test data.

### Summary of results - Precision
All the models showed a 99% precision rate with each model showing a high precision rate but the precision rate is skewed when looking at the precision rate of low risk vs high risk with each model showing a high precision rate for low risk and a low precision rate for high risk.

### Summary of results - Recall
Looking at the recall rates of the various models it is again the Easy Ensemble Classifier that showed the highest average recall at a rate of 94% where 92% of the high risk predictions were correct compared to the testing data.

### Recommendation
For predicting credit risk it is more important to look at the recall rate as falsely predicting an application as low risk when it is actually high risk can result in the loss of money as the applicant may not pay back the credit that was provided. When looking at the accuracy and recall rates it is recommended to use the Easy Ensemble Classifier model as this machine learning model showed the highest accuracy and recall rate compared to all the other models