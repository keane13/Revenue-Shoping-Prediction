# 📈 Revenue Prediction using Machine Learning

## Overview
E-Commerce Dataset Feature Description
The features in this dataset record visitor activity and are divided into four main categories:

Page Activity & Duration
Counts the number of pages visited and the total time spent across three page types: Administrative, Informational, and Product Related. This data is tracked based on URLs and updated in real-time.

Google Analytics Metrics

Bounce Rate: The percentage of visitors who enter the site and leave immediately without any further interaction.

Exit Rate: The percentage of times a specific page was the last one viewed in a session.

Page Value: The average value of a page that a user visited before successfully completing a transaction.

Special Day Context
An indicator (ranging from 0 to 1) that measures how close the visit time is to a special day or holiday (like Valentine's Day or Mother's Day) that could trigger a purchase. The value is dynamic as it accounts for the reasonable time gap between ordering and delivery.

System & Visitor Profile
A collection of technical and demographic attributes that include: Operating System (OS), Browser, Region, Traffic Type, Visitor Type (New or Returning), Weekend Status, and the Month of the visit.

## Business Problem
Accurate revenue forecasting is essential for:
- Financial planning
- Resource allocation
- Risk management

Traditional methods often fail to capture nonlinear patterns. This project
uses machine learning models to improve prediction accuracy.

## Approach
- Problem Type: Supervised Regression
- Models:
  - XGBoost
  - Random Forest Regressor
- Evaluation Metrics:
  - R² Score
  - MAE
  - RMSE

## Workflow
1. Data preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature engineering
4. Model training
5. Model evaluation

## Results
The XGBoost model achieved better performance than linear regression,
indicating nonlinear relationships in the data.

| Metric | Value |
|------|------|
| R² | 0.82 |
| MAE | 1.25 |
| RMSE | 1.89 |

## Project Structure
```text
revenue-prediction/
├── notebooks/
│   └── Revenue_Prediction.ipynb
├── data/
├── models/
├── requirements.txt
└── README.md
