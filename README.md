# Student Performance Analysis using Multiple Linear Regression

## Project Overview

This project implements a multiple linear regression analysis to predict and analyze student performance based on various factors. The implementation includes a custom Multiple Linear Regression class built from scratch, along with comprehensive statistical analysis and visualization tools.

## Features

- Custom Multiple Linear Regression implementation
- Comprehensive statistical analysis (ANOVA, F-tests)
- 3D visualization of regression planes
- Performance metrics calculation
- Data preprocessing and exploration tools

## Project Structure

```plaintext
├── Student_Performance_Analysis.ipynb  # Main analysis notebook
├── Student_Performance.csv            # Dataset
└── README.md                         # Project documentation
```

## Implementation Details

### 1. Data Preparation & Exploration

- Data cleaning and preprocessing
- Feature correlation analysis
- Exploratory data visualization

### 2. Custom MLR Implementation

The `MultipleLinearRegression` class includes:

- Normal equation for coefficient calculation
- Statistical measures (R², MSE, F-statistic)
- 3D visualization capabilities
- ANOVA table generation
- Hypothesis testing

### 3. Model Features

Selected features based on correlation analysis:

- Previous Scores
- Hours Studied

Target variable:

- Performance Index

### 4. Statistical Analysis

- ANOVA (Analysis of Variance)
- F-test for model significance
- R-squared and adjusted R-squared
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)

## Requirements

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy

## Usage

1. Open the Jupyter notebook `Student_Performance_Analysis.ipynb`
2. Ensure the dataset `Student_Performance.csv` is in the same directory
3. Run the cells sequentially to:
   - Load and preprocess the data
   - Train the multiple linear regression model
   - Visualize results
   - Perform statistical analysis

## Results

The analysis provides:

- Prediction accuracy metrics
- Statistical significance tests
- Visual representation of the regression model
- Correlation analysis between variables

## Model Evaluation

Performance metrics include:

- R-squared (R²) for model fit
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- F-statistics and p-values
