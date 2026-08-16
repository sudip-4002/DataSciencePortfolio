# Day 02 — Supervised Machine Learning


## Overview

Supervised Learning is one of the main types of Machine Learning.

In Supervised Learning, a Machine Learning model learns from a dataset where the **input data and correct output (target)** are already known.

The model learns the relationship between the input features and the target and then uses this learned relationship to make predictions on new, unseen data.

---

## Learning Objectives

By completing Day 02, I learned:

* What Supervised Learning is
* How Supervised Learning works
* What features and targets are
* What labeled data means
* The difference between Classification and Regression
* Real-world applications of Supervised Learning
* Common Supervised Learning algorithms

---

# What is Supervised Learning?

**Supervised Learning is a type of Machine Learning where a model learns from labeled training data to predict an output for new data.**

In simple words:

> We give the model inputs along with their correct answers, and the model learns the relationship between them.

### Example

Suppose we want to predict whether an email is spam.

| Email Features                    | Correct Answer |
| --------------------------------- | -------------- |
| Promotional words, unknown sender | Spam           |
| Normal conversation               | Not Spam       |
| Advertisement message             | Spam           |

The model learns from these examples and later predicts whether a new email is **Spam** or **Not Spam**.

---

# 🧩 How Supervised Learning Works

The basic process is:

```text
Labeled Dataset
      ↓
Data Preparation
      ↓
Features (X) + Target (y)
      ↓
Train/Test Split
      ↓
Choose ML Algorithm
      ↓
Train Model
      ↓
Model Learns Patterns
      ↓
Make Predictions
      ↓
Evaluate Model
```

---

# Features and Target

Two important concepts in Supervised Learning are **Features** and **Target**.

## Features (X)

Features are the input variables used by the model to make predictions.

For example, when predicting house prices:

```text
House Size
Number of Bedrooms
Number of Bathrooms
Location
Age of House
```

These are the **features (X)**.

## Target (y)

The target is the output that the model is trying to predict.

For the house price example:

```text
House Price
```

is the **target (y)**.

Therefore:

```text
X = Input Features
y = Target / Output
```

---

# What is Labeled Data?

Labeled data is data where the correct output is already provided.

Example:

| Hours Studied | Attendance | Result |
| ------------: | ---------: | ------ |
|             2 |        60% | Fail   |
|             5 |        75% | Pass   |
|             8 |        90% | Pass   |

Here:

```text
Hours Studied + Attendance → Features
Result → Target
```

Because the correct result is already known, this is **labeled data**.

---

# Types of Supervised Learning

Supervised Learning is mainly divided into two categories:

```text
Supervised Learning
│
├── Regression
│
└── Classification
```

---

# Regression

Regression is used when the target is a **continuous numerical value**.

### Examples

* Predicting house prices
* Predicting salary
* Predicting temperature
* Predicting sales
* Predicting stock prices

### Example

```text
Input:
House Size = 1500 sq.ft
Bedrooms = 3
Location = Kathmandu

Output:
Predicted Price = Rs. 18,000,000
```

The output is a numerical value.

### Common Regression Algorithms

* Linear Regression
* Polynomial Regression
* Decision Tree Regressor
* Random Forest Regressor
* Support Vector Regression
* Gradient Boosting Regressor

---

# Classification

Classification is used when the target belongs to a **category or class**.

### Examples

* Spam or Not Spam
* Pass or Fail
* Disease or No Disease
* Fraud or Not Fraud
* Cat, Dog, or Bird

### Example

```text
Input:
Email Content

Output:
Spam
```

The output belongs to a category.

### Common Classification Algorithms

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)
* Naive Bayes

---

# Regression vs Classification

| Feature          | Regression               | Classification      |
| ---------------- | ------------------------ | ------------------- |
| Purpose          | Predict numerical values | Predict categories  |
| Target           | Continuous               | Categorical         |
| Example          | House Price              | Spam/Not Spam       |
| Output           | 2500000                  | Spam                |
| Common Algorithm | Linear Regression        | Logistic Regression |

---

# Real-World Applications

Supervised Learning is widely used in real-world applications.

### Banking

Predict whether a customer is likely to repay a loan.

### Email

Classify emails as spam or legitimate.

### Real Estate

Predict house prices.

### Healthcare

Predict disease categories based on patient information.

### E-Commerce

Predict whether a customer will purchase a product.

### Education

Predict student performance or pass/fail outcomes.

---

# Common Supervised Learning Algorithms

| Algorithm           | Type                        |
| ------------------- | --------------------------- |
| Linear Regression   | Regression                  |
| Logistic Regression | Classification              |
| KNN                 | Classification / Regression |
| Decision Tree       | Classification / Regression |
| Random Forest       | Classification / Regression |
| SVM                 | Classification / Regression |
| Naive Bayes         | Classification              |

---

# Simple Example

Suppose we have student data:

```text
Hours Studied → Exam Score
```

Training data:

```text
2 hours → 45
4 hours → 60
6 hours → 72
8 hours → 85
```

The model learns the relationship between study hours and exam scores.

If we give:

```text
7 hours
```

the model may predict:

```text
Exam Score ≈ 78
```

This is **Supervised Learning → Regression** because the target is a numerical value.

---

# Key Takeaways

1. Supervised Learning learns from labeled data.
2. Features are the input variables.
3. The target is the output the model predicts.
4. Training data contains known input-output relationships.
5. Supervised Learning is mainly divided into Regression and Classification.
6. Regression predicts continuous numerical values.
7. Classification predicts categories or classes.
8. The choice of algorithm depends on the type of problem.
9. Supervised Learning is widely used in real-world applications.



