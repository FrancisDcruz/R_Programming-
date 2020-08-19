Find the two most correlated stocks.
The sample correlation coefficient formula is
 
where 𝑥⎯⎯⎯x¯ and 𝑦⎯⎯⎯y¯ are the sample means of [𝑥1,𝑥2,...,𝑥𝑛][x1,x2,...,xn] and [𝑦1,𝑦2,...,𝑦𝑛][y1,y2,...,yn]

Data Preparation

Download the historial daily data of the entire 2018 for the 6 stocks
tks = ['IBM', 'MSFT', 'GOOG', 'AAPL', 'AMZN', 'FB']

For example, to download IBM data, use the following link to go to yahoo finance page. Find the "Download Data" link to download the csv file to you local disk. https://finance.yahoo.com/quote/IBM/history?period1=1514782800&period2=1546232400&interval=1d&filter=history&frequency=1d
Replace "IBM" with other stock symbol in the above URL, you will be able to download data for other 5 stocks.
You should have 6 csv files on your disk now. IBM.csv, MSFT.csv, etc.
 
Retrieve the "Adj Close" column values as the daily prices of each stock

Load the data into data frame and retrieve the "Adj Close" column values

Compute the correlation between any two stocks' "Adj Close" prices.

You should use the above formula to implement the correlation algorithm. Try to avoid looping.

Conclusion
Print all stock pairs and their correlations from max to min. The format should look like below. The numbers here are dummy numbers.
IBM:MSFT = 0.763
IBM:GOOG = 0.627
...
AMZN:FB = 0.234

Tips: By definition, the correlation is symmetrical, i.e., r_xy = r_yx, so when you have IBM:MSFT, you can skip MSFT:IBM.

