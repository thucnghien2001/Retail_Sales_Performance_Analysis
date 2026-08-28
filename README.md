## PROJECT OVERVIEW
The project conducts an end-to-end sales performance data analytics of a Global superstore in order to discover the key drivers of the business growth and solve the root cause of decline in profit margin to help improve the overall sales performance.
The project is divided into 4 main parts:
- Business Scenario
- Dataset Review
- Data Cleaning & Transformation
- Data Analysis & Visualization
- Recommendations

## BUSINESS SCENARIO
A U.S. retail superstore is selling different products across various customer segments and regions. Based on the sales performance of the last 4 years, the manager wants to know what are the key drivers of business growth and identify the main factors that result in the decline in profit margin. So the analysis need to answer the following questions:
- What is the trend and seasonality of the business over the last 4 years?
- Which customer segment drives the most value?
- Which product category and region contribute most to the overall sales and profit?
- What negatively impacts the overall profit margin?

## DATASET REVIEW
This dataset contains 9,994 line-item transactions between 2014-2017 across 5,009 orders for a US retail store, capturing shipping, customer, geography, product information as well as sales metrics.

The dataset source: Superstore Sales Dataset (Kaggle)

## DATA CLEANING & PREPARATION
The dataset needs to be cleaned and validated to ensure data quality before use for analysis and reporting. In this case, I use Excel for data cleaning to ensure the accuracy and consistency of the dataset. 
Checklist:
1. No fully blank rows
2. No missing values
3. No duplicate rows 
4. Date columns are recognized as date
5. Sales, quantity, discount and profit are formatted correctly.
6. Customer/Region/Product spelling is consistent and correct

## DATA ANALYSIS & VISUALIZATION
Based on the main questions that are mentioned above, I can divide the analysis into four parts:
- Sales Performance Overview
- Segment Performance Analysis
- Category Part-to-Whole Analysis
- Region Part-to-Whole Analysis

### Sales Performance Overview
This section analyzes the sales performance over the last 4 years to track trends and define the seasonality in the sales data.

First I calculate and represent the main KPIs: Total Sales, Total Profit, Profit Margin, Total Orders, Average Order Value to give a big picture of the overall business performance, using DAX formulas for specific calculations.

Then I use column charts to represent the yearly/quarterly/monthly revenue trend.

<img width="601" height="334" alt="Executive Overview" src="https://github.com/user-attachments/assets/617c103e-30c2-479e-9a0a-10491d797cda" />

Some key insights that are extracted from this analysis:
- The revenue and profit increased consistently in the period of 2014 - 2017, except for the revenue in 2015 which decreased. This indicates sustainable business growth.
- Quarter 4 is the most critical sales season and November is the best month for sales, which is reasonable because of major shopping events such as Black Friday, Cyber Monday and Christmas holiday.

### Segment Performance Analysis
This section analyzes and compares the performance of different customer segments to identify the contribution of the customer segment to the business.

First I calculate and represent the main KPIs: Total Customers, Revenue per Customer, Average Purchase Frequency, Repeat Purchase Rate, Top 10% Customer RevenuênConcentration.

Then I analyzed Revenue by Segment, Revenue per Customer by Segment, Purchase Frequency, Top 5 customers by Revenue, Top 5 customers by Profit.

<img width="601" height="337" alt="Segment_Performance" src="https://github.com/user-attachments/assets/6f91f9a0-efee-4c89-a138-31e919ee738c" />

Some key findings that are extracted from the analysis:
- The consumer segment is the main revenue driver of the business, which accounts for more than 50% of the total revenue.
- On the other hand, the corporate segment has the highest revenue per customer, which means corporate customers generate the most value.

### Category Performance Analysis
This section analyzes sales performance by category in order to find the top-performing category/ sub-category/ product and identify the underlying reason that leads to low profit in some of the categories.

In this section, I analyze Sales and Profit by Category, Discount and Profit correlation by category, Top 10 highest-profit sub-categories and Top 10 lowest-profit sub-categories.

<img width="602" height="334" alt="Category_Performance" src="https://github.com/user-attachments/assets/71108843-61e3-4cb2-a1fb-0e7c19c5f558" />

Some key insights that are extracted from this analysis:
- Technology is the best-performing category in terms of sales and profit, which means Technology is the main category that drives the business growth. Furniture ranks second in terms of sales but generates relatively low profit (0.02M), which may indicate the ineffective discount policy on this category. In order to find the root cause of this problem, I find the correlation between Discount and Profit by each category. The result shows that Furniture is the highest discount category which decreases profit in this category.
- Regarding sub-category, Copies and Phones are the highest-profit, while Tables and Bookcases are consistently unprofitable sub-categories.
- In terms of sales over time, Technology is the fastest-growing category over the years while Furniture maintains consistent sales.

### Regional Performance Analysis
This section analyzes the sales performance by region in order to identify the importance of each region to the business. 

In this section, I analyze Sales by Region, Top 5 highest-profit states, Top 5 lowest-profit states Shipping Mode and Profit correlation. 

<img width="601" height="339" alt="Region_Performance" src="https://github.com/user-attachments/assets/bffb7b02-6910-4a8f-83c8-1b5c9c33bf2a" />

Some key insights from the analysis:
- The West and the East are two main regions that generate the highest revenue and profit.
- Central has the lowest profit margin. This is due to the high discount policy in this region where the average discount rate is ~24%, 1,5 times the average discount rate.
- On the state-level, California and New York are the most profitable markets, while Texas, Ohio and Pennsylvania generate negative profits. This is likely due to the high operational costs in these areas, which needs further investigation. 

## Recommendations
- Based on the findings, I propose some strategic recommendations in order to improve the sales performance of the business:
- Capitalize on Q4 demand by increasing marketing investment and optimizing inventory planning ahead of the peak shopping season to achieve the best sales performance during this period.
- Expand the consumer segment while strengthening relationships with high-value corporate customers through tailored pricing, long-term contracts, and dedicated B2B programs.
- Invest in high-performing markets and products, particularly California, New York and Technology category, while addressing operational inefficiencies in low-profit regions such as Texas and Ohio.
- Optimize the product portfolio by reassessing pricing and promotional strategies for Furniture and considering the repositioning or discontinuation of persistently unprofitable products.



