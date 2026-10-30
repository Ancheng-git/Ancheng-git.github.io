# Heart Disease Risk Analysis

## Overview

A STOR 320.02 Group 8 project investigating heart disease risk factors using a dataset of 918 patient records. We examined blood sugar-by-sex interactions among patients with normal cholesterol and whether ECG ST abnormalities add predictive information in patients over 60 after accounting for exercise-induced ST depression (`oldpeak`).

## Tools and Methods

- R for exploratory subgroup visualizations and statistical modeling.
- Logistic regression with and without interaction terms, decision trees, and XGBoost, compared against a majority-class baseline using a train/test split.
- Nested logistic models and deviance tests for incremental predictor value; ROC-AUC, accuracy, and confusion matrices for model assessment.

## Key Results

- In the normal-cholesterol subgroup, the blood sugar-by-sex interaction had a reported p-value of **0.0458**.
- Interaction logistic regression achieved **84.68% test accuracy** and **0.9247 ROC-AUC**, compared with **81.08%** and **0.9040** for basic logistic regression.
- In patients over 60, adding ECG ST abnormalities to `oldpeak` produced limited evidence of improved fit (**p = 0.0999**); AUC increased from **0.668 to 0.693**.

These are the team's reported results from the paper. The study discusses subgroup size, data-source differences, and unavailable lifestyle factors as limitations.

## Read the Paper

- [Open the full paper](https://ancheng-git.github.io/projects/heart-disease-risk-analysis/Final-Paper-Group8.html)
- [HTML file in this repository](Final-Paper-Group8.html)

The original self-contained HTML report is preserved unchanged. It is dated **April 26, 2026** and credited to **STOR 320.02 Group 8**.
