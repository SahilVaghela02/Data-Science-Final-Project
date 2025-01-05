## Important Libraries
- sklearn.metrics
- sklearn.preprocessing
- sklearn.model_selection
- sklearn.ensemble
- sklearn.linear_model
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- fuzzywuzzy
- xgboost

## Overview
This project focuses on analyzing GPU specifications and modeling CUDA benchmark scores using machine learning techniques. 
It integrates multiple datasets, performs data preprocessing, exploratory data analysis (EDA), and builds predictive models to estimate performance metrics.

## Datasets
- **GPU Specifications Dataset (`gpu_specs_v6.csv`)**:
  - Contains GPU details such as core clock, memory type, memory size, and bandwidth.
  - Link: https://www.kaggle.com/datasets/alanjo/graphics-card-full-specs/data
- **Benchmark Scores Dataset (`GPU_scores_graphicsAPIs.csv`)**:
  - Provides benchmark scores (CUDA, OpenCL, etc.) for various GPUs.
  - Link: https://www.kaggle.com/datasets/alanjo/gpu-scores-with-cuda-metal-opencl-vulkan

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

##  Results:
- XGBoost performed better than all the other models with an R2 score of 0.75.

## Limitations:
- There are certain limitations for this project the first one is dataset which has more details like TDP and Thermal Performance.
- There were no full specifications on which the GPU was tested i.e. with which CPU it was paired and how much was the memory avaiable while testing for benchmarks.
