# Logistic Regression: Binary Classification Systems

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Author
- **Shrri Dharshan D R** — [@shrridharshan27](https://github.com/shrridharshan27)

---

## Overview
This repository contains implementations and empirical evaluations of **Simple Logistic Regression (SiLR)** and **Multiple Logistic Regression (MuLR)** across three real-world binary classification benchmark datasets from the UCI Machine Learning Repository.

The project models binary decision probabilities via the sigmoid link function, optimizes cross-entropy log-loss, explores classification thresholds, and benchmarks precision-recall dynamics and ROC-AUC curves.

---

## Project Modules & Datasets

### 1. Default of Credit Card Clients (`dataset-1/`)
- **Dataset:** Default of Credit Card Clients Dataset ([UCI ID: 350](https://archive.ics.uci.edu/dataset/350))
- **Objective:** Predict credit default risk in the subsequent month (`0 = Non-default`, `1 = Default`) using credit limits, billing statements, and repayment histories.
- **Notebook:** [`dataset-1/23BPS1090_ShrriDharshan_ML_Lab_2.ipynb`](./dataset-1/23BPS1090_ShrriDharshan_ML_Lab_2.ipynb)
- **Methodology:** Univariate logistic regression (strongest single financial metric) vs. full multivariate credit-risk profile modeling.

### 2. Sonar Target Classification: Mines vs. Rocks (`dataset-2/`)
- **Dataset:** Connectionist Bench Sonar Dataset ([UCI ID: 151](https://archive.ics.uci.edu/dataset/151))
- **Objective:** Classify sonar signal returns from metal cylinders (mines) versus cylindrical rocks across 60 spectral frequency bands.
- **Notebook:** [`dataset-2/23BPS1090_ShrriDharshan_ML_Lab_2B_Sonar.ipynb`](./dataset-2/23BPS1090_ShrriDharshan_ML_Lab_2B_Sonar.ipynb)
- **Methodology:** High-dimensional continuous feature discrimination comparing single-band vs. full-spectrum 60-band regression.

### 3. Bank Marketing Term Deposit Subscription (`dataset-3/`)
- **Dataset:** Bank Marketing Dataset ([UCI ID: 222](https://archive.ics.uci.edu/dataset/222))
- **Objective:** Predict client subscription to term deposits (`yes` / `no`) based on direct telemarketing contact features and macroeconomic indicators.
- **Notebook:** [`dataset-3/23BPS1090_ShrriDharshan_ML_Lab_2C_BankMarketing.ipynb`](./dataset-3/23BPS1090_ShrriDharshan_ML_Lab_2C_BankMarketing.ipynb)
- **Methodology:** Univariate call-duration benchmark vs. multivariate campaign feature formulation with threshold tuning.

---

## Evaluation Metrics
- **Confusion Matrix:** True/False Positives and Negatives.
- **Classification Accuracy:** Overall prediction correctness.
- **Precision & Recall:** Specificity in risk identification vs. retrieval sensitivity.
- **F1-Score:** Harmonic balance of precision and recall.
- **Receiver Operating Characteristic (ROC-AUC):** True positive rate vs. false positive rate across thresholds.

---

## Project Structure
```text
Logistic-Regression-ML/
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

## Quickstart & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/Logistic-Regression-ML.git
   cd Logistic-Regression-ML
   ```
2. **Install requirements:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xlrd ucimlrepo jupyter
   ```
3. **Run the notebooks:**
   ```bash
   jupyter notebook
   ```

---

## License
Distributed under the [MIT License](https://opensource.org/licenses/MIT).
