# auc-roc-youden-threshold-finder
A Python tool for computing ROC curves, AUC scores, and finding the optimal classification threshold using Youden’s J Statistic.

# ROC-AUC & Youden's J Threshold Finder

A clean, educational Python script demonstrating how to evaluate binary classification models, compute the Area Under the ROC Curve (ROC-AUC), and find the optimal decision threshold (the "sweet spot") using **Youden’s J Statistic**.

## Features
* **Scikit-Learn Integration:** Utilizes `roc_curve`, `roc_auc_score`, and `confusion_matrix` for robust evaluation.
* **Optimal Threshold Tuning:** Automatically calculates Youden's J statistic ($J = TPR - FPR$) across thresholds to find the best balance between Sensitivity and Specificity.
* **Step-by-Step Breakdown:** Includes a manual threshold-iteration loop to print confusion metrics (`TPR`, `FPR`, and `J`) at every cut-off point.
* **Data Visualization:** Generates a professional `matplotlib` plot highlighting the ROC curve, random guess baseline, and the calculated sweet spot.

## Prerequisites
Make sure you have the required libraries installed:
```bash
pip install numpy matplotlib scikit-learn
