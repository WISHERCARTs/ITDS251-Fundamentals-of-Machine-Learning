# Lab 10: EMNIST Character Classification using CNN

This repository contains the Jupyter Notebook for Lab 10: Convolutional Neural Network (CNN) applied to the EMNIST dataset for character classification.

## 📝 Overview

The goal of this lab is to build, train, and evaluate a CNN model using the EMNIST (Extended MNIST) Balanced dataset. The dataset contains a variety of handwritten letters and digits (47 classes in total).

Functions implemented include:
- Loading and reshaping image data
- Data preprocessing: Normalization, Image Rotation & Flipping
- One-Hot Encoded labels
- Building a deep learning CNN model using TensorFlow/Keras
- Training and tracking the progress (Loss & Accuracy)
- Evaluating the model and saving the optimal weights
- Visualizing predictions using a Confusion Matrix and sample image plots

## 📂 Project Structure

- `6787074_Lab10-CNN-EMNIST.ipynb`: The main notebook containing the data processing, model architecture, training, and evaluation code.
- `6787074_Lab10-CNN-EMNIST.h5`: The trained CNN model saved after evaluating.

## 💾 Dataset Notes

**Important:** The original CSV files for the EMNIST dataset (`emnist-balanced-train.csv` and `emnist-balanced-test.csv`) are **not** included in this repository to save storage space.

If you wish to re-run the notebook, please download the "EMNIST Balanced" dataset and place the CSV files in the same directory as the notebook before execution.

## ⚙️ Requirements

To run this project, make sure you have the following Python libraries installed:
- `numpy`
- `pandas`
- `tensorflow` (which includes `keras`)
- `matplotlib`
- `scikit-learn`
- `opencv-python` (`cv2`)
