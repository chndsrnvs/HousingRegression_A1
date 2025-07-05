# 🏠 HousingRegression: Predicting Boston Home Prices

## 🔍 Project Summary

This project aims to predict housing prices based on features from the Boston Housing dataset using multiple regression models. It includes manual data handling, model comparisons, hyperparameter tuning, and MLOps automation via GitHub Actions. The work reflects an end-to-end machine learning workflow with reproducibility and modular code practices.

---

## 📁 Repository Layout

- `.github/workflows/ci.yml` — CI workflow using GitHub Actions  
- `regression.py` — Implements various regression models  
- `hyper.py` — Performs hyperparameter tuning across models  
- `utils.py` — Modular functions for data loading, splitting, training, and evaluation  
- `requirements.txt` — Package dependencies  
- `README.md` — Project documentation  

---

## 🌿 Branch Structure

- `main` — Final merged codebase  
- `reg_branch` — Baseline regression models and performance evaluations  
- `hyper_branch` — Extended with hyperparameter optimization and tuned model runs  

---

## ⚙️ Environment Setup

To replicate the project locally:

```bash
conda create -n housing_env python=3.9 -y
conda activate housing_env
pip install -r requirements.txt
```

This ensures consistent package versions for regression modeling and automated runs.

---

## ▶️ Script Execution

Use the following commands to run your model scripts manually:

```bash
# Run baseline regression models
python regression.py

# Run hyperparameter tuning
python hyper.py
```

Both scripts will output key evaluation metrics using the dataset loaded via `utils.py`.

---

## 📊 Model Performance Summary

| Model                       | MSE    | R² Score |
|-----------------------------|--------|----------|
| Linear Regression           | 24.29  | 0.6688   |
| Decision Tree               | 10.42  | 0.8580   |
| Random Forest               | 7.90   | 0.8923   |
| **Tuned Decision Tree**     | 9.34   | 0.8726   |
| **Tuned Random Forest**     | 7.90   | 0.8923   |

> Tuning improved the Decision Tree’s performance, while Random Forest retained optimal scores without further gains from hyperparameter adjustments.

---

## 🤖 Continuous Integration via GitHub Actions

This repository uses a CI pipeline triggered automatically by branch updates. The workflow configuration (`ci.yml`) includes:

- Setup of Python 3.9 on Ubuntu runner
- Installation of project dependencies from `requirements.txt`
- Execution of both `regression.py` and `hyper.py` in every run

Branch pushes—including `main`, `reg_branch`, and `hyper_branch`—activate the workflow via wildcard (`'*'`) logic. Logs and results are visible under the **Actions** tab of the GitHub repository.

---
