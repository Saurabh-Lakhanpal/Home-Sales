# Home Sales Analysis with SparkSQL

This project explores home sales data using SparkSQL to determine key housing market metrics. By leveraging Spark's powerful capabilities, we analyze pricing trends, optimize queries, and enhance performance through caching and partitioning techniques.

[Solution - Collab](https://github.com/Saurabh-Lakhanpal/Home-Sales/blob/main/Home_Sales.ipynb)

## Data Processing

The dataset, `home_sales_revised.csv`, is loaded into a PySpark DataFrame and transformed into a temporary table called `home_sales`. SparkSQL is used to extract meaningful insights from the data, answering key questions regarding price trends, square footage, and view ratings.

## Analytical Focus

Key analyses performed in this project include:
- Determining the **average price of four-bedroom houses** sold per year.
- Evaluating the **average price of homes** built per year with three bedrooms and three bathrooms.
- Assessing pricing trends for **homes with three bedrooms, three bathrooms, two floors, and ≥2,000 sq ft**.
- Calculating the **average price per "view" rating** for homes priced at $350,000 or higher.
- Measuring query execution times and comparing performance optimization techniques.

## Performance Optimization

To enhance efficiency, caching mechanisms are implemented to store query results in memory. The impact of caching on execution time is compared against uncached queries. Additionally, data is partitioned by `date_built`, and a temporary table is created for the partitioned parquet dataset to further evaluate query performance.
