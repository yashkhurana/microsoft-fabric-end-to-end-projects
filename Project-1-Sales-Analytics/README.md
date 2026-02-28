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

10. Read Sales Clean Table

   - ![Spark](screenshots/read_sales_clean_table.png)

11. Created Product Wise Revenue Table

    - ![Spark](screenshots/product_revenue.png)
   
12. Created Categort Wise Revenue Table

    - ![Spark](screenshots/category_revenue.png)

13. Created Monthly Revenue Table

    - ![Spark](screenshots/Monthly_revenue.png)

14. Created Category Profit Table

    - ![Spark](screenshots/category_profit.png)

15. Save Category Profit Table

    - ![Spark](screenshots/save_category_profit.png)



# Now we will create Gold Layer ( Star Schema ) with the help of Spark SQL in notebook

We will create the following tables in gold layer:-
1) dim_date
2) dim_product
3) dim_region
4) fact_sales

We will follow the below steps:-

1) dim_product table

   - ![Spark](screenshots/dim_product.png)

2) dim_region

    - ![Spark](screenshots/dim_region.png)
  
3) dim_date

    - ![Spark](screenshots/dim_date.png)
  
4) fact_sales

   - ![Spark](screenshots/fact_sales.png)


  
