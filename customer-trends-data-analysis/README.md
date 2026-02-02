# 📊 Customer Trends & Revenue Analysis  
### End-to-End Data Analytics Project | Python • SQL • Power BI  

---

## 🔍 Project Overview

This project presents a **business-driven, end-to-end data analytics solution** designed to mirror the analytical approach expected of a  **Data Analyst**.

The objective is to transform raw customer transaction data into **actionable business insights** that can support:

- Strategic decision-making  
- Customer segmentation  
- Revenue optimization  
- Performance monitoring through dashboards  

The project follows a **structured analytics lifecycle** commonly used in consulting and professional services environments.

---

## 🧠 Business Context & Problem Statement

Organizations often struggle to answer key questions such as:

- Which customers drive the most revenue?
- Which products and regions perform best?
- How does customer behavior change over time?
- Where should management focus growth and optimization efforts?

Using historical customer transaction data, this project aims to:

- Analyze customer purchasing behavior  
- Identify revenue drivers  
- Detect trends and patterns  
- Present insights in a **stakeholder-friendly dashboard**

---

## 🛠️ Tools & Technologies

| Tool | Business Purpose |
|----|----|
| **Python (Pandas, NumPy)** | Data cleaning, transformation, exploratory analysis |
| **SQL** | Structured querying, aggregation, KPI generation |
| **Power BI** | Interactive dashboards & executive reporting |
| **GitHub** | Version control & portfolio presentation |

---

## 📂 Repository Structure

```text
customer-trends-data-analysis/
│
├── data/
│   └── customer_data.csv
│
├── notebooks/
│   └── customer_trends_analysis.ipynb
│
├── sql/
│   └── business_analysis_queries.sql
│
├── powerbi/
│   └── customer_trends_dashboard.pbix
│
└── README.md
```

---

## 🔄 Analytical Approach (Consulting-Style Workflow)

### 1️⃣ Data Understanding & Preparation

* Reviewed dataset structure and business relevance
* Validated data types and consistency
* Removed duplicates and handled missing values
* Created derived business metrics such as **Total Sales**

```python
df['Total_Sales'] = df['Quantity'] * df['Price']
```

### 2️⃣ Exploratory Data Analysis (EDA)

Exploratory analysis focused on business questions, not just visuals:

* Revenue trends over time
* High-value customers
* Product and regional performance
* Purchase frequency patterns

```python
df.groupby('Region')['Total_Sales'].sum().sort_values(ascending=False)
```

### 3️⃣ SQL-Based Business Analysis

The cleaned dataset was queried using SQL to simulate enterprise analytics workflows.

**Key SQL Analyses:**

* Revenue by product category
* Top customers by total spend
* Monthly revenue trends
* Region-wise sales contribution

```sql
SELECT 
    customer_id,
    SUM(total_sales) AS customer_revenue
FROM customer_data
GROUP BY customer_id
ORDER BY customer_revenue DESC
LIMIT 10;
```

### 4️⃣ Power BI Dashboard & Reporting

A management-ready Power BI dashboard was developed to communicate insights clearly and effectively.

**Dashboard Features:**

* **KPIs:** Total Revenue, Total Customers, Average Order Value
* Time-series sales trends
* Category and regional breakdowns
* Top customer identification
* Interactive slicers for dynamic analysis

---

## 📈 Key Insights (Business-Focused)

* **Pareto Effect:** A small subset of customers contributes a significant share of total revenue.
* **Product Performance:** Certain product categories consistently outperform others.
* **Seasonality:** Seasonal trends strongly influence customer purchasing behavior.
* **Growth Zones:** Regional performance varies, indicating targeted growth opportunities.

---

## 💼 Business Impact

The insights generated from this analysis can help organizations:

* Optimize marketing and customer engagement strategies.
* Focus retention efforts on high-value customers.
* Improve inventory and demand planning.
* Strengthen data-driven decision-making at leadership level.

---

## 🚀 How to Run the Project

1. **Clone the repository**
```bash
git clone https://github.com/sgr9/Data_Analysis.git
```

2. **Run the Jupyter Notebook**
   * Navigate to `notebooks/` and open `customer_trends_analysis.ipynb`.

3. **Execute SQL queries**
   * Use the scripts in `sql/` in your preferred SQL environment.

4. **Open the Dashboard**
   * Open the `.pbix` file in Power BI Desktop.

---

## 🎯 Skills Demonstrated 

* Data Cleaning & Validation
* Business-Focused Exploratory Analysis
* SQL for Decision Support
* KPI Development & Reporting
* Data Visualization & Storytelling
* End-to-End Analytics Project Ownership

---

## 🔮 Future Enhancements

* Customer segmentation using clustering (K-Means).
* Predictive sales forecasting.
* Automated ETL and reporting pipeline.

---

## 👤 Author

**Sagar Sharma**  
*Aspiring Data Analyst *  

---

⭐ If you found this project valuable, feel free to star the repository.
