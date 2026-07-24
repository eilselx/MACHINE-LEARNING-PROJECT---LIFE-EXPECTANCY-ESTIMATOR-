# Predicting Life Expectancy Using National Health Indicators: A Machine Learning Approach

## Overview

This project is part of the **Statistics and Machine Learning** course. The objective is to develop a machine learning model that predicts the **life expectancy of a country** using national health, demographic, economic, and healthcare indicators obtained from the WHO Health Indicators dataset.

The project follows the complete machine learning workflow taught in class, from problem definition and data exploration to model development and evaluation.

---

# Problem Definition

Life expectancy is one of the most important indicators of a country's overall health and development. It is influenced by numerous factors, including healthcare access, disease burden, economic conditions, sanitation, healthcare expenditure, and lifestyle.

Understanding how these factors contribute to life expectancy is essential for governments and public health organizations to make informed decisions and allocate healthcare resources effectively.

Traditional statistical methods often struggle to capture the complex relationships between these variables. Machine learning provides a data-driven approach capable of learning these relationships and generating accurate predictions.

---

# Project Goal

The goal of this project is to build a machine learning model capable of predicting a country's **life expectancy** using a variety of national health indicators.

The project also aims to identify the most influential factors affecting life expectancy and compare the performance of multiple machine learning algorithms.

---

# Research Question

**Can machine learning accurately predict a country's life expectancy using demographic, healthcare, economic, and public health indicators?**

---

# Dataset

**Dataset:** WHO Health Dataset – 43+ Health Indicators, 200 Countries

The dataset contains health-related indicators collected across multiple countries over several years, including:

- Population demographics
- GDP per capita
- Healthcare expenditure
- Physician density
- Hospital beds
- Mortality indicators
- Immunization coverage
- Disease prevalence
- Smoking prevalence
- Obesity rates
- Sanitation and clean water access
- Life expectancy (Target Variable)

---

# Machine Learning Workflow

This project follows the workflow presented in class:

1. Problem Definition
2. Data Collection & Understanding
3. Data Cleaning & Preprocessing
4. Exploratory Data Analysis (EDA)
5. Statistical Analysis
6. Feature Engineering
7. Model Selection
8. Model Training
9. Model Evaluation
10. Final Report & Presentation

---

# Machine Learning Task

**Problem Type:** Regression

### Input Features (X)

Examples include:

- GDP per capita
- Health expenditure
- Physicians per 1,000 people
- Hospital beds per 1,000 people
- Immunization coverage
- Maternal mortality
- Under-5 mortality
- Smoking prevalence
- Obesity prevalence
- Population
- Sanitation coverage
- Safe drinking water access
- Other national health indicators

### Target Variable (Y)

- **Life Expectancy**

---

# Machine Learning Models

To identify the most suitable algorithm for predicting life expectancy, multiple regression models will be trained, evaluated, and compared.

The models include:

- Linear Regression (Baseline Model)
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

Each model will be evaluated using the same training and testing data and compared based on:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The model that achieves the best predictive performance while maintaining good generalization will be selected as the final model.

# Expected Outcomes

By the end of this project, we aim to:

- Develop an accurate life expectancy prediction model.
- Identify the most influential health indicators affecting life expectancy.
- Compare the performance of different machine learning algorithms.
- Provide insights that could support evidence-based public health planning and policy decisions.

---

# Team Members & Responsibilities

| Team Member | Responsibility |
|--------------|----------------|
| **Shikhin** | Problem Definition, Data Collection, Dataset Understanding, Data Dictionary |
| **Lavanya** | Data Cleaning, Preprocessing, Exploratory Data Analysis (EDA), Data Visualization |
| **Advait** | Statistical Analysis, Correlation Analysis, Feature Engineering, Feature Selection |
| **Leslie Wambo Laghom** | Machine Learning Model Development, Model Training, Hyperparameter Tuning, Model Comparison |
| **Omar** | Model Evaluation, Feature Importance Analysis, Final Report, Presentation Preparation |

---

# Repository Structure

```
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── src/
│   ├── preprocessing.py
│   ├── feature_engineering.py
│   ├── train_models.py
│   ├── evaluate_models.py
│
├── reports/
│
├── presentation/
│
├── figures/
│
├── README.md
│
└── requirements.txt
```

---

# Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

# Supervisor

**Statistics and Machine Learning**

SRH University – Summer Semester

---
