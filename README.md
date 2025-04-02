# Predicting Housing Prices with Machine Learning

This project aims to predict housing prices using machine learning models. The dataset contains various features such as crime rate, property tax, number of rooms, and more. The goal is to develop a predictive model using algorithms like Linear Regression, Random Forest, and XGBoost to predict house prices based on these features.

## Project Overview

The main objective of this project is to predict housing prices using machine learning models. The dataset used contains features such as crime rate, property tax, number of rooms, and more, with the target variable being the house price.

## Dataset

The dataset used in this project is a well-known housing dataset containing various features about homes. The dataset includes the following columns:

- **CRIM**: Crime rate
- **ZN**: Proportion of residential land zoned for large lots
- **INDUS**: Proportion of non-retail business acres per town
- **CHAS**: Charles River dummy variable (1 if tract bounds river, 0 otherwise)
- **NOX**: Nitrogen oxides concentration (parts per 10 million)
- **RM**: Average number of rooms per dwelling
- **AGE**: Proportion of owner-occupied units built before 1940
- **DIS**: Weighted distance to employment centers
- **RAD**: Index of accessibility to radial highways
- **TAX**: Property tax rate per $10,000
- **PTRATIO**: Pupil-teacher ratio by town
- **B**: Proportion of Black residents
- **LSTAT**: Percentage of lower status population

## Models Used

This project uses three machine learning models to predict housing prices:

1. **Linear Regression**: A basic regression model used as a baseline.
2. **Random Forest Regressor**: An ensemble learning method for regression that constructs multiple decision trees.
3. **XGBoost Regressor**: A more advanced boosting model designed for performance and speed.

## Performance Evaluation

The models are evaluated using two key metrics:

- **Root Mean Squared Error (RMSE)**: Measures the difference between predicted and actual values.
- **R² Score**: Indicates how well the model explains the variance in the data.

The following are the performance results:

- **Linear Regression**:  
  - RMSE = 6.2187  
  - R² = 0.4727
- **Random Forest**:  
  - RMSE = 2.7582  
  - R² = 0.8963
- **XGBoost**:  
  - RMSE = 2.7880  
  - R² = 0.8940

The Random Forest and XGBoost models performed significantly better than Linear Regression, achieving higher R² scores and lower RMSE.

## Feature Importance

To understand which features are most important for predicting house prices, we visualized feature importances for the Random Forest and XGBoost models. The following features were found to be most important:

- **RM** (Average number of rooms per dwelling)
- **LSTAT** (Percentage of lower status population)

These features have the highest impact on the model's predictions.

## Conclusion

In this project, we successfully predicted housing prices using machine learning techniques. The Random Forest and XGBoost models outperformed Linear Regression, demonstrating the power of tree-based algorithms in regression tasks. By analyzing feature importance, we identified key features that influence house prices the most, such as the average number of rooms and the percentage of lower-status population.

The project showcases the importance of selecting the right model and understanding the key features that drive predictions in machine learning.

## Requirements

To run this project, you need the following libraries:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- xgboost
