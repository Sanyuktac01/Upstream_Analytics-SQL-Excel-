# Upstream_Analytics [SQL-Excel]

## Tasks:
# Exploratory analysis and data manipulation and in SQL.
You are receiving two CSV files “Example_main.csv” and “Example_monthly.csv”. That is an extract from real well data. The first one is the well header (one record per well), and the second file is production data (one record per well – year - month). Oil production is expressed in barrels while gas production is expressed in thousand cubic feet.
Explore the tables write scripts: one in SQL. 
1.Write a code to calculate the average intervals between spud date and completion date by county and spud year. You may want to exclude outliers from this calculation (think: how to decide which values are outliers?)

2.Write a code to output total production of both oil and gas (separately) in the State 2, by month. Display the values in daily rates (barrels per day, thousand cubic feet Mcf per day) instead of total volumes, as is standard in the industry. For example, 28,000 barrels in February and 31,000 in March both correspond to 1,000 barrels per day, which is interpreted as no change,

3.Write a code to generate a new temporary table (resp, dataframe) with columns: year, month, County, oil (bbl), gas (Mcf), and total production, which is oil + gas/6 (as 6,000 Mcf of gas are equivalent energetically to one barrel of oil). Treat NULLs as 0.

4.The key task is to write a code that computes the average well initial productivity by completion year. The initial productivity of a single well is defined, for this exercise, as total production over the first 4 full months after the well is completed.
Note to complete task in SQL: it is recommended to install and use an actual SQL engine, since it will help you explore the data, check the syntax of the queries, etc. Instructions on how to install a SQL server engine locally, such as SQL Server Express, are widely available online; you should then create a database and import the two provided csv files as flat files.


# Excel manipulation and interpretation
Export data from Task 2, step 3, into Excel or open-source alternative, and generate a pivot chart that visualizes total production (oil+gas/6) over time, split by county. Comment on trends you might see: how can they be explained? What drives, fundamentally, the historical trends and short-lived swings? For context, you should be aware these are horizontal shale wells in a certain area of the Permian Basin in the US.
