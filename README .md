# Credit Card Fraud Detection using Genetic Algorithm Optimized Random Forest

## Overview

This project presents an intelligent credit card fraud detection system designed to handle highly imbalanced transaction datasets. The proposed solution combines **SMOTE (Synthetic Minority Oversampling Technique)** with a **Genetic Algorithm (GA) optimized Random Forest classifier** to improve the detection of fraudulent transactions while minimizing false negatives.

## Features

- Credit Card Fraud Detection
- Imbalanced Data Handling using SMOTE
- Genetic Algorithm-based Hyperparameter Optimization
- Random Forest Classification
- Feature Normalization using Z-score Scaling
- Accuracy, Precision, Recall, F1-Score and ROC-AUC Evaluation

## Dataset

Dataset: Credit Card Fraud Detection Dataset (Kaggle)

- Total Transactions: 284,807
- Fraudulent Transactions: 492
- Fraud Ratio: 0.172%

## Methodology

1. Data Preprocessing and Normalization
2. Class Balancing using SMOTE
3. Train-Test Split (70:30)
4. Genetic Algorithm Hyperparameter Optimization
5. Random Forest Training
6. Model Evaluation

## Results

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---------|------------|------------|----------|------------|------------|
| Logistic Regression | 0.99842 | 0.9992 | 0.99763 | 0.99842 | 0.99982 |
| SVM | 0.99870 | 0.99943 | 0.99797 | 0.99870 | 0.99980 |
| KNN | 0.99920 | 0.99854 | 0.99987 | 0.99920 | 0.99920 |
| Decision Tree | 0.99945 | 0.99953 | 0.99937 | 0.99972 | 0.99952 |
| Baseline RF | 0.99972 | 0.99990 | 0.99953 | 0.99972 | 0.99996 |
| GA Tuned RF | 0.99967 | 0.99987 | 0.99947 | 0.99967 | 0.99992 |

## Technologies Used

- MATLAB / Python
- Random Forest
- Genetic Algorithm
- SMOTE
- Machine Learning

## Future Improvements

- Real-Time Fraud Detection
- Federated Learning
- Explainable AI
- Cloud Deployment

## Authors

- Ganga Lohitha Y.B.
- Reha Sai M.
- Divya Sree P.V.
