# StockTrendPrediction
Predicting stock price trends using historical price data and sentiment scores from scraped tweets


In this project we are using previously scraped tweets and pre-trained sentiment analysis models to extract sentiment scores for each working day.
Using historical price data and those sentiment scores we are training 3 different models to predict the stock price trend.

SentAn notebook contains the sentiment analysis part, trendExtraction notebook is used to add trend columns to the price data,
AggByDay aggregates the sentiment scores per each day and combines them with the prices into one dataframe, and the final notebook trains and tests 3 models.
The models are SVM, LSTM and EA-LSTM.
More about EA-LSTM: https://arxiv.org/pdf/1811.03760.pdf .
ea_lstm.py is used to simplify the ea-lstm training process.
