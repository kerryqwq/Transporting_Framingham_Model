# Transporting Framingham Risk Prediction Model to New Target Populations

## Overview
This project investigates the performance of the Framingham cardiovascular disease (CVD) risk score model when applied to new target populations, specifically NHANES and simulated NHANES data. The Framingham risk score model is a logistic regression model developed using the Framingham Heart Study data. It predicts 10-year CVD risk based on risk factors like age, BMI, blood pressure, smoking status, etc. The goal is to evaluate the model's performance in the Framingham source population, the actual NHANES target population, and a simulated NHANES target population. Performance is measured using the Brier score.

## Contents
The project report contains the following sections:

Abstract

Introduction - background and goals

Methodology - data sources, prediction model details, performance metrics

Analysis - 3 analyses done to evaluate performance in different scenarios

Results - key results presented in tables and plots

Discussion - interpretation of results, limitations

## Running the Code

The R Markdown document contains code to:

Prepare and explore the Framingham and NHANES datasets
Define and fit CVD prediction models.

Evaluate model performance using training/test splits
Simulate NHANES data based on summary statistics.

Calculate modified Brier scores for model evaluation

## Clone this repo
Open the R Markdown document
Install any missing libraries
Run all code chunks
Output will include data visualizations, summary tables, and Brier score metrics.

## Key Findings
The prediction model showed better performance (lower Brier score) when applied to new target populations compared to the source population.

Performance was similar for both actual and simulated NHANES target data.

The model performed better for women compared to men across all scenarios.

## References
References are included for the modified Brier score method and related prediction model transportation techniques.
