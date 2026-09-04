## Project Overview
The project conducts an end-to-end analysis of sales transaction data of a global superstore in order to discover key drivers of business growth and identify the root cause of profit loss using SQL and Power BI.

The structure of the project consists of 5 sections:
1. Business Problem
2. Dataset Overview
3. Data Quality Check & Data Cleaning
4. Analysis & Insights
5. Recommendations
   
## Business Problem 
Context: A U.S. retail superstore is selling different products across various customer segments and regions.

Problem Statement: The sales manager wants to know what was actually driving its sales performance and what was negatively impacting the profit margin.

Objective: 
- Understand the trend and seasonality that may have in our business
- Identify the main customer segment that drives the most value
- Identify the top performer and bottom performer by product category and region
- Investigate the main factors reducing overall profit. 

Approach: 
9994 transaction records were profiled and analyzed using Excel and SQL, covering data quality checks, exploratory data analysis, descriptive analysis, diagnosis analysis - then rebuilt as a 4-page interactive Power BI dashboard with custom DAX measures for ongoing business reporting.

Outcome:
The analysis demonstrates that there was trend and seasonality pattern in the business; determined consumer as the main revenue driver while corporate with highest customer value;  and identified technology and West region as the strongest performers - translated into 5 prioritized recommendations across inventory, pricing, operations and marketing.

## Dataset Overview
The dataset contains 9,994 line-item sales transaction data during the period from 2014 to 2017, capturing shipping, customer, geography, product information and sales metrics. 
The dataset source: Superstore Sales Dataset from Kaggle 

## Data Quality Check & Data Cleaning
1. No fully blank rows
2. No missing values
3. No duplicate rows 
4. Date columns are recognized as date
5. Sales, quantity, discount and profit are formatted correctly.
6. Customer/Region/Product spelling is consistent and correct

## Analysis & Insights
Analytical approach: This is a descriptive and diagnostic analysis rather than a predictive one: the goal is to quantify performance by product, segment and region to find top-performer and bottom performers and diagnose the root causes in under-performing product/ region - then visualize the analytical results into a Power BI dashboard to present insights to stakeholders.

### 1. Sales performance 
<img width="601" height="339" alt="Executive Overview Page" src="https://github.com/user-attachments/assets/05cac6e6-7bc6-4174-90ad-e89e4a4348b2" />

Key findings: 
- Revenue increased consistently from 2014 to 2017 except for 2015 which slightly decreased. This indicates sustainable business growth.
- Quarter 4 is the most critical sales season and November is the peak sales month.
- Consumer dominates with over 50% of overall sales, making it the main revenue driver.
- The West region leads in revenue ($0.75M), closely followed by the East region ($0.68M).
- Technology is the best-performing category in terms of sales ($0.84M), followed by Furniture ($0.74M) and Office Supplies ($0.72M).

### 2. Product Analysis
<img width="601" height="335" alt="Product Analysis Page" src="https://github.com/user-attachments/assets/0da65f3d-c5fa-433b-9f7e-0f11756333ff" />

Key findings:
- Technology leads in both sales ($0.84M) and profit ($0.15M).
- Furniture ranks second in revenue ($0.74M) but generated relatively low profit (0.02M).
- Office Supplies fall behind in revenue ($0.72M) but generated higher profit than Furniture ($0.12M)
- Copiers is the best-performer among 12 sub-categories ($56K), followed by Phone ($45K).
- Bookcases (-18K) and Tables (-3K) are the two under-performing sub-categories with minor profit.

### 3. Segment & Region Analysis
<img width="601" height="336" alt="Segment and Region Analysis Page" src="https://github.com/user-attachments/assets/f02c342d-2aa8-47f1-a495-0c84de28f383" />

Key findings:
- Consumer leads in both sales and profit, but Corporate has the highest revenue per customer.
- The West ($0.75M) and the East ($0.68M) are the top two regions.
- The Central ($0.50M) and the South ($0.39M) are smaller markets, with the South being the most underserved.
- California ($76M) and NewYork ($74M) are the two core markets.
- There are several unprofitable states like Texas ($-26M) and Ohio ($-17M).

## Recommendations
- Capitalize on Quarter 4 demand by increasing marketing investment and optimizing inventory planning ahead of the peak shopping season.
- Prioritize investment in top-performing sub-categories in Technology like Copiers and Phones to sustain their contribution to revenue and profit.
- Reassess the discount and pricing strategies for Furniture and consider the repositioning or discontinuation of persistently unprofitable products like Bookcases and Tables.
- Expand the consumer segment to sustain revenue contribution while strengthening relationships with high-value corporate customers through tailored pricing, long-term contracts and dedicated B2B programs.
- Prioritize investment in core markets like California and NewYork, while investigating operational issues in under-performing markets like Texas and Ohio. 










