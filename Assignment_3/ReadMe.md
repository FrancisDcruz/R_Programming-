Homework Assignment 3: Find all dividends

Data Preparation

Use the 6 stocks ['IBM', 'MSFT', 'GOOG', 'AAPL', 'AMZN', 'FB'] historical data from homework assignment 2.

Load the data to dataframes

You will have 6 dataframes.

Understand how to compute the dividends

There are two columns in each csv file, "Close" and "Adj Close". 
If we compute the ratio of previous day's "Close" price and today's "Close" price, then compare with the ratio of previous day's "Adj Close" price and today's "Adj Close" price, 
on most of days, the two ratios should be equal. On dividend day, the two ratios will have a difference. The difference times today's "Close" price, you will get the dividend.
As the example below, you should be able to use the method to reproduce the $1.5 dividend on 2/8/2018.
 
The result
You result will have 6 dataframes, each of them have two columns, Date and Dividend. The dataframe should only have the rows that represent the divident day and amount.
