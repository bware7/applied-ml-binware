# Lab 5: Ensemble Wine Quality Prediction

**Author:** Bin Ware  
**Date:** April 11, 2025  

## Overview
This project predicts red wine quality (classified as low, medium, high) using ensemble machine learning models on the UCI Wine Quality Dataset. It tests two models—Random Forest and Voting Classifier—using 11 physicochemical features, evaluating performance with accuracy and F1 scores. The dataset is sourced from the UCI Machine Learning Repository, and the goal is to identify the best model for wine quality classification.

## Key Findings
- **Best Performance:** Random Forest (100 estimators) achieved test accuracy 0.887 and F1 0.866, excelling at capturing patterns.  
- **Voting Classifier (DT+SVM+NN):** Slightly lower test accuracy (0.866) and F1 (0.843) but better generalization (smaller train-test gaps: Acc 0.057, F1 0.063 vs. 0.112, 0.134 for Random Forest).  
- **Feature Impact:** Using all 11 features outperformed simpler subsets, though accuracy capped at ~0.89 due to data limitations.  
- **Challenges:** Class imbalance (3.94% low-quality wines) and feature power limited predictive accuracy, skewing results toward the medium class.

## Files
- `ml05_binware.ipynb`: Jupyter notebook with code, analysis, and results.  
- `winequality-red.csv`: Local dataset file required for execution.

## Requirements
- Python 3.x  
- Libraries: pandas, numpy, matplotlib, scikit-learn  

## How to Run
1. Place `winequality-red.csv` in the same directory as `ml05_binware.ipynb`.  
2. Open `ml05_binware.ipynb` in Jupyter Notebook.  
3. Run all cells to replicate results, focusing on Random Forest (best performer).  
4. Modify model parameters (e.g., `n_estimators` in Random Forest, `estimators` in Voting Classifier) in Section 4.2 to experiment.
