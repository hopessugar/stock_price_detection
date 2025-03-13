Stock Price Prediction Model 
Overview
This project demonstrates a simple machine learning model for predicting stock prices using Linear Regression. 
The model is trained on historical stock price data (e.g., Apple Inc. - AAPL) and can be used to predict future stock prices. 
The project includes data preprocessing, feature engineering, model training, evaluation, and saving/loading the model for future predictions.

Features
Data Preprocessing: Handles missing values, converts dates to numerical features, and prepares the dataset for training.
Linear Regression Model: A simple yet effective model for predicting stock prices.
Model Saving and Loading: The trained model can be saved and reused for future predictions without retraining.
Visualization: Includes plots for historical stock prices and predicted prices.
Customizable: Easily adaptable to other stocks or datasets.

Requirements
To run this project, you need the following Python libraries:
pandas
numpy
scikit-learn
matplotlib
joblib

Dataset
The dataset used in this project is the historical stock price data for Apple Inc. (AAPL), which can be downloaded from Yahoo Finance. The dataset includes the following columns:
Date: The date of the stock price.
Open: The opening price of the stock.
High: The highest price of the stock on that day.
Low: The lowest price of the stock on that day.
Close: The closing price of the stock (target variable).
Volume: The trading volume of the stock.

Code Structure
The project is organized into the following steps:

Data Loading:
Load the dataset from a CSV file or directly from Yahoo Finance.
Select relevant columns (Date and Close).

Data Preprocessing:
Convert the Date column to datetime format.
Set Date as the index.
Handle missing values.

Feature Engineering:
Create a new feature Days, which represents the number of days since the first date in the dataset.

Model Training:
Split the data into training and testing sets.
Train a Linear Regression model using the training data.

Model Evaluation:
Evaluate the model using Mean Squared Error (MSE) and R² Score.
Plot actual vs predicted stock prices.

Model Saving:
Save the trained model to a file using joblib.

Model Loading and Prediction:
Load the saved model.
Prepare new data for prediction.
Predict stock prices for new dates.


