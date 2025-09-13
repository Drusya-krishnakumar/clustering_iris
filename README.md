Clustering Assessment on Iris Dataset
Objective

The objective of this assessment is to evaluate the understanding and application of clustering techniques on a real-world dataset. Specifically, we apply KMeans and Hierarchical Clustering to the Iris dataset to group similar samples and visualize patterns in the data.

Dataset

Dataset used: Iris Dataset from sklearn.datasets

Features:

Sepal Length

Sepal Width

Petal Length

Petal Width

Target/Label: Species (removed for clustering as it is an unsupervised task)

Clustering Methods Implemented
1. KMeans Clustering

Description:
KMeans partitions the dataset into k clusters by minimizing the distance between each data point and its cluster centroid. The algorithm iterates between assigning points to the nearest centroid and updating centroid positions until convergence.

Suitability for Iris dataset:

The dataset has numeric features suitable for distance-based clustering.

Data points are relatively well-separated, making KMeans effective.

Implementation:

Standardized the dataset using StandardScaler.

Applied KMeans with n_clusters=3.

Visualized clusters using a scatter plot.

2. Hierarchical Clustering

Description:
Hierarchical clustering builds a dendrogram by iteratively merging (agglomerative) or splitting (divisive) clusters. It provides a tree-like structure of data similarity.

Suitability for Iris dataset:

Does not require pre-specifying the number of clusters (can be inferred from dendrogram).

Helps visualize hierarchical relationships between samples.

Implementation:

Used Ward’s linkage method.

Plotted dendrogram to identify clusters.

Assigned 3 clusters based on dendrogram cut and visualized clusters.

Results & Visualizations

KMeans Clustering:
Scatter plot showing 3 clusters based on Sepal Length and Sepal Width.

Hierarchical Clustering:
Dendrogram displaying hierarchical relationships and 3 clusters visualized on scatter plot.

Insight: Both clustering methods group Iris samples effectively. Clusters roughly correspond to actual species, demonstrating the effectiveness of unsupervised learning.



Libraries Used

pandas, numpy – Data manipulation

matplotlib, seaborn – Visualization

sklearn – Dataset loading, KMeans, preprocessing

scipy – Hierarchical clustering and dendrogram
