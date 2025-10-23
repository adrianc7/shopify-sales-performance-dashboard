# Shopify E-Commerce Analytics Dashboard

This project presents an analytical dashboard built using Microsoft Power BI to explore e-commerce sales and customer behavior from a Shopify-based dataset. The analysis demonstrates how transactional data can be transformed into insights for evaluating business performance and digital commerce operations.

**View the interactive dashboard here:**  
[Shopify E-Commerce Analytics Dashboard (Power BI)](https://app.powerbi.com/view?r=eyJrIjoiOTE4ZTc2YzQtM2Q1OS00NWIxLWJkMDEtYjgzMmQxM2NlMjBiIiwidCI6ImFjMzUyZjliLWViNjMtNGNhMi05Y2Y5LWY0YzQwMDQ3Y2VmZiIsImMiOjZ9)

## Data Source

The dataset is an anonymized export modeled after the Shopify Admin GraphQL API schema. It represents a one-week snapshot of transactional sales data from March 18 to March 24, 2025.  
Each record corresponds to a single line item from a customer order, including information about billing address, product type, payment gateway, pricing, and tax amounts.  

The data includes:
- 7,431 line-item transactions  
- 4,431 unique customers  
- 202 distinct products  
- All transactions in USD currency  
- Geographic scope limited to the United States  

### Payment Methods

- **Shopify Payments**: Primary payment processor provided by Shopify for card transactions.  
- **PayPal**: External online payment platform.  
- **Amazon Payments**: Payment option through Amazon accounts.  
- **Gift Card**: Purchases made with issued gift balances.  
- **Manual**: Offline or alternative transactions entered manually (e.g., cash, bank transfer).

## Metrics and Definitions

| Metric | Description |
|--------|--------------|
| Net Sales | Total revenue excluding taxes and discounts. |
| Total Quantity | Number of individual items sold during the period. |
| Average Order Value (AOV) | Net sales divided by the total number of orders, measuring average spend per transaction. |
| Total Customers | Number of unique customers who placed orders. |
| Single Order Customers | Customers who made only one purchase in the dataset period. |
| Repeat Customers | Customers with more than one order, used to calculate retention. |
| Repeat Rate | Percentage of customers who made more than one purchase (Repeat ÷ Total Customers). |
| Lifetime Value (LTV) | Estimated total value per customer across purchases. |
| Purchase Frequency | Average number of purchases per customer (Total Orders ÷ Total Customers). |
| Total Tax | Combined tax revenue from all transactions. |

## Summary of Results

- **Sales period:** March 18–24, 2025  
- **Net sales:** \$4,180,874  
- **Total quantity sold:** 7,534 units  
- **Average order value:** \$562.60  
- **Repeat rate:** 46%  
- **Customer lifetime value:** \$943.60  
- **Purchase frequency:** 1.68  

Net sales gradually increased across the week, with the highest revenue recorded on March 24. The sales distribution shows steady daily activity and consistent consumer demand.  
Running and tennis shoes generated the largest share of total sales, while accessories, sandals, and jackets contributed smaller amounts.  
Transactions were concentrated in major cities such as Washington D.C., Houston, and New York City.

Payment distribution was led by Shopify Payments, followed by PayPal and Amazon Payments, with smaller proportions from gift cards and manual entries. The inclusion of multiple payment gateways indicates diverse customer preferences and flexibility in transaction handling.

## Dashboard Overview

### Page 1 – Shopify Analysis
- High-level KPIs summarizing sales and customer metrics.  
- Visualizations for sales by day, hour, product type, state, and city.  
- Filters for payment method and state to enable segmented analysis.  

### Page 2 – Customer Sales Details
- Detailed transaction table showing each customer’s purchases with corresponding product type, payment gateway, and price breakdown.  
- Aggregated totals:  
  - Net Sales: \$4,180,874  
  - Total Tax: \$418,087.35  
  - Total Price (including tax): \$4,598,960.87  

## Tools and Methods

- Power BI: Data modeling, measure creation, and dashboard design.  
- Excel: Initial data review and integrity checks.  
- Python (optional): Data extraction from Shopify Admin GraphQL API for reproducibility.  

## File Structure

/data/Shopify_Sales.xlsx              Raw dataset  
/reports/Shopify_Sales_Report.pdf     Exported dashboard  
/README.md                            Project documentation  



## Key Insights

Repeat customers accounted for nearly half of all transactions, demonstrating moderate retention and engagement.  
Sales volume was balanced across multiple product types and payment options, illustrating a diversified e-commerce portfolio.
