# [ENG] Data Analysis Project📊
## _➡️Supply Chain Issue In The FMCG Domain_
_Industry: Food, Dairy Products_

## ISSUE: 

Altiq Mart CEO is concerned about the non-renewal of product supply contracts with key clients. They are requesting the analytics team to conduct an investigation to identify the reasons why clients are unwilling to maintain their business relationship with the company.

## OBJETIVES:
- Try to obtain key performance indicators (KPIs) for logistic lines such as On Time, In Full, On Time In Full Ratio, in order to identify the problems that arise when shipping our orders

- Explore other metrics such as VOFR and LIFR, and try to filter by products, months, days, etc. It is important to create visual graphics to represent the metric vs. target during this exploratory data analysis (EDA).

- Deliver our findings and critical points identified to improve our effectiveness ratios and strengthen our customer relationships to our CEO and Supply Chain Manager, in order to maintain a long-term business relationship.

## DATA:

Our data engineering team has delivered six datasheets in .CSV format containing all logistic supply chain information. This information was recorded during fiscal year 2022 and is distributed as follows:

- Dim_customers: This table contains all the information about customers
- Dim_date : This table contains all the information about the products
- Dim_products: This table contains the dates at daily, monthly level and week numbers of the year
- Dim_targets_orders: This table contains all target data at the customer level
- Fact_order_lines: This table contains all information about orders and each item inside the orders.
- Fact_orders_aggregate: This table contains information about OnTime, InFull and OnTime Infull information aggregated at the order level per customer
