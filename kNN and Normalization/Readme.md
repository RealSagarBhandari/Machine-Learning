# kNN Classification & Feature Normalization

## Project Overview
This notebook acts as an applied introduction and rigorous demonstration of **K-Nearest Neighbors (KNN)** classification, emphasizing the absolute necessity of data normalization. By utilizing a real-world Fuel Economy dataset (`vehicles.csv`), this project showcases how unscaled, independent features can wildly disrupt distance-based learning algorithms.

## Core Concepts Explored
- **k-Nearest Neighbors (kNN):** A distance-based classification algorithm that determines the class of a data point by polling its \(k\) nearest neighbors.
- **Feature Normalization:** A critical preprocessing stage designed to scale all features to a common range (e.g., 0 to 1) or standardized distribution (Z-score). Without this step, features with inherently larger magnitudes will artificially dominate the Euclidean distance calculations.

*The Jupyter Notebook provides a self-documenting, end-to-end implementation comparing models built on raw data versus normalized data.*

## How to Run
1. Ensure the `vehicles.csv` dataset is present in the current directory. *(Data sourced from [fueleconomy.gov](https://www.fueleconomy.gov/feg/download.shtml))*
2. Open `KNN and Normalization.ipynb` in a Jupyter Notebook environment (or Google Colab).
3. Execute the cells sequentially to observe data ingestion, preprocessing steps, model fits, and evaluation visualizations.

---
**Author:** Sagar Bhandari  
**Date:** September 16, 2025