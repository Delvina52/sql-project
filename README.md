SQL Data Analysis Portfolio
Farmer's Market (Mandi) | Window Functions & Business Analysis

A SQL project on a Farmer's Market database, written from the view of a data analyst helping the market manager understand vendors, customers and daily sale

Farmer's Market Analysis
Dataset: InterviewBit – Exploring the Farmer's Market (9 tables: `customer`, `customer_purchases`, `vendor`, `vendor_inventory`, `vendor_booth_assignments`, `booth`, `product`, `product_category`, `market_date_info`)

Key Analysis:
- Vendor revenue ranking using `DENSE_RANK()` (ties share a rank, no gaps)
- Latest purchase per customer using `ROW_NUMBER()` with tie-breaking on time and product
- Running total of spend per customer using `SUM() OVER (PARTITION BY ...)`
- Rolling 7-market-day average of daily revenue using a CTE and window frame

Business Value:
Helps the market manager identify top-earning vendors, track what each customer bought last and how much they spend over time, and spot sales trends without daily noise.


 Questions Solved

Question 
| 1 | Which vendors earn the most? | JOIN, GROUP BY, DENSE_RANK |
| 2 | What was each customer's most recent purchase? | ROW_NUMBER, PARTITION BY |
| 3 | How does each customer's spend build up over time? | Running total with window SUM |
| 4 | What is the sales trend across market days? | CTE, rolling AVG |


 Tools & Skills
- SQL (Joins, Aggregations, CTEs, Window Functions)
- Business Analytics
- Data Exploration
