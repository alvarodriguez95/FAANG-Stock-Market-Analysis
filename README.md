# FAANG-Stock-Market-Analysis
By Alvaro Rodriguez
## Business Understanding
Given the historical stock price data for Meta (Facebook), Apple, Amazon, Netflix and Alphabet (Google) over the past year, I want to analyze and compare the performance of these companies in the stock market using various data science techniques.

This topic is relevant as there are numerous banks and financial institutions that would benefit from this analysis in order to help their clients either invest or divest from these companies, and help them make better judgments when holding stocks from these companies in order to maximize profits from these holdings.

This topic primarily is focused on the investment and finance side of companies and not purely on the technology side of it, although certain aspects of these companies would affect the financial side as well.

The target audience would be investors that are either looking to invest in these companies or are currently invested and would like to see how the future performance of the stocks of these companies will be.

The impact of the answer would help investors either decide to include these into their investment portfolios or divest from these companies and utilize other forms of investments.

The main domain knowledge we are relying upon would be the previous historical stock prices of these companies given to us through the stock market.

## Data Understanding
The data will be collected from Yahoo Finance for all five companies within the last year.

The raw data will be straight from Yahoo Finance using pip install yfinance.

The features that will be used are the tickers for the companies as well as start dates and end dates of the stock market price of each company, respectively.



## Data Preparation
Stock market performance analysis includes calulating close stock prices, moving averages, and measuring volatility.
![Five Year Stock Price of FAANG](Images/5YrStockPrice.png)

Five-Year Return on Investment from FAANG Companies


Heatmap of Apple Closing Stock Prices from June 2018 to May 2023





## Modeling
Train-Test Split Apple Closing Prices


Sarima Model 

Predicted Model

## Evaluation
The Apple stock would be the best company to predict future prices as it has a 250% rate of return (ROI) in 5 years compared to the rest of the FAANG companies.

This heatmap also shows the closing stock price of Apple from June 2018 to May 2023. The price ranges from 40 (USD) to 180 (USD) in the past 5 years.

Then, a SARIMA Model was used for our train-test split data in order to set up the predictions for June 2023-May 2024.

For our SARIMA model, an order of (1, 1, 1) and a seasonal order (9, 0, 8, 12) was used as it averaged out the Apple prices on the test data.

Our true and predicted data are not aligned, however the predicted data averages the true data from July 2022 to May 2023.

To get a better representation of the variable prices, a root mean squared-error was used.

In this case, the calculated RMSE value is 12.908619305373424. This means that, on average, the predictions of the SARIMAX model have an error of approximately 12.91 (USD) when compared to the actual values. A lower RMSE value indicates better accuracy, so you would ideally want a lower value for the RMSE.

## Conclusion
- Forecasted prices of the Apple stock price tends to generally average the peaks and valleys of the actual stock price instead of giving an identical return.

- Forecasted prices would be better for a long term investment rather than a short-term investment, as it is averaging out the values of the stock price, which is generally trending upwards.

- Apple would still be the best company to invest out of all the FAANG companies.

## Next Steps

- SARIMA Model Iterations: Iterate more models with better accuracy instead of just retreiving a model that averages out the stock price in the future.

- Portfolio Diversity: looking into other companies instead of FAANG to invest in, and polling wither more years or less years depending on the type of investment, whether short term or long term.
