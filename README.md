# 🦠 COVID-19 Risk Classification & Analysis Project

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-yellow.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

Welcome to the **COVID-19 Risk Classification & Analysis Project**!  
This project uses clinical and demographic data of COVID-19 patients to predict the severity of the disease using various machine learning algorithms. It also explores the effect of dimensionality reduction (PCA) on model performance.

---

## 📊 Project Overview

- **🎯 Objective**: Predict whether a COVID-19 patient is at **high risk or not** based on medical features.
- **📁 Dataset**: Official government data from Mexico, provided on [Kaggle](https://www.kaggle.com/datasets/inversion/covid19-mexico).
- **🧪 Key Tasks**:
  - Data loading and cleaning.
  - Exploratory Data Analysis (EDA) and visualization.
  - Feature encoding and scaling.
  - Training multiple classifiers:
    - Logistic Regression
    - Random Forest
    - XGBoost
    - Support Vector Machine (SVM)
  - Evaluation using classification metrics and ROC curves.
  - PCA comparison for dimensionality reduction.

---



## 📈 Dataset Description

The dataset contains over **77,000 records** and includes:

- **Demographics**: Age, Gender, Pregnancy
- **Medical History**: Diabetes, COPD, Asthma, Hypertension, Cardiovascular Disease, Obesity, Renal Chronic Disease, Smoking
- **Clinical Info**: Pneumonia, Intubated, ICU Admission
- **Target Variable**: A binary classification (e.g., high-risk or not)

### 📊 Sample Visualizations

#### 🎯 Target Class Distribution
![Target Class Distribution](images/class_distribution.png)

#### 🔥 Feature Correlation Heatmap
![Feature Correlation](images/heatmap.png)

#### 📉 ROC Curve for Best Model (XGBoost)
![ROC Curve](images/model_performance.png)

---

## 🤖 Models & Results

| Model               | Accuracy | Precision | Recall | F1-score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression|    ✓     |     ✓     |   ✓    |    ✓     |
| Random Forest      |    ✓     |     ✓     |   ✓    |    ✓     |
| XGBoost            |  **Best**|  **✓✓✓**  | **✓✓✓**| **✓✓✓**  |
| SVM                |    ✓     |     ✓     |   ✓    |    ✓     |

> ✅ **XGBoost** gave the highest predictive performance and was chosen as the final model.

---

## 🧠 PCA Comparison

Principal Component Analysis (PCA) was applied to reduce dimensionality and compare performance.  
While PCA helped improve speed slightly, model accuracy was slightly better **without** PCA due to loss of explainability.

---

## 💾 How to Run

1. Clone the repo:
   ```bash
   git clone [https://github.com/your-username/covid19-risk-classifier.git](https://github.com/your-username/covid19-risk-classifier.git)
   cd covid19-risk-classifier
pip install -r requirements.txt
jupyter notebook notebooks/covid19_risk_classifier.ipynb
