# Hybrid-Algorithmic-Trading-Strategy-with-LSTM-and-SMA
This repository implements a hybrid algorithmic trading strategy that combines LSTM-based deep learning predictions with technical analysis indicators (SMA, RSI, ATR). The project demonstrates superior performance over traditional buy-and-hold strategies through rigorous backtesting across multiple asset classes.
# Hybrid Algorithmic Trading Strategy with LSTM and SMA

This repository contains a hybrid trading strategy that integrates deep learning (LSTM) and technical analysis indicators to optimize trading decisions. The strategy is designed to outperform traditional approaches by leveraging predictive modeling and dynamic risk management techniques.

## Features

- **Deep Learning Integration:** LSTM model predicts price movements based on historical data.
- **Technical Analysis Indicators:** Utilizes SMA, RSI, ATR, and other indicators for enhanced decision-making.
- **Dynamic Risk Management:** Adjusts thresholds based on rolling volatility to reduce false signals.
- **Backtesting:** Rigorous testing across multiple asset classes (e.g., BTC, COCOA, ETH).

## Results

- **BTC:** Total Return: 196.82%, Sharpe Ratio: 2.59
- **COCOA:** Total Return: 163.88%, Sharpe Ratio: 2.16
- **ETH:** Optimization opportunities identified for better performance.

## Project Structure

```
├── code/                   # Jupyter notebooks for LSTM and strategy implementation
├── data/                   # Historical asset data used for modeling and backtesting
├── results/                # Performance metrics and visualizations
├── reports/                # Detailed project report and analysis
├── README.md               # Repository overview
```

## Methodology

1. **Data Preparation:**
   - Historical price data and indicators (SMA, RSI, ATR, etc.)
   - Normalization using MinMaxScaler
2. **LSTM Model:**
   - Predicts next 5 closing prices based on 48 past time steps
   - Optimized using Adam optimizer and Mean Squared Error (MSE) loss
3. **Hybrid Strategy Implementation:**
   - SMA Crossover for momentum-based trading
   - LSTM predictions for price forecasting
   - Dynamic thresholds based on rolling volatility
4. **Backtesting:**
   - Compared hybrid strategy with traditional buy-and-hold
   - Evaluated using Sharpe and Sortino ratios

## Getting Started

### Prerequisites

- Python 3.8+
- Required libraries: `pandas`, `numpy`, `tensorflow`, `matplotlib`, `sklearn`

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/hybrid-trading-strategy.git
   ```
2. Navigate to the project directory:
   ```bash
   cd hybrid-trading-strategy
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Prepare the dataset:
   - Place historical asset data in the `data/` directory.
2. Run the LSTM model and strategy implementation:
   - Execute the Jupyter notebooks in the `code/` directory.
3. View results:
   - Results and visualizations will be saved in the `results/` directory.

## Contributions

Contributions are welcome! Please fork the repository and submit a pull request for review.
