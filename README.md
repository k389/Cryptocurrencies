# Cryptocurrencies
Supervised Machine Learning

# Project Overview/Challenge
	- Preprocess the data for dimensions reduction with PCA and clustering using K-means.
	- Reduce data dimensions using PCA algorithms from sklearn.
	- Predit data using cryptocurrencies data using K-means algorith from sklearn.
	- Create 3d and scatter plot, and a table using hvplot. 

# Resources
- Data Source: "crypto_data.csv" from The data was retrieved from https://min-api.cryptocompare.com/data/all/coinlist.
- Software: Python 3.6.9:: Anaconda, Inc., Jupyter Notebook, 6.0.2, Visual Studio Code, 1.40.2, sklearn

# Summary
- Preprocessed the crypto_data
	- removed null values.
	- removed all cryptocurrencies that were not trading - InTrading =False.
	- removed columns that will not be used for analysis.
	- created dummies variables for all text features and stored the data in a dataframe X
	- scaled the data using StandardScaler
- Reduce data dimensions using PCA algorithms from sklearn.
	- reduced the preprocessed dataframe down to three principal components.
	- after data reduction stored the reduced data into a dataframe named pcs_df.
- Predit data using cryptocurrencies data using K-means algorith from sklearn.
	- used K-means to cluster the cryptocurrencies using the PCA data that was stored in pcs_df.
	- created an Elbow Curve to determine how many clusters to use for K-means.
	- ran K-means algorithm with 4 clusters. 
- Create 3d and scatter plot, and a table using hvplot.
	- created new dataframe to include columns (Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class) to be used for the plots and table
	- used 3d scatter plot to plot 3 principal components (PC 1, PC 2, PC 3) with CoinName and Algorithms to display when hovering over the data point.
	- used hvplot.table to create table with CoinName, Algorithm, ProofType, TotalCoinSupply, TotalCoinsMined, and Class columns.
	- scaled the values in TotalCoinsMined, TotalCoinSupply columns to be used in the scatter plot.
	- used hvplot.scatter to create a scatter plot with scaled TotalCoinsMined, TotalCoinSupply and CoinName to display when hovering over the data point.

