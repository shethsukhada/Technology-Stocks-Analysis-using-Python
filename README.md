# Technology-Stocks-Analysis-using-Python

Analyzed the technology stocks viz Google, Microsoft, Twitter and Amazon to study the trend of daily price, daily return, moving average etc. Also derived the risk involved based on the historical performance of the stocks using Monte Carlo technique.

-	Libraries Used : pandas, numpy, matplotlib, seaborn
-	Data Source    : yahoo finance ( used pandas_datareader.data to extract the data from yahoo finance. )

Initial Analysis :
1. Analyzed the trend of Adjusted Closing Price, Stock Volume and Moving Averages over 10,20 and 50 days.
2. Studied the daily stock returns for all stocks, compared the daily stock returns in pair to see if there is linear relationship.
3. Used pair-plot for visual comparison of all the stock comparisons for Daily Returns and Closing Prices.
4. Used the correlation plot to compare the actual numerical values for the correlation between the stocks' daily return values. Used heatmap to plot the correlation.

Value at Risk Analysis :
Used Bootstrap and Monte Carlo methods to get the value at risk.
Value at risk tell you the maximum amount you could lose for any given stock.
 -	Bootstrap Method - For this calculated empirical quantiles from a histogram of daily returns
 
Useful Links Referred :

 https://www.investopedia.com/terms/v/var.asp
 https://www.investopedia.com/terms/r/risk-analysis.asp
 https://www.investopedia.com/terms/m/montecarlosimulation.asp
 https://www.investopedia.com/articles/07/montecarlo.asp




	




