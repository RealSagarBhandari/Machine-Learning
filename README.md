#  Machine Learning Concepts & Applications

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.0%2B-orange.svg)](https://scikit-learn.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-ee4c2c.svg)](https://pytorch.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626.svg)](https://jupyter.org/)

A comprehensive collection of Machine Learning projects and experiments exploring various algorithms, from foundational concepts like k-Nearest Neighbors (kNN) and Decision Trees to Deep Learning architectures like Convolutional Neural Networks (CNNs) and Multilayer Perceptrons (MLPs).

This repository is designed as a self-documenting workflow, with detailed Jupyter Notebooks that integrate data theory, code execution, and visual insights.

---

##  Table of Contents
1. [Deep Learning: Image Recognition](#1-deep-learning-image-recognition-mlp-vs-cnn)
2. [Scikit-Learn: kNN & Decision Tree Regressor](#2-scikit-learn-knn--decision-tree-regressor)
3. [Stellar Classification: Algorithmic Benchmarking](#3-stellar-classification-algorithmic-benchmarking)
4. [kNN Regression & Cross Validation](#4-knn-regression--cross-validation)
5. [kNN Classification & Normalization](#5-knn-classification--normalization)
6. [Tech Stack](#️-tech-stack)
7. [Installation & Setup](#-installation--setup)

---

##  Projects Overview

### 1. Deep Learning: Image Recognition (MLP vs. CNN)
**Directory:** [`Deep_Learning/`](./Deep_Learning) | **Dataset:** CIFAR-10
* **Objective:** Compare the performance of a Multilayer Perceptron (MLP) against a Convolutional Neural Network (CNN) for small-scale color image classification.
* **Key Features:**
  * Baseline fully connected neural network (MLP) implementation.
  * Specialized CNN architecture designed for capturing spatial hierarchies.
  * Custom training loops with forward passes, backpropagation, and mixed-precision optimization.
  * Leverages Apple Silicon (MPS) for hardware-accelerated training.
* **Conclusion:** CNNs significantly outperform MLPs by preserving structural integrity without losing spatial features during flattening.

### 2. Scikit-Learn: kNN & Decision Tree Regressor
**Directory:** [`Scikit_kNN_DecisionTree/`](./Scikit_kNN_DecisionTree) | **Dataset:** White Wine Quality (`winequality-white.csv`)
* **Objective:** Predict wine quality ratings based on chemical properties (acidity, pH, sulfur levels, etc.) using supervised learning models.
* **Key Features:**
  * **kNN Regressor:** Evaluated both Uniform (unweighted) and Distance-based (weighted) neighbor voting, highlighting the importance of Z-score normalization to ensure fair feature representation.
  * **Decision Tree Regressor:** Analyzed node splitting and the effects of limiting tree depth to prevent overfitting (optimal max_depth found between 5-8).

### 3. Stellar Classification: Algorithmic Benchmarking
**Directory:** [`Stellar-Classification/`](./Stellar-Classification) | **Dataset:** Sloan Digital Sky Survey DR-17 (100k observations)
* **Objective:** Classify celestial objects (Stars, Galaxies, Quasars) using an array of experimental machine learning configurations.
* **Key Features:**
  * Comprehensive dimensionality reduction, astrometric, and photometric feature engineering.
  * **kNN Suite Benchmarks:** Baseline, Distance-Weighted, and Normalized trials to prove the *Normalization Hypothesis*.
  * **Tree-based Models:** Decision Tree and Random Forest classifiers.
* **Conclusion:** Tree-based models proved highly robust and invariant to feature scaling (achieving >97% accuracy), while kNN required strict standardization to properly weigh redshift against celestial coordinates.

### 4. kNN Regression & Cross Validation
**Directory:** [`kNN Regression/`](./kNN Regression) | **Dataset:** Car Price Prediction (`Car_Price_Prediction.csv`)
* **Objective:** Implement a kNN Regressor to predict continuous dependent variables based on multi-dimensional independent variables.
* **Key Features:**
  * Non-parametric regression modeling.
  * Rigid evaluation utilizing Cross-Validation techniques.
  * Performance benchmarking primarily focusing on Mean Absolute Error (MAE) and Mean Squared Error (MSE).

### 5. kNN Classification & Normalization
**Directory:** [`kNN and Normalization/`](./kNN and Normalization) | **Dataset:** Fuel Economy Vehicles (`vehicles.csv`)
* **Objective:** Build a robust kNN classifier emphasizing the absolute necessity of preprocessing and scaling in distance-based algorithms.
* **Key Features:**
  * End-to-end data normalization implementations.
  * Clear demonstration of how drastically unscaled features can skew Euclidean distance calculations.

---

##  Tech Stack
* **Language:** Python 3.8+
* **Deep Learning Framework:** PyTorch, Torchvision, Fast.ai (optional integration)
* **Machine Learning:** Scikit-Learn
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebooks (`.ipynb`)

---

##  Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/RealSagarBhandari/Machine-Learning
   cd Machine-Learning
   ```

2. **Install Dependencies:**
   Ensure you have Python 3.x installed. Next, install required packages:
   ```bash
   pip install numpy pandas scikit-learn torch torchvision matplotlib seaborn jupyter
   ```
   
3. **Run the Notebooks:**
   Launch Jupyter Notebook from the root of the repository:
   ```bash
   jupyter notebook
   ```
   Navigate into any project directory and open the respective `.ipynb` file to run the code cells sequentially.

---

**Author:** Sagar Bhandari  
**Date:** Fall 2025  
*Note: These projects were developed as part of an academic curriculum encompassing various machine learning concepts and applications.*
