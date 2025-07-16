# K_Means_Clustering

K-Means Clustering is an unsupervised machine learning algorithm used to group unlabeled datasets into a specific number of clusters, denoted by 'K'.

Here's how it generally works:

1.  **Choose K:** You decide how many clusters (K) you want to find in your data.
2.  **Initialize Centroids:** The algorithm randomly picks K data points from your dataset to be the initial "centroids" (the center points of your clusters).
3.  **Assign to Closest Centroid:** Each data point in your dataset is then assigned to the closest centroid. "Closest" is usually determined by distance (like Euclidean distance). This forms K initial clusters.
4.  **Update Centroids:** Once all data points are assigned, the centroids are re-calculated. The new centroid for each cluster becomes the mean (average) of all the data points assigned to that cluster.
5.  **Repeat:** Steps 3 and 4 are repeated iteratively. Data points are reassigned to the new closest centroids, and centroids are updated again. This process continues until the cluster assignments no longer change significantly, or a maximum number of iterations is reached.

**The Goal:** The aim of K-Means is to minimize the sum of squared distances between data points and their assigned cluster's centroid. This results in clusters where data points within the same cluster are as similar as possible, and data points in different clusters are as dissimilar as possible.

**Analogy:** Imagine you have a pile of different colored candies mixed together, but you don't know which colors they are. You want to sort them into K different bowls.
* You randomly pick K candies and place them in the K bowls (initial centroids).
* Then, you look at each remaining candy and put it in the bowl with the candy it looks most like (assign to closest centroid).
* After all candies are in bowls, you might realize the "center" of each bowl's candies has shifted. So, you adjust the "center" of each bowl to be the average color of the candies in it (update centroids).
* You keep repeating this sorting and adjusting until the candies in each bowl are very similar, and moving them to a different bowl wouldn't make them any "more similar" to the candies already there.
