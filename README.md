# AdventureWorks_Sales_Analysis
This is a dashboard from several reports built using Microsoft Excel for exploring the sales by adventure works

# What is Adventure Works?
AdventureWorks is a frictious bicycle manufacturing database designed by Microsoft. The Organization is based in Bothell, Washington and sells to other part of the world. The database contain information about Sales, Purchasing, Production, Contact management and Human resources. ENJOY!

# Project Objective:
This project only serve as an exploratory of the sales data to better understand the companies progress so far and recommend ways to improve the companies revenue.
In this project, I have sufficiently displayed my indepth knowledge and expeerience in the following:
1. Problem-solving and decision-making skills,
2. Analytical and critical thinking skills,
3. Power query and m-language for advanced data importation and manipulation,
4. Power pivot for advanced data modeling and analysis,
5. Data Analysis Expression (DAX) foradvanced analytics,
6. Creation of calculated tables, columns and measures in power pivot for analysis,
7. Pivot tables, and accurate use of slicers,
8. Customized visualizations and story-telling with data
9. Creation of dashboard and linking of reports in microsoft excel,
10. Automation, macros and VBA in microsoft excel.

# Data Source: 
The datasets used consisted of 5 tables containing various information which can be downloaded here. 
The tables on the 5 tables are:
1. Customer Table: This contains information on the customers that in one time or the other, purchased items from the store. Columns in this table can be seen below:
[[Attach photo]]
2. Staff Table: Contains information on staff working with Adventure Works. Columns in this table are shown below:
[[Attach photo]]
3. Product Table: Contains information on the products that the company sells. Columns in this table can be seen below:
[[Attach Photo]]
4. Orders Table: This contains a list of all the orders and the specific information. Columns here are shown below:
[[Attach photo]]
5. Order Items: This contains the items ordered for in the order table and their details. Columns here are shown below: 
[[Attach photo]]

# Data Transformation and Modeling:
Various transformations were made to this dataset, which included correct specifications of the data types per column to ensure proper analysis, handling of null values and modeling.
The data was loaded into power pivot for advanced analytics. In power pivot, I firstly created a calendar table to ensure the use of a unified calendar for my analysis using the CALENDAR DAX function  The calendar table is shown below:
[[Attach photo of calendar table]]

I also noticed that the sales data started from July 2017. Using such dates like that will give inaccurate conclusions as July will be counted as the 7 month while it was actually the 1st month of sales for the company, hence the need for fiscal date calculations.
I employed my knowledge of DAX functions to create several fiscal date columns. The functions used are: 
[[Insert DAX for fiscal year]]
[[Insert DAX for fiscal month]]
[[Insert DAX for fiscal month number]]
[[Insert DAX for fiscal Quarter]]

The new table with all columns calculated is shown below:
[[Attach calendar full table]]

## Modeling:
Cleaning and modeling data correctly is the most important step to take before Analysis. Otherwise analysis will never be accurate. Thus a very good understanding of modeling data and how to relate fact and dimension tables together is core to achieving a successful data model. 
I carried out the modeling of this data on power pivot and the model is shown on the image below:
[[Attach data model]]

# Data Analysis and Visualization:
The data from power pivot model was then loaded into pivot tables for analysis.

## Revenue over Time Analysis
The total revenue grew per year exponentially except in 2020  which was most likely due to the pandemic.
[[Attach picture of YoY Growth]]

This shows the drill down by month to see the Month over Month Growth in Revenue
[[Attach picture of MoM Growth]]


