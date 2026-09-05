Customer Churn Prediction Using Logistic Regression

Overview

This project predicts whether a telecom customer will churn using Logistic Regression.

Dataset

Telco Customer Churn dataset with customer information such as:

Tenure

Contract

Internet Service

Monthly Charges

Total Charges

Payment Method

Churn

Technologies

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

Machine Learning Workflow

Data Collection
      ↓
Data Cleaning
      ↓
EDA
      ↓
Feature Encoding
      ↓
Train-Test Split
      ↓
Feature Scaling
      ↓
Logistic Regression
      ↓
Model Evaluation

Preprocessing

Converted TotalCharges to numeric

Handled missing values

Applied one-hot encoding

Applied feature scaling using StandardScaler

Model Performance

Metric

Score

Accuracy

77.97%

Precision

69.75%

Recall

30.21%

F1 Score

42.16%

Project Structure

Customer-Churn-Logistic-Regression/
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── Customer_Churn_Logistic_Regression.ipynb
├── README.md
└── requirements.txt

How to Run

pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook

Open Customer_Churn_Logistic_Regression.ipynb and run the cells sequentially.

Conclusion

This project demonstrates a complete basic machine learning workflow for predicting customer churn using Logistic Regression.