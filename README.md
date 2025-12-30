# Portfolio-Optimiser-Sharpe-Ratio-benchmarked-against-S-P-500
📈 Stock Portfolio Analysis & Optimization
A Python-based financial tool designed to analyze historical stock performance, calculate key risk metrics, and visualize asset correlations. This project utilizes yfinance to fetch real-time market data and provides insights into cumulative returns, drawdowns, and portfolio covariance.

🚀 Features
Dynamic Data Fetching: Automatically downloads historical stock data using the Yahoo Finance API (yfinance).

Performance Metrics: Calculates Daily Returns, Cumulative Returns, and Annualized Volatility.

Risk Analysis: Computes Max Drawdown (in both nominal and percentage terms) to assess downside risk.

Correlation Visualization: Generates a heatmap of the Covariance Matrix to identify asset dependencies.

Interactive Input: Allows users to define their own portfolio tickers and risk-free rate dynamically.

🛠️ Tech Stack
Python

Data Manipulation: pandas, numpy

Market Data: yfinance

Visualization: matplotlib, seaborn

Optimization: scipy

📊 How It Works
User Input: The script prompts the user to enter a Risk-Free Rate (%) and a list of Stock Tickers (e.g., QQQM, SCHD, KO).

Data Processing: It fetches the 'Close' prices starting from 1900-01-01 to the present.

Statistical Analysis:

Computes log returns for daily changes.

Calculates the covariance matrix (annualized).

Derives cumulative max and max drawdown for each asset.

Visualization: Plots a correlation heatmap to visualize how assets move in relation to one another.
The notebook generates a Covariance Heatmap to help with diversification strategies:

Darker Red: Higher positive correlation (assets move together).

Lighter Colors: Lower or negative correlation (potential for diversification).

Shows optimal portfolio weightings + returns benchmarked against S&P500 based on weightings that obtain the highest sharpe ratio
