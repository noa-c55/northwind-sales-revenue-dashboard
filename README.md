# northwind-sales-revenue-dashboard
End-to-end sales & revenue analysis using Power BI, built on a dbt-modeled analytics layer (Northwind dataset). Focused on business insights, revenue drivers, and performance trends.
## Data & Modeling
The dashboard is built on top of a dbt-modeled analytics layer based on the Northwind dataset.
The data model follows a star schema approach.

Fact tables capture order-level and line-item sales data, including revenue calculations and quantities,
while dimension tables provide descriptive context for employees, products, categories, customers, and shippers.
All business logic, transformations, and aggregations are implemented upstream in dbt.

## Dashboard Highlights
- Revenue trends over time with interactive date filtering
- Top revenue-contributing employees and their share of total revenue
- Key product categories driving the majority of sales
- Geographic revenue concentration by city to identify major markets

## Key Insights
- Revenue is highly concentrated among a small group of employees
- A limited number of product categories account for a significant portion of total revenue
- Revenue peaks in 2014, followed by a decline in the following period
- Sales activity is concentrated in specific geographic regions

## Notes on the Data
The data available for the final year is partial, which should be considered when interpreting
revenue trends toward the end of the timeline.

## How to Use
Download and open the `.pbix` file using Power BI Desktop to explore the dashboard,
interact with filters, and drill down into the analysis.

## Data Modeling (dbt)

The analytical layer powering this dashboard was built using dbt, following analytics engineering best practices.
It includes a star schema with well-defined fact and dimension tables, data quality tests, and reusable business logic.

🔗 dbt project repository:  
https://github.com/noa-c55/proj_northwind_dbt
