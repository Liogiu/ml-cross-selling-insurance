# Cross-Selling Insurance Prediction

This project develops a machine learning model to predict whether an insurance customer is likely to purchase an additional vehicle insurance policy. The analysis includes exploratory data analysis (EDA), feature engineering, handling class imbalance, and model evaluation.

## Overview

Insurance companies often attempt to cross-sell additional vehicle insurance to existing customers. The objective of this project is to analyze customer characteristics and build predictive models that estimate the probability of a customer making an additional purchase.

The dataset used consists of 381,109 rows and 12 variables, including demographic features, vehicle-related information, and details about previous insurance status.

## Main Steps

### 1. Exploratory Data Analysis (EDA)
- Inspection of dataset structure and variable types.
- Distribution analysis of categorical and numerical variables.
- Analysis of the target variable imbalance.
- Identification of the most relevant predictors.

### 2. Data Preprocessing
- Removal of unnecessary columns.
- Label encoding of categorical variables.
- Ordinal encoding for ordered features (e.g., Vehicle Age).
- Scaling of numerical features using StandardScaler.

### 3. Handling Class Imbalance
Since the dataset is highly imbalanced (only a small percentage of customers purchase), several methods were tested:
- Class_weight parameter in Logistic Regression
- SMOTE oversampling
- Random undersampling

These approaches were compared in terms of precision, recall and balanced performance.

### 4. Model Training
The main model used is Logistic Regression.  
Models were trained on:
- Original data with class_weight balancing
- Oversampled (SMOTE) data
- Undersampled data

Performance was evaluated on a separate test set.

### 5. Evaluation Metrics
- Classification report (precision, recall, f1-score)
- Confusion matrix
- Business interpretation of false positives and false negatives

## Files in this Repository

- `cross_selling_insurance_analysis.ipynb`: Jupyter Notebook containing the full analysis, EDA, preprocessing, model training and evaluation.
- `insurance_cross_sell.csv` (not included): the dataset used for the project. If not available, instructions to download or reference the dataset should be added.

## How to Run the Notebook

1. Install the required libraries
2. Place the dataset file (`insurance_cross_sell.csv`) in the same directory as the notebook.
3. Open the notebook
4. Run the cells in order.

## Purpose of the Project

This project is part of my Data Science and Machine Learning training path. The goal is to demonstrate:
- Solid understanding of data preprocessing
- Ability to handle real-world imbalance problems
- Competence with supervised classification models
- Capability to evaluate models from both technical and business perspectives

## Author

Giulio Zerilli  
Data Analyst | Python and Machine Learning  

