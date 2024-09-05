# Crypto Clustering Project

## Overview

This project performs clustering analysis on cryptocurrency market data using K-Means and PCA (Principal Component Analysis). The main objective is to cluster cryptocurrencies based on their market performance, and then compare the clusters created using the original data versus the PCA-transformed data.

## Project Structure

- **`Crypto_Clustering.ipynb`**: Jupyter notebook containing the data processing, clustering, and visualization steps.
- **`crypto_market_data.csv`**: The dataset used for the analysis, containing market data for various cryptocurrencies.
- **`Resources/`**: Folder containing external datasets and files used for the project.

## Key Steps in the Notebook

### Data Preprocessing:
- Load cryptocurrency market data from a CSV file.
- Normalize the data using `StandardScaler` to ensure features are on the same scale.

### Clustering with K-Means:
- Fit K-Means clustering on the original scaled data.
- Compute the optimal number of clusters using the Elbow method (inertia-based) and silhouette score.

### Dimensionality Reduction with PCA:
- Apply PCA to reduce the data to two principal components.
- Perform K-Means clustering on the PCA-transformed data and visualize the clusters.

### Visualization:
- Generate Elbow plots comparing inertia values for both original and PCA-reduced data.
- Visualize the clusters for both original and PCA data, displaying the clustering structure side by side.
