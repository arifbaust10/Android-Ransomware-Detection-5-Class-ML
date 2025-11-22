# Multi-Class Android Ransomware Detection (5-Class ML Model)

This repository contains the full implementation of the research work titled:

**“Multi-Class Android Ransomware Detection Based on Behavioural Analysis for Smarter Mobile Security.”**

The project was developed as part of the **Machine Learning Laboratory coursework** at  
**Bangladesh Army University of Science and Technology (BAUST), Saidpur**.

---

## 🔍 Project Overview

Android ransomware remains one of the most dangerous forms of mobile malware.  
Most traditional methods treat detection as a simple **binary classification** problem (benign vs. malicious),  
but this approach fails to differentiate between *behaviourally distinct ransomware families*.

In this project, we propose a **five-class behavioural classification system**:

- 🟢 **Benign**
- 🔵 **Locker-based ransomware**
- 🔐 **Encryptor-based ransomware**
- 💳 **SMS/Banking-related ransomware**
- 🔞 **Adult-themed / Social-engineering ransomware**

Our machine learning pipeline includes preprocessing, feature engineering, model training, evaluation,  
and explainable AI using **LIME** and **SHAP**.

---

## 📊 Key Results

| Algorithm | Accuracy |
|----------|----------|
| Logistic Regression | 71% |
| KNN | 84% |
| Random Forest | 98% |
| **XGBoost** | **99.76%** |
| **LightGBM** | **99.78%** |
| CatBoost | 99.56% |

Gradient-boosting models like **LightGBM** and **XGBoost** showed the best performance.

---

---

## 🗂 Dataset

Dataset used in this study:  
https://www.kaggle.com/datasets/subhajournal/android-ransomware-detection

Total samples used after cleaning: **355,939 applications**.

---

## 🚀 How to Run

### 1. Install Required Packages

```bash
pip install -r requirements.txt


