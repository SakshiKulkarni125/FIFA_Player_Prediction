# FIFA Player Market Value Prediction ⚽📊

A Machine Learning project that predicts the **market value of football players** using FIFA player statistics.

This project applies **data preprocessing, exploratory data analysis, PCA, regression models, and hyperparameter tuning** to build a highly accurate predictive model.

## 🚀 Project Overview

The football transfer market is a multi-billion-dollar industry where accurate player valuation is extremely important for clubs, agents, scouts, and analysts.

This project uses machine learning to predict a player's **market value (USD)** based on:

- Technical skills
- Physical attributes
- Goalkeeping stats
- Age and demographic features
- Club and country information

The best model achieved an **R² score of 0.9106** using a **Tuned Random Forest Regressor**.

---

## 📂 Dataset Information

- **Dataset:** FIFA Player Statistics
- **Records:** 5,682 players
- **Features:** 41 columns
- **Target Variable:** `value`
- **Target Type:** Continuous (Regression)

### Important Features
- reactions
- ball_control
- dribbling
- age
- sprint_speed
- interceptions
- stand_tackle

---

## 🛠 Tech Stack

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📈 Machine Learning Workflow

### 1. Data Preprocessing
- Handling missing values
- Duplicate removal
- Label Encoding
- Outlier removal
- Log transformation of target variable
- Standardization using `StandardScaler`

### 2. Exploratory Data Analysis
- Univariate analysis
- Correlation heatmap
- Scatter plots
- Feature relationships

### 3. Dimensionality Reduction
- PCA (Principal Component Analysis)
- Variance analysis
- Component selection

### 4. Model Building
Models used:
- Linear Regression
- Random Forest Regressor
- Tuned Random Forest

### 5. Hyperparameter Tuning
Used **GridSearchCV** for:
- `n_estimators`
- `max_depth`
- `min_samples_split`

---

## 📊 Model Performance

| Model | R² Score |
|-------|-------|
| Linear Regression | 0.7516 |
| Random Forest | 0.9101 |
| Tuned Random Forest | **0.9106** |

---

## 🏆 Best Model

**Tuned Random Forest Regressor**

Best Parameters:
```python
{
    "n_estimators": 200,
    "max_depth": 20,
    "min_samples_split": 2
}
