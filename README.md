# 🍷 Wine Quality Prediction using Supervised Machine Learning

This is my **Data Mining mini project** (EC9560) where I developed machine learning models to predict the quality of Portuguese red wine based on physicochemical properties.

---

## 📌 Project Overview
- **Goal:** Predict wine quality (scores 0–10) using physicochemical features.  
- **Dataset:** Red Wine Quality dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality).  
- **Samples:** 1,599 red wine samples  
- **Features:** 11 physicochemical attributes (acidity, alcohol, sugar, etc.) + target (quality)

---

## 🔬 Methodology
1. **Dataset Acquisition**
2. **Exploratory Data Analysis (EDA)**  
   - Distribution analysis, correlations, outliers  
3. **Data Preprocessing**  
   - Min-Max scaling, SMOTE oversampling for imbalance  
4. **Feature Selection**  
   - Correlation, RFE, Random Forest Importance  
5. **Model Training & Evaluation**  
   - Logistic Regression (baseline)  
   - Random Forest (final model)  
6. **Hyperparameter Tuning**  
   - GridSearchCV (best params: `n_estimators=200`, `max_depth=20`, `min_samples_split=5`)  
7. **Result Validation**  
   - Final accuracy: **88.3%**  
   - Macro precision/recall: ~88%  
   - Balanced performance across minority classes  

---

## 📊 Results
- **Random Forest (SMOTE + Tuning):**  
  - Accuracy: **88.3%**  
  - Macro F1: **87.9%**  
- Logistic Regression baseline achieved only ~55% accuracy.  

📈 The Random Forest model proved most effective, especially after handling class imbalance with SMOTE.

---

## ⚙️ Technologies Used
- Python  
- Scikit-learn  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- imbalanced-learn (SMOTE)

---

## ✨ Insights
- Alcohol ↑ → Higher quality  
- Volatile acidity ↑ → Lower quality  
- Proper class balancing significantly improved fairness in predictions.

---

## 📅 Timeline
-09 Jul 2025 - Topic Selection & Project Plan
-16 Jul 2025 - Data Understanding & Exploration
-27 Aug 2025 - Data Preprocessing
-29 Aug 2025 - Feature Selection
-01 Sep – 10 Sep 2025 - Model Training & Evaluation

---

## 🙌 Acknowledgement
This project was completed as part of **EC9560: Data Mining (Semester 07)** at the University of Jaffna.
