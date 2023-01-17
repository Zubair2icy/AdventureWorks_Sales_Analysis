# AdventureWorks_Sales_Analysis
This is a dashboard from several reports built using Microsoft Excel for exploring the sales by adventure works

![Sales Dashboard](https://user-images.githubusercontent.com/88923136/212889328-a4ae56a5-0717-4035-8b68-f1b6a7e8fc8c.png)

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

![Customer Table](https://user-images.githubusercontent.com/88923136/212890110-149e7cc6-59c4-4cbe-94ce-b9ed1f4c7b1d.jpg)

2. Staff Table: Contains information on staff working with Adventure Works. Columns in this table are shown below:

![Staff table](https://user-images.githubusercontent.com/88923136/212890407-f21e361b-beef-4713-a0bb-b096f56da5c2.jpg)

3. Product Table: Contains information on the products that the company sells. Columns in this table can be seen below:

![Products Table](https://user-images.githubusercontent.com/88923136/212890455-8fa0188c-aaa5-4b81-9220-cdafebc1198a.jpg)

4. Orders Table: This contains a list of all the orders and the specific information. Columns here are shown below:

![Orders Table](https://user-images.githubusercontent.com/88923136/212890512-cd76287f-dcff-42dc-b819-aeccc512fbe4.jpg)

5. Order Items: This contains the items ordered for in the order table and their details. Columns here are shown below: 

![Order Items Table](https://user-images.githubusercontent.com/88923136/212890560-8e37d020-da8b-4f60-a281-ab28775a9881.jpg)

# Data Transformation and Modeling:
Various transformations were made to this dataset, which included correct specifications of the data types per column to ensure proper analysis, handling of null values and modeling.
The data was loaded into power pivot for advanced analytics. In power pivot, I firstly created a calendar table to ensure the use of a unified calendar for my analysis using the CALENDAR DAX function  The calendar table is shown below:

![Calendar Table](https://user-images.githubusercontent.com/88923136/212890664-840531fd-fc6c-4d59-a353-3fc71d66c472.jpg)

I also noticed that the sales data started from July 2017. Using such dates like that will give inaccurate conclusions as July will be counted as the 7 month while it was actually the 1st month of sales for the company, hence the need for fiscal date calculations.
I employed my knowledge of DAX functions to create several fiscal date columns. The functions used are:
1. `Fiscal Year = IF('Calendar'[Month Number]>6,'Calendar'[Year]+1,'Calendar'[Year])`
2. `Fiscal Month Number=IF('Calendar'[Month Number]>6,'Calendar'[Month Number]-6,'Calendar'[Month Number]+6)`
3. `Fiscal Quarter=if('Calendar'[Month Number]>9,"2",if('Calendar'[Month Number]>6,"1",if('Calendar'[Month Number]>3,"4","3")))`

The new table with all columns calculated is shown below:

![calendar table](https://user-images.githubusercontent.com/88923136/212892821-5edcfd68-a486-4e39-84e6-6342280a5ef0.jpg)


## Modeling:
Cleaning and modeling data correctly is the most important step to take before Analysis. Otherwise analysis will never be accurate. Thus a very good understanding of modeling data and how to relate fact and dimension tables together is core to achieving a successful data model. 
I carried out the modeling of this data on power pivot and the model is shown on the image below:

![complete model](https://user-images.githubusercontent.com/88923136/212892861-24650170-3b4b-439c-b42d-8d2af8326694.jpg)
 

# Data Analysis and Visualization:
The data from power pivot model was then loaded into pivot tables for analysis.

## Revenue over Time Analysis
The total revenue grew per year exponentially except in 2020  which was most likely due to the pandemic.

![YoY Growth](https://user-images.githubusercontent.com/88923136/212902492-cb0b350c-9bc6-4853-bec7-4736b0f2250b.jpg)


This shows the drill down by month to see the Month over Month Growth in Revenue

![MoM Growth](https://user-images.githubusercontent.com/88923136/212902562-97ad02aa-a00c-427e-9eda-5354e70abdad.jpg)


## Revenue by Region and Country
Consistently for over the years, United States have made higher sales than other region. The reason for the poor sales in other region should be looked into and investigated properly.

![map](https://user-images.githubusercontent.com/88923136/212902691-494356ca-846d-452f-84c9-de4565279efe.jpg)


## Revenue and Product Categories
Bikes sales yield far higher revenues than others even though a lesser number of it is been sold compared to components that yeild a lower revenue. 

![Category](https://user-images.githubusercontent.com/88923136/212902768-34cc4f2f-5237-4c9d-8a48-69acbd768a6c.jpg)


## Customer Satisfaction Analysis:
The report shows there's always delivery delay in about half of orders sold yearly. This translates to a poor customer experience.

![Delays](https://user-images.githubusercontent.com/88923136/212902825-150cc052-c2fa-4da5-8b93-700f0b2f1f4f.jpg)


This poor experience is clearly visible in the massive drop down of customers on the chart below. Customer loss is highest in 2020 due to COVID-19 pandemic and the lockdown in almost all countries.

![Customer Growth](https://user-images.githubusercontent.com/88923136/212902915-6a4c13c0-7b5a-4575-b9ab-30ddea08befb.jpg)



# Recommendations:
1. A diagnostic analysis should be carried out to study why other regions have been generating poor revenues over the years.
2. Issues of delay in delivery of products to customers should be addressed for better customer satisfaction.
3. In depth analysis should be done to understand how the categories of products are being purchased to boost revenue production.


# Dashboard
This is a picture of the completed dashboard.[Click here](zubair2icy@gmail.com) to send am email for a copy of thr dashboard to interact with.

![Sales Dashboard](https://user-images.githubusercontent.com/88923136/212902994-35570766-b07b-4403-be1e-8fa7995d5975.png)



Thanks! Enjoy.

