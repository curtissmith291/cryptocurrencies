# cryptocurrencies

This repository contains the jupyter notebook and csv data for the Module 18 cryptocurrency analysis challenge.


## Background

A manager for Accountability Accounting asked for a report on the cryptocurrencies on the trading market and how they could be grouped. As there is no known output for the dataset, it was determined that unsupervised learning would be the correct approach. 

## Results

Prior to analysis, the raw data were preprocessed using Pandas, and included dropping missing values, selecting for cryptocurrencies that were currently being traded, and converting datatypes to appropriate types. Dummies were created for string data; then data were scaled as the magnitude between datatypes were quite drastic. 

After preprocessing, PCA was employed to reduce the dimensions to 3. 

An elbow curve was prepared to determine the best value for K for clustering the cryptocurrencies using K-Means - it was determined that K=4 would be the appropriate value. 

Following the grouping and plotting; four cryptocurrencies were significantly apart from the main grouping: BitTorrent, BiblePay, LiteCoinCash, and POA Network. Removing these from the dataset could improve further grouping. 