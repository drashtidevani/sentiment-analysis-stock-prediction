# sentiment-analysis-stock-prediction
A comprehensive study on leveraging AI and sentiment analysis to enhance stock market prediction models

Overview
This research explores how adding sentiment analysis to stock market prediction models can improve their accuracy. We focused on seven key European stock indices:

🇩🇪 DE40 (Germany)
🇫🇷 FR40 (France)
🇳🇱 NL25 (Netherlands)
🇮🇹 IT40 (Italy)
🇪🇸 SP35 (Spain)
🇬🇧 UK100 (United Kingdom)
🇪🇺 EU50 (Europe)
🔬 Key Findings
By incorporating sentiment scores from financial news with traditional market data:

✅ The SimpleNN model recognized additional trends
✅ Enhanced prediction accuracy for certain indices
✅ Evaluated using MSE, MAE, and SMAPE metrics
⚠️ Sentiment data can also add noise to certain indices, showing non-uniform impact

📁 Repository Structure

📓 Jupyter Notebooks
File	Purpose
ADF_test.ipynb	Augmented Dickey-Fuller test for time series stationarity (required for ARIMA)
ARIMA.ipynb	ARIMA model implementation for stock market trend forecasting
stocks_data.ipynb	Data preprocessing, visualization, and exploration of stock market data

🐍 Python Scripts
File	Description
Data Collection Script - REUTERS.py	Web scraping of financial news articles from Reuters for sentiment analysis
NN with Sentiment.py	SimpleNN model with sentiment indicators for stock prediction
NN without Indicator.py	SimpleNN model using only historical stock data (baseline)
NN without Sentiment.py	Alternative SimpleNN model excluding sentiment data
Relevance Score Script.py	Computes relevance scores for news articles vs. market events
Sentiment Score Script.py	Calculates sentiment scores from financial news data

📊 Data
Source: Major European stock indices (DE40, FR40, NL25, IT40, SP35, UK100, EU50)
Processing: Loaded, preprocessed, and visualized in stocks_data.ipynb
News Data: Reuters financial news articles for sentiment analysis

🚀 Getting Started
📋 Prerequisites
Python: 3.8 or higher
Jupyter Notebook: For running .ipynb files
Required Libraries:
pandas - Data manipulation
numpy - Numerical computing
matplotlib - Data visualization
scikit-learn - Machine learning utilities
statsmodels - ARIMA modeling
tensorflow or pytorch - Neural network models
nltk or textblob - Sentiment analysis
