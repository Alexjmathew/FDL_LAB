# NIFTY 50 Stock Price Prediction

## Project Overview
This project implements a machine learning model to predict NIFTY 50 stock prices using Linear Regression. The model uses historical stock data with engineered features to forecast future prices.

## Author
**Alex J Mathew**

## Algorithm Steps

### 1. Data Collection
- Download historical NIFTY 50 data from Yahoo Finance
- Time period: January 1, 2010 to January 1, 2022
- Primary data: Daily closing prices

### 2. Data Preparation
- Extract closing price data
- Reset index to make dates a column
- Prepare data for feature engineering

### 3. Feature Engineering
- **Days**: Number of days since start date
- **Year**: Extract year from date
- **Month**: Extract month from date
- **DayOfYear**: Day number in the year
- **Prev_Close**: Previous day's closing price
- **Rolling_Mean_7**: 7-day moving average
- **Rolling_Mean_30**: 30-day moving average

### 4. Data Cleaning
- Remove rows with missing values
- Handle NaN values from lag features and rolling averages

### 5. Train-Test Split
- Split data chronologically (time-series split)
- Training set: First 80% of data
- Testing set: Last 20% of data
- No shuffling to preserve time order

### 6. Feature Selection
- Select all engineered features as model inputs
- Target variable: Closing price

### 7. Model Training
- Use Linear Regression algorithm
- Train model on training dataset
- Learn relationships between features and stock prices

### 8. Prediction
- Make predictions on test dataset
- Generate forecasted stock prices

### 9. Model Evaluation
- **MSE**: Mean Squared Error
- **RMSE**: Root Mean Squared Error
- **MAE**: Mean Absolute Error
- **R²**: R-squared Score
- **MAPE**: Mean Absolute Percentage Error

### 10. Results Analysis
- Feature importance ranking
- Model coefficients interpretation
- Visualization of actual vs predicted prices
- Residual analysis

## Key Features
- Time-series appropriate train-test split
- Multiple technical indicators as features
- Comprehensive model evaluation metrics
- Visualizations for result interpretation

## Requirements
- pandas
- numpy
- yfinance
- matplotlib
- scikit-learn

## Usage
Run the Python script to:
1. Download and preprocess data
2. Train the prediction model
3. Evaluate model performance
4. Generate prediction visualizations

## Note
Stock market prediction is inherently uncertain and this model should be used for educational purposes only.
