# Stock-Price-Prediction
This project builds time-series forecasting models (Simple RNN and LSTM) using historical Tesla stock price data to predict the next day's opening price.

🚀 What This Project Covers
✅ Load and explore historical Tesla stock data
✅ Preprocess and scale the data
✅ Build and train a Simple RNN model
✅ Build and train a LSTM model
✅ Visualize predictions on training and validation data
✅ Predict future open price using last 50 days’ data

🗂️ Dataset
Tesla.csv file with historical stock prices
Focuses on the Date and Open columns

🧠 Model Architectures

🔄 Simple RNN
4 stacked SimpleRNN layers with Dropout
Output: 1 neuron (Open price)
Trained on 70% data (X_train, y_train)

🔁 LSTM
2 stacked LSTM layers with Dense output
Better memory handling for time series
Compared with RNN on the same dataset

📊 Visualizations
📉 Training Loss & Accuracy vs Epochs
📈 Predicted vs Actual (both Train & Validation sets)
🕓 Future prediction for next day's opening price

📦 Libraries Used
TensorFlow / Keras (RNN, LSTM)
Pandas, NumPy, Matplotlib
Sklearn (MinMaxScaler)

📅 Future Prediction Example
Predicted Tesla Open Price for 3/18/2017
Simple RNN: $XXX.XX
LSTM: $YYY.YY
(Exact numbers are printed during execution)

💡 How It Works
Prepares training/validation datasets
Scales input features to [0, 1]
Splits data into sequences of 50-day windows
Trains and evaluates models on real historical data
Uses final 50 days for next day forecast
