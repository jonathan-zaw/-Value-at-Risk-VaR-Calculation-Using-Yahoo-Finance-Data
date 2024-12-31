# -Value-at-Risk-VaR-Calculation-Using-Yahoo-Finance-Data
Calculates the Value at Risk (VaR) and Conditional VaR (CVaR) for a diversified portfolio using historical stock data from Yahoo Finance. The project estimates potential portfolio losses based on past returns, with visualizations and risk metrics at a 95% confidence level.




The project uses stock tickers such as **AAPL**, **BND**, **GLD**, **QQQ**, and **VTI**, and involves calculating daily returns, cumulative returns, portfolio returns, and rolling historical returns. The Value at Risk is estimated at a 95% confidence level, with visualizations for better interpretation of risk.

## Key Concepts & Techniques
- **Data Collection**: Downloaded historical stock price data for tickers like AAPL, BND, GLD, QQQ, and VTI using the `yfinance` library.
- **Daily Returns Calculation**: Logarithmic returns are used to calculate the daily percentage change in stock prices.
- **Cumulative Returns**: Calculated to track long-term portfolio performance.
- **Portfolio Return Calculation**: A portfolio is formed with equal weights across the selected tickers, and daily portfolio returns are calculated.
- **Rolling Historical Returns**: Calculated over a rolling 5-day window to assess short-term risk.
- **Value at Risk (VaR)**: VaR is calculated at the 95% confidence level using the Historical Method to estimate potential losses in a 5-day period.
- **Conditional VaR (CVaR)**: Calculated as the average loss beyond the VaR threshold, providing a deeper insight into tail risk.
- **Visualization**: Uses `matplotlib` to create histograms and highlight VaR thresholds for better understanding of portfolio risk.
