# Lab 4: Titanic Fare Prediction

**Author:** Bin Ware  
**Date:** April 04, 2025  

## Overview
This project predicts Titanic passenger fares (a continuous target) using regression models: Linear Regression, Ridge, ElasticNet, and Polynomial Regression. It tests four feature cases:  
1. `age` (continuous)  
2. `family_size` (continuous)  
3. `age + family_size` (combined)  
4. `age + family_size + sex_numeric` (combined with binary sex)  

## Key Findings
- Best performance: Case 4 with Linear Regression (R² = 0.119, RMSE = 35.70).  
- `age + family_size + sex_numeric` outperformed simpler cases, though R² remains low due to fare variance.  
- Ridge tied Linear (R² = 0.119), ElasticNet slightly worse (R² = 0.101), and Polynomial (degree 3) failed (R² = -0.003).  
- Fare’s high variance and outliers limited model accuracy across all cases.

## Files
- `ml04_binware.ipynb`: Jupyter notebook with code, analysis, and results.  

## Requirements
- Python 3.x  
- Libraries: seaborn, pandas, numpy, matplotlib, scikit-learn  

## How to Run
1. Open `ml04_binware.ipynb` in Jupyter Notebook.  
2. Run all cells to replicate results, focusing on Case 4 (best performer).  
3. Modify `X` and `y` in Section 4 to test Cases 1, 2, or 3.  
4. Adjust model parameters (e.g., `alpha` in Ridge/ElasticNet, `degree` in Polynomial) in Section 5 for experimentation.
