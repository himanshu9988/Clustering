# Clustering
Comparitive performance study of different clustering algorithms using different pre-processing techniques with different numbers of clusters on different evaluation parameters

Clustering: An Overview
Clustering is a fundamental technique in unsupervised machine learning, aiming to group similar data points together based on certain features or characteristics. The primary goal is to discover inherent patterns, structures, or relationships within the data without the need for predefined labels. Clustering finds applications in various fields, including data analysis, pattern recognition, image segmentation, and customer segmentation.

Key Concept:
1. Objective
The primary objective of clustering is to partition a dataset into groups, or clusters, where points within the same cluster are more similar to each other than to those in other clusters.

2. Similarity Measure
Clustering relies on a similarity measure to quantify the likeness between data points. Common metrics include Euclidean distance, cosine similarity, and correlation coefficient.

Clustering Methods:
1. K-Means Clustering
K-Means is a popular partitioning method that divides the dataset into 'k' clusters. It minimizes the sum of squared distances between data points and their assigned cluster centroids. The algorithm iteratively refines cluster assignments until convergence.

2. Affinity Propagation
Affinity Propagation identifies exemplars (representative points) in the dataset and assigns each point to the nearest exemplar based on similarity. It doesn't require the number of clusters 'k' to be predefined, making it suitable for diverse cluster shapes and sizes.

3. Mean Shift Clustering
Mean Shift is a density-based clustering method that identifies cluster centers by iteratively shifting towards the mode of the data distribution. It is capable of detecting clusters with irregular shapes and sizes.

4. Spectral Clustering
Spectral Clustering leverages the eigenvalues of the similarity matrix to reduce the dimensionality of the data before clustering. It is effective for non-convex clusters and can capture complex relationships between data points.

5. Agglomerative Clustering
Agglomerative Clustering is a hierarchical method that starts with each point as a singleton cluster and recursively merges the most similar clusters until only one cluster remains. The result is a dendrogram illustrating the hierarchical structure of the data.

6. Density-Based Spatial Clustering (DBSCAN)
DBSCAN identifies clusters based on the density of data points. It groups points that are closely packed and separates outliers. It doesn't require specifying the number of clusters in advance and can discover clusters of arbitrary shapes.

7. OPTICS Clustering
Ordering Points To Identify the Clustering Structure (OPTICS) is an extension of DBSCAN. It provides a more flexible cluster extraction method, allowing the discovery of clusters with varying densities and shapes.

8. Birch Clustering
BIRCH (Balanced Iterative Reducing and Clustering using Hierarchies) is a hierarchical clustering algorithm designed for large datasets. It incrementally builds a tree-like structure to represent the data, making it memory-efficient and suitable for streaming data.

About The Notebook(Clustering.ipynb):
Clustering.ipynb notebook is been generated to perform clustering on the dataset-Raisin_Dataset.csv.All the 8 type of clustering is been done on the dataset and got value of certain set of parameters mainly;Silhouette,Calinski-Harabasz,Davies-Bouldin

First five rows of dataset:- image

Elbow-Plot

image

Distribution-Plot: image

Result of K-means after applying different normalization techniques:

image

Result of Affinity Propagation after applying different normalization techniques:

image

Result of Agglomerative Clustering after applying different normalization techniques:

image

Result of Mean shift clustering after applying different normalization techniques:

image

Result of Spectral Clustering after applying different normalization techniques:

image

Result of Density-Based Spatial Clustering after applying different normalization techniques:

image

Result of OPTICS Clustering after applying different normalization techniques:

image

Result of Birch Clustering after applying different normalization techniques:

image

Conclusions
In context of no data preprocessing among the 8 types of clustering provided , the mean shift clustering gave the best silhouette value with no of clusters = 4

In context of using normalization, among the 8 types of clustering provided , the Spectral Clustering gave the best silhouette value with no of clusters = 3

In context of using transformation, among the 8 types of clustering provided , the Spectral Clustering gave the best silhouette value with no of clusters = 3

In context of using PCA, among the 8 types of clustering provided , the Mean shift clustering gave the best silhouette value with no of clusters = 3

In context of using normalization + transformation, among the 8 types of clustering provided , the Spectral Clustering gave the best silhouette value with no of clusters = 3

In context of using normalization + transformation + PCA, among the 8 types of clustering provided , the Spectral Clustering gave the best silhouette value with no of clusters = 3
