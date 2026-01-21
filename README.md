# 🩺 Breast Cancer Classification Project

## 📌 Overview
This project applies Machine Learning techniques to predict whether a breast tumor is **Benign (0)** or **Malignant (1)** based on digitized image features (like radius, texture, and concavity).

The goal was to build a model that not only achieves high accuracy but also minimizes "False Negatives" (missing a cancer diagnosis), which is critical in medical AI.

## 🛠️ The Process
1.  **Data Cleaning:** Handled missing values and removed unnecessary columns (e.g., Patient IDs).
2.  **Exploratory Data Analysis (EDA):** Used Heatmaps and Pairplots to identify key correlations between features.
3.  **Preprocessing:** Applied `StandardScaler` to normalize the data, ensuring that features with larger ranges (like Area) didn't dominate the model.
4.  **Model Benchmarking:** Trained and compared three different algorithms:
    * Logistic Regression
    * Decision Tree Classifier
    * Random Forest Classifier

## 📊 Results
I evaluated the models using **Accuracy**, **Precision**, and **Recall** on a dedicated Test Set.

| Model | Accuracy | Recall (Malignant) | Verdict |
| :--- | :--- | :--- | :--- |
| **Logistic Regression** | **97.36%** | **0.95** |
| Random Forest | 96.49% | 0.93 | 
| Decision Tree | 95.61% | 0.91 | 

**Key Finding:**
While Random Forest is usually powerful, **Logistic Regression** performed the best on this dataset. It achieved the highest recall (95%), meaning it successfully identified 95% of the malignant cases in the test set, making it the safest model for medical diagnosis in this experiment.

## 💻 Tech Stack
* **Python**
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Visualization)
* **Scikit-Learn** (Machine Learning & Metrics)
