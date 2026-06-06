Credit Card Fraud Detection using Genetic Algorithm Optimized Random Forest
Overview

This project presents an intelligent credit card fraud detection system designed to handle highly imbalanced transaction datasets. The proposed solution combines SMOTE (Synthetic Minority Oversampling Technique) with a Genetic Algorithm (GA) optimized Random Forest classifier to improve the detection of fraudulent transactions while minimizing false negatives.

The model is evaluated against several machine learning algorithms, including Logistic Regression, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), Decision Trees, and a baseline Random Forest. Results demonstrate that the GA-tuned Random Forest achieves superior performance across multiple evaluation metrics.

Features
Credit Card Fraud Detection
Imbalanced Data Handling using SMOTE
Genetic Algorithm-based Hyperparameter Optimization
Random Forest Classification
Feature Normalization using Z-score Scaling
Performance Evaluation using:
Accuracy
Precision
Recall
F1-Score
ROC-AUC
Comparison with Multiple Machine Learning Models
Dataset

The project uses the Credit Card Fraud Detection Dataset from Kaggle.

Dataset Characteristics
Total Transactions: 284,807
Fraudulent Transactions: 492
Fraud Ratio: 0.172%
Highly Imbalanced Dataset

Dataset Link:

https://www.kaggle.com/mlg-ulb/creditcardfraud

Methodology
1. Data Preprocessing
Load transaction dataset
Handle missing values (if any)
Normalize features using Z-score normalization
X
norm
	​

=
σ
X−μ
	​

2. Handling Class Imbalance

The dataset contains very few fraud cases compared to normal transactions.

Techniques used:

Majority Class Downsampling
SMOTE (Synthetic Minority Oversampling Technique)

SMOTE generates synthetic fraud samples to balance the dataset.

3. Train-Test Split

The balanced dataset is divided into:

Training Set: 70%
Testing Set: 30%
4. Genetic Algorithm Optimization

A Genetic Algorithm is employed to optimize Random Forest hyperparameters.

Search Space
Parameter	Range
Number of Trees	10 – 50
Maximum Splits	5 – 15
Minimum Leaf Size	1 – 10
Optimization Objective

Minimize classification error:

Error=1−Accuracy

The GA performs:

Population Initialization
Fitness Evaluation
Selection
Crossover
Mutation
Generation Update
5. Random Forest Training

The optimized hyperparameters obtained from the Genetic Algorithm are used to train the final Random Forest model.

Features:

Ensemble Learning
Bootstrap Sampling
Out-of-Bag Validation
6. Model Evaluation

Performance metrics used:

Accuracy
Accuracy=
TP+TN+FP+FN
TP+TN
	​

Precision
Precision=
TP+FP
TP
	​

Recall
Recall=
TP+FN
TP
	​

F1 Score
F1=
Precision+Recall
2×Precision×Recall
	​

ROC-AUC

Measures the model's ability to distinguish between fraudulent and legitimate transactions.

Results
Model	Accuracy	Precision	Recall	F1 Score	ROC-AUC
Logistic Regression	0.99842	0.9992	0.99763	0.99842	0.99982
SVM	0.99870	0.99943	0.99797	0.99870	0.99980
KNN	0.99920	0.99854	0.99987	0.99920	0.99920
Decision Tree	0.99945	0.99953	0.99937	0.99972	0.99952
Baseline RF	0.99972	0.99990	0.99953	0.99972	0.99996
GA Tuned RF	0.99967	0.99987	0.99947	0.99967	0.99992
Why Genetic Algorithm Optimized Random Forest?
Advantages

✔ Improved Recall

✔ Better Generalization

✔ Reduced Overfitting

✔ Hyperparameter Optimization

✔ Scalability for Large Datasets

✔ Superior Balance Between Precision and Recall

Project Structure
CreditCardFraudDetection/
│
├── data/
│   └── creditcard.csv
│
├── preprocessing/
│   ├── normalization.py
│   └── smote.py
│
├── optimization/
│   └── genetic_algorithm.py
│
├── models/
│   ├── logistic_regression.py
│   ├── svm.py
│   ├── knn.py
│   ├── decision_tree.py
│   └── random_forest.py
│
├── evaluation/
│   └── metrics.py
│
├── results/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── performance_comparison.png
│
├── main.py
├── requirements.txt
└── README.md
Technologies Used
MATLAB / Python
Random Forest
Genetic Algorithm
SMOTE
Machine Learning
Data Preprocessing
Statistical Analysis
Future Improvements
Deep Learning-based Fraud Detection
Real-time Transaction Monitoring
Federated Learning Integration
Explainable AI (XAI)
Online Learning for Adaptive Fraud Detection
Deployment using REST APIs and Cloud Platforms
Authors

Ganga Lohitha Y.B.
Amrita Vishwa Vidyapeetham, Bengaluru

Reha Sai M.
Amrita Vishwa Vidyapeetham, Bengaluru
