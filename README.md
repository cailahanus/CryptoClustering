# CryptoClustering

## Overview
This project involves a detailed analysis of cryptocurrency data to identify patterns and group similar cryptocurrencies using machine learning clustering techniques. The analysis uses both the original dataset and a dimensionally reduced dataset obtained through Principal Component Analysis (PCA).

## Data Preparation
- Normalization: Data is normalized using StandardScaler from scikit-learn to ensure that the clustering algorithm functions optimally.
- DataFrames: Two main DataFrames are created:
- 1 - Original Scaled DataFrame: Normalized data maintaining original features.
- 2 - PCA DataFrame: Data reduced to three principal components to simplify the feature set.

## Determining Optimal Clusters
- Elbow Method: The number of clusters (k) is determined using the elbow method, where inertia is plotted against different values of k for both the original and PCA-reduced datasets.
- Optimal k: The best value for k is identified from the plots, noted for both datasets.

## Clustering Cryptocurrencies
- K-Means Clustering: Cryptocurrencies are clustered using K-means based on the optimal k values identified.
- Visualization: Results are visualized using hvPlot, with points colored by their cluster labels to show groupings.
- For the original data, principal components are used as axes.
- For the PCA data, selected percentage change features are used.

## Results and Analysis
- Cluster Analysis: An analysis of the clustering results is conducted to compare how the data clusters in the original versus the PCA-reduced datasets.
- Explained Variance: The variance explained by the PCA components is calculated to quantify the information retained after dimensionality reduction.
## Questions Addressed
- Optimal k Value: Determination of the best number of clusters for both original and PCA-reduced datasets, including any differences between them.
- Impact of Dimensionality Reduction: Analysis of how reducing the number of features affects clustering effectiveness and results.

## Conclusion
The project concludes with insights into the patterns within the cryptocurrency market based on the clustering results, highlighting the practical implications of using PCA for dimensionality reduction in clustering scenarios.
