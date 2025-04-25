
Bitcoin Price Prediction using LSTM
Project Overview
This project utilizes a Long Short-Term Memory (LSTM) model to predict the price of Bitcoin over the next 30 days. LSTM, a type of Recurrent Neural Network (RNN), is highly effective for time series forecasting tasks, making it ideal for predicting the price trends of Bitcoin, which is heavily influenced by historical data.

The model is trained on historical Bitcoin price data and predicts future values based on patterns identified during training.

Features
Data Preprocessing: The dataset is cleaned and normalized for better model performance.

LSTM Model: An LSTM network is used to capture long-term dependencies in Bitcoin's historical price data.

Prediction for Next 30 Days: The model predicts the closing price of Bitcoin for the next 30 days.

Data Visualization: Predicted prices are plotted alongside actual prices to visualize the model’s performance.

Dataset
The dataset used in this project contains daily Bitcoin prices including the opening price, closing price, highest price, lowest price, and trading volume. The dataset is typically sourced from platforms like:

Yahoo Finance

Dependencies
This project requires the following Python libraries:

pandas - For data manipulation and analysis.

numpy - For numerical operations.

matplotlib - For plotting the results.

tensorflow - For building the LSTM model.

sklearn - For data preprocessing and evaluation.

Model Architecture
The LSTM model in this project is designed with the following layers:

LSTM Layers: Capture sequential data patterns from the historical Bitcoin prices.

Dropout Layers: Prevent overfitting by randomly disabling a fraction of neurons during training.

Dense Layer: Outputs the final prediction for the Bitcoin price.

The model is trained using Mean Squared Error (MSE) as the loss function and Adam optimizer.

Model Training and Evaluation
Training: The model is trained using 80% of the dataset and tested on the remaining 20%.

Prediction: The trained model predicts the Bitcoin prices for the next 30 days based on the test data.

Evaluation: The performance is evaluated using Mean Squared Error (MSE) and Mean Absolute Error (MAE) to assess the prediction accuracy.

Results
The model predicts Bitcoin’s future prices based on historical trends. Below is a sample of the predicted prices for the next 30 days:

The results are visualized in graphs comparing the predicted prices with the actual closing price

Conclusion
The LSTM model provides a solid foundation for predicting Bitcoin prices. While the model can make reasonably accurate predictions, further enhancements like including more features (e.g., market sentiment, trading volume) and utilizing more advanced techniques could improve its performance.

Future Work
Incorporating More Features: Consider including features like social media sentiment, news articles, and trading volumes to improve accuracy.

Hyperparameter Tuning: Fine-tune the LSTM model’s hyperparameters for optimal performance.

Higher Frequency Data: Use minute-level or hourly data for more granular predictions.
