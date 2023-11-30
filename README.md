# Pizzza-Sales-Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Results](#results)
- [Recommendations](#recommendations)

## Project Overview
This data analysis project aims to provide insights into the sales performance of an Pizza Sales over 
the past year. By analyzing various aspects of the sales data, we seek to identify trends, 
make data-driven recommendations, and gain a deeper understanding of the sales performance.

Dahboard First Page
![WhatsApp Image 2023-11-30 at 5 45 49 PM](https://github.com/Siddhu-T/Pizzza-Sales-Analysis/assets/101640915/bfca18f7-7019-4e56-9551-cf0e78e5c3eb)


## Data Source
Sales Data: The dataset used for this analysis is in the "pizza_sales.csv" file, contain detail information 
about the sales in the company

## Tools
- Excel - Data Cleaning
- SQL - Data Analysis
- Tableau - Creating Dashboards

## Data Analysis
Percentage of sakes by Pizza Category
```sql
select pizza_category,round(sum(total_price),2) as price,
round(sum(total_price)/(select sum(total_price) from pizza_sales)*100,2) as pct
from pizza_sales
group by pizza_category
```

## Results

1. Peak Orders of pizza are between 12:00 pm to 1:00 pm in afternoon and in the
evening from 4:00 pm to 6:00 pm
2. The highest order was placed in the 48th week from the month of December
3. Classic Category contibutes to maximum sales, total orders, and total pizza sold
4. Large Size Pizza contributes to the maximum sales

## Recommendations

1. Workers should be increased during the peak hours.
2. Offers should be applied on the pizzas which are sold in very less quantity
3. Inventory storage for the Classic Category Pizzas should be increased as the demand
for them is also high

😄💻
