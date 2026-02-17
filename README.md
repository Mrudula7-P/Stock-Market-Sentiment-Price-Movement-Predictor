# Stock-Market-Sentiment-Price-Movement-Predictor
Stock Market Sentiment and Price Movement Predictor
Project Overview

This project aims to predict the next-day stock price movement (Up or Down) by combining historical market data with sentiment information. The model integrates technical indicators and sentiment scores to build a robust machine learning pipeline for financial prediction.

The objective is to demonstrate how structured financial data and sentiment signals can be leveraged together to forecast stock price direction using supervised learning techniques.

# Problem Statement

Stock prices are influenced by both historical trading patterns and external sentiment. Traditional technical analysis focuses on price and volume trends, while sentiment analysis captures market psychology.

This project builds a classification model that:

Processes historical stock market data

Incorporates sentiment scores

Engineers technical indicators

Predicts whether the stock price will increase or decrease the next trading day

# Dataset Description

The dataset includes the following features:

date – Trading date

open_value – Opening price

high_value – Highest price of the day

low_value – Lowest price of the day

last_value – Closing price

turnover – Trading volume

change_prev_close_percentage – Percentage change from previous close

Sentiment – Sentiment score associated with market information

# Feature Engineering

Additional features were created to enhance predictive performance:

SMA_5 – 5-day Simple Moving Average

SMA_10 – 10-day Simple Moving Average

Price_Change – Daily percentage price change

Target Variable – Binary classification label

1 → Price increases the next day

0 → Price decreases the next day

Data was sorted chronologically to preserve time-series structure, and missing values were handled appropriately.

# Machine Learning Model

The project uses a Random Forest Classifier for prediction.

Reasons for choosing Random Forest:

Captures non-linear relationships

Robust to noise and overfitting

Performs well on structured financial datasets

Provides feature importance analysis

# Model Evaluation

Model performance was evaluated using:

Accuracy Score

Confusion Matrix

Precision

Recall

F1-Score

Feature importance was analyzed to understand the contribution of each engineered variable.

# Project Workflow

Data loading and preprocessing

Chronological sorting of time-series data

Missing value handling

Feature engineering (technical indicators)

Target variable creation

Time-based train-test split

Model training using Random Forest

Prediction and performance evaluation

Feature importance visualization

# Technologies Used

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

# Key Insights

Technical indicators such as moving averages significantly influence predictive performance.

Sentiment features add contextual value when combined with structured market data.

Time-aware data splitting is critical in financial machine learning tasks.

# Future Enhancements

Incorporate additional technical indicators such as RSI and MACD

Implement gradient boosting models such as XGBoost

Explore deep learning approaches using LSTM for time-series prediction

Deploy the model using Streamlit or Flask

Integrate real-time news scraping for dynamic sentiment scoring

# Learning Outcomes

Financial time-series preprocessing

Feature engineering for market data

Integration of sentiment features in predictive modeling

Supervised classification for directional forecasting

Model interpretation through feature importance analysis
