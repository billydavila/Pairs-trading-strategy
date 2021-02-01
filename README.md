# Pairs-trading-strategy

# Objective: In this repository, we will create a pairs trading strategy using two commodities(Lead and Aluminium) future data from the Multi Commodity Exchange of India Limited from April 2014 to July 2016.   

# Background
Arbitrage in commodities can be found in three instances: cash and carry, future calendar spread, and inter-commodity arbitrage. Our focus in this repository will be inter-commodity arbitrage. By considering different commodities on the same exchange having the same cash flow or in the same category, there is a possibility for creating an inter-commodity arbitrage. One example could be the pair commodity Lead and Aluminium which are in the same market category (metal) with a similar cash flow. The strategy suggests to take positions against the general norms of the market, short the overperforming asset, go long the underperforming one. The idea is that cointegrated assets are mean-reverting in nature. Hence, the bought underperforming asset will likely rise and the sold underperforming asset will likely fall back to its mean. Cointegrated assets are found when the spread of the portfolio is stationary. To find a linear combination, we use a Linear Regression. To check if the linear combination or the spread is stationary, we use the augmented dicker-fuller test. The lookback period chose to perform the linear regression was 90 days. For entering a position, we used a threshold and z-score to determine the position to take. If the z-score is above the threshold, we take a short position. If the z-score is below the negative threshold, we take a long position. For exiting the position, we used stop loss, take profit, and cointegration break status.

# Financial Data
We used quandl to gather future data for two commodities(Lead and Aluminium). The collected data was stored in two separated CSV files. The collected data was from date April 2014 to July 2016. Before employing the strategy, we cleaned the data and ensure we only deal with common dates only. As a threshold decider, we used a 1.75 standard deviation away from the mean. The stop loss trigger is -10000 and the take profit trigger is 20000.   

# Analysis Results
For the analysis results, we only calculated: the Hit Ratio, Sharpe Ratio, Positive trades, Negative Trades, and total Profit & Loss.   


