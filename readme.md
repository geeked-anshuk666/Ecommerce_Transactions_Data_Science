# eCommerce Customer Segmentation and Lookalike Modeling - Data Science Assignment

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This repository contains the deliverables for a Data Science assignment focused on eCommerce transaction data analysis. The assignment involved Exploratory Data Analysis (EDA), building a Lookalike Model, and performing Customer Segmentation using clustering techniques on a provided eCommerce dataset.

## Table of Contents

1.  [**Project Description**](#project-description)
2.  [**Dataset**](#dataset)
3.  [**Tasks and Deliverables**](#tasks-and-deliverables)
    *   [Task 1: Exploratory Data Analysis (EDA) and Business Insights](#task-1-exploratory-data-analysis-eda-and-business-insights)
    *   [Task 2: Lookalike Model](#task-2-lookalike-model)
    *   [Task 3: Customer Segmentation / Clustering](#task-3-customer-segmentation--clustering)
4.  [**Tech Stack and Libraries**](#tech-stack-and-libraries)
5.  [**Installation / Requirements**](#installation--requirements)

## Project Description

This project analyzes eCommerce transaction data to derive business insights, build a model to find lookalike customers, and segment customers based on their profiles and transaction history. The goal is to demonstrate data analysis, machine learning, and business understanding skills in an eCommerce context.

## Dataset

The dataset consists of three CSV files:

*   **Customers.csv:** Customer profile information (CustomerID, CustomerName, Region, SignupDate).
*   **Products.csv:** Product information (ProductID, ProductName, Category, Price).
*   **Transactions.csv:** Transaction records (TransactionID, CustomerID, ProductID, TransactionDate, Quantity, TotalValue, Price).

The dataset files are available in the main repository directory.

## Tasks and Deliverables

### Task 1: Exploratory Data Analysis (EDA) and Business Insights

*   **Description:** Performed Exploratory Data Analysis (EDA) on the eCommerce dataset to understand data characteristics and derive business insights.
*   **Deliverables:**
    *   `Anshuk_Jirli_EDA.pdf`: PDF report containing 5 business insights derived from EDA.
    *   `Anshuk_Jirli_EDA.ipynb`: Jupyter Notebook containing the Python code for EDA.

### Task 2: Lookalike Model

*   **Description:** Built a Lookalike Model to recommend 3 similar customers for a given user, based on their profile and transaction history. Cosine similarity was used to calculate similarity scores.
*   **Deliverables:**
    *   `Anshuk_Jirli_Lookalike.csv`: CSV file (`Map<cust_id, List<cust_id, score>>` format) containing top 3 lookalike customer recommendations and similarity scores for the first 20 customers (C0001-C0020).
    *   `Anshuk_Jirli_Lookalike.ipynb`: Jupyter Notebook explaining the Lookalike Model development and code.

### Task 3: Customer Segmentation / Clustering

*   **Description:** Performed customer segmentation using K-Means clustering, leveraging both customer profile and transaction information. Evaluated clustering using the Davies-Bouldin Index and visualized the clusters using PCA.
*   **Deliverables:**
    *   `Anshuk_Jirli_Clustering.pdf`: PDF report on customer segmentation results, including the number of clusters, DB Index value, other clustering metrics, cluster profiles, and visualizations.
    *   `Anshuk_Jirli_Clustering.ipynb`: Jupyter Notebook containing the Python code for customer segmentation, metric calculation, and visualization.



## Tech Stack and Libraries

*   **Programming Language:** Python
*   **Libraries Used:**
    *   pandas
    *   numpy
    *   matplotlib
    *   seaborn
    *   scikit-learn (sklearn):
        *   `sklearn.cluster` (KMeans)
        *   `sklearn.metrics` (davies_bouldin_score, silhouette_score, calinski_harabasz_score, cosine_similarity)
        *   `sklearn.preprocessing` (StandardScaler, OneHotEncoder)
        *   `sklearn.decomposition` (PCA)

## Installation / Requirements

To run the code in the Jupyter Notebooks, you will need to have Python 3.x installed along with the following libraries. You can install these libraries using pip:

```bash
pip install -r requirements.txt
```

Alternatively, you can use conda:
```bash
conda install pandas numpy matplotlib seaborn scikit-learn
```

