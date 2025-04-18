# Clustering Analysis on Wholesale Customers Dataset

This project performs a **comparative performance study of clustering algorithms** using the [Wholesale Customers dataset](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers) from the UCI Machine Learning Repository. The analysis leverages different preprocessing techniques, varying cluster sizes, and multiple evaluation metrics to determine the most effective clustering configuration.

---

## 📊 Dataset Overview

- **Name:** Wholesale Customers Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers)  
- **Number of Features:** 7  
- **Number of Records:** 440  
- **Description:** The dataset contains annual spending in monetary units on various product categories for customers from a wholesale distributor.

---

## ⚙️ Methodology

### 💡 Clustering Algorithms Used
- K-Means
- Hierarchical Clustering (HCLUST)
- MeanShift

### 🔁 Preprocessing Techniques
- No Processing  
- Normalization  
- Transformation  
- PCA  
- Transformation + Normalization (T+N)  
- Transformation + Normalization + PCA (T+N+PCA)

### 🔢 Cluster Counts
- 3 clusters
- 4 clusters
- 5 clusters

### 📐 Evaluation Metrics
- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Score**

---

## ✅ Results Summary

| Metric               | Best Value     |
|----------------------|----------------|
| **Best Algorithm**   | MEANSHIFT       |
| **Best Clusters**    | 3               |
| **Best Silhouette**  | 0.9076          |

All evaluations were performed using the [PyCaret](https://pycaret.org/) library.

---

## 📊 Visualizations

All model evaluations are also visualized using grouped bar plots for:
- Silhouette Score
- Calinski-Harabasz Index
- Davies-Bouldin Score

Each model's performance across different preprocessing techniques and cluster sizes is presented.

---

## 📁 Files Included

- `clustering_comparison_results.csv` – Final result table with all configurations  
- `clustering_KMEANS_Silhouette.png` – Saved plots for each metric/model  
- Jupyter Notebook / Colab Notebook for reproducibility


