# Module 12 Report Template

## Overview of the Analysis

In this project, I used various techniques to train and evaluate a model based on loan risk. The dataset used contains historical lending activity from a peer-to-peer lending services company. I built a model that can identify the creditworthiness of borrowers.

The purpose of the analysis is to classify loans as either Healthy or High-Risk< The data provided contained information on the follwoing features

1. Loan size	
2. Interest rate	
3. Borrower income	
4. Debt to income ratio
5. Number of accounts	
6. Derogatory marks	
7. Total debt	
8. Loan status (Healthy or High-Risk)

Using features numbered 1-7 above, the model will predict loan status.

The initial data file was clean and no pre-processessing was needed. Using Python the outcome (loan status) was separated from the rest of the dataframe. The data was then split into training and test data sets using the sklearn train_test_split method. The model was initialized using sklearn LogisticRegression and the training data was fit to the model. The model predictions were found using classifier.predict method and saved. To check the performnce of the model, a confusion matrix and classification report were obtained using the confusion_matrix and classification_report functions.

## Results

* The classification report shows that the model has an accuracy of 0.99 which shows a very high ratio of correctly predicted oberservations to the total number of observations.

* For Healthly Loans, the precison is 1.0 which means all predicted Healthy Loans were actually Healthy Loans. The recall is also 1.0 which means all of the actual Healthy Loans were predicted correctly.

* For High Risk Loans, the precison is 0.87 which means 87% of predicted High Risk Loans were actually High Risk Loans. The recall is 0.89 which means 89% of the actual High Risk Loans were predicted correctly.

## Summary

Given the high accuracy, precision and recall scores, I would recomend the use of this model witht he caveat that there may be errors of 10-13% on identifying High-Risk Loans. If this is not acceptable, then I would first recommend addressing the imbalance of Healthy (~7500) to High-Risk (~2500) in the dataset. 
