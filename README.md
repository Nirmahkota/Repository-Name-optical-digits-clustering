# Optical Recognition of Handwritten Digits Clustering Analysis

## Project Overview

This project explores the Optical Recognition of Handwritten Digits Dataset from the UCI Machine Learning Repository using unsupervised learning techniques. The analysis focuses on discovering latent structures within handwritten digit data through dimensionality reduction and clustering methods.

## Objectives

* Explore the characteristics of handwritten digit data.
* Apply Principal Component Analysis (PCA) for dimensionality reduction.
* Identify natural groupings using K-Means Clustering.
* Compare clustering results with Hierarchical Clustering.
* Evaluate clustering quality using Silhouette Analysis and Cluster Purity.

## Dataset

The dataset contains handwritten digit observations represented by 64 numerical features extracted from image pixels.

Source:
https://archive.ics.uci.edu/ml/datasets/Optical+Recognition+of+Handwritten+Digits

## Methods

* Data Preprocessing
* Feature Standardization
* Principal Component Analysis (PCA)
* Elbow Method
* Silhouette Analysis
* K-Means Clustering
* Hierarchical Clustering
* Cluster Evaluation

## Technologies

* R
* RStudio
* tidyverse
* ggplot2
* cluster
* factoextra
* caret

## Repository Structure

```text
.
├── digits_clustering.Rmd
├── digits_clustering.html
├── README.md
```

## Results

The analysis demonstrates that dimensionality reduction using PCA combined with clustering techniques can effectively reveal underlying structures within handwritten digit data. Several digit categories exhibit clear separation, while others show overlapping characteristics due to similarities in handwritten patterns.

## Author

Dzaki

Statistics Student

Universitas Sultan Ageng Tirtayasa
