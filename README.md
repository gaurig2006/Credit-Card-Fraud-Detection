# Credit-Card-Fraud-Detection# 🕵️‍♀️ Credit Card Fraud Detection Using Machine Learning

Detecting fraudulent credit card transactions using supervised machine learning models: Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Machine (SVM), and Decision Tree.

## 📌 Overview

With the rise of online transactions, **credit card fraud** has become a major concern for banks and consumers. This project explores multiple machine learning models to effectively identify fraudulent transactions from genuine ones using a real-world dataset.

**Goal**: Build robust classification models that can detect fraudulent transactions with high accuracy and low false positives.

## 📊 Dataset Description

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records**: 284,807 transactions
- **Fraudulent cases**: 492 (~0.17%)
- **Features**:
  - `V1` to `V28`: Anonymized PCA-transformed features
  - `Time`: Seconds from first transaction
  - `Amount`: Transaction amount
  - `Class`: 1 = fraud, 0 = genuine

## 🔧 Methodology

### 1. Data Preprocessing
- Checked for missing/null values
- Normalized `Amount` and `Time` features
- Handled class imbalance using undersampling
- Split into training and testing sets (80-20 split)

### 2. Models Implemented
- 📉 **Logistic Regression**
- 🌲 **Decision Tree Classifier**
- 💠 **Support Vector Machine (SVM)**
- 👥 **K-Nearest Neighbors (KNN)** (K=3 and K=7)

### 3. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC

## 🧪 Results Summary

| Model                | Accuracy (Test) | Notes                                     |
|---------------------|-----------------|-------------------------------------------|
| Logistic Regression | 91.88%          | Strong baseline, interpretable            |
| Decision Tree       | ~98%            | Effective but may overfit                 |
| SVM                 | 97.59%          | Performs well on imbalanced data          |
| KNN (K=3, K=7)       | 100%*           | High score, but computationally expensive |

\* Perfect accuracy due to dataset configuration; not ideal for large-scale real-time use.

## 📁 File Structure

```bash
.
├── Credit Card Fraud Detection - Logistic Regression.ipynb
├── Credit Card Fraud Detection - Decision Tree.ipynb
├── Credit Card Fraud Detection - Support Vector Machines.ipynb
├── Credit Card Fraud Detection - K-Nearest Neighbor.ipynb
└── README.md
