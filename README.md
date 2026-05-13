# House Price Estimation Using Gradient Boosting


## Overview
This project applies a gradient boosting framework to estimate residential
house prices using structured housing data as a part of a Kaggle competition. 
Cross-validation hyperparameter tuning was used to choose a Gradient Boosting Regression model

In addition to predictive modeling, the project includes exploratory data
analysis, feature engineering, and preprocessing pipelines to improve model reliability and interpretability.

## Dataset
The dataset consists of residential housing features such as property size,
location-related variables, structural characteristics, and other attributes
commonly associated with home valuation from homes in Ames, Iowa.


## Methods
- Exploratory data analysis (EDA)
- Data preprocessing and cleaning
- Feature engineering and transformation
- Pipeline imputation and feature encoding
- Train/test splitting
- Cross-validation
- Hyperparameter tuning
- Regression modeling

## Models
- **Gradient Boosting Regressor:** Used as the primary predictive model framework to
improve estimation accuracy and capture complex feature interactions
- **Stochastic Gradient Boosting Regressor:** A gradient boosting regressor variant
used to further reduce overfitting

## Results
A Stochastic Gradient Boosting Regressor was chosen as the RMSE-minimizing model via cross-validation.
This model was used to predict the sales prices of houses in the testing data provided by the
Kaggle competition. The result was an RMSE of .12859 between the log of prediction prices
and the log of the true observed prices, resulting in a relatively good competition placement.

The project highlights how ensemble learning methods can effectively model
house pricing behavior using structured tabular data.

## Technologies
- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Structure
- House_Price_Estimation.ipynb - Main analysis and results notebook
- House Price Estimation.pdf - Analysis report
- Requirements.txt - Python dependencies

## Notes
This project was completed as part of a machine learning project and is
accompanied by a paper discussing the methodology, modeling
approach, preprocessing decisions, and predictive performance results in
greater detail.