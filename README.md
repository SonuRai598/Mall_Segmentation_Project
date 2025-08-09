# 🛍️ Mall Customer Segmentation Using K-Means Clustering

This project applies **K-Means Clustering** to the Mall Customers dataset from Kaggle to identify distinct customer segments based on their **Annual Income** and **Spending Score**. The goal is to uncover meaningful customer groups to help businesses better understand their clientele and tailor marketing strategies.


## 📌 Objectives

- Load and explore the Mall Customers dataset
- Preprocess the data: handle missing values, drop irrelevant columns
- Use the **Elbow Method** to determine the optimal number of clusters
- Apply **K-Means clustering**
- Visualize customer segments in 2D space
- Analyze the characteristics of each cluster

## 📂 Dataset Overview

- **Rows:** 200 customers
- **Columns:** 5 attributes:
  - 'CustomerID'
  - 'Gender'
  - 'Age'
  - 'Annual Income (k$)'
  - 'Spending Score (1–100)'
- No missing or duplicate values were found in the dataset.

## 🔧 Technologies Used

- **Python**
- **Pandas** – data handling
- **Matplotlib & Seaborn** – visualizations
- **Scikit-learn** – scaling & clustering

## 📊 Key Steps & Findings

### ✅ Data Preprocessing
- Dropped `CustomerID` as it doesn’t contribute to clustering.
- Selected `Annual Income (k$)` and `Spending Score (1–100)` as clustering features.
- Applied `StandardScaler` to normalize data.

### ✅ Finding Optimal Clusters
- Used the **Elbow Method** to visualize WCSS (Within-Cluster Sum of Squares).
- Optimal number of clusters chosen: **k = 5**

### ✅ K-Means Clustering
- Fitted KMeans with 5 clusters.
- Assigned each customer to a cluster.

### ✅ Cluster Visualization
- Created a **scatter plot** with clusters colored distinctly.
- Clear separation observed between customer types.

## 📈 Cluster Insights

| Cluster | No. of Customers | Traits   |   Interpretation |
| **0**   | 81               | Moderate income, moderate spending | Value-conscious shoppers |
| **1**   | 39               | High income, high spending        | Profitable, brand-aware |
| **2**   | 22               | Low income, high spending         | Impulsive or experience-driven buyers |
| **3**   | 35               | High income, low spending         | Wealthy but cautious spenders |
| **4**   | 23               | Low income, low spending          | Budget-conscious group |

## 📌 Business Implications

- Target **Cluster 1** for premium services and loyalty programs.
- Convert **Cluster 3** with trust-building and personalization.
- Engage **Cluster 2** with perceived-value offerings.
- Use discounts or bundles for **Cluster 0**.
- Approach **Cluster 4** with entry-level, low-cost strategies.

## 📁 File Structure

Mall_Segmentation_Project/

├── Mall_Segmentation.ipynb
├── Mall_Customers.csv # Dataset 
├── README.md # Project description

## ✅ How to Run

1. Clone the repository or upload the `.ipynb` and `.csv` file to Google Colab or Jupyter Notebook.
2. Run all cells in order.
3. Ensure `Mall_Customers.csv` is in the same directory as the notebook.

## 📎 Dataset Source

Kaggle:https://www.kaggle.com/code/bhaskarchandrajoshi/customer-analysis-mall-customer-csv

## 🧠 Conclusion

This project demonstrates how clustering can help businesses segment their customers and create more targeted, effective marketing strategies using simple, interpretable visualizations.
