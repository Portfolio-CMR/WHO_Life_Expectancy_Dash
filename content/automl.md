+++
title = 'Automatic Machine Learning'
date = 2024-05-24T20:19:22-07:00
draft = false
weight = 2
+++

### **Using H2O AutoML Workflow**

1. **Prep work:** I load my data, figure out what I'm trying to predict (the target variable), and deal with any missing values.
2. **Set the stage:** I tell H2O what kind of problem I'm solving (like predicting numbers) and if there are any special rules I want to follow.
3. **Let H2O do its magic:** AutoML takes over, training lots of different models and figuring out the best settings for each.
4. **Pick the winner:** I look at how well each model did and choose the one that performed the best.
5. **Put it to work:** I export the chosen model and use it to make predictions on new data. 
