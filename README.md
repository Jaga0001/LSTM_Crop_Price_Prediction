# Agri-Horticultural Commodity Price Prediction using LSTM

This repository contains the code and model for predicting prices of agri-horticultural commodities like onion, potato, and pulses using a Long Short-Term Memory (LSTM) model built with PyTorch. The model was developed to assist the Department of Consumer Affairs in predicting commodity prices and aiding in strategic market interventions.

## Problem Statement

The Department of Consumer Affairs monitors the daily prices of 22 essential food commodities through 550 price reporting centres across the country. This project aims to predict the prices of key commodities using AI/ML techniques based on time series data, historical trends, and other market factors. The primary goal is to forecast commodity prices using an LSTM model to assist in managing buffer stock and stabilizing market prices.

## Model Overview

The model uses an LSTM (Long Short-Term Memory) network, a type of Recurrent Neural Network (RNN), which is well-suited for time series forecasting. The key features used in the model include:

- **State**: The region where the price is being monitored.
- **Humidity**: Climate condition affecting crop production.
- **Seasonality**: The cropping season (Rabi/Kharif).
- **Buffer Stock**: Available stock of commodities.
- **Rainfall**: A critical factor affecting crop yield and market supply.
- **Category**: Type of commodity (Onion, Potato, Pulses, etc.).

## Project Structure

    
    ├── dataset.csv                # Data used for training and testing the model
    ├── model.py                   # PyTorch model implementation
    ├── model.ipynb                   # Script to train the LSTM model
    ├── lstm_price_prediction_model.pkl   # Trained model saved in .pkl format
    ├── requirements.txt           # Required dependencies
    └── README.md                  # Project documentation

## Setup and Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/commodity-price-prediction.git
    cd commodity-price-prediction

2.  Install dependencies: The project requires Python 3.12.5. Install the necessary libraries using `requirements.txt`:
   
    ```bash
    pip install -r requirements.txt

3. **Prepare the Dataset**: Make sure the `dataset (dataset.csv)` is available in the root folder.

4. Train the Model: To train the LSTM model using the provided dataset, run the following command:

   ```bash
   python train.py

  This will train the model and save it as lstm_price_prediction_model.pkl.

5. **Make Predictions**: Use the model.ipynb script to make predictions for a particular state and commodity:

  
## Model Performance
The model was evaluated using Mean Absolute Percentage Error (MAPE) and achieved a test accuracy of approximately 89.25%.


## Contributing
We welcome contributions! Please follow these steps:

1. Fork this repository.
2. Create a new branch: git checkout -b feature-name.
3. Make your changes and commit them: git commit -m 'Add new feature'.
4. Push to the branch: git push origin feature-name.
5. Submit a pull request
