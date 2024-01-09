# HMM-CryptoStrategist

## Introduction
This project explores the application of Hidden Markov Models (HMM) in developing a cryptocurrency trading strategy. Focusing on Bitcoin (BTC-USD), it utilizes historical data for model training and strategy testing.

## Data Extraction
Historical BTC-USD data is fetched from Yahoo Finance for the period from '2022-01-01' to '2023-12-31', including features like Open, High, Low, Adjusted Close, and Volume.

## Feature Engineering
- Daily returns and price ranges are calculated.
- 12-day and 21-day moving averages are computed.
- The dataset is split into training and testing sets.

## Model Training
A Gaussian Hidden Markov Model with 4 components is trained on 'Returns' and 'Range', aimed at uncovering latent financial states for generating trading signals.

## Signal Generation
- Trading signals are generated based on Moving Average and HMM predictions.
- A combined signal integrates both MA and HMM for decision-making.

## Performance Metrics
- Cumulative returns for both the benchmark (Bitcoin) and the strategy are calculated.
- The Sharpe Ratio, assessing risk-adjusted returns, is computed for both.

## Output Metrics
- `Returns Benchmark`: Total percentage return of Bitcoin.
- `Returns Strategy`: Total percentage return of the strategy.
- `Sharpe Benchmark`: Risk-adjusted return of Bitcoin.
- `Sharpe Strategy`: Risk-adjusted return of the trading strategy.

## Conclusion
This project demonstrates the integration of machine learning in financial trading, particularly using HMM for cryptocurrency trading strategies.

## Running the Project
1. Install Python packages: `pandas`, `numpy`, `hmmlearn`, `yfinance`, `matplotlib`.
2. Execute the script to perform data fetching, model training, and strategy evaluation.
3. Review the output for performance analysis.

## Acknowledgments
- Data source: Yahoo Finance
- Libraries: `pandas`, `numpy`, `hmmlearn`, `yfinance`, `matplotlib`

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
