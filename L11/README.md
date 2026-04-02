# Lab 11: Dimensionality Reduction using PCA

This repository contains the Jupyter Notebook for Lab 11: Dimensionality Reduction using Principal Component Analysis (PCA) on the Wine dataset.

## 📝 Overview

The goal of this lab is to explore the technique of PCA to reduce the dimensionality of high-dimensional datasets while preserving as much information (variance) as possible.

Key steps implemented include:
- **Data Loading**: Importing the Wine dataset and exploring its 13 chemical features.
- **Data Preprocessing**: Feature standardization to prepare for variance-based analysis.
- **PCA Implementation**:
  - Calculating the Covariance Matrix.
  - Obtaining Eigenvalues and Eigenvectors.
  - Sorting and selecting Principal Components based on their explained variance.
- **Visualization**: Creating 2D plots of the transformed data to see how the classes (wine types) are separated in a reduced feature space.
- **Explained Variance**: Analyzing the Explained Variance Ratio to decide how many components are sufficient to represent the dataset.

## 📂 Project Structure

- `6787074_Lab11_pca.ipynb`: The primary notebook for implementing PCA and visualizing the results.
- `pca-jupyter-notebook.ipynb`: Reference notebook for PCA steps.
- `wine dataset.csv`: The chemical analysis dataset of wines grown in the same region in Italy.

## ⚙️ Requirements

To run this project, make sure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
