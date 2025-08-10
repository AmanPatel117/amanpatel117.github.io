---
layout: single
title: "Injury Prediction for Runners"
weight: 4
permalink: /projects/running/
---
[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AmanPatel117/Injury-In-Runners-Data-Science-Project)
[![View on Kaggle](https://img.shields.io/badge/View_on_Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/code/yehonam/running-injury-prediction)

# Goal
The goal of this project is to develop a predictive model that identifies the likelihood of a runner sustaining an injury based on their training data, physiological attributes, and historical injury patterns. By proactively identifying at-risk athletes, training plans can be adjusted to reduce injury risk. This was my first data science project which I created with a friend, and we were able to get a bronze medal on Kaggle for our efforts

# Methodology
## Data Collection
The dataset comes from a publicly available running injury study, containing demographic information, training logs, prior injury history, and physiological measurements.  
Each record corresponds to a runner over a given training period, with the target variable indicating whether the runner sustained an injury.

## Feature Engineering
The preprocessing pipeline included:
- Encoding categorical variables such as gender and injury history
- Creating aggregated features from training logs (weekly mileage, training frequency, intensity distribution)
- Scaling numerical features for model stability

## Modeling
Multiple classification algorithms were evaluated using both oversampling and undersampling to handle class imbalance, including Logistic Regression, Random Forest, and XGBoost.  
The best-performing model was **XGBoost**, achieving a 60% overall accuracy rate, with 60% for injured prediction and 60% for non-injured prediction. While these metrics are not great, the work is a step in the right direction. Further work can be done to better understand and utilize the timeseries nature of the data to make predictions, rather than naively classify.
