# Overview of the Analysis 

The goal of this investigation is to develop a supervised machine learning model that can classify loans as either high-risk (class 1) or healthy (class 0). For this model, the binary classifier used is logistic regression. The analysis was conducted on financial data, including information such as loan amount, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective was to predict whether a loan will be classified as high-risk (1) or healthy (0). The dataset used for this analysis is a CSV file containing 77,500 data points.

The stages of the machine learning process in this analysis included:

* Splitting data into labels and features, with the loan status (healthy or high-risk) as the label and the remaining seven columns as features.
* Splitting the data into training and testing datasets.
* Creating a Logistic Regression model from sklearn.
* Choosing Logistic Regression as a binary classifier since we are classifying loans as healthy OR high-risk.
* Training the model with the training data.
* Making predictions with the test data.
* Evaluating the model's performance using accuracy, precision, and recall scores.

# Results 

Description of Logistic Regression Model Accuracy, Precision, and Recall scores:

* Accuracy: 0.95
  
* Precision:

  * Healthy Loan (class 0): 1.00
  * High-Risk Loan (class 1): 0.85
    
* Recall:

  * Healthy Loan (class 0): 0.99
  * High-Risk Loan (class 1): 0.91

# Summary

With a precision of 1.00 and recall of 0.99, the logistic regression model is performing exceptionally well in predicting the healthy loans (class 0). The model continues to forecast risky loans (class 1) well, with a precision of 0.85 and recall of 0.91.

Given that the support test data for class 1 is just 619—a very low number when compared to 18,765 for class 0—the imbalanced dataset may be the source of the reduced precision and recall in forecasting the high-risk loans (class 1). Predicting high-risk loans could still use some work. Put another way, relative to the quantity of healthy loans in the data set, there are comparatively few high-risk loans for the model to learn from. The model might be improved if more high-risk loan examples were included in the training data.

In the process of classifying loans, preventing high-risk loans is more crucial than actually making loans, as the loss of money from a single default can be greater than the interest received. The model's overall accuracy is high, at 99%.
