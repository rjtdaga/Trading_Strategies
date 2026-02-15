# Trading_Strategies
In this repository, I have explored momentum and reversal trading strategies for Bitcoin trading without pairing. I have compared the trading strategies to a buy-and-hold strategy and S&P500 returns during the same period. To quantify and compare the strategies, I have computed the following parameters:
* Sharpe Ratio
* Volatility
* Maximum Drawdown
* Maximum Drawdown duration
* Gross return
* Net return adjusted for execution cost (assumed constant at 20bps)
The work has been done on data obtained from binance API from 1 Jan 2020 to 31 Dec 2025 in a 4 hour time period. The data is split 70/30 into backtest data and test data to predict returns on unseen data. First, optimal parameters (like look back period, threshold to buy) have been calculating for different strategies using back test data. Then the strategies with optimal parameters have been used to predict returns for the rest of the data (30%).

From the analysis done specifically on the above strategies, the following points are concluded:
* Momentum-based strategies outperform buy-and-hold and reversal strategy. Reversal strategies do worse than buy-and-hold strategy for data with period of 4 hours.
* The best Sharpe ratio with momentum strategy for back-test data is 1.41, with volatility 0.525 and mean return 0.000484 for 4-hour data. For test data, the Sharpe ratio is 0.8 with volatility 0.34 and mean return 0.000185 for 4-hour data.
* For buy-and-hold strategy, the Sharpe ratio for back-test data is 1.1 with volatility 0.69 and mean return 0.0005. For test data, the Sharpe ratio is -0.055 with volatility 0.572 and mean return -0.00002.
* For reversal strategy, the Sharpe ratio for back-test data is 1.1 with volatility 0.447 and mean return 0.000313. For test data, Sharpe ratio is -0.616 with volatility 0.42 and mean return -0.00017.
 
