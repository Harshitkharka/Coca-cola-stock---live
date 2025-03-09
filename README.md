
# Stock Price Prediction of Coca-Cola Using LSTM and Yahoo Finance Data

## Description
This project aims to predict the future closing price of Coca-Cola (KO) stock using a Long Short-Term Memory (LSTM) neural network. The dataset is sourced from Yahoo Finance, and the model is trained on historical stock price data from 2012 to 2019. The project follows a systematic approach that includes data collection, preprocessing, feature engineering, model training, evaluation, and forecasting. By leveraging LSTM—a type of recurrent neural network (RNN) designed for time series forecasting—this project seeks to improve prediction accuracy compared to traditional methods like ARIMA.

## Features
- **Historical Data Collection:** Downloads historical stock data for KO from Yahoo Finance.
- **Data Preprocessing:** Scales the data using MinMaxScaler and prepares sequences for the LSTM.
- **Model Training:** Trains an LSTM model to predict the next day's closing price.
- **Evaluation:** Compares predicted prices with actual prices on a test set.
- **Live Prediction:** Uses a live-updating system (with scheduling) to fetch the latest stock data and predict the next closing price in real time.

 **Install the required libraries:**
   You can install the necessary Python libraries using pip. If you have a `requirements.txt` file, run:
   ```bash
   pip install -r requirements.txt
   ```
   Otherwise, ensure you have installed:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `scikit-learn`
   - `tensorflow` (or `tensorflow-gpu` if using GPU)
   - `yfinance`
   - `schedule`

## How to Run
1. **Train the Model & Evaluate:**
   - Open the `CocaCola_Stock_Prediction.ipynb` notebook in Jupyter.
   - Run the cells sequentially to train the model and visualize the predictions on the historical test data.

2. **Live Prediction:**
   - At the bottom of the notebook, a live prediction system is implemented using the `schedule` library.
   - To test live predictions, run the live prediction cell. The system fetches the latest stock data every minute and prints the predicted next closing price.
   - Note: For faster testing, you can adjust the scheduling interval.

## Usage
- **Historical Analysis:** Use the notebook cells to visualize historical trends and model performance.
- **Live Predictions:** The live prediction loop fetches the most recent data, updates the model’s input sequence, and outputs a prediction to the console.


## Acknowledgments
- Data is sourced from Yahoo Finance using the `yfinance` library.
- This project leverages LSTM neural networks using TensorFlow and Keras.
```
