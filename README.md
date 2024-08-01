# Formative-Assessment-Unsupervised-Learning
The objective of this project is to evaluate the understanding and application of clustering techniques using the Iris dataset.In the dataset we will , preprocess it, and apply two clustering algorithms- (KMeans and Hierarchical clustering). The results will be visualized to understand the clusters formed by each method.

1. Loading and Preprocessing
   
Dataset Overview:

The dataset contains 150 samples with each sample belonging to one of three species. For clustering purposes, the species column will be dropped to focus solely on the feature data.

The Iris dataset is a well-known dataset that contains measurements of four features from three different species of Iris.

 The features are:
•	Sepal length
•	Sepal width
•	Petal length
•	Petal width

Preprocessing Steps:
1.	Load the Dataset: Use load_iris() from the sklearn.datasets module.

2.	Drop the Species Column: Since the species label is not used in clustering, it will be excluded from the feature set.

3.	Standardize the Data: Although not specified, it is often beneficial to scale the data to ensure that all features contribute equally to the clustering process.
	

2. Clustering Algorithm Implementation:

 A) KMeans Clustering:
  
Description of KMeans Clustering:

KMeans clustering is a partition-based method that aims to divide a dataset into K distinct, non-overlapping clusters.

1.	Initializing K centroids randomly.
2.	Assigning each data point to the nearest centroid based on Euclidean distance.
3.	Recalculating the centroids as the mean of the assigned data points.
4.	Repeating steps 2 and 3 until the centroids converge

Why KMeans is Suitable for the Iris Dataset:

The Iris  dataset contains relatively well-separated groups, making it easier for KMeans to identify distinct clusters.
KMeans is efficient for datasets with a moderate number of features and samples. 
The number of clusters (K) can be set to 3, corresponding to the three known species, allowing us to compare the clusters with the actual categories.

Application and Visualization:

•	Apply KMeans: Using KMeans from sklearn.cluster with a specified number of clusters (K=3, based on the known number of species).

•	Visualization: Use a scatter plot with color coding to represent the different clusters.

 B) Hierarchical Clustering
 
Description of Hierarchical Clustering:

Hierarchical clustering is a technique that builds a hierarchy of clusters. It can be agglomerative (bottom-up) or divisive (top-down). Agglomerative clustering starts with each data point as a separate cluster and merges them iteratively until all points belong to a single cluster.: Hierarchical clustering is useful for exploring data when the number of clusters is not known in advance. It provides a dendrogram, which is a tree-like diagram that shows the arrangement of the clusters formed at each stage. This can help identify the optimal number of clusters by examining where large jumps in distances occur.

Why Hierarchical Suitable for the Iris Dataset: 

Hierarchical clustering provides a visual representation of the data's clustering structure through a dendrogram, which can be useful for understanding the data's natural grouping. It does not require the number of clusters to be specified in advance, which can be advantageous for exploratory data analysis.


Conclusion:

Both KMeans and Hierarchical clustering techniques are applied to the Iris dataset. The clusters create  the KMeans were compared with the clusters from Hierarchical clustering. Visualizations provided insights into how these methods grouped the data points and how these clusters relate to the actual species. The project demonstrates the practical application of clustering algorithms and the importance of data preprocessing and visualization in understanding clustering results.





