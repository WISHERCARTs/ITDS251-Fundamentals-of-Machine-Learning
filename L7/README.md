# Lab 7: Deep Learning for Multiclass Classification

## Overview

Neural network implementation for **multiclass classification** on the **Covertype dataset** using Keras/TensorFlow. The goal is to classify forest cover types (7 classes) based on 54 cartographic features.

## Dataset

- **Name**: Covertype Dataset
- **Samples**: 581,012
- **Features**: 54 (elevation, aspect, slope, distances, hillshade, wilderness area, soil type)
- **Target**: Cover_Type (7 classes, originally labeled 1–7)
- **File**: `cover_dataset.csv`

## Project Structure

```
L7/
├── 6787074_Lab7 DL-Classification.ipynb   # Main lab notebook (multiclass)
├── L7.1 binary_classification.ipynb       # Demo: binary classification
├── L7.2 iris_classification.ipynb         # Demo: iris classification
├── cover_dataset.csv                      # Dataset
├── .gitignore
└── README.md
```

## Model Architecture

| Layer       | Units | Activation | Dropout |
| :---------- | :---: | :--------: | :-----: |
| Dense       |  256  |    ReLU    |   0.3   |
| Dense       |  128  |    ReLU    |   0.3   |
| Dense       |  64   |    ReLU    |    —    |
| Dense (out) |   7   |  Softmax   |    —    |

## Training Configuration

| Parameter     | Value                    |
| :------------ | :----------------------- |
| Optimizer     | Adam (lr=0.001)          |
| Loss          | Categorical Crossentropy |
| Epochs        | 20                       |
| Batch Size    | 64                       |
| Train/Test    | 80% / 20%                |
| Preprocessing | StandardScaler           |

## Results

- **Test Accuracy**: ~88.82%
- First 10 predictions matched true labels perfectly

## Requirements

```
numpy
pandas
scikit-learn
tensorflow
```

## Author

Student ID: 6787074
