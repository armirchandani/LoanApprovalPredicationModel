# 🏦 Loan Approval Prediction System

A machine learning project that predicts whether a loan application will be approved using a **Support Vector Machine (SVM)** classifier. The project analyzes applicant demographic and financial information to identify patterns associated with loan approval decisions.

The project demonstrates the complete machine learning workflow, including data preprocessing, feature engineering, model training, and prediction on new applicant data.

---

## Table of Contents

1. Features
2. How It Works
3. Why It Matters
4. Tech Stack
5. Installation
6. Usage
7. Project Structure
8. Results
9. Future Improvements
10. Contributors

---

# Features

- **Data Preprocessing**
  - Cleaned missing values across applicant information
  - Applied logarithmic transformation to loan amount to reduce skewness
  - Encoded categorical variables into numerical values

- **Feature Engineering**
  - Processed applicant income, co-applicant income, credit history, education, and property area
  - Standardized applicant information for model training
  - Removed unnecessary identifiers such as Loan ID

- **Loan Approval Prediction**
  - Built a Support Vector Machine (SVM) classifier
  - Predicted whether a loan application would be approved or rejected
  - Generated predictions for new applicant information

- **Model Evaluation**
  - Split the dataset into **80% training** and **20% testing**
  - Evaluated model performance on unseen loan applications
  - Compared predicted loan status with actual outcomes

---

# How It Works

1. **Load Dataset**
   - Import loan application data containing demographic and financial attributes.

2. **Preprocess Data**
   - Handle missing values
   - Transform skewed numerical variables
   - Encode categorical features

3. **Train the Model**
   - Train a Support Vector Machine classifier using historical loan applications.

4. **Evaluate Performance**
   - Measure prediction accuracy on the testing dataset.

5. **Predict Loan Approval**
   - Input applicant information to determine the likelihood of loan approval.

---

# Why It Matters

Financial institutions review thousands of loan applications every year.

This project demonstrates how machine learning can:

- Support faster loan approval decisions
- Reduce manual review time
- Improve consistency in lending decisions
- Identify patterns in applicant financial profiles
- Assist banks in making data-driven lending decisions

---

# Tech Stack

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Machine Learning

- Support Vector Machine (SVM)

### Development Tools

- Jupyter Notebook
- Git
- GitHub

---

# Installation

Clone the repository

```bash
git clone https://github.com/armirchandani/LoanApprovalPredictionModel.git
cd LoanApprovalPredictionModel
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook LoanApprovalPredictionSystem.ipynb
```

---

# Usage

### Load the Dataset

```python
import pandas as pd

df = pd.read_csv("loan.csv")
```

### Train the SVM Model

```python
from sklearn import svm

model = svm.SVC(kernel="linear")
model.fit(X_train, Y_train)
```

### Predict Loan Approval

```python
prediction = model.predict(new_application)
```

---

# Project Structure

```
LoanApprovalPredictionModel/
│
├── loan.csv
├── LoanApprovalPredictionSystem.ipynb
├── README.md
└── requirements.txt
```

---

# Results

📊 Processed **614 loan applications** containing demographic and financial information

📈 Built a Support Vector Machine classifier for binary loan approval prediction

⚙️ Applied preprocessing techniques including missing value handling, categorical encoding, and logarithmic feature transformation

🏦 Successfully generated predictions for new loan applicants using financial and demographic features

---

# Future Improvements

- Compare SVM performance with Random Forest, XGBoost, and Logistic Regression
- Perform hyperparameter tuning using GridSearchCV
- Address class imbalance with SMOTE
- Build a Streamlit web application for real-time loan approval predictions
- Explain model decisions using SHAP or LIME for greater interpretability

---

# Contributors

**Aastha Mirchandani**

Business Analytics Student | University of San Francisco

Interested in Machine Learning, Financial Analytics, Data Science, and FinTech

---

⭐ If you found this project helpful, consider giving it a star!
