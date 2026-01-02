# Rock vs Mine Prediction with RDNN

This repository contains a PyTorch implementation of a **Recurrent Deep Neural Network (RDNN)** for classifying underwater objects (Rocks vs. Mines) using sonar data. [cite_start]This project implements the methodology described in the paper *"Rock vs Mine Prediction and Detection for Aquatic Systems: A Comparative Analysis of Different Machine Learning and Deep Learning Algorithms"*[cite: 1, 3].

## Project Overview
* **Goal:** Classify sonar signals as either "Rock" (R) or "Mine" (M).
* [cite_start]**Model:** Recurrent Deep Neural Network (RDNN) using PyTorch[cite: 124, 128].
* [cite_start]**Dataset:** Kaggle Sonar Dataset (`sonar.all-data.csv`)[cite: 90, 100].
* **Hardware:** Optimized for GPU acceleration (CUDA).

## Dependencies
* Python 3.8+
* PyTorch (CUDA support recommended)
* Pandas
* Scikit-learn
* Numpy

## Usage
1.  Ensure `sonar.all-data.csv` is located in the project root directory.
2.  Open the Jupyter Notebook file.
3.  Run the cells sequentially to load data, train the RDNN model, and evaluate performance.

## Current Evaluation Results
The following metrics were achieved in the latest experimental run:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 34.92% |
| **Precision** | 34.92% |
| **Recall** | 100.00% |
| **F1 Score** | 0.5176 |

> **Note:** A Recall of 1.0 with low precision indicates the model is currently biased towards the positive class (predicting "Mine" for most inputs). Future work involves hyperparameter tuning to balance these metrics.
