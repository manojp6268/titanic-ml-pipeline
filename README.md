# 🚢 titanic-ml-pipeline

![Status](https://img.shields.io/badge/Status-Work_In_Progress-orange?style=flat-square)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-F7931E?style=flat-square&logo=scikit-learn)
![Commits](https://img.shields.io/github/commit-activity/w/manojp6268/titanic-ml-pipeline?style=flat-square&color=brightgreen)

> Building this the right way - not the fast way.

---

## What this is

An end-to-end machine learning pipeline built on the Kaggle Titanic 
dataset. The goal is not simply to maximise accuracy - it is to build 
a **thoroughly documented, defensible analytical pipeline** that 
demonstrates how a data scientist actually thinks through a problem.

Every decision in this repo - which plot, which imputation strategy, 
which model, which metric - is explained and justified in the notebook.

---

## Pipeline stages

| Stage | Status | Description |
|---|---|---|
| EDA — Univariate Analysis | ✅ Complete | Target, numeric, and categorical distributions |
| EDA — Bivariate Analysis | 🔄 In progress | Survival rate by Sex, Pclass, Age group |
| Missing Value Treatment | ⏳ Pending | Age, Cabin, Embarked imputation strategy |
| Feature Engineering | ⏳ Pending | Title extraction, family size, deck, fare log |
| Preprocessing | ⏳ Pending | Encoding, scaling, train/test split |
| Modelling | ⏳ Pending | Logistic Regression, Random Forest, XGBoost |
| Hyperparameter Tuning | ⏳ Pending | RandomizedSearchCV |
| Explainability | ⏳ Pending | SHAP values — why did the model predict this? |
| Final Write-up | ⏳ Pending | Conclusions and key learnings |

---

## Why each stage matters

**EDA first - always.**
You cannot make good modelling decisions without understanding your data.
Most beginner pipelines skip straight to models and wonder why performance
is poor. This pipeline treats EDA as the foundation, not a formality.

**Feature engineering over model complexity.**
A well-engineered feature beats a complex model on structured tabular data
almost every time. Extracting titles from passenger names, building family
size from SibSp and Parch, and deriving deck from cabin numbers will matter
more than which algorithm is chosen.

**Explainability is not optional.**
A model nobody can explain is a model nobody will trust or deploy. SHAP
values will be used to answer the question a stakeholder always asks —
*"why did the model make this prediction?"*

---

## Current notebook

| Notebook | Description |
|---|---|
| `titanic_eda.ipynb` | Exploratory Data Analysis - univariate analysis complete |

---

## Key findings so far

- **Survival rate:** 38.4% survived, 61.6% did not — moderate class imbalance
- **Missing values:** Age (19.9%), Cabin (77.1%), Embarked (0.2%)
- **Fare:** Heavily right-skewed - log transformation likely needed
- **Age:** Roughly normal distribution - median imputation as baseline

---

## Tech stack

`Python` `Pandas` `NumPy` `Matplotlib` `Scikit-learn` `SHAP`

---

## Commit discipline

This repo is updated daily - each commit reflects a specific analytical
decision or pipeline stage. The commit history is intentional and readable.

---

## Author

**Manoj Prakash** — Data Scientist & AI/ML Engineer
M.Sc. Data Science @ Universität Trier · ex-Oracle Cerner · ex-Huawei

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/manoj-p-a95b7b1a2)
[![Email](https://img.shields.io/badge/Email-manojp6268@gmail.com-1A2B4A?style=flat-square&logo=gmail)](mailto:manojp6268@gmail.com)

---

*The Titanic sank. This pipeline won't.*
