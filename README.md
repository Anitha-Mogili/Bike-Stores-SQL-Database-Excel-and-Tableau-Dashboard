# Bike-Stores-SQL-Database-Excel-and-Tableau-Dashboard

## Project Overview
This project focuses on analyzing and visualizing data related to Bike Stores. The goal is:
* To know the condition of the sales activities within the company and gain insights into the various trends happening in the sales volume over the 2016 to 2018 period.
* To know the revenues per region, per store, per product category and per brand.

## Collecting and Cleaning Data

### Generating Dataset in SQL:
The SQL database named BikeStores consisted of 9 tables. Using these tables, generated a dataset for the Analysis and Visualizations **by joining the tables and extracting the required columns.**

**By joining the tables and using window functions got the below columns for the dataset:**
* **order_id**
* **customers** (Name of the Customer obtained by combining first_name and last_name columns using **CONCAT function**)
* **city** (the city in which the customer lives)
* **state** (the state in which the customer lives)
* **order_date**
* **Total_units** (total units of bikes sold per order obtained by using **SUM** function on quantity column)
* **Revenue** (Revenue generated per order obtained by using **SUM** function and mathematical operations on quantity and list_price columns)
* **Product_name** (Names of the bikes that were purchased)
* **Category_name** (category to which the bikes belonged to)
* **Brand_name** (brands of the bikes that were purchased)
* **Store_name** (the store at which the sales took place)
* **Sales_rep** (Sales representative name that made the sale obtained by combining first_name and last_name columns using **CONCAT function**)

### Connecting SQL database to Excel Workbook:
Connected the entire Excel Workbook to the SQL database and then imported the dataset directly into a worksheet. This way any changes/updates in the database will be automatically reflected in our Excel Workbook dataset sparing us the time to makes changes in the excel dataset whenever there is an update in the SQL database.

## Generated Dataset:
![image](https://github.com/Anitha-Mogili/Bike-Stores-SQL-Database-Excel-and-Tableau-Dashboard/assets/64921654/55553779-33cd-47d9-b831-9f022a39e742)


## Excel Dashboard:
Created an Excel dashboard by importing the cleaned data and setting up **interactive visualizations** and **pivot tables**. The Dashboard contains **pivot charts, filters, slicers, maps** to gain insights on the Revenue generated per year, per month, per state, per store, per brand, per product category, by customers and by sales rep.

![image](https://github.com/Anitha-Mogili/Bike-Stores-SQL-Database-Excel-and-Tableau-Dashboard/assets/64921654/c8fd6d59-e281-4cde-910f-fc0e29a0e249)



## Insights:
* The state of New York generated the highest revenue over the three years followed by California and Texas.
* The bikes belonging to the Trek Brand took the top place for the highest revenue generated for all the 3 years.
* Mountain bikes category which had highest sales in both 2016 and 2017 lost to Road Bikes in the year 2018.
* Sales representatives Marcelene Boyer, Venita Daniel, Genna Serrano always stood in the top 3 positions in all the 3 years.
* The top 3 customers belong to the New York state.
* The year 2018 recorded its peak sales in the month of April and made very little after June.

## Recommendations:
* Priority to be given to New York Customers for generating the highest revenue at the same time not neglecting the other state customers.
* Introduce special offers in the holiday season to generate more sales as we can see a decline in the revenue generated in those months.
* Have a surplus of the most sold brand and category to meet the demands of customers.
* To increase sales, efforts should be made by applying, regularly reviewing and revising SMART (specific, measurable, achievable, relevant and time-bound) objectives and marketing strategies to increase sales in the state of Texas.
