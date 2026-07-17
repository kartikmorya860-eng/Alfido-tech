# Loan Approval Prediction

This project focuses on building a machine learning model to predict whether a loan application will be approved or rejected based on applicant-related information.

## Project Overview

The notebook in this folder, Loan_Approval_Predicition.ipynb, performs an end-to-end machine learning workflow for loan approval prediction. It includes:

- Loading and exploring the loan dataset
- Checking missing values and data quality
- Performing exploratory data analysis (EDA)
- Preparing features for model training
- Encoding categorical variables
- Scaling numerical features
- Handling class imbalance using SMOTE
- Training and comparing multiple classification models
- Selecting the best-performing model for prediction

## Objective

The main goal of this project is to help financial institutions make faster and more consistent loan approval decisions by using historical applicant data.

## Dataset

The dataset used in this project is stored in:

- loan_prediction.csv

It contains information such as:

- Applicant income
- Co-applicant income
- Loan amount
- Loan amount term
- Credit history
- Property area
- Marital status
- Education level
- Employment status
- Loan approval status

## Workflow

The notebook follows these major steps:

1. Importing required Python libraries
2. Loading the dataset
3. Understanding the structure of the data
4. Exploring missing values and duplicates
5. Visualizing distributions and relationships between features
6. Cleaning and preprocessing the data
7. Splitting data into training and testing sets
8. Encoding categorical features
9. Scaling numerical features
10. Balancing the training dataset using SMOTE
11. Training classification models
12. Evaluating performance using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC
13. Selecting the best model for final use

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- imbalanced-learn (SMOTE)

## Installation

Install the required Python packages using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

## How to Run

Open the notebook file:

- Loan_Approval_Predicition.ipynb

Run the cells in order to:

- load the dataset
- perform analysis
- train the machine learning models
- view evaluation results

## Expected Outcome

This project aims to build a predictive model that can estimate whether a loan applicant is likely to be approved based on available applicant information.

## Notes

The notebook focuses on practical machine learning steps for classification problems and is designed as an internship-style data science project.
