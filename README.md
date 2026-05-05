# Kernel SVM from Scratch

This project implements a **Kernel Support Vector Machine (SVM)** from scratch using Python, without relying on high-level machine learning libraries.

## Overview
The goal of this project is to understand the inner workings of Support Vector Machines by implementing the dual optimization formulation and the RBF kernel from first principles.

The model is evaluated on a binary classification dataset (MAGIC Gamma Telescope).

## Method
- Implemented SVM dual optimization manually using NumPy
- Applied the **RBF (Gaussian) kernel** for non-linear classification
- Tuned hyperparameters including:
  - Regularization parameter (C)
  - Kernel width (γ)
  - Learning rate and optimization settings

## Results
- Achieved approximately **87% test accuracy**
- Demonstrated that RBF kernels can effectively separate non-linear data
- Observed sensitivity of performance to γ and learning rate

## Tech Stack
- NumPy for numerical computation
- Pandas for data handling
- Matplotlib for visualization
- Scikit-learn (limited use for dataset loading, evaluation, and hyperparameter tuning)

## Dataset
- MAGIC Gamma Telescope dataset (~19,000 samples, 10 features)
- Binary classification: gamma rays vs hadronic showers

## Key Insights
- Kernel SVM significantly improves performance over linear separation
- Proper tuning of γ is critical for generalization
- Gradient-based dual optimization is sensitive but effective when stabilized

## Repository Structure
- `kernel-svm-from-scratch.ipynb` – full implementation and experiments

## Next Steps
- Compare with scikit-learn SVM implementation
- Improve optimization stability and convergence speed
- Extend to multiclass classification
