# Network Intrusion Detection System (NIDS)

## Overview
Machine learning project to classify network traffic as Normal or Attack
using the NSL-KDD dataset, developed as the final project for the
Machine Learning course at NTI.

## Dataset
NSL-KDD (KDDTrain.csv, KDDTest.csv) — 41 features per connection,
binary classification (0 = Normal, 1 = Attack).

## Models & Results
| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | 75.38%   |
| Random Forest       | 76.48%   |
| XGBoost             | 80.18%   |

## Pipeline
Label binarization → One-Hot Encoding → Column alignment →
StandardScaler → SimpleImputer → Model training → Evaluation

## Deployment
An interactive Gradio web app allows live predictions using the
trained models.

## Requirements
pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn, gradio, joblib
