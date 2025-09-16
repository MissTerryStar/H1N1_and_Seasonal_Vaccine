# H1N1_and_Seasonal_Vaccine
# Predict H1N1 and Seasonal Flu Vaccines

## Overview
This project aims to predict whether individuals received the H1N1 or seasonal flu vaccine using data from the 2009 H1N1 Flu Survey. By analyzing demographic, social, behavioral, and opinion-based factors, the project seeks to provide insights that can inform public health strategies and improve vaccination campaigns.

## Table of Contents
1. [Business Understanding](#business-understanding)
2. [Problem Statement](#problem-statement)
3. [Objectives](#objectives)
4. [Data Science Goal](#data-science-goal)
5. [Metrics of Success](#metrics-of-success)
6. [Data Understanding](#data-understanding)
7. [Data Preparation](#data-preparation)
8. [Exploratory Data Analysis](#exploratory-data-analysis)
9. [Modeling](#modeling)
10. [Conclusion](#conclusion)
11. [Future Work](#future-work)
12. [Installation and Usage](#installation-and-usage)

## Business Understanding
Vaccination is one of the most effective public health strategies for preventing the spread of infectious diseases. However, vaccine uptake varies significantly across different populations due to factors such as personal beliefs, risk perception, health behaviors, and access to healthcare. This project leverages data from the 2009 H1N1 Flu Survey to explore these patterns.

## Problem Statement
The primary goal of this project is to predict whether an individual received the H1N1 or seasonal flu vaccine based on various factors. The dataset includes two target variables:
- **h1n1_vaccine**: 0 (Did not receive H1N1 vaccine) or 1 (Received H1N1 vaccine)
- **seasonal_vaccine**: 0 (Did not receive seasonal flu vaccine) or 1 (Received seasonal flu vaccine)

## Objectives
1. Predict H1N1 and seasonal flu vaccination rates using demographic and behavioral features.
2. Identify key factors that influence vaccine intake.
3. Build and optimize models (e.g., Random Forest) to enhance predictive performance.
4. Evaluate model performance using metrics such as accuracy, AUC, precision, recall, and F1-score.
5. Provide actionable insights for public health organizations to improve vaccination strategies.

## Data Science Goal
The analysis aims to develop a robust predictive model that accurately predicts vaccination behavior and identifies significant influencing factors, thus aiding in public health decision-making.

## Metrics of Success
The primary metric for success is the AUC (Area Under the Curve), which measures the model's ability to discriminate between vaccinated and non-vaccinated individuals. Supporting metrics include:
- **Accuracy**: Overall correctness of the model.
- **Precision**: Correct positive predictions relative to total positive predictions.
- **Recall**: Correct positive predictions relative to actual positive cases.
- **F1-score**: Harmonic mean of precision and recall.

## Data Understanding
The dataset consists of:
- **Total Records**: 26,707
- **Total Features**: 38, including both demographic (age, education, income) and behavioral (health practices, opinions on vaccines) variables.
- **Missing Values**: Initial analysis revealed several features with missing data, necessitating data cleaning and imputation.

## Data Preparation
Key steps in data preparation included:
1. **Data Cleaning**: Checking for duplicates and handling missing values through imputation (mean, median, mode).
2. **Feature Encoding**: Converting categorical variables into numerical formats suitable for modeling.
3. **Normalization/Scaling**: Ensuring features are on a similar scale to improve model performance.

## Exploratory Data Analysis
Several visualizations were created to analyze:
- Distribution of demographic features.
- Correlations between features and vaccination outcomes.
- Patterns of vaccine uptake across different demographics.

## Modeling
The following models were used:
- **Random Forest Classifier**: For its robustness and ability to handle non-linear relationships.
- **Logistic Regression**: As a baseline model.
- **XGBoost**: For its performance in classification tasks.

Hyperparameter tuning was performed using techniques such as Grid Search and Randomized Search to optimize model performance.

## Conclusion
This project provides valuable insights into vaccination behavior that can assist public health organizations in designing targeted interventions, improving vaccination campaigns, and ultimately increasing vaccine coverage to reduce the spread of infectious diseases.

## Future Work
- Explore additional modeling techniques and ensemble methods.
- Conduct deeper analysis on the impact of social media and public opinion on vaccine uptake.
- Expand the dataset with more recent vaccination data for longitudinal studies.

## Installation and Usage
To run the analysis:
1. Clone this repository.
2. Ensure you have Python and the required libraries installed (e.g., Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn).
3. Open the Jupyter Notebook `Predict H1N1 and Seasonal Flu Vaccines.ipynb`.
4. Run the notebook cells sequentially to execute the analysis.
