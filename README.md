# Credit Risk Classification Analysis Report

## Overview

The purpose of this analysis was to use historical data on loan/lending activity and test a supervized learning model used to find the creditworthiness of borrowers. The features set used for this analysis included the following: 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income', 'num_of_accounts', 'derogatory_marks', 'total_debt'. From the given features the model was meant to predict 'loan_status' where 0 represents a Healthy Loan and 1 represents a High-Risk Loan. 

In order to analyze the model, data was split between training and testing data for both the features set (X) and the label set (y). With the given training and testing sets a Logistic Regression classifier was created and fit with the X and y training data. Once trained the classifier was made to predict loan status based on the X testing data. 

## Results

Model classification report scores: 
* Precision:
    * Healthy loan 1.00
    * High-Risk loan .87
* Recall:
    * Healthy loan 1.00
    * High-Risk loan .89
* Overall Accuracy: .99

## Summary

While the overall accuracy of this model shows to be very high, the independent precision and recall scores for the high-risk loans are not ideal. The precision score evaluates what percent of instances classified as positive were correct. The recall score evaluates all instances that were true positives and tells what percent were idenitfied as such. 

Within this model incorrectly identifing borrowers has costly consequences, especially those within the high-risk category. For this reason I would not recommend the model for use until the precision and recall scores for both healthy and high-risk has surpassed at least 98%.  

## References

This assignment was completed individually with code guided by in class examples and lecture material. Data for this assignment was provided by EdX. 

Further information on classification reports can be found at https://www.scikit-yb.org/en/latest/api/classifier/classification_report.html 