# DSCI 552 Homework 7

| | |
|---|---|
| **Name** | Arnila Kumari |
| **GitHub Username** | Arnila-Kumari |
| **USC ID** | 5892633819 |
| **Course** | DSCI 552: Machine Learning for Data Science |
| **Instructor** | Mohammad Reza Rajati |
| **Homework** | 7 |
| **Description** | Multi-class and multi-label classification with SVMs, k-means clustering, and hierarchical clustering on the Anuran Calls (MFCCs) data set |

## Repository Structure

```
Homework-7/
├── Notebook/
│   └── HW-7.ipynb          # Code, results, and write-ups for all problems
├── data/
│   ├── Frogs_MFCCs.csv     # Anuran Calls (MFCCs) data set
│   └── Readme.txt          # Data set description from UCI
├── .gitignore
└── README.md
```

## Contents

**1. Multi-class and Multi-Label Classification Using SVMs**
- (a) 70/30 random train/test split
- (b)(i) Exact match ratio, Hamming loss, and Hamming score
- (b)(ii) Gaussian-kernel SVM, one-vs-all, tuned by 10-fold CV, on raw and standardized attributes
- (b)(iii) L1-penalized linear SVM on standardized attributes
- (b)(iv) L1-penalized SVM with SMOTE to address class imbalance
- (b)(v) Extra practice: classifier chain

**2. K-Means Clustering on a Multi-Class and Multi-Label Data Set**
- (a) k chosen automatically by the average silhouette score
- (b) Majority (family, genus, species) triplet per cluster
- (c) Hamming distance, Hamming loss, and Hamming score
- Monte Carlo simulation over 50 runs

**3. ISLR 12.6.2**
- Complete and single linkage dendrograms, two-cluster cuts, and an equivalent dendrogram with repositioned leaves

## Key Results

| Model | Exact Match | Hamming Loss |
|---|---|---|
| Gaussian SVM (raw) | 0.9889 | 0.0076 |
| Classifier chain, Gaussian SVM (raw) | 0.9926 | 0.0063 |
| L1 linear SVM | 0.9125 | 0.0570 |
| L1 linear SVM + SMOTE | 0.8536 | 0.0769 |

K-means (k = 4 in all 50 runs): average Hamming distance 0.6719 (SD 0.0170), Hamming loss 0.2240 (SD 0.0057).

## How to Run

1. Install the dependencies:
