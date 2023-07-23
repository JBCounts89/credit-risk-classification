# Module 12 Report 

## Overview of the Analysis

The model included data on the following:  
-size of the loan  
-interest rate  
-borrower's income  
-debt/income ratio  
-number of borrower held accounts  
-derogatory marks against the borrower  
-total debt

To conduct this analysis the data was initially split into two different sets, training and
testing. I used the training set to build a logistic regression model from the scikit-learn
LogisticRegression module. I then applied this model to the testing dataset to determine whether
a borrower's loan would be low or high risk. Please see the results below for a summary.

The dataset for this initial model drew on 75,036 low risk and 2500 high risk data points.
Following this initial model the training data was resampled with the RandomOverSampler from
imbalanced-learn. This generated a similar large quantity of low and high risk loans from the
original dataset and was used to build a new, oversamplled logistic regression model. Finally
this new logistic regression model was used to calculate whether a borrower's loan in
the testing set would qualify as low or high risk. Please see the results below for a summary.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:  
  Precision: 93% (The model was 100% precise in predicting low risk loans but 87% in predicting               high risk loans, making 93% the average)  
  Accuracy: 94%  
  
  Recall: 95% (The model was 100% precise in predicting low risk loans but 89% in predicting high          risk loans, making 95% the average)


* Machine Learning Model 2:  
  Precision: 93% (The model was 100% precise in predicting low risk loans but 87% in predicting               high risk loans, making 93% the average)  
  Accuracy: 100% (overfit)  
  
  Recall: 100% (overfit)

## Summary

Ultimately I would contend that the purpose of this analysis is to accurately determine the
risk in making high-risk loans due to their higher rates of interest. On this point neither model 
scores above 90% precision, which when considered against other factors (such as the lending
institution's debt ratios and overall balance sheet) suggests that another model should be sought.
However, in the event these models were the only options the second model possessed higher recall
and accuracy scores that suggest it would be the better choice.
