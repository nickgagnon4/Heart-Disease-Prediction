# Heart-Disease-Prediction
## Project Overview

### Heart disease remains the #1 global cause of death. Early detection is essential to prevent complications and improve patient outcomes.
### This project applies machine learning to a cleaned version of a popular heart disease dataset, originally sourced from Kaggle.

### The project includes:

### Data cleaning & validation

### Exploratory data analysis (EDA)

### One-hot encoding & feature scaling

### Multiple ML models

### Model evaluation with ROC curves, confusion matrices, and cross-validation

### Feature importance analysis

### A custom risk binning strategy to categorize patients by risk level

## Data Cleaning & Preprocessing
### Duplicate Removal

### The original dataset contained 1,025 rows, but 723 were duplicates.
### After removing duplicates, 302 unique patient records remained.

### Feature Engineering

### One-hot encoding applied to: sex, cp, fbs, restecg, exang, slope, ca

### Standardization applied to numerical features:
### age, trestbps, chol, thalach, oldpeak

### Implemented a custom risk binning strategy:
### High Risk → low max heart rate, high ST depression, severe chest pain  
### Review Needed → ambiguous cases  
### Low Risk  → high exercise capacity, low ST depression, non-anginal chest pain

## Exploratory Data Analysis

### The notebook includes:

### Correlation heatmap

### Chest pain type vs. disease

### Max heart rate distributions

### Histograms of age & cholesterol

### Key insights:

### Cholesterol, chest pain type, age, ST depression, and max heart rate emerged as strong predictors.

### Heart disease patients tended to have lower exercise capacity and higher ST depression.

## Models Implemented

### Three models were trained and evaluated without pipelines for transparency:

### 1. Logistic Regression

### Best recall (0.897) — safest model for medical screening

### Easy to interpret

### 2. Random Forest

### Best overall accuracy (0.852)

### Strong feature interpretability

### 3. Gradient Boosting

### Competitive performance

### Good at capturing nonlinear relationships

## Model Evaluation
### Metrics recorded:

### Accuracy

### Precision

### Recall

### F1 Score

### ROC AUC

### 5-fold cross-validation mean & std

### Visuals Included

### ROC Curves

### Confusion Matrices

### Feature Importance Charts
