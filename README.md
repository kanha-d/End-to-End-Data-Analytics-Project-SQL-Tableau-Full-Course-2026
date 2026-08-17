# 📊 End-to-End E-Commerce Data Analytics Project (SQL & Tableau)

## 📝 Project Overview
This project focuses on evaluating e-commerce sales performance and customer behavior. The goal of this analysis is to identify key sales trends, customer segmentation, and product performance using SQL for data extraction and cleaning, followed by Tableau for interactive data visualization. 

**View the Live Interactive Dashboard:** https://public.tableau.com/views/WalMartSalesDashboard/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## 🎯 Business Problem & Objective
The management team needed a way to track Key Performance Indicators (KPIs) regarding sales, profit, and customer retention. 

**Objectives:**
1. Clean and format raw sales data for analysis.
2. Identify the highest-grossing product categories and seasonal sales trends.
3. Determine customer purchase frequency and segment high-value customers.
4. Build an interactive dashboard for stakeholders to filter data dynamically by year, region, and product type.

## 🛠️ Tools & Technologies Used
* **SQL (MySQL / PostgreSQL / SQL Server):** Used for Data Cleaning, Exploratory Data Analysis (EDA), Aggregations, Window Functions, and CTEs.
* **Tableau:** Used for connecting the database, creating calculated fields, and building an interactive dashboard layout.
* **Excel / CSV:** Initial raw dataset formats before database importing.

## 🗂️ Data Preparation & SQL Exploration
The raw data contained inconsistencies, null values, and formatting errors. I used SQL to clean the data and perform exploratory analysis. 

**Key SQL Skills Demonstrated:**
* Creating tables and importing data constraints.
* Handling Null values and duplicate records.
* Using `JOIN` to combine Customer and Sales tables.
* Utilizing `CTE`s (Common Table Expressions) and `Window Functions` (e.g., `RANK()`, `PARTITION BY`) to find top-selling items per region.
* Date manipulation (`EXTRACT`, `DATE_TRUNC`) for time-series forecasting.

*(You can view the full SQL script in the `sql_queries.sql` file in this repository).*

## 📈 Tableau Dashboard Development
After exporting the cleaned datasets from SQL, I connected them to Tableau to build out visual representations of the data. 

**Key Dashboard Features:**
* **Executive KPI Banner:** Total Revenue, Total Profit, and Profit Margin percentage.
* **Time-Series Area Chart:** Showing month-over-month sales growth.
* **Geographical Map:** Heatmap of sales distribution across different states/regions.
* **Interactive Filters:** Allows the end-user to slice data by Year, Customer Segment, and Product Category.

## 💡 Key Insights & Recommendations
1. **Seasonal Spikes:** Revenue consistently spikes in Q4, specifically in November and December. **Recommendation:** Increase marketing spend and inventory stock by mid-October.
2. **Underperforming Regions:** The Southern region has a high volume of sales but the lowest profit margins due to extreme discounting. **Recommendation:** Restrict discount usage in this region to improve profitability.
3. **Customer Retention:** 20% of customers account for over 60% of total revenue. **Recommendation:** Implement a targeted loyalty program for these high-value clients.

## 🚀 How to Run This Project
1. Clone this repository to your local machine.
2. Open your preferred SQL client (e.g., MySQL Workbench, pgAdmin) and run the `schema_setup.sql` script to create the database.
3. Import the `raw_dataset.csv` file into the newly created tables.
4. Run the queries in the `analysis_queries.sql` file to view the data manipulation steps.
5. Open the `Sales_Dashboard.twbx` file in Tableau Desktop to interact with the visualizations.
