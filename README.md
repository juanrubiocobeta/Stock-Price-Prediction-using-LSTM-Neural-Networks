# Stock Price Prediction using LSTM

This project is a demonstration of time-series forecasting using a **Long Short-Term Memory (LSTM)** neural network to predict stock closing prices.

## Project Goal
The objective is to build and train an LSTM model in Python to forecast future price movements based on historical data. The project showcases a complete workflow from data cleaning to model evaluation.

## Methodology
1.  **Data Processing:** The historical stock data is loaded using **Pandas**, cleaned, and indexed by date.
2.  **Scaling:** Data is normalized using `MinMaxScaler` to improve neural network performance. Crucially, the scaler is fit **only on the training data** to prevent data leakage.
3.  **Sequence Generation:** The dataset is transformed into supervised learning sequences (i.e., using a window of past days to predict the next day).
4.  **Modeling:** A multi-layer LSTM model is built using **TensorFlow/Keras**.
5.  **Evaluation:** The model is trained and its predictions are plotted against the actual prices from the validation set to visually assess its performance.

## Technologies Used
- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
