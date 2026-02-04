📊 E-commerce Sales Analysis Dashboard (Power BI)
An interactive Power BI dashboard designed to analyze e-commerce performance by connecting transaction details with customer geography. This project transforms raw CSV data into a star-schema model to deliver insights on profitability, payment preferences, and regional trends.

📋 Table of Contents
Overview
Data Sources
Key Features
Technical Implementation
Insights Delivered
Technologies Used

🎯 Overview
This project involves building a comprehensive E-commerce Sales Dashboard that focuses on profitability analysis and customer distribution. By linking order details with geographic data, the dashboard allows stakeholders to identify high-margin products and optimize logistics based on regional demand.

📂 Data Sources
The project utilizes two specific datasets:

Details.csv: Contains transaction-level specifics.

Order ID, Amount, Profit, Quantity, Category, Sub-Category, PaymentMode (COD, UPI, Credit Card, EMI).

Orders.csv: Contains customer and temporal data.

Order ID, Order Date, CustomerName, State, City.

✨ Key Features
Profitability Tracking: Monitor total profit and profit margins across different categories.

Payment Mode Analysis: Visualization of customer preferences (e.g., high usage of COD vs. UPI).

Geographic Mapping: Drill down into sales performance by Indian States and Cities.

Category Deep-dives: Comparative analysis of Clothing, Electronics, and Furniture.

🛠️ Technical Implementation
Data Modeling
Relationship: Established a One-to-Many (1:N) relationship between Orders.csv and Details.csv using the Order ID column.

Star Schema: Treated Orders as the lookup table (Dimension) and Details as the fact table.

DAX Measures
Custom calculations created to drive the visuals:

Code snippet
Total Sales = SUM(Details[Amount])

Total Profit = SUM(Details[Profit])

Total Quantity = SUM(Details[Quantity])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Avg Order Value = DIVIDE([Total Sales], DISTINCTCOUNT(Details[Order ID]))
Data Transformation (Power Query)
Converted Order Date into a proper Date format.

Cleaned null values in Sub-Category.

Created a "Profit Status" column to highlight orders with negative margins.

💡 Insights Delivered
High-Volume Categories: Clothing (specifically Saree and Handkerchiefs) drives the highest order frequency.

Regional Leaders: Maharashtra and Madhya Pradesh emerge as top-performing states.

Profit Leakage: Identified specific sub-categories where the Profit column shows negative values, signaling high return rates or pricing issues.

Payment Trends: A significant portion of transactions relies on COD and UPI, informing cash-flow management.

🔧 Technologies Used
Power BI Desktop: Data modeling and visualization.

Power Query: ETL (Extract, Transform, Load) processes.

DAX (Data Analysis Expressions): Complex calculated measures.

GitHub: Version control and documentation.
