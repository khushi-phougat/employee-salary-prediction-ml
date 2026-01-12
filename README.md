# Employee Salary Prediction using Machine Learning

## Overview
This project focuses on predicting employee salaries using supervised machine learning techniques. A regression model is trained on structured employee data to estimate salary values based on demographic and professional attributes.

The project demonstrates the complete machine learning workflow, including data preprocessing, model training, evaluation, and result interpretation.

## Dataset
The dataset contains employee-related information such as:
- Age  
- Gender  
- Education Level  
- Job Title  
- Years of Experience  
- Salary (target variable)

The data is extracted from a ZIP file and loaded into a pandas DataFrame. Missing values are handled before model training.

## Methodology

### 1. Data Preprocessing
- Missing numerical values handled using median imputation  
- Missing categorical values handled using mode imputation  
- Categorical variables encoded using One-Hot Encoding  
- Numerical features passed without scaling  

### 2. Model Pipeline
- `ColumnTransformer` used to apply preprocessing steps  
- `Pipeline` integrates preprocessing and model training  
- Linear Regression used as the prediction model  

### 3. Train–Test Split
- Dataset split into 80% training and 20% testing data  

## Model Evaluation
Model performance is evaluated using multiple regression metrics:
- **R² Score** – measures how much variance in salary is explained by the model  
- **Mean Absolute Error (MAE)** – average absolute prediction error  
- **Mean Squared Error (MSE)** and **Root Mean Squared Error (RMSE)** – measure prediction deviation and penalize large errors  

Printed interpretations are included to explain what each metric indicates about model performance.

## Visual Analysis
To further assess model behavior, the following visualizations are used:
- **Actual vs Predicted Salary Plot** to observe prediction accuracy  
- **Residual Plot** to detect bias and variance patterns  
- **Histogram of Salaries** to understand data distribution  

These plots help validate whether the model assumptions are reasonable.

## User Interaction
The program allows users to input employee details such as age, years of experience, education level, job title, and gender. Based on the trained model, the system predicts an expected salary.

## Tools & Technologies
- Python  
- pandas  
- NumPy  
- scikit-learn  
- matplotlib  
- seaborn  

## Limitations
- The model is trained on a limited dataset and may not generalize across industries or regions.  
- Salary prediction depends on factors not included in the dataset, such as company size and market conditions.  
- Linear regression may not capture complex non-linear relationships.  

## Conclusion
This project demonstrates an end-to-end implementation of a machine learning regression model, including preprocessing, training, evaluation, visualization, and prediction. It serves as a foundational machine learning project with strong emphasis on interpretability and evaluation.
