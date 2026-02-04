# Lab 5: k-NN & Decision Tree Classification

## 📋 Overview

Binary classification lab using **k-Nearest Neighbors (k-NN)** and **Decision Tree** algorithms on the Heart Attack dataset.

## 📁 Files

| File               | Description                        |
| ------------------ | ---------------------------------- |
| `L5_Demo.ipynb`    | Demo notebook with examples        |
| `L5_Lab.ipynb`     | Lab exercises (completed)          |
| `Heart_Attack.csv` | Dataset (303 samples, 14 features) |

## 📊 Dataset

**Heart Attack Prediction Dataset**

- **Samples:** 303 patients
- **Features:** 13 (age, sex, cp, trtbps, chol, fbs, restecg, thalachh, exng, oldpeak, slp, caa, thall)
- **Target:** `output` (0 = low risk, 1 = high risk)

## 🧪 Lab Results

### Model Comparison

| Model             | Test Accuracy | Best Hyperparameter |
| ----------------- | ------------- | ------------------- |
| **k-NN**          | 88.52%        | k = 13              |
| **Decision Tree** | 81.97%        | max_depth = 3       |

### Key Learnings

1. **k-NN requires scaling** - uses distance-based calculations
2. **Decision Tree does NOT require scaling** - uses threshold-based splits
3. **Cross-Validation** - used to find optimal hyperparameters (k and max_depth)
4. **StratifiedKFold** - preserves class distribution across folds

## 🔧 Dependencies

```python
numpy
pandas
scikit-learn
```

## 🚀 How to Run

1. Open `L5_Lab.ipynb` in Jupyter Notebook
2. Run all cells sequentially
3. Results will show accuracy and predictions for both models
