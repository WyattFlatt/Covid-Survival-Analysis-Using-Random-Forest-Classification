# Covid Survival Analysis Using Random Forest Classification

## Overview

This project applies a Random Forest classification framework to predict
COVID-19 patient survival outcomes using demographic and clinical data.
The analysis focuses on identifying relationships between patient characteristics
and mortality outcomes while evaluating the predictive performance of ensemble
machine learning methods.

In addition to predictive modeling, the project includes exploratory data
analysis, conditional probability analysis, preprocessing, and
feature preparation techniques to improve model reliability and interpretability.

## Dataset

The dataset consists of COVID-19 patient records reported to the Centers for Disease Control and Prevention
from across the United States and it contains demographic,
hospitalization, and symptom-related variables. Features used for analysis include:

- age group
- sex
- race
- ethnicity
- hospitalization status
- ICU status
- symptom status
- current case status
- death status

Observations with confirmed survival outcomes were retained for analysis,
and missing values were handled through preprocessing and imputation methods.

🔗 **View Data:**
https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-with-Ge/n8mc-b4w4/about_data

## Methods

- Exploratory data analysis (EDA)
- Conditional probability analysis
- Data preprocessing and cleaning
- Missing value handling and mode imputation
- Feature encoding using categorical factors
- Stratified train/test splitting
- Random Forest classification
- Model evaluation and prediction analysis

## Models
- **Random Forest Classifier:** Used as the primary ensemble learning model to
capture nonlinear relationships and interactions between demographic and
clinical variables associated with COVID-19 mortality risk. Two cross-validation classifiers were
created: one optimized for accuracy and one optimized for sensitivity.

## Results
The Random Forest classification framework demonstrated very strong predictive
capabilities in identifying COVID-19 survival outcomes using structured
clinical and demographic data. The accuracy-optimized model achieved an accuracy of 
87.39 percent and sensitivity of 95.92 percent, and the sensitivity-optimized model 
achieved an accuracy of 86.99 percent and a sensitivity of 96.30 percent. This means that 
both models were able to accurately predict patients' death statuses with high accuracy while performing
even better on patients who did not survive, making them highly appropriate for
a healthcare-style setting in which those who will die are of higher priority.

Conditional probability and feature importance analysis highlighted meaningful relationships between
mortality risk and patient characteristics such as hospitalization status,
ICU admission, and demographic variables, indicating potential risk factors.


## Technologies
- R
- tidyverse
- caret
- randomForest
- ranger
- ggplot2
- sqldf
- rsample
- stringr
- R Markdown

## Structure
- covid_survival_analysis.Rmd - Main analysis and modeling code
- Covid Survival Analysis.pdf - Final analysis report
- Requirements.txt - R dependencies

## Notes
This project was completed as part of a machine learning and predictive
analytics study and is accompanied by a research paper discussing the
methodology, preprocessing decisions, exploratory analysis, and predictive
modeling results in greater detail.