# Transporting Framingham Risk Prediction Model to New Target Populations

## Abstract

Objective: The source data often not a random sample from the target population due to differences in covariate distributions between the two populations. Transportation analysis techniques can overcome this challenge. In this project, our goals are 1) to evaluate the Cardiovascular Disease Risk Prediction model's performance on individual-level NHANES data, originally developed from the Framingham Heart Study, and 2) to assess the model's performance on simulated NHANES data when actual data are unavailable. We will consider three simulation scenarios: observed Framingham correlation, no correlation, and high correlation (0.6).
   
   Methods: We employ a logistic regression model, developed from the Framingham dataset, which is trained using the training set. This model is used to predict the risk of cardiovascular disease, with each version of the model stratified by sex. Additionally, we utilize logistic regression to estimate the inverse-odds weighting estimator by calculating $\text{Pr}[S=1 \mid X, D_{\text{test},i}=1]$, and assessed the performance of each sex-stratified risk score prediction model using modified Brier Score when the target population is different from the source population.

  Results: The Brier scores for the women's risk score prediction model were consistently lower than those for the men's model. Notably, the Brier score for the men's model using simulated NHANES data was higher than that using actual NHANES data. The women's model performs well with no and observed correlation in the simulated data, showing slightly lower Brier scores than the actual NHANES data. The high correlation scenario for the women's model leads to a significantly higher predictive error.


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


## References
References are included for the modified Brier score method, related prediction model transportation techniques, and data source.
