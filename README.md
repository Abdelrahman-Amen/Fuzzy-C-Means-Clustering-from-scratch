# Fuzzy C-Means Clustering
Welcome to the Fuzzy C-Means Clustering repository! This repository hosts an implementation of the Fuzzy C-Means (FCM) algorithm from scratch, a powerful tool in the realm of clustering and data analysis.

# Introduction
Fuzzy C-Means (FCM) is a widely used clustering algorithm that offers a flexible and intuitive approach to partitioning data into clusters. Unlike traditional crisp clustering algorithms, FCM assigns membership degrees to data points, allowing for a soft assignment of points to clusters. This characteristic makes FCM particularly useful in scenarios where data points may belong to multiple clusters simultaneously or when dealing with noisy or ambiguous data.

In this repository, we provide an implementation of the Fuzzy C-Means algorithm along with usage examples and documentation to help you leverage its benefits in your projects. Whether you're exploring the structure of your data, FCM can be a valuable addition to your toolkit.






*"When employing PCA in conjunction with Fuzzy C-means clustering, it appears that the algorithm converges more efficiently, displaying a notable improvement in convergence quality compared to using the entire (all) dataset. This observation is particularly evident when the dataset is smaller and simpler than our own."



 


# Fuzzy C-mean (FCM): 
* Dividing the data points to set of clusters using membership function between each point in the dataset and all clusters centroids.
* A particular data of the set may be the member of several clusters with different values of membership.
* Input for FCM: Data , C (number of clusters)
* Output for FCM: Mij(Membership matrix) , Cj (cluster centroid) [1 <=j<= C], [1<=i<=n]
  

#steps for Fuzzy C-mean (FCM):
1. Assume the number of clusters to be made C. Such that: 2<=C<=N (N: # of samples)
2. Choose an appropriate level of cluster fuzziness g  Such that: g > 1
3. Initialize the NxC sized membership matrix [M] at random such that: (a) Mij∈ [0.0 ,1.0] and there sum should be 1
4. Compute centroids



![Screenshot 2024-02-20 001143](https://github.com/Abdelrahman-Amen/Fuzzy-C-Means-Clustering-from-scratch/assets/103226865/bbe0b15e-6b70-41e5-964d-ba29e8d5ae1c)
5. Calculate the Euclidean distance between each data point i-th and j-th cluster center dij  
6. Update fuzzy membership matrix[M] according to dij



![Screenshot 2024-02-20 001132](https://github.com/Abdelrahman-Amen/Fuzzy-C-Means-Clustering-from-scratch/assets/103226865/c4401a82-2017-45d0-8cfc-1c5efe7034cf)
7. Repeat until the changes in [M] come out to be less than some pre-specified values.




## We used two datasets
### the first one has a low correlation, so the updated membership matrix was converging very slowly (more iterations).
### the second one has a high relative correlation, so the updated membership matrix was converging relatively fast.
 






