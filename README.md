# LSTM_Stock Price Prediction and Bitcoin

I have just read a paper on SIGKDD 2017 about stock price prediction, named Stock Price Prediction via Discovering Multi-Frequency Trading Patterns. And implemented a LSTM version on the 50 stock dataset they provided.

Please read my

[Report PDF](https://github.com/RenXiangyuan/LSTM_SFM/blob/master/stock-prediction-lstm%20(1).pdf) 

for detail information about the stock prediction on LSTM and SFM.

* Language: Python 2.7
* Framework: Keras
* Backend: Theano 

SFM is a model that can make predictions on different strategies, short term or long term. It make prediction on users' choice. For example, those looking at a long period investment may use long term strategy.

However, it is accurate enough in term of Mean Square Error but It Doesn't work!

The model will always yield a prediction after the changes have happened, e.g. the stock A turns from rise to fell in Monday, but the model can only realize this change after the change has happened. This make me thinking about whether time series have been used for prediction.
