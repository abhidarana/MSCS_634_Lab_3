# MSCS 634 Lab 3 - K-Means and K-Medoids Clustering

## Purpose

This lab explores unsupervised clustering using the Wine Dataset from the
scikit-learn library. K-Means and K-Medoids clustering algorithms were applied
with three clusters.

The clustering results were evaluated using the Silhouette Score and Adjusted
Rand Index (ARI).

## Dataset

The Wine Dataset contains 178 observations, 13 numerical features, and three
wine classes.

Before clustering, the dataset was examined for:

- Missing values
- Duplicate observations
- Potential outliers
- Feature distributions

The numerical features were standardized using z-score normalization.

## Methods

### K-Means

K-Means clustering was performed using:

- Number of clusters: 3
- Random state: 42
- Multiple centroid initializations

### K-Medoids

K-Medoids clustering was performed using:

- Number of clusters: 3
- Euclidean distance
- Random state: 42

## Evaluation

Both algorithms were evaluated using:

- Silhouette Score
- Adjusted Rand Index (ARI)

PCA was used to visualize the 13-dimensional dataset in two dimensions.

## Key Insights

The clustering results were compared using both quantitative metrics and
visualizations. The algorithm with the higher Silhouette Score produced the
better-defined clusters, while the higher ARI indicated stronger agreement
with the known wine classes.

K-Means uses calculated centroids and is generally efficient for numerical
datasets. K-Medoids uses actual observations as cluster representatives and
can be more robust to outliers.

## Challenges

One challenge was installing and importing the K-Medoids implementation because
the package used for K-Medoids is separate from the standard scikit-learn
package.

Another consideration was determining how to handle potential outliers.
Potential outliers were inspected but were not automatically removed because
they may represent legitimate wine measurements.

## Files

- `MSCS_634_Lab_3.ipynb` - Jupyter Notebook containing the complete analysis
- `README.md` - Project documentation
