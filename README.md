# Titanic Survival Prediction using Machine Learning

## 📌 Overview

This project applies supervised machine learning techniques to predict passenger survival on the Titanic dataset. The goal is to analyze passenger attributes and build a classification model capable of predicting survival outcomes.

The project demonstrates data preprocessing, feature engineering, model training, and evaluation using multiple performance metrics.

---

## 📊 Dataset

- Source: Kaggle – Titanic: Machine Learning from Disaster
- Data Set Link: " https://www.kaggle.com/datasets/amineipad/titanic-dataset?select=test.csv "
- Training Records: 891
- Features: 12 original attributes
- Target Variable: Survived (0 = No, 1 = Yes)

---

## 🧹 Data Preprocessing

- Handled missing values:
  - Age → Median imputation
  - Fare → Median imputation
  - Embarked → Mode imputation
- Dropped high-missing or irrelevant features (Cabin, Ticket, Name)
- Created new feature:
  - **FamilySize = SibSp + Parch**
- Applied One-Hot Encoding to categorical variables
- Aligned training and testing feature columns

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights:

- Female passengers had significantly higher survival rates (~74%) than males (~19%)
- 1st class passengers had better survival probability
- Higher fare correlated positively with survival
- Smaller family sizes showed improved survival chances

---

## 🤖 Model Used

### Logistic Regression

Why Logistic Regression?

- Suitable for binary classification
- Interpretable coefficients
- Strong baseline performance for structured datasets

---

## 📈 Model Evaluation

- Train-Test Split: 80% / 20%
- Accuracy: **81%**
- Confusion Matrix:
  - True Positives: 55
  - True Negatives: 90
  - False Positives: 15
  - False Negatives: 19

### Additional Metrics:
- Precision
- Recall
- F1-score

---

## 🧠 Key Learnings

- Importance of feature engineering (FamilySize improved prediction)
- Handling missing data improves model reliability
- Accuracy alone is not sufficient for evaluating classification models
- Correlation analysis helps identify influential predictors

---

## 🚀 Future Improvements

- Compare with Random Forest and XGBoost
- Perform hyperparameter tuning using GridSearchCV
- Add cross-validation
- Deploy model using Streamlit

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## 📂 Project Structure
