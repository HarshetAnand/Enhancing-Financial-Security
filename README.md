# Enhancing Financial Security: Credit Card Fraud Detection System

A machine learning project developing a comprehensive credit card fraud detection system. Tackles the challenge of severely imbalanced transaction data (0.17% fraud rate) using multiple resampling techniques and CART decision tree classification, with statistical evaluation of model performance.

## Problem

Credit card fraud detection is a classic imbalanced classification problem. Fraudulent transactions represent less than 0.2% of all transactions, so a naive classifier can reach high accuracy by predicting "not fraud" for everything. This project addresses that challenge through resampling and evaluation that looks beyond accuracy.

## Methodology

1. **Data Exploration:** Analyzed 284,807 transactions with 492 fraudulent cases
2. **Sampling:** Drew a 10 percent random sample for modeling, split 80/20 into training and test sets
3. **Resampling Techniques Applied:**
   - Random oversampling (minority class)
   - Random undersampling (majority class)
   - Combined over/under sampling
   - SMOTE (Synthetic Minority Over-sampling Technique)
4. **Model:** CART (Classification and Regression Tree) decision trees, trained on the SMOTE-balanced data and on the original imbalanced data for comparison
5. **Evaluation:** Confusion matrices with 95% confidence intervals and McNemar's test

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

Credit card transaction dataset containing 284,807 transactions with anonymized features (V1-V28 from PCA transformation) plus Amount, Time, and Class label. The analysis reads `creditcard.csv`, the Credit Card Fraud Detection dataset published on Kaggle by the ULB Machine Learning Group.

## Key Concepts Demonstrated

- Handling imbalanced classification problems
- Multiple resampling strategies and their tradeoffs
- Decision tree classification
- Statistical model evaluation
- Real-world fraud detection challenges
