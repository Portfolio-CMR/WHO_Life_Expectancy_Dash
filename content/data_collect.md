+++
title = 'Data Collection and Cleaning'
date = 2024-05-24T20:18:57-07:00
draft = false
weight = 1
+++

1.  **Explore:** I check for columns with missing values and look for relationships that could help fill them in.
2.  **Correlate:** I calculate correlations between columns and focus on the strongest ones.
3.  **Predict:** For each missing value, I use a strongly correlated column as a predictor in a simple regression model.
4.  **Impute:** I use the model to predict the missing value and fill it in.
5.  **Validate:** I double-check the results to make sure they're reasonable. If not, I might try different models or predictors.

The key is to think of the strongly correlated column as a stand-in for the missing information. It's a simple but often effective way to clean up my data.
