+++
title = 'Automatic Machine Learning'
date = 2024-05-24T20:19:22-07:00
draft = false
weight = 2
+++

### **Using H2O AutoML Workflow**

1. **Prep work:** I load my data, point out the target column "Life expectancy", and impute missing values.
2. **Let H2O do its magic:** AutoML takes over, and benchmarks hundreds of different models using cross-validation. Here are the top performers:

| model_id                                             | rmse   | mse    | mae    | rmsle  | mean_residual_deviance |
| ---------------------------------------------------- | ------ | ------ | ------ | ------ | ---------------------- |
| StackedEnsemble_AllModels_5_AutoML_8_20240523_123256 | 1.5141 | 2.2926 | 0.7862 | 0.0235 | 2.2926                 |
| StackedEnsemble_AllModels_4_AutoML_8_20240523_123256 | 1.5210 | 2.3134 | 0.8363 | 0.0236 | 2.3134                 |
| StackedEnsemble_AllModels_3_AutoML_8_20240523_123256 | 1.5612 | 2.4374 | 0.8530 | 0.0241 | 2.4374                 |
| GBM_grid_1_AutoML_8_20240523_123256_model_11         | 1.5655 | 2.4509 | 0.8601 | 0.0242 | 2.4509                 |

3. **Explainability:** Models can be used more effectively if you know why they perform well. Here are some explainability charts for top performing models.

4. **Put it to work:** I export the chosen model and use it to make predictions on new data. 
