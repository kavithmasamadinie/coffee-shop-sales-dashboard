# ☕ coffee-shop-sales-dashboard

## 📌 Project Overview
This project is an end-to-end data engineering and business intelligence solution designed for a retail coffee shop chain. Instead of relying on static flat files, this project simulates a real-world enterprise environment by provisioning a live cloud database, transforming raw data via SQL, and connecting it securely to Power BI to deliver actionable insights.

The final deliverable is an interactive, two-page Power BI dashboard that empowers stakeholders to optimize staff scheduling, analyze location-based revenue, and manage inventory effectively.

## 🛠️ Tech Stack
* **Cloud Database:** PostgreSQL (Hosted via Aiven Cloud)
* **Database Management:** DBeaver
* **Query Language:** SQL (DDL & Aggregation)
* **Business Intelligence:** Power BI
* **Data Modeling:** DAX (Data Analysis Expressions)

## 🏗️ Architecture & Pipeline Steps

### 1. Cloud Database Provisioning
* Deployed a secure PostgreSQL database on Aiven Cloud.
* Ingested over 149,000 rows of raw retail transaction data into the cloud server.

### 2. Data Transformation (SQL)
* Connected to the live database using DBeaver via SSL encryption.
* Executed SQL Data Definition Language (DDL) commands to clean the schema.
* Converted raw text fields into proper `DATE` and `TIME` data types for accurate time-series analysis.

### 3. Business Intelligence Integration
* Established a direct, encrypted connection between Power BI Desktop and the Aiven PostgreSQL server.
* Wrote custom DAX measures to calculate dynamic Key Performance Indicators (KPIs), including Total Revenue, Average Order Value, and Total Items Sold.
* Extracted the `Hour` from timestamp data using DAX to enable peak-hour operational analysis.

### 4. Dashboard UI/UX Design
Designed a professional, two-page interactive report using a custom, high-contrast color palette (Espresso, Cream, and Caramel):
* **Page 1: Executive Overview:** High-level KPIs, location filtering, and a peak-hours trend analysis to drive staffing decisions.
* **Page 2: Store Deep-Dive:** A granular matrix breakdown of category performance and a Top-10 Best-Selling Items chart utilizing advanced Top-N filtering.

## 💡 Key Business Insights Generated
1. **Operational Efficiency:** Identified exact peak traffic hours (e.g., 8:00 AM - 10:00 AM), allowing for data-driven barista shift scheduling.
2. **Location Performance:** Visualized revenue distribution across three prime locations (Astoria, Hell's Kitchen, Lower Manhattan) to assess store health.
3. **Inventory Optimization:** Highlighted the top 10 highest-grossing menu items, enabling better supply chain and ordering decisions.

## 👨‍💻 Author
**Kavithma Samarawickrama**
* ASspring Data Analyst &  Data Engineer
* [Connect with me on LinkedIn](#) *(Add your LinkedIn link here)*
