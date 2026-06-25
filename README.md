# Customer Segmentation using RFM Analysis and Clustering

## Project Overview

Customer segmentation is a key business strategy that helps companies understand customer behavior and design targeted marketing campaigns. This project uses RFM (Recency, Frequency, Monetary) analysis along with K-Means and DBSCAN clustering algorithms to identify distinct customer segments from transactional e-commerce data.

The objective is to transform raw customer transaction data into actionable business insights and recommend marketing strategies for each customer group.

---

## Business Problem

Businesses often treat all customers similarly, leading to inefficient marketing efforts and reduced customer retention. By segmenting customers based on purchasing behavior, organizations can:

* Identify high-value customers
* Improve customer retention
* Personalize marketing campaigns
* Increase customer lifetime value
* Optimize promotional spending

---

## Dataset

**Dataset:** Online Retail Dataset

The dataset contains one year of transactional data from an online retail store, including customer purchases, quantities, prices, and transaction dates.

### Key Features

* InvoiceNo
* StockCode
* Description
* Quantity
* InvoiceDate
* UnitPrice
* CustomerID
* Country

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Cleaning

* Removed missing Customer IDs
* Removed cancelled transactions
* Removed records with invalid quantities and prices

### 2. Feature Engineering

Created the following RFM features:

#### Recency

Number of days since the customer's last purchase.

#### Frequency

Number of unique purchases made by the customer.

#### Monetary

Total amount spent by the customer.

### 3. Data Transformation

* Applied logarithmic transformation to reduce skewness
* Standardized features using StandardScaler

### 4. Clustering

#### K-Means Clustering

* Used Elbow Method to determine optimal number of clusters
* Evaluated clustering quality using Silhouette Score

#### DBSCAN Clustering

* Applied density-based clustering
* Compared performance with K-Means

### 5. Cluster Profiling

Analyzed customer behavior within each cluster using average RFM values.

### 6. Marketing Recommendations

Developed business strategies tailored to each customer segment.

---

## Visualizations

### RFM Distributions

### Elbow Method

### Silhouette Score Analysis

### Customer Clusters (PCA Visualization)

---

## Customer Segments

### Champions

Characteristics:

* Recent purchases
* High purchase frequency
* High spending

Marketing Strategy:

* VIP rewards
* Exclusive offers
* Early access to new products

### Loyal Customers

Characteristics:

* Frequent purchases
* Consistent engagement

Marketing Strategy:

* Loyalty programs
* Product recommendations
* Cross-selling campaigns

### Big Spenders

Characteristics:

* High monetary value
* Premium purchasing behavior

Marketing Strategy:

* Premium memberships
* Personalized promotions
* Priority customer support

### At-Risk / Lost Customers

Characteristics:

* Long time since last purchase
* Low recent activity

Marketing Strategy:

* Win-back campaigns
* Discount coupons
* Re-engagement emails

---

## Key Findings

* RFM features successfully captured customer purchasing behavior.
* K-Means clustering produced interpretable customer segments suitable for business applications.
* DBSCAN identified outliers and dense customer groups but was less effective for generating business-friendly segments.
* Customer segmentation can help organizations improve retention, personalization, and revenue generation.

---

## Future Improvements

* Customer Lifetime Value (CLV) prediction
* Churn prediction using machine learning
* Advanced clustering techniques such as Hierarchical Clustering and Gaussian Mixture Models
* Interactive dashboard development using Power BI or Streamlit

---

## Author

Snigdha Singh

Data Science | Customer Analytics
