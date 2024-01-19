[Enlace a la sección de análisis de datos](#proyecto-de-analisis-de-datos📊)

# Data Analysis Project📊
## _➡️Supply Chain Issue In The FMCG Domain_
_Industry: Food, Dairy Products_

## ISSUE: 

Altiq Mart CEO is concerned about the non-renewal of product supply contracts with key clients. They are requesting the analytics team to conduct an investigation to identify the reasons why clients are unwilling to maintain their business relationship with the company.

## OBJETIVES:
- Try to obtain key performance indicators (KPIs) for logistic lines such as On Time, In Full, On Time In Full Ratio, in order to identify the problems that arise when shipping our orders

- Explore other metrics such as VOFR and LIFR, and try to filter by products, months, days, etc. It is important to create visual graphics to represent the metric vs. target during this exploratory data analysis (EDA).

- Present our findings and key insights aimed at enhancing our efficiency metrics and bolstering our customer relationships to both our CEO and Supply Chain Manager. This will help us maintain a long-term business partnership

## DATA:

Our data engineering team has delivered six datasheets in .CSV format containing all logistic supply chain information. This information was recorded during fiscal year 2022 and is distributed as follows:

- Dim_customers: This table contains all the information about customers
- Dim_date : This table contains all the information about the products
- Dim_products: This table contains the dates at daily, monthly level and week numbers of the year
- Dim_targets_orders: This table contains all target data at the customer level
- Fact_order_lines: This table contains all information about orders and each item inside the orders.
- Fact_orders_aggregate: This table contains information about OnTime, InFull and OnTime Infull information aggregated at the order level per customer

💻 To find all the analytical development done in Python [click here](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/blob/main/SupplyChain_Challengue.ipynb)

📚 You can also check the dash board [click here](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/blob/main/dashboard.pbix)

📊 live presentation in video [youtube](https://youtube.com)

![dashb1](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/9a9ecc61-7c30-41e1-b7cc-609ef8845b9a)
![dashb2](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/c2a0db05-3799-432d-b0a3-c3227d9e5930)
![dashb3](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/d96ca1c5-7116-48fd-b808-818a7ab63b1c)

## INSIGHTS

1. After analyzing our KPIs, we have found that our logistics chain needs to increase efforts and allocate resources to optimize shipments by an additional 50% beyond the current level, especially to ensure on-time and complete deliveries. We have observed that our OTIF indicator only reaches about ≈49% of the expected goal, leading to only ≈30% of our deliveries meeting the minimum effectiveness standard.
   
2. Looking at KPIs by customer, we note that customers with high volume orders (>1000) have been adversely affected in terms of the timing or the full quantity of their orders(OTIF%). However, this metric is general, and to see the difference over a longer period of time, it is necessary to examine the entire supply chain within the timeframe.
   
3. To ensure accuracy, let's review the customer codes step-by-step and compare the metrics for each user. It has come to our attention that the following accounts: 789122, 789420, 789522, 789421, 789422, 789520, 789601, and 789903 are experiencing serious issues with delivery, specifically with delays and incomplete shipments. These problems have persisted over a significant period of time, indicating consistent supply chain challenges. Similarly, the accounts 789121, 789521, 789603, 789702, 789621, 789503, 789103, and 789501 are facing challenges with incomplete deliveries, which are adversely impacting our key performance indicator (KPI) and customer relationships.
   
4. Upon reviewing the last graphs, we have come to the conclusion that we lack quantitative evidence to determine if our problem lies in the complete order quantity. Currently, all our products are at approximately 60% - 70% of the LIFR% (Lead-time Inventory Fill Rate), but all our orders have already reached 95% in VOFR%. Furthermore, this percentage has remained stable over a long period of time. Hence, we can conclude that our problem lies in the supply chain, specifically in the preparation and dispatch of products to the final customer.

At this juncture, it is crucial to assess whether our KPIs are directly correlated with specific products.

## CONCLUSIONS

After analyzing the performance of each product, we have determined that Surat City is facing significant supply chain challenges with completed orders, with an alarming error rate of 90% across all product ranges. The graphs and boxplots reveal two major issues:

- High Volatility: The boxplots for Surat City show a wide range, indicating instability in our product supply chain. This is adversely affecting our customers, particularly in economic terms. Each range already has a 40% LIFR (Late and In Full Rate) issue.

- Vadodara City is also experiencing problems with incomplete orders for specific products, including Butter 500, Curd 100, Ghee 100, and Ghee 250.

- Our products, Milk 100, Milk 250, and Milk 500, have encountered delivery and production issues in all cities.

- In light of these findings, we urge the Production and Logistics departments to thoroughly analyze and review the manufacturing lines for the following products: Biscuits 750, Butter 100, Butter 250, Butter 500, Curd 100, Curd 50, Ghee 100, and Ghee 250.
