# StockPricePrediction
The goal of this project is to use sentiment analysis to determine the average mood of Twitter users regarding the Nifty50 stock market, and then use a Long Short-Term Memory (LSTM) model to predict the final stock price based on the obtained sentiment score and historic stock data.

The project is divided into 2 parts:
1. Creating a sentiment analysis model on nifty50 tweets data using Naive Bayes Classifier. We used available stock tweet data on kaggle to to train our model, after which the model was used to classify the collected daily tweets containing keyword 'Nifty50' for the past 5 years. Using this dataset, we found average daily sentiment of the Nifty50 stock.

2. We combined our daily sentiment dataset with the daily historic OHLC of the Nifty50 stock data for the past 5 years. We used this dataset to train our LSTM model to predict stock prices for the next day.
