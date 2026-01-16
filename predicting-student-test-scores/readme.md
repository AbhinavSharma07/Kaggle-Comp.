# 📊 Kaggle Playground Series 2026 – Student Exam Score Prediction
       
Welcome to this repository! 🚀
This project is built for the **2026 Kaggle Tabular Playground Series**, where the goal is to predict **students' exam scores** using tabular machine learning techniques.

---

## 🧠 Competition Overview

The Kaggle Playground Series provides lightweight, beginner-friendly datasets each month to practice and improve machine learning skills.

**Objective:**
Predict the continuous target variable **`exam_score`** for students based on provided features.

* **Problem Type:** Regression
* **Evaluation Metric:** Root Mean Squared Error (RMSE)

---

## 📁 Dataset Description

* The dataset is **synthetically generated** using a deep learning model.
* Designed to simulate real-world patterns while remaining beginner-friendly.
* May contain artifacts or correlations that differ slightly from real data.

### Files

* `train.csv` – Training data with features and target (`exam_score`)
* `test.csv` – Test data without target values
* `sample_submission.csv` – Submission format reference

---

## 🧪 Evaluation Metric

Submissions are evaluated using **Root Mean Squared Error (RMSE):**

[ RMSE = \sqrt{\frac{1}{n} \sum (y_{pred} - y_{true})^2} ]

Lower RMSE indicates better performance.

---

## 🛠️ Approach

Typical workflow used in this project:

1. Exploratory Data Analysis (EDA)
2. Feature Engineering
3. Data Preprocessing
4. Model Training
5. Cross-Validation
6. Hyperparameter Tuning
7. Prediction & Submission

Models commonly used:

* Linear Regression
* Random Forest
* XGBoost / LightGBM / CatBoost
* Neural Networks (optional)
