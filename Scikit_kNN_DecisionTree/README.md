# Scikit-Learn: kNN & Decision Tree Regressor

## Project Overview
This project evaluates and compares two supervised learning models—**k-Nearest Neighbors (kNN)** and **Decision Tree Regressor**—on the **White Wine Quality** dataset. The dataset tracks chemical properties such as acidity, pH, and sulfur levels to predict a sensory quality rating.

## Models & Approaches
### 1. k-Nearest Neighbors (kNN) Model
The kNN model makes predictions by examining the wines most similar (closest in feature space) to the one being predicted.
- **Weighted vs. Unweighted Voting:** Explored both `Uniform` (all neighbors have equal say) and `Distance-based` (closer neighbors have more influence) approaches. The weighted version consistently performed better.
- **The Importance of Normalization:** Since features have varying scales (e.g., "Total Sulfur Dioxide" vs "pH"), standard Euclidean distance calculations can be heavily skewed. **Z-score normalization** was strictly applied to ensure every feature contributed fairly.

### 2. Decision Tree Regressor
The Decision Tree makes a sequence of conditional "Yes/No" splits to categorize the data into leaves containing similar target values.
- **Node Splitting:** Optimizes groups so wines in each leaf are as similar as possible.
- **Tree Depth limits:** Allowing the tree to grow indefinitely led to "memorization" of the training data (overfitting) and poor generalization on test data. Constraining the `max_depth` to approximately **5 to 8** yielded the best evaluation metrics on unseen data.

## How to Use
1. Ensure `winequality-white.csv` is in the directory.
2. Open and run the `Scikit_kNN_DecisionTree.ipynb` notebook using Jupyter.

---
**Author:** Sagar Bhandari  
**Date:** October 09, 2025