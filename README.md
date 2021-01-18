# Pairs-trading-strategy

# Objective: In this repository, we will create a pairs trading strategy between two cointegrated instruments (two ETFs: EWA and EWC) 

# Background
Statistical Arbitrage is a group of trading strategies employing large, diverse portfolio that are traded on a very short-term basis. One example of a statistical arbitrage is the pairs trading strategy. 

Pairs trading is a contrarian strategy designed to harness mean-reverting behavior of cointegrated instruments. By forming a portfolio of two or more instruments such that the portfolio is stationary, we can find instruments that are cointegrated and suitable for our strategy. Since cointegrated pairs are assumed to be mean reverting in nature, we can build a mean reverting strategy where we enter a position when the spread reaches a standard deviation away from its mean and close the position when it goes back to its mean.


# Financial Data
We gather the data for the two ETFs: EWC and EWA from yahoo finance for dates from 2010-01-01 to 2020-12-31. Build the spread between the two instruments by doing a regression. Once we have the spread, we did an augmented dickey-fuller for checking the stationarity in the spread. If the spread is stationary, we have found cointegrated pairs which are mean-reverting in nature and perform the strategy. 

# Analysis Results
For the analysis, we only calculated the Hit Ratio, Sharpe Ratio, Standard deviation of returns, Cumulative PNL, positive trades, negative trades, and Drawdowns of the strategy. We did not calculate more sophisticated profitable return measurements.


