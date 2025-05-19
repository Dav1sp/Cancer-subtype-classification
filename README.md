# Cancer subtype classification 

## Overview

This project investigates the application of machine learning techniques to classify molecular subtypes of Glioblastoma Multiforme (GBM), a highly aggressive brain cancer. Specifically, the study focuses on distinguishing between the Classical (prognostically favorable) and Mesenchymal (prognostically adverse) subtypes using high-dimensional gene expression data. Through both unsupervised and supervised learning approaches, the goal is to assess whether gene expression patterns can reveal intrinsic biological structure and enable accurate subtype prediction. The insights gained from this classification task can support improved prognosis and the development of personalized treatment strategies.

## Project Scope

### Input Data:

- A gene expression matrix (logTPM values) across 5000 protein-coding genes.
- A label file indicating the cancer subtype: Classical (0) or Mesenchymal (1).

### Unsupervised Learning:

- Apply dimensionality reduction methods (e.g., PCA, UMAP) for visualization.

- Perform clustering (e.g., K-means, hierarchical clustering) to explore whether subtypes naturally emerge from gene expression patterns.

- Visualize and interpret clustering results in the context of known subtype labels.

### Supervised Learning:

- Develop a binary classification pipeline to predict subtypes based on gene expression.

- Pipeline components include:

  - Cross-validation with K < 5 for model evaluation.

  - Preprocessing with feature scaling (e.g., StandardScaler).

  -Feature selection (e.g., variance filtering, ANOVA F-test, correlation analysis).

  - Model training using at least two classifiers (e.g., SVM, Random Forest, Logistic Regression).

  - Hyperparameter tuning and performance evaluation using metrics: accuracy, precision, recall, and F1-score (mean ± standard deviation across folds).

  - Summarize model performance and discuss findings.
