# Proyecto de análisis de datos📊
## ➡️Problema en cadena logística en bienes de consumo rápido
_industria: alimentos, lácteos_

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

💻 Si desea ver el análisis a profundidad desarrollado en python [click aquí](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/blob/main/SupplyChain_Challengue.ipynb)

📚 puede ver el dashboard hecho en PowerBI [click aquí](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/blob/main/dashboard.pbix)

📊 presentación de evidencias en vivo [youtube](https://youtube.com)

![dashb1](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/9a9ecc61-7c30-41e1-b7cc-609ef8845b9a)
![dashb2](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/c2a0db05-3799-432d-b0a3-c3227d9e5930)
![dashb3](https://github.com/PyAngel/Supply-chain-issue-in-the-FMCG-domain/assets/127798134/d96ca1c5-7116-48fd-b808-818a7ab63b1c)

 ## HALLAZGOS:

1. Después de analizar nuestros indicadores clave de rendimiento (KPIs), hemos encontrado que nuestra cadena logística necesita aumentar esfuerzos y asignar recursos para optimizar los envíos en un 50% adicional más allá del nivel actual, especialmente para garantizar entregas completas y a tiempo. Hemos observado que nuestro indicador de OTIF solo alcanza aproximadamente un ≈49% de la meta esperada, lo que resulta en que solo aproximadamente un ≈30% de nuestras entregas cumplan con el estándar mínimo de efectividad.

2. Al observar los KPIs por cliente, notamos que los clientes con pedidos de alto volumen (>1000 ordenes) se han visto afectados negativamente en cuanto al tiempo o la cantidad completa de sus pedidos (OTIF%). Sin embargo, esta métrica es general, y para ver la diferencia a lo largo de un período más largo, es necesario examinar toda la cadena de suministro dentro del marco de tiempo.

3. Para garantizar la precisión, revisemos los códigos de cliente paso a paso y comparemos las métricas para cada usuario. Nos ha llamado la atención que las siguientes cuentas: 789122, 789420, 789522, 789421, 789422, 789520, 789601 y 789903, estas están experimentando problemas graves con la entrega, específicamente retrasos y envíos incompletos. Estos problemas han persistido durante un período de tiempo significativo, lo que indica desafíos consistentes en la cadena de suministro. Del mismo modo, las cuentas 789121, 789521, 789603, 789702, 789621, 789503, 789103 y 789501 enfrentan desafíos con entregas incompletas, que están afectando negativamente nuestro indicador clave de rendimiento (KPI) y las relaciones contractuales con los clientes.

4. Tras revisar los últimos gráficos, hemos llegado a la conclusión de que nos falta evidencia cuantitativa para determinar si nuestro problema radica en la cantidad total de los pedidos. Actualmente, todos nuestros productos se encuentran en aproximadamente un 60% - 70% del LIFR% (Tasa de Relleno de Inventario en el Plazo de Entrega), pero todos nuestros pedidos ya han alcanzado un 95% en VOFR%. Además, este porcentaje se ha mantenido estable durante un largo período de tiempo. Por lo tanto, podemos concluir que nuestro problema radica en la cadena de suministro, específicamente en la preparación y el envío de productos al cliente final.

En este punto, es crucial evaluar si nuestros KPIs están directamente correlacionados con productos específicos.


## CONCLUSIONES:

Tras analizar el rendimiento de cada producto, hemos determinado que la ciudad de Surat enfrenta desafíos significativos en su cadena de suministro con respecto a los pedidos completados, con una alarmante tasa de error del 90% en todas las gamas de productos. Los gráficos y diagramas de caja revelan dos problemas principales.

1. Alta Volatilidad: Los diagramas de caja para la ciudad de Surat muestran un amplio rango, lo que indica inestabilidad en nuestra cadena de suministro de productos. Esto está afectando negativamente a nuestros clientes, especialmente en términos económicos. el rango de desempeño ya tiene un problema del 40% en la tasa de LIFR%.

2. La ciudad de Vadodara también está experimentando problemas con pedidos incompletos en productos específicos tales como Mantequilla 500, Yogur 100, Ghee 100 y Ghee 250.

3. Nuestros productos Leche 100, Leche 250 y Leche 500, han enfrentado problemas de entrega y producción en todas las ciudades.

A la luz de estos hallazgos, instamos a los departamentos de Producción y Logística a analizar y revisar minuciosamente las líneas de fabricación de los siguientes productos: Galletas 750, Mantequilla 100, Mantequilla 250, Mantequilla 500, Yogur 100, Yogur 50, Ghee 100 y Ghee 250.
Es importante validar si la capacidad instalada en plantas de producción están a la orden de sostener el flujo de pedidos de nuestros principales clientes, de no ser así, es necesario evaluar alternativas de fabricación por terceros de forma temporal.
