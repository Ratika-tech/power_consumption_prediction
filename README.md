# power_consumption_prediction
# Power Consumption Prediction

## Overview
A machine learning project that forecasts electricity consumption for three power zones 10 minutes ahead using weather data, calendar features, and historical power consumption.

## Problem Statement
Accurately forecasting short-term electricity demand can help with energy planning and resource management.

## Dataset
The dataset contains timestamped weather observations and electricity consumption for three zones in 2017.

Source: [Electric Power Consumption Dataset — Kaggle](https://www.kaggle.com/datasets/fedesoriano/electric-power-consumption)

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost (when available)
- Jupyter Notebook

## Project Workflow
1. Data cleaning and validation
2. Exploratory data analysis
3. Time-series feature engineering
4. Chronological train, validation, and test split
5. Comparison of multiple regression models
6. Evaluation using MAE, RMSE, and R²
7. Comparison against a persistence baseline
8. Saving the selected model and test predictions

## Model Evaluation
The notebook selects the model using validation data and reports final performance on a held-out test set. See the notebook for the actual per-zone metrics.

## How to Run
1. Clone or download this repository.
2. Install the dependencies listed in `requirements.txt`.
3. Keep the CSV dataset in the same directory as the notebook.
4. Open the notebook in Jupyter or VS Code.
5. Run all cells from top to bottom.

**Note:** The model performs sequential 10-minute-ahead forecasting and assumes current weather and consumption observations are available at prediction time.
