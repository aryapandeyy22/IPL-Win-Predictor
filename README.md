# American Express Campus Challenge 2024 - T20 Cricket Match Prediction

This repository contains my work for the **American Express Campus Challenge 2024**, where I built a machine learning system to predict the winning team in T20 cricket matches.

## Objective

I aimed to develop an accurate machine learning model that predicts the winning team in T20 cricket matches using historical match data, including detailed batsman and bowler statistics.

## Project Overview

- **Dataset**: I used historical T20 match data (domestic and international) from 2021 to 2023, including detailed scorecards for batsmen and bowlers.  
- **Task**: I implemented boosting algorithms (XGBoost, LightGBM) to predict match outcomes using a combination of match-level and player-level features.  
- **Evaluation**: I evaluated model performance based on accuracy by comparing predictions with actual match results.

## My Contributions / Work Done

- **Data Preparation**  
  - Cleaned and processed match-level, batsman-level, and bowler-level datasets.  
  - Handled missing values, encoded categorical features, and normalized numerical features.  

- **Feature Engineering**  
  - Created aggregated statistics like `team_winp_last5`, `ground_avg_runs_last15`, and player form metrics.  
  - Engineered combined features from batsman and bowler stats to capture match dynamics.  

- **Modeling**  
  - Trained XGBoost and LightGBM models and optimized hyperparameters for best performance.  
  - Built ensemble models to improve prediction accuracy.  

- **Validation & Evaluation**  
  - Implemented cross-validation and holdout validation to ensure model generalization.  
  - Analyzed feature importance to interpret model predictions.  

- **Submission Generation**  
  - Prepared submission files for both evaluation and training datasets with predicted match outcomes.  

## Dataset Summary

- **Training Data**: 948 rows × 23 columns (match-level info)  
- **Additional Data**:  
  - Match-level: 1,689 rows × 30 columns  
  - Batsman-level: 24,483 rows × 21 columns  
  - Bowler-level: 18,539 rows × 18 columns  

## Key Features

- **Match-level**: `match_id`, `team1_id`, `team2_id`, `winner_id`, `toss_winner`, `toss_decision`, `venue`, `city`, `match_dt`, ratios and win percentages like `team_count_50runs_last15`, `team_winp_last5`, and `ground_avg_runs_last15`.  
- **Batsman-level**: `runs`, `balls_faced`, `strike_rate`, `inning`, etc.  
- **Bowler-level**: `runs_conceded`, `wicket_count`, `economy`, `inning`, etc.  

## Approach

1. **Boosting Algorithms**: Focused on XGBoost, LightGBM, and ensemble models.  
2. **Feature Engineering**: Leveraged detailed player-level stats to generate meaningful features.  
3. **Validation**: Used cross-validation and holdout validation to avoid overfitting and ensure robustness.  

## Repository Contents

- **Data Preprocessing**: Scripts for cleaning and preparing datasets.  
- **Feature Engineering**: Scripts for generating custom features from batsman and bowler data.  
- **Model Training**: Code for training and tuning boosting models.  
- **Evaluation**: Scripts for validating model performance and generating submission files.  

## Competition Structure

- **Round 1**: Trained models on labeled data and evaluated on unseen test data.  
- **Round 2**: Applied the same methodology on a different dataset.  
- **Final Round**: Prepared a presentation summarizing my approach, feature importance, and model results.



