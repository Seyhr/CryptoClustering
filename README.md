# CryptoClustering
The purpose of the project is to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

Steps
 --Find the Best Value for k Using the Scaled DataFrame and plot the line chart with inertia value
 --Cluster Cryptocurrencies with K-means Using the Scaled DataFrame( Scatter plot  with x-axis as "price_change_percentage_24h" 
    and the y-axis as "price_change_percentage_7d.
 --Optimize Clusters with Principal Component Analysis( Perform PCA on Scaled DataFrame and reduce the feature upto 3.
 --Find the Best Value for k Using the PCA DataFrame and plot the line chart with inertia value
 --Cluster Cryptocurrencies with K-means Using the PCA DataFrame ( Create a scatter plot with the x-axis as "PC1" and the y- - 
 --axis as "PC2")

Next step is to create Composite plot to contrast the Elbow curves
[Composite Plot for Elbow CUrve](images/Elbow_curve.png)

FInal step is to Composite plot to contrast the clusters
[Composite Plot forCryptoCurrency Clusters](images/cluster_plot.png)

The Elbow Curve for the PCA data shows that with k=4, the inertia is 49.665, while the Elbow Curve for the original scaled data has k=4 with inertia of 79.022. The cluster plot reveals that lower inertia corresponds to tighter, more closely-knit clusters, while higher inertia results in more spread-out clusters. This indicates that PCA helps reduce noise, leading to more accurate clusters. After performing the cluster analysis, we can conclude that using fewer features (via PCA) results in more refined and compact clusters.
