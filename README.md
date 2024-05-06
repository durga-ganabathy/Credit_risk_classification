# Credit_risk_classification

# Credit Risk Analysis Report

## Overview of the Analysis


### Purpose of the analysis:
The primary purpose of the analysis is to build a machine learning model that can identify the creditworthiness of borrowers and classify the borrowers into categories such as "Healthy Loan" or "High Risk Loan" based on their attributes and historical performance. This predictive capability is crucial for financial institutions to assess the risk associated with loans and make informed lending decisions. Ultimately, the goal is to enhance effective lending process.


* The analysis used a dataset of historical lending activity from a peer-to-peer lending services company. The financial data has loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, loan status. The task was to predict the loan status, categorized as "Healthy Loan" (0) or "High Risk Loan" (1), based on these financial attributes.

*  Based on the financial factors the model aims to assess whether a borrower is likely to belong to the "Healthy Loan" category or the "High Risk Loan" category. Used value_counts() to gain insights into the distribution of loan statuses and assess the balance between different classes, which is crucial for building and evaluating predictive models for loan risk analysis.

* Stages of the machine learning process:
 1. Read the data and converted into the pandas dataframe.

 2. Created the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

3. Split the data into training and testing datasets by using train_test_split.

4. Fit a logistic regression model by using the training data (X_train and y_train). 

5. Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. 

6. Evaluate the model’s performance by doing the following:
   Generate a confusion matrix.
   Print the classification report.


* Methods used:
This analysis uses Logistic Regression. It models the probability that an instance belongs to a particular class using the logistic function. Logistic regression is a statistical method for predicting binary outcomes from data. 

Steps in Logistic regression : Preprocess, Train, Validate and Predict


## Results
1. For "Healthy Loan (0)" - 
   Precision: 1.00
   Recall: 1.00
   F1-score: 1.00

2. For "High Risk Loan (1)" - 
   Precision: 0.87
   Recall: 0.95 
   F1-score: 0.91

Precision is the ratio of correctly predicted positive observations to the total predicted positive observations. 

Recall is the ratio of correctly predicted positive observations to all predicted observations for that class. 

Accuracy is how often the model is correct—the ratio of correctly predicted observations to the total number of observations. 

 ## Summary  
* Class 0 healthy loan model (100%) has a perfect precision, recall and f1 score. This suggests that there is no false positive or false negative. All instances predicted as "Healthy Loan" are indeed "Healthy Loan", and the model correctly identifies all "Healthy Loan" instances. High precision relates to a low false positive rate. High recall correlates to a more comprehensive output and a low false negative rate.

* Class 1 high risk loan model has a slightly low value compared to the healthy loan model. The precision of 0.87, suggests that 87% of the instances predicted as "High Risk Loan" are actually "High Risk Loan". The recall of 0.95 indicates that the model identifies 95% of the actual "High Risk Loan" instances correctly. The f1-score 91% reflects a balance between precision and recall for this class.

* Overall, the accuracy of this logistic regression model is 99%. This demonstrates a strong predicting performance for Healthy loans and a effective performance in identifying high risk loans.







