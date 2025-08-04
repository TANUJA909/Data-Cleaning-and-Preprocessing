# Task 1: Data Cleaning & Preprocessing – Titanic Dataset

## Objective
To clean and preprocess the Titanic dataset by handling missing values, encoding categorical variables, scaling features, and removing outliers — preparing the dataset for machine learning models.

---

## Tools Used
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn

---

## Dataset
Dataset used: [Titanic Dataset – Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

---

## Steps Performed

### 1. Data Import & Exploration
- Loaded the dataset using `pandas`.
- Checked basic information, null values, and data types using `df.info()` and `df.isnull().sum()`.

### 2. Handling Missing Values
- Filled missing `Age` values using the median.
- Filled missing `Embarked` values using the mode.
- Dropped the `Cabin` column due to excessive missing values.

### 3. Encoding Categorical Variables
- Used one-hot encoding on `Sex` and `Embarked` with `drop_first=True` to avoid the dummy variable trap.

### 4. Feature Scaling
- Applied standardization on `Age` and `Fare` using `StandardScaler` from `sklearn`.

### 5. Outlier Detection & Removal
- Used boxplots to detect outliers.
- Removed extreme outliers from the `Fare` column beyond the 99th percentile.

---

## Final Output
- A cleaned and preprocessed version of the Titanic dataset ready for machine learning.
- File saved as `titanic_cleaned.csv` (or used directly for modeling).

---

## Prepared By
Tanuja Deshmukh  
AI & ML Internship - Task 1
