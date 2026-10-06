# ML Lab 02: Simple & Multiple Logistic Regression

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)

---

## Academic Details
- **Student Name:** Shrri Dharshan D R
- **Register Number:** 23BPS1090
- **Course Code:** BCSE209P
- **Course Title:** Machine Learning Laboratory
- **Faculty:** Dr. S. Shridevi
- **Institution:** School of Computer Science and Engineering (SCOPE), VIT Chennai

---

## Overview
This repository contains laboratory implementations and empirical comparative studies of **Simple Logistic Regression (SiLR)** and **Multiple Logistic Regression (MuLR)** across three benchmark binary classification datasets from the UCI Machine Learning Repository.

The objective is to formulate binary classification models using the logistic/sigmoid link function, optimize log-loss (binary cross-entropy), evaluate classification performance across decision thresholds, and analyze ROC-AUC curves and confusion matrices.

---

## Experiments & Datasets

### 1. Default of Credit Card Clients (dataset-1/)
- **Dataset:** Default of Credit Card Clients Dataset ([UCI ID: 350](https://archive.ics.uci.edu/dataset/350))
- **Objective:** Predict whether a credit card client will default on payment next month (binary: `0 = Non-default`, `1 = Default`) using credit limits, demographic factors, bill statements, and payment histories.
- **Notebook:** [dataset-1/23BPS1090_ShrriDharshan_ML_Lab_2.ipynb](./dataset-1/23BPS1090_ShrriDharshan_ML_Lab_2.ipynb)
- **Algorithms:** Simple Logistic Regression (single strongest financial predictor) vs. Multiple Logistic Regression (full multi-attribute financial profile).

### 2. Connectionist Bench Sonar: Mines vs. Rocks (dataset-2/)
- **Dataset:** Connectionist Bench (Sonar, Mines vs. Rocks) ([UCI ID: 151](https://archive.ics.uci.edu/dataset/151))
- **Objective:** Classify sonar signal returns from metal cylinders (mines) versus cylindrical rocks across 60 spectral frequency bands.
- **Notebook:** [dataset-2/23BPS1090_ShrriDharshan_ML_Lab_2B_Sonar.ipynb](./dataset-2/23BPS1090_ShrriDharshan_ML_Lab_2B_Sonar.ipynb)
- **Algorithms:** SiLR (single frequency energy band) vs. MuLR (all 60 continuous sonar frequency bands).

### 3. Bank Marketing Term Deposit Subscription (dataset-3/)
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Predict whether a client will subscribe to a bank term deposit (`yes` / `no`) based on direct telemarketing campaigns, economic indicators, and customer profiles.
- **Notebook:** [dataset-3/23BPS1090_ShrriDharshan_ML_Lab_2C_BankMarketing.ipynb](./dataset-3/23BPS1090_ShrriDharshan_ML_Lab_2C_BankMarketing.ipynb)
- **Algorithms:** SiLR (call duration predictor) vs. MuLR (full campaign and socio-economic feature set).

---

## Evaluation Metrics
Binary classification performance is evaluated using:
- **Confusion Matrix:** True Positives (TP), True Negatives (TN), False Positives (FP), False Negatives (FN).
- **Classification Accuracy:** Overall ratio of correctly predicted instances.
- **Precision:** Specificity in positive class predictions ($\frac{TP}{TP + FP}$).
- **Recall (Sensitivity):** Proportion of actual positives identified ($\frac{TP}{TP + FN}$).
- **F1-Score:** Harmonic mean of precision and recall.
- **Receiver Operating Characteristic (ROC) & AUC:** Trade-off analysis across decision thresholds (True Positive Rate vs. False Positive Rate).

---

## Repository Structure
```text
ML-Lab-02-Logistic-Regression/
├── dataset-1/
│   └── 23BPS1090_ShrriDharshan_ML_Lab_2.ipynb
├── dataset-2/
│   └── 23BPS1090_ShrriDharshan_ML_Lab_2B_Sonar.ipynb
├── dataset-3/
│   └── 23BPS1090_ShrriDharshan_ML_Lab_2C_BankMarketing.ipynb
├── .gitignore
└── README.md
```

---

## How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/ML-Lab-02-Logistic-Regression.git
   cd ML-Lab-02-Logistic-Regression
   ```
2. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xlrd ucimlrepo jupyter
   ```
3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
