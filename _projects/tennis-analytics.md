---
layout: single
title: "Tennis Analytics"
weight: 5
permalink: /projects/tennis-analytics/
---

# Goal
The goal of this project is to create a model that can predict the winner of a tennis match given various data about the two players competing, such as their respective rankings, head to head and win ratio on the given surface.

# Methodology
## Data Collection
The data was collected by programatically scraping the ATP website for tournaments, players, rankings, and match results. The initial data is stored in 4 pandas dataframes one for each of tournaments, players, rankings, and match results.

## Feature Engineering
To prepare a tabular dataset for modeling, I started off with the match results. Using merges and lookups, I was able to add features such as the ranking of each player, their head to head, precentage one of last 10 matches, and win percentage on the surface. Since the match dataset had the Winner as the player in the Player 1 column, I shuffled the data to avoid overfitting to that pattern.

## Modeling
After testing several types of models, it was determined that XGBoost had the best performance, with an accuracy of about 70%.

## Sports Betting Simulation
I pulled some old sports betting odds from Kaggle, and made sure that these matches were not in the training data. I simulated placing bets of equal increment based on the model output and was able to achieve a profit margin of 5%.

# Future Work
Currently, I am in the process of organizing my code and seeing if I can create a CI/CD pipeline where new match data is scraped periodically, and a new model is trained and deployed.
