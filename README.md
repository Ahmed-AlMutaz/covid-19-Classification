# 🦠 COVID-19 Classification & Analysis Project

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-yellow.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

Welcome to the **COVID-19 Classification & Analysis Project**! This project leverages machine learning to analyze a COVID-19 patient dataset and predict outcomes such as infection severity or mortality. By applying dimensionality reduction with Principal Component Analysis (PCA), we compare the performance of multiple classification models before and after PCA to assess its impact on predictive accuracy and efficiency.

## 📊 Project Overview

- **Objective**: Predict patient outcomes using machine learning classification models and evaluate the effect of PCA on model performance.
- **Dataset**: `Covid Data.csv` containing 77,065 records with 21 features related to patient demographics, medical history, and clinical outcomes.
- **Key Tasks**:
  - Data preprocessing and cleaning
  - Feature scaling with `StandardScaler`
  - Dimensionality reduction using PCA
  - Training and evaluating multiple machine learning models
  - Visualizing performance metrics before and after PCA

## 📈 Dataset Description

The dataset (`Covid Data.csv`) includes the following key features:
- **Demographic**: Age, Sex, Pregnancy status
- **Medical History**: Diabetes, COPD, Asthma, Hypertension, Cardiovascular, Obesity, Renal Chronic, Tobacco use
- **Clinical**: Pneumonia, Intubation status, ICU admission
- **Outcome**: `CLASIFFICATION_FINAL` (target variable, indicating COVID-19 diagnosis or severity)
- **Other**: Date of death, Medical unit, Patient type

### Dataset Statistics
- **Rows**: 77,065
- **Columns**: 21
- **Target Variable Distribution**:
