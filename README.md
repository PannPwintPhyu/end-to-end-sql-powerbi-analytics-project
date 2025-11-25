# end-to-end-sql-powerbi-analytics-project
 ETL |  Medallion Architecture |  SQL Server |  Power BI |  DAX |  Data Modeling

This project delivers a complete end-to-end data analytics solution, starting from raw CSV files and ending in a fully interactive Power BI dashboard.
It demonstrates skills in data warehousing, analytics modeling, and BI visualization.

🗂️ 1. Architecture Overview
🔷 Medallion Architecture (Bronze → Silver → Gold)

This solution follows the modern Medallion Architecture to build a scalable data warehouse:

Bronze Layer — Raw Zone

Direct ingestion of CRM & ERP source files

No business rules applied

Loaded using BULK INSERT

Silver Layer — Cleaned Zone

Standardization & business logic applied

Data validation, deduplication, and type corrections

Transformation of product lines, gender, marital status

Fixing missing/invalid dates, recalculating sales fields

Gold Layer — Analytics Zone

Final analytical models prepared for reporting

Dimensional modeling (facts + dimensions)

Creation of surrogate keys & time-based metrics

Pre-aggregation for customer & product reporting

Business-ready attributes such as:
✔ Recency
✔ Customer lifespan
✔ Average monthly spend
✔ Product profitability metrics
✔ RFM (Recency-Frequency-Monetary) scoring
✔ Cohort tagging for retention analysis

The Gold Layer provides a consistent, optimized semantic layer for BI tools.

🥉 2. Bronze Layer (Raw Ingestion)

The Bronze layer stores raw transactional and master data from CRM and ERP sources:

No filtering

No data quality rules

Structure matches source fields

Loaded using automated SQL stored procedures

This ensures full traceability and supports reproducible ETL.

🥈 3. Silver Layer (Cleansed / Standardized Zone)

The Silver layer applies business transformations such as:

Removing duplicate customer records

Converting numeric dates to proper DATE format

Normalizing categorical values (gender, marital status, product line)

Recalculating sales values when incorrect

Ensuring referential integrity

Aligning field naming & formats

Generating cleansing audit timestamps

By the end of the Silver stage, the dataset is clean, standardized, and business-ready.

🥇 4. Gold Layer (Analytics / Semantic Zone)

The Gold Layer transforms cleaned data into analytics-ready models, enabling high-performance BI reporting.

Key capabilities implemented:

✔ Dimensional Modeling (Star Schema)

Creation of customer, product, and date dimensions

Fact table for sales transactions

Conformed keys and optimized relationships

✔ Analytical Enhancements

Customer behavioral attributes

Product lifecycle and performance tagging

Normalized financial measures

Time-aware metrics (recency, lifespan, cohorts)

✔ Pre-Aggregated Business Views

Customer activity summary

Product performance summary

Recency, frequency, monetary scores

Cohort retention view

Price segmentation and profitability classes

✔ Optimization for BI Consumption

Column trimming

Indexing

Business-friendly naming

View-based semantic layer for Power BI

The Gold Layer is the foundation for all reporting and analytics.

📊 5. Power BI Dashboards

The final dashboard includes 4 major analytical modules, each built with advanced DAX and structured storytelling.

1️⃣ Performance Overview Dashboard

Revenue, Profit, Orders, Customer KPIs

Trend analysis

Category performance

Customer distribution

Dynamic YoY calculations

Interactive date filtering

2️⃣ Product Analytics Dashboard

Product lifecycle (Active / At-Risk / Dormant)

Price tier profitability

Category-level performance

High vs Low performer analysis

Profit vs Orders scatter (Quantity as bubble size)

Top & bottom product comparison

3️⃣ RFM Customer Segmentation Dashboard

Behavioral segmentation using Recency, Frequency & Monetary

Segment distribution (Champions, Loyal, At-Risk, Hibernating…)

R/F/M score heatmaps

Customer value comparison

Bubble relationship analysis

4️⃣ Cohort Retention Dashboard

First purchase month grouping

Month-over-month retention behavior

Lifecycle decay patterns

Comparison across cohorts

Insights into acquisition quality and retention strategy

🧠 6. Key Insights Generated
Customer Insights

VIP & Loyal customers contribute the majority of revenue

Large share of At-Risk customers → retention opportunity

High R-Score customers show strong recent engagement

Product Insights

Exclusive tier products generate the highest profit

Clear 80/20 rule: minority of SKUs produce majority of value

Dormant products require marketing or pricing intervention

Cohort Insights

Strongest retention occurs in first ~3 months

Long-term retention stabilizes between 3–5%

Acquisition quality differs by period

🧩 7. Skills Demonstrated
🔧 Data Engineering

Advanced SQL ETL

Stored procedures

Bulk loading

Data quality validation

Transformation logic

Indexing and optimization

📦 Data Warehousing

Medallion architecture

Dimensional modeling (Star Schema)

Fact & dimension design

Surrogate keys

Analytical feature engineering

📊 Business Intelligence

DAX measures & modeling

KPI design

RFM segmentation

Cohort retention modeling

Data storytelling

Interactive dashboards
