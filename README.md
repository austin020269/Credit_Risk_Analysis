# Credit_Risk_Analysis

UT Bootcamp Module 17 Challenge

## Project Overview
Create a machine learning model abd analysis using different sampling techniques and the imbalanced-learn and scikit-learn libraries on the credit risk dataset from LendingClub by:
1. Oversampling the data using the RandomOverSampler and SMOTE algorithms
2. Undersampling the data using the ClusterCentroids algorithm
3. Oversampling and undersampling the data using the SMOTEEN algorithm
4. Comparing the two models that reduce bias to predice risk: BalancedRandomForestClassifier and EasyEnsembleClassifier
5. Evaluate the performance of the models and their effieciency in predicting risk 

## Resources
Data Sources provided to analyze and minipulate included:
- LoanStats_2019Q1.csv data file

Software utilized for this study included: 
- Python 3.7.6 
- Conda 4.9.2 
- Jupyter Notebook 6.1.4
- Personal GitHub account

## Analysis and Workflow 
### Deliverable 1: Linear Regression to Predict MPG (Six variables used - vehicle length, vehicle weight, spoiler angle, ground clearance, AWD and mpg) 
1. Use the library() function to load the dplyr package.
2. Import and read in the MechaCar_mpg.csv file as a dataframe.
3. Perform linear regression using the lm() function and pass in all six variables (i.e., columns), and add the dataframe you created to the data parameter.
4. Using the summary() function, determine the p-value and the r-squared value for the linear regression model. 

![alt text](https://github.com/austin020269/MechaCar_Staistical_Analysis/blob/main/Deli_1_Image_1.PNG)

### Linear Regression to Predict MPG (Analysis)
For this deliverable we are asked to provide answers to the following questions:
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Variables that show lower p-values provide a non-random amount of variance and have the greatest significance.  These would be the vehicle length and the ground clearance.
- Is the slope of the linear model considered to be zero? Why or why not?
The slope is of the linear regression is not considered to be zero because of the effect the independent veriables have on the depandent variable. 
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
This linear model does predict the prototypes reasonably well as it has an R-squared value is 0.7149, which means it is correct approximateky 71% of the time. 

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
