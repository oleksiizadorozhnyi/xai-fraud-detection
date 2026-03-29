# Explainable AI for Fraud Detection

This project explores explainable artificial intelligence (XAI) methods for credit card fraud detection. The goal is to understand how a machine learning model makes decisions and why it sometimes makes mistakes.

## Project Overview

A Random Forest classifier is trained on a credit card fraud dataset. Two XAI methods are used:
- SHAP (SHapley Additive exPlanations)
- Counterfactual explanations (DiCE)
The project compares a true positive fraud case and a false positive case to better understand model behavior.

## Dataset

The dataset used is the Credit Card Fraud Detection dataset from Kaggle:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
Dataset characteristics:
- highly imbalanced
- anonymized numerical features V1 to V28
- additional features: Time, Amount
- target variable: Class (1 = fraud, 0 = normal)

## Model

Random Forest Classifier

Evaluation metrics:
- ROC-AUC
- classification report
- confusion matrix

## Main Results

- ROC-AUC: ~0.96
- High precision for fraud class
- Lower recall due to class imbalance
- Important features: V12, V14, V10
- Small feature changes can flip predictions

## Installation

pip install -r requirements.txt

## How to Run

1. Download dataset from Kaggle
2. Put creditcard.csv in data/ folder
3. Run:
   jupyter notebook

## Author

Oleksii Zadorozhnyi
Explainable AI 2025–2026
