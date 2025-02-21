# S&P 500 Market Prediction Model

## Overview
This project implements a machine learning model to predict S&P 500 market movements using historical data. The model uses Random Forest classification to predict whether the market will rise or fall on the next trading day. The tools and technologies used are Python and JupyterLab along with the requirements listed below.

## Features
- Historical S&P 500 data analysis from 1927 to 2025
- Random Forest classifier implementation
- Multiple prediction horizons (2, 5, 60, 250, and 1000 days)
- Rolling average and trend analysis
- Backtesting functionality
- Precision score evaluation

## Technical Details

### Data Processing
- Uses yfinance API to fetch S&P 500 historical data
- Processes daily market data including:
  - Opening price
  - Closing price
  - High/Low prices
  - Trading volume
  - Price ratios
  - Rolling averages

### Model Features
- Implements RandomForestClassifier with:
  - 200 estimators
  - Minimum split size of 50
  - Probability threshold of 0.6 for predictions

### Performance Metrics
- Achieves precision score of ~57% in predicting market movements
- Includes comprehensive backtesting framework
- Provides detailed market trend analysis

## Requirements
```
pandas
numpy
scikit-learn
yfinance
matplotlib
```

## Usage
1. Clone the repository
2. Install the required dependencies
3. Run the Jupyter notebook to:
   - Download historical S&P 500 data
   - Train the prediction model
   - Generate and evaluate predictions

## Project Structure
- `market_prediction.ipynb`: Main Jupyter notebook containing analysis and model
- `sp500.csv`: Historical S&P 500 data
- Data processing and model training functions
- Backtesting and evaluation code

## Results
The model demonstrates improved prediction accuracy over random chance, with specific focus on:
- Trend identification
- Market movement patterns
- Risk management through probability thresholds

## Future Improvements
- Additional technical indicators
- Feature engineering optimization
- Alternative machine learning models
- Real-time prediction capabilities

## Note
This project is for educational purposes only. Trading decisions should not be made solely based on this model's predictions.

## License
[MIT License](LICENSE)
