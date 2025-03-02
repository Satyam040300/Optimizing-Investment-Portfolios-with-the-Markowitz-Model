Portfolio Optimization using Python

This project implements Modern Portfolio Theory (MPT) using Python to optimize stock allocations for maximum returns and minimal risk. It employs Markowitz’s Efficient Frontier and Sharpe Ratio Maximization to construct an optimal investment portfolio.

The analysis is based on historical stock data fetched via yfinance and includes risk-adjusted return computations, volatility estimation, and efficient frontier visualization.

Features

Fetches Historical Stock Data using yfinance
Computes Mean Returns & Covariance Matrix for asset risk modeling
Optimizes Portfolio via Markowitz’s Efficient Frontier
Maximizes the Sharpe Ratio for best risk-adjusted returns
Finds Minimum Volatility Portfolio (Safest Investment Option)
Plots the Efficient Frontier with 10,000 simulated portfolios
Handles Missing Data & Numerical Stability Issues

Project Methodology

This project follows a structured approach to construct an optimized portfolio:

Data Collection 

Fetches daily stock prices for selected tickers (AAPL, GOOGL, DIS, XOM, PFE) from Yahoo Finance.
Computes daily & annualized returns.

Portfolio Analysis 

Computes the correlation matrix to analyze asset dependencies.
Calculates mean returns and covariance matrix for risk estimation.

Optimization Using SciPy 

Max Sharpe Ratio Portfolio → Finds the best risk-adjusted return.
Minimum Volatility Portfolio → Identifies the safest allocation.

Efficient Frontier Simulation 
Generates 10,000 random portfolios to visualize the risk-return tradeoff.
Highlights optimal portfolios on the Efficient Frontier Plot.

📂 Project Files

File Name	Description

Satyam_Portfolio Optimization using Markowitz Model.ipynb	Main Python script for portfolio optimization
README.md	Project documentation

📈 Example Output

Optimal Portfolio Weights (Max Sharpe Ratio):
AAPL: 0.40
GOOGL: 0.00
DIS: 0.35
XOM: 0.00
PFE: 0.25

Optimal Portfolio (Max Sharpe Ratio): 
Return: 0.2623, Volatility: 0.2187, Sharpe Ratio: 1.0164

Optimal Portfolio Weights (Minimum Volatility):
AAPL: 0.30
GOOGL: 0.10
DIS: 0.20
XOM: 0.20
PFE: 0.20

Optimal Portfolio (Minimum Volatility): 
Return: 0.1821, Volatility: 0.1803
Efficient Frontier Plot
The script generates an Efficient Frontier plot with:
 
Simulated portfolios (scatter plot)
Max Sharpe Ratio Portfolio (red star 🌟)
Minimum Volatility Portfolio (blue star 🌟)

 Concepts Used
 
Modern Portfolio Theory (MPT) - Portfolio diversification to maximize returns for a given risk level.
Sharpe Ratio - Measures risk-adjusted returns.
Efficient Frontier - Visual representation of optimal portfolios.
Covariance & Correlation Matrix - Measures interdependencies among stocks.

 Potential Improvements
 
Add real-time data updates
Incorporate sector-based constraints for risk control
Implement Monte Carlo simulations for better risk modeling
Extend to multi-asset portfolios (bonds, ETFs, crypto, etc.)


Author & Contributions

Satyam(MS in Business Analytics majoring in Finance from University at Buffalo School of Management)
If you found this helpful, feel free to ⭐ the repo and contribute!

