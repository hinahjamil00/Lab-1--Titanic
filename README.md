# 🚢 Titanic Data Cleaning and Exploratory Data Analysis (EDA)

This project focuses on data preprocessing and exploratory data analysis (EDA) using the Titanic dataset. The main objective was to clean the dataset, handle missing values, perform feature engineering, and analyze important patterns related to passenger survival.

---

## 📌 Project Overview

The Titanic dataset contains information about passengers such as age, gender, ticket class, fare, family information, and survival status.

This project includes:

- Data merging
- Missing value treatment
- Duplicate checking
- Feature engineering
- Correlation analysis
- Distribution analysis
- Outlier detection
- Survival-based visual analysis

---

## 🧹 Data Cleaning Steps

### 1. Dataset Integration
- Combined train and test datasets into a single file
- Used `PassengerId` as the primary key

---

### 2. Duplicate Check
- Checked for duplicate `PassengerId` values
- No duplicate primary keys were found

---

### 3. Missing Value Treatment

| Column | Treatment |
|---|---|
| Age | Filled using mean |
| Fare | Filled using mean |
| Embarked | Filled using mode |
| Cabin | Dropped due to excessive missing values |

---

### 4. Encoding
- Applied label encoding on the `Sex` variable:
  - Male = 0
  - Female = 1

- Applied One-Hot Encoding on the `Embarked` variable:
  - `Embarked_C`
  - `Embarked_Q`
  - `Embarked_S`

---

### 5. Feature Engineering
Created a new feature:

- `Has_Family`
  - Indicates whether a passenger was traveling with family members or not

---

## 📊 Exploratory Data Analysis (EDA)

### Correlation Analysis
- Generated correlation matrix for numeric variables
- Calculated p-values with respect to the target variable (`Survived`)

---

### Distribution Analysis

#### Age
- Age distribution appeared approximately normal

#### Fare
- Fare distribution was positively skewed
- Presence of high-fare outliers was observed

---

### Boxplots
Boxplots were created for numeric variables to identify outliers and data spread.

Key observations:
- Fare contained strong outliers
- Age showed relatively fewer outliers

---

### Survival Analysis

#### Family vs Survival
Passengers traveling with family had a higher survival rate compared to passengers traveling alone.

| Category | Survival Rate |
|---|---|
| No Family | ~29% |
| Has Family | ~51% |

Bar plots were used to visualize these differences.

---

## 📈 Visualizations Included

- Histograms / Distribution Plots
- Boxplots
- Correlation Heatmap
- Survival Comparison Bar Plots

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

---

## 📂 Files Included

```text
train.csv
test.csv
titanic_combined_cleaned.csv
titanic_analysis.ipynb
README.md
```

---

## 📌 Conclusion

The project successfully cleaned and prepared the Titanic dataset for further analysis and machine learning applications. Exploratory analysis revealed important insights regarding survival patterns, fare distribution, age trends, and the impact of family presence on survival probability.

---

## 👩‍💻 Author

This project was developed as part of a data analysis and machine learning learning exercise on the Titanic dataset.

**Name:** Hina  
Data Analysis & Machine Learning Practice Project  

Titanic Data Cleaning and EDA Project
