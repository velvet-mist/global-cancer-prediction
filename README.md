# global-cancer-prediction

Cancer Survival Prediction using Machine Learning

This project presents a complete end-to-end machine learning pipeline to analyze and predict 5-year cancer survival outcomes using demographic, clinical, lifestyle, and socioeconomic data.
The study emphasizes structured exploratory data analysis (EDA), feature selection, and model comparison with a focus on interpretability and performance.

Problem Statement

Cancer survival is influenced by a complex interaction of clinical severity, early detection, treatment access, and socioeconomic factors.
This project aims to:

Identify key factors affecting 5-year survival

Reduce redundancy among predictors

Build and compare predictive models

Justify model choice using statistical and ML-based evidence


Dataset Overview

Records: 167,497 patients

Features: 28 variables

Target Variable: Survival_5_years (binary)

Feature Categories

Demographic: Age, Gender, Urban/Rural, Country

Clinical: Cancer Stage, Tumor Size, Genetic Mutation, Comorbidities

Lifestyle: Smoking, Alcohol, BMI, Diet, Physical Activity

Screening & Detection: Screening History, Early Detection

Treatment & Cost: Treatment Type, Healthcare Costs

Socioeconomic: Economic Classification, Insurance, Healthcare Access

Methodology
1- Variable Audit & Grouping

Classified features into conceptual groups

Removed identifiers and leakage-prone variables

Selected Survival_5_years as the primary target

2- Exploratory Data Analysis (EDA)

Univariate analysis (distribution, skewness, outliers)

Target-based bivariate analysis

Survival rate comparisons across categories

3- Multicollinearity Analysis

Correlation matrix

Variance Inflation Factor (VIF)

Result: No severe multicollinearity detected

4- Feature Importance & Selection

Random Forest feature importance

Identified dominant predictors:

Cancer Stage

Tumor Size

Early Detection

Treatment Type

Healthcare Access

5- Model Building & Comparison

Logistic Regression (baseline, interpretable)

Random Forest Classifier (non-linear, high performance)

Models & Evaluation
Model	Strengths	Outcome
Logistic Regression	Interpretability	Moderate performance
Random Forest	Captures non-linear interactions	Best ROC-AUC & Recall

Final Model Selected: Random Forest
Justified by superior performance across multiple metrics.
