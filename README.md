# Low-Volatility-Factor-Portfolio

## Introduction

### This project aims to demonstrate the volatility factor portfolios which are able to outperform the BSE100 benchmark index when mean variance optimisation is applied. The portfolios are able to have better risk adjusted returns compared to the benchmark index on a one-year period.
### The portfolios are constructed on a quarterly basis and are rebalanced at the end of every quarter.
### The top 20 stocks ranked by the volatility factor are chosen for a particular quarter form the equal weight portfolio. 
### The mean variance optimisation produces risk-parity and Minimum volatility portfolios. The Equal Weight portfolio, risk-parity portfolio and Minimum volatility ### portfolios out of- sample performance is recorded against the benchmark index on a quarterly performance basis.
### The back-test runs in a walk-forward fashion wherein the in-sample training set data forms the rebalanced portfolio and its performance metrics are calculated ### in the subsequent next quarter against the benchmark index performance. This ensures that look ahead bias is eliminated from the back-test. A total of five ### ### quarters of performance metrics of the portfolios out of sample returns are recorded against the benchmark BSE100 index.
### The out of sample quarterly returns series based on daily data for the five quarters are stitched together to form a continuous returns time series to  calculate and visualise performance metrics.

## The Low Volatility Factor 

### The Volatility Factor
### The volatility factor is inspired from the paper “Asian Equity Fundamental Factor Model” from Bloomberg authored by Ercument Cahan and Lei Ji in August 2016. ### The factor is comprised of three subfactors as follows:
1.	Return volatility (38%): The volatility of daily returns annualised.
2.	CAPM Beta (27%): The beta of the stock calculated with respect to the benchmark index.
3.	Cumulative range ( 35%) : The ratio of the maximum and minimum stock price over one year.
### The factors are calculated for all the stocks in the universe at the end of each quarter. The zscores are calculated for each subfactor to rescale sector and ### market cap effects across the universe. Finally, the zscores of each of the subfactors are summed up and the final list is ranked and sorted to the get the ### final top 20 stocks for the portfolio.

## Portfolios Performance

## Equal Weight Portfolio

![image](https://github.com/user-attachments/assets/28a95b57-c001-4f95-9164-98d9491925fc)

## Minimum Volatility Portfolio

![image](https://github.com/user-attachments/assets/91e17343-fbe2-4300-977f-ddfce0f8de1d)

## Risk Parity Portfolio

![image](https://github.com/user-attachments/assets/8986b204-7962-4c9e-a7a4-1db290655582)





