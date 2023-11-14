# Stock Price Prediction Project

Welcome to the Stock Price Prediction project! This project aims to predict the future stock prices of Nifty50 using sentiment analysis of Twitter data and a Long Short-Term Memory (LSTM) model. This README file provides an overview of the project and instructions on how to use it.

## Table of Contents

- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [Data Collection](#data-collection)
- [Sentiment Analysis](#sentiment-analysis)
- [Stock Price Prediction](#stock-price-prediction)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The primary goal of this project is to predict the future stock prices of Nifty50, an Indian stock market index, by analyzing sentiment data from Twitter users. The project is divided into two main parts:

1. **Sentiment Analysis**: In this part, we build a sentiment analysis model using a Naive Bayes Classifier. We train the model using available stock tweet data from Kaggle and classify daily tweets containing the keyword 'Nifty50' for the past 5 years. This process helps us determine the average daily sentiment of the Nifty50 stock.

2. **Stock Price Prediction**: We combine the daily sentiment dataset with the daily historic OHLC (Open, High, Low, Close) data of the Nifty50 stock for the past 5 years. This combined dataset is used to train an LSTM model to predict stock prices for the next day based on both historic stock data and sentiment scores.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/MaitreeVaria/StockPricePrediction.git
   ```

2. Install the required dependencies by running:

   ```bash
   pip install -r requirements.txt
   ```

3. Follow the instructions in the [Data Collection](#data-collection) section to obtain the necessary data.

4. Follow the instructions in the [Sentiment Analysis](#sentiment-analysis) section to perform sentiment analysis on the Twitter data.

5. Follow the instructions in the [Stock Price Prediction](#stock-price-prediction) section to train and use the LSTM model for stock price prediction.

## Data Collection

To replicate this project, you'll need the following datasets:

- Stock tweet data from Kaggle or a similar source for training the sentiment analysis model.

- Daily historic OHLC data for Nifty50 for the past 5 years. You can obtain this data from financial data providers or stock market APIs.

- Daily tweets containing the keyword 'Nifty50' for the past 5 years, which you can collect using Twitter API or other data collection methods.

## Sentiment Analysis

The sentiment analysis part of the project involves the following steps:

1. Collect daily tweets containing the keyword 'Nifty50' for the past 5 years.
2. Preprocess the the tweets - Remove stop words, perform lemmitization and tokenize the tweets
3. Train the sentiment analysis model using the preprocessed stock tweet data.
4. Use the trained model to classify the sentiment of these daily tweets and calculate the average daily sentiment score for Nifty50.

Detailed instructions for each step can be found in the project's documentation.

## Stock Price Prediction

The stock price prediction part of the project involves the following steps:

1. Combine the daily sentiment dataset with the daily historic OHLC data of Nifty50 for the past 5 years.
2. Preprocess and split the dataset into training and testing sets.
3. Train an LSTM model using the combined dataset to predict stock prices for the next day.
4. Evaluate the model's performance and make predictions.

Detailed instructions for each step can be found in the project's documentation.

## Usage

You can use this project as a starting point for your own stock price prediction experiments. Feel free to customize the sentiment analysis model or the LSTM model, collect different datasets, and adapt the code to your specific needs.

To run the project, follow the steps outlined in the [Getting Started](#getting-started) section. You can also refer to the project's documentation for more details on how to use and customize the code.

## Contributing

Contributions to this project are welcome! If you have any improvements, bug fixes, or new features to propose, please open an issue or submit a pull request. Make sure to follow the project's coding standards and guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Feel free to use, modify, and distribute the code as per the terms of the license.

Happy stock price prediction!

**Disclaimer**: This project is for educational and research purposes only. Stock market prediction is a complex task, and the accuracy of the models developed in this project may not be suitable for real-world trading decisions. Use the predictions at your own risk, and always consult with financial professionals before making any investment decisions.
