# Credit Card Fraud Detection Using Machine Learning

## Overview

This project analyzes credit card transactions and develops machine learning models to identify potentially fraudulent transactions. The project focuses on handling a highly imbalanced classification problem and evaluating model performance using appropriate metrics beyond accuracy.

## Business Problem

Financial institutions process a large volume of transactions every day, making it challenging to manually identify fraudulent activity. Fraudulent transactions can result in significant financial losses and negatively impact customer trust.

The objective of this project is to build and evaluate machine learning models capable of distinguishing between legitimate and fraudulent credit card transactions.

## Dataset

The dataset contains anonymized credit card transactions, including:

* Time
* Transaction Amount
* Anonymized features (V1–V28)
* Transaction Class

Target variable:

* 0 — Legitimate Transaction
* 1 — Fraudulent Transaction

The dataset is highly imbalanced, making traditional accuracy an unreliable evaluation metric.

## Project Workflow

1. Data Loading
2. Data Exploration
3. Data Cleaning
4. Exploratory Data Analysis
5. Class Imbalance Analysis
6. Data Preprocessing
7. Model Training
8. Model Evaluation
9. Feature Importance Analysis
10. Business Insights

## Machine Learning Models

* Logistic Regression
* Random Forest Classifier

## Evaluation Metrics

The models were evaluated using:

* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

## Key Insights

* Fraudulent transactions represent only a small percentage of total transactions.
* Accuracy alone is insufficient for evaluating fraud detection models.
* Recall is critical because failing to identify fraudulent transactions can result in financial losses.
* Precision is important to reduce unnecessary blocking of legitimate customer transactions.
* Model selection should consider the trade-off between detecting fraud and minimizing false positives.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
credit-card-fraud-detection/
│
├── data/
├── notebooks/
│   └── fraud_detection.ipynb
│
├── images/
│
├── requirements.txt
├── README.md
└── .gitignore
```

## How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Download the dataset and place `creditcard.csv` inside the `data` folder.
4. Open the Jupyter Notebook:

```bash
notebook
```

5. Run `fraud_detection.ipynb`.

## Future Improvements

* Hyperparameter tuning
* SMOTE for class imbalance handling
* XGBoost model comparison
* Fraud detection threshold optimization
* Model deployment using Streamlit or Flask
* Real-time transaction scoring

