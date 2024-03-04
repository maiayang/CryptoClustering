# CryptoClustering

In this challenge, we used what we learned about KMeans clustering and Principal Component Analysis to analyze 24-hour and 7-day price changes for different cryptocurrencies.

First, we preprocessed the data by using the StandardScaler to normalize the data. Next, we used a for loop to fit the data to the KMeans model using k values between 1 and 10. Then we plotted an elbow curve of the k values and their inertia values and picked the best value of k based on the plot.

We fit the data to the KMeans model again using the optimal value of k from the previous step. Then we predicted the clusters for each cryptocurrency and plotted the first two features showing the clusters by color.

In the second part of the challenge, we used Principal Component Analysis to see if we would get different results. We reduced the number of features to three principal components and performed the KMeans model on the new data using the same process as before. It was found that the PCA data yielded the same optimal k value as the original data. 

Lastly, we compared the elbow curves and clusters for each set of data in side-by-side hvpots. In conclusion, the PCA data seems to cluster the cryptocurrencies a little more accurately, with fewer overlaps between the clusters.