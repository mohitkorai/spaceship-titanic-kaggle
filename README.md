# spaceship-titanic-kaggle
Classification project using CatBoost, SVM, pseudo-labeling, and threshold tuning — Top 4.5% on Kaggle Spaceship Titanic competition (80.874% score)
# 🚀 Spaceship Titanic - Kaggle ML Project

This project addresses the [Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic) classification challenge on Kaggle. The goal is to predict whether passengers were transported to an alternate dimension, using demographic and travel-related features.

🎯 **Final Kaggle Score:** 80.874%  
🏅 **Leaderboard Rank:** Top 90 of 2,022 (Top 4.5%)

---

## 🔍 Problem Statement

A mysterious gravitational anomaly has affected the spaceship *Titanic*, and some passengers have vanished. Your task is to build a binary classifier that predicts whether each passenger was "Transported" based on available data.

---

## 📂 Project Overview

This notebook demonstrates a complete machine learning pipeline:

- **Data Cleaning & Preprocessing**
  - Handling missing values with mode/median imputation
  - Splitting complex features (e.g., `Cabin` → Deck/Side/Number)
  - Creating missing-value indicators

- **Feature Engineering**
  - Derived features: `IsChild`, `IsFamily`, etc.
  - Encoding strategies adapted for model types

- **Modeling**
  - Trained and tuned:
    - **CatBoostClassifier** (main model)
    - **SVM** (used in meta-modeling)
  - Used **Stratified K-Fold** with Out-of-Fold (OOF) predictions
  - Applied **threshold optimization** to boost performance

- **Advanced Techniques**
  - **Pseudo-labeling** with confidence thresholds (0.98 and 0.05)
  - **Meta-modeling** (stacked blending of CatBoost + SVM)
  - Evaluated multiple models (XGBoost, LightGBM, HGB, RF) for ensembling

- **Final Submission**
  - Best performance achieved using a **solo CatBoost model**, enhanced with pseudo-labeled data and optimal thresholding.

---

## 📊 Results Summary

| Metric              | Value               |
|---------------------|---------------------|
| OOF Accuracy        | 82.56%              |
| Kaggle Public Score | 80.874%             |
| Leaderboard Rank    | 90 / 2,022 (Top4.5) |

---

## 🧰 Tools & Libraries

- Python (pandas, numpy, scikit-learn)
- CatBoost, SVM
- Optuna (hyperparameter tuning)
- Matplotlib / seaborn (EDA, visuals)
- Jupyter Notebook

---

## 📁 Repository Contents

- `spaceship-titanic.ipynb`: Full notebook with code, tuning, and insights
- `README.md`: Project overview and results

---

## 📌 Author

**Mohit Venkata Rama Swamy Korai**  
Machine Learning & Data Science Enthusiast  
[GitHub](https://github.com/mohitkorai) • [Kaggle](https://www.kaggle.com/mohitkorai) • [LinkedIn](www.linkedin.com/in/venkatasw)

---


