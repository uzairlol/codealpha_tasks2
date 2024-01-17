Task 2: Stock Prediction - Take stock price of any company you want and predicts its price by using LSTM. Use only Jupyter notebook code.

Certainly! Let's break down the code and its purpose step by step:

1. **Import Necessary Libraries**:
   - Imports essential libraries such as pandas, numpy, matplotlib, MinMaxScaler, and TensorFlow for building and training the LSTM model.

2. **Load AAPL Stock Price Data:**
   - Reads Apple Inc. (AAPL) stock price data from a CSV file using pandas.

3. **Consider Only 'Close' Prices:**
   - Extracts and retains only the 'Close' prices from the dataset for analysis.

4. **Visualize Stock Price History:**
   - Plots a time series chart to visualize the historical 'Close' prices of AAPL stock.

5. **Normalize the Data:**
   - Applies Min-Max scaling to normalize the stock prices, ensuring values are within a specified range (0 to 1).

6. **Create Training Dataset:**
   - Prepares the training dataset, comprising 95% of the normalized stock prices.

7. **Create x_train and y_train Datasets:**
   - Creates input sequences (x_train) and corresponding output values (y_train) for training the LSTM model.

8. **Reshape Data for LSTM Model:**
   - Reshapes the input data to meet the requirements of the LSTM model.

9. **Build the LSTM Model:**
   - Constructs an LSTM model with two LSTM layers and two Dense layers, specifying the architecture for time series prediction.

10. **Compile the Model:**
    - Compiles the LSTM model by specifying the optimizer and loss function.

11. **Train the Model:**
    - Trains the LSTM model using the training data, specifying the batch size and number of epochs.

12. **Create Testing Dataset:**
    - Prepares the testing dataset, comprising the remaining 5% of the normalized stock prices.

13. **Create x_test and y_test Datasets:**
    - Generates input sequences (x_test) and corresponding output values (y_test) for evaluating the model.

14. **Reshape Data for LSTM Model:**
    - Reshapes the input test data to meet the LSTM model requirements.

15. **Get Predicted Stock Prices:**
    - Predicts the stock prices using the trained LSTM model and inversely scales the predictions to the original price range.

16. **Visualize Predictions:**
    - Plots the actual stock prices, predictions, and training data to visually assess the model's performance.

The overall goal of this code is to demonstrate the application of Long Short-Term Memory (LSTM) networks for predicting stock prices. The LSTM model is trained on historical stock data, and its performance is evaluated by comparing predicted and actual stock prices on a validation dataset. The visualization provides a clear representation of how well the model captures the stock price trends.
