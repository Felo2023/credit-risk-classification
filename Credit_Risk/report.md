# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

Purpose:
By using a dataset of historical lending activity from a peer-to-peer lending services company, we will identify the creditworthiness of borrowers.

Financial information:
The dataset contained the following parameters:
  Loan size 
  Interest rate 
  Borrower income 
  Debt to income
  Number of accounts
  Derogatory marks
  Total debt
  Loan status
We required to predict if the creditworthiness of burrowers by identifying if they were a high risk loan (1 - Loan status) or were a healthy loan (0-Loan status). 

Process:

Step 1 =  Load the dataset and splitting it into "labels (y)" and "features (X)"
Step 2 = Splitting labels and features on test and train samples using "train_test_split"
Step 3 = Create a "classifier" using "LogisticRegression(solver='lbfgs', random_state=1)"
Step 4 = Review accuracy score

In order to improve our model we used the random over sampler and repeated step 3 and 4.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:


Classification Report
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

Classification Report
              precision    recall  f1-score   support

           0       0.99      0.99      0.99     75036
           1       0.99      0.99      0.99     75036

    accuracy                           0.99    150072
   macro avg       0.99      0.99      0.99    150072
weighted avg       0.99      0.99      0.99    150072



## Summary

I would recommend to use model 1 since the accuracy on the the healthy loan was perfect. We want to make sure that we dont give a loan to a customer that will have difficulties and could actually be a high risk for the company.