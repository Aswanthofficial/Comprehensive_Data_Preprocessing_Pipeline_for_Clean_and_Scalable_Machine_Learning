# 🧹 Comprehensive Data Preprocessing Pipeline for Machine Learning

This project demonstrates a full-fledged data preprocessing pipeline on a structured dataset, preparing it for effective use in machine learning models. It includes handling missing values, detecting and treating outliers, encoding categorical variables, and applying feature scaling techniques.

---

## 📁 Dataset

- **File**: `preprocessing_dataset.csv`
- **Sample Features**:
  - `Age` (numeric)
  - `Gender` (categorical)
  - `Salary` (numeric)
  - `Department` (categorical)

---

## 🎯 Objectives

- Handle missing values with appropriate strategies
- Detect and treat outliers using IQR, Z-score, and Isolation Forest
- Encode categorical features using Label Encoding, One-Hot Encoding
- Standardize and Normalize numeric features for better ML performance
- Visualize data completeness and distributions using `missingno`, `seaborn`, and `matplotlib`

---

## 🛠️ Tools & Libraries Used

- **Python 3.11**
- **Pandas**, **NumPy** – Data manipulation
- **Matplotlib**, **Seaborn**, **missingno** – Data visualization
- **Scikit-learn** – Preprocessing utilities:
  - `LabelEncoder`, `OneHotEncoder`
  - `StandardScaler`, `MinMaxScaler`
  - `IsolationForest` (outlier detection)

---

## 🧪 Preprocessing Steps

### 🔹 1. Missing Value Handling
- `Age` & `Salary` filled with **median**
- `Gender` filled with **mode**
- Visualized missingness using `missingno.bar()` and `sns.heatmap()`

### 🔹 2. Outlier Detection & Treatment
- IQR-based method (`Q1`, `Q3`, `IQR`)
- Z-score method with threshold = 2.3
- `IsolationForest` to detect anomalous rows
- Replaced unrealistic `Age > 100` with median

### 🔹 3. Categorical Encoding
- `Gender` encoded with both:
  - `LabelEncoder`
  - `OneHotEncoder`
- `Department` converted using `pd.get_dummies()`

### 🔹 4. Feature Scaling
- `StandardScaler` used to standardize `Age` and `Salary`
- `MinMaxScaler` used to normalize `Age` into `[0,1]` range

---

## 📊 Sample Visualizations

- ✅ Heatmap of missing values
- ✅ Boxplot for outlier detection
- ✅ Scatterplot (Age vs Gender)
- ✅ Bar chart of missing values

---

