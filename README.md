# credit-card-fraud-detection

#1. Introduction
Credit card fraud is a critical problem in the financial industry. With millions of transactions processed every day, manually identifying fraudulent activity is impossible. Machine learning provides an automated, scalable solution that can detect fraud patterns in real-time.
This report documents the complete machine learning pipeline applied to a real-world credit card fraud dataset. It covers data collection, preprocessing, model building, evaluation, and deployment recommendation.

Dataset: Kaggle — Credit Card Fraud Detection Dataset (ULB Machine Learning Group) Total Records: 284,807 transactions | Fraudulent: 492 (0.17%) | Non-Fraudulent: 284,315 (99.83%) Features: 30 (V1–V28 PCA-anonymized + Time + Amount) + 1 target column (Class)

#2. Problem Statement
The goal is to build a binary classification model that can accurately predict whether a given credit card transaction is fraudulent (Class = 1) or legitimate (Class = 0).

Key Challenges:
•	Extreme class imbalance: fraud cases represent only 0.17% of all transactions
•	Features V1–V28 are PCA-transformed for privacy — no direct business interpretation
•	High cost of false negatives: missing a fraud transaction is far more costly than a false alarm
•	High-dimensional dataset with 30 features requiring proper scaling and preprocessing
