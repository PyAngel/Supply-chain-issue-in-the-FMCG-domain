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
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# Proyecto de análisis de datos📊
## _➡️Problema en cadena logística en bienes de consumo rápido_
_industria: alimentos, lacteos_

## PROBLEMA: 

El gerente general de Altiq Mart está preocupado por la no renovación de los contratos de suministro de productos con clientes clave. Solicitan al equipo de análisis que lleve a cabo una investigación para identificar las razones por las que los clientes no están dispuestos a mantener su relación comercial con la empresa.

## OBJETIVOS:

- Obtener los indicadores de desempeño (KPIs) para líneas logísticas como a tiempo, completo, a tiempo/completo, para identificar los problemas que tenemos al enviar nuestros pedidos.

- Revisar otras métricas como VOFR (ratio de llena por volumen) y LIFR (ratio de llenado por línea), y realizar filtrado por producto, mes, año, etc. Es importante crear gráficos visuales para representar la métrica frente al objetivo durante este análisis exploratorio de datos (EDA).
  
- Presentar nuestras conclusiones y puntos de vista clave destinados a mejorar nuestras métricas de eficiencia y reforzar las relaciones de nuestros clientes con nuestro Director General y Director de la Cadena de Suministro. Esto nos ayudará a mantener una asociación comercial a largo plazo.

## DATOS:

Nuestro equipo de ingeniería de datos ha entregado 6 tablas en formato .CSV que contienen toda la información de la cadena logística. Esta información fue registrada en el año fiscal 2022 y se distribuye de la siguiente manera:

- Dim_customers: Esta tabla contiene la información de los clientes
- Dim_date : Esta tabla contiene información sobre productos
- Dim_products: Esta tabla contiene las fechas como día, mes etiqueta y número de semana en el año
- Dim_targets_orders: Esta tabla contiene todos los niveles objetivos para cada cliente
- Fact_order_lines: Esta tabla contiene todas las ordenes y cada item correspondiente en cada orden
- Fact_orders_aggregate: Esta tabla contiene la información de a tiempo, completo y a tiempo y completo agregada a cada nivel de orden por cliente.

 ## HALLAZGOS:

1. Después de analizar nuestros indicadores clave de rendimiento (KPIs), hemos encontrado que nuestra cadena logística necesita aumentar esfuerzos y asignar recursos para optimizar los envíos en un 50% adicional más allá del nivel actual, especialmente para garantizar entregas completas y a tiempo. Hemos observado que nuestro indicador de OTIF solo alcanza aproximadamente un ≈49% de la meta esperada, lo que resulta en que solo aproximadamente un ≈30% de nuestras entregas cumplan con el estándar mínimo de efectividad.

2. Al observar los KPIs por cliente, notamos que los clientes con pedidos de alto volumen (>1000 ordenes) se han visto afectados negativamente en cuanto al tiempo o la cantidad completa de sus pedidos (OTIF%). Sin embargo, esta métrica es general, y para ver la diferencia a lo largo de un período más largo, es necesario examinar toda la cadena de suministro dentro del marco de tiempo.

3. Para garantizar la precisión, revisemos los códigos de cliente paso a paso y comparemos las métricas para cada usuario. Nos ha llamado la atención que las siguientes cuentas: 789122, 789420, 789522, 789421, 789422, 789520, 789601 y 789903 están experimentando problemas graves con la entrega, específicamente retrasos y envíos incompletos. Estos problemas han persistido durante un período significativo, lo que indica desafíos consistentes en la cadena de suministro. Del mismo modo, las cuentas 789121, 789521, 789603, 789702, 789621, 789503, 789103 y 789501 enfrentan desafíos con entregas incompletas, que están afectando negativamente nuestro indicador clave de rendimiento (KPI) y las relaciones con los clientes.

4. Tras revisar los últimos gráficos, hemos llegado a la conclusión de que nos falta evidencia cuantitativa para determinar si nuestro problema radica en la cantidad total de los pedidos. Actualmente, todos nuestros productos se encuentran en aproximadamente un 60% - 70% del LIFR% (Tasa de Relleno de Inventario en el Plazo de Entrega), pero todos nuestros pedidos ya han alcanzado un 95% en VOFR%. Además, este porcentaje se ha mantenido estable durante un largo período de tiempo. Por lo tanto, podemos concluir que nuestro problema radica en la cadena de suministro, específicamente en la preparación y el envío de productos al cliente final.

En este punto, es crucial evaluar si nuestros KPIs están directamente correlacionados con productos específicos.


## CONCLUSIONES:

Tras analizar el rendimiento de cada producto, hemos determinado que la ciudad de Surat enfrenta desafíos significativos en su cadena de suministro con respecto a los pedidos completados, con una alarmante tasa de error del 90% en todas las gamas de productos. Los gráficos y diagramas de caja revelan dos problemas principales.

1. Alta Volatilidad: Los diagramas de caja para la ciudad de Surat muestran un amplio rango, lo que indica inestabilidad en nuestra cadena de suministro de productos. Esto está afectando negativamente a nuestros clientes, especialmente en términos económicos. Cada rango ya tiene un problema del 40% en la tasa de LIFR%.

2. La ciudad de Vadodara también está experimentando problemas con pedidos incompletos en productos específicos, incluyendo Mantequilla 500, Yogur 100, Ghee 100 y Ghee 250.

3. Nuestros productos, Leche 100, Leche 250 y Leche 500, han enfrentado problemas de entrega y producción en todas las ciudades.

A la luz de estos hallazgos, instamos a los departamentos de Producción y Logística a analizar y revisar minuciosamente las líneas de fabricación de los siguientes productos: Galletas 750, Mantequilla 100, Mantequilla 250, Mantequilla 500, Yogur 100, Yogur 50, Ghee 100 y Ghee 250.
