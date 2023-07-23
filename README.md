**credit-risk-classification**
Module 20 Challenge

#Background
    In this Challenge I used various techniques to train and evaluate a model based on loan
risk. It included a dataset of historical lending activity from a peer-to-peer lending services
company used to build a model that can identify the creditworthiness of borrowers.

#Split the Data into Training and Testing Sets
Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
Created the labels set (y) from the “loan_status” column and then created the features (X)
DataFrame from the remaining columns. Split the data into training and testing datasets by using
train_test_split.

#Create a Logistic Regression Model with the Original Data
-Fit a logistic regression model by using the training data (X_train and y_train).

-Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

-Evaluate the model’s performance by doing the following:

    Generate a confusion matrix.

    Print the classification report.

-Answered the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

#Write a Credit Risk Analysis Report
    Write a brief report that includes a summary and analysis of the performance of the machine
learning models that you used in this homework. The Analysis Report can be found in this github
repository. The report contains the following:

-An overview of the analysis.
-The results
-A summary

#Comments
Please see the Credit_Risk folder for the completed code and my full report. Thank you!
