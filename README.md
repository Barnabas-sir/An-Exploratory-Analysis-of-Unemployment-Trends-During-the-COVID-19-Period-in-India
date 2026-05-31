# An Exploratory Analysis of Unemployment Trends During the COVID-19 Period in India

## Project Overview

This project investigates the impact of COVID-19 on unemployment across Indian states using data analysis, statistical testing, machine learning, and explainable AI techniques.

The study examines unemployment patterns before and during the COVID-19 period, identifies the most affected regions, evaluates urban-rural disparities, and develops an XGBoost model to understand the key drivers of unemployment.

## Objectives

* Analyse unemployment trends across India.
* Compare unemployment rates before and during COVID-19.
* Identify the most affected states and regions.
* Compare unemployment patterns between urban and rural areas.
* Perform statistical testing to validate COVID-19 impacts.
* Build a predictive machine learning model.
* Explain model predictions using SHAP.

## Dataset

The dataset contains monthly unemployment statistics for Indian states between May 2019 and June 2020.

Key variables include:

* Region
* Date
* Area (Urban/Rural)
* Estimated Unemployment Rate (%)
* Estimated Employed
* Estimated Labour Participation Rate (%)
* Geographic Zone
* Latitude and Longitude

## Methodology

### Data Preparation

* Standardised column names
* Removed empty records
* Removed duplicate observations
* Merged unemployment and geographic datasets
* Added zone-level geographic information

### Exploratory Data Analysis

* National unemployment trends
* Regional unemployment comparisons
* Urban vs Rural unemployment analysis
* Zone-level unemployment trends
* Top affected regions during COVID-19

### Statistical Analysis

Welch's Two-Sample T-Test was performed to compare unemployment rates before and during COVID-19.

Results:

* T-statistic: -7.85
* P-value: 4.59e-13

This confirms a statistically significant increase in unemployment during the pandemic.

### Machine Learning

Model: XGBoost Regressor

Target Variable:

* Estimated Unemployment Rate (%)

Features:

* Estimated Employed
* Labour Participation Rate
* Region
* Zone
* Area
* Month
* COVID Period

### Model Performance

| Metric | Value |
| ------ | ----- |
| MAE    | 3.85  |
| RMSE   | 6.42  |
| R²     | 0.72  |

## Explainable AI

SHAP (SHapley Additive exPlanations) was used to identify the most influential factors affecting unemployment.

Top drivers included:

* Estimated Employed
* COVID Period
* Geographic Zone
* Labour Participation Rate
* Region

## Key Findings

* COVID-19 increased unemployment by approximately 110%.
* Urban areas consistently experienced higher unemployment than rural areas.
* Eastern and Northern regions recorded the largest unemployment spikes.
* Tripura, Haryana, Jharkhand, and Bihar were among the most affected states.
* Employment levels and COVID-related disruptions were the strongest predictors of unemployment.

## Dashboard

A Streamlit dashboard was developed to present:

* National unemployment trends
* Urban vs Rural comparisons
* Regional rankings
* Zone-level analysis
* XGBoost model performance
* SHAP explainability results

## Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-Learn
* XGBoost
* SHAP
* Streamlit

## Project Outcome

This project demonstrates how data science, statistical analysis, machine learning, and explainable AI can be applied to understand the socioeconomic impact of major glo<img width="801" height="940" alt="shap_summary" src="https://github.com/user-attachments/assets/324cabc1-431d-4149-9d23-63c41adbb4c1" />
<img width="1022" height="568" alt="shap_bar" src="https://github.com/user-attachments/assets/c6056544-1ca2-4195-8e07-cc423c0ecc9e" />
bal events such as COVID-19.
