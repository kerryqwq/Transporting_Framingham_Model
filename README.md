# Transporting Framingham Risk Prediction Model to New Target Populations

## Abstract

Objective: The source data often cannot treated as a random sample from the target population due to differences in covariate distributions between the two populations. Transportation analysis techniques can overcome this challenge. In this project, our goals are 1) to evaluate the Cardiovascular Disease Risk Prediction model's performance on individual-level NHANES data, originally developed from the Framingham Heart Study, and 2) to assess the model's performance on simulated NHANES data when actual data are unavailable. We will consider three simulation scenarios: observed Framingham correlation, no correlation, and high correlation (0.6).
   
   Methods: We employ a logistic regression model, developed from the Framingham dataset, which is trained using the training set. This model is used to predict the risk of cardiovascular disease, with each version of the model stratified by sex. Additionally, we utilize logistic regression to estimate the inverse-odds weighting estimator by calculating $\text{Pr}[S=1 \mid X, D_{\text{test},i}=1]$, and assessed the performance of each sex-stratified risk score prediction model using modified Brier Score when the target population is different from the source population.

  Results: The Brier scores for the women's risk score prediction model were consistently lower than those for the men's model. Notably, the Brier score for the men's model using simulated NHANES data was higher than that using actual NHANES data. The women's model performs well with no and observed correlation in the simulated data, showing slightly lower Brier scores than the actual NHANES data. 


