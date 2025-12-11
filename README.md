# E-Commerce Revenue & Retention Analysis
### *End-to-End Data Analytics Project: SQL, Python, Tableau*

[![Tableau Dashboard](https://img.shields.io/badge/Tableau-View_Dashboard-E97627?style=for-the-badge&logo=tableau&logoColor=white)](https://public.tableau.com/app/profile/delia.cangelosi/viz/Dashboardanalisivenditee-commerce_17654686860500/Home)
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)]()
[![SQL](https://img.shields.io/badge/SQL-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)]()

![Dashboard Overview](Images/Dashboard_pag1.jpg)

## Project Overview
This project simulates a real-world Data Analyst scenario for an E-commerce company. The goal was to analyze 12 months of sales data (2023) to identify performance bottlenecks, customer segmentation opportunities, and revenue drivers.

**Key Context:**
* **Duration:** 160-hour Intensive Data Analytics Bootcamp.
* **Role:** Full Stack Data Analyst (Data Engineering, Analysis, Visualization).
* **Tools:** SQL for extraction, Python for ETL & Clustering, Tableau for Dashboarding.

---

## Business Objectives
The management team required a deep dive into the business performance to answer three critical questions:
1.  **Profitability:** Which products and regions are driving actual profit vs. just revenue?
2.  **Retention:** Who are our VIP customers, and how can we segment them?
3.  **Operations:** Why is our return rate impacting margins, and how can we fix it?

---

## 📊 Dashboard Gallery & Key Insights

### 1. High-Level Overview (KPIs & Regional Performance)
* **Goal:** Immediate view of Revenue, Orders, and Average CLV.
* **Insight:** Sales are heavily concentrated in the North region, while the Center lags behind.
![Overview](Images/Dashboard_pag1.jpg)

### 2. Product Profitability & Returns Analysis
* **Goal:** Analyze margins and return rates by category.
* **Discovery:** The **Return Rate is 35.50%**. Products in *Home* and *Electronics* have high revenues but suffer from return rates >50%, severely impacting net profit.
![Product Analysis](Images/Dashboard_pag2.jpg)

### 3. Monthly Trends & Seasonality
* **Goal:** Track performance over time.
* **Insight:** Revenue peaks in May and December, but margins fluctuate significantly due to variable costs and returns.
![Monthly Trends](Images/Dashboard_pag3.jpg)

### 4. Customer Segmentation & Detailed Tables
* **Goal:** Drill-down into customer clusters (Gold, Silver, Bronze) and raw data.
* **Insight:** **Top 20 Customers** generate **60%** of total revenue. Machine Learning (K-Means) identified a cluster of "Whale" clients with basket sizes >€20k.
![Segmentation Details](Images/Dashboard_pag4.jpg)

---

## Technical Approach & Stack

### 1. Data Extraction (SQL)
* Performed complex **JOINs** across 6 relational tables (Orders, Customers, Payments, etc.).
* Used **Window Functions** and Aggregations to calculate monthly revenue and net sales.
* Filtered data to exclude cancelled orders directly at the source.

### 2. Data Processing & Advanced Analysis (Python)
* **ETL:** Data cleaning using `Pandas` and `NumPy`.
* **Feature Engineering:** Calculated Margins, CLV, and Return Rates.
* **Machine Learning:** Applied `Scikit-learn` for **K-Means Clustering** to group customers based on behavior (StandardScaler + Elbow Method).
* **AI Integration:** Leveraged LLMs (Claude/OpenAI) to interpret complex correlation matrices and generate strategic recommendations.

### 3. Visualization (Tableau)
* Built an interactive **4-page Dashboard**.
* Implemented dynamic filters for Region and Category.
* Visualized "Outliers" to highlight anomalous high-value transactions.

---

## 📂 Repository Structure
* `Analisi_Python_E_commerce_database.ipynb`: The main Python notebook containing ETL, EDA, and K-Means Clustering.
* `Analisi_preliminare_sql_e-commerce_database.ipynb`: SQL scripts used for data extraction and initial validation.
* `Dashboard_pag1.jpg` to `Dashboard_pag4.jpg`: Dashboard screenshots.

---

## 👥 The Team
This project was developed in collaboration with:
* **[Cangelosi Delia]** - *[www.linkedin.com/in/delia-cangelosi-6731a6301]*
* [Attino Alessandro]
* [Labile Vittoria ]
* [Facchini chiara]
* [Pashaei Kuchesfahani Nastaran]

---

### 🔗 [Click here to explore the Interactive Dashboard on Tableau Public](https://public.tableau.com/app/profile/delia.cangelosi/viz/Dashboardanalisivenditee-commerce_17654686860500/Home)