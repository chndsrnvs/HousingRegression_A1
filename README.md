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

To create and activate the Conda environment:

```bash
conda create -n housing_env python=3.9 -y
conda activate housing_env
pip install -r requirements.txt
