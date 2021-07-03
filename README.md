# Credit_Risk_Analysis

UT Bootcamp Module 17 Challenge

## Project Overview
Create a machine learning model and analysis using different sampling techniques and the imbalanced-learn and scikit-learn libraries on the credit risk dataset from LendingClub by:
1. Oversampling the data using the RandomOverSampler and SMOTE algorithms
2. Undersampling the data using the ClusterCentroids algorithm
3. Oversampling and undersampling the data using the SMOTEEN algorithm
4. Comparing the two models that reduce bias to predice risk: BalancedRandomForestClassifier and EasyEnsembleClassifier
5. Evaluate the performance of the models and their efficiency in predicting risk 

## Resources
Data Sources provided to analyze and minipulate included:
- LoanStats_2019Q1.csv

Software utilized for this study included: 
- Python 3.7.6 
- Conda 4.9.2 
- Jupyter Notebook 6.1.4
- Personal GitHub account

## Analysis and Workflow
The general workflow in running these models are to :
1. Read and clean the data
2. Split the data into training and testing
3. Resample the data according to the algorithm method (SMOTE, Naive Random, Undersampling, etc.)
4. Run the confusion matrix and show statistical results

### Deliverable 1: Resampling Models to Predict Credit Risk

Specifically for this deliverable we did the following:
1. Create the training variables by converting the string values into numerical ones using the get_dummies() method.
2. Create the target variables.
3. Check the balance of the target variables.
4. Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
5. Calculate the accuracy score of the model.
6. Generate a confusion matrix.
7. Print out the imbalanced classification report (see below).

Naive Random Oversampling:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_1a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_1.PNG)

SMOTE Oversampling:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_2a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_2.PNG)

Undersampling:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_3a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli1_3.PNG)

### Deliverable 2: Use the SMOTEEN algorithm to Predict Credit Risk

Specifically for this deliverable we did the following:
1. Use the credit_risk_resampling.ipynb file to create your training and target variables.
2. Resample the training data using the SMOTEENN algorithm.
3. Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
4. Calculate the accuracy score of the model.
6. Generate a confusion matrix.
7. Print out the imbalanced classification report (see below).

SMOTEEN - Combination (Over and Under) Sampling:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli2_1a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli2_1.PNG)


### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Specifically for this deliverable we did the following:
1. Create the training variables by converting the string values into numerical ones using the get_dummies() method.
2. Create the target variables.
3. Check the balance of the target variables.
4. Resample the training data using the BalancedRandomForestClassifier algorithm with 100 estimators.
5. Calculate the accuracy score of the model
6. Generate a confusion matrix
7. Print out the imbalanced classification report (see below).

Balanced Random Forest Classifier:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli3_1a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli3_1.PNG)

9. Print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
10. Resample the training data using the EasyEnsembleClassifier algorithm with 100 estimators.
11. Calculate the accuracy score of the model
12. Generate a confusion matrix
13. Print out the imbalanced classification report (see below).

Easy Ensemble Classifier:
![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli3_2a.PNG)

![alt text](https://github.com/austin020269/Credit_Risk_Analysis/blob/main/Deli3_2.PNG)
