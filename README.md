# Cryptocurrencies

## Purpose

This project seeks to use unsupervised machine learning techniques to cluster currenty traded cryptocurrencies to assist in the creation of a crytocurrency investment portfolio for Accountability Accounting.

## Project Overview

Using data from [Cryto Compare](https://min-api.cryptocompare.com/data/all/coinlist), we began by preprocessing the data for use with our clustering techniques. This required the creation of dummies for the categorical variables, the standardization of the data, and the reduction of data dimensions using PCA. 

Once the preprocessing was complete and the resulting data recompiled, we created an elbow curve and determined the best value for K = 4. We then used this K to perform K-means clustering on the dataset, grouping the cryptocurrencies into 4 distinct clusters.

Finally, we visualized our results by creating a 3d scatter plot of the K-means clusters, and a table and 2d scatter plot of the total coins mined and the total coins in each cryptocurrency's supply.

## Repositiory

There are two files in the repository:
- Data
- crypto_clustering.ipynb

Data contains the data file _crypto_data.csv_ (drawn from [Crypto Compare](https://min-api.cryptocompare.com/data/all/coinlist)), whereas crypto_clustering.ipynb contains the code needed to cluster the data.

