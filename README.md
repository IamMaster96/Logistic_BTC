Logistic_BTC is a Python-based project aimed at analyzing Bitcoin price trends using machine learning, particularly logistic regression. The project includes data preparation, feature engineering, and modeling to predict potential price movements of Bitcoin.

Features

Data Collection: Uses market data for Bitcoin, including historical prices and volume.
Feature Engineering: Implements technical indicators like RSI, MACD, Bollinger Bands, and Momentum to enhance prediction capabilities.
Machine Learning: Employs logistic regression to predict market directions (uptrend or downtrend) (Under construction).
Visualization: Generates performance metrics and visualizations for the logistic regression model (Under construction).
Prerequisites

Before using this project, ensure you have the following installed:

Python 3.8+
Key libraries: numpy, pandas, matplotlib, scikit-learn, and ccxt

Step 1: Data Preparation
Use data_collector.py to fetch or preprocess Bitcoin historical data. The data should include columns like timestamp, open, high, low, close, volume, and exchange.

Step 2: Feature Engineering
Run the feature engineering script to calculate technical indicators:
python script feature_engineer.py

Step 3: Train the Model (Under construction)
Train the logistic regression model on the engineered dataset:

Step 4: Evaluate Results (Under construction)
Analyze model predictions and performance metrics through visualizations in the notebooks provided.
