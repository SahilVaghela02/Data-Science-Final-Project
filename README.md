## Overview
This project focuses on analyzing GPU specifications and modeling CUDA benchmark scores using machine learning techniques. 
It integrates multiple datasets, performs data preprocessing, exploratory data analysis (EDA), and builds predictive models to estimate performance metrics.

## Features
- **Data Cleaning and Feature Engineering**:
  - Handles missing values and standardizes memory type mappings.
  - Computes derived features such as memory bandwidth.
- **Exploratory Data Analysis (EDA)**:
  - Visualizes data distributions using histograms, bar charts, scatter plots, and more.
- **Predictive Modeling**:
  - Trains and evaluates models including:
    - XGBoost
    - Random Forest
    - Gradient Boosting
    - Linear Regression
  - Optimizes hyperparameters and identifies feature importance.
- **Performance Metrics**:
  - Outputs RMSE,MAE and R² scores for train and test sets.

## Datasets
- **GPU Specifications Dataset (`gpu_specs_v6.csv`)**:
  - Contains GPU details such as core clock, memory type, memory size, and bandwidth.
- **Benchmark Scores Dataset (`GPU_scores_graphicsAPIs.csv`)**:
  - Provides benchmark scores (CUDA, OpenCL, etc.) for various GPUs.
