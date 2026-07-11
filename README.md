# Superstore Data Project: From Raw Data to Power BI Dashboard

This project demonstrates an end-to-end analytics workflow. I took a messy, raw retail dataset, cleaned and staged it using SQL, and built a high-end, multi-page Power BI dashboard to track executive metrics.

## The Files in This Repo
* `Sample - Superstore.csv` - Raw, uncleaned source data with duplicates and formatting issues.
* `susuperstore_staging.csv` - Cleaned, deduplicated data exported from my SQL staging environment.
* `Superstore Dashboard.pbix` - Final Power BI file with the live data model and interactive visuals.
* `S.Home.png`, `S.Sales.png`, `S.Customers.png` - Screenshots of the dashboard pages.

## The Project Flow

### 1. Data Cleaning (SQL)
The raw dataset (`Sample - Superstore.csv`) had several data integrity issues that would distort business metrics if left unchecked. I imported it into SQL and performed the following cleaning steps:
* **Removed Duplicates:** Dropped redundant rows to ensure transaction and order counts were completely accurate.
* **Standardized Text:** Cleaned up geographical data fields (State and City) to fix casing and naming errors.
* **Handled Blanks:** Cleaned missing values in shipping and fulfillment columns to keep logistics tracking accurate.
* **Exported Staging Layer:** Saved the clean output as `susuperstore_staging.csv` as the clean source of truth for reporting.

### 2. Dashboard Architecture & Metrics
I loaded the clean staging data into Power BI and built a dark-themed dashboard using custom floating containers for a clean, application-style UI.

#### Page 1: Overview (`S.Home.png`)
Tracks high-level company health:
* **Total Revenue:** $2.29M | **Total Profit:** $286.41K | **Total Orders:** 9,993
* **Key Visuals:** A combined Sales & Profit trend line over time, a breakdown showing Technology as the top profit category, and a map showing regional income distribution.

#### Page 2: Sales Performance (`S.Sales.png`)
Deep dive into product and margin performance:
* **Total Quantity Sold:** 37,871 items | **Profit Margin:** 12.47%
* **Key Visuals:** A Top 10 products chart identifying Phones and Chairs as top revenue drivers, and a breakdown of sales share by product category.

#### Page 3: Customer Insights (`S.Customers.png`)
Analyzes customer purchasing behavior:
* **Unique Customers:** 793 | **Avg Sales Per Customer:** $2,896.49
* **Key Visuals:** A leaderboard tracking top-spending clients, and a chart showing that the "Consumer" segment makes up 51.95% of the business.
