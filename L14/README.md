# Lab 14: Machine Learning Model Deployment (Heart Attack Prediction)

This repository contains the Jupyter Notebooks and resources for Lab 14. The objective of this lab is to develop a machine learning model to predict heart attack risk and deploy it as a REST API using the Flask framework.

## 📝 Overview

In this lab, we implemented a complete end-to-end machine learning deployment pipeline, consisting of the following stages:

### 1. Model Development (`Create Model`)
- **Data Exploration**: Analyzed the `Heart_Attack.csv` dataset, including statistical analysis and correlation visualization using heatmaps.
- **Data Cleaning**: Handled missing values and removed duplicate rows to ensure data quality.
- **Feature Engineering**: Selected relevant features for prediction (e.g., `cp`, `thalachh`, `exng`, `oldpeak`).
- **Training**: Trained a machine learning model using `scikit-learn` and applied `StandardScaler` for data normalization.
- **Serialization**: Saved the trained model (`model.pk`) and the scaler (`scaler.pk`) using the `pickle` library for deployment.

### 2. Model Server (`Model Server`)
- **API Development**: Created a RESTful API using **Flask**.
- **Inference Logic**: Implemented a POST route (`/`) that:
    - Receives JSON input containing patient features.
    - Loads the pre-trained model and scaler.
    - Preprocesses the input data and returns the prediction result.

### 3. Client Implementation (`client`)
- **Request Handling**: Implemented a client notebook that uses the `requests` library to send data to the server and receive prediction results.
- **Validation**: Tested the deployment by verifying that the server correctly classifies different patient profiles.

## 📂 Project Structure

- `6787074_Lab14_Create Model.ipynb`: Notebook for data analysis, model training, and serialization.
- `6787074_Lab14_Model Server.ipynb`: Flask-based server for model inference.
- `6787074_Lab14_client.ipynb`: Client application for requesting predictions.
- `Heart_Attack.csv`: The dataset used for model training.
- `model.pk` & `scaler.pk`: The serialized machine learning model and feature scaler.

## ⚙️ Requirements

To run this project, ensure you have the following Python libraries installed:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `flask`
- `requests`
- `pickle`
