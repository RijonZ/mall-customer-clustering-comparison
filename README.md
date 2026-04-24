# Clustering Comparison on Mall Customers

This project compares two clustering techniques, K-Means Clustering and Hierarchical Clustering, using the `Mall_Customers.csv` dataset.

The main file in this project is [kmeans_hierarchical_clustering_comparison.ipynb](C:/Users/rijon/Downloads/kmeans_hierarchical_clustering_comparison.ipynb), which brings both methods into one notebook so they can be analyzed on the same data and compared more clearly.

## Files

- [kmeans_hierarchical_clustering_comparison.ipynb](C:/Users/rijon/Downloads/kmeans_hierarchical_clustering_comparison.ipynb): Combined notebook for K-Means and Hierarchical Clustering comparison
- [Mall_Customers.csv](C:/Users/rijon/Mall_Customers.csv): Dataset used for clustering

## Dataset

The dataset contains customer information from a shopping mall. In this notebook, the clustering analysis uses:

- `Annual Income (k$)`
- `Spending Score (1-100)`

These two features are commonly used to group customers based on how much they earn and how much they spend.

## What the Notebook Covers

The notebook is divided into three main parts:

1. K-Means Clustering
2. Hierarchical Clustering
3. Comparison of both models

In the notebook, you will find:

- data loading and feature selection
- the elbow method for K-Means
- the dendrogram for Hierarchical Clustering
- cluster training and prediction
- cluster visualizations
- metric-based comparison between both methods

## Comparison Goal

The purpose of this notebook is not only to build both clustering models, but also to compare how they perform on the same dataset.

The comparison includes:

- visual comparison of the customer groups
- Silhouette Score
- Calinski-Harabasz Score
- Davies-Bouldin Score

These metrics help evaluate how well-separated and meaningful the clusters are.

## Main Result

When both methods were compared on the same dataset using 5 clusters, K-Means performed slightly better overall.

Observed results:

- K-Means Silhouette Score: `0.5539`
- Hierarchical Clustering Silhouette Score: `0.5530`
- K-Means Calinski-Harabasz Score: `247.36`
- Hierarchical Clustering Calinski-Harabasz Score: `243.07`
- K-Means Davies-Bouldin Score: `0.5726`
- Hierarchical Clustering Davies-Bouldin Score: `0.5782`

Based on these values, K-Means gave a slightly stronger clustering result for this dataset, although both methods performed very similarly.

## How to Run

1. Make sure `kmeans_hierarchical_clustering_comparison.ipynb` and `Mall_Customers.csv` are in the same folder.
2. Open the notebook in Jupyter Notebook or JupyterLab.
3. Run the cells from top to bottom.

## Libraries Used

The notebook uses the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`
- `scipy`

If needed, you can install them with:

```bash
pip install pandas numpy matplotlib scikit-learn scipy
```

## Conclusion

This notebook is useful for understanding how two popular unsupervised learning algorithms behave on the same customer segmentation dataset.

It helps show:

- how K-Means forms centroid-based clusters
- how Hierarchical Clustering builds clusters using linkage
- how both approaches compare visually and mathematically

This makes the notebook a good reference for learning clustering as well as comparing different unsupervised learning methods in a simple and practical way.
