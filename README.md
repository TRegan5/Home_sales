## Module 22 Challenge
# Home_sales
Repository for this challenge found at: https://github.com/TRegan5/Home_sales

Coding done using Google Colab

In this challenge, I used SparkSQL to determine key metrics about provided home sales data. I created temporary views, partitioned the data, cached and uncached a temporary table, and finally verified the uncaching of that table. 

1. Created Spark DataFrame from the dataset
2. Created temporary table of the original DataFrame
3. Queried temporary table for average price (rounded to two decimal places) for four-bedroom houses sold each year
4. Queried temporary table for average price (rounded to two decimal places) for three bedroom and three bathroom homes built each year
5. Queried average price (rounded to two decimal places) of homes with three bedrooms, three bathrooms, two floors, and square footage greater than or equal to 2,000, built each year
6. Queried average price of homes (rounded to two decimal places) per "view" rating having an average home price greater than or equal to $350,000, with output showing query run time
7. Cached temporary "home_sales" table validated creation
8. Reran query from step 6 is run on cached temporary table, again computing run time
9. Created partition of home sales dataset by "date_built" field and read formatted parquet data
10. Created temporary table of the parquet data
11. Reran query from step 6 on parquet temporary table, again computing run time
12. Uncached and verified removal of "home_sales" temporary table