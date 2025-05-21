# M5Prime Insurance Premium Prediction

## Introduction
The `M5Prime` library, developed by Sylvain Marié, is a Python implementation of the M5P decision tree algorithm, originally proposed by Ross Quinlan. This project demonstrates the use of the M5Prime library to predict insurance premiums based on customer data. The library is actively being developed, with plans for future enhancements, including better support for categorical variables without requiring encoding. Currently, encoding is necessary for categorical features, as full support for handling them natively is not yet implemented.

This repository includes code to preprocess, analyze, and visualize insurance-related datasets, train an M5Prime model, and evaluate its performance. Two datasets are used: a custom dataset (`data_project.csv`) and a publicly available dataset from [Kaggle](https://www.kaggle.com/noordeen/insurance-premium-prediction). The goal is to predict the "Premium Amount" or "expenses" column using features like age, gender, occupation, and more.

## Features
- **Data Preprocessing**: Handling missing values, encoding categorical variables (one-hot and label encoding), and feature engineering (e.g., converting policy start dates to duration in days).
- **Exploratory Data Analysis (EDA)**: Visualizations of feature distributions and relationships with the target variable using Plotly, Matplotlib, and Seaborn.
- **Model Training**: Implementation of the M5Prime decision tree algorithm for regression tasks.
- **Model Evaluation**: Performance metrics including Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² score.
- **Cross-Dataset Validation**: Testing the model on a secondary dataset to evaluate generalizability.

## Datasets
1. **Primary Dataset (`data_project.csv`)**
   - Contains 27,884 rows and 20 columns with customer information.
   - Target variable: `Premium Amount`.
   - Features include age, gender, occupation, policy start date, and more.
   - Challenges: Significant missing values in some columns (e.g., Occupation, Previous Claims) and skewed target variable.

2. **Secondary Dataset (Kaggle Insurance Dataset)**
   - Source: [Kaggle](https://www.kaggle.com/noordeen/insurance-premium-prediction).
   - Contains 1,338 rows and 7 columns.
   - Target variable: `expenses`.
   - Features include age, sex, BMI, number of children, smoking status, and region.

## Installation
To run the code, you need to install the required dependencies and the `M5Prime` library manually, as it is not available via pip.

### Prerequisites
- Python 3.8+
- Required libraries:
  ```bash
  pip install numpy pandas sklearn plotly matplotlib seaborn

  
### Notes
- Replace `your-username` in the repository URL with your actual GitHub username.
- Ensure `data_project.csv` and `insurance.csv` are included in the repository or provide instructions for users to obtain them.
