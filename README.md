# Customer Shopping Behavior Analysis

End-to-end analysis of 3,900 retail purchases using **Python, SQL and Power BI**, to understand spending patterns, customer segments, discount dependency and subscription behavior.

![Dashboard](images/dashboard.png)

## Business question
How can a retailer use customer shopping data to identify purchasing trends, improve engagement and loyalty, and optimize marketing and product strategy?

## Dataset
- 3,900 rows, 18 columns: demographics, purchase details, shopping behavior (discounts, shipping, reviews, previous purchases, frequency).
- Source: _add the link to the dataset here (e.g. Kaggle)._

## Workflow
1. Python (pandas): loaded and explored the data, imputed 37 missing review ratings with the median rating of each product category, standardized column names to snake_case, engineered `age_group` (quartile bins) and `purchase_frequency_days`, and dropped `promo_code_used` because it duplicated `discount_applied`.
2. SQL: loaded the cleaned table into a relational database and answered 10 business questions using aggregation, subqueries, `CASE`, CTEs and window functions (`ROW_NUMBER`).
3. Power BI: built an interactive dashboard with 4 KPIs, 5 charts and 5 slicers.

Key findings
- Revenue: $233,081 total from 3,900 customers (average purchase $59.76, average rating 3.75).
- Category mix: Clothing generates about 45% of revenue ($104,264), followed by Accessories ($74,200).
- Subscriptions: 27% of customers subscribe, but subscribers spend the same as non-subscribers ($59.49 vs $59.87 on average).
- Gender: males account for about 68% of revenue, but that matches their share of customers; average spend is nearly equal ($59.50 vs $60.20).
- Loyalty: 80% of customers (3,116) have more than 10 previous purchases ("Loyal"); only 83 are "New".
- Discounts: about 43% of purchases use a discount; Hat (50.0%) and Sneakers (49.7%) are the most discount-dependent products.
- Age: revenue is spread fairly evenly across age groups ($55.8K to $62.1K).
- Shipping: Express orders average $60.48 vs $58.46 for Standard.


## Tools
Python (pandas, NumPy), SQL (PostgreSQL / SQL Server), Power BI.
