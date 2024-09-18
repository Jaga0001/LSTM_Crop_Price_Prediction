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

```bash
.
├── dataset.csv                # Data used for training and testing the model
├── model.py                   # PyTorch model implementation
├── model.ipynb                   # Script to train the LSTM model
├── lstm_price_prediction_model.pkl   # Trained model saved in .pkl format
├── requirements.txt           # Required dependencies
└── README.md                  # Project documentation



