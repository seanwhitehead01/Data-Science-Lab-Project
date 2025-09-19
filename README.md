# Data-Science-Lab-Project
Implementation of a machine learning pipeline to predict hit positions with Resistive Silicon Detectors (RSD), combining data preprocessing, regression models, and sensor-specific optimizations for spatial accuracy.
We designed and implemented a complete pipeline, from raw data exploration to optimized model deployment:

## Data preprocessing:
Cleaning, merging development and evaluation datasets, and removing redundant or highly correlated features (area, tmax, rms, selected pmax and negpmax indices).

## Exploratory analysis: 
Conducted correlation studies, boxplots, and heatmaps to identify relevant sensor features impacting prediction accuracy.

## Modeling: 
Built multi-output regression models to simultaneously predict both spatial coordinates (x, y).

## Optimization: 
Performed extensive grid search tuning of tree-based models (Random Forest, Extra Trees), comparing performance across n_estimators, max_depth, and splitting criteria.

## Final model: 
Selected Extra Trees Regressor with tuned hyperparameters (n_estimators=700, max_depth=29, criterion=friedman_mse), which significantly reduced prediction error compared to baseline models.

The project demonstrates how machine learning and sensor-specific feature engineering can enhance the reconstruction of hit positions in particle physics experiments, contributing to more precise measurements in future applications.
