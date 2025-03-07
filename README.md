# Retail Sales Analysis Forcast with python
## Overview
This project leverages predictive analytics to drive strategic business decisions by forecasting future sales trends and identifying high-value customers. Two models were implemented: a Logistic Regression model to predict high-spending customers and an ARIMA time series model to forecast sales for the next 12 months.

## Data Description
### Columns:
- InvoiceNo - Unique invoice identifier.
- StockCode - Product code.
- Description - Product name.
- Quantity - Number of products purchased.
- InvoiceDate - Date and time of transaction.
- UnitPrice - Price per unit.
- CustomerID - Unique customer identifier.
- Country - Customer's country.
### Identified Issues:
- 1,454 missing values in Description.
- 135,080 missing values in CustomerID.
- 10,624 negative values in Quantity.
- 2 negative values in UnitPrice.
- 2,515 zero values in UnitPrice.
- Special characters and blanks in Description.
- 5,268 duplicate rows.
- Some rows in Country labeled as 'Unspecified'.
### Data Cleaning Process
- Filled missing values in Description as "Unknown".
- Assigned unique negative CustomerID values for missing entries.
- Removed rows with negative Quantity and zero or negative UnitPrice.
- Dropped 5,268 duplicate rows.
- Standardized Country by removing 'Unspecified' entries.
### Exploratory Data Analysis (EDA)
####  Key Insights
- Top 3 Selling Products
1. Paper Craft Little Birdie (80,995 units sold).
2. Medium Ceramic Top Storage Jar (78,033 units).
3. World War 2 Gliders Asstd Designs (54,855 units).
- Top 3 Revenue-Generating Products
 1. Dotcom Postage ($206,248.77 revenue).
 2. Regency Cakestand 3 Tier ($174,131.04 revenue).
 3. Paper Craft Little Birdie ($168,469.60 revenue).
- Top 3 Total Revenue Per Country
1. United Kingdom: $9,001,855.17
2. Netherlands: $285,446.34
3. EIRE: $283,170.52
- Number of Transactions Per Country
1. United Kingdom:18,019.
2. Germany: 457.
3. France: 392.

## Dashboard and Visualizations
![Top selling products](https://github.com/user-attachments/assets/156264cd-bfad-410c-88ae-1ec2ac56eaad)
![Top revenue generating products](https://github.com/user-attachments/assets/f803ecb5-62b5-450f-8f75-e4906a20c327)
![Top countries](https://github.com/user-attachments/assets/1cd31653-4bd3-4379-bccb-854b4e9be839)
![Sales trend](https://github.com/user-attachments/assets/ef6458c1-5db6-4980-ae9c-1043f359e9bc)
![Sales forecast](https://github.com/user-attachments/assets/4c45021f-61d9-47ee-a662-46cb211b5195)

## Recommendations
- Inventory Optimization: Given the steady growth in sales, businesses should ensure sufficient stock levels to meet demand, particularly in February, which sees a slight peak.
- Pricing Strategy: UnitPrice has the highest impact on high spenders. Businesses should experiment with pricing strategies to maximize revenue without discouraging purchases.
- Geographical Expansion: The UK dominates in transactions and revenue, but potential growth opportunities exist in Germany and France.
- Targeted Promotions: Customers with high AvgSpendPerPurchase and frequent transactions should be targeted for loyalty programs and exclusive offers.
- Product Strategy: High revenue-generating products should be prioritized in marketing and inventory planning.
- Seasonal Adjustments: Peak sales months (Nov-Dec) should be leveraged with promotional campaigns to maximize revenue.
## Conclusions
This project provides actionable insights into customer behavior, sales forecasting, and revenue generation. The predictive models help businesses make data-driven decisions, optimize inventory, and enhance customer engagement.
