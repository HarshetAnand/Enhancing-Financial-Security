# Enhancing Financial Security: Credit Card Fraud Detection System

A machine learning project developing a comprehensive credit card fraud detection system. Tackles the challenge of severely imbalanced transaction data (0.17% fraud rate) using multiple resampling techniques and CART decision tree classification, with rigorous statistical evaluation of model performance.

## Problem

Credit card fraud detection is a classic imbalanced classification problem — fraudulent transactions represent less than 0.2% of all transactions, making naive classifiers achieve high accuracy by predicting "not fraud" for everything. This project addresses that challenge through proper resampling and evaluation.

## Methodology

- **Data Exploration:** Analyzed 284,807 transactions with 492 fraudulent cases
- **Resampling Techniques Applied:**
  - Random oversampling (minority class)
  - Random undersampling (majority class)
  - Combined over/under sampling
  - SMOTE (Synthetic Minority Over-sampling Technique)
- **Model:** CART (Classification and Regression Tree) decision trees
- **Evaluation:** Confusion matrices, 95% confidence intervals, McNemar's Test for model comparison

## Key Results

- Baseline accuracy on imbalanced data: 99.83% (misleadingly high due to class imbalance)
- SMOTE-trained model achieved 99.95% accuracy with significantly improved fraud detection sensitivity
- Demonstrated importance of balanced evaluation metrics beyond accuracy for fraud detection

## Tech Stack

- R (caret, dplyr, ggplot2, ROSE, smotefamily, rpart)
- CART decision trees
- Statistical hypothesis testing
- Data visualization with ggplot2

## Dataset

Credit card transaction dataset containing 284,807 transactions with anonymized features (V1-V28 from PCA transformation) plus Amount, Time, and Class label.

## Key Concepts Demonstrated

- Handling imbalanced classification problems
- Multiple resampling strategies and their tradeoffs
- Decision tree classification
- Statistical model evaluation
- Real-world fraud detection challenges
