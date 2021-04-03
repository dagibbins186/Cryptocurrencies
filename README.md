# Cryptocurrencies Project Overview
Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. This analysis examines what cryptocurrencies are on the trading market, and how they could be grouped to create a classification system. Since there is no known output for what Accountability Accounting is looking for, the project relies upon unsupervised learning. A clustering algorithm groups the cryptocurrencies into possible new investments. Finally, data visualizations explore the results.
\
\
**Data Cleaning**

Data cleaning steps included:
\
-Keeping all the cryptocurrencies that are being traded.
\
-Maintaining all the cryptocurrencies that have a working algorithm.
\
-Dropping the 'IsTrading' column.
\
-Removing rows that have at least one null value.
\
-Filtering the crypto_df DataFrame so it only has rows where coins have been mined.
\
-Creating a new DataFrame that holds only the cryptocurrency names, and references the crypto_df DataFrame index for this new df.
\
-Removing the CoinName column from the crypto_df DataFrame since it's not going to be used on the clustering algorithm.
\
\
**Unsupervised Learning**

PCA is a statistical technique to speed up machine learning algorithms when the number of input features (or dimensions) is too high. In this model, the PCA algorithm reduces the dimensions of the 'pca' DataFrame down to three principal components. Then, the 'pcs_df' DataFrame is created, with columns 'PC 1', 'PC 2','PC 3', and has the index from the 'crypto_df' DataFrame.
\
\
K-means is an unsupervised learning algorithm used to identify and solve clustering issues. K represents how many clusters there will be. These clusters are then determined by the means of all the points that will belong to the cluster. The K-means algorithm groups the data into K clusters, where belonging to a cluster is based on some similarity or distance measure to a centroid. This project creates an elbow curve using hvPlot to find the best value for K from the 'pcs_df' DataFrame '. Then, it runs the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.
# Results
Data visualizatons with results are below:
\
!["elbow_curve.png"](https://github.com/dagibbins186/Cryptocurrencies/blob/main/Images/elbow_curve.png)
\
!["scatter_plot.png"](https://github.com/dagibbins186/Cryptocurrencies/blob/main/Images/scatter_plot.png)
\
!["newplot.png"](https://github.com/dagibbins186/Cryptocurrencies/blob/main/Images/newplot.png)
