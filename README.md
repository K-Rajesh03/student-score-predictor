# Student Exam Score Predictor

Predicts a student's exam score based on hours studied, using SQL for data analysis and Linear Regression for prediction.

## Overview
This project demonstrates an end-to-end data workflow: loading data into a SQL database, running analytical queries, and training a regression model to predict outcomes.

## Tech Stack
- Python (pandas, scikit-learn, matplotlib)
- SQLite (SQL queries for exploratory analysis)
- Google Colab

## What I Did
- Loaded student study data into a SQLite database
- Wrote SQL queries to group students by study level (Low/Medium/High) and compare average scores
- Trained and compared two models: Linear Regression and Decision Tree Regressor
- Visualized the relationship between study hours and scores

## Results
| Model | R² Score | MAE |
|---|---|---|
| Linear Regression | 0.968 | 3.92 |
| Decision Tree | 0.946 | 5.40 |

Linear Regression performed better, consistent with the near-linear relationship between study hours and scores.

## Key Insight
Students studying 6+ hours averaged significantly higher scores than those studying under 3 hours (see SQL grouping query in notebook).

## Files
- `Untitled0.ipynb` — full code and analysis
- `student_data.csv` — dataset used
