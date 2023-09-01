<h1>Stock Market Prediction using Numerical and Textual Analysis</h1>


<h2>Objective:</h2>

To create a hybrid model for stock price/performance prediction using numerical analysis of historical stock prices, and sentimental analysis of news headlines(of that particular day).

<h2>Approach: </h2>

- Extract Sentiment Scores from given newspaper headlines data, with the help of nltk's SentimentIntensityAnalyzer.
- For this problem statement, I took inspiration from this [paper](https://www.researchgate.net/publication/306925671_Deep_learning_for_stock_prediction_using_numerical_and_textual_information) and decided to carry out Multivariate Time Series Forecasting using Keras' LSTM.
- I used randomforestregressor, adaboostregressor, xgboost, etc. to model the temporal effects of past events(both Textual, i.e the sentiment scores and Historical stock data) on opening prices.
- Highest accuracy was obtained with randomforestregressor.
- RMSE was lowest with lightbgm

<h2>Data used to analyze and predict:</h2>

- Historical stock prices(SENSEX (S&P BSE SENSEX)) from https://finance.yahoo.com/
- Textual (News) data from https://bit.ly/36fFPI6
