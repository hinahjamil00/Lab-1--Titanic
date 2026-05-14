# 🚢 Titanic Survival Prediction (Machine Learning Project)

This project is a complete end-to-end **data analysis and machine learning pipeline** built on the famous Titanic dataset. The goal is to predict whether a passenger survived or not based on their personal and travel-related features.

---

## 📌 Project Overview

- Dataset: Titanic (Train + Test)
- Target Variable: `Survived`
- Problem Type: **Binary Classification**
- Approach: Data Cleaning → EDA → Feature Engineering → ML Model → Evaluation

---

## 📊 Steps Performed

### 1. Data Preparation
- Combined train and test datasets
- Handled missing values:
  - Age → median imputation
  - Fare → median imputation
  - Embarked → mode imputation
  - Cabin → dropped due to high missing values

---

### 2. Feature Engineering
- Created `Has_Family` feature:
  - Combines `SibSp` + `Parch`
- Encoded categorical variables:
  - `Sex` → Label Encoding
  - `Embarked` → One-Hot Encoding

---

### 3. Exploratory Data Analysis (EDA)
- Distribution plots (Age, Fare, etc.)
- Boxplots for outlier detection
- Correlation analysis
- Survival rate comparisons:
  - Family vs No Family
  - Passenger class impact

---

### 4. Machine Learning Model
- Algorithm used: **Random Forest Classifier**
- Training data: PassengerId 1–891
- Test data: PassengerId 892+

#### Model Settings:
- n_estimators = 300
- max_depth = 6
- class_weight = "balanced"
- random_state = 42

---

### 5. Evaluation
- Accuracy score
- Classification report (Precision, Recall, F1-score)

---

## 📈 Key Insights

- Passengers with family had higher survival rates (~50%)
- Females had significantly higher survival chances
- First-class passengers survived more than third-class passengers
- Fare and Pclass strongly influenced survival probability

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 📂 Project Structure
