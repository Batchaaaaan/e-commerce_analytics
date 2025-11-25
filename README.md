# E-Commerce Analytics

### Overview
This project was created as part of my submission for the **Onyx DataDNA Challenge - November 2025**, wherein I created three-pager report to analyze ecommerce sales dataset from a global software retailer.
The objective is to identify loyal customers (repeat buyers) and determine which channels and promotional campaigns drive their repeat purchases. 

### Data
The dataset was from a global software retailer that sells subscriptions and add-ons across analytics, design, collaboration, and AI.  

#### Data Dictionary
The dataset have three tables called **Events**, **Products**, and **Customers**.
- **Customer** Table list all the unique customers within the business and their infos.
  | Column              | Description                                                   |
  | ------------------- | ------------------------------------------------------------- |
  | customer_id         | Unique ID for each customer.                                  |
  | signup_date         | When the customer signed up.                                  |
  | region              | State/province/region.                                        |
  | currency_preference | Preferred currency if the customer chose one.                 |
  | segment             | Customer segment (e.g., Student, SMB, Enterprise).            |
  | acquisition_channel | How the customer first found or was acquired by the business. |
  | age_band            | Age group (e.g., 18–24).                                      |
  | currency            | Currency used for pricing on events.                          |
  | country             | Customer’s country.                                           |
  | country_latitude    | Customer’s country centroid latitude coordinates              |
  | country_longitude   | Customer’s country centroid longitude coordinates             |

- **Products** Table list all the unique products that is being sold within the business.
  | Column              | Description                                                   |
  | ------------------- | ------------------------------------------------------------- |
  | product_id          | Unique ID for each product/plan.                              |
  | product_name        | Product/plan name.                                            |
  | category            | Product category (e.g., Analytics, Collaboration).            |
  | is_subscription     | Subscription vs one-time item.                                |
  | billing_cycle       | Monthly, Annual, or One-time.                                 |
  | base_price_usd      | List price in USD before discounts/taxes.                     |
  | first_release_date  | Approximate “first availability” of the product family/plan.  |

- **Events** Table list all the events/transactions that happened over the years.
  | Column              | Description                                                   |
  | ------------------- | ------------------------------------------------------------- |
  | event_id            | Unique ID for each transaction-like record.                   |
  | event_type          | order (new sale) or invoice (renewal/billing).                |
  | event_date          | Timestamp when the event occurred.                            |
  | customer_id         | Customer on the event.                                        |
  | product_id          | Product/plan on the event.                                    |
  | country / region    | Customer location on the event.                               |
  | channel             | Sales channel (Website, Direct Sales, etc.).                  |
  | payment_method      | Payment type (Credit Card, Invoice, etc.).                    |
  | currency            | Currency used for this event.                                 |
  | fx_rate_to_usd      | Conversion rate used for USD amounts.                         |
  | quantity            | Number of seats/units.                                        |
  | unit_price_local    | Unit list price in local currency.                            |
  | discount_code       | Code applied to the event.                                    |
  | discount_local      | Discount amount in local currency.                            |
  | tax_local           | Tax/VAT in local currency.                                    |
  | net_revenue_local   | Net amount in local currency.                                 |
  | net_revenue_usd     | Net amount converted to USD.                                  |
  | is_refunded         | True/False if refunded.                                       |
  | refund_datetime     | When refund happened.                                         |
  | refund_reason       | Reason for refund.                                            |

#### Data Source
- downloaded from onyx data dataDNA [website](https://datadna.onyxdata.co.uk/challenges/november-2025-datadna-ecommerce-analytics-challenge).

### Purpose
The challenge tasked us to identify sales performance drivers across the business, opportunities, and what hurts the business. The report should answer the following guiding questions:
- How do total sales change by month?
-	Which channels bring in the most sales?
-	Which channels bring the most repeat (loyal) customers?
-	What percent of monthly sales comes from loyal customers?
-	Which products or plans sell the most?
-	Which products are most popular with loyal customers?
-	How long do customers wait before their second purchase?
-	Which discount codes are used most, and do they increase repeat purchases?
-	What is the average selling price (ASP) by country or currency?
-	Where do refunds happen most (by product or channel)?
-	Do annual plans bring higher revenue per customer than monthly plans?
-	Which add-ons are most often bought with core products (attach rate)?

### Analysis

### Reference
Refer to this [post](https://www.linkedin.com/posts/batchaaan22_datafam-datadna-datavisualization-activity-7398700528467357696-cXrF?utm_source=share&utm_medium=member_desktop&rcm=ACoAADU37-4BvZkdxoNILB6GhzRJGT7OoLWMMoY) to view my submission.
