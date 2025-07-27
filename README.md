# 🛍️ Online Retail Customer Segmentation – Capstone Project

This project focuses on **segmenting customers** of an online retail store based on their purchasing behavior. Using **Machine Learning and RFM (Recency, Frequency, Monetary) analysis**, we identified key customer segments to help businesses tailor marketing strategies, improve customer engagement, and boost overall profitability.

---

## 🧾 Objective

To perform customer segmentation using clustering algorithms (KMeans and Agglomerative Clustering) by analyzing transactional data from an online retail business. This segmentation helps identify high-value customers, frequent buyers, and inactive clients, enabling data-driven business decisions.

---

## 🧠 Project Pipeline

### 1. 🧹 Data Preprocessing
- Loaded the dataset and handled missing values.
- Filtered out records with negative or zero quantity and price.
- Converted date columns into datetime formats.
- Removed canceled orders and duplicates.
- Extracted useful time-based features like Invoice Month.

### 2. 📊 Exploratory Data Analysis (EDA)
- Analyzed customer distribution across countries.
- Checked purchase trends across time.
- Identified top-selling products and purchase patterns.

### 3. 🧾 RFM Analysis
- **Recency**: Days since last purchase.
- **Frequency**: Number of purchases.
- **Monetary**: Total spent by the customer.

Based on RFM scores, we assigned customer segments such as:
- **Platinum** – Recent, frequent, and high spenders.
- **Gold** – Active and moderate spenders.
- **Silver/Bronze** – Irregular or low-value customers.

### 4. 🤖 Customer Segmentation
Applied two clustering techniques:
- **KMeans Clustering** (with optimal k using Elbow & Silhouette Score).
- **Agglomerative Clustering** (Hierarchical linkage analysis).

### 5. 📈 Visualization
- Cluster scatter plots
- Dendrograms for hierarchy
- RFM distributions across segments

---

## 📁 Dataset Details

- **Source**: UCI Machine Learning Repository  
- **Records**: 541,909 transactions  
- **Period**: December 2010 – December 2011  
- **Attributes**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🛠️ Technologies Used

- **Python 3.10+**
- **Libraries**:
  - `pandas`, `numpy` – Data manipulation
  - `matplotlib`, `seaborn` – Visualizations
  - `scikit-learn` – Clustering models
  - `scipy` – Hierarchical clustering

---

## 📊 Model Evaluation

| Algorithm              | Optimal Clusters | Silhouette Score |
|------------------------|------------------|------------------|
| KMeans Clustering      | 4                | ~0.53            |
| Agglomerative Clustering | 4              | ~0.51            |

✅ **KMeans** was selected as the final model due to its better clustering cohesion and computational efficiency.

---

## 🔍 Key Business Insights

- A small portion of customers (Platinum) accounts for most revenue — high retention value.
- Many customers buy infrequently and spend little — opportunity for re-engagement strategies.
- RFM segmentation allows personalized offers, loyalty programs, and targeted promotions.

---

## 📂 Project Structure
📦 Customer_Segmentation/
📒 Online_Retail_Customer_Segmentation_Capstone_Project.ipynb
├── 📄 README.md
├── 📊 data.csv 
