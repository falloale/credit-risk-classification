# credit-risk-classification

# Module 20 Report 

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers.
A dataset of historical lending activity from a peer-to-peer lending services company was used.
Dependant variable (y value) in this analysis was the "loan status" indicating if a loan is healthy or at risk.
Independent Variables (x values) were loan size, interest rate, borrower income, debt to income ratio, number of accounts and derogatory marks.
In this analysis, we first split our data to traning and test sets. Then, define our dependent and independent variables. Next, we create logistic regression model and fit our original data to this model. Trained model is used to make predictions. Lastly, we evaluate the models performance.
Two diffeent Logistic Regression models were created by using the original data set and randomy over resampled data set (to get rid of the imbalances). In the end, their results -which was gathered with scikit-learn library- were compared.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: Original Data
  * Description of Model 1 Accuracy, Precision, and Recall scores.
<img width="379" alt="Screenshot 2023-05-24 at 7 14 42 PM" src="https://github.com/falloale/credit-risk-classification/assets/119981413/79129b8a-4673-430e-b1b8-ce12fe1d093b">

![Screenshot 2023-05-24 at 7 17 10 PM](https://github.com/falloale/credit-risk-classification/assets/119981413/afc02431-64c4-48e2-b3f6-4cca8e93851f)



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

![Screenshot 2023-05-24 at 7 21 17 PM](https://github.com/falloale/credit-risk-classification/assets/119981413/eeec667a-1268-4b5b-9adc-e20e89bb22a4)


![Screenshot 2023-05-24 at 7 18 24 PM](https://github.com/falloale/credit-risk-classification/assets/119981413/18b0a800-d3be-41c4-9a48-0287464e19b9)



## Summary

Analysis show that collected data can be effectively used to train and test the Machine Learning Classification Model. For better preditions solving the imbalance sampling issue is needed.

Randomly oversampling the data helps us to get higher balanced accuracy and recall scores. With higher recall value, model can predict risky loans more accurately.

With incorrect predictions we have two issues:

False positives (where users are flagged as risky, but are actually healthy)
False negatives (where users are not flagged as risky but are actually risky)

both cases have its costs. It is important to predict both 1s and 0s. Therefore, model should have good accuracy in terms of both.
