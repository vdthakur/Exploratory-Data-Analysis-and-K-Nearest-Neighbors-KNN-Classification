# Exploratory Data Analysis and K-Nearest Neighbors (KNN) Classification

This repository contains a detailed analysis and implementation of K-Nearest Neighbors (KNN) classification on the Vertebral Column Data Set. The dataset includes six biomechanical attributes derived from the shape and orientation of the pelvis and lumbar spine. The goal is to classify patients into two binary categories: `Normal (0)` and `Abnormal (1)`.

---

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Project Tasks](#project-tasks)
  - [Preprocessing and Exploratory Data Analysis (EDA)](#preprocessing-and-exploratory-data-analysis-eda)
  - [KNN Classification](#knn-classification)
  - [Metric Variants and Weighted Voting](#metric-variants-and-weighted-voting)
  - [Learning Curve](#learning-curve)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [References](#references)

---

## Introduction

This project was built as part of an assignment for my graduate Machine Learning course. The main objective is to perform binary classification on the Vertebral Column dataset using KNN and its variations. We also explore the effects of different distance metrics, weighted voting, and training set sizes on classification performance.

---

## Data

The Vertebral Column Data Set contains six biomechanical attributes of the pelvis and lumbar spine. The dataset is publicly available at the UCI Machine Learning Repository:

### Attributes:
1. **Pelvic Incidence**
2. **Pelvic Tilt**
3. **Lumbar Lordosis Angle**
4. **Sacral Slope**
5. **Pelvic Radius**
6. **Grade of Spondylolisthesis**

### Classes:
- **Normal (0)**
- **Abnormal (1)**

---

## Project Tasks

### Preprocessing and Exploratory Data Analysis (EDA)
1. **Scatterplots**: Visualize relationships between independent variables, using color to indicate the class labels.
2. **Boxplots**: Analyze the distribution of each feature for both classes.
3. **Train-Test Split**: Select the first 70 rows of `Normal (0)` and the first 140 rows of `Abnormal (1)` for training, using the remaining data for testing.

### KNN Classification
1. **Implementation**: Implement KNN with the Euclidean distance metric or use a software library.
2. **Hyperparameter Tuning**: Evaluate test errors for various values of `k` and identify the optimal `k*`.
3. **Performance Metrics**: Compute the following for the optimal `k*`:
   - Confusion Matrix
   - True Positive Rate
   - True Negative Rate
   - Precision
   - F1-Score

### Metric Variants and Weighted Voting
1. Replace Euclidean distance with:
   - **Minkowski Distance**:
     - Manhattan distance 
     - Logarithmic Minkowski distance
     - Chebyshev distance
   - **Mahalanobis Distance**
2. Replace majority voting with **weighted voting**, using distances as weights. Evaluate performance for Euclidean, Manhattan, and Chebyshev metrics.

### Learning Curve
1. Evaluate the best test error rate for different training set sizes.
2. Plot the relationship between training set size and test error.

---

## Results

- **Optimal k**: Identified using training and test error rates.
- **Distance Metrics**: Comparison of test errors across Euclidean, Manhattan, Minkowski, and Mahalanobis distances.
- **Weighted Voting**: Improvements over majority polling were analyzed and reported.
- **Learning Curve**: Visualized the impact of training set size on performance.

---

