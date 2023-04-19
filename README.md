# Credit Risk Analysis

# BootCamp - Module 20 Challenge

Student Name - Anush De Costa Module 20 Challenge Name - credit-risk-classification

# Overview of the Analysis

The goal of this analysis is to evaluate the performance of two logistic regression machine learning models in predicting the credit risk associated with loans. The analysis uses financial data, specifically focusing on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The objective is to predict the loan status, either as a healthy loan (0) or high-risk loan (1).

# Methodology

This analysis follows a machine learning process that includes the following stages:

- Data splitting: The data is split into training and testing datasets.
- Model creation: A logistic regression model is created and fitted with the original data.
- Model evaluation: The model's performance is evaluated using accuracy, precision, and recall scores.
- Data resampling: RandomOverSampler is used to resample the data to address class imbalance.
- Model creation: Another logistic regression model is created and fitted with the resampled data.
- Model evaluation: The performance of the resampled model is evaluated using the same metrics.
- The methods used in this analysis include LogisticRegression and RandomOverSampler for resampling.

# Results

## Machine Learning Model 1: Logistic Regression with Original Data

- Model 1 achieves an accuracy score of 0.9924, indicating that it correctly classifies 99% of the instances. Its precision score is excellent for identifying healthy loans (0) with a score of 0.9964, indicating very few false positives. However, the model's precision score for identifying high-risk loans (1) is only 0.8746, indicating moderate effectiveness with some false positives. The model's recall score is excellent for identifying healthy loans (0) with a score of 0.9957, indicating very few false negatives. However, the recall score for identifying high-risk loans (1) is only 0.8928, indicating effectiveness with some false negatives.

## Machine Learning Model 2: Logistic Regression with Resampled Data

- Model 2 achieves an improved accuracy score of 0.9942, indicating that it correctly classifies 99% of the instances. Its precision score for high-risk loans (1) has improved significantly to 0.9941 from the model using the original data while the healthy loans (0) have seen a slight fall to 0.9942 from 0.9964 but overall the precision is excellent for identifying both healthy loans (0) and high-risk loans (1) with scores of 0.99, indicating very few false positives. The model's recall score is excellent for identifying both healthy loans (0) and high-risk loans (1) with scores of 0.99, indicating very few false negatives.

# Conclusion

In conclusion, the logistic regression model trained with resampled data (Model 2) outperforms the original data model (Model 1), particularly in predicting high-risk loans. Its higher precision and recall scores for high-risk loans are essential in minimizing potential financial losses for the lending company. Therefore, it is recommended to use Model 2 for credit risk analysis, as it will enable the company to effectively assess loan applications and make informed decisions, mitigating credit risk.
