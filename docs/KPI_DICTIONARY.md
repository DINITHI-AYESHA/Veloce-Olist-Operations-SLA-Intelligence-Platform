# KPI & Metric Dictionary: Veloce Platform

| Metric Name | Business Definition | Mathematical Calculation / Logic | Power BI Target Location |
|---|---|---|---|
| **Gross Merchandise Value (GMV)** | Total sales value of all completed transactions | SUM(olist_order_items[price]) where order_status = "delivered" | Page 1 (Sales Overview) |
| **Order Volume** | Total distinct orders processed | DISTINCTCOUNT(olist_orders[order_id]) | Page 1 (Sales Overview) |
| **Average Order Value (AOV)** | Average spend per distinct order | GMV / Total Delivered Orders | Page 1 (Sales Overview) |
| **Carrier SLA Breach Rate (%)** | Share of orders arriving after estimated date | (Orders where delivered_customer_date > estimated_delivery_date) / Total Delivered Orders * 100 | Page 2 (Logistics SLA) |
| **Average Delivery Delay (Days)** | Mean elapsed delay beyond SLA for late orders | AVERAGE(delivered_customer_date - estimated_delivery_date) for breach orders | Page 2 (Logistics SLA) |
| **Freight Burden Share (%)** | Proportion of total basket cost attributable to shipping | SUM(freight_value) / (SUM(price) + SUM(freight_value)) * 100 | Page 2 (Logistics SLA) |
| **Merchant Dispatch Lag (Hours)** | Time taken by seller to hand over package to carrier | AVERAGE(delivered_carrier_date - order_approved_at) in hours | Page 3 (Fulfillment Risk) |