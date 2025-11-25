# end-to-end-sql-powerbi-analytics-project
 ETL |  Medallion Architecture |  SQL Server |  Power BI |  DAX |  Data Modeling

---

# 🚀 **Welcome to End-to-End SQL + Power BI Analytics Project**

This project demonstrates a full modern analytics solution starting from raw CSV files to a production-ready data warehouse and a fully interactive Power BI dashboard for **customer, product, RFM, and cohort analysis**.

It showcases:

✔ Data engineering (ETL) using SQL Server
✔ Data warehousing using Medallion Architecture (Bronze → Silver → Gold)
✔ Dimensional modeling (facts & dimensions)
✔ Data quality corrections and business logic implementation
✔ Advanced Power BI modeling and DAX
✔ Customer analytics, Product analytics, RFM segmentation, Cohort retention analysis

---

# 🏗️ **Data Warehouse Architecture (Bronze → Silver → Gold)**

This project follows the **Medallion Architecture** to create a scalable, analytics-ready warehouse.

---

## 🥉 **Bronze Layer — Raw Ingestion**

The Bronze layer stores raw CRM, ERP, and sales files exactly as received.

### **Purpose**

* Preserve raw data
* Maintain source-of-truth
* Act as input for all transformations

### **Key Actions**

* No transformations
* No standardization
* Bulk-loaded using `BULK INSERT`

---

## 🥈 **Silver Layer — Clean / Standardized Zone**

The Silver Layer applies data cleaning and business standardization:

### **What Happens in Silver**

✔ Deduplication
✔ Data type corrections
✔ Date parsing
✔ Product-line normalization
✔ Customer gender/marital standardization
✔ Missing value imputation
✔ Sales recalculation rules

The result: **clean, validated, business-ready staging tables**.

---

## 🥇 **Gold Layer — Analytics / Semantic Zone**

The Gold Layer builds **analytical models** and prepares everything for BI.

### ⭐ **What Gold Layer Adds**

* Recency
* Customer lifespan
* Average monthly spend
* Product profitability metrics
* RFM scoring
* Cohort month & lifecycle metrics

This layer delivers a **fully optimized star-schema** for Power BI consumption.

---

# 📊 **Power BI Dashboards**

The final Power BI report contains **4 main analysis modules**:

---

### **1️⃣ Overview Dashboard**

Shows company-wide KPIs and customer-level trends:

* Revenue
* Profit
* Orders
* Customer count
* AOV
* Category/segment distributions
* Monthly/Yearly performance trends

---

### **2️⃣ Product Performance Dashboard**

Includes:

* Product lifecycle (Active / At-Risk / Dormant)
* Price tier profit distribution
* Category performance
* High vs Low performer segmentation
* Profit–Orders–Quantity scatter
* Top & Bottom 5 products

---

### **3️⃣ RFM Customer Segmentation Dashboard**

Behavior-based customer segmentation:

* Recency scores
* Frequency scores
* Monetary scores
* RFM segment distribution
* RFM impact on revenue
* Customer behavior clustering

---

### **4️⃣ Cohort Analysis Dashboard**

Customer retention analysis:

* First purchase cohort grouping
* Month-over-month retention
* Long-term customer activity decay
* Cohort performance comparison

---

# ❓ **Business Questions Answered**

### **🛒 Customer Behavior**

* Who are our most valuable customers?
* Which customers are becoming inactive?
* What are spending patterns across RFM groups?

### **📦 Product Insights**

* Which products generate the most profit?
* Which products are declining or dormant?
* Which categories produce long-term value?

### **📈 Performance Trends**

* How are revenue, profit, orders growing over time?
* What seasons/days show highest activity?

### **🔁 Retention**

* How long do customers stay active?
* Which cohorts are strongest or weakest?

---

# 🚀 **Skills Demonstrated**

* **SQL Data Warehousing (Bronze/Silver/Gold)**
* **Dimensional & Star Schema Modeling**
* **ETL Development (Stored Procedures, Bulk Insert)**
* **Business Logic Transformation**
* **RFM & Cohort Analysis (DAX)**
* **Power BI Modeling & Storytelling**
* **Performance Optimization (Indexing & Views)**

This project is designed as a **professional BI/Analytics portfolio** showcasing real-world analytical engineering capabilities.

---






