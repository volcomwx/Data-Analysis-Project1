# Data-Analysis-Project1

This is an demostration of SQL and Analysis skills along with data visualization skills as an emxaple:

__Inquiry:__

Explore these tables and their underlying data, then write a query that properly joins these three tables. Please answer the following questions and provide a copy of your script along with the output in your answer document.

1.What was the total sales revenue in 2020, and how did this compare to the year prior?  Are there any particular months that drove or hurt sales year-over-year?  Note that sales revenue is a derived field from the KPIs provided.

2.What were the Top 5 Stores (based on revenue) in 2018 and what was their Inventory Sell-Through %? Please provide the store ID, store name, revenue, unit sales, inventory, and sell-through %. Note that ST% is a derived field from the KPIs provided.

3.What were the Top 5 Suppliers and each of their Top 5 Products (based on profit) in 2019? Note that profit is a derived field from the KPIs provided.

Create a one-page dashboard with a couple of visualizations that provide key insights into the data.  

# Clean the Data

__Executive Summary__ 

The Data Cleaning process during the Preparation Period aimed to ensure the quality, accuracy, and consistency of our dataset. This report outlines the steps taken, issues identified, and actions performed to clean the data. 

__Data Sources__ 

During this phase, I utilized data from three primary sources: Sales, Products, and Inventory tables. 

__Data Cleaning Steps__ 

1)Identifying Missing Values: 

I systematically examined each table for missing values. Fortunately, I found no missing data, ensuring that our dataset was complete.

2)Handling Duplicate Values: 

I conducted a thorough check for duplicate values and successfully eliminated any duplicates encountered. 

3)Outlier Detection and Correction: 

I used plots in Excel to identify and assess outliers. Fortunately, I found no significant outliers in our dataset. 

4)Ensuring Data Consistency: 

I meticulously cross-referenced foreign keys in the Sales and Inventory tables with the primary keys in the Products and Inventory tables to ensure data consistency. 

__Data Cleaning Results:__


No missing values were identified in any of the tables.

No duplicates in any of the tables. 

No significant outliers were detected. 

Data consistency was confirmed across the tables.

# Answer to the Questions:
__1.What was the total sales revenue in 2020, and how did this compare to the year prior?  Are there any particular months that drove or hurt sales year-over-year?__  

| Total_Sales_Revenue | Year |
| -------- | -------- |
| 8329108.88 | 2020 |
| 8251369.7  | 2019 |

The total sales revenue in 2020 was $8,329,108.88. When compared to the year prior (2019), the total sales revenue in 2020 was higher by $77,739.18 ($8,329,108.88 - $8,251,369.70).

1)Year-over-Year Comparison: 

Percentage Change = ((Total Revenue in 2020 - Total Revenue in 2019) / Total Revenue in 2019) * 100 

Percentage Change = (($8,329,108.88 - $8,251,369.70) / $8,251,369.70) * 100 ≈ 0.94%

2)Year-over-year monthly sales analysis:

The overall yearly comparison indicates a modest YoY increase in total revenue for 2020 compared to 2019. Several months experienced notable changes: March 2020 saw a significant decline in revenue, while April 2020 showed significant growth compared to April 2019. November 2020 had a substantial increase, contributing positively to the overall yearly performance. 

February experienced a notable decrease in both of the two years, followed by a subsequent increase in March.


__2.What were the Top 5 Stores (based on revenue) in 2018 and what was their Inventory Sell-Through %? Please provide the store ID, store name, revenue, unit sales, inventory, and sell-through %.__


|StoreName                  |StoreId |Revenue   |Unit_Sales |Inventory |Sell_Through_Rate|
|---------------------------|--------|----------|-----------|----------|------------------|
|Ben Franklin               |84879   |374340.8  |115649     |15893     |87.92%            |
|Family Dollar              |71053   |346013.82 |96418      |10879     |89.86%            |
|Burlington Coat Factory    |22745   |342312.46 |79011      |9206      |89.56%            |
|Shopko                     |22726   |340826.5  |97426      |11641     |89.33%            |
|Renys                      |22748   |327836.39 |83244      |9749      |89.52%            |

__3.What were the Top 5 Suppliers and each of their Top 5 Products (based on profit) in 2019?__

The top 5 Suppliers are:

| Supplier                | Profit     |
|-------------------------|------------|
| Ben Franklin            | 160028.5   |
| Shopko                  | 151974.58  |
| Family Dollar           | 144965.16  |
| Renys                   | 138228.15  |
| Burlington Coat Factory | 137484.6   |

Top 5 Products are:

| Supplier      | ProductName                     | Profit   |
|---------------|---------------------------------|----------|
| Ben Franklin  | Flour - Rye                     | 18374.92 |
| Ben Franklin  | Soup - Campbells, Minestrone    | 13474.8  |
| Ben Franklin  | Wine - Red, Metus Rose          | 8508     |
| Ben Franklin  | Parsley Italian - Fresh         | 7884.81  |
| Ben Franklin  | Pepper - Cubanelle              | 7606.4   |


| Supplier | ProductName                        | Profit   |
|----------|-----------------------------------|----------|
| Shopko   | Chocolate - Liqueur Cups With Foil | 17021.21 |
| Shopko   | Latex Rubber Gloves Size 9        | 11019.16 |
| Shopko   | Wine - Cousino Macul Antiguas     | 10269    |
| Shopko   | Cheese - Pont Couvert             | 9245.61  |
| Shopko   | Bandage - Flexible 1x3            | 7790.55  |

| Supplier      | ProductName                     | Profit   |
|---------------|---------------------------------|----------|
| Family Dollar | Cheese - Valancey               | 10450.08 |
| Family Dollar | Onions - Cooking                | 10424.4  |
| Family Dollar | Container - Foam Dixie 12 Oz    | 9715.2   |
| Family Dollar | Coffee Cup 16oz Foam            | 9429.37  |
| Family Dollar | Juice - Apple, 500 Ml           | 8058.26  |

| Supplier | ProductName                       | Profit   |
|----------|-----------------------------------|----------|
| Renys    | Bread - Italian Sesame Poly       | 14318.53 |
| Renys    | Vodka - Hot, Inferno               | 13200.66 |
| Renys    | Pepper - Green, Chili              | 11412.54 |
| Renys    | Tarragon - Primerba, Paste         | 7272.6  |
| Renys    | Soup - Tomato Mush. Florentine     | 6463.1  |

| Supplier                | ProductName                  | Profit   |
|-------------------------|-----------------------------|----------|
| Burlington Coat Factory | Chips Potato Salt Vinegar 43g | 13145.63 |
| Burlington Coat Factory | Soup - French Onion, Dry     | 9938.09  |
| Burlington Coat Factory | Oranges                     | 9767.52  |
| Burlington Coat Factory | Lid - 3oz Med Rec            | 9246.53  |
| Burlington Coat Factory | Table Cloth 54x72 Colour    | 8388     |
