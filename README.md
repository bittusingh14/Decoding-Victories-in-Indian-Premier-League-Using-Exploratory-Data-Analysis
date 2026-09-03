# Decoding Victories in Indian Premier League — Using Exploratory Data Analysis 

An IPL match analysis and machine learning project that uses Exploratory Data Analysis (EDA) and supervised machine learning to analyze Indian Premier League match outcomes from 2008 to 2024.

## Project Overview

This project analyzes IPL match data to identify patterns and trends related to team performance, toss decisions, win margins, seasonal performance, and match outcomes.

The analysis is based on approximately 1,100 IPL match records covering 17 seasons from 2008 to 2024.

## Objectives

- Perform Exploratory Data Analysis on IPL match data
- Analyze team performance and winning trends
- Study the relationship between toss decisions and match outcomes
- Analyze the distribution of win margins
- Identify correlations between important features
- Predict match winners using Random Forest
- Predict win margins using Linear Regression

## Dataset

The dataset contains IPL match records from 2008 to 2024.

### Key Features

- Team1
- Team2
- Toss_Winner
- Toss_Decision
- City
- Season
- Winner
- Win_Margin
- Target_Score

### Data Preprocessing

- Handled missing values
- Standardized historical franchise names
- Resolved inconsistent text values
- Applied Label Encoding to categorical features
- Applied StandardScaler for feature scaling
- Created derived features such as `Team1_Win` and `Toss_Win_Match_Win`

## Exploratory Data Analysis

The project includes 12 visualizations to analyze IPL match patterns:

1. Top 10 winning teams
2. Toss decision distribution
3. Win margin distribution
4. Win margin by toss decision
5. Average win margin over seasons
6. Target score vs. win margin
7. Correlation heatmap
8. Toss decision vs. match winner
9. Win margin density by toss decision
10. Win margin violin plot
11. Team1 vs. Winner distribution
12. Win margin distribution with mean line

## Machine Learning Models

### Random Forest Classifier

Used to predict the match winner.

- Train-Test Split: 80/20
- Random State: 42
- Number of Estimators: 100
- Accuracy: 42.53%

### Linear Regression

Used to predict the win margin.

- Train-Test Split: 80/20
- Random State: 42
- R² Score: -0.029
- Mean Absolute Error: 26.09
- Mean Squared Error: 879.21

## Key Findings

- Toss decisions showed negligible influence on win margins.
- Toss decisions were almost evenly distributed between batting and fielding first.
- Most matches were decided by relatively narrow win margins.
- Win margins showed a strongly right-skewed distribution.
- Team identity showed stronger relationships with winning tendency than toss decision.
- The 2023 season recorded the highest average win margin in the analyzed dataset.
- The Random Forest model achieved 42.53% accuracy in predicting match winners.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

```text
IPL Match Dataset
       ↓
Data Preprocessing
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Data Visualization
       ↓
Feature Encoding & Scaling
       ↓
Machine Learning
       ↓
Random Forest + Linear Regression
       ↓
Model Evaluation
       ↓
Insights & Findings
```

## Results

| Model | Task | Performance |
|---|---|---|
| Random Forest Classifier | Match Winner Prediction | 42.53% Accuracy |
| Linear Regression | Win Margin Prediction | 26.09 MAE |
| Linear Regression | Win Margin Prediction | -0.029 R² |

## Future Improvements

- Include ball-by-ball match data
- Add player availability and performance features
- Include weather conditions
- Include pitch information
- Explore advanced ensemble models such as XGBoost
- Experiment with deep learning models
- Improve feature engineering for match outcome prediction

## Author

**Bittu Kumar Singh**

GitHub: https://github.com/bittusingh14
