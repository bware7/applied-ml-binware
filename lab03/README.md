# Lab 3: Titanic Survival Prediction

**Author:** Bin Ware  
**Date:** March 28, 2025  

## Overview
This project predicts Titanic passenger survival using Decision Trees, SVM, and Neural Networks. It tests three feature cases:  
1. `alone` (binary)  
2. `age` (continuous)  
3. `age + family_size` (combined)  

## Key Findings
- Best performance: Case 3 with Decision Tree (73% accuracy).  
- `age + family_size` outperformed single-feature cases.  
- SVC and NN struggled with limited features (e.g., 0% recall in Case 1).  

## Files
- `ml03_binware.ipynb`: Jupyter notebook with code, analysis, and results.  
- `decision_tree_titanic.png`: Decision Tree visualization for Case 3.  

## Requirements
- Python 3.x  
- Libraries: seaborn, pandas, numpy, matplotlib, scikit-learn  

## How to Run
1. Open `ml03_binware.ipynb` in Jupyter Notebook.  
2. Run all cells to replicate results for Case 3.  
3. Modify `X` and `y` in Section 3 to test Cases 1 and 2.