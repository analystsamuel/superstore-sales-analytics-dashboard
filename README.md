# Global Superstore Sales & Customer Performance Dashboard

## Project Overview
An application-style enterprise retail analytics dashboard built in Power BI to optimize sales tracking, profitability analysis, and customer segmentation. This multi-page dashboard shifts raw transactional data into interactive, executive-ready insights designed to maximize profit margins and identify high-value consumer groups.

## Tech Stack
* **Data Visualization & Business Intelligence:** Power BI (DAX, Data Modeling, Multi-Page UX Navigation)
* **Data Engineering & Preprocessing:** SQL (Duplicate removal, data cleaning)

## Dashboard Architecture & Key Metrics

### 1. Executive Overview (Home Page)
Designed with a premium dark theme utilizing floating containers to isolate core enterprise-level KPIs:
* **Total Revenue:** $2.29M
* **Total Profit:** $286.41K
* **Fulfillment Volume:** 9,993 Total Orders
* **Key Visuals:** A synchronized Sales & Profit Trend timeline, category income analysis (highlighting Technology as the primary profit driver), and a geographical Income Distribution map tracking US performance.

### 2. Sales Performance Deep-Dive
A specialized operational view focusing on product lines, margins, and volume metrics:
* **Total Quantity Sold:** 37,871 items
* **Blended Profit Margin:** 12.47%
* **Key Visuals:** A "Top 10 Sold Products" horizontal bar chart identifying Phones ($330K) and Chairs ($328K) as core revenue generators, paired with a categorical breakdown revealing Technology controls 36.4% of total sales distribution.

### 3. Customer Insights & Segmentation
An analytical view dedicated to understanding purchasing patterns across client profiles:
* **Active Customer Base:** 793 Unique Customers
* **Average Customer Lifetime Value (Sales):** $2,896.49
* **Key Visuals:** High-value acquisition matrix tracking top individual clients (e.g., Christopher Conant and Sanjit Engle), complemented by corporate segment distribution charts showing the "Consumer" bracket drives 51.95% of total engagement.

## Data Preparation & Cleaning (SQL)
To safeguard data integrity before importing models into Power BI, the underlying dataset underwent extensive cleaning via SQL:
* Executed advanced duplicate removal scripts to ensure transaction counts were unskewed.
* Cleaned and standardized data fields to ensure strict tracking and data integrity.
