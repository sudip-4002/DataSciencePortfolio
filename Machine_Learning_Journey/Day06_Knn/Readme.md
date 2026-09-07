# KNN Classification Projects

This repository contains two supervised machine learning projects built using the **K-Nearest Neighbors (KNN)** algorithm.

---

## 📁 Project 1: Employee Attrition Prediction

Predicts whether an employee will leave the company (Attrition: Yes/No) using HR data.

### Dataset
- `WA_Fn-UseC_-HR-Employee-Attrition.csv`

### Workflow
1. **Data Understanding** – shape, dtypes, null check, duplicate check, target class distribution
2. **Data Cleaning** – dropped non-informative columns: `EmployeeCount`, `StandardHours`, `Over18`, `EmployeeNumber`
3. **Feature/Target Split** – `X` (features) and `y` (Attrition)
4. **Encoding**
   - Target encoded: `No → 0`, `Yes → 1`
   - Categorical features encoded using `pd.get_dummies()` (One-Hot Encoding)
5. **Train/Test Split** – 80/20 split, stratified on target
6. **Feature Scaling** – `StandardScaler`
7. **Class Imbalance Handling** – `SMOTE` (oversampling minority class) applied on training data only
8. **Model Building** – `KNeighborsClassifier`
9. **Hyperparameter Tuning** – tested K = 1 to 20 using 5-fold cross-validation, selected best K by F1-score
10. **Model Evaluation**
    - Accuracy, Precision, Recall, F1-score
    - Confusion Matrix
    - Classification Report
    - ROC Curve & ROC-AUC Score

### Libraries Used
`pandas`, `numpy`, `matplotlib`, `scikit-learn`, `imbalanced-learn (SMOTE)`

---

## 📁 Project 2: Breast Cancer Detection

Predicts whether a tumor is **Benign (B)** or **Malignant (M)** using diagnostic measurements.

### Dataset
- `breast-cancer-selected-columns.csv`

### Workflow
1. **Data Loading & Inspection** – shape, dtypes, null check, target class distribution
2. **Data Cleaning** – dropped `id` column (non-informative)
3. **Feature/Target Split** – `x` (features) and `y` (diagnosis)
4. **Encoding** – target encoded using `LabelEncoder` (`B → 0`, `M → 1`)
5. **Train/Test Split** – 80/20 split
6. **Feature Scaling** – `StandardScaler`
7. **Model Building** – `KNeighborsClassifier`
8. **Hyperparameter Tuning** – tested K = 1 to 20, selected best K by accuracy score
9. **Model Evaluation**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report (Benign vs Malignant)

### Libraries Used
`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

##  Common Algorithm: K-Nearest Neighbors (KNN)

A distance-based classification algorithm that predicts the class of a data point based on the majority class among its **K** nearest neighbors in feature space. Key steps common to both projects:

- Feature scaling (KNN is distance-sensitive, so scaling is mandatory)
- Choosing the optimal value of **K** via iteration + cross-validation/accuracy comparison
- Evaluating with confusion matrix, accuracy, precision, recall, and F1-score


Open the respective `.ipynb` file and run all cells in order.

##  Output
Each notebook prints final evaluation metrics and displays visualizations (confusion matrix, K-vs-score curve, ROC curve where applicable).