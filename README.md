# Cryptocurrencies
# Analysis Overview
The purpose of this project is to use unsupervised machine learning to analyze a database of cryptocurrencies and create a report including the traded cryptocurrencies classified by group according to their features.
This classification report could be used by an investment bank to propose a new cryptocurrency investment portfolio to its clients.
We use the following methods for the analysis:

* preprocessing the database,
* reducing the data dimension using Principal Component Analysis,
* clustering cryptocurrencies using K-Means,
* visualizing classification results with 2D and 3D scatter plots.

# Results
Following the preprocessing and cleaning phase we have a total of 532 tradable cryptocurrencies.


# Clustering Cryptocurrencies using K-Means - Elbow Curve
We don't know what would be the output of the analysis so we are using unsupervised machine learning to identify clusters of the cryptocurrencies.
We produced the elbow curve below using the K-Means method iterating on k values from 1 to 10.

![image](https://user-images.githubusercontent.com/86137857/138979037-4ca0838d-4825-4f15-be70-c9c852984fb7.png)

The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crytocurrencies.

# Visualizing Cryptocurrencies Results
## 3D-Scatter plot with clusters

![image](https://user-images.githubusercontent.com/86137857/138979109-bfdd1be5-9623-4ad2-8f30-eaf9f6d17f46.png)

This 3-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to three principal components.

## 2D-Scatter plot with clusters

![image](https://user-images.githubusercontent.com/86137857/138979469-09b53151-7758-4321-b91b-5adcb38febd6.png)

This 2-D scatter plot was obtained using the PCA algorithm to reduce the crytocurrencies dimensions to two principal components.

Both these scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.

# Tradable Cryptocurrencies Table

![image](https://user-images.githubusercontent.com/86137857/138979586-092f6836-ef95-4b0d-b194-57a2fe98995c.png)

Most of the cryptocurrencies are part of class #0 and #1.
The snapshot above shows that BitTorrent is the only cryptocurrency in class #2.

# 2D-Scatter plot with TotalCoinMined vs TotalCoinSupply

![image](https://user-images.githubusercontent.com/86137857/138979694-d02073f9-b26c-47ff-b12f-5bb7d79a1366.png)

Plotting the scatter plot from two cryptocurrency features directly does not efficiently segregate the different classes. Then using the PCA algorithm is the right method for better visualizations.

# Summary
We have identified the classification of 532 cryptocurrencies based on similarities of their features.
Particularities of each group need to be analyzed to determined their performance and potential interest for the investment bank's clients.
