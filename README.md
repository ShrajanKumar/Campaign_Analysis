# Campaign_Analysis

To Interact with dashboard : https://app.powerbi.com/view?r=eyJrIjoiYTg4NWM1M2YtZTRjYS00OGExLWFmZTMtNzRkZGYzZTU2MmI5IiwidCI6IjBlNjA2MTkxLWJkMTctNDI3NC1iOWZkLTgxMDY5YTM5ZDlkMiJ9&pageName=ReportSectionf2e0683b73cf982f241a



## About Dataset :
In a database design, there are typically two primary types of tables: Dimension tables and Fact tables. Fact table : A fact table contains records that combine attributes from different dimension tables.Examples of Fact tables include recording of sales transactions, order quantities, or financial transactions.

Dimension table : It provides the context and background information for the measures recorded in the fact table.Examples of Dimension tables include tables storing region names, store addresses, or product categories.

### Terms included in the dataset .
1. dim_campaigns
2. dim_products
3. dim_stores
4. fact_events


Column Description for dim_campaigns:
- campaign_id: Unique identifier for each promotional campaign.
- campaign_name: Descriptive name of the campaign (e.g., Diwali, Sankranti).
- start_date: The date on which the campaign begins, formatted as DD-MM-YYYY.
- end_date: The date on which the campaign ends, formatted as DD-MM-YYYY.


*******************************************


Column Description for dim_products:
- product_code: Unique code assigned to each product for identification.
- product_name: The full name of the product, including brand and specifics (e.g., quantity, size).
- category: The classification of the product into broader categories such as Grocery & Staples, Home Care, Personal Care, Home Appliances, etc.


*******************************************



Column Description for dim_stores:
- store_id: Unique code identifying each store location.
- city: The city where the store is located, indicating the geographical market.


*******************************************



Column Description for fact_events:
- event_id: Unique identifier for each sales event.
- store_id: Refers to the store where the event took place, linked to the dim_stores table.
- campaign_id: Indicates the campaign under which the event was recorded, linked to the dim_campaigns table.
- product_code: The code of the product involved in the sales event, linked to the dim_products table.
- base_price: The standard price of the product before any promotional discount.
- promo_type: The type of promotion applied (e.g., percentage discount, BOGOF(Buy One Get One Free), cashback).
- quantity_sold(before_promo): The number of units sold in the week immediately preceding the start of the campaign, serving as a baseline for comparison with promotional sales.
- quantity_sold(after_promo): The quantity of the product sold after the promotion was applied.


*******************************************
