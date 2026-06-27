# Heart-Disease-Prediction-Using-Machine-Learning
#  Heart Disease Prediction Using Machine Learning

##  Project Overview

This project aims to predict the presence of heart disease using supervised machine learning techniques. The model analyzes various medical attributes of a patient and predicts whether the patient is likely to have heart disease. Three classification algorithms were implemented and compared to determine the best-performing model.

---

##  Problem Statement

Heart disease is one of the leading causes of death worldwide. Early prediction can assist healthcare professionals in making timely decisions and improving patient outcomes. This project develops a machine learning model that predicts the presence or absence of heart disease using patient clinical data.

---

##  Dataset

**Source:** UCI Machine Learning Repository

**Dataset:** Cleveland Heart Disease Dataset

https://archive.ics.uci.edu/dataset/45/heart+disease

### Dataset Information

- Total Records: **303**
- Total Features: **14**
- Input Features: **13**
- Target Variable: **Heart Disease**

The original target variable contained five classes (0–4). It was converted into binary form:

- **0 → No Heart Disease**
- **1 → Heart Disease Present**

---

##  Data Preprocessing

The following preprocessing steps were performed:

- Checked dataset structure and data types
- Handled missing values in **ca** and **thal** using mode imputation
- Verified that no duplicate records were present
- Converted the target variable into binary classification
- Identified numerical and categorical features
- Applied StandardScaler for Logistic Regression

---

## Exploratory Data Analysis (EDA)

EDA was performed using:

- Target variable distribution
- Age distribution
- Gender distribution
- Chest pain type distribution
- Correlation heatmap
- Feature importance visualization

These analyses helped understand the relationships between features and identify important predictors of heart disease.

---

##  Machine Learning Models

The following supervised learning algorithms were trained and evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

---

##  Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

### Performance Comparison

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|---------:|----------:|--------:|---------:|
| Logistic Regression | 86.89% | 81.25% | 92.86% | 86.67% |
| Decision Tree | 73.77% | 67.65% | 82.14% | 74.19% |
| **Random Forest** | **88.52%** | **83.87%** | **92.86%** | **88.14%** |

---

##  Best Model

The **Random Forest Classifier** achieved the best performance with:

- **Accuracy:** 88.52%
- **Precision:** 83.87%
- **Recall:** 92.86%
- **F1 Score:** 88.14%

Feature importance analysis showed that **Maximum Heart Rate Achieved (thalach)**, **Chest Pain Type (cp)**, **Thal**, **Number of Major Vessels (ca)**, and **Age** were among the most influential features.

---


## 💻 Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

## ✅ Conclusion

This project demonstrates that machine learning techniques can effectively predict the presence of heart disease using clinical patient data. Among the evaluated models, the Random Forest Classifier achieved the highest performance with an accuracy of **88.52%**. Such predictive models can serve as decision-support tools to assist healthcare professionals in early diagnosis and risk assessment.

---

## 📚 References

1. UCI Machine Learning Repository – Heart Disease Dataset  
   https://archive.ics.uci.edu/dataset/45/heart+disease

2. Pedregosa, F., et al. (2011). *Scikit-learn: Machine Learning in Python.*

3. McKinney, W. (2010). *Data Structures for Statistical Computing in Python.*

4. Hunter, J. D. (2007). *Matplotlib: A 2D Graphics Environment.*

5. Waskom, M. (2021). *Seaborn: Statistical Data Visualization.*
