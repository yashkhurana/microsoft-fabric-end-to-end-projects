# Project 1 - Sales_Analytics ( Lakehouse Set Up)

# Objective

Build an end to end analytics solution using Microsoft Fabric starting with Lakehouse Ingestion.

# Architecture

CSV → Lakehouse → Transformation → Reporting

# Tools Used

- Microsoft Fabric
- Lakehouse
- Delta Table

# Dataset

Sales transaction dataset containing order details, price and region.

# Steps Performed:

1. Created Fabric Workspace
2. Created Lakehouse
3. Uploaded Raw CSV Data
4. Loaded Into Delta Table

# Screenshots

1. Created Lakehouse

![Lakehouse](screenshots/lakehouse-overview.png)

2. Lakehouse Table

![Lakehouse](screenshots/lakehouse-table.png)

3. SQL Analytics Endpoint

![Lakehouse](screenshots/sql-analytics-endpoint.png)

4. Data Transformation ( Notebooks )
   - Removed invalid quantity
   - Removed null prices
   - Added revenue column

5. Raw data preview

   - ![Raw](screenshots/raw-data-preview.png)
  
6. Added revenue column

   - ![Raw](screenshots/added_revenue_column.png)
  
7. Cleaned Data Preview

   - ![Raw](screenshots/cleaned-data-preview.png)
  
8. Sales_Clean Table

   - ![Raw](screenshots/Sales_clean.png)

9. Gold Layer ( Aggregated Sales Summary )

   - Created region wise revenue summary using Pyspark groupby and aggregation.
  
   ### Spark Aggregation

   - ![Spark](screenshots/spark-groupby-output.png)
  
   - ![Spark](screenshots/save_sales_summary.png)
  
   - ![Spark](screenshots/sql-query-result.png)





