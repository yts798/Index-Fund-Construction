# Index Fund Construction

This repository contains a demonstration of how to construct a replicated index fund, aiming to approximate the performance of the S&P 500. The project showcases a methodology for selecting a representative subset of stocks and continuously rebalancing this subset to maintain a close correlation with the index.

## Project Overview

The main goal of this project is to replicate the S&P 500 index by selecting a small set of stocks (5, 10, 20, etc.) using K-means clustering and linear optimization techniques. This approach considers factors such as market capitalization, return, and volatility to form a portfolio that mirrors the index's performance as closely as possible.

## Features

- **K-Means Clustering**: This machine learning technique is used to group stocks with similar characteristics to identify representative stocks for the index fund.
- **Linear Optimization**: After the clusters are formed, linear optimization is applied to determine the optimal weights for each selected stock in the portfolio.
- **Rebalancing Strategy**: A strategy is implemented to periodically adjust the portfolio to maintain its alignment with the S&P 500 index.
- **Performance Evaluation**: The tracking error, which measures the divergence between the portfolio's performance and the index, is reported to evaluate how well the index fund replicates the S&P 500.

## Repository Structure

- `cluster.ipynb`: Jupyter notebook containing the clustering algorithm implementation.
- `data_preparation.ipynb`: Jupyter notebook for preparing and cleaning the dataset for analysis.
- `index_daily.csv`: Daily index data used for the analysis.
- `index_monthly.csv`: Monthly index data used for a more granular analysis.
- `stock_daily.csv`: Daily stock data for individual stocks.
- `stock_monthly.csv`: Monthly stock data for individual stocks.
- `stocks_market_caps.csv`: Market capitalization data for the stocks considered in the index fund.
