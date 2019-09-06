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
 -	Monte Carlo Method - used geometric Brownian motion (GBM) along with Monte Carlo Method

	Monte Carlo Method - We run many trials with random market conditions, then we calculate portfolio losses for each trial. At the end, we use the aggregation of all these simulations to establish how risky the stock is.

	Geometric Brownian motion (GBM) means that past information on the price of a stock is independent of where the stock price will be in the future, basically meaning, we can't perfectly predict the future solely based on the previous price of a stock.
	
		ΔS=S(μΔt+σϵ√Δt)
			 -	Where S is the stock price, 
			 -	mu is the expected return (which we calculated earlier),
			 -	sigma is the standard deviation of the returns, 
			 -	t is time, and 
			 -	epsilon is the random variable.
			 
			 

	Implementation : 
	-	Used random function to genearte random coefficient, used daily returns to calculate sigma and mu. Developed a logic to calculate above formula in loop for more than 1000 occurences for 365 days each. 
	-	Plotted the graph of only the last values in 365 days and calculated the VaR using empirical quartile at 0.01.
		
			 
==============================================================================

Conclusion - 
-	Amazon for every initial stock purchase one would be putting $54.61 at risk 99% of the time (initial price 1192.95 )
-	Google for every initial stock purchase one would be putting $41.11 at risk 99% of the time ( initial price 1065.96)
-	Microsoft for every initial stock purchase one would be putting $3.05 at risk 99% of the time ( initial price 83.75)
-	Twitter for every initial stock purchase one would be putting $1.80 at risk 99% of the time ( initial price 24.62)

===============================================================================


Useful Links Referred :

 https://www.investopedia.com/terms/v/var.asp
 
 https://www.investopedia.com/terms/r/risk-analysis.asp
 
 https://www.investopedia.com/terms/m/montecarlosimulation.asp
 
 https://www.investopedia.com/articles/07/montecarlo.asp




	




