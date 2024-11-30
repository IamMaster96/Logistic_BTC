Logistic_BTC is a Python-based project aimed at analyzing Bitcoin price trends using machine learning, particularly logistic regression. The project includes data preparation, feature engineering, and modeling to predict potential price movements of Bitcoin.

Features

Data Collection: Uses market data for Bitcoin, including historical prices and volume.
Feature Engineering: Implements technical indicators like RSI, MACD, Bollinger Bands, and Momentum to enhance prediction capabilities.
Machine Learning: Employs logistic regression to predict market directions (uptrend or downtrend).
Visualization: Generates performance metrics and visualizations for the logistic regression model.
Prerequisites

Before using this project, ensure you have the following installed:

Python 3.8+
Key libraries: numpy, pandas, matplotlib, scikit-learn, and ccxt
Install dependencies via:

pip install -r requirements.txt
Installation

Clone the repository:
git clone https://github.com/IamMaster96/Logistic_BTC.git
cd Logistic_BTC
Set up your environment:
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Project Structure

data/: Contains CSV files with historical Bitcoin data.
scripts/: Python scripts for data collection, preprocessing, feature engineering, and modeling.
notebooks/: Jupyter notebooks for exploratory data analysis and model evaluation.
README.md: Documentation for the project.
Usage

Step 1: Data Preparation
Use scripts/data_collector.py to fetch or preprocess Bitcoin historical data. The data should include columns like timestamp, open, high, low, close, volume, and exchange.

Step 2: Feature Engineering
Run the feature engineering script to calculate technical indicators:

python scripts/feature_engineer.py
Step 3: Train the Model
Train the logistic regression model on the engineered dataset:

python scripts/model_train.py
Step 4: Evaluate Results
Analyze model predictions and performance metrics through visualizations in the notebooks provided.

Key Functions and Modules

Feature Engineering:
Implements RSI, MACD, Bollinger Bands, and Momentum.
Handles missing values effectively.
Logistic Regression:
Predicts binary outcomes: upward or downward price trends.
Includes model evaluation metrics such as accuracy, precision, recall, and ROC curves.
Data Collection:
Supports multiple exchanges using ccxt for robust historical data collection.
Example Usage

from scripts.feature_engineer import FeatureEngineer
from scripts.model_train import train_logistic_model

# Load data
data = pd.read_csv('data/btc_data.csv')

# Feature engineering
engineer = FeatureEngineer(data)
processed_data = engineer.generate_technical_indicators()

# Model training
train_logistic_model(processed_data)
Contribution

Contributions are welcome! Feel free to fork the project, create pull requests, or open issues for suggestions and bug reports.

License

This project is open-source and licensed under the MIT License.
