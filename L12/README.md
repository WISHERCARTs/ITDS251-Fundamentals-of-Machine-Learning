# Lab 12: Comparing Clustering Algorithms on Iris Dataset

This repository contains the Jupyter Notebook for Lab 12: Comparing Multiple Clustering Algorithms (K-means, DBSCAN, and Agglomerative Hierarchical Clustering) on the classic Iris Dataset.

## 📝 Overview

The goal of this lab is to investigate how different clustering algorithms perform on the same dataset and evaluate their effectiveness using standard metrics.

Key steps implemented include:
- **Data Loading**: Importing the Iris dataset.
- **Data Preprocessing**: Feature standardization using `StandardScaler` to ensure all features contribute equally to distance calculations.
- **Dimensionality Reduction**: Applying **PCA (Principal Component Analysis)** to reduce data to 2D for visualization.
- **Clustering Models**:
  - **K-means Clustering**: Partitioning data into $K$ spherical clusters.
  - **DBSCAN**: Density-based clustering to identify clusters of arbitrary shapes and handle noise.
  - **Agglomerative Hierarchical Clustering**: Building a hierarchy of clusters using a bottom-up approach.
- **Model Evaluation**: Comparing results using:
  - **Silhouette Score** (Closeness of points within clusters vs. separation between clusters)
  - **Calinski-Harabasz Index** (Ratio of between-cluster dispersion and within-cluster dispersion)
  - **Davies-Bouldin Index** (Similarity between clusters, where lower is better)
- **Conclusion**: Analysis of the optimal number of clusters and the pros/cons of each algorithm based on the Iris data structure.

## 📂 Project Structure

- `6787074_Lab12-Clustering.ipynb`: The main notebook containing the data processing, model implementation, and performance evaluation.
- `iris_dataset.csv`: The dataset file used for training and exploration.

## ⚙️ Requirements

To run this project, make sure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`
