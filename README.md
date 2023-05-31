# Assessing Credit Risk: A Comparative Evaluation of Logistic Regression Models

![credit-risk](https://github.com/AnushDeCosta/ML-credit-risk-classification/assets/67308030/299d8a77-4dd8-43b8-8a3f-b621fee13496)

## Analysis Synopsis
The central aim of this analysis is to scrutinize the efficacy of two logistic regression machine learning models in forecasting the credit risk associated with various loans. This examination utilizes financial data, focusing specifically on elements such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The ultimate goal is to predict the loan status, segregating it either as a healthy loan (0) or a high-risk loan (1).

## Analysis Procedure
The following stages outline the machine learning process utilized in this analysis:

- **Data Division:** The dataset is bifurcated into training and testing datasets.
- **Model Formulation:** A logistic regression model is structured and tailored to the original data.
- **Model Evaluation:** The model's effectiveness is gauged using metrics such as accuracy, precision, and recall scores.
- **Data Resampling:** The RandomOverSampler is employed to resample the data and address class imbalance.
- **Model Formulation:** Another logistic regression model is formed and tailored to the resampled data.
- **Model Evaluation:** The effectiveness of the resampled model is gauged using identical metrics.
This analysis employs the methods of LogisticRegression and RandomOverSampler for resampling.
Results

## Machine Learning Model 1: Logistic Regression with Original Data
Model 1 yields an accuracy score of 0.9924, reflecting that it accurately classifies 99% of the instances. The model excels in identifying healthy loans (0) with a precision score of 0.9964, indicating minimal false positives. Nevertheless, the model's precision score for recognizing high-risk loans (1) is a moderate 0.8746, pointing to some false positives. The model's recall score for identifying healthy loans (0) is outstanding at 0.9957, indicating minimal false negatives. However, the recall score for recognizing high-risk loans (1) is only 0.8928, signifying some false negatives.

## Machine Learning Model 2: Logistic Regression with Resampled Data
Model 2 achieves a superior accuracy score of 0.9942, indicating that it accurately classifies 99% of the instances. The precision score for high-risk loans (1) has experienced a significant improvement to 0.9941 from the model utilizing the original data. However, the precision score for healthy loans (0) has experienced a slight decline to 0.9942 from 0.9964. Yet, overall the precision for identifying both healthy loans (0) and high-risk loans (1) is excellent with scores of 0.99, reflecting very few false positives. The model's recall score is superb for identifying both healthy loans (0) and high-risk loans (1) with scores of 0.99, indicating very few false negatives.

## Conclusion
In conclusion, the logistic regression model trained with resampled data (Model 2) surpasses the performance of the model using original data (Model 1), particularly in forecasting high-risk loans. The heightened precision and recall scores for high-risk loans with Model 2 are crucial in minimizing prospective financial losses for the lending company. Therefore, Model 2 is recommended for credit risk analysis. Its deployment will empower the company to effectively evaluate loan applications and make well-informed decisions, thus mitigating credit risk.

## Tools
- Python
- Pandas
- Numpy
- scikit-learn
- Jupyter Notebook

## Files
- [Machine Learning Model Script](./credit_risk_classification.ipynb)
- [Lending Data Set](./Resources/lending_data.csv)



