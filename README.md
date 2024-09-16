

---

## Instructions

### 1. Initial Setup

- **Import Required Libraries:**
  - Import the necessary PySpark SQL functions for the assignment.
  
- **Load Data:**
  - Read the `home_sales_revised.csv` file into a Spark DataFrame.
  
- **Create Temporary Table:**
  - Create a temporary table named `home_sales` from the DataFrame.

### 2. Data Analysis Using SparkSQL

- **Query 1:**
  - Calculate the average price for four-bedroom houses sold each year. Round your results to two decimal places.
  
- **Query 2:**
  - Determine the average price of homes built each year that have three bedrooms and three bathrooms. Round your results to two decimal places.
  
- **Query 3:**
  - Find the average price of homes for each year that have three bedrooms, three bathrooms, two floors, and a living area of 2,000 square feet or more. Round your results to two decimal places.
  
- **Query 4:**
  - Identify the "view" rating for homes priced at $350,000 or more. Measure the runtime for this query, rounding the runtime to two decimal places.

### 3. Performance Optimization

- **Cache Data:**
  - Cache the `home_sales` temporary table.
  
- **Verify Caching:**
  - Confirm that the `home_sales` table is cached.
  
- **Run Cached Query:**
  - Using the cached data, run the query that filters for view ratings with an average price of $350,000 or more. Measure and compare the runtime to the uncached version.

### 4. Data Partitioning and Further Optimization

- **Partition Data:**
  - Partition the parquet home sales data by the `date_built` field.
  
- **Create Temporary Table:**
  - Create a temporary table from the partitioned parquet data.
  
- **Run Partitioned Query:**
  - Execute the query that filters for view ratings with an average price of $350,000 or more. Measure the runtime and compare it to the uncached version.

### 5. Clean Up

- **Uncache Data:**
  - Uncache the `home_sales` temporary table.
  
- **Verify Uncaching:**
  - Ensure that the `home_sales` temporary table is no longer cached using PySpark.

---

