# 🌧️ Rainfall Classification with Supervised Machine Learning

This project explores a binary classification problem using a real-world rainfall dataset. The goal is to predict whether it will rain or not on a given day based on meteorological features.

---

## 📌 Project Overview

This repository contains a complete supervised machine learning pipeline applied to the **Playground Series - Season 5, Episode 3** Kaggle dataset. It was developed as the final project for the IBM Machine Learning course: **Supervised Machine Learning: Classification**.

The project also serves as a submission to the Kaggle competition:
[Binary Prediction with a Rainfall Dataset](https://www.kaggle.com/competitions/playground-series-s5e3)

---

## 👨‍💻 About Me

My name is **Cesar Pedraja**, an Industrial Engineer with advanced studies in Data Analytics, Machine Learning, and AI. I bring real-world managerial experience and apply data science to solve practical problems that impact decision-making and operations.

---

## 🎯 Objective

- 📘 **Educational Goal:** Complete the capstone project for the IBM classification module using a structured and well-documented ML pipeline.
- 🏆 **Competitive Goal:** Participate in a Kaggle competition by building a high-performance classification model using real meteorological data.

---

## 📂 Dataset

- `train.csv` – Contains features and the binary target: `"rainfall"` (1 = rain, 0 = no rain)
- `test.csv` – Same features as train, but without the target (used for final prediction)
- `sample_submission.csv` – Submission format required by the competition

---

## 🔍 Steps Followed

1. **Exploratory Data Analysis (EDA)** – Class imbalance analysis, correlation heatmaps, feature distribution comparisons.
2. **Preprocessing** – Null value removal and consistent feature handling.
3. **Model Training** – Evaluated 8 different classifiers:
   - Random Forest
   - Logistic Regression
   - Gradient Boosting
   - KNN
   - SVM
   - Random Forest with SMOTE
   - Weighted Logistic Regression
   - XGBoost
4. **Performance Evaluation** – Using accuracy, precision, recall, and F1-score.
5. **Model Selection** – Gradient Boosting and XGBoost showed the best balance.
6. **Visualization** – Comparison bar chart of all evaluation metrics.
7. **Final Predictions** – Best model used to generate predictions on test set.

---

## 📈 Results Summary

| Model                         | Accuracy | Precision | Recall | F1 Score |
|------------------------------|----------|-----------|--------|----------|
| Gradient Boosting            | 0.867    | 0.886     | 0.945  | 0.915    |
| XGBoost                      | 0.847    | 0.881     | 0.921  | 0.901    |
| Random Forest (SMOTE)        | 0.849    | 0.900     | 0.900  | 0.900    |
| Logistic Regression (Weighted)| 0.840   | 0.911     | 0.873  | 0.892    |

---

## 📁 Files Included

- `kaggle.ipynb` – Full project notebook with code, visuals, and model training.
- `Supervised Machine Learning - Final Project.pdf` – Clean formatted report version.
- `train.csv`, `test.csv`, `sample_submission.csv` – Competition dataset (not included due to size, available on Kaggle).

---

## 🛠️ How to Run

```bash
# Clone repository
git clone https://github.com/your-username/rainfall-prediction-ml.git
cd rainfall-prediction-ml

# Install dependencies (if using virtualenv or conda)
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook kaggle.ipynb
