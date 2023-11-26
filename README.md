# Unsupervised Machine Learning Evaluation Code: Wine Dataset

The provided code applies four different unsupervised machine-learning algorithms to a dataset containing information about wine. The objective is to perform clustering and evaluate the results using common metrics.

brief summary of each algorithm used in the code:

1. KMeans:
Purpose: KMeans is a partitioning method that aims to divide data points into k clusters based on similarity.
Key Parameters: n_clusters specifies the number of clusters.
Evaluation Metrics: Silhouette Score and Davies-Bouldin Score.

2. DBSCAN (Density-Based Spatial Clustering of Applications with Noise):
Purpose: DBSCAN identifies dense regions in data, separating clusters based on the density of data points.
Key Parameters: eps defines the maximum distance between two samples for one to be considered as in the neighborhood of the other, and min_samples sets the number of samples in a neighborhood for a point to be considered a core point.
Evaluation Metrics: Silhouette Score and Davies-Bouldin Score.

3. Agglomerative Clustering:
Purpose: Agglomerative Clustering is a hierarchical clustering method that recursively merges clusters based on proximity.
Key Parameters: n_clusters sets the number of clusters.
Evaluation Metrics: Silhouette Score and Davies-Bouldin Score.

4. Gaussian Mixture Model (GMM):
Purpose: GMM assumes that the data points are generated from a mixture of several Gaussian distributions. It's a probabilistic model that assigns probabilities to each point belonging to different clusters.
Key Parameters: n_components sets the number of Gaussian components.
Evaluation Metrics: Silhouette Score and Davies-Bouldin Score.

Steps in the Code:

1. Import Libraries: The code starts by importing necessary libraries, including scikit-learn for machine learning and pandas for data manipulation.

2. Load Data: The wine dataset is loaded from a CSV file, and the relevant columns for analysis are specified.

3. Feature Extraction: The selected columns are extracted as features (X) for clustering.

4. Apply Unsupervised Algorithms:

- KMeans: Utilizes the KMeans algorithm with the number of clusters set to 2.
- DBSCAN: Applies DBSCAN with specified parameters for epsilon (eps) and minimum samples.
- Agglomerative Clustering: Uses hierarchical clustering with the number of clusters set to 2.
- Gaussian Mixture Model (GMM): Applies GMM with the specified number of Gaussian components.

5. Fit Models and Get Predictions: Each algorithm is fitted to the data, and predictions are obtained.

6. Evaluation Metrics:
For each algorithm, Silhouette Score and Davies-Bouldin Score are calculated to assess the quality of clustering.

7. Print Results and Metrics: Predictions and evaluation metrics are printed for each algorithm.



