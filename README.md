

# 🛒 RFM-Based Customer Segmentation using Clustering

## 📌 Project Overview

This project focuses on **customer segmentation in e-commerce** using **RFM (Recency, Frequency, Monetary) analysis** combined with multiple clustering techniques. The goal is to identify distinct customer groups and derive actionable business insights.

---

## 🎯 Objectives

* Segment customers based on purchasing behavior
* Identify **high-value (VIP), regular, and churn-risk customers**
* Compare different clustering algorithms
* Detect **outliers and hidden customer patterns**

---

## 📂 Dataset

* **Online Retail Dataset**
* Source: UCI Machine Learning Repository / Kaggle
* Contains transactional data including:

  * CustomerID
  * InvoiceDate
  * Quantity
  * UnitPrice

---

## 🧠 Methodology

### 1. Data Preprocessing

* Removed missing `CustomerID` values
* Removed invalid transactions (negative quantity, zero price)


---

### 2. Feature Engineering (RFM)

* **Recency (R):** Days since last purchase
* **Frequency (F):** Number of transactions
* **Monetary (M):** Total spending

---

### 3. Data Transformation

* Applied **log transformation** to handle skewness
* Adjusted **Recency direction** for consistency
* Performed **feature scaling** (Standardization)

---

### 4. Clustering Techniques

#### 🔹 K-Means Clustering

* Determined optimal K using:

  * Elbow Method
  * Silhouette Score
* Selected **K = 3**

#### 🔹 Hierarchical Clustering

* Used Agglomerative clustering
* Validated K-Means results
* Visualized with dendrogram

#### 🔹 DBSCAN

* Identified:

  * Outliers
  * Niche customer groups
* Captured non-linear patterns

---

## 📊 Results & Insights

### 🔹 Customer Segments Identified

* 🟢 **VIP Customers**

  * High frequency and spending
  * Major contributors to revenue

* 🟡 **Regular Customers**

  * Customer engagement and value
  * Potential for growth

* 🔴 **Churn-Risk Customers**

  * Low activity and spending
  * Require re-engagement

---

### 🔥 Key Insights

* A small group of customers contributes most of the revenue (**Pareto Principle**)
* Customer behavior is clearly segmented and consistent across algorithms
* DBSCAN revealed hidden patterns and high-value outliers
* Medium-value customers represent strong growth opportunities

---

## 📈 Visualizations

* Recency vs Monetary scatter plot
* Frequency vs Monetary scatter plot


---

## ⚙️ Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 🚀 Business Impact

* Enables **targeted marketing strategies**
* Improves **customer retention**
* Identifies **high-value customers for loyalty programs**
* Helps detect **inactive customers for re-engagement**

---

## 📁 Project Structure

```
RFM-Customer-Segmentation/
│
├── Dataset/                         # Raw + processed data
│   ├── online_retail.xlsx
│   ├── processed/
│   │   └── rfm_data.csv
│
├── notebooks/                    # Jupyter notebooks
│   └── rfm_customer_segmentation.ipynb
│
├── README.md                     # Project documentation
├── requirements.txt              # Dependencies
├── .gitignore

```

---

## ⭐ Conclusion

This project demonstrates that combining multiple clustering techniques provides a **comprehensive understanding of customer behavior**. While K-Means offers clear segmentation, Hierarchical clustering validates the structure, and DBSCAN uncovers hidden patterns and outliers, enabling better business decision-making.


---

## 📌 Author

**Apabrita Maity**
(Aspiring Data Scientist)

---
