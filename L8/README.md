# Lab 8: Machine Learning Evaluation Methods

## Overview

This lab covers **evaluation methods** for machine learning models using Scikit-learn and TensorFlow/Keras. It includes two main tasks: **regression** (Boston Housing) and **classification** (Iris), each comparing three models with multiple evaluation metrics.

## Datasets

| Dataset        | Samples | Features | Target              | File                 |
| :------------- | :-----: | :------: | :------------------ | :------------------- |
| Boston Housing |   506   |    13    | Median house value  | `boston-dataset.npy` |
| Iris           |   150   |    4     | Species (3 classes) | `iris_dataset.csv`   |

## Project Structure

```
L8/
├── 6787074_Lab8 Evaluation.ipynb       # Main lab notebook
├── L8 EvaluationMethods.ipynb          # Demo: evaluation metrics
├── boston-dataset.npy                   # Boston housing dataset
├── iris_dataset.csv                    # Iris dataset
├── .gitignore
└── README.md
```

## Task 1: Regression (Boston Housing)

### Models

| Model                   | Description                                      |
| :---------------------- | :----------------------------------------------- |
| Linear Regression       | Baseline linear model                            |
| Random Forest Regressor | Ensemble method (random_state=42)                |
| Neural Network          | 2 hidden layers (64 units each), ReLU, 50 epochs |

### Evaluation Metrics

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

### Results

| Model                   |    MSE |  RMSE |   MAE |    R² |
| :---------------------- | -----: | ----: | ----: | ----: |
| Linear Regression       | 11.738 | 3.426 | 2.243 | 0.840 |
| Random Forest Regressor |  7.843 | 2.800 | 2.036 | 0.840 |
| Neural Network          | 12.584 | 3.547 | 2.391 | 0.840 |

## Task 2: Classification (Iris)

### Models

| Model                    | Description                                     |
| :----------------------- | :---------------------------------------------- |
| Logistic Regression      | Baseline linear classifier                      |
| Random Forest Classifier | Ensemble method (random_state=42)               |
| Neural Network           | 2 hidden layers (64 units each), softmax output |

### Evaluation Metrics

- Accuracy
- Precision (weighted)
- Recall (weighted)
- F1 Score (weighted)
- Confusion Matrix

## Training Configuration

| Parameter     | Value          |
| :------------ | :------------- |
| Train/Test    | 80% / 20%      |
| Random State  | 42             |
| Preprocessing | StandardScaler |

## Demo Notebook

`L8 EvaluationMethods.ipynb` demonstrates evaluation metrics for:

- **Regression**: MSE, MAE, RMSE, R²
- **Classification**: F1, Accuracy, Precision, Recall, Confusion Matrix, Classification Report
- **Clustering**: Silhouette Score, Calinski-Harabasz Index, Davies-Bouldin Index

## Requirements

```
numpy
pandas
scikit-learn
tensorflow
scipy
matplotlib
```

## Author

Student ID: 6787074
