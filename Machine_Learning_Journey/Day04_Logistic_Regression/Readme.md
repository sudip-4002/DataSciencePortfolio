# Logistic Regression

Part of my Data Science & Machine Learning Journey, this section covers Logistic Regression, a supervised learning algorithm used for classification tasks. It includes two projects — one multiclass and one binary — implemented on real-world and built-in datasets.

## Concepts Covered

- Logistic Regression
- Binary & Multiclass Classification
- Sigmoid Function
- Train-Test Split
- Feature Scaling
- Model Training & Prediction
- Confusion Matrix
- Accuracy, Precision, Recall, F1-Score
- Classification Report

## Tech Stack

Python, Jupyter Notebook, NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn

---

## Projects

### 1. Iris Flower Classification

Classifies iris flowers into species using sepal/petal length and width, with the built-in Scikit-learn dataset.

```python
from sklearn.datasets import load_iris

X, y = load_iris(return_X_y=True, as_frame=True)
```

| | |
|---|---|
| **Algorithm** | Logistic Regression |
| **Problem Type** | Multiclass Classification |
| **Workflow** | Load Data → EDA → Preprocessing → Train/Test Split → Feature Scaling → Model Training → Prediction → Evaluation |

### 2. Titanic Survival Prediction

Predicts passenger survival using features like class, sex, age, fare, and family details from `titanic.csv`.

| | |
|---|---|
| **Algorithm** | Logistic Regression |
| **Problem Type** | Binary Classification |
| **Target** | `0` = Did Not Survive, `1` = Survived |
| **Workflow** | Load CSV → Data Cleaning → EDA → Feature Engineering → Encoding → Train/Test Split → Feature Scaling → Model Training → Prediction → Evaluation |

---

## Model Evaluation

Both models were assessed using Accuracy, Precision, Recall, F1-Score, the Confusion Matrix, and a full Classification Report.

## Key Takeaways

- Applied Logistic Regression to both multiclass (Iris) and binary (Titanic) problems.
- Practiced data preprocessing, categorical encoding, and feature scaling for classification.
- Learned to evaluate models using multiple performance metrics beyond accuracy.

---

