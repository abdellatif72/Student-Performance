# Student Performance Multiple Linear Regression

## Project Overview

This project analyzes and predicts student performance using a custom-built multiple linear regression model implemented entirely from scratch in Python. Utilizing a dataset of 10,000 student records, the goal was to identify the key academic drivers of performance and quantify their impact without relying on pre-built machine learning libraries for the core algorithm. The project encompasses full exploratory data analysis, mathematical implementation of regression via the normal equation, and comprehensive statistical significance testing to validate the model's predictive power.

## Key Technical Steps

- **Data Cleaning & Preprocessing:** Processed 10,000 records by identifying and removing 127 duplicate entries, and converted categorical variables like 'Extracurricular Activities' into numeric binary features for analysis.
- **Exploratory Data Analysis (EDA):** Generated a correlation matrix heatmap using `seaborn` to quantify relationships between variables, identifying "Previous Scores" and "Hours Studied" as the most highly correlated features with the target variable.
- **Algorithm Engineering:** Developed an object-oriented `MultipleLinearRegression` class from scratch using `numpy` matrix operations to solve the normal equation ($\beta = (X^T X)^{-1} X^T y$), completely bypassing standard modeling libraries.
- **Statistical Analysis:** Engineered custom functions to calculate and generate an ANOVA (Analysis of Variance) table, deriving SSR, SSE, Mean Squared Error (MSE), F-statistics, and p-values to rigorously test the null hypothesis.
- **3D Visualization:** Created interactive 3D surface plots using `matplotlib` to visually demonstrate how the regression plane fits the multidimensional relationship between the two independent variables and the predicted performance index.

## Results

- Built a highly accurate predictive model achieving an **$R^2$ of 0.9850**, explaining 98.5% of the variance in student performance.
- Evaluated model error on a 20% holdout test set, yielding a **Mean Squared Error (MSE) of 5.57** and a **Mean Absolute Error (MAE) of 1.88** on the performance index scale.
- Confirmed the statistical significance of the model through rigorous F-testing, yielding a p-value strictly below the 0.05 alpha threshold, decisively rejecting the null hypothesis.

## Technologies Used

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Statistical Testing:** `scipy.stats`
- **Visualization:** `matplotlib`, `seaborn`
- **Evaluation:** `scikit-learn` (for train/test splitting and benchmark metric validation)
