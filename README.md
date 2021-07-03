# Credit_Risk_Analysis

UT Bootcamp Module 17 Challenge

## Project Overview
Create a machine learning model abd analysis using different sampling techniques and the imbalanced-learn and scikit-learn libraries on the credit risk dataset from LendingClub by:
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
The general process in running the models is to :
1. Read and clean the data
2. Split the data into training and testing
3. Sample the data according to the method
4. Run the confusion matrix and show results

### Deliverable 1: Resampling Models to Predict Credit Risk

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_1_Image.PNG)

### Deliverable 2: Summary Statistics on Suspension Coils
1. Download the Suspension_Coil.csv file, and place it in the active directory for your R session.
2. In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.
3. Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
4. Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column.

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_2_Image_1.PNG)

total_summary dataframe:

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_2_Image_2.PNG)

lot_summary dataframe:

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_2_Image_3.PNG)

## Summary Statistics on Suspension Coils (Analysis)
Whether or not the lots meet the design specifications can be answered by looking at the variance as a total and individually and can be seen in both dataframes.  As a whole, the total_summry table shows that they do with the variance of 76, which is within our tolerance of < 100.  Individually, Lots 1 and 2 meet this requirement, however Lot 3 does not.  

### Deliverable 3: T-tests on Suspension Coils
1. In your MechaCarChallenge.RScript, write an RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
2. Next, write three more RScripts in your MechaCarChallenge.RScript using the t.test() function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_3_Image_1.PNG)

All manufacturing lots (all cars):

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_3_Image_2.PNG)

Test 1 (Lot 1):

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_3_Image_3.PNG)

Test 2 (Lot 2):

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_3_Image_4.PNG)

Test 3 (Lot 3):

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_3_Image_5.PNG)



### Deliverable 4: Study Design: MechaCar vs Competition (Analysis)
For this deliverable we are asked to provide answers to the following questions:
- What metric or metrics are you going to test? City and Highway fuel economy.
- What is the null hypothesis or alternative hypothesis? The null is that they all have the same fuel economy vs the alternative is that they are different.
- What statistical test would you use to test the hypothesis? And why? An ANOVA test because it is a good way of testing the significance of the experimental results.
- What data is needed to run the statistical test? At least a population of 50-100 cars to get a good respresentation of all cars.
