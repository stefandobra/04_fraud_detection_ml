# 04 Fraud Detection ML

A machine learning project that trains a model to detect fraudulent credit card transactions using a real-world dataset from Kaggle. Built in Python as part of a portfolio project series demonstrating AI and full-stack development skills.

## Overview

Credit card fraud detection is a core challenge in fintech. This project uses a real anonymised dataset of 284,807 transactions (0.17% fraudulent) to train and evaluate a classification model. Key challenges addressed: class imbalance, choosing the right evaluation metrics, and building a clean data science narrative in Jupyter.

## Dataset

- Source: [Kaggle — Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 284,807 transactions — 492 fraud (0.17%), 284,315 genuine (99.83%)
- Features: Time, V1-V28 (PCA-anonymised), Amount, Class (0=genuine, 1=fraud)
- Not included in repo — download from Kaggle and place in project root as `creditcard.csv`

## Concepts Demonstrated

- Pandas — loading, exploring, and preparing a real dataset
- NumPy — numerical operations underpinning ML pipeline
- Matplotlib — data visualisation and class distribution charts
- Scikit-learn — train/test split, Random Forest classifier, evaluation metrics
- imbalanced-learn (SMOTE) — oversampling to fix class imbalance
- Jupyter Notebook — data story format: explore → clean → train → evaluate
- Class imbalance problem — why accuracy is a misleading metric for fraud detection
- Precision, Recall, F1 Score — correct metrics for imbalanced classification
- Train/test split — evaluating model on unseen data to prevent overfitting
- Overfitting — why training and testing on the same data produces misleading results
- PCA — understanding why V1-V28 are anonymised numerical features

## Project Structure

```
04_fraud_detection_ml/
│
├── fraud_detection.ipynb    # Main Jupyter notebook — full ML pipeline
├── requirements.txt         # Python dependencies
├── .gitignore               # Excludes venv, dataset, checkpoints
└── README.md
```

> Note: `creditcard.csv` is not committed — download from Kaggle link above.

## How to Run

```powershell
cd 04_fraud_detection_ml
venv\Scripts\activate
jupyter notebook
```

Then open `fraud_detection.ipynb` in the browser.

Requires `creditcard.csv` in the project root (download from Kaggle).

## Progress

- [x] Project setup — venv, dependencies, Jupyter
- [x] Data loading — Pandas, shape, head
- [x] Class distribution — value_counts, bar chart with percentages
- [ ] Exploratory data analysis
- [ ] Data preparation — train/test split, SMOTE
- [ ] Model training — Random Forest
- [ ] Evaluation — precision, recall, F1, confusion matrix
- [ ] Results and conclusions

## Part of a Larger Project Series

| # | Project | Status |
|---|---------|--------|
| 01 | Finance Tracker | ✅ Complete |
| 02 | Booking System | ✅ Complete |
| 03 | Stock Dashboard | ✅ Complete |
| 04 | Fraud Detection ML | 🔄 In Progress |
| 05 | RAG System | ⏳ Planned |
| 06 | AI Agent | ⏳ Planned |
| 07 | Multi-Agent System | ⏳ Planned |
| 08 | AI Receptionist SaaS (Capstone) | ⏳ Planned |

---
