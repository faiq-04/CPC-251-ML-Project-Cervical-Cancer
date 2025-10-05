# 🧠 Cervical Cancer Prediction using Machine Learning

### CPC251W – Machine Learning and Computational Intelligence  
**Group 3** | Academic Session 2024/2025  

**Contributors:**  
- Syeda Laiba Faraz   
- Faiq Ahmed Shaikh  
- Ma Bowen   

---

## 📘 Project Overview

This project explores how **machine learning** can assist in the **early detection of cervical cancer** using patient medical data.  
We developed and compared two classification models — **Random Forest** and **Decision Tree** — to predict biopsy test results based on demographic, lifestyle, and health features.

The dataset is **highly imbalanced**, with only 6.41% of positive cases. To address this, we focused on metrics like **Recall** and **F1-score** instead of accuracy, since identifying true positives is more critical than overall correctness in a medical context.

---

## 🧩 Objectives
- Predict the likelihood of a patient testing positive for cervical cancer.  
- Evaluate the performance of Random Forest and Decision Tree models.  
- Apply **GridSearchCV** and **RandomizedSearchCV** for hyperparameter tuning.  
- Compare models using **Precision, Recall, F1-score**, and **Confusion Matrix**.  
- Improve interpretability and reliability for potential healthcare applications.

---

## 🧾 Dataset

- **Source:** Provided in USM e-Learning (Cervical Cancer Risk Factors Dataset).  
- **Size:** 858 entries × 36 attributes.  
- **Target Variable:** `Biopsy` (binary classification).  
- **Imbalance:** Only 6.41% of samples are positive for cancer.  

Main features include:
- Demographic details (age, education, etc.)
- Lifestyle factors (smoking, hormonal contraceptives)
- Sexual and reproductive history
- Medical history (STDs, screening results)

---

## ⚙️ Data Preprocessing Steps
1. **Data Cleaning:**  
   - Removed columns with excessive null values.  
   - Imputed missing values using the **median**.  
   - Dropped duplicate rows.  

2. **Feature Selection:**  
   - Used **Chi-Squared (χ²)** test to select top-performing predictors.  

3. **Splitting:**  
   - 70% Training, 15% Validation, 15% Testing.  

---

## 🧮 Machine Learning Models

### 1. Random Forest
- **Baseline Model:** Default parameters.  
- **Grid Search:** Tuned parameters such as `n_estimators`, `max_depth`.  
- **Random Search:** Explored a wider parameter space.  
- **Class Weight:** Balanced to handle data imbalance.

### 2. Decision Tree
- **Baseline:** Default model.  
- **Feature Importance:** Focused on top features.  
- **Criterion Comparison:** Gini vs. Entropy.  
- **GridSearchCV:** Tuned for optimal depth and split size.

---

## 📊 Results Summary

| Metric | Decision Tree | Random Forest |
|:-------|:--------------:|:--------------:|
| **Accuracy** | Moderate | High |
| **F1-Score (Minority)** | Balanced | Higher |
| **Recall (Class 1)** | Good | Best |
| **Training Time** | Fast | Slower |
| **Interpretability** | Excellent | Low |

- **Random Forest** achieved the best recall and F1-score for minority cases (0.91 and 0.80).  
- **Decision Tree** with GridSearchCV performed best for interpretability and speed — valuable in healthcare contexts.  

---

## 🧠 Technologies Used
- Python (Anaconda 2.5.2)  
- Jupyter Notebook (v7.3.2)  
- scikit-learn  
- pandas, numpy  
- matplotlib, seaborn  

---

## 💻 How to Run the Project

1. **Download or clone** this repository:
   ```bash
   git clone https://github.com/faiq-04/CPC251-ML-Project-Cervical-Cancer.git
   cd CPC251-ML-Project-Cervical-Cancer

2. **Open the notebook**
   ```bash
   jupyter notebook CPC251_Project_Part1_GroupNo.3.ipynb
3. **Install the required packages**
   ```bash
   pip install -r requirements.txt
4. **Run the notebook**
   Execute all cells sequentially to reproduce the results.
