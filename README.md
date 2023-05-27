# Home_Sales
![image](https://github.com/diego-lazaro/Home_Sales/assets/115186079/ecaec539-a227-4c44-95a6-7556980273ab)

# Synopsis

The purpose of this analysis is to determine key metrics about home sale data. Utilized PySpark and SparkSQL to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

# Data Preperation
* Create a temporary table
* Cache a temporary table and check if it is cached
* Run the query that filters out the view ratings with an average price of greater than or equal to $350,000 then determine the runtime and compare it to uncached runtime.
* Partition by the "date_built" field on the formatted parquet home sales data.
* Create a temporary table for the parquet data.
* Run the query that filters out the view ratings with an average price of greater than or equal to $350,000 then determine the runtime and compare it to uncached runtime.
* Uncache the temporary table.
* Verify that the temporary table is uncached using PySpark

# Conclusion
The runtime for the cached data took less time to run than the parquet data. Both the parquett and the cached data took less time to run than the uncached data. Overall, a cached data should be used to for a larger dataset because it was the fastest which will save time. 
