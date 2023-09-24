### Datasets Selected

I selected two transparent pricing datasets from two different hospital systems: Stony Brook University Hospital and Catholic Health St. Joseph Hospital. I found these datasets under the HHA 504 Week 3 folder. Thes datasets provided a lot fo info with various categorical and numerical columns. The first set of Stony Brook had a lot of info regarding deidentified rates, cash prices, gross charges, and different types of insurances. The second set of Catholic Health had a lot of inforegarding charges, prices, and packages.

### Exploratory Data Analysis Process

I conducted the same process for both datasets. First, I wanted a data overview of the first few rows of each column. From this, I saw many NaN outputs so I wanted to check for the sum of the missing values of each column in the individual dataset. There were a lot. Then, I checked for frequency counts for categorical columns, which varied between the datasets. Next, I wanted to see the data distribution using histograms and boxplots. The histograms showed skewness of the data and the boxplots showed outliers. Loops were used for both because there were a lot of numerical columns. Finally I generated summary statistics for both datasets.


### Instructions to replicate my SQLite database setup

 To create a temporary and local DB using SQLITE, I used the 'sqlite3' library in Python. I named my database 'health.db', but can be named otherwise. Then, I manually created a table using SQL queries. In my example, I created a table named 'stonybrook' using the 'CREATE TABLE' SQL query with the following columns: hospital_name, type, code, cost_minimum, and cost_maximum. Some of these are numerical columns and some are categorical columns. Then, I inserted a row of sample data of which I inputted random fake data using the 'INSERT INTO' SQL query. Then, I automatically created a table by implementing the 'to_sql' function from Pandas to take the example data from the beginning part of the assignment into the SQLite database. You can check if it worked by using the SQL 'SELECT' statement.
                   
