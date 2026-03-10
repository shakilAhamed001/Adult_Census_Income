# Adult_Census_Income

# 📊 Predicting Income Levels with Machine Learning  
### End-to-End Classification Project

This project focuses on **predicting whether an individual's income exceeds $50K** using the **Adult Census Income dataset**.  
It demonstrates a **complete Machine Learning workflow**, including data preprocessing, exploratory data analysis, model training, evaluation, and validation.

---

# 🔎 Key Findings & Results

## 1. Exploratory Data Analysis (EDA)

- Identified and handled `?` values in `workclass`, `occupation`, and `native.country` by converting them to `np.nan` and imputing with their respective **mode values**.
- Visualized **age distribution** across income levels using **boxplots**, showing individuals earning `>50K` tend to have a **higher median age**.
- Analyzed numerical features using **histograms** and **correlation heatmaps**.
- Observed **weak linear correlations** among most numerical features.

---

## 2. Model Performance

After preprocessing and feature engineering, two classification models were trained:

### Logistic Regression
- **Accuracy:** `0.8518`
- **Precision (>50K):** `0.7361`
- **Recall (>50K):** `0.5995`

### Random Forest Classifier
- **Accuracy:** `0.8524`
- **Precision (>50K):** `0.7304`
- **Recall (>50K):** `0.6135`
- **F1 Score:** `0.6669`

The **Random Forest model performed slightly better overall**, showing improved balance between precision and recall.

### Cross Validation

- **5-Fold Stratified Cross Validation**
- **Mean Accuracy:** `0.8518`
- **Low Standard Deviation**, indicating stable and reliable performance.

---

# ⚙️ Technical Workflow

## 1. Data Cleaning & Preprocessing

- Replaced missing values (`?`) with `np.nan`
- Imputed missing values using **mode** for:
  - `workclass`
  - `occupation`
  - `native.country`
- Applied **One-Hot Encoding** to categorical features (excluding target variable `income`)
- Scaled numerical features using **StandardScaler**

---

## 2. Model Development & Evaluation

- Implemented **Logistic Regression** as a baseline model
- Built a **Random Forest Classifier**
- Evaluated models using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- Performed **Stratified 5-Fold Cross Validation** for robust performance estimation.

---

## 3. Full Data Science Lifecycle

This project demonstrates a **complete end-to-end machine learning pipeline**, including:

- Data Exploration
- Data Cleaning
- Feature Engineering
- Model Training
- Model Evaluation
- Model Validation

---

# 🧰 Tech Stack

- 🐍 **Python**
- 🐼 **Pandas**
- 📊 **Matplotlib**
- 📊 **Seaborn**
- 🤖 **Scikit-learn**

---

# 📂 Dataset

Adult Census Income Dataset  
Used for predicting whether a person's income exceeds **$50K per year** based on demographic and employment features.

---

# 📈 Project Goals

- Build a reliable **income classification model**
- Compare baseline and ensemble models
- Practice a **complete machine learning workflow**
- Perform meaningful **data analysis and visualization**

---

# 🚀 Future Improvements

- Hyperparameter tuning using **GridSearchCV**
- Try advanced models such as **XGBoost / Gradient Boosting**
- Feature importance analysis
- Deploy the model using **Streamlit or Flask**

---

⭐ If you found this project useful, consider giving it a star!