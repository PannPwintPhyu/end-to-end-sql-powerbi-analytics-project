# 🚀 **End-to-End SQL + Power BI Analytics Project**

**ETL | Medallion Architecture | SQL Server | Power BI | DAX**

---

# 🔗 **Live Power BI Dashboard**

 **Click to View Interactive Report**
**[https://app.powerbi.com/view?r=eyJrIjoiNGQ4NjY1MTAtZjg2MS00MjA5LWFkMDctMDE4Nzg0MmZiZDdiIiwidCI6IjhlZjRhZjJkLTkwY2YtNGIzMS1hMTI4LTNmYWE5M2EzMmJjOCIsImMiOjEwfQ%3D%3D](https://app.powerbi.com/view?r=eyJrIjoiNGQ4NjY1MTAtZjg2MS00MjA5LWFkMDctMDE4Nzg0MmZiZDdiIiwidCI6IjhlZjRhZjJkLTkwY2YtNGIzMS1hMTI4LTNmYWE5M2EzMmJjOCIsImMiOjEwfQ%3D%3D)**

---

#  **Dashboard Preview**

<table>
<tr>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/1_Overview.png?raw=true" width="300"></td>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/2_ProductAnalysis.png?raw=true" width="300"></td>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/3_ProductDetails.png?raw=true" width="300"></td>
</tr>

<tr>
<td align="center"><b>Overview Dashboard</b></td>
<td align="center"><b>Product Analysis</b></td>
<td align="center"><b>Product Details</b></td>
</tr>

<tr>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/4_RFMAnalysis.png?raw=true" width="300"></td>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/5_CustomerRecords.png?raw=true" width="300"></td>
<td><img src="https://github.com/PannPwintPhyu/end-to-end-sql-powerbi-analytics-project/blob/main/assets/6_Cohort.png?raw=true" width="300"></td>
</tr>

<tr>
<td align="center"><b>RFM Analysis</b></td>
<td align="center"><b>Customer Records</b></td>
<td align="center"><b>Cohort Analysis</b></td>
</tr>
</table>

---

#  **Project Overview**

This project demonstrates a full modern analytics solution starting from raw CSV files to a production-ready data warehouse and a fully interactive Power BI dashboard for **customer, product, RFM, and cohort analysis**.

It showcases:

✔ Data engineering (ETL) using SQL Server                                                                                      
✔ Data warehousing using Medallion Architecture (Bronze → Silver → Gold)                                                                          
✔ Dimensional modeling (facts & dimensions)                                                                                          
✔ Data quality corrections and business logic implementation                                                                                      
✔ Advanced Power BI modeling and DAX                                                                                        
✔ Customer analytics, Product analytics, RFM segmentation, Cohort retention analysis                                                                              

---

#  **Data Warehouse Architecture (Bronze → Silver → Gold)**

This project follows the modern **Medallion Architecture** to create a scalable, analytics-ready warehouse.

---

##  **Bronze Layer - Raw Ingestion**

The Bronze layer stores raw CRM, ERP, and sales files exactly as received.

### **Purpose**

* Preserve raw data
* Maintain source-of-truth
* Act as input for all transformations

### **Key Actions**

* No transformations
* No standardization
* Loaded using `BULK INSERT`

---

##  **Silver Layer - Clean / Standardized Zone**

The Silver Layer applies business cleaning and data standardization:

✔ Deduplication                                                                                        
✔ Data type corrections                                                                                          
✔ Date parsing                                                                                                          
✔ Product-line normalization                                                                                          
✔ Customer gender/marital standardization                                                                            
✔ Missing value imputation                                                                                            
✔ Sales recalculation rules                                                                                                  

The result: **clean, validated, business-ready staging tables**.

---

##  **Gold Layer - Analytics / Semantic Zone**

The Gold Layer builds **analytics-ready dimensional models** for BI consumption.

* Recency
* Customer lifespan
* Average monthly spend
* Product profitability metrics
* RFM scoring
* Cohort month & lifecycle metrics

This layer delivers a **fully optimized star schema** for Power BI.

---

#  **Power BI Dashboards**

The final Power BI report contains **4 major analytical modules**:

---

### **1. Overview Dashboard**

* Revenue
* Profit
* Orders
* Customer count
* AOV
* Category/segment distributions
* Monthly/Yearly performance trends

---

### **2. Product Performance Dashboard**

* Product lifecycle (Active / At-Risk / Dormant)
* Price tier profit distribution
* Category performance
* High vs Low performer segmentation
* Profit–Orders–Quantity scatter
* Top & Bottom 5 products

---

### **3. RFM Customer Segmentation Dashboard**

* Recency scores
* Frequency scores
* Monetary scores
* RFM segment distribution
* RFM impact on revenue
* Customer behavior clustering

---

### **4. Cohort Analysis Dashboard**

* First purchase cohort grouping
* Month-over-month retention
* Long-term activity patterns
* Cohort performance comparison

---

# ❓ **Business Questions Answered**

###  **Customer Behavior**

* Who are our most valuable customers?
* Which customers are becoming inactive?
* What are spending patterns across RFM groups?

###  **Product Insights**

* Which products generate the most profit?
* Which products are declining or dormant?
* Which categories deliver long-term value?

###  **Performance Trends**

* How are revenue, profit, orders growing over time?
* What seasons/days show highest activity?

###  **Retention**

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

This project is designed as a professional **BI/Analytics portfolio** showcasing real-world analytical engineering capabilities.

---

# 📌 **Key Insights & Business Recommendations**

### 🔹 **1. Strengthen Early Customer Engagement**

Cohort retention drops sharply after Month 2–3.                                                                                          
**Recommendation:**
Introduce onboarding campaigns, reminder notifications, and early-purchase incentives to improve early lifecycle retention.

---

### 🔹 **2. Prioritize High-Value Customer Segments (Champions & Loyal)**

RFM analysis shows these customers generate the majority of revenue.                                                                                                        
**Recommendation:**
Create premium loyalty benefits, targeted promotions, and exclusive offers to maintain long-term value.

---

### 🔹 **3. Reactivate At-Risk & Hibernating Customers**

These groups represent lost revenue opportunities.
**Recommendation:**
Launch reactivation campaigns—discount reminders, personalized product recommendations, and seasonal offers.                                                  

---

### 🔹 **4. Optimize Product Portfolio**

Top performer products generate dominant profit while dormant products show declining trends.                                                          
**Recommendation:**
Increase stock & marketing for high performers; reprice, bundle, or retire underperforming SKUs.

---

### 🔹 **5. Leverage High-Profit Price Segments**

Exclusive/Signature tiers produce the highest profit contribution.                                                                    
**Recommendation:**
Focus upselling strategies to move mid-tier customers into premium product lines.

---

### 🔹 **6. Expand Customer Value Through Upsell/Cross-Sell**

Large number of customers fall under low Monetary score groups.                                                      
**Recommendation:**
Offer product bundles, personalized recommendations, and frequency-based discounts.

---

### 🔹 **7. Monitor Long-Term Retention Trends**

Cohort patterns show acquisition quality shifts over time.                                                                        
**Recommendation:**
Use Cohort page regularly to evaluate marketing effectiveness and customer loyalty patterns.

---

