# Maven Toys Sales Analysis
![](Toy_Store.png)
---
## Introduction
This is a SQL project that aims to provide **Maven Toys**, a fictional chain of toy stores in Mexico, with actionable insights into product profitability, seasonal sales trends, stock outs impact, and inventory efficiency.

## Table Of Content
- Project Overview
- Project Scope
- Business Objective
- Document Purpose
- Use Case
- Skills Demonstrated
- Data Source
- Data Cleaning and Processing
- Data Analysis and Insight
- Recommendation
- Conclusion

## Project Overview
The objective of the Maven Toy Sales and Inventory Analysis project is to offer practical insights regarding product profitability, seasonal sales patterns, the impact of stockouts, and inventory efficiency to Maven Toys, a fictitious chain of toy stores in Mexico.

The goal of this project is to thoroughly analyze the data from Maven Toys to pinpoint important areas in need of enhancement and optimization.

## Project Scope
This project entails a thorough analysis of Maven Toys' sales and inventory data, including stores, inventory levels, daily sales and products. The analysis covers data from January 1, 2022, to September 30, 2023, to provide a comprehensive view of Maven Toys' operational performance.

## Business Objective
The main goal of the Maven Toys Sales and Inventory project is to find the product categories that bring in the most profits and check if these categories are consistently profitable in all store locations. it seeks to ascertain the patterns and trends in sales over different time periods, identify any potential loss of sales due to out-of-stock products at specific locations, and determine the amount of money tied up in inventory at the toy stores and how long it will last.

## Document Purpose
This documentation serves as a guide for project stakeholders, providing insights into the project's objectives, data sources, data analysis, and any other relevant information.

## Use Case
The insights gained from the analysis of Maven Toys sales can assist multiple stakeholders. The following important parties may find this analysis useful and advantageous.

### 1.	Maven Toys Executives and Management:
Executives and upper management can use the analysis to make informed decisions about product offerings, store locations, and overall business strategy.

### 2.	Sales Teams: 
Based on the analysis, sales teams can identify possible opportunities for growth and gain insight into popular products, customer preferences, and sales trends.

### 3.	Inventory managers: 
By using the analysis, those in charge of inventory can improve stocking plans, spot slow-moving goods, and lower the frequency of stockouts.

### 4.	Marketing Teams:
By utilizing the analysis, marketing teams can align their marketing efforts with the most profitable product categories and customize promotional strategies, particularly during peak seasons.

### 5.	Store managers 
Store managers can enhance their individual store operations by utilizing inventory management strategies, seasonal trends, and insights into product performance.

## Skills/ Concepts Demonstrated
The following SQL featuresbwere incorporated:
- Data Connection in Microsoft SQL Server
- Data Cleaning and Processing
- Developed a Database Schema
- Data Analysis
- Join
- CTE (Common Table Expression)
- SQL Window Functions

- ## Data Source
The project utilizes a dataset containing information on sales and inventory. The dataset used for this analysis was downloaded from **check**  website where datasets are available for practice purposes. The dataset is a CSV file, and it consists of four main tables which are sales table, product table, inventory table, and store table.

The product table, which has 35 rows and 5 columns, contains information about the goods that Maven Toys sells. The table contains details about each product, including its name, category, cost, and price. Each product is uniquely identified by its Product ID.
The inventory table shows the current stock levels of every product in every store. It has 1,593 rows and 3 columns. The columns include Product ID, Store ID, and Stock on Hand.
Store table comprises 50 rows and 5 columns. The columns include Store ID, Store Name, Store City, Store Location, and Store Open Date.
The sales table, which includes 829,262 rows and 5 columns, records the quantity and type of products sold. With columns for Sale ID, Date, Store ID, Product ID, and Units, this table offers insights into daily sales activity.

## Data Cleaning and Processing
Data cleaning is necessary because the accuracy and dependability of the input data have a significant impact on the quality of analysis and insights obtained from it. Inaccurate conclusions and difficulty making decisions can result from incomplete or inconsistent data. I can make sure that my analyses are based on a strong foundation and produce more dependable results and well-informed decision-making by carefully cleaning and preparing the data.

For each table used in the analysis, extensive data cleaning procedures were carried out. For every table, the following steps were taken to guarantee high data accuracy and integrity and to improve the dataset's high quality.

### 1. Correcting Data Types:

Ensured that data types are appropriate for the values in each column, converting datatype if needed.

### 2. Recognizing and Managing Null Values:
Extensive checks were conducted to detect and manage any occurrences of null values on the primary columns in every table. In this dataset, null values denote missing or insufficient data. Therefore, by guaranteeing that every observation contains all relevant information, addressing rows with null values helps maintain the dataset's overall integrity. Results from incomplete data analysis can be deceptive.

Upon executing a query to identify null values in each table, the output indicates that every table involved in this analysis contains complete information. Importantly, there are no instances of null values detected in the key columns across all tables, highlighting the completeness and data integrity of the dataset used for this analysis.

### 3. Handling Duplicates:

Duplicate records were found and eliminated to prevent redundancy and preserve data integrity.

After running a query to find and remove all duplicate rows in each table, it has been confirmed that every table used in this analysis is free of duplicate rows. Each row in these tables contains unique information, ensuring the integrity of the dataset and providing distinct and valuable data for the analysis.

### 4. Standardizing Data: 

Ensuring uniformity in data representation and format, including text case and date formats. 

During the data processing phase, the following procedures were also completed.
- #### Added a new column
A new column called "product profit" was added to the product table, calculating the profit for each product.  This column is essential for determining which product category is profitable, as it offers insightful information about the most lucrative product categories.

New columns were also added to the sales table. These are Weekday, Month Number, Month Name, and Year, these additions are crucial for a thorough look at sales trends. Businesses can quickly identify trends with these columns, such as which days, months, or years have higher sales. Making informed decisions about product inventory management, promotion scheduling, and general business strategy is made easier with the use of this information.
- #### Established Relationships Between Tables.
Establishing connections between the tables is essential to this analysis. In addition to keeping the data organized, it also facilitates quicker query execution, prevents needless data duplication, and creates a flexible database structure.




