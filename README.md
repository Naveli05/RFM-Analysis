📊 RFM Customer Segmentation Using Superstore Dataset

This project applies RFM (Recency, Frequency, Monetary) Analysis to the popular Sample Superstore dataset to identify customer value segments and support data-driven marketing strategies. The workflow includes data preprocessing, feature engineering, scoring, segmentation, and visualization.

📁 Project Overview

RFM analysis is a proven technique used in CRM and marketing analytics to classify customers based on their purchase behavior:

Recency → How recently a customer made a purchase

Frequency → How often they purchased

Monetary → How much revenue they generated

Using these metrics, customers are classified into meaningful segments (e.g., Top, High Value, Lost Customers), enabling targeted marketing and retention strategies.

🧰 Tools & Libraries Used

Python

Pandas

NumPy

Matplotlib

xlrd (for reading Excel files)

📂 Dataset

The project uses the Sample Superstore dataset containing:

Order details

Customer details

Product data

Sales, quantity, discount & profit

💡 Total records: 9,994 rows | Columns: 21

🔍 Workflow Summary
1. Data Loading and Exploration

Loaded the Excel dataset using pandas.read_excel.

Checked datatypes, null counts, basic statistics.

Explored categorical frequency distributions.

2. RFM Feature Engineering

Created separate R, F, and M dataframes:

Recency: Days since last purchase

Frequency: Number of transactions per customer

Monetary: Total revenue per customer (Sales × Quantity)

3. Merging into RFM Table

Combined Recency, Frequency, and Monetary values into a single RFM dataframe.

4. Ranking & Normalization

Ranked Recency, Frequency, and Monetary scores.

Normalized to 0–100 scale for comparison.

5. RFM Scoring

Final score computed using weighted formula:

Metric	Weight
Recency	15%
Frequency	28%
Monetary	57%
6. Customer Segmentation

Customers categorized based on RFM Score:

RFM Score Range	Segment
> 4.5	Top Customer
4.0 – 4.5	High Value Customer
3.0 – 4.0	Medium Value Customer
1.5 – 3.0	Low Value Customer
≤ 1.5	Lost Customer
7. Visualization

A pie chart shows the distribution of customer segments.

📈 Insights

The segmentation reveals how customers differ in buying behavior.

High-value segments can be targeted for loyalty programs.

Low and lost segments can be targeted for reactivation campaigns.

Monetary value strongly influences the final customer score.

🚀 How to Run the Project

Clone this repository

git clone <your-repository-url>


Install dependencies

pip install pandas numpy matplotlib xlrd


Place the dataset in the project folder.

Run the Python script/Jupyter notebook.
