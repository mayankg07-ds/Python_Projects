# S&P 500 Stock Prediction Model

This project implements a machine learning model to predict S&P 500 stock movements using historical price data and technical indicators.

## Overview

The model uses Random Forest Classifier to predict whether the S&P 500 will go up or down on the next trading day based on:
- Historical price data (Open, High, Low, Close, Volume)
- Technical indicators including:
  - Rolling averages over different time horizons (2, 5, 60, 250, 1000 days)
  - Price ratios relative to moving averages
  - Trend indicators

## Features

- **Data Source**: Yahoo Finance (yfinance) for S&P 500 data
- **Model**: Random Forest Classifier with optimized parameters
- **Backtesting**: Rolling window backtesting framework
- **Performance Metrics**: Precision score evaluation
- **Technical Indicators**: Multiple time horizon analysis

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- yfinance
- matplotlib

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Open the `SMprediction.ipynb` Jupyter notebook and run the cells sequentially to:
1. Download S&P 500 data
2. Prepare features and targets
3. Train the model
4. Evaluate performance through backtesting

## Model Performance

The model uses a threshold of 0.6 for prediction confidence and evaluates performance using precision score on out-of-sample data.

## License

This project is for educational purposes. Please ensure compliance with relevant financial regulations when using for actual trading decisions.
