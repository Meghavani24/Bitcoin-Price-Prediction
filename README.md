# Bitcoin-Price-Prediction Using Machine Learning

This project aims to predict the closing price of Bitcoin using historical price data and engineered features through machine learning models, with a focus on tree-based algorithms like XGBoost. The project demonstrates how data-driven techniques can help capture market trends and enhance forecasting in volatile financial environments.

🧠 Project Objective
To build a reliable and interpretable machine learning model that forecasts Bitcoin's future closing prices based on past performance and engineered indicators such as lag features, rolling means, and trading volume changes.

📂 Dataset

Data Includes:

Daily closing prices of Bitcoin

Volume traded

Time-based market indicators (e.g., date, lag values)

🔧 Key Components

✅ Data Preprocessing
Parsing and formatting time series

Handling missing values

Sorting chronologically for time-aware modeling

🛠️ Feature Engineering
Lag Features: Close_Lag1, Close_Lag7

Rolling Statistics: 7-day & 30-day Rolling Mean

Returns & Volatility: Daily Return, Volume Change

📊 Model Building
Baseline Model: SARIMA (to model seasonality and trend)

ML Models:

XGBoost (Untuned & Tuned)

Linear Regression

Final model selected: ✅ Tuned XGBoost Regressor

📈 Model Evaluation
Train-Test Split (Chronological)

Cross-Validation: TimeSeriesSplit (5-fold)

Metric Used: RMSE (Root Mean Squared Error)

Best RMSE (Tuned XGBoost): 1347.47

📉 Results
The tuned XGBoost model significantly outperformed baseline models.

Visualization showed accurate tracking of Bitcoin price trends, although high-volatility spikes remain a challenge.

Cross-validation confirmed generalization capability and stability of the tuned model.


🔍 Tools & Technologies
Python

Pandas, NumPy, Matplotlib, Seaborn

XGBoost, Scikit-Learn

Statsmodels for SARIMA

Jupyter Notebook
