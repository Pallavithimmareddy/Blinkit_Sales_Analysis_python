# 🛒 Blinkit Sales Analysis using Python

## 📘 Project Overview
The **Blinkit Sales Analysis Project** focuses on analyzing sales data to uncover performance trends, customer behavior, and revenue insights using Python.  
This project applies **Exploratory Data Analysis (EDA)** and visualization techniques to identify the top-performing categories, regional sales patterns, and time-based sales fluctuations.  

The goal is to help business teams make data-driven decisions for better **inventory management**, **marketing optimization**, and **sales forecasting**.

---

## 🎯 Business Objectives
- Analyze total revenue, total orders, and average order value (AOV).  
- Study category-wise and regional sales patterns.  
- Identify top-performing and low-performing products.  
- Explore customer buying behavior using time-based trends.  
- Visualize insights using Matplotlib and Seaborn.

---

## 🧰 Tools & Technologies Used
| Category | Tools |
|-----------|-------|
| **Programming Language** | Python 🐍 |
| **Libraries** | Pandas, NumPy, Matplotlib, Seaborn |
| **Development Environment** | Jupyter Notebook |
| **Data Source** | Blinkit Sales CSV Dataset |
| **Report Format** | PDF & Jupyter Notebook |

---

## 📊 Project Workflow

### 1️⃣ Data Collection
- The dataset (`Blinkit_Sales.csv`) includes fields such as `Order ID`, `Date`, `Category`, `Item Name`, `Quantity`, `Price`, `Total Price`, and `Region`.  
- Example shape of dataset: **(119,390 rows × 32 columns)**.

---

### 2️⃣ Data Cleaning & Exploration
Performed the following preprocessing steps:
- Checked for **null values** and **duplicates**.
- Identified **data types** and **summary statistics**.
- Renamed inconsistent columns and formatted dates.
- Used `df.describe()`, `df.isnull().sum()`, and `df.info()` for profiling.

---

### 3️⃣ Exploratory Data Analysis (EDA)
EDA was conducted using Python to uncover insights such as:
- **Total revenue**, **average order value**, and **total quantity sold**.
- **Sales by product category and region**.
- **Daily and monthly order trends**.
- **Top 10 products by revenue** and **bottom 10 by demand**.

Example EDA Queries:
```python
# Total Revenue
df['Total Price'].sum()

# Top Categories by Revenue
df.groupby('Category')['Total Price'].sum().sort_values(ascending=False)

# Monthly Sales Trends
df.groupby('Month')['Total Price'].sum()
## 4️⃣ Data Visualization
Visualized sales and performance patterns using Matplotlib and Seaborn.  
**Example Visuals:**

- **Bar Chart** — Revenue by Category  
- **Pie Chart** — Revenue by Region  
- **Line Chart** — Monthly Sales Trend  
- **Heatmap** — Correlation between numerical variables

<p align="center">
  <img src="reports/category_revenue.png" alt="Revenue by Category" width="500"/> &nbsp;&nbsp;
  <img src="reports/monthly_trends.png" alt="Monthly Sales Trends" width="500"/>
</p>

---

## 5️⃣ Key Insights
- ✅ **Most Ordered Categories:** Snacks and Beverages  
- ✅ **Peak Order Days:** Fridays and Weekends  
- ✅ **Top Performing Regions:** Metro and Tier-1 Cities  
- ✅ **Revenue Growth:** Increased during festive months (October–December)  
- ✅ **Customer Trend:** High demand for ready-to-eat and quick snacks

---

## 6️⃣ Final Deliverables

- 📘 **Notebook:** `notebooks/Blinkit_Python_Analysis.ipynb`  
- 📄 **Professional Report (PDF):** `reports/Blinkit_Python_Analysis_Report.pdf`  
- 📊 **Sample Dataset:** `data/Blinkit_Sales.csv`

---


