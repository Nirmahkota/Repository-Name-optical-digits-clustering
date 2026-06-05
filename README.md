#  Optical Recognition of Handwritten Digits Clustering Analysis

### Unsupervised Learning Project using PCA, K-Means, and Hierarchical Clustering

Exploring latent patterns in handwritten digit images through advanced clustering techniques and dimensionality reduction in R.

---

##  Project Overview

The **Optical Recognition of Handwritten Digits Dataset** is a classical machine learning dataset containing handwritten digit images represented by numerical pixel-based features.

This project investigates whether handwritten digits naturally form meaningful groups without using class labels.

The analysis incorporates:

* Principal Component Analysis (PCA)
* K-Means Clustering
* Hierarchical Clustering
* Silhouette Analysis
* Cluster Purity Evaluation

---

##  Research Objectives

* Explore the structure of handwritten digit data.
* Perform feature standardization.
* Apply dimensionality reduction using PCA.
* Determine optimal clustering structures.
* Compare clustering algorithms.
* Evaluate cluster quality using multiple metrics.

---

##  Dataset Information

| Attribute     | Value                                     |
| ------------- | ----------------------------------------- |
| Dataset       | Optical Recognition of Handwritten Digits |
| Source        | UCI Machine Learning Repository           |
| Observations  | 5,620                                     |
| Features      | 64 Numerical Variables                    |
| Classes       | 10 Digits (0–9)                           |
| Learning Type | Unsupervised Learning                     |

### Dataset Source

https://archive.ics.uci.edu/ml/datasets/Optical+Recognition+of+Handwritten+Digits

---

##  Methodology

```text
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Feature Standardization
     │
     ▼
Principal Component Analysis
     │
     ▼
Cluster Optimization
(Elbow + Silhouette)
     │
     ▼
K-Means Clustering
     │
     ▼
Cluster Evaluation
     │
     ▼
Hierarchical Clustering
```

---

## Technologies

### Software

* R
* RStudio
* Git
* GitHub

### Main Libraries

```r
library(tidyverse)
library(ggplot2)
library(cluster)
library(factoextra)
library(caret)
library(corrplot)
```

---

##  Code Preview

### Data Standardization

```r
X <- digits[,1:64]
y <- digits$Digit

zero_var <- apply(X,2,var)==0
X <- X[,!zero_var]

X_scaled <- scale(X)
```

### Principal Component Analysis

```r
pca_model <- prcomp(
  X_scaled,
  center = FALSE,
  scale. = FALSE
)
```

### K-Means Clustering

```r
set.seed(123)

kmeans_model <- kmeans(
  X_scaled,
  centers = 10,
  nstart = 50
)
```

---

##  Repository Structure

```text
.
├── README.md
├── digits_clustering.Rmd
├── digits_clustering.html
```

---

##  Key Findings

* PCA successfully reduced dimensional complexity.
* K-Means identified meaningful latent groups.
* Silhouette analysis provided cluster quality assessment.
* Hierarchical clustering revealed hierarchical relationships among observations.

---

##  Future Improvements

* Gaussian Mixture Models (GMM)
* DBSCAN Clustering
* Spectral Clustering
* Interactive PCA Visualization
* Davies-Bouldin Index
* Calinski-Harabasz Index

---

##  handsome Author

**Dzakyyy good person**

Statistics Student - Enggineering Faculty
Universitas Sultan Ageng Tirtayasa

### Interests

* Data Science
* Statistical Learning
* Machine Learning
* Data Analytics
* Applied Statistics

---

 If you find this project useful, consider giving it a star HEHEHEHEHEHEHE
