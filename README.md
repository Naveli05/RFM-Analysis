# 📊 RFM Customer Segmentation Using Superstore Dataset

This project performs **RFM (Recency, Frequency, Monetary)** analysis on the popular **Sample Superstore** dataset to segment customers based on their purchasing behavior. These insights help businesses design targeted marketing, retention strategies, and customer value optimization.

---

## 📁 Project Overview

**RFM analysis** is a widely used CRM and marketing analytics technique that evaluates customers based on:

- **Recency (R):** How recently the customer purchased  
- **Frequency (F):** How often they purchased  
- **Monetary (M):** How much money they spent  

Using these metrics, customers are classified into meaningful value segments such as **Top Customers**, **High Value**, **Medium Value**, and **Lost Customers**.

---

## 🧰 Tools & Libraries Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- xlrd (for reading Excel files)

---

## 📂 Dataset

The project uses the **Sample Superstore** dataset containing:

- Order details  
- Customer details  
- Product data  
- Sales, quantity, discount & profit  

**📌 Total Records:** 9,994 rows  
**📌 Columns:** 21  

---

## 🔍 Workflow Summary

### **1. Data Loading and Exploration**
- Loaded the dataset using `pandas.read_excel()`
- Checked data types, missing values, and summary statistics
- Explored categorical frequency distributions

---

### **2. RFM Feature Engineering**
Created individual R, F, M metrics:

- **Recency:** Days since last purchase  
- **Frequency:** Total number of transactions per customer  
- **Monetary:** Total revenue per customer *(Sales × Quantity)*

---

### **3. Merging into RFM Table**
Combined R, F, and M values into a single **RFM dataframe**.

---

### **4. Ranking & Normalization**
- Ranked customers based on R, F, M  
- Normalized scores to a **0–100 scale** for comparability

---

### **5. RFM Scoring**
Final RFM Score computed using weighted formula:

| Metric    | Weight |
|----------|--------|
| Recency  | 15%    |
| Frequency| 28%    |
| Monetary | 57%    |

---

### **6. Customer Segmentation**

Customers grouped based on RFM Score:

| RFM Score Range | Segment              |
|-----------------|----------------------|
| > 4.5           | Top Customer         |
| 4.0 – 4.5       | High Value Customer  |
| 3.0 – 4.0       | Medium Value Customer|
| 1.5 – 3.0       | Low Value Customer   |
| ≤ 1.5           | Lost Customer        |

---

### **7. Visualization**
- Pie chart of customer segment distribution  
- Helps understand which customer groups dominate the business  
- Enables targeted campaigns and retention strategies  

---

## 📈 Insights

- **Top and High-Value customers** drive the most revenue  
- **Lost customers** represent potential reactivation opportunities  
- Monetary value shows the strongest influence on the final score  
- RFM segmentation provides a clear view of customer lifetime value  

---

## 🚀 How to Run the Project

### **1. Clone the Repository**
```bash
git clone <your-repository-url>
