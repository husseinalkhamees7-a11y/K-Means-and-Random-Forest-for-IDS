============================================================
# Hybrid Intrusion Detection System (K-Means + Random Forest)
============================================================
This repository contains the implementation of the hybrid Intrusion Detection System (IDS) evaluated on the CICIDS2017 dataset, as described in the accompanying manuscript. The model utilizes K-Means clustering, SMOTE oversampling, and PCA/Chi-Square feature selection to achieve a 99.85% accuracy across 12 evaluated traffic classes.

## Reproducibility Instructions

To exactly reproduce the reported results (e.g., 99.85% accuracy, MCC ≈ 0.996, ARI ≈ 0.997), 
please follow the steps below.

### 1. Environment Setup
The code was developed and tested using Python 3.12.0. Install the required dependencies by running:

pip install -r requirements.txt


This code presents a hybrid intrusion detection system that integrates K-Means clustering with 
the Random Forest algorithm to improve multiclass network traffic classification.
By combining unsupervised and supervised machine learning techniques, the model effectively captures
latent traffic patterns and enhances detection performance. The study addresses class imbalance
using the Synthetic Minority Over-Sampling Technique (SMOTE) and evaluates feature selection
through both Principal Component Analysis (PCA) and Chi-squared (Chi²) methods across multiple
feature subsets. The use of Silhouette Coefficient and Davies–Bouldin Index ensures the optimal
number of clusters is selected. Performance is comprehensively assessed using accuracy, precision,
recall, F1-score, Matthews Correlation Coefficient (MCC), Adjusted Rand Index (ARI), and execution
time. Experimental results on the CICIDS2017 dataset demonstrate outstanding performance.
