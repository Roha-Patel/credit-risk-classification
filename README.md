# Overview of the Analysis 

The purpose of this analysis is to create a supervised machine learning model that will predict if a loan is healthy (class 0) or high-risk (class 1). Logistic regression is used as a binary classifier for this model. The analysis was conducted on financial data, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective was to predict the loan status, either as a healthy loan (0) or a high-risk loan (1). The data used is a 77,500-line CSV file.

The stages of the machine learning process in this analysis included:

Splitting data into labels and features, with the loan status (healthy or high-risk) as the label and the remaining seven columns as features.
Splitting the data into training and testing datasets.
Creating a Logistic Regression model from sklearn.
Choosing Logistic Regression as a binary classifier since we are classifying loans as healthy OR high-risk.
Training the model with the training data.
Making predictions with the test data.
Evaluating the model's performance using accuracy, precision, and recall scores.

# Results 

Description of Logistic Regression Model Accuracy, Precision, and Recall scores:

Accuracy: The overall accuracy of the model is 0.99, indicating that it correctly classifies 99% of the instances.

Precision:

Healthy Loan (class 0): 1.00
High-Risk Loan (class 1): 0.85
Recall:

Healthy Loan (class 0): 0.99
High-Risk Loan (class 1): 0.91

# Summary

The logistic regression model is performing very well in predicting healthy loans (class 0), with a precision of 1.00 and a recall of 0.99. For high-risk loans (class 1), the model is also doing a good job, with a precision of 0.85 and a recall of 0.91.

The lower precision and recall in predicting the high-risk loans (class 1) could be due to the imbalanced dataset, as the testing data for class 1 only has 619 instances, compared to 18,765 for class 0. This suggests that the model has fewer examples of high-risk loans to learn from, which may limit its performance in this class.

For loan classification, preventing high-risk loans is more important than approving healthy loans, as a single defaulted loan can result in greater financial losses than the interest earned from a healthy loan. The overall high accuracy of 99% indicates that this model is a strong candidate for use in credit risk classification.
