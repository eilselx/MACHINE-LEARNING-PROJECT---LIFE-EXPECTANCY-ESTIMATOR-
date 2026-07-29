# Predicting Life Expectancy Using National Health Indicators: A Machine Learning Approach

## Project Overview

Life expectancy is one of the most widely used indicators of a country's overall health and development. It is influenced by numerous demographic, socioeconomic, healthcare, and environmental factors. Understanding these relationships enables governments and healthcare organizations to make informed policy decisions and allocate healthcare resources more effectively.

This project develops and compares several machine learning regression models to predict life expectancy using national health indicators obtained from the World Health Organization (WHO). The complete machine learning workflow was implemented, including data preprocessing, exploratory data analysis, feature engineering, model development, evaluation, and interpretation.

---

## Objectives

The objectives of this project were to:

- Predict life expectancy using national health indicators.
- Compare the performance of multiple machine learning regression algorithms.
- Identify the factors that contribute most to life expectancy.
- Select the best-performing predictive model.
- Interpret the model's predictions using feature importance analysis.

---

## Dataset

The project uses the **WHO Health Indicators Dataset**, which contains country-level information describing healthcare, demographic, economic, and environmental conditions.

The dataset includes indicators such as:

- Under-five mortality
- Maternal mortality
- Neonatal mortality
- GDP per capita
- Health expenditure
- Immunization coverage
- Birth rate
- Death rate
- Tuberculosis incidence
- Access to sanitation
- Access to safe drinking water
- Physicians per 1,000 population
- Hospital beds per 1,000 population

The target variable is:

**Life Expectancy**

---

## Machine Learning Workflow

The project follows a complete end-to-end machine learning pipeline.

### 1. Data Cleaning

- Missing value treatment
- Duplicate removal
- Outlier inspection
- Data consistency checks

### 2. Exploratory Data Analysis

- Summary statistics
- Feature distributions
- Correlation analysis
- Outlier visualization

### 3. Feature Engineering

Several meaningful features were created to improve predictive performance, including:

- Disease Burden Ratio
- Overall Immunization Index
- Log transformation of highly skewed variables

### 4. Data Leakage Prevention

To ensure reliable model evaluation:

- Target leakage variables (`life_expectancy_male` and `life_expectancy_female`) were removed.
- The dataset was split into training and testing sets before feature engineering.
- Feature engineering was applied independently to the training and testing datasets.

### 5. Model Development

Five regression algorithms were trained and evaluated:

- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Gradient Boosting Regression
- XGBoost Regression

---

## Model Evaluation

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R²)

### Model Performance

| Model | MAE | RMSE | R² |
|------|------:|------:|------:|
| **XGBoost** | **0.423** | **0.701** | **0.9936** |
| Random Forest | 0.429 | 0.734 | 0.9930 |
| Decision Tree | 0.632 | 1.064 | 0.9853 |
| Gradient Boosting | 0.844 | 1.121 | 0.9837 |
| Linear Regression | 1.365 | 1.824 | 0.9569 |

---

## Best Model

Among all evaluated algorithms, **XGBoost** achieved the best performance.

It produced:

- Highest R²
- Lowest MAE
- Lowest RMSE

Therefore, XGBoost was selected as the final predictive model.

---

## Feature Importance

Feature importance analysis identified the most influential predictors of life expectancy.

The five most important features were:

1. Under-five mortality
2. Maternal mortality
3. GDP per capita
4. Death rate
5. Sanitation coverage

These findings are consistent with public health research, demonstrating that child survival, maternal health, economic development, and sanitation play major roles in determining life expectancy.

---

## Model Validation

Model performance was further evaluated using:

- Actual vs Predicted scatter plot
- Residual distribution
- Residuals vs Predicted Values

The results showed:

- Predictions closely aligned with actual values.
- Residuals were centered around zero.
- No systematic prediction bias was observed.
- Only a small number of outliers were identified.

These findings indicate that the selected model generalizes well to unseen data.

---

## Discussion

The project demonstrates that machine learning can accurately predict life expectancy using national health indicators. XGBoost significantly outperformed the other regression models by effectively capturing complex nonlinear relationships within the data.

Feature importance analysis confirmed that indicators related to child mortality, maternal health, economic development, and sanitation have the greatest influence on life expectancy. These findings align with established public health knowledge and highlight the importance of investments in healthcare systems, maternal and child health services, sanitation infrastructure, and economic development.

---

## Limitations

Although the model achieved excellent predictive performance, several limitations should be considered:

- The analysis relies on historical WHO data.
- Some determinants of life expectancy (e.g., genetics, environmental factors, political stability, lifestyle) were not included.
- Machine learning models identify predictive relationships but do not establish causation.

---

## Conclusion

This project successfully developed an accurate machine learning model for predicting life expectancy using national health indicators.

Among the evaluated models, XGBoost achieved the highest predictive performance with an R² score of **0.9936** while maintaining very low prediction errors.

The results demonstrate the potential of machine learning to support public health planning and policy by identifying the key factors associated with life expectancy.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## Repository Structure



---

## Future Improvements



---

## Author



MSc Digital Health and Data Science  
SRH University, Germany
