# Stock Closing Price Prediction

The stock prediction model is a project that revolves around predicting the adjusted closing price of stocks using deep learning neural networks that have been fitted with LSTM cells. The model takes the last 75
days of closing data and uses it to predict the current closing price. The predictions are then visually displayed using matplotlib to guage the viability of the model.

## How it Works

### Model production (stock_pred_dev.ipynb)

The core functionality of predicting the closing price is located inside `stock_pred_dev.ipynb`. The file uses stock closing data found at https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs, to train a deep learning model using LSTMS to predict closing price. This file also contains stock data analysis to see the relationship between stock closing prices, volume, price variance etc. 

### Model (seq-2LSTM-DenseLinOutput)

`seq-2LSTM-DenseLinOutput` contains the model that is used for predicting the closing prices. 

## Model Usage requirements

In order to use the deep learning model accurately, the input shape must be (75, 1) with the array being made up of the previous 75 days of adjusted closing price. The y or the dependant variable should be the current closing price. 
