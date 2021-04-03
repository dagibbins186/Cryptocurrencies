# Cryptocurrencies Project Overview
Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. This analysis examines what cryptocurrencies are on the trading market, and how they could be grouped to create a classification system. Since there is no known output for what Accountability Accounting is looking for, the project relies upon unsupervised learning. A clustering algorithm groups the cryptocurrencies into possible new investments. Finally, data visualizations explore the results.
# Results
**Data Cleaning**
\
Data cleaning steps included:
\
1. Keeping all the cryptocurrencies that are being traded.
\
2. Maintaining all the cryptocurrencies that have a working algorithm.
\
3. Dropping the 'IsTrading' column.
\
4. Removing rows that have at least one null value.
\
5. Filtering the crypto_df DataFrame so it only has rows where coins have been mined.
\
6. Creating a new DataFrame that holds only the cryptocurrency names, and use the crypto_df DataFrame index as the index for this new DataFrame.
\
7. Removing the CoinName column from the crypto_df DataFrame since it's not going to be used on the clustering algorithm.
