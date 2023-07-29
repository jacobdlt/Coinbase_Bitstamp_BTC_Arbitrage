# Coinbase / Bitstamp BTC Arbitrage

## Overview

The purpose of this analysis is to identify potential Bitcoin arbitrage opportunities historically within Coinbase and Bitstamp. 

To this I collected, prepared, and analyzed BTC trade data from both exchanges from January - April 2018.

1.) I first read the trade data for each exchange into a Pandas dataframe.

2.) Secondly, I dropped all "na" values and duplicates as well as converted the data in the close price column to a float from a string to prep for analysis.

3.) I then generated summary statistics and used line graphs to plot the close prices for both dataframes. I overlayed the plots for easier comparison

4.) Next I focused my analysis on three dates, January 15th, February 10th, and March 15th and did the following:

    * measured the arbitrage spread between both exchanges (subtracted lower-priced exchange from higher-priced)

    * calculated the spread returns by dividing the instances that have a positive arbitrage spread by the price of BTC from the lower-priced exchange

    * narrowed down trading opportunities even further by determining the number of times trades with positive returns exceeded the 1% minimum threshold needed to cover trading costs

    * calculated the potential profit in dollars per trade by multiplying the spread returns greater than 1% by the BTC cost

    * calculated the arbitrage profits made on each day by summing proift_per_trade

## Results


