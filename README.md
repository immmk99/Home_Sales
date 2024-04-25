# Home_Sales
 


 This project utilized PySpark to perform a comprehensive analysis of home sales data. The goal was to uncover trends in home prices based on various characteristics such as the number of bedrooms, bathrooms, floors, and view ratings.


- **Data Analysis Using SparkSQL**
  - Executed multiple SparkSQL queries to extract insights from the data:
    - Calculated the average price of four-bedroom homes sold each year.
    - Determined the average price of homes each year for properties with three bedrooms and three bathrooms.
    - Analyzed the average price for homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet.
    - Evaluated the average price per "view" rating for homes priced at or above $350,000.

- **Performance Optimization**
  - Implemented caching for the home_sales temporary table to enhance query performance.
  - Compared runtimes of the same query on cached vs. non-cached data.
  - Partitioned the data by the "date_built" field and assessed the impact on query execution speed.

- **Data Management and Cleanup**
  - Created and managed a temporary table for the partitioned data in parquet format.
  - Successfully uncached the  temporary table and verified the cleanup using PySpark commands.

### Key Insights and Impact
The analysis provided valuable insights into the factors influencing home prices over various years and conditions. By leveraging PySpark's in-memory processing capabilities, we significantly improved the efficiency of data queries, especially for complex calculations.

### Conclusion
This project demonstrated effective use of PySpark for data analysis and optimization in a big data environment. The insights gained are crucial for understanding market trends and can assist real estate analysts and investors in making informed decisions. The project was documented and stored in a GitHub repository to facilitate collaboration and future reference.
