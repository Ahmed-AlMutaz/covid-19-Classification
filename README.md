# 🦠 COVID-19 Classification & Analysis Project

This project focuses on classifying and analyzing COVID-19 patient data using various machine learning models. The objective is to explore patterns in the dataset and evaluate model performance in predicting outcomes.

## 📊 Overview

- **Dataset**: CSV file containing COVID-19 case data
- **Goal**: Predict patient outcome (e.g., infection severity, recovery) using classification algorithms
- **Approach**:
  - Data preprocessing and cleaning
  - Feature scaling using StandardScaler
  - Dimensionality reduction using PCA
  - Model training and comparison

## 🤖 Models Used

- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)

## 📈 Evaluation Metrics

- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- ROC AUC Score

## 🛠️ Technologies

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

## 🚀 How to Run

1. Clone the repository or open the notebook in Google Colab.
2. Make sure to upload `Covid Data.csv` to your runtime if using Colab.
3. Run all cells in the notebook step by step.

```python
# Example to read the dataset
df = pd.read_csv('Covid Data.csv')
